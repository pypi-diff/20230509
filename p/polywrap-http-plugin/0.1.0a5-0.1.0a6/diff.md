# Comparing `tmp/polywrap_http_plugin-0.1.0a5.tar.gz` & `tmp/polywrap_http_plugin-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_http_plugin-0.1.0a5.tar", max compression
+gzip compressed data, was "polywrap_http_plugin-0.1.0a6.tar", max compression
```

## Comparing `polywrap_http_plugin-0.1.0a5.tar` & `polywrap_http_plugin-0.1.0a6.tar`

### file list

```diff
@@ -1,5 +1,9 @@
--rw-r--r--   0        0        0     1713 2023-04-28 16:11:47.613778 polywrap_http_plugin-0.1.0a5/README.md
--rw-r--r--   0        0        0     3658 2023-04-28 16:11:47.617779 polywrap_http_plugin-0.1.0a5/polywrap_http_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 16:11:47.617779 polywrap_http_plugin-0.1.0a5/polywrap_http_plugin/py.typed
--rw-r--r--   0        0        0     1371 2023-04-28 16:11:47.617779 polywrap_http_plugin-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 polywrap_http_plugin-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1713 2023-05-09 18:15:59.859879 polywrap_http_plugin-0.1.0a6/README.md
+-rw-r--r--   0        0        0     3658 2023-05-09 18:15:59.859879 polywrap_http_plugin-0.1.0a6/polywrap_http_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 18:15:59.859879 polywrap_http_plugin-0.1.0a6/polywrap_http_plugin/py.typed
+-rw-r--r--   0        0        0      163 2023-05-09 18:16:20.636005 polywrap_http_plugin-0.1.0a6/polywrap_http_plugin/wrap/__init__.py
+-rw-r--r--   0        0        0     1322 2023-05-09 18:16:20.636005 polywrap_http_plugin-0.1.0a6/polywrap_http_plugin/wrap/module.py
+-rw-r--r--   0        0        0     1527 2023-05-09 18:16:20.636005 polywrap_http_plugin-0.1.0a6/polywrap_http_plugin/wrap/types.py
+-rw-r--r--   0        0        0     6044 2023-05-09 18:16:20.636005 polywrap_http_plugin-0.1.0a6/polywrap_http_plugin/wrap/wrap_info.py
+-rw-r--r--   0        0        0     1369 2023-05-09 18:15:59.859879 polywrap_http_plugin-0.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 polywrap_http_plugin-0.1.0a6/PKG-INFO
```

### Comparing `polywrap_http_plugin-0.1.0a5/README.md` & `polywrap_http_plugin-0.1.0a6/README.md`

 * *Files identical despite different names*

### Comparing `polywrap_http_plugin-0.1.0a5/polywrap_http_plugin/__init__.py` & `polywrap_http_plugin-0.1.0a6/polywrap_http_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `polywrap_http_plugin-0.1.0a5/pyproject.toml` & `polywrap_http_plugin-0.1.0a6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-http-plugin"
-version = "0.1.0a5"
+version = "0.1.0a6"
 description = ""
 authors = ["Niraj <niraj@polywrap.io>"]
 readme = "README.md"
-packages = [{include = "polywrap_http_plugin"}]
+
+include = ["polywrap_http_plugin/wrap/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 polywrap-plugin = "0.1.0a29"
 httpx = "^0.23.3"
 polywrap-core = "^0.1.0a29"
 polywrap-msgpack = "^0.1.0a29"
```

### Comparing `polywrap_http_plugin-0.1.0a5/PKG-INFO` & `polywrap_http_plugin-0.1.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polywrap-http-plugin
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: 
 Author: Niraj
 Author-email: niraj@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

