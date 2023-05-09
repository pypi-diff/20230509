# Comparing `tmp/jobbergate-core-3.5.0a2.tar.gz` & `tmp/jobbergate_core-3.5.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate-core-3.5.0a2.tar", max compression
+gzip compressed data, was "jobbergate_core-3.5.0a3.tar", max compression
```

## Comparing `jobbergate-core-3.5.0a2.tar` & `jobbergate_core-3.5.0a3.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1082 2023-04-27 21:34:07.112423 jobbergate-core-3.5.0a2/LICENSE
--rw-r--r--   0        0        0      420 2023-04-27 21:34:07.112423 jobbergate-core-3.5.0a2/README.rst
--rw-r--r--   0        0        0      329 2023-04-27 21:34:07.112423 jobbergate-core-3.5.0a2/jobbergate_core/__init__.py
--rw-r--r--   0        0        0      366 2023-04-27 21:34:07.112423 jobbergate-core-3.5.0a2/jobbergate_core/auth/__init__.py
--rw-r--r--   0        0        0      279 2023-04-27 21:34:07.112423 jobbergate-core-3.5.0a2/jobbergate_core/auth/exceptions.py
--rw-r--r--   0        0        0    11813 2023-04-27 21:34:07.112423 jobbergate-core-3.5.0a2/jobbergate_core/auth/handler.py
--rw-r--r--   0        0        0     5534 2023-04-27 21:34:07.112423 jobbergate-core-3.5.0a2/jobbergate_core/auth/token.py
--rw-r--r--   0        0        0      133 2023-04-27 21:34:07.112423 jobbergate-core-3.5.0a2/jobbergate_core/version.py
--rw-r--r--   0        0        0     1769 2023-04-27 21:34:07.112423 jobbergate-core-3.5.0a2/pyproject.toml
--rw-r--r--   0        0        0     1271 2023-04-27 21:34:29.329498 jobbergate-core-3.5.0a2/setup.py
--rw-r--r--   0        0        0     1634 2023-04-27 21:34:29.329962 jobbergate-core-3.5.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-09 14:04:30.141068 jobbergate_core-3.5.0a3/LICENSE
+-rw-r--r--   0        0        0      420 2023-05-09 14:04:30.141068 jobbergate_core-3.5.0a3/README.rst
+-rw-r--r--   0        0        0      329 2023-05-09 14:04:30.141068 jobbergate_core-3.5.0a3/jobbergate_core/__init__.py
+-rw-r--r--   0        0        0      366 2023-05-09 14:04:30.141068 jobbergate_core-3.5.0a3/jobbergate_core/auth/__init__.py
+-rw-r--r--   0        0        0      279 2023-05-09 14:04:30.141068 jobbergate_core-3.5.0a3/jobbergate_core/auth/exceptions.py
+-rw-r--r--   0        0        0    11813 2023-05-09 14:04:30.145068 jobbergate_core-3.5.0a3/jobbergate_core/auth/handler.py
+-rw-r--r--   0        0        0     5534 2023-05-09 14:04:30.145068 jobbergate_core-3.5.0a3/jobbergate_core/auth/token.py
+-rw-r--r--   0        0        0      133 2023-05-09 14:04:30.145068 jobbergate_core-3.5.0a3/jobbergate_core/version.py
+-rw-r--r--   0        0        0     1769 2023-05-09 14:04:30.145068 jobbergate_core-3.5.0a3/pyproject.toml
+-rw-r--r--   0        0        0     1733 1970-01-01 00:00:00.000000 jobbergate_core-3.5.0a3/PKG-INFO
```

### Comparing `jobbergate-core-3.5.0a2/LICENSE` & `jobbergate_core-3.5.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate-core-3.5.0a2/jobbergate_core/auth/handler.py` & `jobbergate_core-3.5.0a3/jobbergate_core/auth/handler.py`

 * *Files identical despite different names*

### Comparing `jobbergate-core-3.5.0a2/jobbergate_core/auth/token.py` & `jobbergate_core-3.5.0a3/jobbergate_core/auth/token.py`

 * *Files identical despite different names*

### Comparing `jobbergate-core-3.5.0a2/pyproject.toml` & `jobbergate_core-3.5.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-core"
-version = "3.5.0-alpha.2"
+version = "3.5.0-alpha.3"
 description = "Jobbergate Core"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `jobbergate-core-3.5.0a2/PKG-INFO` & `jobbergate_core-3.5.0a3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: jobbergate-core
-Version: 3.5.0a2
+Version: 3.5.0a3
 Summary: Jobbergate Core
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: httpx (>=0.22.0,<0.23.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: py-buzz (>=3.1.0,<4.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
```

