# Comparing `tmp/funcx-2.0.2a0.tar.gz` & `tmp/funcx-2.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcx-2.0.2a0.tar", last modified: Mon May  1 15:17:58 2023, max compression
+gzip compressed data, was "funcx-2.0.2a1.tar", last modified: Mon May  8 22:01:37 2023, max compression
```

## Comparing `funcx-2.0.2a0.tar` & `funcx-2.0.2a1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:17:58.824521 funcx-2.0.2a0/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 funcx-2.0.2a0/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 funcx-2.0.2a0/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     1997 2023-05-01 15:17:58.824570 funcx-2.0.2a0/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     1051 2023-04-20 03:21:56.000000 funcx-2.0.2a0/PyPI.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:17:58.822991 funcx-2.0.2a0/funcx/
--rw-r--r--   0 lei        (501) staff       (20)      467 2023-04-10 19:02:41.000000 funcx-2.0.2a0/funcx/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:17:58.824152 funcx-2.0.2a0/funcx/sdk/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-20 15:03:07.000000 funcx-2.0.2a0/funcx/sdk/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)       78 2023-04-25 18:47:02.000000 funcx-2.0.2a0/funcx/sdk/client.py
--rw-r--r--   0 lei        (501) staff       (20)       84 2023-04-25 18:47:02.000000 funcx-2.0.2a0/funcx/sdk/executor.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:17:58.824299 funcx-2.0.2a0/funcx/sdk/login_manager/
--rw-r--r--   0 lei        (501) staff       (20)      445 2023-04-10 19:02:41.000000 funcx-2.0.2a0/funcx/sdk/login_manager/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)       88 2023-04-10 19:02:41.000000 funcx-2.0.2a0/funcx/sdk/web_client.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:17:58.824416 funcx-2.0.2a0/funcx/serialize/
--rw-r--r--   0 lei        (501) staff       (20)      110 2023-04-10 19:02:41.000000 funcx-2.0.2a0/funcx/serialize/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1146 2023-05-01 15:06:29.000000 funcx-2.0.2a0/funcx/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:17:58.823564 funcx-2.0.2a0/funcx.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     1997 2023-05-01 15:17:58.000000 funcx-2.0.2a0/funcx.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      377 2023-05-01 15:17:58.000000 funcx-2.0.2a0/funcx.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-05-01 15:17:58.000000 funcx-2.0.2a0/funcx.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)       28 2023-05-01 15:17:58.000000 funcx-2.0.2a0/funcx.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)        6 2023-05-01 15:17:58.000000 funcx-2.0.2a0/funcx.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      305 2023-05-01 15:17:58.824795 funcx-2.0.2a0/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     1915 2023-05-01 15:05:41.000000 funcx-2.0.2a0/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:37.877369 funcx-2.0.2a1/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 funcx-2.0.2a1/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 funcx-2.0.2a1/MANIFEST.in
+-rw-r--r--   0 lei        (501) staff       (20)     1997 2023-05-08 22:01:37.877433 funcx-2.0.2a1/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     1051 2023-04-20 03:21:56.000000 funcx-2.0.2a1/PyPI.md
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:37.871739 funcx-2.0.2a1/funcx/
+-rw-r--r--   0 lei        (501) staff       (20)      467 2023-04-10 19:02:41.000000 funcx-2.0.2a1/funcx/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:37.876869 funcx-2.0.2a1/funcx/sdk/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-20 15:03:07.000000 funcx-2.0.2a1/funcx/sdk/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)       78 2023-05-01 18:50:06.000000 funcx-2.0.2a1/funcx/sdk/client.py
+-rw-r--r--   0 lei        (501) staff       (20)       84 2023-05-01 18:50:06.000000 funcx-2.0.2a1/funcx/sdk/executor.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:37.877056 funcx-2.0.2a1/funcx/sdk/login_manager/
+-rw-r--r--   0 lei        (501) staff       (20)      445 2023-04-10 19:02:41.000000 funcx-2.0.2a1/funcx/sdk/login_manager/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)       88 2023-04-10 19:02:41.000000 funcx-2.0.2a1/funcx/sdk/web_client.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:37.877227 funcx-2.0.2a1/funcx/serialize/
+-rw-r--r--   0 lei        (501) staff       (20)      110 2023-04-10 19:02:41.000000 funcx-2.0.2a1/funcx/serialize/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1146 2023-05-08 21:59:08.000000 funcx-2.0.2a1/funcx/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:37.872617 funcx-2.0.2a1/funcx.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)     1997 2023-05-08 22:01:37.000000 funcx-2.0.2a1/funcx.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)      377 2023-05-08 22:01:37.000000 funcx-2.0.2a1/funcx.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-05-08 22:01:37.000000 funcx-2.0.2a1/funcx.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)       28 2023-05-08 22:01:37.000000 funcx-2.0.2a1/funcx.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)        6 2023-05-08 22:01:37.000000 funcx-2.0.2a1/funcx.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      305 2023-05-08 22:01:37.877714 funcx-2.0.2a1/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     1915 2023-05-08 21:58:59.000000 funcx-2.0.2a1/setup.py
```

### Comparing `funcx-2.0.2a0/LICENSE` & `funcx-2.0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `funcx-2.0.2a0/PKG-INFO` & `funcx-2.0.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcx
-Version: 2.0.2a0
+Version: 2.0.2a1
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: The Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `funcx-2.0.2a0/PyPI.md` & `funcx-2.0.2a1/PyPI.md`

 * *Files identical despite different names*

### Comparing `funcx-2.0.2a0/funcx/version.py` & `funcx-2.0.2a1/funcx/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from globus_compute_sdk.errors import VersionMismatch
 from packaging.version import Version
 
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.0.2a0"
+__version__ = "2.0.2a1"
 
 DEPRECATION_FUNCX = """
 The funcX SDK has been renamed to Globus Compute SDK and the new package is
 available on PyPI:
     https://pypi.org/project/globus-compute-sdk/
 
 Please consider upgrading to Globus Compute.  More information can be found at:
```

### Comparing `funcx-2.0.2a0/funcx.egg-info/PKG-INFO` & `funcx-2.0.2a1/funcx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcx
-Version: 2.0.2a0
+Version: 2.0.2a1
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: The Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `funcx-2.0.2a0/setup.py` & `funcx-2.0.2a1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import re
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
-    "globus-compute-sdk>=2.0.2a0",
+    "globus-compute-sdk>=2.0.2a1",
 ]
 
 
 def parse_version():
     # single source of truth for package version
     version_string = ""
     version_pattern = re.compile(r'__version__ = "([^"]*)"')
```

