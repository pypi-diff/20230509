# Comparing `tmp/byu_pytest_utils-0.6.0.tar.gz` & `tmp/byu_pytest_utils-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byu_pytest_utils-0.6.0.tar", max compression
+gzip compressed data, was "byu_pytest_utils-0.6.1.tar", max compression
```

## Comparing `byu_pytest_utils-0.6.0.tar` & `byu_pytest_utils-0.6.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-04-21 21:42:09.303677 byu_pytest_utils-0.6.0/byu_pytest_utils/__init__.py
--rw-r--r--   0        0        0      714 2022-03-14 21:00:52.263812 byu_pytest_utils-0.6.0/byu_pytest_utils/decorators.py
--rw-r--r--   0        0        0     9871 2023-04-21 21:40:40.002962 byu_pytest_utils-0.6.0/byu_pytest_utils/dialog.py
--rw-r--r--   0        0        0     3088 2023-03-04 23:37:17.852701 byu_pytest_utils-0.6.0/byu_pytest_utils/edit_dist.py
--rw-r--r--   0        0        0     3595 2023-03-06 23:42:26.126776 byu_pytest_utils-0.6.0/byu_pytest_utils/pytest_plugin.py
--rw-r--r--   0        0        0     3474 2023-04-21 21:39:00.608118 byu_pytest_utils-0.6.0/byu_pytest_utils/utils.py
--rw-r--r--   0        0        0      562 2023-04-21 21:37:59.023625 byu_pytest_utils-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 byu_pytest_utils-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-21 21:42:09.303677 byu_pytest_utils-0.6.1/byu_pytest_utils/__init__.py
+-rw-r--r--   0        0        0      714 2022-03-14 21:00:52.263812 byu_pytest_utils-0.6.1/byu_pytest_utils/decorators.py
+-rw-r--r--   0        0        0     9913 2023-05-09 20:05:05.372932 byu_pytest_utils-0.6.1/byu_pytest_utils/dialog.py
+-rw-r--r--   0        0        0     3088 2023-03-04 23:37:17.852701 byu_pytest_utils-0.6.1/byu_pytest_utils/edit_dist.py
+-rw-r--r--   0        0        0     3595 2023-03-06 23:42:26.126776 byu_pytest_utils-0.6.1/byu_pytest_utils/pytest_plugin.py
+-rw-r--r--   0        0        0     3474 2023-04-21 21:39:00.608118 byu_pytest_utils-0.6.1/byu_pytest_utils/utils.py
+-rw-r--r--   0        0        0      562 2023-05-09 20:05:17.878302 byu_pytest_utils-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 byu_pytest_utils-0.6.1/PKG-INFO
```

### Comparing `byu_pytest_utils-0.6.0/byu_pytest_utils/__init__.py` & `byu_pytest_utils-0.6.1/byu_pytest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.6.0/byu_pytest_utils/decorators.py` & `byu_pytest_utils-0.6.1/byu_pytest_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.6.0/byu_pytest_utils/dialog.py` & `byu_pytest_utils-0.6.1/byu_pytest_utils/dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         # func should have empty (pass) body and no arguments
         def new_func(group_name):
             group_stat = group_stats[group_name]
             if not group_stat['passed']:
                 assert group_stat['observed'] == group_stat['expected']
 
         new_func._group_stats = group_stats
+        new_func.__name__ = func.__name__
         return new_func
 
     return decorator
 
 
 class DialogChecker:
     DEFAULT_GROUP = '.'
```

### Comparing `byu_pytest_utils-0.6.0/byu_pytest_utils/edit_dist.py` & `byu_pytest_utils-0.6.1/byu_pytest_utils/edit_dist.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.6.0/byu_pytest_utils/pytest_plugin.py` & `byu_pytest_utils-0.6.1/byu_pytest_utils/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.6.0/byu_pytest_utils/utils.py` & `byu_pytest_utils-0.6.1/byu_pytest_utils/utils.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.6.0/pyproject.toml` & `byu_pytest_utils-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "byu_pytest_utils"
-version = "0.6.0"
+version = "0.6.1"
 description = "A few utilities for pytest to help with integration into gradescope"
 authors = ["Gordon Bean <gbean@cs.byu.edu>", "Daniel Zappala <daniel.zappala@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Framework :: Pytest"
 ]
```

### Comparing `byu_pytest_utils-0.6.0/PKG-INFO` & `byu_pytest_utils-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byu-pytest-utils
-Version: 0.6.0
+Version: 0.6.1
 Summary: A few utilities for pytest to help with integration into gradescope
 License: MIT
 Author: Gordon Bean
 Author-email: gbean@cs.byu.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
```

