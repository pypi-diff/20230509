# Comparing `tmp/cvxsimulator-0.2.2.tar.gz` & `tmp/cvxsimulator-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.2.2.tar", max compression
+gzip compressed data, was "cvxsimulator-0.2.3.tar", max compression
```

## Comparing `cvxsimulator-0.2.2.tar` & `cvxsimulator-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1102 2023-05-09 06:24:57.711927 cvxsimulator-0.2.2/LICENSE
--rw-r--r--   0        0        0     4050 2023-05-09 06:24:57.711927 cvxsimulator-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-05-09 06:24:57.739927 cvxsimulator-0.2.2/cvx/simulator/__init__.py
--rw-r--r--   0        0        0     1163 2023-05-09 06:24:57.739927 cvxsimulator-0.2.2/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     1409 2023-05-09 06:24:57.739927 cvxsimulator-0.2.2/cvx/simulator/month.py
--rw-r--r--   0        0        0     6143 2023-05-09 06:24:57.739927 cvxsimulator-0.2.2/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      464 2023-05-09 06:24:57.739927 cvxsimulator-0.2.2/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      596 2023-05-09 06:25:53.088667 cvxsimulator-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 cvxsimulator-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-05-09 06:58:46.820700 cvxsimulator-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4050 2023-05-09 06:58:46.820700 cvxsimulator-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 06:58:46.848700 cvxsimulator-0.2.3/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-09 06:58:46.848700 cvxsimulator-0.2.3/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     1341 2023-05-09 06:58:46.848700 cvxsimulator-0.2.3/cvx/simulator/month.py
+-rw-r--r--   0        0        0     6225 2023-05-09 06:58:46.848700 cvxsimulator-0.2.3/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      464 2023-05-09 06:58:46.848700 cvxsimulator-0.2.3/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      596 2023-05-09 06:59:34.361648 cvxsimulator-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 cvxsimulator-0.2.3/PKG-INFO
```

### Comparing `cvxsimulator-0.2.2/LICENSE` & `cvxsimulator-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.2.2/README.md` & `cvxsimulator-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.2.2/cvx/simulator/metrics.py` & `cvxsimulator-0.2.3/cvx/simulator/metrics.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.2.2/cvx/simulator/month.py` & `cvxsimulator-0.2.3/cvx/simulator/month.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # -*- coding: utf-8 -*-
 """
 Popular year vs month performance table.
-
-Supports compounded and cumulative (i.e. fixed AUM) returns logic.
 """
 from __future__ import annotations
 
 import calendar
 
 import numpy as np
 import pandas as pd
```

### Comparing `cvxsimulator-0.2.2/cvx/simulator/portfolio.py` & `cvxsimulator-0.2.3/cvx/simulator/portfolio.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,18 @@
         previous_stocks = self.stocks.shift(1).fillna(0.0)
         return (previous_stocks * price_changes).dropna(axis=0, how="all").sum(axis=1)
 
     def __mul__(self, scalar):
         """
         Multiplies positions by a scalar
         """
-        return _EquityPortfolio(prices=self.prices, stocks=self.stocks * scalar, initial_cash=self.initial_cash * scalar, model=self.trading_cost_model)
+        return _EquityPortfolio(prices=self.prices, stocks=self.stocks * scalar, initial_cash=self.initial_cash * scalar, trading_cost_model=self.trading_cost_model)
+
+    def __rmul__(self, scalar):
+        return self.__mul__(scalar)
 
     def __add__(self, port_new):
         """
         Adds two portfolios together
         """
         assert isinstance(port_new, _EquityPortfolio)
```

### Comparing `cvxsimulator-0.2.2/pyproject.toml` & `cvxsimulator-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.2.2"
+version = "v0.2.3"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxsimulator-0.2.2/PKG-INFO` & `cvxsimulator-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

