# Comparing `tmp/motion_python-0.1.37.tar.gz` & `tmp/motion_python-0.1.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.37.tar", max compression
+gzip compressed data, was "motion_python-0.1.38.tar", max compression
```

## Comparing `motion_python-0.1.37.tar` & `motion_python-0.1.38.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     2752 2023-05-08 17:55:47.056983 motion_python-0.1.37/README.md
--rw-r--r--   0        0        0      120 2023-05-08 17:55:47.060983 motion_python-0.1.37/motion/__init__.py
--rw-r--r--   0        0        0    16074 2023-05-08 17:55:47.060983 motion_python-0.1.37/motion/component.py
--rw-r--r--   0        0        0     6413 2023-05-08 17:55:47.060983 motion_python-0.1.37/motion/execute.py
--rw-r--r--   0        0        0      595 2023-05-08 17:55:47.060983 motion_python-0.1.37/motion/route.py
--rw-r--r--   0        0        0     3089 2023-05-08 17:55:47.060983 motion_python-0.1.37/motion/utils.py
--rw-r--r--   0        0        0     1602 2023-05-08 17:56:11.377088 motion_python-0.1.37/pyproject.toml
--rw-r--r--   0        0        0     3875 1970-01-01 00:00:00.000000 motion_python-0.1.37/PKG-INFO
+-rw-r--r--   0        0        0     2752 2023-05-09 20:46:58.513933 motion_python-0.1.38/README.md
+-rw-r--r--   0        0        0      120 2023-05-09 20:46:58.513933 motion_python-0.1.38/motion/__init__.py
+-rw-r--r--   0        0        0     1327 2023-05-09 20:46:58.513933 motion_python-0.1.38/motion/cli.py
+-rw-r--r--   0        0        0    16300 2023-05-09 20:46:58.513933 motion_python-0.1.38/motion/component.py
+-rw-r--r--   0        0        0    12116 2023-05-09 20:46:58.513933 motion_python-0.1.38/motion/execute.py
+-rw-r--r--   0        0        0      595 2023-05-09 20:46:58.513933 motion_python-0.1.38/motion/route.py
+-rw-r--r--   0        0        0     3089 2023-05-09 20:46:58.513933 motion_python-0.1.38/motion/utils.py
+-rw-r--r--   0        0        0     1657 2023-05-09 20:47:19.349975 motion_python-0.1.38/pyproject.toml
+-rw-r--r--   0        0        0     3875 1970-01-01 00:00:00.000000 motion_python-0.1.38/PKG-INFO
```

### Comparing `motion_python-0.1.37/README.md` & `motion_python-0.1.38/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.37/motion/component.py` & `motion_python-0.1.38/motion/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import atexit
+import functools
 import inspect
 import logging
 from typing import Any, Callable, Dict, Tuple, Union, get_type_hints
 
 from motion.execute import Executor
 from motion.utils import (
     CustomDict,
@@ -311,14 +312,15 @@
             type_hint = get_type_hints(func).get("value", None)
             if not validate_args(inspect.signature(func).parameters, "infer"):
                 raise ValueError(
                     f"Infer function {func.__name__} should have 2 arguments "
                     + "`state` and `value`"
                 )
 
+            @functools.wraps(func)
             def wrapper(state: CustomDict, value: Any) -> Any:
                 if type_hint and not isinstance(value, type_hint):
                     try:
                         value = type_hint(**value)
                     except Exception:
                         raise ValueError(
                             f"value argument must be of type {type_hint.__name__}"
@@ -493,7 +495,13 @@
                 )
             fit_event.wait()
 
         if return_fit_event:
             return infer_result, fit_event
 
         return infer_result
+
+    def get_graph(self) -> Dict[str, Any]:
+        """
+        Gets the graph of infer and fit ops for this component.
+        """
+        return self._executor.get_graph()
```

### Comparing `motion_python-0.1.37/motion/route.py` & `motion_python-0.1.38/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.37/motion/utils.py` & `motion_python-0.1.38/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.37/pyproject.toml` & `motion_python-0.1.38/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.37"
+version = "0.1.38"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -40,14 +40,17 @@
 pytkdocs = "^0.16.1"
 linkchecker = "^10.2.1"
 ruff = "^0.0.261"
 maturin = "^0.14.17"
 mike = "^1.1.2"
 scikit-learn = "^1.2.2"
 
+[tool.poetry.scripts]
+motion = "motion.cli:motioncli"
+
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.mypy]
 files = "motion"
 mypy_path = "motion"
 warn_return_any = true
```

### Comparing `motion_python-0.1.37/PKG-INFO` & `motion_python-0.1.38/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.37
+Version: 0.1.38
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

