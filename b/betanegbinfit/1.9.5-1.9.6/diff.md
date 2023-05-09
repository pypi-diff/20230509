# Comparing `tmp/betanegbinfit-1.9.5.tar.gz` & `tmp/betanegbinfit-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betanegbinfit-1.9.5.tar", last modified: Sun May  7 16:02:31 2023, max compression
+gzip compressed data, was "betanegbinfit-1.9.6.tar", last modified: Tue May  9 16:39:15 2023, max compression
```

## Comparing `betanegbinfit-1.9.5.tar` & `betanegbinfit-1.9.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-07 16:02:31.053848 betanegbinfit-1.9.5/
--rw-r--r--   0 georgy    (1000) georgy    (1001)     4054 2023-05-07 16:02:31.053848 betanegbinfit-1.9.5/PKG-INFO
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3534 2022-01-12 15:51:26.000000 betanegbinfit-1.9.5/README.md
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-07 16:02:31.050515 betanegbinfit-1.9.5/betanegbinfit/
--rw-r--r--   0 georgy    (1000) georgy    (1001)      725 2023-05-07 16:01:20.000000 betanegbinfit-1.9.5/betanegbinfit/__init__.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14720 2023-04-24 17:33:25.000000 betanegbinfit-1.9.5/betanegbinfit/betacdnb.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     2534 2023-04-24 17:33:25.000000 betanegbinfit-1.9.5/betanegbinfit/betainc.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     5146 2023-04-24 17:33:25.000000 betanegbinfit-1.9.5/betanegbinfit/bridge_mixalime.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     6400 2023-05-07 16:00:30.000000 betanegbinfit-1.9.5/betanegbinfit/cdnb.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     5148 2023-04-24 17:33:25.000000 betanegbinfit-1.9.5/betanegbinfit/combine.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14940 2023-04-24 17:33:25.000000 betanegbinfit-1.9.5/betanegbinfit/create.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    38510 2023-05-07 14:53:13.000000 betanegbinfit-1.9.5/betanegbinfit/distributions.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3125 2023-04-24 17:33:25.000000 betanegbinfit-1.9.5/betanegbinfit/hyp.py
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-07 16:02:31.053848 betanegbinfit-1.9.5/betanegbinfit/models/
--rw-r--r--   0 georgy    (1000) georgy    (1001)      258 2023-04-24 17:33:25.000000 betanegbinfit-1.9.5/betanegbinfit/models/__init__.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    15251 2023-04-24 17:33:25.000000 betanegbinfit-1.9.5/betanegbinfit/models/model.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    22116 2023-04-24 17:33:25.000000 betanegbinfit-1.9.5/betanegbinfit/models/model_line.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3341 2023-04-24 17:33:25.000000 betanegbinfit-1.9.5/betanegbinfit/models/model_line_lrt.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14364 2023-04-24 17:33:25.000000 betanegbinfit-1.9.5/betanegbinfit/models/model_mixture.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     8477 2023-04-24 17:33:25.000000 betanegbinfit-1.9.5/betanegbinfit/models/model_mixtures.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    29845 2023-04-24 17:33:25.000000 betanegbinfit-1.9.5/betanegbinfit/models/model_window.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    13557 2023-04-24 17:33:25.000000 betanegbinfit-1.9.5/betanegbinfit/plot.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14689 2023-04-24 17:33:25.000000 betanegbinfit-1.9.5/betanegbinfit/stats.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     6960 2023-04-24 17:33:25.000000 betanegbinfit-1.9.5/betanegbinfit/tests.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    29604 2023-04-24 17:33:25.000000 betanegbinfit-1.9.5/betanegbinfit/utils.py
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-07 16:02:31.050515 betanegbinfit-1.9.5/betanegbinfit.egg-info/
--rw-r--r--   0 georgy    (1000) georgy    (1001)     4054 2023-05-07 16:02:31.000000 betanegbinfit-1.9.5/betanegbinfit.egg-info/PKG-INFO
--rw-r--r--   0 georgy    (1000) georgy    (1001)      777 2023-05-07 16:02:31.000000 betanegbinfit-1.9.5/betanegbinfit.egg-info/SOURCES.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)        1 2023-05-07 16:02:31.000000 betanegbinfit-1.9.5/betanegbinfit.egg-info/dependency_links.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       43 2023-05-07 16:02:31.000000 betanegbinfit-1.9.5/betanegbinfit.egg-info/requires.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       14 2023-05-07 16:02:31.000000 betanegbinfit-1.9.5/betanegbinfit.egg-info/top_level.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       38 2023-05-07 16:02:31.053848 betanegbinfit-1.9.5/setup.cfg
--rw-r--r--   0 georgy    (1000) georgy    (1001)      963 2023-04-16 06:18:26.000000 betanegbinfit-1.9.5/setup.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-09 16:39:15.612772 betanegbinfit-1.9.6/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     4108 2023-05-09 16:39:15.612772 betanegbinfit-1.9.6/PKG-INFO
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3534 2022-01-12 15:51:26.000000 betanegbinfit-1.9.6/README.md
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-09 16:39:15.612772 betanegbinfit-1.9.6/betanegbinfit/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      725 2023-05-09 16:38:06.000000 betanegbinfit-1.9.6/betanegbinfit/__init__.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14720 2023-04-24 17:33:25.000000 betanegbinfit-1.9.6/betanegbinfit/betacdnb.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     2534 2023-04-24 17:33:25.000000 betanegbinfit-1.9.6/betanegbinfit/betainc.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     5146 2023-04-24 17:33:25.000000 betanegbinfit-1.9.6/betanegbinfit/bridge_mixalime.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     6400 2023-05-07 16:00:30.000000 betanegbinfit-1.9.6/betanegbinfit/cdnb.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     5148 2023-04-24 17:33:25.000000 betanegbinfit-1.9.6/betanegbinfit/combine.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14940 2023-04-24 17:33:25.000000 betanegbinfit-1.9.6/betanegbinfit/create.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    38510 2023-05-07 14:53:13.000000 betanegbinfit-1.9.6/betanegbinfit/distributions.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3125 2023-05-09 16:38:00.000000 betanegbinfit-1.9.6/betanegbinfit/hyp.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-09 16:39:15.612772 betanegbinfit-1.9.6/betanegbinfit/models/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      258 2023-04-24 17:33:25.000000 betanegbinfit-1.9.6/betanegbinfit/models/__init__.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    15251 2023-04-24 17:33:25.000000 betanegbinfit-1.9.6/betanegbinfit/models/model.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    22116 2023-04-24 17:33:25.000000 betanegbinfit-1.9.6/betanegbinfit/models/model_line.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3341 2023-04-24 17:33:25.000000 betanegbinfit-1.9.6/betanegbinfit/models/model_line_lrt.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14364 2023-04-24 17:33:25.000000 betanegbinfit-1.9.6/betanegbinfit/models/model_mixture.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     8477 2023-04-24 17:33:25.000000 betanegbinfit-1.9.6/betanegbinfit/models/model_mixtures.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    29845 2023-04-24 17:33:25.000000 betanegbinfit-1.9.6/betanegbinfit/models/model_window.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    13557 2023-04-24 17:33:25.000000 betanegbinfit-1.9.6/betanegbinfit/plot.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14689 2023-04-24 17:33:25.000000 betanegbinfit-1.9.6/betanegbinfit/stats.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     6960 2023-04-24 17:33:25.000000 betanegbinfit-1.9.6/betanegbinfit/tests.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    29604 2023-04-24 17:33:25.000000 betanegbinfit-1.9.6/betanegbinfit/utils.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-09 16:39:15.612772 betanegbinfit-1.9.6/betanegbinfit.egg-info/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     4108 2023-05-09 16:39:15.000000 betanegbinfit-1.9.6/betanegbinfit.egg-info/PKG-INFO
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      777 2023-05-09 16:39:15.000000 betanegbinfit-1.9.6/betanegbinfit.egg-info/SOURCES.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)        1 2023-05-09 16:39:15.000000 betanegbinfit-1.9.6/betanegbinfit.egg-info/dependency_links.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       43 2023-05-09 16:39:15.000000 betanegbinfit-1.9.6/betanegbinfit.egg-info/requires.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       14 2023-05-09 16:39:15.000000 betanegbinfit-1.9.6/betanegbinfit.egg-info/top_level.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       38 2023-05-09 16:39:15.612772 betanegbinfit-1.9.6/setup.cfg
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      963 2023-04-16 06:18:26.000000 betanegbinfit-1.9.6/setup.py
```

### Comparing `betanegbinfit-1.9.5/PKG-INFO` & `betanegbinfit-1.9.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 Metadata-Version: 2.1
 Name: betanegbinfit
-Version: 1.9.5
+Version: 1.9.6
+Summary: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
@@ -72,7 +75,9 @@
 
 
 **Please note, that all functions have plenty of optional arguments and they all are documented, so please consider reading through `help(function of interest)`.**
 
 
 ### A note on performance
 As far as we are concerned, **BetaNegBinFit** should work within a manageable amounts of time. For insance, when `ModelLine` with `model='BetaNB'` ran against *chipseq.tsv* dataset, it finishes in 6 minutes when ran at Ryzen 5600U. It does so under 2 minutes with `model='NB'`.
+
+
```

### Comparing `betanegbinfit-1.9.5/README.md` & `betanegbinfit-1.9.6/README.md`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.5/betanegbinfit/__init__.py` & `betanegbinfit-1.9.6/betanegbinfit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.9.5'
+__version__ = '1.9.6'
 
 import warnings
 # This will omit annoying FutureWarnings by JAX and RutimeWarnings caused by
 # estimates being clipped at bounds.
 warnings.simplefilter(action='ignore', category=FutureWarning)
 warnings.simplefilter(action='ignore', category=RuntimeWarning)
```

### Comparing `betanegbinfit-1.9.5/betanegbinfit/betacdnb.py` & `betanegbinfit-1.9.6/betanegbinfit/betacdnb.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.5/betanegbinfit/betainc.py` & `betanegbinfit-1.9.6/betanegbinfit/betainc.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.5/betanegbinfit/bridge_mixalime.py` & `betanegbinfit-1.9.6/betanegbinfit/bridge_mixalime.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.5/betanegbinfit/cdnb.py` & `betanegbinfit-1.9.6/betanegbinfit/cdnb.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.5/betanegbinfit/combine.py` & `betanegbinfit-1.9.6/betanegbinfit/combine.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.5/betanegbinfit/create.py` & `betanegbinfit-1.9.6/betanegbinfit/create.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.5/betanegbinfit/distributions.py` & `betanegbinfit-1.9.6/betanegbinfit/distributions.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.5/betanegbinfit/hyp.py` & `betanegbinfit-1.9.6/betanegbinfit/hyp.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     return ((3 * n + b1 + 1) * (3 * n + b2 + 1) - (2 * n + a1 + 1) * (2 * n + a2 + 1)) / ((2 * n + 1) * (2 * n + a2 + 1))
 
 def _calc_q(a1, a2, b1, b2, n):
     i = n % 3 + 3 * (n == 0)
     return switch(i, [__calc_q0, __calc_q1, __calc_q2, __calc_one], a1, a2, b1, b2, n // 3)
 
 
-def hyp3f2(a1, a2, b1, b2, n=10, eps=1e-1, tiny=1e-100):
+def hyp3f2(a1, a2, b1, b2, n=20, eps=1e-1, tiny=1e-100):
     def lentz_iteration(prev):
         res, params, c, d, i = prev
         rn = _calc_r(*params, i)
         qn = _calc_q(*params, i)
         c = qn + rn / c
         t = qn + rn * d
         c = jnp.where(c == 0, tiny, c)
```

### Comparing `betanegbinfit-1.9.5/betanegbinfit/models/model.py` & `betanegbinfit-1.9.6/betanegbinfit/models/model.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.5/betanegbinfit/models/model_line.py` & `betanegbinfit-1.9.6/betanegbinfit/models/model_line.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.5/betanegbinfit/models/model_line_lrt.py` & `betanegbinfit-1.9.6/betanegbinfit/models/model_line_lrt.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.5/betanegbinfit/models/model_mixture.py` & `betanegbinfit-1.9.6/betanegbinfit/models/model_mixture.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.5/betanegbinfit/models/model_mixtures.py` & `betanegbinfit-1.9.6/betanegbinfit/models/model_mixtures.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.5/betanegbinfit/models/model_window.py` & `betanegbinfit-1.9.6/betanegbinfit/models/model_window.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.5/betanegbinfit/plot.py` & `betanegbinfit-1.9.6/betanegbinfit/plot.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.5/betanegbinfit/stats.py` & `betanegbinfit-1.9.6/betanegbinfit/stats.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.5/betanegbinfit/tests.py` & `betanegbinfit-1.9.6/betanegbinfit/tests.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.5/betanegbinfit/utils.py` & `betanegbinfit-1.9.6/betanegbinfit/utils.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.5/betanegbinfit.egg-info/PKG-INFO` & `betanegbinfit-1.9.6/betanegbinfit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 Metadata-Version: 2.1
 Name: betanegbinfit
-Version: 1.9.5
+Version: 1.9.6
+Summary: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
@@ -72,7 +75,9 @@
 
 
 **Please note, that all functions have plenty of optional arguments and they all are documented, so please consider reading through `help(function of interest)`.**
 
 
 ### A note on performance
 As far as we are concerned, **BetaNegBinFit** should work within a manageable amounts of time. For insance, when `ModelLine` with `model='BetaNB'` ran against *chipseq.tsv* dataset, it finishes in 6 minutes when ran at Ryzen 5600U. It does so under 2 minutes with `model='NB'`.
+
+
```

### Comparing `betanegbinfit-1.9.5/betanegbinfit.egg-info/SOURCES.txt` & `betanegbinfit-1.9.6/betanegbinfit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.5/setup.py` & `betanegbinfit-1.9.6/setup.py`

 * *Files identical despite different names*

