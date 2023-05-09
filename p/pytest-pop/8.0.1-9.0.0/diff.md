# Comparing `tmp/pytest-pop-8.0.1.tar.gz` & `tmp/pytest-pop-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-pop-8.0.1.tar", last modified: Thu Aug 19 01:14:05 2021, max compression
+gzip compressed data, was "pytest-pop-9.0.0.tar", last modified: Wed Apr 20 01:48:44 2022, max compression
```

## Comparing `pytest-pop-8.0.1.tar` & `pytest-pop-9.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-08-19 01:14:05.359005 pytest-pop-8.0.1/
--rw-r--r--   0 akmod     (1000) akmod     (1000)    11357 2021-05-04 22:58:15.000000 pytest-pop-8.0.1/LICENSE
--rw-r--r--   0 akmod     (1000) akmod     (1000)     5003 2021-08-19 01:14:05.359005 pytest-pop-8.0.1/PKG-INFO
--rw-r--r--   0 akmod     (1000) akmod     (1000)     4231 2020-11-23 10:10:03.000000 pytest-pop-8.0.1/README.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      255 2020-11-23 10:10:06.000000 pytest-pop-8.0.1/pyproject.toml
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-08-19 01:14:05.359005 pytest-pop-8.0.1/pytest_pop/
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-08-19 01:14:05.359005 pytest-pop-8.0.1/pytest_pop/mods/
--rw-r--r--   0 akmod     (1000) akmod     (1000)    12764 2021-08-19 01:12:39.000000 pytest-pop-8.0.1/pytest_pop/mods/testing.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     4990 2021-05-25 23:42:29.000000 pytest-pop-8.0.1/pytest_pop/plugin.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-08-19 01:14:05.359005 pytest-pop-8.0.1/pytest_pop.egg-info/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     5003 2021-08-19 01:14:05.000000 pytest-pop-8.0.1/pytest_pop.egg-info/PKG-INFO
--rw-r--r--   0 akmod     (1000) akmod     (1000)      296 2021-08-19 01:14:05.000000 pytest-pop-8.0.1/pytest_pop.egg-info/SOURCES.txt
--rw-r--r--   0 akmod     (1000) akmod     (1000)        1 2021-08-19 01:14:05.000000 pytest-pop-8.0.1/pytest_pop.egg-info/dependency_links.txt
--rw-r--r--   0 akmod     (1000) akmod     (1000)       43 2021-08-19 01:14:05.000000 pytest-pop-8.0.1/pytest_pop.egg-info/entry_points.txt
--rw-r--r--   0 akmod     (1000) akmod     (1000)       75 2021-08-19 01:14:05.000000 pytest-pop-8.0.1/pytest_pop.egg-info/requires.txt
--rw-r--r--   0 akmod     (1000) akmod     (1000)       11 2021-08-19 01:14:05.000000 pytest-pop-8.0.1/pytest_pop.egg-info/top_level.txt
--rw-r--r--   0 akmod     (1000) akmod     (1000)       38 2021-08-19 01:14:05.359005 pytest-pop-8.0.1/setup.cfg
--rw-r--r--   0 akmod     (1000) akmod     (1000)     2725 2021-08-19 01:13:28.000000 pytest-pop-8.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-20 01:48:44.247918 pytest-pop-9.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-04-20 01:48:28.000000 pytest-pop-9.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5003 2022-04-20 01:48:44.247918 pytest-pop-9.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4231 2022-04-20 01:48:28.000000 pytest-pop-9.0.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)      255 2022-04-20 01:48:28.000000 pytest-pop-9.0.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-20 01:48:44.246918 pytest-pop-9.0.0/pytest_pop/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-20 01:48:44.247918 pytest-pop-9.0.0/pytest_pop/mods/
+-rw-r--r--   0 root         (0) root         (0)    12821 2022-04-20 01:48:28.000000 pytest-pop-9.0.0/pytest_pop/mods/testing.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2022-04-20 01:48:28.000000 pytest-pop-9.0.0/pytest_pop/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-20 01:48:44.247918 pytest-pop-9.0.0/pytest_pop.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5003 2022-04-20 01:48:44.000000 pytest-pop-9.0.0/pytest_pop.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      296 2022-04-20 01:48:44.000000 pytest-pop-9.0.0/pytest_pop.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-04-20 01:48:44.000000 pytest-pop-9.0.0/pytest_pop.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2022-04-20 01:48:44.000000 pytest-pop-9.0.0/pytest_pop.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      113 2022-04-20 01:48:44.000000 pytest-pop-9.0.0/pytest_pop.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2022-04-20 01:48:44.000000 pytest-pop-9.0.0/pytest_pop.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-04-20 01:48:44.247918 pytest-pop-9.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2725 2022-04-20 01:48:28.000000 pytest-pop-9.0.0/setup.py
```

### Comparing `pytest-pop-8.0.1/LICENSE` & `pytest-pop-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-pop-8.0.1/PKG-INFO` & `pytest-pop-9.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-pop
-Version: 8.0.1
+Version: 9.0.0
 Summary: A pytest plugin to help with testing pop projects
 Home-page: https://gitlab.com/saltstack/pop/pytest-pop
 Author: Tyler Johnson
 Author-email: tjohnson@saltstack.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Framework :: Pytest
```

### Comparing `pytest-pop-8.0.1/README.rst` & `pytest-pop-9.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-pop-8.0.1/pytest_pop/mods/testing.py` & `pytest-pop-9.0.0/pytest_pop/mods/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 
 import pop.contract
 import pop.hub
 import pop.loader
 
 try:
     HAS_TEST = False
-    from asynctest.mock import create_autospec, Mock
+    from asynctest.mock import create_autospec
 
     HAS_TEST = True
 except (ImportError, ModuleNotFoundError):
     try:
-        from unittest.mock import create_autospec as mock_create_autospec, Mock
+        from unittest.mock import create_autospec as mock_create_autospec
 
         HAS_TEST = True
 
         def create_autospec(spec, *args, **kwargs):
             if asyncio.iscoroutinefunction(spec):
                 raise Exception(
                     "MockHub requires asynctest in order to mock async functions"
@@ -276,14 +276,17 @@
     """
     Provides mocks mirroring a real hub::
 
         hub.sub.mod.fn()  # mock
         hub.sub.mod.attr  # mock
     """
 
+    def __getitem__(self, item):
+        return getattr(self, item)
+
     def _mock_function(self, f: pop.contract.Contracted) -> Callable:
         afunc = create_autospec(strip_hub(f.func), spec_set=True)
         afunc.__signature__ = f.signature
         return afunc
 
 
 def fn_hub(hub: pop.hub.Hub) -> "NoContractHub":
```

### Comparing `pytest-pop-8.0.1/pytest_pop.egg-info/PKG-INFO` & `pytest-pop-9.0.0/pytest_pop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-pop
-Version: 8.0.1
+Version: 9.0.0
 Summary: A pytest plugin to help with testing pop projects
 Home-page: https://gitlab.com/saltstack/pop/pytest-pop
 Author: Tyler Johnson
 Author-email: tjohnson@saltstack.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Framework :: Pytest
```

### Comparing `pytest-pop-8.0.1/setup.py` & `pytest-pop-9.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import Command
 from setuptools import setup
 
 NAME = "pytest_pop"
 DESC = "A pytest plugin to help with testing pop projects"
 
 # Version info -- read without importing
-VERSION = "8.0.1"
+VERSION = "9.0.0"
 
 SETUP_DIRNAME = os.path.dirname(__file__)
 if not SETUP_DIRNAME:
     SETUP_DIRNAME = os.getcwd()
 
 with open("README.rst", encoding="utf-8") as f:
     LONG_DESC = f.read()
```

