# Comparing `tmp/intake_dataframe_catalog-0.0.3.tar.gz` & `tmp/intake_dataframe_catalog-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake_dataframe_catalog-0.0.3.tar", last modified: Mon May  8 07:46:50 2023, max compression
+gzip compressed data, was "intake_dataframe_catalog-0.0.4.tar", last modified: Tue May  9 06:34:54 2023, max compression
```

## Comparing `intake_dataframe_catalog-0.0.3.tar` & `intake_dataframe_catalog-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:46:50.525992 intake_dataframe_catalog-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-08 07:46:50.525992 intake_dataframe_catalog-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-08 07:46:50.525992 intake_dataframe_catalog-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:46:50.521992 intake_dataframe_catalog-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:46:50.525992 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-08 07:46:50.525992 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:46:50.525992 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-08 07:46:50.000000 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-08 07:46:50.000000 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:46:50.000000 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-08 07:46:50.000000 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 07:46:50.000000 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 07:46:50.000000 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:46:50.525992 intake_dataframe_catalog-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21272 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:34:54.629875 intake_dataframe_catalog-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-09 06:34:54.629875 intake_dataframe_catalog-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-09 06:34:54.629875 intake_dataframe_catalog-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:34:54.625875 intake_dataframe_catalog-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:34:54.629875 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-09 06:34:54.629875 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:34:54.629875 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-09 06:34:54.000000 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-09 06:34:54.000000 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:34:54.000000 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-09 06:34:54.000000 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 06:34:54.000000 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 06:34:54.000000 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:34:54.629875 intake_dataframe_catalog-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/versioneer.py
```

### Comparing `intake_dataframe_catalog-0.0.3/LICENSE` & `intake_dataframe_catalog-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.3/pyproject.toml` & `intake_dataframe_catalog-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -28,17 +28,23 @@
   "setuptools >= 61.0.0",
   "versioneer[toml]",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
-[tool.pytest]
+[tool.pytest.ini_options]
 addopts = "--cov=./src --cov-report=xml"
 
 [tool.versioneer]
 VCS = "git"
 style = "pep440"
 versionfile_source = "src/intake_dataframe_catalog/_version.py"
 versionfile_build = "intake_dataframe_catalog/_version.py"
 tag_prefix = "v"
 parentdir_prefix = "intake-dataframe-catalog-"
+
+[tool.coverage.run]
+omit = [
+    "src/intake_dataframe_catalog/_version.py",
+]
+
```

### Comparing `intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog/_search.py` & `intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog/_search.py`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog/core.py` & `intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog/core.py`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog.egg-info/SOURCES.txt` & `intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 LICENSE
-README.md
+README.rst
 pyproject.toml
 setup.cfg
 setup.py
 versioneer.py
 src/intake_dataframe_catalog/__init__.py
 src/intake_dataframe_catalog/_search.py
 src/intake_dataframe_catalog/_version.py
```

### Comparing `intake_dataframe_catalog-0.0.3/tests/test_core.py` & `intake_dataframe_catalog-0.0.4/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright 2023 ACCESS-NRI and contributors. See the top-level COPYRIGHT file for details.
+# SPDX-License-Identifier: Apache-2.0
+
 import ast
 from io import UnsupportedOperation
 
 import pytest
 
 import xarray as xr
 import pandas as pd
```

### Comparing `intake_dataframe_catalog-0.0.3/tests/test_search.py` & `intake_dataframe_catalog-0.0.4/tests/test_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright 2023 ACCESS-NRI and contributors. See the top-level COPYRIGHT file for details.
+# SPDX-License-Identifier: Apache-2.0
+
 import re
 
 import pytest
 
 import pandas as pd
 
 from intake_dataframe_catalog._search import _is_pattern, search
```

### Comparing `intake_dataframe_catalog-0.0.3/versioneer.py` & `intake_dataframe_catalog-0.0.4/versioneer.py`

 * *Files identical despite different names*

