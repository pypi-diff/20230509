# Comparing `tmp/pytest-httpdbg-0.1.0.tar.gz` & `tmp/pytest-httpdbg-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-httpdbg-0.1.0.tar", last modified: Mon May  8 20:44:32 2023, max compression
+gzip compressed data, was "pytest-httpdbg-0.1.1.tar", last modified: Tue May  9 19:48:27 2023, max compression
```

## Comparing `pytest-httpdbg-0.1.0.tar` & `pytest-httpdbg-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:44:32.051973 pytest-httpdbg-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-05-08 20:44:18.000000 pytest-httpdbg-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-08 20:44:32.051973 pytest-httpdbg-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-08 20:44:18.000000 pytest-httpdbg-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-08 20:44:18.000000 pytest-httpdbg-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:44:32.051973 pytest-httpdbg-0.1.0/pytest_httpdbg/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-08 20:44:18.000000 pytest-httpdbg-0.1.0/pytest_httpdbg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-08 20:44:18.000000 pytest-httpdbg-0.1.0/pytest_httpdbg/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:44:32.051973 pytest-httpdbg-0.1.0/pytest_httpdbg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-08 20:44:32.000000 pytest-httpdbg-0.1.0/pytest_httpdbg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-08 20:44:32.000000 pytest-httpdbg-0.1.0/pytest_httpdbg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:44:32.000000 pytest-httpdbg-0.1.0/pytest_httpdbg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 20:44:32.000000 pytest-httpdbg-0.1.0/pytest_httpdbg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 20:44:32.000000 pytest-httpdbg-0.1.0/pytest_httpdbg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 20:44:32.000000 pytest-httpdbg-0.1.0/pytest_httpdbg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-08 20:44:32.051973 pytest-httpdbg-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:44:32.051973 pytest-httpdbg-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-08 20:44:18.000000 pytest-httpdbg-0.1.0/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:48:27.762827 pytest-httpdbg-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-05-09 19:48:08.000000 pytest-httpdbg-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-09 19:48:27.762827 pytest-httpdbg-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-09 19:48:08.000000 pytest-httpdbg-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-09 19:48:08.000000 pytest-httpdbg-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:48:27.762827 pytest-httpdbg-0.1.1/pytest_httpdbg/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-09 19:48:08.000000 pytest-httpdbg-0.1.1/pytest_httpdbg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-09 19:48:08.000000 pytest-httpdbg-0.1.1/pytest_httpdbg/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:48:27.762827 pytest-httpdbg-0.1.1/pytest_httpdbg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-09 19:48:27.000000 pytest-httpdbg-0.1.1/pytest_httpdbg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-09 19:48:27.000000 pytest-httpdbg-0.1.1/pytest_httpdbg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:48:27.000000 pytest-httpdbg-0.1.1/pytest_httpdbg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-09 19:48:27.000000 pytest-httpdbg-0.1.1/pytest_httpdbg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-09 19:48:27.000000 pytest-httpdbg-0.1.1/pytest_httpdbg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 19:48:27.000000 pytest-httpdbg-0.1.1/pytest_httpdbg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-09 19:48:27.766827 pytest-httpdbg-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:48:27.762827 pytest-httpdbg-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-09 19:48:08.000000 pytest-httpdbg-0.1.1/tests/test_plugin.py
```

### Comparing `pytest-httpdbg-0.1.0/LICENSE` & `pytest-httpdbg-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-httpdbg-0.1.0/PKG-INFO` & `pytest-httpdbg-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: pytest-httpdbg
-Version: 0.1.0
+Version: 0.1.1
 Summary: A pytest plugin to record HTTP(S) requests with stack trace
 Author-email: cle-b <cle@tictac.pm>
 License: Apache-2.0
 Project-URL: repository, https://github.com/cle-b/pytest-httpdbg
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Pytest
-Requires-Python: >=3.6
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytest-httpdbg
 
 A pytest plugin to record HTTP(S) requests with stack trace.
 
+![](ui.png)
+
 ## installation 
 
 ```
 pip install pytest-httpdbg
 ```
 
 ## usage
```

### Comparing `pytest-httpdbg-0.1.0/README.md` & `pytest-httpdbg-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # pytest-httpdbg
 
 A pytest plugin to record HTTP(S) requests with stack trace.
 
+![](ui.png)
+
 ## installation 
 
 ```
 pip install pytest-httpdbg
 ```
 
 ## usage
```

### Comparing `pytest-httpdbg-0.1.0/pyproject.toml` & `pytest-httpdbg-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "pytest-httpdbg"
 authors = [
     {name = "cle-b", email = "cle@tictac.pm"},
 ]
 description="A pytest plugin to record HTTP(S) requests with stack trace"
 readme="README.md"
 urls = {repository = "https://github.com/cle-b/pytest-httpdbg"}
-requires-python = ">=3.6"
+requires-python = ">=3.7.0"
 license = {text = "Apache-2.0"}
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
```

### Comparing `pytest-httpdbg-0.1.0/pytest_httpdbg/plugin.py` & `pytest-httpdbg-0.1.1/pytest_httpdbg/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-httpdbg-0.1.0/pytest_httpdbg.egg-info/PKG-INFO` & `pytest-httpdbg-0.1.1/pytest_httpdbg.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: pytest-httpdbg
-Version: 0.1.0
+Version: 0.1.1
 Summary: A pytest plugin to record HTTP(S) requests with stack trace
 Author-email: cle-b <cle@tictac.pm>
 License: Apache-2.0
 Project-URL: repository, https://github.com/cle-b/pytest-httpdbg
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Pytest
-Requires-Python: >=3.6
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytest-httpdbg
 
 A pytest plugin to record HTTP(S) requests with stack trace.
 
+![](ui.png)
+
 ## installation 
 
 ```
 pip install pytest-httpdbg
 ```
 
 ## usage
```

### Comparing `pytest-httpdbg-0.1.0/tests/test_plugin.py` & `pytest-httpdbg-0.1.1/tests/test_plugin.py`

 * *Files identical despite different names*

