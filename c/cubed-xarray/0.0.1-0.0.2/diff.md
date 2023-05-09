# Comparing `tmp/cubed-xarray-0.0.1.tar.gz` & `tmp/cubed-xarray-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubed-xarray-0.0.1.tar", last modified: Tue May  9 15:39:01 2023, max compression
+gzip compressed data, was "cubed-xarray-0.0.2.tar", last modified: Tue May  9 16:06:13 2023, max compression
```

## Comparing `cubed-xarray-0.0.1.tar` & `cubed-xarray-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-05-09 15:39:01.067148 cubed-xarray-0.0.1/
--rw-rw-r--   0 tom       (1001) tom       (1001)     1799 2023-03-24 16:03:06.000000 cubed-xarray-0.0.1/.gitignore
--rw-rw-r--   0 tom       (1001) tom       (1001)    11357 2023-03-24 16:03:06.000000 cubed-xarray-0.0.1/LICENSE
--rw-rw-r--   0 tom       (1001) tom       (1001)     2334 2023-05-09 15:39:01.067148 cubed-xarray-0.0.1/PKG-INFO
--rw-rw-r--   0 tom       (1001) tom       (1001)     1342 2023-05-05 20:01:03.000000 cubed-xarray-0.0.1/README.md
-drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-05-09 15:39:01.067148 cubed-xarray-0.0.1/cubed_xarray/
--rw-rw-r--   0 tom       (1001) tom       (1001)      243 2023-04-06 18:08:26.000000 cubed-xarray-0.0.1/cubed_xarray/__init__.py
--rw-rw-r--   0 tom       (1001) tom       (1001)     5641 2023-05-08 19:56:58.000000 cubed-xarray-0.0.1/cubed_xarray/cubedmanager.py
-drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-05-09 15:39:01.067148 cubed-xarray-0.0.1/cubed_xarray/tests/
--rw-rw-r--   0 tom       (1001) tom       (1001)        0 2023-04-06 18:08:26.000000 cubed-xarray-0.0.1/cubed_xarray/tests/__init__.py
--rw-rw-r--   0 tom       (1001) tom       (1001)        0 2023-05-05 21:02:48.000000 cubed-xarray-0.0.1/cubed_xarray/tests/test_wrapping.py
-drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-05-09 15:39:01.067148 cubed-xarray-0.0.1/cubed_xarray.egg-info/
--rw-rw-r--   0 tom       (1001) tom       (1001)     2334 2023-05-09 15:39:01.000000 cubed-xarray-0.0.1/cubed_xarray.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1001) tom       (1001)      418 2023-05-09 15:39:01.000000 cubed-xarray-0.0.1/cubed_xarray.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)        1 2023-05-09 15:39:01.000000 cubed-xarray-0.0.1/cubed_xarray.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)       70 2023-05-09 15:39:01.000000 cubed-xarray-0.0.1/cubed_xarray.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)       40 2023-05-09 15:39:01.000000 cubed-xarray-0.0.1/cubed_xarray.egg-info/requires.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)       13 2023-05-09 15:39:01.000000 cubed-xarray-0.0.1/cubed_xarray.egg-info/top_level.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)     1575 2023-05-09 15:36:05.000000 cubed-xarray-0.0.1/pyproject.toml
--rw-rw-r--   0 tom       (1001) tom       (1001)       44 2023-05-04 22:39:07.000000 cubed-xarray-0.0.1/requirements.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)       38 2023-05-09 15:39:01.067148 cubed-xarray-0.0.1/setup.cfg
--rw-rw-r--   0 tom       (1001) tom       (1001)       93 2023-04-06 18:08:26.000000 cubed-xarray-0.0.1/setup.py
+drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-05-09 16:06:13.729138 cubed-xarray-0.0.2/
+-rw-rw-r--   0 tom       (1001) tom       (1001)     1799 2023-03-24 16:03:06.000000 cubed-xarray-0.0.2/.gitignore
+-rw-rw-r--   0 tom       (1001) tom       (1001)    11357 2023-03-24 16:03:06.000000 cubed-xarray-0.0.2/LICENSE
+-rw-rw-r--   0 tom       (1001) tom       (1001)     2334 2023-05-09 16:06:13.729138 cubed-xarray-0.0.2/PKG-INFO
+-rw-rw-r--   0 tom       (1001) tom       (1001)     1342 2023-05-05 20:01:03.000000 cubed-xarray-0.0.2/README.md
+drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-05-09 16:06:13.725139 cubed-xarray-0.0.2/cubed_xarray/
+-rw-rw-r--   0 tom       (1001) tom       (1001)      243 2023-04-06 18:08:26.000000 cubed-xarray-0.0.2/cubed_xarray/__init__.py
+-rw-rw-r--   0 tom       (1001) tom       (1001)     5641 2023-05-08 19:56:58.000000 cubed-xarray-0.0.2/cubed_xarray/cubedmanager.py
+drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-05-09 16:06:13.729138 cubed-xarray-0.0.2/cubed_xarray/tests/
+-rw-rw-r--   0 tom       (1001) tom       (1001)        0 2023-04-06 18:08:26.000000 cubed-xarray-0.0.2/cubed_xarray/tests/__init__.py
+-rw-rw-r--   0 tom       (1001) tom       (1001)        0 2023-05-05 21:02:48.000000 cubed-xarray-0.0.2/cubed_xarray/tests/test_wrapping.py
+drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-05-09 16:06:13.725139 cubed-xarray-0.0.2/cubed_xarray.egg-info/
+-rw-rw-r--   0 tom       (1001) tom       (1001)     2334 2023-05-09 16:06:13.000000 cubed-xarray-0.0.2/cubed_xarray.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1001) tom       (1001)      418 2023-05-09 16:06:13.000000 cubed-xarray-0.0.2/cubed_xarray.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)        1 2023-05-09 16:06:13.000000 cubed-xarray-0.0.2/cubed_xarray.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)       70 2023-05-09 16:06:13.000000 cubed-xarray-0.0.2/cubed_xarray.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)       40 2023-05-09 16:06:13.000000 cubed-xarray-0.0.2/cubed_xarray.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)       13 2023-05-09 16:06:13.000000 cubed-xarray-0.0.2/cubed_xarray.egg-info/top_level.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)     1575 2023-05-09 15:42:25.000000 cubed-xarray-0.0.2/pyproject.toml
+-rw-rw-r--   0 tom       (1001) tom       (1001)       44 2023-05-04 22:39:07.000000 cubed-xarray-0.0.2/requirements.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)       38 2023-05-09 16:06:13.729138 cubed-xarray-0.0.2/setup.cfg
+-rw-rw-r--   0 tom       (1001) tom       (1001)       93 2023-04-06 18:08:26.000000 cubed-xarray-0.0.2/setup.py
```

### Comparing `cubed-xarray-0.0.1/.gitignore` & `cubed-xarray-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cubed-xarray-0.0.1/LICENSE` & `cubed-xarray-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cubed-xarray-0.0.1/PKG-INFO` & `cubed-xarray-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubed-xarray
-Version: 0.0.1
+Version: 0.0.2
 Summary: Interface for using cubed with xarray for parallel computation.
 Author-email: Tom Nicholas <tomnicholas1@googlemail.com>
 License: Apache-2
 Project-URL: homepage, https://github.com/xarray-contrib/cubed-xarray
 Project-URL: documentation, https://github.com/xarray-contrib/cubed-xarray#readme
 Project-URL: repository, https://github.com/xarray-contrib/cubed-xarray
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cubed-xarray-0.0.1/README.md` & `cubed-xarray-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cubed-xarray-0.0.1/cubed_xarray/cubedmanager.py` & `cubed-xarray-0.0.2/cubed_xarray/cubedmanager.py`

 * *Files identical despite different names*

### Comparing `cubed-xarray-0.0.1/cubed_xarray.egg-info/PKG-INFO` & `cubed-xarray-0.0.2/cubed_xarray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubed-xarray
-Version: 0.0.1
+Version: 0.0.2
 Summary: Interface for using cubed with xarray for parallel computation.
 Author-email: Tom Nicholas <tomnicholas1@googlemail.com>
 License: Apache-2
 Project-URL: homepage, https://github.com/xarray-contrib/cubed-xarray
 Project-URL: documentation, https://github.com/xarray-contrib/cubed-xarray#readme
 Project-URL: repository, https://github.com/xarray-contrib/cubed-xarray
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cubed-xarray-0.0.1/pyproject.toml` & `cubed-xarray-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cubed-xarray"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name = "Tom Nicholas", email = "tomnicholas1@googlemail.com"}
 ]
 description = "Interface for using cubed with xarray for parallel computation."
 license = {text = "Apache-2"}
 readme = "README.md"
 classifiers = [
```

