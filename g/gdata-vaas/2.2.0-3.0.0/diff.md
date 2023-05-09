# Comparing `tmp/gdata-vaas-2.2.0.tar.gz` & `tmp/gdata-vaas-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdata-vaas-2.2.0.tar", last modified: Mon Mar  6 09:25:48 2023, max compression
+gzip compressed data, was "gdata-vaas-3.0.0.tar", last modified: Tue May  9 14:19:12 2023, max compression
```

## Comparing `gdata-vaas-2.2.0.tar` & `gdata-vaas-3.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 09:25:48.527345 gdata-vaas-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-03-06 09:24:53.000000 gdata-vaas-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-03-06 09:25:48.527345 gdata-vaas-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-03-06 09:24:53.000000 gdata-vaas-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-03-06 09:24:53.000000 gdata-vaas-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      740 2023-03-06 09:25:48.527345 gdata-vaas-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 09:25:48.523345 gdata-vaas-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 09:25:48.523345 gdata-vaas-2.2.0/src/gdata_vaas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-03-06 09:25:48.000000 gdata-vaas-2.2.0/src/gdata_vaas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-03-06 09:25:48.000000 gdata-vaas-2.2.0/src/gdata_vaas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-06 09:25:48.000000 gdata-vaas-2.2.0/src/gdata_vaas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-03-06 09:25:48.000000 gdata-vaas-2.2.0/src/gdata_vaas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-03-06 09:25:48.000000 gdata-vaas-2.2.0/src/gdata_vaas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 09:25:48.527345 gdata-vaas-2.2.0/src/vaas/
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-03-06 09:24:53.000000 gdata-vaas-2.2.0/src/vaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      938 2023-03-06 09:24:53.000000 gdata-vaas-2.2.0/src/vaas/client_credentials_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (122)    10378 2023-03-06 09:24:53.000000 gdata-vaas-2.2.0/src/vaas/vaas.py
--rw-r--r--   0 runner    (1001) docker     (122)      292 2023-03-06 09:24:53.000000 gdata-vaas-2.2.0/src/vaas/vaas_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 09:25:48.527345 gdata-vaas-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-03-06 09:24:53.000000 gdata-vaas-2.2.0/tests/test_client_credentials_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (122)     8305 2023-03-06 09:24:53.000000 gdata-vaas-2.2.0/tests/test_vaas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:19:12.783696 gdata-vaas-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-05-09 14:18:27.000000 gdata-vaas-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-05-09 14:19:12.783696 gdata-vaas-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-05-09 14:18:27.000000 gdata-vaas-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-09 14:18:27.000000 gdata-vaas-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-05-09 14:19:12.783696 gdata-vaas-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:19:12.779696 gdata-vaas-3.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:19:12.783696 gdata-vaas-3.0.0/src/gdata_vaas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-05-09 14:19:12.000000 gdata-vaas-3.0.0/src/gdata_vaas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-09 14:19:12.000000 gdata-vaas-3.0.0/src/gdata_vaas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 14:19:12.000000 gdata-vaas-3.0.0/src/gdata_vaas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-09 14:19:12.000000 gdata-vaas-3.0.0/src/gdata_vaas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-09 14:19:12.000000 gdata-vaas-3.0.0/src/gdata_vaas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:19:12.783696 gdata-vaas-3.0.0/src/vaas/
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-05-09 14:18:27.000000 gdata-vaas-3.0.0/src/vaas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      938 2023-05-09 14:18:27.000000 gdata-vaas-3.0.0/src/vaas/client_credentials_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10389 2023-05-09 14:18:27.000000 gdata-vaas-3.0.0/src/vaas/vaas.py
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-05-09 14:18:27.000000 gdata-vaas-3.0.0/src/vaas/vaas_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:19:12.783696 gdata-vaas-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-05-09 14:18:27.000000 gdata-vaas-3.0.0/tests/test_client_credentials_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8305 2023-05-09 14:18:27.000000 gdata-vaas-3.0.0/tests/test_vaas.py
```

### Comparing `gdata-vaas-2.2.0/LICENSE` & `gdata-vaas-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdata-vaas-2.2.0/PKG-INFO` & `gdata-vaas-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdata-vaas
-Version: 2.2.0
+Version: 3.0.0
 Summary: gdata-vaas is a Python library for the VaaS-API.
 Home-page: https://github.com/GDATASoftwareAG/vaas/tree/main/python
 Author: G DATA CyberDefense AG
 Author-email: oem@gdata.de
 Project-URL: Bug Tracker, https://github.com/GDATASoftwareAG/vaas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gdata-vaas-2.2.0/README.md` & `gdata-vaas-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `gdata-vaas-2.2.0/setup.cfg` & `gdata-vaas-3.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gdata-vaas
-version = 2.2.0
+version = 3.0.0
 author = G DATA CyberDefense AG
 author_email = oem@gdata.de
 description = gdata-vaas is a Python library for the VaaS-API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/GDATASoftwareAG/vaas/tree/main/python
 project_urls =
```

### Comparing `gdata-vaas-2.2.0/src/gdata_vaas.egg-info/PKG-INFO` & `gdata-vaas-3.0.0/src/gdata_vaas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdata-vaas
-Version: 2.2.0
+Version: 3.0.0
 Summary: gdata-vaas is a Python library for the VaaS-API.
 Home-page: https://github.com/GDATASoftwareAG/vaas/tree/main/python
 Author: G DATA CyberDefense AG
 Author-email: oem@gdata.de
 Project-URL: Bug Tracker, https://github.com/GDATASoftwareAG/vaas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gdata-vaas-2.2.0/src/vaas/__init__.py` & `gdata-vaas-3.0.0/src/vaas/__init__.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-2.2.0/src/vaas/client_credentials_grant_authenticator.py` & `gdata-vaas-3.0.0/src/vaas/client_credentials_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-2.2.0/src/vaas/vaas.py` & `gdata-vaas-3.0.0/src/vaas/vaas.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 class Vaas:
     """Verdict-as-a-Service client"""
 
     def __init__(
         self,
         tracing=VaasTracing(),
         options=VaasOptions(),
-        url="wss://gateway-vaas.gdatasecurity.de",
+        url="wss://gateway.production.vaas.gdatasecurity.de",
     ):
         self.tracing = tracing
         self.loop_result = None
         self.websocket = None
         self.session_id = None
         self.results = {}
         self.httpx_client: Optional[httpx.AsyncClient] = None
```

### Comparing `gdata-vaas-2.2.0/tests/test_client_credentials_grant_authenticator.py` & `gdata-vaas-3.0.0/tests/test_client_credentials_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-2.2.0/tests/test_vaas.py` & `gdata-vaas-3.0.0/tests/test_vaas.py`

 * *Files identical despite different names*

