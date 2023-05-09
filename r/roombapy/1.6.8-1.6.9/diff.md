# Comparing `tmp/roombapy-1.6.8.tar.gz` & `tmp/roombapy-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roombapy-1.6.8.tar", max compression
+gzip compressed data, was "roombapy-1.6.9.tar", max compression
```

## Comparing `roombapy-1.6.8.tar` & `roombapy-1.6.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2023-04-07 10:09:20.211472 roombapy-1.6.8/LICENSE
--rwxr-xr-x   0        0        0     1300 2023-04-07 10:09:20.211472 roombapy-1.6.8/README.md
--rw-r--r--   0        0        0     1040 2023-04-07 10:09:20.211472 roombapy-1.6.8/pyproject.toml
--rw-r--r--   0        0        0      252 2023-04-07 10:09:20.211472 roombapy-1.6.8/roombapy/__init__.py
--rw-r--r--   0        0        0     4258 2023-04-07 10:09:20.211472 roombapy-1.6.8/roombapy/const.py
--rw-r--r--   0        0        0     3165 2023-04-07 10:09:20.211472 roombapy-1.6.8/roombapy/discovery.py
--rw-r--r--   0        0        0     2121 2023-04-07 10:09:20.211472 roombapy-1.6.8/roombapy/entry_points.py
--rw-r--r--   0        0        0     2466 2023-04-07 10:09:20.211472 roombapy-1.6.8/roombapy/getpassword.py
--rw-r--r--   0        0        0     4591 2023-04-07 10:09:20.215473 roombapy-1.6.8/roombapy/remote_client.py
--rwxr-xr-x   0        0        0    17743 2023-04-07 10:09:20.215473 roombapy-1.6.8/roombapy/roomba.py
--rw-r--r--   0        0        0      637 2023-04-07 10:09:20.215473 roombapy-1.6.8/roombapy/roomba_factory.py
--rw-r--r--   0        0        0     1061 2023-04-07 10:09:20.215473 roombapy-1.6.8/roombapy/roomba_info.py
--rw-r--r--   0        0        0     2315 1970-01-01 00:00:00.000000 roombapy-1.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-09 20:17:35.256978 roombapy-1.6.9/LICENSE
+-rwxr-xr-x   0        0        0     1389 2023-05-09 20:17:35.256978 roombapy-1.6.9/README.md
+-rw-r--r--   0        0        0     1040 2023-05-09 20:17:35.256978 roombapy-1.6.9/pyproject.toml
+-rw-r--r--   0        0        0      252 2023-05-09 20:17:35.256978 roombapy-1.6.9/roombapy/__init__.py
+-rw-r--r--   0        0        0     4258 2023-05-09 20:17:35.256978 roombapy-1.6.9/roombapy/const.py
+-rw-r--r--   0        0        0     3165 2023-05-09 20:17:35.256978 roombapy-1.6.9/roombapy/discovery.py
+-rw-r--r--   0        0        0     2121 2023-05-09 20:17:35.256978 roombapy-1.6.9/roombapy/entry_points.py
+-rw-r--r--   0        0        0     2466 2023-05-09 20:17:35.256978 roombapy-1.6.9/roombapy/getpassword.py
+-rw-r--r--   0        0        0     4735 2023-05-09 20:17:35.256978 roombapy-1.6.9/roombapy/remote_client.py
+-rwxr-xr-x   0        0        0    17743 2023-05-09 20:17:35.256978 roombapy-1.6.9/roombapy/roomba.py
+-rw-r--r--   0        0        0      637 2023-05-09 20:17:35.256978 roombapy-1.6.9/roombapy/roomba_factory.py
+-rw-r--r--   0        0        0     1061 2023-05-09 20:17:35.256978 roombapy-1.6.9/roombapy/roomba_info.py
+-rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 roombapy-1.6.9/PKG-INFO
```

### Comparing `roombapy-1.6.8/LICENSE` & `roombapy-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `roombapy-1.6.8/README.md` & `roombapy-1.6.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # roombapy
 
 [![CI](https://github.com/pschmitt/roombapy/actions/workflows/ci.yaml/badge.svg)](https://github.com/pschmitt/roombapy/actions/workflows/ci.yaml)
-![PyPI](https://img.shields.io/pypi/v/roombapy)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/roombapy)
-![PyPI - License](https://img.shields.io/pypi/l/roombapy)
+[![PyPI](https://img.shields.io/pypi/v/roombapy)](https://pypi.org/project/roombapy/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/roombapy)](https://pypi.org/project/roombapy/)
+[![PyPI - License](https://img.shields.io/pypi/l/roombapy)](./LICENSE)
 
 Unofficial iRobot Roomba python library (SDK).
 
 Fork of [NickWaterton/Roomba980-Python](https://github.com/NickWaterton/Roomba980-Python)
 
 This library was created for the [Home Assistant Roomba integration](https://www.home-assistant.io/integrations/roomba/).
```

### Comparing `roombapy-1.6.8/pyproject.toml` & `roombapy-1.6.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "roombapy"
-version = "1.6.8"
+version = "1.6.9"
 description = "Python program and library to control Wi-Fi enabled iRobot Roombas"
 authors = ["Philipp Schmitt <philipp@schmitt.co>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/pschmitt/roombapy"
 classifiers = [
     "Topic :: Software Development",
@@ -21,15 +21,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 paho-mqtt = "^1.5.1"
 orjson = ">=3.8.7"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.2"
+pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 black = "^23.3"
 isort = "^5.11.5"
 flake8 = "^5.0.4"
 amqtt = "^0.10.1"
 
 [build-system]
```

### Comparing `roombapy-1.6.8/roombapy/const.py` & `roombapy-1.6.9/roombapy/const.py`

 * *Files identical despite different names*

### Comparing `roombapy-1.6.8/roombapy/discovery.py` & `roombapy-1.6.9/roombapy/discovery.py`

 * *Files identical despite different names*

### Comparing `roombapy-1.6.8/roombapy/entry_points.py` & `roombapy-1.6.9/roombapy/entry_points.py`

 * *Files identical despite different names*

### Comparing `roombapy-1.6.8/roombapy/getpassword.py` & `roombapy-1.6.9/roombapy/getpassword.py`

 * *Files identical despite different names*

### Comparing `roombapy-1.6.8/roombapy/remote_client.py` & `roombapy-1.6.9/roombapy/remote_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
     We only want to do this once ever because it's expensive.
     """
     ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS)
     ssl_context.verify_mode = ssl.CERT_NONE
     ssl_context.set_ciphers("DEFAULT:!DH")
     ssl_context.load_default_certs()
+    # ssl.OP_LEGACY_SERVER_CONNECT is only available in Python 3.12a4+
+    ssl_context.options |= getattr(ssl, "OP_LEGACY_SERVER_CONNECT", 0x4)
     return ssl_context
 
 
 class RoombaRemoteClient:
     address = None
     port = None
     blid = None
```

### Comparing `roombapy-1.6.8/roombapy/roomba.py` & `roombapy-1.6.9/roombapy/roomba.py`

 * *Files identical despite different names*

### Comparing `roombapy-1.6.8/roombapy/roomba_factory.py` & `roombapy-1.6.9/roombapy/roomba_factory.py`

 * *Files identical despite different names*

### Comparing `roombapy-1.6.8/roombapy/roomba_info.py` & `roombapy-1.6.9/roombapy/roomba_info.py`

 * *Files identical despite different names*

### Comparing `roombapy-1.6.8/PKG-INFO` & `roombapy-1.6.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roombapy
-Version: 1.6.8
+Version: 1.6.9
 Summary: Python program and library to control Wi-Fi enabled iRobot Roombas
 Home-page: https://github.com/pschmitt/roombapy
 License: MIT
 Author: Philipp Schmitt
 Author-email: philipp@schmitt.co
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -22,17 +22,17 @@
 Requires-Dist: paho-mqtt (>=1.5.1,<2.0.0)
 Project-URL: Repository, https://github.com/pschmitt/roombapy
 Description-Content-Type: text/markdown
 
 # roombapy
 
 [![CI](https://github.com/pschmitt/roombapy/actions/workflows/ci.yaml/badge.svg)](https://github.com/pschmitt/roombapy/actions/workflows/ci.yaml)
-![PyPI](https://img.shields.io/pypi/v/roombapy)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/roombapy)
-![PyPI - License](https://img.shields.io/pypi/l/roombapy)
+[![PyPI](https://img.shields.io/pypi/v/roombapy)](https://pypi.org/project/roombapy/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/roombapy)](https://pypi.org/project/roombapy/)
+[![PyPI - License](https://img.shields.io/pypi/l/roombapy)](./LICENSE)
 
 Unofficial iRobot Roomba python library (SDK).
 
 Fork of [NickWaterton/Roomba980-Python](https://github.com/NickWaterton/Roomba980-Python)
 
 This library was created for the [Home Assistant Roomba integration](https://www.home-assistant.io/integrations/roomba/).
```

