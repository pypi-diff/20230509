# Comparing `tmp/emgregs-0.0.4.dev0.tar.gz` & `tmp/emgregs-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emgregs-0.0.4.dev0.tar", max compression
+gzip compressed data, was "emgregs-0.0.5.tar", max compression
```

## Comparing `emgregs-0.0.4.dev0.tar` & `emgregs-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-02-28 09:33:19.384647 emgregs-0.0.4.dev0/LICENSE
--rw-r--r--   0        0        0      206 2023-02-28 10:04:12.806983 emgregs-0.0.4.dev0/emgregs/__init__.py
--rw-r--r--   0        0        0    11268 2023-02-28 09:38:15.991593 emgregs-0.0.4.dev0/emgregs/emg_reg.py
--rw-r--r--   0        0        0     7921 2023-02-28 09:33:19.384647 emgregs-0.0.4.dev0/emgregs/flare_reg.py
--rw-r--r--   0        0        0     4802 2023-02-28 09:33:19.384647 emgregs-0.0.4.dev0/emgregs/simulation.py
--rw-r--r--   0        0        0      563 2023-02-28 10:04:50.654414 emgregs-0.0.4.dev0/pyproject.toml
--rw-r--r--   0        0        0      761 2023-02-28 10:05:55.705272 emgregs-0.0.4.dev0/setup.py
--rw-r--r--   0        0        0      630 2023-02-28 10:05:55.705460 emgregs-0.0.4.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-09 09:31:46.018734 emgregs-0.0.5/LICENSE
+-rw-r--r--   0        0        0      201 2023-05-09 09:35:38.134557 emgregs-0.0.5/emgregs/__init__.py
+-rw-r--r--   0        0        0    11320 2023-05-09 09:32:38.834251 emgregs-0.0.5/emgregs/emg_reg.py
+-rw-r--r--   0        0        0     7933 2023-05-09 09:28:55.480384 emgregs-0.0.5/emgregs/flare_reg.py
+-rw-r--r--   0        0        0     4802 2023-05-09 09:31:46.018734 emgregs-0.0.5/emgregs/simulation.py
+-rw-r--r--   0        0        0      558 2023-05-09 09:35:38.134557 emgregs-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      756 2023-05-09 09:35:55.372085 emgregs-0.0.5/setup.py
+-rw-r--r--   0        0        0      625 2023-05-09 09:35:55.372276 emgregs-0.0.5/PKG-INFO
```

### Comparing `emgregs-0.0.4.dev0/LICENSE` & `emgregs-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `emgregs-0.0.4.dev0/emgregs/emg_reg.py` & `emgregs-0.0.5/emgregs/emg_reg.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,14 +332,18 @@
     y: npt.ArrayLike,
     intercept: Optional[bool] = False,
     beta: Optional[npt.ArrayLike] = None,
     sigma: Optional[float] = None,
     alpha: Optional[float] = None,
     **kwargs,
 ):
+    
+    x = numpy.array(x)
+    y = numpy.array(y)
+
     if not intercept:
         try:
             x = numpy.concatenate((numpy.ones((x.shape[0], 1)), x), axis=1)
         except ValueError:
             x = numpy.concatenate((numpy.ones((x.shape[0], 1)), x.reshape(-1, 1)), axis=1)
 
     k_passed = kwargs.pop("k", None)
```

### Comparing `emgregs-0.0.4.dev0/emgregs/flare_reg.py` & `emgregs-0.0.5/emgregs/flare_reg.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,31 +69,31 @@
     return (x.T * z).T
 
 
 def apply_column_sum(x):
     return numpy.sum(x, axis=0)
 
 
-def try_flare_ref(
+def _flare_reg(
     y,
     x,
     k=None,
     beta=None,
     sigma=None,
     alpha=None,
     emg=1,
     epsilon=1e-4,
     maxit=1e4,
     verb=False,
     restart=50,
 ):
 
     # Preamble
-
     x = numpy.concatenate((numpy.ones((x.shape[0], 1)), x), axis=1)
+    
     n = len(y)
     p = x.shape[1]
 
     if k is None:
         kmean_fit = KMeans(n_clusters=2, random_state=None, init="k-means++").fit(
             y.reshape(-1, 1)
         )
@@ -260,22 +260,22 @@
     emg: Optional[bool] = True,
     epsilon: Optional[float] = 1e-4,
     maxit: Optional[int] = 1e4,
     verb: Optional[bool] = False,
     restart: Optional[int] = 50,
 ):
 
-    x = numpy.atleast_2d(numpy.array(x))
+    x = numpy.atleast_2d(numpy.array(x)).reshape(-1,1)
 
     if intercept:
         x = x[..., 1:]
 
     y = numpy.array(y).reshape((-1,))
 
-    return try_flare_ref(
+    return _flare_reg(
         y=y,
         x=x,
         k=k,
         beta=beta,
         sigma=sigma,
         alpha=alpha,
         emg=emg,
```

### Comparing `emgregs-0.0.4.dev0/emgregs/simulation.py` & `emgregs-0.0.5/emgregs/simulation.py`

 * *Files identical despite different names*

### Comparing `emgregs-0.0.4.dev0/pyproject.toml` & `emgregs-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emgregs"
-version = "0.0.4-dev0"
+version = "0.0.5"
 description = "Python port to Yanxi Li's R emg flare code"
 authors = ["jgori <juliengori@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 numpy = "^1.22.3"
 scipy = "^1.8.0"
```

### Comparing `emgregs-0.0.4.dev0/setup.py` & `emgregs-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'scikit-learn>=1.0.2,<2.0.0',
  'scipy>=1.8.0,<2.0.0',
  'statsmodels>=0.13.2,<0.14.0',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'emgregs',
-    'version': '0.0.4.dev0',
+    'version': '0.0.5',
     'description': "Python port to Yanxi Li's R emg flare code",
     'long_description': None,
     'author': 'jgori',
     'author_email': 'juliengori@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `emgregs-0.0.4.dev0/PKG-INFO` & `emgregs-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emgregs
-Version: 0.0.4.dev0
+Version: 0.0.5
 Summary: Python port to Yanxi Li's R emg flare code
 Author: jgori
 Author-email: juliengori@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```

