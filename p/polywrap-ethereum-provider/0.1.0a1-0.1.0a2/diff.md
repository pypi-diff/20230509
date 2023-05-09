# Comparing `tmp/polywrap_ethereum_provider-0.1.0a1.tar.gz` & `tmp/polywrap_ethereum_provider-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_ethereum_provider-0.1.0a1.tar", max compression
+gzip compressed data, was "polywrap_ethereum_provider-0.1.0a2.tar", max compression
```

## Comparing `polywrap_ethereum_provider-0.1.0a1.tar` & `polywrap_ethereum_provider-0.1.0a2.tar`

### file list

```diff
@@ -1,7 +1,11 @@
--rw-r--r--   0        0        0     6850 2023-05-02 15:19:25.311865 polywrap_ethereum_provider-0.1.0a1/polywrap_ethereum_provider/__init__.py
--rw-r--r--   0        0        0     1815 2023-05-02 15:19:25.311865 polywrap_ethereum_provider-0.1.0a1/polywrap_ethereum_provider/connection.py
--rw-r--r--   0        0        0     2837 2023-05-02 15:19:25.311865 polywrap_ethereum_provider-0.1.0a1/polywrap_ethereum_provider/connections.py
--rw-r--r--   0        0        0     1451 2023-05-02 15:19:25.311865 polywrap_ethereum_provider-0.1.0a1/polywrap_ethereum_provider/networks.py
--rw-r--r--   0        0        0        0 2023-05-02 15:19:25.311865 polywrap_ethereum_provider-0.1.0a1/polywrap_ethereum_provider/py.typed
--rw-r--r--   0        0        0     1509 2023-05-02 15:19:25.311865 polywrap_ethereum_provider-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 polywrap_ethereum_provider-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     6850 2023-05-09 17:51:20.952227 polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/__init__.py
+-rw-r--r--   0        0        0     1815 2023-05-09 17:51:20.952227 polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/connection.py
+-rw-r--r--   0        0        0     2837 2023-05-09 17:51:20.952227 polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/connections.py
+-rw-r--r--   0        0        0     1451 2023-05-09 17:51:20.952227 polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/networks.py
+-rw-r--r--   0        0        0        0 2023-05-09 17:51:20.952227 polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/py.typed
+-rw-r--r--   0        0        0      163 2023-05-09 17:51:45.292402 polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/wrap/__init__.py
+-rw-r--r--   0        0        0     2637 2023-05-09 17:51:45.292402 polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/wrap/module.py
+-rw-r--r--   0        0        0      843 2023-05-09 17:51:45.292402 polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/wrap/types.py
+-rw-r--r--   0        0        0     5228 2023-05-09 17:51:45.292402 polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/wrap/wrap_info.py
+-rw-r--r--   0        0        0     1561 2023-05-09 17:51:20.952227 polywrap_ethereum_provider-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 polywrap_ethereum_provider-0.1.0a2/PKG-INFO
```

### Comparing `polywrap_ethereum_provider-0.1.0a1/polywrap_ethereum_provider/__init__.py` & `polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0a1/polywrap_ethereum_provider/connection.py` & `polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/connection.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0a1/polywrap_ethereum_provider/connections.py` & `polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/connections.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0a1/polywrap_ethereum_provider/networks.py` & `polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/networks.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0a1/pyproject.toml` & `polywrap_ethereum_provider-0.1.0a2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-ethereum-provider"
-version = "0.1.0a1"
+version = "0.1.0a2"
 description = "Ethereum provider in python"
 authors = ["Cesar <cesar@polywrap.io>"]
 
+include = ["polywrap_ethereum_provider/wrap/**/*"]
+
 [tool.poetry.dependencies]
 python = "^3.10"
 web3 = "6.1.0"
 eth_account = "0.8.0"
 polywrap-plugin = "0.1.0a29"
 polywrap-core = "^0.1.0a29"
 polywrap-msgpack = "^0.1.0a29"
```

### Comparing `polywrap_ethereum_provider-0.1.0a1/PKG-INFO` & `polywrap_ethereum_provider-0.1.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polywrap-ethereum-provider
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Ethereum provider in python
 Author: Cesar
 Author-email: cesar@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

