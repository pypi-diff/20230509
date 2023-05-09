# Comparing `tmp/greenlab-0.0.1.tar.gz` & `tmp/greenlab-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greenlab-0.0.1.tar", last modified: Tue May  9 00:31:42 2023, max compression
+gzip compressed data, was "greenlab-0.0.2.tar", last modified: Tue May  9 04:24:52 2023, max compression
```

## Comparing `greenlab-0.0.1.tar` & `greenlab-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-05-09 00:31:42.406347 greenlab-0.0.1/
--rw-rw-r--   0 max       (1000) max       (1000)     1073 2023-05-09 00:21:58.000000 greenlab-0.0.1/LICENSE
--rw-rw-r--   0 max       (1000) max       (1000)      667 2023-05-09 00:31:42.406347 greenlab-0.0.1/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)      170 2023-05-09 00:22:25.000000 greenlab-0.0.1/README.md
--rw-rw-r--   0 max       (1000) max       (1000)      569 2023-05-09 00:30:53.000000 greenlab-0.0.1/pyproject.toml
--rw-rw-r--   0 max       (1000) max       (1000)       38 2023-05-09 00:31:42.406347 greenlab-0.0.1/setup.cfg
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-05-09 00:31:42.406347 greenlab-0.0.1/src/
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-05-09 00:31:42.406347 greenlab-0.0.1/src/greenlab/
--rw-rw-r--   0 max       (1000) max       (1000)        0 2023-05-08 23:35:32.000000 greenlab-0.0.1/src/greenlab/__init_.py
--rw-rw-r--   0 max       (1000) max       (1000)        0 2023-05-08 23:35:37.000000 greenlab-0.0.1/src/greenlab/example.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-05-09 00:31:42.406347 greenlab-0.0.1/src/greenlab.egg-info/
--rw-rw-r--   0 max       (1000) max       (1000)      667 2023-05-09 00:31:42.000000 greenlab-0.0.1/src/greenlab.egg-info/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)      224 2023-05-09 00:31:42.000000 greenlab-0.0.1/src/greenlab.egg-info/SOURCES.txt
--rw-rw-r--   0 max       (1000) max       (1000)        1 2023-05-09 00:31:42.000000 greenlab-0.0.1/src/greenlab.egg-info/dependency_links.txt
--rw-rw-r--   0 max       (1000) max       (1000)        9 2023-05-09 00:31:42.000000 greenlab-0.0.1/src/greenlab.egg-info/top_level.txt
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-05-09 04:24:52.521800 greenlab-0.0.2/
+-rw-rw-r--   0 max       (1000) max       (1000)     1073 2023-05-09 00:21:58.000000 greenlab-0.0.2/LICENSE
+-rw-rw-r--   0 max       (1000) max       (1000)      667 2023-05-09 04:24:52.521800 greenlab-0.0.2/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)      170 2023-05-09 00:22:25.000000 greenlab-0.0.2/README.md
+-rw-rw-r--   0 max       (1000) max       (1000)      569 2023-05-09 04:24:41.000000 greenlab-0.0.2/pyproject.toml
+-rw-rw-r--   0 max       (1000) max       (1000)       38 2023-05-09 04:24:52.521800 greenlab-0.0.2/setup.cfg
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-05-09 04:24:52.521800 greenlab-0.0.2/src/
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-05-09 04:24:52.521800 greenlab-0.0.2/src/greenlab/
+-rw-rw-r--   0 max       (1000) max       (1000)        0 2023-05-08 23:35:32.000000 greenlab-0.0.2/src/greenlab/__init_.py
+-rw-rw-r--   0 max       (1000) max       (1000)       42 2023-05-09 04:22:16.000000 greenlab-0.0.2/src/greenlab/example.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-05-09 04:24:52.521800 greenlab-0.0.2/src/greenlab.egg-info/
+-rw-rw-r--   0 max       (1000) max       (1000)      667 2023-05-09 04:24:52.000000 greenlab-0.0.2/src/greenlab.egg-info/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)      224 2023-05-09 04:24:52.000000 greenlab-0.0.2/src/greenlab.egg-info/SOURCES.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        1 2023-05-09 04:24:52.000000 greenlab-0.0.2/src/greenlab.egg-info/dependency_links.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        9 2023-05-09 04:24:52.000000 greenlab-0.0.2/src/greenlab.egg-info/top_level.txt
```

### Comparing `greenlab-0.0.1/LICENSE` & `greenlab-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `greenlab-0.0.1/PKG-INFO` & `greenlab-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greenlab
-Version: 0.0.1
+Version: 0.0.2
 Summary: Green Learning Library
 Author-email: Hong-Shuo Chen <hongshuo@usc.edu>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `greenlab-0.0.1/pyproject.toml` & `greenlab-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "greenlab"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Hong-Shuo Chen", email="hongshuo@usc.edu" },
 ]
 description = "Green Learning Library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `greenlab-0.0.1/src/greenlab.egg-info/PKG-INFO` & `greenlab-0.0.2/src/greenlab.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greenlab
-Version: 0.0.1
+Version: 0.0.2
 Summary: Green Learning Library
 Author-email: Hong-Shuo Chen <hongshuo@usc.edu>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

