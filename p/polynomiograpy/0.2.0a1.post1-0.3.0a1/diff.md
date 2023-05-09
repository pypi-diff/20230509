# Comparing `tmp/polynomiograpy-0.2.0a1.post1.tar.gz` & `tmp/polynomiograpy-0.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polynomiograpy-0.2.0a1.post1.tar", max compression
+gzip compressed data, was "polynomiograpy-0.3.0a1.tar", max compression
```

## Comparing `polynomiograpy-0.2.0a1.post1.tar` & `polynomiograpy-0.3.0a1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-05-01 01:47:51.256690 polynomiograpy-0.2.0a1.post1/LICENSE
--rw-r--r--   0        0        0       68 2023-05-01 01:39:06.537562 polynomiograpy-0.2.0a1.post1/README.md
--rw-r--r--   0        0        0      420 2023-05-02 08:57:40.472153 polynomiograpy-0.2.0a1.post1/polynomiograpy/__init__.py
--rw-r--r--   0        0        0     4797 2023-05-02 08:54:25.623761 polynomiograpy-0.2.0a1.post1/polynomiograpy/cli/__init__.py
--rw-r--r--   0        0        0      970 2023-05-02 08:39:43.286847 polynomiograpy-0.2.0a1.post1/polynomiograpy/common/finite_field.py
--rw-r--r--   0        0        0     1458 2023-05-01 02:13:32.052248 polynomiograpy-0.2.0a1.post1/polynomiograpy/common/polynomial.py
--rw-r--r--   0        0        0     1991 2023-05-02 08:14:34.251805 polynomiograpy-0.2.0a1.post1/polynomiograpy/iterations/__init__.py
--rw-r--r--   0        0        0     1266 2023-05-02 07:52:35.745113 polynomiograpy-0.2.0a1.post1/polynomiograpy/iterations/helpers.py
--rw-r--r--   0        0        0     2279 2023-05-02 07:44:10.901452 polynomiograpy-0.2.0a1.post1/polynomiograpy/iterations/methods.py
--rw-r--r--   0        0        0      915 2023-05-02 08:43:46.491492 polynomiograpy-0.2.0a1.post1/polynomiograpy/roots/__init__.py
--rw-r--r--   0        0        0      931 2023-05-02 08:15:06.208942 polynomiograpy-0.2.0a1.post1/polynomiograpy/roots/helpers.py
--rw-r--r--   0        0        0      744 2023-05-02 08:56:30.404622 polynomiograpy-0.2.0a1.post1/pyproject.toml
--rw-r--r--   0        0        0      744 1970-01-01 00:00:00.000000 polynomiograpy-0.2.0a1.post1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-02 09:33:04.682513 polynomiograpy-0.3.0a1/LICENSE
+-rw-r--r--   0        0        0       68 2023-05-02 09:33:04.683048 polynomiograpy-0.3.0a1/README.md
+-rw-r--r--   0        0        0      414 2023-05-09 09:31:09.276312 polynomiograpy-0.3.0a1/polynomiograpy/__init__.py
+-rw-r--r--   0        0        0     4797 2023-05-02 09:33:04.685799 polynomiograpy-0.3.0a1/polynomiograpy/cli/__init__.py
+-rw-r--r--   0        0        0      970 2023-05-02 09:33:04.686106 polynomiograpy-0.3.0a1/polynomiograpy/common/finite_field.py
+-rw-r--r--   0        0        0     1458 2023-05-08 09:49:29.117520 polynomiograpy-0.3.0a1/polynomiograpy/common/polynomial.py
+-rw-r--r--   0        0        0     2302 2023-05-08 09:50:57.025154 polynomiograpy-0.3.0a1/polynomiograpy/iterations/__init__.py
+-rw-r--r--   0        0        0     1266 2023-05-08 09:31:50.010724 polynomiograpy-0.3.0a1/polynomiograpy/iterations/helpers.py
+-rw-r--r--   0        0        0     3146 2023-05-08 09:49:20.206774 polynomiograpy-0.3.0a1/polynomiograpy/iterations/methods.py
+-rw-r--r--   0        0        0      915 2023-05-02 09:33:04.687769 polynomiograpy-0.3.0a1/polynomiograpy/roots/__init__.py
+-rw-r--r--   0        0        0      931 2023-05-02 09:33:04.688126 polynomiograpy-0.3.0a1/polynomiograpy/roots/helpers.py
+-rw-r--r--   0        0        0      737 2023-05-09 09:30:55.687964 polynomiograpy-0.3.0a1/pyproject.toml
+-rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 polynomiograpy-0.3.0a1/PKG-INFO
```

### Comparing `polynomiograpy-0.2.0a1.post1/LICENSE` & `polynomiograpy-0.3.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.2.0a1.post1/polynomiograpy/cli/__init__.py` & `polynomiograpy-0.3.0a1/polynomiograpy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.2.0a1.post1/polynomiograpy/common/finite_field.py` & `polynomiograpy-0.3.0a1/polynomiograpy/common/finite_field.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.2.0a1.post1/polynomiograpy/common/polynomial.py` & `polynomiograpy-0.3.0a1/polynomiograpy/common/polynomial.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.2.0a1.post1/polynomiograpy/iterations/__init__.py` & `polynomiograpy-0.3.0a1/polynomiograpy/iterations/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 __all__ = [
     "compute_screen_for_single_poly",
     "available_methods",
 ]
 
 
 def compute_screen_for_single_poly(
-    method: Literal["newton", "halley", "steffensen"],
+    method: Literal["newton", "halley", "secant", "steffensen"],
     poly: Polynomial,
     delta: float,
     width: int,
     height: int,
     screen: np.ndarray,
     screen_buffer: np.ndarray,
     *,
@@ -48,14 +48,26 @@
                 poly,
                 val,
                 delta,
                 max_iter_count=max_value,
             )
             return iter_count
 
+    elif method == "secant":
+
+        def func(val: complex) -> int:
+            new_val, iter_count = methods.secant_method(
+                poly,
+                val,
+                None,
+                delta,
+                max_iter_count=max_value,
+            )
+            return iter_count
+
     elif method == "steffensen":
 
         def func(val: complex) -> int:
             new_val, iter_count = methods.steffensen_method(
                 poly,
                 val,
                 delta,
```

### Comparing `polynomiograpy-0.2.0a1.post1/polynomiograpy/iterations/helpers.py` & `polynomiograpy-0.3.0a1/polynomiograpy/iterations/helpers.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.2.0a1.post1/polynomiograpy/iterations/methods.py` & `polynomiograpy-0.3.0a1/polynomiograpy/iterations/methods.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from typing import Optional
 from polynomiograpy import common
 
-available_methods = {"newton", "halley", "steffensen"}
+available_methods = {"newton", "halley", "secant", "steffensen"}
 
 
 def newton_method(
     poly: common.polynomial.Polynomial,
     x: complex,
     delta: float,
     *,
@@ -12,15 +13,15 @@
     max_iter_count: int = 16,
 ) -> tuple[complex, int]:
     if step > max_iter_count:
         return x, 0
     res = poly.eval(x)
     deriv_res = poly.eval_deriv(x)
     if deriv_res == 0:
-        return x, 0
+        return x, max_iter_count - step
     newton_res = x - res / deriv_res
     if abs(newton_res - x) < delta:
         return newton_res, 0
     else:
         new_res, count = newton_method(
             poly,
             newton_res,
@@ -57,14 +58,46 @@
             delta,
             step=step + 1,
             max_iter_count=max_iter_count,
         )
         return new_res, count + 1
 
 
+def secant_method(
+    poly: common.polynomial.Polynomial,
+    x_0: complex,
+    x_1: Optional[complex],
+    delta: float,
+    *,
+    step: int = 0,
+    max_iter_count: int = 16,
+) -> tuple[complex, int]:
+    if step > max_iter_count:
+        return x_0, 0
+    if x_1 is None:
+        x_1, _ = newton_method(poly, x_0, delta, step=0, max_iter_count=0)
+    fx_0 = poly.eval(x_0)
+    fx_1 = poly.eval(x_1)
+    if fx_1 == fx_0:
+        return x_1, max_iter_count - step
+    res = x_1 - fx_1 * (x_1 - x_0) / (fx_1 - fx_0)
+    if abs(res - x_1) < delta:
+        return res, 0
+    else:
+        new_res, count = secant_method(
+            poly,
+            fx_1,
+            res,
+            delta,
+            step=step + 1,
+            max_iter_count=max_iter_count,
+        )
+        return new_res, count + 1
+
+
 def steffensen_method(
     poly: common.polynomial.Polynomial,
     x: complex,
     delta: float,
     *,
     step: int = 0,
     max_iter_count: int = 16,
```

### Comparing `polynomiograpy-0.2.0a1.post1/polynomiograpy/roots/__init__.py` & `polynomiograpy-0.3.0a1/polynomiograpy/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.2.0a1.post1/polynomiograpy/roots/helpers.py` & `polynomiograpy-0.3.0a1/polynomiograpy/roots/helpers.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.2.0a1.post1/pyproject.toml` & `polynomiograpy-0.3.0a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polynomiograpy"
-version = "0.2.0.a1.post1"
+version = "0.3.0.a1"
 description = ""
 authors = ["İsmail Tapan <ismltpn@gmail.com>"]
 maintainers = ["İsmail Tapan <ismltpn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = ""
 repository = "https://github.com/ismltpn/polynomiograpy/"
@@ -12,15 +12,15 @@
 keywords = [
     "Polynomiography",
     "Polynomials",
     "Visual Art"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.9"
 numpy = "^1.24.2"
 pillow = "^9.4.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
```

