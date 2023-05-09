# Comparing `tmp/alfred_pyflow-0.4.0.tar.gz` & `tmp/alfred_pyflow-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred_pyflow-0.4.0.tar", max compression
+gzip compressed data, was "alfred_pyflow-0.4.1.tar", max compression
```

## Comparing `alfred_pyflow-0.4.0.tar` & `alfred_pyflow-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       15 2023-05-09 07:14:52.171790 alfred_pyflow-0.4.0/README.md
--rw-r--r--   0        0        0       31 2023-05-09 07:14:52.171790 alfred_pyflow-0.4.0/pyflow/__init__.py
--rw-r--r--   0        0        0      542 2023-05-09 07:14:52.171790 alfred_pyflow-0.4.0/pyflow/cache.py
--rw-r--r--   0        0        0     6609 2023-05-09 07:14:52.171790 alfred_pyflow-0.4.0/pyflow/icon.py
--rw-r--r--   0        0        0     2629 2023-05-09 07:14:52.171790 alfred_pyflow-0.4.0/pyflow/item.py
--rw-r--r--   0        0        0     1303 2023-05-09 07:14:52.171790 alfred_pyflow-0.4.0/pyflow/testing.py
--rw-r--r--   0        0        0     2344 2023-05-09 07:14:52.171790 alfred_pyflow-0.4.0/pyflow/workflow.py
--rw-r--r--   0        0        0      963 2023-05-09 07:14:52.171790 alfred_pyflow-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 alfred_pyflow-0.4.0/setup.py
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 alfred_pyflow-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       15 2023-05-09 07:22:30.973520 alfred_pyflow-0.4.1/README.md
+-rw-r--r--   0        0        0       31 2023-05-09 07:22:30.973520 alfred_pyflow-0.4.1/pyflow/__init__.py
+-rw-r--r--   0        0        0      542 2023-05-09 07:22:30.973520 alfred_pyflow-0.4.1/pyflow/cache.py
+-rw-r--r--   0        0        0     6609 2023-05-09 07:22:30.973520 alfred_pyflow-0.4.1/pyflow/icon.py
+-rw-r--r--   0        0        0     2629 2023-05-09 07:22:30.973520 alfred_pyflow-0.4.1/pyflow/item.py
+-rw-r--r--   0        0        0     1303 2023-05-09 07:22:30.973520 alfred_pyflow-0.4.1/pyflow/testing.py
+-rw-r--r--   0        0        0     2344 2023-05-09 07:22:30.973520 alfred_pyflow-0.4.1/pyflow/workflow.py
+-rw-r--r--   0        0        0      982 2023-05-09 07:22:30.973520 alfred_pyflow-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      728 1970-01-01 00:00:00.000000 alfred_pyflow-0.4.1/setup.py
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 alfred_pyflow-0.4.1/PKG-INFO
```

### Comparing `alfred_pyflow-0.4.0/pyflow/cache.py` & `alfred_pyflow-0.4.1/pyflow/cache.py`

 * *Files identical despite different names*

### Comparing `alfred_pyflow-0.4.0/pyflow/icon.py` & `alfred_pyflow-0.4.1/pyflow/icon.py`

 * *Files identical despite different names*

### Comparing `alfred_pyflow-0.4.0/pyflow/item.py` & `alfred_pyflow-0.4.1/pyflow/item.py`

 * *Files identical despite different names*

### Comparing `alfred_pyflow-0.4.0/pyflow/testing.py` & `alfred_pyflow-0.4.1/pyflow/testing.py`

 * *Files identical despite different names*

### Comparing `alfred_pyflow-0.4.0/pyflow/workflow.py` & `alfred_pyflow-0.4.1/pyflow/workflow.py`

 * *Files identical despite different names*

### Comparing `alfred_pyflow-0.4.0/pyproject.toml` & `alfred_pyflow-0.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "alfred-pyflow"
 description = "Minimal library for the development of Alfred Workflows."
 documentation = "https://github.com/fedecalendino/alfred-pyflow/blob/main/README.md"
 homepage = "https://github.com/fedecalendino/alfred-pyflow"
 license = "MIT"
 readme = "README.md"
-version = "0.4.0"
+version = "0.4.1"
 
 authors = [
   "Fede Calendino <fede@calendino.com>",
 ]
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
@@ -25,14 +25,15 @@
 packages = [
   { include = "pyflow" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.30.0"
+urllib3 = "1.26.6"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 ddt = "^1.6.0"
 coverage = "^7.2.5"
 
 [build-system]
```

### Comparing `alfred_pyflow-0.4.0/setup.py` & `alfred_pyflow-0.4.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['pyflow']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['requests>=2.30.0,<3.0.0']
+['requests>=2.30.0,<3.0.0', 'urllib3==1.26.6']
 
 setup_kwargs = {
     'name': 'alfred-pyflow',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'Minimal library for the development of Alfred Workflows.',
     'long_description': '# alfred-pyflow',
     'author': 'Fede Calendino',
     'author_email': 'fede@calendino.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fedecalendino/alfred-pyflow',
```

### Comparing `alfred_pyflow-0.4.0/PKG-INFO` & `alfred_pyflow-0.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred-pyflow
-Version: 0.4.0
+Version: 0.4.1
 Summary: Minimal library for the development of Alfred Workflows.
 Home-page: https://github.com/fedecalendino/alfred-pyflow
 License: MIT
 Keywords: alfred,workflow
 Author: Fede Calendino
 Author-email: fede@calendino.com
 Requires-Python: >=3.8,<4.0
@@ -16,11 +16,12 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: urllib3 (==1.26.6)
 Project-URL: Documentation, https://github.com/fedecalendino/alfred-pyflow/blob/main/README.md
 Description-Content-Type: text/markdown
 
 # alfred-pyflow
```

