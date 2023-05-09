# Comparing `tmp/tllab_common-2023.4.0.tar.gz` & `tmp/tllab_common-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tllab_common-2023.4.0.tar", max compression
+gzip compressed data, was "tllab_common-2023.4.1.tar", max compression
```

## Comparing `tllab_common-2023.4.0.tar` & `tllab_common-2023.4.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2023.4.0/LICENSE
--rw-r--r--   0        0        0      770 2021-11-19 15:34:09.296030 tllab_common-2023.4.0/README.md
--rw-r--r--   0        0        0      890 2023-04-26 07:40:47.944715 tllab_common-2023.4.0/pyproject.toml
--rw-r--r--   0        0        0      461 2023-04-26 07:34:18.368614 tllab_common-2023.4.0/tllab_common/__init__.py
--rwxr-xr-x   0        0        0    10047 2022-09-20 13:24:57.600406 tllab_common-2023.4.0/tllab_common/findcells.py
--rw-r--r--   0        0        0     5273 2023-04-26 17:33:28.869142 tllab_common-2023.4.0/tllab_common/fit.py
--rw-r--r--   0        0        0    10422 2023-04-26 14:30:00.605612 tllab_common-2023.4.0/tllab_common/misc.py
--rw-r--r--   0        0        0      187 2021-10-14 16:27:02.346127 tllab_common-2023.4.0/tllab_common/transform.txt
--rw-r--r--   0        0        0     9202 2022-08-08 15:25:51.713820 tllab_common-2023.4.0/tllab_common/transforms.py
--rwxr-xr-x   0        0        0    68716 2023-04-06 14:47:24.519652 tllab_common-2023.4.0/tllab_common/wimread.py
--rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 tllab_common-2023.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2023.4.1/LICENSE
+-rw-r--r--   0        0        0      770 2021-11-19 15:34:09.296030 tllab_common-2023.4.1/README.md
+-rw-r--r--   0        0        0      890 2023-05-09 13:39:29.933328 tllab_common-2023.4.1/pyproject.toml
+-rw-r--r--   0        0        0      461 2023-04-26 07:34:18.368614 tllab_common-2023.4.1/tllab_common/__init__.py
+-rwxr-xr-x   0        0        0    10047 2022-09-20 13:24:57.600406 tllab_common-2023.4.1/tllab_common/findcells.py
+-rw-r--r--   0        0        0     5262 2023-05-09 13:37:30.393996 tllab_common-2023.4.1/tllab_common/fit.py
+-rw-r--r--   0        0        0    10422 2023-04-26 14:30:00.605612 tllab_common-2023.4.1/tllab_common/misc.py
+-rw-r--r--   0        0        0      187 2021-10-14 16:27:02.346127 tllab_common-2023.4.1/tllab_common/transform.txt
+-rw-r--r--   0        0        0     9202 2022-08-08 15:25:51.713820 tllab_common-2023.4.1/tllab_common/transforms.py
+-rwxr-xr-x   0        0        0    68716 2023-04-06 14:47:24.519652 tllab_common-2023.4.1/tllab_common/wimread.py
+-rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 tllab_common-2023.4.1/PKG-INFO
```

### Comparing `tllab_common-2023.4.0/LICENSE` & `tllab_common-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.4.0/README.md` & `tllab_common-2023.4.1/README.md`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.4.0/pyproject.toml` & `tllab_common-2023.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tllab_common"
-version = "2023.4.0"
+version = "2023.4.1"
 description = "Common code for the Lenstra lab."
 authors = ["Lenstra lab NKI <t.lenstra@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["burst", "transcription"]
 include = ["transform.txt"]
 repository = "https://github.com/Lenstralab/tllab_common"
```

### Comparing `tllab_common-2023.4.0/tllab_common/findcells.py` & `tllab_common-2023.4.1/tllab_common/findcells.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.4.0/tllab_common/fit.py` & `tllab_common-2023.4.1/tllab_common/fit.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from functools import cached_property
-from scipy.optimize import minimize
+from scipy.optimize import minimize, OptimizeResult
 from abc import ABCMeta, abstractmethod
 
 
 class Fit(metaclass=ABCMeta):
     def __init__(self, x, y, w=None, log_scale=False):
         x = np.asarray(x)
         y = np.asarray(y)
@@ -55,24 +55,23 @@
                 return np.sum(self.w * (self.y - self.fun(p, self.x)) ** 2)
         return cost
 
     @cached_property
     def r(self):
         if len(self.x):
             r = minimize(self.get_cost_fun(), self.p0, method='Nelder-Mead', bounds=self.bounds)
-            if self.log_scale:
-                self.chi_squared, self.p_ci95, self.r_squared = fminerr(lambda p, x: np.log(self.fun(p, x)),
-                                                                        r.x, np.log(self.y), (self.x,), self.w)
-            else:
-                self.chi_squared, self.p_ci95, self.r_squared = fminerr(self.fun, r.x, self.y, (self.x,), self.w)
-            self.r_squared_adjusted = 1 - (1 - self.r_squared) * (self.n - 1) / (len(r.x) - 1)
         else:
-            r = None
-            self.chi_squared, self.r_squared, self.r_squared_adjusted = np.nan, np.nan, np.nan
-            self.p_ci95 = np.full(self.n_p, np.nan)
+            r = OptimizeResult(fun=np.nan, message='Empty data', nfev=0, nit=0, status=1, success=False,
+                               x=np.full(self.n_p, np.nan))
+        if self.log_scale:
+            self.chi_squared, self.p_ci95, self.r_squared = fminerr(lambda p, x: np.log(self.fun(p, x)),
+                                                                    r.x, np.log(self.y), (self.x,), self.w)
+        else:
+            self.chi_squared, self.p_ci95, self.r_squared = fminerr(self.fun, r.x, self.y, (self.x,), self.w)
+        self.r_squared_adjusted = 1 - (1 - self.r_squared) * (self.n - 1) / (len(r.x) - 1)
         return r
 
     @property
     def p(self):
         return np.full(self.n_p, np.nan) if self.r is None else self.r.x
 
     @property
```

### Comparing `tllab_common-2023.4.0/tllab_common/misc.py` & `tllab_common-2023.4.1/tllab_common/misc.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.4.0/tllab_common/transforms.py` & `tllab_common-2023.4.1/tllab_common/transforms.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.4.0/tllab_common/wimread.py` & `tllab_common-2023.4.1/tllab_common/wimread.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.4.0/PKG-INFO` & `tllab_common-2023.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tllab-common
-Version: 2023.4.0
+Version: 2023.4.1
 Summary: Common code for the Lenstra lab.
 Home-page: https://github.com/Lenstralab/tllab_common
 License: GPLv3
 Keywords: burst,transcription
 Author: Lenstra lab NKI
 Author-email: t.lenstra@nki.nl
 Requires-Python: >=3.8,<4.0
```

