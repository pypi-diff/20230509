# Comparing `tmp/gridstatusio-0.2.0.tar.gz` & `tmp/gridstatusio-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/github/workspace/dist/.tmp-ooox1f17/gridstatusio-0.2.0.tar", last modified: Thu May  4 19:55:00 2023, max compression
+gzip compressed data, was "/github/workspace/dist/.tmp-e08qpimp/gridstatusio-0.2.1.tar", last modified: Mon May  8 23:29:44 2023, max compression
```

## Comparing `gridstatusio-0.2.0.tar` & `gridstatusio-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     1461 2023-05-04 19:54:46.000000 gridstatusio-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3258 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      848 2023-05-04 19:54:46.000000 gridstatusio-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/gridstatusio/
--rw-r--r--   0 root         (0) root         (0)       98 2023-05-04 19:54:46.000000 gridstatusio-0.2.0/gridstatusio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8289 2023-05-04 19:54:46.000000 gridstatusio-0.2.0/gridstatusio/gs_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/gridstatusio/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 19:54:46.000000 gridstatusio-0.2.0/gridstatusio/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1315 2023-05-04 19:54:46.000000 gridstatusio-0.2.0/gridstatusio/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-04 19:54:46.000000 gridstatusio-0.2.0/gridstatusio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/gridstatusio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3258 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/gridstatusio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      348 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/gridstatusio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/gridstatusio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      237 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/gridstatusio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/gridstatusio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2319 2023-05-04 19:54:46.000000 gridstatusio-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-05-08 23:29:30.000000 gridstatusio-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3258 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      848 2023-05-08 23:29:30.000000 gridstatusio-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/gridstatusio/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-05-08 23:29:30.000000 gridstatusio-0.2.1/gridstatusio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8292 2023-05-08 23:29:30.000000 gridstatusio-0.2.1/gridstatusio/gs_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/gridstatusio/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 23:29:30.000000 gridstatusio-0.2.1/gridstatusio/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1315 2023-05-08 23:29:30.000000 gridstatusio-0.2.1/gridstatusio/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-08 23:29:30.000000 gridstatusio-0.2.1/gridstatusio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/gridstatusio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3258 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/gridstatusio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      348 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/gridstatusio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/gridstatusio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/gridstatusio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/gridstatusio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-05-08 23:29:30.000000 gridstatusio-0.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/setup.cfg
```

### Comparing `gridstatusio-0.2.0/LICENSE` & `gridstatusio-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gridstatusio-0.2.0/PKG-INFO` & `gridstatusio-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridstatusio
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python Client for GridStatus.io API
 Author-email: Max Kanter <kmax12@gmail.com>
 Maintainer-email: Max Kanter <kmax12@gmail.com>
 License: Copyright 2022 James Max Kanter
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

### Comparing `gridstatusio-0.2.0/README.md` & `gridstatusio-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gridstatusio-0.2.0/gridstatusio/gs_client.py` & `gridstatusio-0.2.1/gridstatusio/gs_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from tabulate import tabulate
 from termcolor import colored, cprint
 
 from gridstatusio import __version__
 
 
 class GridStatusClient:
-    def __init__(self, api_key=None, host="https://api.gridstatus.io"):
+    def __init__(self, api_key=None, host="https://api.gridstatus.io/v1"):
         """Create a GridStatus.io API client
 
         Parameters:
             api_key (str): The API key to use for authentication.
             If not provided, the GRIDSTATUS_API_KEY environment variable will be used.
 
             host (str): The host to use for the API.
```

### Comparing `gridstatusio-0.2.0/gridstatusio/tests/test_api.py` & `gridstatusio-0.2.1/gridstatusio/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `gridstatusio-0.2.0/gridstatusio.egg-info/PKG-INFO` & `gridstatusio-0.2.1/gridstatusio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridstatusio
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python Client for GridStatus.io API
 Author-email: Max Kanter <kmax12@gmail.com>
 Maintainer-email: Max Kanter <kmax12@gmail.com>
 License: Copyright 2022 James Max Kanter
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

### Comparing `gridstatusio-0.2.0/pyproject.toml` & `gridstatusio-0.2.1/pyproject.toml`

 * *Files identical despite different names*

