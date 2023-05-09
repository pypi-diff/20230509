# Comparing `tmp/resotoclient-1.4.0.tar.gz` & `tmp/resotoclient-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoclient-1.4.0.tar", max compression
+gzip compressed data, was "resotoclient-1.4.1.tar", max compression
```

## Comparing `resotoclient-1.4.0.tar` & `resotoclient-1.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-05-08 13:39:50.853873 resotoclient-1.4.0/LICENSE
--rw-r--r--   0        0        0     1243 2023-05-08 13:39:50.853873 resotoclient-1.4.0/README.md
--rw-r--r--   0        0        0     2082 2023-05-08 13:39:50.857874 resotoclient-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    20715 2023-05-08 13:39:50.857874 resotoclient-1.4.0/resotoclient/__init__.py
--rw-r--r--   0        0        0    23316 2023-05-08 13:39:50.857874 resotoclient-1.4.0/resotoclient/async_client.py
--rw-r--r--   0        0        0     6219 2023-05-08 13:39:50.857874 resotoclient-1.4.0/resotoclient/ca.py
--rw-r--r--   0        0        0     2813 2023-05-08 13:39:50.857874 resotoclient-1.4.0/resotoclient/http_client/__init__.py
--rw-r--r--   0        0        0    12959 2023-05-08 13:39:50.857874 resotoclient-1.4.0/resotoclient/http_client/aiohttp_client.py
--rw-r--r--   0        0        0     1282 2023-05-08 13:39:50.857874 resotoclient-1.4.0/resotoclient/http_client/event_loop_thread.py
--rw-r--r--   0        0        0      693 2023-05-08 13:39:50.857874 resotoclient-1.4.0/resotoclient/json_utils.py
--rw-r--r--   0        0        0     3813 2023-05-08 13:39:50.857874 resotoclient-1.4.0/resotoclient/jwt_utils.py
--rw-r--r--   0        0        0     2283 2023-05-08 13:39:50.857874 resotoclient-1.4.0/resotoclient/models.py
--rw-r--r--   0        0        0     2721 1970-01-01 00:00:00.000000 resotoclient-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-09 13:17:30.428599 resotoclient-1.4.1/LICENSE
+-rw-r--r--   0        0        0     1243 2023-05-09 13:17:30.428599 resotoclient-1.4.1/README.md
+-rw-r--r--   0        0        0     2083 2023-05-09 13:17:30.428599 resotoclient-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0    20715 2023-05-09 13:17:30.428599 resotoclient-1.4.1/resotoclient/__init__.py
+-rw-r--r--   0        0        0    23316 2023-05-09 13:17:30.428599 resotoclient-1.4.1/resotoclient/async_client.py
+-rw-r--r--   0        0        0     6219 2023-05-09 13:17:30.428599 resotoclient-1.4.1/resotoclient/ca.py
+-rw-r--r--   0        0        0     2813 2023-05-09 13:17:30.428599 resotoclient-1.4.1/resotoclient/http_client/__init__.py
+-rw-r--r--   0        0        0    12959 2023-05-09 13:17:30.428599 resotoclient-1.4.1/resotoclient/http_client/aiohttp_client.py
+-rw-r--r--   0        0        0     1282 2023-05-09 13:17:30.428599 resotoclient-1.4.1/resotoclient/http_client/event_loop_thread.py
+-rw-r--r--   0        0        0      693 2023-05-09 13:17:30.428599 resotoclient-1.4.1/resotoclient/json_utils.py
+-rw-r--r--   0        0        0     3813 2023-05-09 13:17:30.428599 resotoclient-1.4.1/resotoclient/jwt_utils.py
+-rw-r--r--   0        0        0     2283 2023-05-09 13:17:30.428599 resotoclient-1.4.1/resotoclient/models.py
+-rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 resotoclient-1.4.1/PKG-INFO
```

### Comparing `resotoclient-1.4.0/LICENSE` & `resotoclient-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.0/README.md` & `resotoclient-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.0/pyproject.toml` & `resotoclient-1.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "resotoclient"
-version = "1.4.0"
+version = "1.4.1"
 description = "Resoto Python client library"
 authors = ["Some Engineering Inc."]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/someengineering/resotoclient-python"
 repository = "https://github.com/someengineering/resotoclient-python"
 packages = [
@@ -37,15 +37,15 @@
 python = "^3.9"
 jsons="^1.6.1"
 PyJWT="^2.3.0"
 cryptography=">=36.0.2"
 pandas = { version = "^1.4.2", optional = true }
 graphviz = { version = "^0.20", optional = true }
 aiohttp = "^3.8.1"
-certifi = "^2022.9.24"
+certifi = ">=2017.4.17"
 
 
 [tool.poetry.extras]
 extras = ["pandas", "graphviz"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
```

### Comparing `resotoclient-1.4.0/resotoclient/__init__.py` & `resotoclient-1.4.1/resotoclient/__init__.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.0/resotoclient/async_client.py` & `resotoclient-1.4.1/resotoclient/async_client.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.0/resotoclient/ca.py` & `resotoclient-1.4.1/resotoclient/ca.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.0/resotoclient/http_client/__init__.py` & `resotoclient-1.4.1/resotoclient/http_client/__init__.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.0/resotoclient/http_client/aiohttp_client.py` & `resotoclient-1.4.1/resotoclient/http_client/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.0/resotoclient/http_client/event_loop_thread.py` & `resotoclient-1.4.1/resotoclient/http_client/event_loop_thread.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.0/resotoclient/json_utils.py` & `resotoclient-1.4.1/resotoclient/json_utils.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.0/resotoclient/jwt_utils.py` & `resotoclient-1.4.1/resotoclient/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.0/resotoclient/models.py` & `resotoclient-1.4.1/resotoclient/models.py`

 * *Files identical despite different names*

### Comparing `resotoclient-1.4.0/PKG-INFO` & `resotoclient-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoclient
-Version: 1.4.0
+Version: 1.4.1
 Summary: Resoto Python client library
 Home-page: https://github.com/someengineering/resotoclient-python
 License: Apache-2.0
 Author: Some Engineering Inc.
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Provides-Extra: extras
 Requires-Dist: PyJWT (>=2.3.0,<3.0.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
-Requires-Dist: certifi (>=2022.9.24,<2023.0.0)
+Requires-Dist: certifi (>=2017.4.17)
 Requires-Dist: cryptography (>=36.0.2)
 Requires-Dist: graphviz (>=0.20,<0.21) ; extra == "extras"
 Requires-Dist: jsons (>=1.6.1,<2.0.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0) ; extra == "extras"
 Project-URL: Changelog, https://github.com/someengineering/resotoclient-python/releases
 Project-URL: Repository, https://github.com/someengineering/resotoclient-python
 Description-Content-Type: text/markdown
```

