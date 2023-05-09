# Comparing `tmp/cvxsimulator-0.2.1.tar.gz` & `tmp/cvxsimulator-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.2.1.tar", max compression
+gzip compressed data, was "cvxsimulator-0.2.2.tar", max compression
```

## Comparing `cvxsimulator-0.2.1.tar` & `cvxsimulator-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1102 2023-05-08 20:13:39.782319 cvxsimulator-0.2.1/LICENSE
--rw-r--r--   0        0        0     4050 2023-05-08 20:13:39.782319 cvxsimulator-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-05-08 20:13:39.810319 cvxsimulator-0.2.1/cvx/simulator/__init__.py
--rw-r--r--   0        0        0     1163 2023-05-08 20:13:39.810319 cvxsimulator-0.2.1/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     1409 2023-05-08 20:13:39.810319 cvxsimulator-0.2.1/cvx/simulator/month.py
--rw-r--r--   0        0        0     5814 2023-05-08 20:13:39.810319 cvxsimulator-0.2.1/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      464 2023-05-08 20:13:39.810319 cvxsimulator-0.2.1/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      596 2023-05-08 20:14:34.870395 cvxsimulator-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 cvxsimulator-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-05-09 06:24:57.711927 cvxsimulator-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4050 2023-05-09 06:24:57.711927 cvxsimulator-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 06:24:57.739927 cvxsimulator-0.2.2/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-09 06:24:57.739927 cvxsimulator-0.2.2/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     1409 2023-05-09 06:24:57.739927 cvxsimulator-0.2.2/cvx/simulator/month.py
+-rw-r--r--   0        0        0     6143 2023-05-09 06:24:57.739927 cvxsimulator-0.2.2/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      464 2023-05-09 06:24:57.739927 cvxsimulator-0.2.2/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      596 2023-05-09 06:25:53.088667 cvxsimulator-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 cvxsimulator-0.2.2/PKG-INFO
```

### Comparing `cvxsimulator-0.2.1/LICENSE` & `cvxsimulator-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.2.1/README.md` & `cvxsimulator-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.2.1/cvx/simulator/metrics.py` & `cvxsimulator-0.2.2/cvx/simulator/metrics.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.2.1/cvx/simulator/month.py` & `cvxsimulator-0.2.2/cvx/simulator/month.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.2.1/cvx/simulator/portfolio.py` & `cvxsimulator-0.2.2/cvx/simulator/portfolio.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,17 +35,22 @@
             self.cash -= model.eval(self.prices,  trades=trades, **kwargs).sum()
 
         return self
 
 
 def build_portfolio(prices, stocks=None, initial_cash=1e6, trading_cost_model=None):
     assert isinstance(prices, pd.DataFrame)
+    assert prices.index.is_monotonic_increasing
+    assert prices.index.is_unique
 
     if stocks is None:
         stocks = pd.DataFrame(index=prices.index, columns=prices.columns, data=0.0, dtype=float)
+    else:
+        assert stocks.index.is_monotonic_increasing
+        assert stocks.index.is_unique
 
     assert set(stocks.index).issubset(set(prices.index))
     assert set(stocks.columns).issubset(set(prices.columns))
 
     prices = prices[stocks.columns].loc[stocks.index]
 
     trading_cost_model = trading_cost_model or LinearCostModel(name="LinearCostModel cost model")
@@ -155,15 +160,15 @@
         previous_stocks = self.stocks.shift(1).fillna(0.0)
         return (previous_stocks * price_changes).dropna(axis=0, how="all").sum(axis=1)
 
     def __mul__(self, scalar):
         """
         Multiplies positions by a scalar
         """
-        return _EquityPortfolio(prices=self.prices, stocks=self.stocks * scalar)
+        return _EquityPortfolio(prices=self.prices, stocks=self.stocks * scalar, initial_cash=self.initial_cash * scalar, model=self.trading_cost_model)
 
     def __add__(self, port_new):
         """
         Adds two portfolios together
         """
         assert isinstance(port_new, _EquityPortfolio)
 
@@ -183,8 +188,9 @@
 
         prices_left = self.prices.combine_first(port_new.prices)
         prices_right = port_new.prices.combine_first(self.prices)
 
         pd.testing.assert_frame_equal(prices_left, prices_right)
 
         return build_portfolio(prices=prices_right, stocks=positions,
-                               initial_cash=self.initial_cash + port_new.initial_cash)
+                               initial_cash=self.initial_cash + port_new.initial_cash,
+                               trading_cost_model=self.trading_cost_model)
```

### Comparing `cvxsimulator-0.2.1/pyproject.toml` & `cvxsimulator-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.2.1"
+version = "v0.2.2"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxsimulator-0.2.1/PKG-INFO` & `cvxsimulator-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

