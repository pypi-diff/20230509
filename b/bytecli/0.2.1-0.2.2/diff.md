# Comparing `tmp/bytecli-0.2.1.tar.gz` & `tmp/bytecli-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytecli-0.2.1.tar", max compression
+gzip compressed data, was "bytecli-0.2.2.tar", max compression
```

## Comparing `bytecli-0.2.1.tar` & `bytecli-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1072 2023-05-09 19:50:24.619093 bytecli-0.2.1/LICENSE
--rw-r--r--   0        0        0      597 2023-05-09 19:50:24.619093 bytecli-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-05-09 19:50:24.619093 bytecli-0.2.1/bytecli/__init__.py
--rw-r--r--   0        0        0     3507 2023-05-09 19:50:24.619093 bytecli-0.2.1/bytecli/main.py
--rw-r--r--   0        0        0      705 2023-05-09 19:50:24.619093 bytecli-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 bytecli-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-09 20:18:41.733312 bytecli-0.2.2/LICENSE
+-rw-r--r--   0        0        0      597 2023-05-09 20:18:41.733312 bytecli-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 20:18:41.733312 bytecli-0.2.2/bytecli/__init__.py
+-rw-r--r--   0        0        0     3507 2023-05-09 20:18:41.733312 bytecli-0.2.2/bytecli/main.py
+-rw-r--r--   0        0        0      933 2023-05-09 20:18:41.733312 bytecli-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 bytecli-0.2.2/PKG-INFO
```

### Comparing `bytecli-0.2.1/LICENSE` & `bytecli-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bytecli-0.2.1/README.md` & `bytecli-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bytecli-0.2.1/bytecli/main.py` & `bytecli-0.2.2/bytecli/main.py`

 * *Files identical despite different names*

### Comparing `bytecli-0.2.1/pyproject.toml` & `bytecli-0.2.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bytecli"
-version = "0.2.1"
+version = "0.2.2"
 description = "Bytesized Hosting CLI app to get information on your App Box"
 authors = ["Allan <allanklp@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bytecli"}]
 homepage = "https://pypi.org/project/bytecli"
 repository = "https://github.com/allankp/bytecli"
@@ -17,15 +17,24 @@
 requests = "^2.28.2"
 rich = "^13.3.4"
 typer = "^0.7.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
+commitizen = "^3.2.1"
+pre-commit = "^3.3.1"
 
 [tool.black]
 line-length = 132
 target-version = ['py310']
 
+[tool.commitizen]
+name = "cz_conventional_commits"
+tag_format = "$version"
+version_type = "pep440"
+version_provider = "poetry"
+update_changelog_on_bump = true
+major_version_zero = true
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `bytecli-0.2.1/PKG-INFO` & `bytecli-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytecli
-Version: 0.2.1
+Version: 0.2.2
 Summary: Bytesized Hosting CLI app to get information on your App Box
 Home-page: https://pypi.org/project/bytecli
 License: MIT
 Author: Allan
 Author-email: allanklp@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

