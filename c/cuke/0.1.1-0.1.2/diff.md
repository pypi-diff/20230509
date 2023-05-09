# Comparing `tmp/cuke-0.1.1.tar.gz` & `tmp/cuke-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuke-0.1.1.tar", max compression
+gzip compressed data, was "cuke-0.1.2.tar", max compression
```

## Comparing `cuke-0.1.1.tar` & `cuke-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       37 2023-05-09 03:30:00.925539 cuke-0.1.1/README.md
--rw-r--r--   0        0        0    12131 2023-05-09 03:30:00.925539 cuke-0.1.1/cuke/__init__.py
--rw-r--r--   0        0        0      655 2023-05-09 03:30:00.925539 cuke-0.1.1/cuke/errors.py
--rw-r--r--   0        0        0     1702 2023-05-09 03:30:00.925539 cuke-0.1.1/cuke/util.py
--rw-r--r--   0        0        0      557 2023-05-09 03:30:00.925539 cuke-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      576 1970-01-01 00:00:00.000000 cuke-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      405 2023-05-09 03:43:27.198481 cuke-0.1.2/README.md
+-rw-r--r--   0        0        0    12131 2023-05-09 03:43:27.198481 cuke-0.1.2/cuke/__init__.py
+-rw-r--r--   0        0        0      655 2023-05-09 03:43:27.198481 cuke-0.1.2/cuke/errors.py
+-rw-r--r--   0        0        0     1702 2023-05-09 03:43:27.198481 cuke-0.1.2/cuke/util.py
+-rw-r--r--   0        0        0      750 2023-05-09 03:43:27.198481 cuke-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1138 1970-01-01 00:00:00.000000 cuke-0.1.2/PKG-INFO
```

### Comparing `cuke-0.1.1/cuke/__init__.py` & `cuke-0.1.2/cuke/__init__.py`

 * *Files identical despite different names*

### Comparing `cuke-0.1.1/cuke/errors.py` & `cuke-0.1.2/cuke/errors.py`

 * *Files identical despite different names*

### Comparing `cuke-0.1.1/cuke/util.py` & `cuke-0.1.2/cuke/util.py`

 * *Files identical despite different names*

### Comparing `cuke-0.1.1/pyproject.toml` & `cuke-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 [tool.poetry]
 name = "cuke"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python client for cuke.cool"
 authors = ["tomgrek <tom.grek@gmail.com>"]
 readme = "README.md"
 packages = [{include = "cuke"}]
+homepage = "https://cuke.cool"
+repository = "https://github.com/tomgrek/cuke.cool"
+documentation = "https://docs.cuke.cool"
+keywords = ["publishing", "faas", "serverless", "webpage", "python"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 typer = {extras = ["all"], version = "^0.7.0"}
 requests = "^2.30.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `cuke-0.1.1/PKG-INFO` & `cuke-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,36 @@
 Metadata-Version: 2.1
 Name: cuke
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python client for cuke.cool
+Home-page: https://cuke.cool
+Keywords: publishing,faas,serverless,webpage,python
 Author: tomgrek
 Author-email: tom.grek@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Project-URL: Documentation, https://docs.cuke.cool
+Project-URL: Repository, https://github.com/tomgrek/cuke.cool
 Description-Content-Type: text/markdown
 
 # Python client library for cuke.cool
+
+This is a Python client library for [cuke.cool](https://cuke.cool).
+
+## Documentation
+
+See the [cuke.cool documentation](https://docs.cuke.cool) for more information.
+
+## Testing
+
+The tests are run as part of the (currently, closed source) cuke.cool CI pipeline.
+
+## Release
+
+* Update version number in pyproject.toml
+* Push to main branch, CICD will publish to PyPI
```

