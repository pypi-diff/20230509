# Comparing `tmp/bytecli-0.2.0.tar.gz` & `tmp/bytecli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytecli-0.2.0.tar", max compression
+gzip compressed data, was "bytecli-0.2.1.tar", max compression
```

## Comparing `bytecli-0.2.0.tar` & `bytecli-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1072 2023-04-25 09:12:39.624516 bytecli-0.2.0/LICENSE
--rw-r--r--   0        0        0      597 2023-04-25 09:12:39.624516 bytecli-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-25 09:12:39.624516 bytecli-0.2.0/bytecli/__init__.py
--rw-r--r--   0        0        0     3507 2023-04-25 09:12:39.624516 bytecli-0.2.0/bytecli/main.py
--rw-r--r--   0        0        0      456 2023-04-25 09:12:39.624516 bytecli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 bytecli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-09 19:50:24.619093 bytecli-0.2.1/LICENSE
+-rw-r--r--   0        0        0      597 2023-05-09 19:50:24.619093 bytecli-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 19:50:24.619093 bytecli-0.2.1/bytecli/__init__.py
+-rw-r--r--   0        0        0     3507 2023-05-09 19:50:24.619093 bytecli-0.2.1/bytecli/main.py
+-rw-r--r--   0        0        0      705 2023-05-09 19:50:24.619093 bytecli-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 bytecli-0.2.1/PKG-INFO
```

### Comparing `bytecli-0.2.0/LICENSE` & `bytecli-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bytecli-0.2.0/README.md` & `bytecli-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bytecli-0.2.0/bytecli/main.py` & `bytecli-0.2.1/bytecli/main.py`

 * *Files identical despite different names*

### Comparing `bytecli-0.2.0/PKG-INFO` & `bytecli-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: bytecli
-Version: 0.2.0
-Summary: 
+Version: 0.2.1
+Summary: Bytesized Hosting CLI app to get information on your App Box
+Home-page: https://pypi.org/project/bytecli
+License: MIT
 Author: Allan
 Author-email: allanklp@gmail.com
 Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: black (>=23.3.0,<24.0.0)
-Requires-Dist: ipdb (>=0.13.13,<0.14.0)
-Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
+Project-URL: Repository, https://github.com/allankp/bytecli
 Description-Content-Type: text/markdown
 
 Bytesized Hosting CLI
 ===============
 
 ![](https://github.com/allankp/bytecli/workflows/main/badge.svg)
 [![PyPI version](https://badge.fury.io/py/bytecli.svg)](https://badge.fury.io/py/bytecli)
```

