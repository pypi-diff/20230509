# Comparing `tmp/CalSciPy-0.2.4.tar.gz` & `tmp/CalSciPy-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CalSciPy-0.2.4.tar", last modified: Wed May  3 20:02:40 2023, max compression
+gzip compressed data, was "CalSciPy-0.2.5.tar", last modified: Tue May  9 19:36:55 2023, max compression
```

## Comparing `CalSciPy-0.2.4.tar` & `CalSciPy-0.2.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 20:02:40.139025 CalSciPy-0.2.4/
--rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     4998 2023-05-03 20:02:40.138025 CalSciPy-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     2840 2023-04-03 15:47:56.000000 CalSciPy-0.2.4/README.md
--rw-rw-rw-   0        0        0     2330 2023-05-03 20:02:03.000000 CalSciPy-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 20:02:40.139025 CalSciPy-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-03 20:02:40.072024 CalSciPy-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 20:02:40.108025 CalSciPy-0.2.4/src/CalSciPy/
--rw-rw-rw-   0        0        0      388 2023-04-03 13:04:29.000000 CalSciPy-0.2.4/src/CalSciPy/__init__.py
--rw-rw-rw-   0        0        0    11403 2023-04-05 15:38:36.000000 CalSciPy-0.2.4/src/CalSciPy/bruker.py
--rw-rw-rw-   0        0        0     3060 2023-05-03 19:59:44.000000 CalSciPy-0.2.4/src/CalSciPy/coloring.py
--rw-rw-rw-   0        0        0     2237 2023-04-03 13:04:29.000000 CalSciPy-0.2.4/src/CalSciPy/event_processing.py
--rw-rw-rw-   0        0        0     4621 2023-05-03 19:58:49.000000 CalSciPy-0.2.4/src/CalSciPy/image_processing.py
--rw-rw-rw-   0        0        0     5914 2023-05-03 20:01:36.000000 CalSciPy-0.2.4/src/CalSciPy/interactive_visuals.py
--rw-rw-rw-   0        0        0     9653 2023-04-26 15:19:07.000000 CalSciPy-0.2.4/src/CalSciPy/io_tools.py
--rw-rw-rw-   0        0        0     7557 2023-05-03 19:58:49.000000 CalSciPy-0.2.4/src/CalSciPy/misc.py
--rw-rw-rw-   0        0        0     3444 2023-03-29 17:06:08.000000 CalSciPy-0.2.4/src/CalSciPy/reorganization.py
--rw-rw-rw-   0        0        0    10343 2023-05-03 20:01:23.000000 CalSciPy-0.2.4/src/CalSciPy/trace_processing.py
--rw-rw-rw-   0        0        0      199 2023-02-20 22:24:54.000000 CalSciPy-0.2.4/src/CalSciPy/version.py
-drwxrwxrwx   0        0        0        0 2023-05-03 20:02:40.117025 CalSciPy-0.2.4/src/CalSciPy.egg-info/
--rw-rw-rw-   0        0        0     4998 2023-05-03 20:02:40.000000 CalSciPy-0.2.4/src/CalSciPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2023-05-03 20:02:40.000000 CalSciPy-0.2.4/src/CalSciPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 20:02:40.000000 CalSciPy-0.2.4/src/CalSciPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      365 2023-05-03 20:02:40.000000 CalSciPy-0.2.4/src/CalSciPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-03 20:02:40.000000 CalSciPy-0.2.4/src/CalSciPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.2.4/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 20:02:40.136025 CalSciPy-0.2.4/tests/
--rw-rw-rw-   0        0        0     1933 2023-04-03 13:04:29.000000 CalSciPy-0.2.4/tests/test_a_install.py
--rw-rw-rw-   0        0        0     3074 2023-04-05 17:07:30.000000 CalSciPy-0.2.4/tests/test_bruker.py
--rw-rw-rw-   0        0        0      887 2023-04-07 16:44:54.000000 CalSciPy-0.2.4/tests/test_coloring.py
--rw-rw-rw-   0        0        0     1218 2023-04-03 15:39:20.000000 CalSciPy-0.2.4/tests/test_event_processing.py
--rw-rw-rw-   0        0        0    12735 2023-04-05 16:39:27.000000 CalSciPy-0.2.4/tests/test_io_tools.py
--rw-rw-rw-   0        0        0     2373 2023-04-05 15:55:20.000000 CalSciPy-0.2.4/tests/test_misc.py
--rw-rw-rw-   0        0        0     5124 2023-03-29 19:08:15.000000 CalSciPy-0.2.4/tests/test_reorganization.py
--rw-rw-rw-   0        0        0     3250 2023-03-29 21:11:25.000000 CalSciPy-0.2.4/tests/test_trace_processing.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:36:55.825379 CalSciPy-0.2.5/
+-rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     4947 2023-05-09 19:36:55.824382 CalSciPy-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2840 2023-04-03 15:47:56.000000 CalSciPy-0.2.5/README.md
+-rw-rw-rw-   0        0        0     2300 2023-05-09 19:12:27.000000 CalSciPy-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 19:36:55.825379 CalSciPy-0.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 19:36:55.760411 CalSciPy-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 19:36:55.789380 CalSciPy-0.2.5/src/CalSciPy/
+-rw-rw-rw-   0        0        0      388 2023-04-03 13:04:29.000000 CalSciPy-0.2.5/src/CalSciPy/__init__.py
+-rw-rw-rw-   0        0        0    11403 2023-04-05 15:38:36.000000 CalSciPy-0.2.5/src/CalSciPy/bruker.py
+-rw-rw-rw-   0        0        0     3060 2023-05-03 19:59:44.000000 CalSciPy-0.2.5/src/CalSciPy/coloring.py
+-rw-rw-rw-   0        0        0    12779 2023-05-09 19:11:20.000000 CalSciPy-0.2.5/src/CalSciPy/event_processing.py
+-rw-rw-rw-   0        0        0     4621 2023-05-03 19:58:49.000000 CalSciPy-0.2.5/src/CalSciPy/image_processing.py
+-rw-rw-rw-   0        0        0     5914 2023-05-03 20:01:36.000000 CalSciPy-0.2.5/src/CalSciPy/interactive_visuals.py
+-rw-rw-rw-   0        0        0     9653 2023-04-26 15:19:07.000000 CalSciPy-0.2.5/src/CalSciPy/io_tools.py
+-rw-rw-rw-   0        0        0     7557 2023-05-03 19:58:49.000000 CalSciPy-0.2.5/src/CalSciPy/misc.py
+-rw-rw-rw-   0        0        0     3444 2023-03-29 17:06:08.000000 CalSciPy-0.2.5/src/CalSciPy/reorganization.py
+-rw-rw-rw-   0        0        0    10343 2023-05-03 20:01:23.000000 CalSciPy-0.2.5/src/CalSciPy/trace_processing.py
+-rw-rw-rw-   0        0        0      199 2023-02-20 22:24:54.000000 CalSciPy-0.2.5/src/CalSciPy/version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:36:55.802381 CalSciPy-0.2.5/src/CalSciPy.egg-info/
+-rw-rw-rw-   0        0        0     4947 2023-05-09 19:36:55.000000 CalSciPy-0.2.5/src/CalSciPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2023-05-09 19:36:55.000000 CalSciPy-0.2.5/src/CalSciPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 19:36:55.000000 CalSciPy-0.2.5/src/CalSciPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      373 2023-05-09 19:36:55.000000 CalSciPy-0.2.5/src/CalSciPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-09 19:36:55.000000 CalSciPy-0.2.5/src/CalSciPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.2.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:36:55.820379 CalSciPy-0.2.5/tests/
+-rw-rw-rw-   0        0        0     1933 2023-04-03 13:04:29.000000 CalSciPy-0.2.5/tests/test_a_install.py
+-rw-rw-rw-   0        0        0     3074 2023-04-05 17:07:30.000000 CalSciPy-0.2.5/tests/test_bruker.py
+-rw-rw-rw-   0        0        0      887 2023-04-07 16:44:54.000000 CalSciPy-0.2.5/tests/test_coloring.py
+-rw-rw-rw-   0        0        0     1218 2023-04-03 15:39:20.000000 CalSciPy-0.2.5/tests/test_event_processing.py
+-rw-rw-rw-   0        0        0    12735 2023-04-05 16:39:27.000000 CalSciPy-0.2.5/tests/test_io_tools.py
+-rw-rw-rw-   0        0        0     2373 2023-04-05 15:55:20.000000 CalSciPy-0.2.5/tests/test_misc.py
+-rw-rw-rw-   0        0        0     5124 2023-03-29 19:08:15.000000 CalSciPy-0.2.5/tests/test_reorganization.py
+-rw-rw-rw-   0        0        0     3250 2023-03-29 21:11:25.000000 CalSciPy-0.2.5/tests/test_trace_processing.py
```

### Comparing `CalSciPy-0.2.4/LICENSE` & `CalSciPy-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.4/PKG-INFO` & `CalSciPy-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.2.4
+Version: 0.2.5
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
         
@@ -30,15 +30,14 @@
 Project-URL: repository, https://github.com/darikoneil/CalSciPy
 Keywords: CalSciPy,Calcium Imaging
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: gpu
```

### Comparing `CalSciPy-0.2.4/README.md` & `CalSciPy-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.4/pyproject.toml` & `CalSciPy-0.2.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CalSciPy"
-version = "0.2.4"
+version = "0.2.5"
 description = "A collection"
 readme = "README.md"
 requires-python = ">=3.7, <4"
 license = {file = "LICENSE"}
 keywords = ["CalSciPy", "Calcium Imaging"]
 authors = [
   {name = "Darik A. O'Neil"}
@@ -18,29 +18,29 @@
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX",
     "Operating System :: Unix",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 dependencies = [
     "matplotlib",
     "numpy",
     "opencv-python",
     "pillow",
     "PPVD",
     "prettytable",
     "pyside2",
     "seaborn",
+    "sklearn",
     "scipy",
     "tqdm"
 ]
 
 [project.urls]
 documentation = "https://calscipy.readthedocs.io/en/latest/?badge=latest"
 repository = "https://github.com/darikoneil/CalSciPy"
```

### Comparing `CalSciPy-0.2.4/src/CalSciPy/bruker.py` & `CalSciPy-0.2.5/src/CalSciPy/bruker.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.4/src/CalSciPy/coloring.py` & `CalSciPy-0.2.5/src/CalSciPy/coloring.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.4/src/CalSciPy/image_processing.py` & `CalSciPy-0.2.5/src/CalSciPy/image_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.4/src/CalSciPy/interactive_visuals.py` & `CalSciPy-0.2.5/src/CalSciPy/interactive_visuals.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.4/src/CalSciPy/io_tools.py` & `CalSciPy-0.2.5/src/CalSciPy/io_tools.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.4/src/CalSciPy/misc.py` & `CalSciPy-0.2.5/src/CalSciPy/misc.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.4/src/CalSciPy/reorganization.py` & `CalSciPy-0.2.5/src/CalSciPy/reorganization.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.4/src/CalSciPy/trace_processing.py` & `CalSciPy-0.2.5/src/CalSciPy/trace_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.4/src/CalSciPy.egg-info/PKG-INFO` & `CalSciPy-0.2.5/src/CalSciPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.2.4
+Version: 0.2.5
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
         
@@ -30,15 +30,14 @@
 Project-URL: repository, https://github.com/darikoneil/CalSciPy
 Keywords: CalSciPy,Calcium Imaging
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: gpu
```

### Comparing `CalSciPy-0.2.4/src/CalSciPy.egg-info/SOURCES.txt` & `CalSciPy-0.2.5/src/CalSciPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.4/tests/test_a_install.py` & `CalSciPy-0.2.5/tests/test_a_install.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.4/tests/test_bruker.py` & `CalSciPy-0.2.5/tests/test_bruker.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.4/tests/test_coloring.py` & `CalSciPy-0.2.5/tests/test_coloring.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.4/tests/test_event_processing.py` & `CalSciPy-0.2.5/tests/test_event_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.4/tests/test_io_tools.py` & `CalSciPy-0.2.5/tests/test_io_tools.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.4/tests/test_misc.py` & `CalSciPy-0.2.5/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.4/tests/test_reorganization.py` & `CalSciPy-0.2.5/tests/test_reorganization.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.4/tests/test_trace_processing.py` & `CalSciPy-0.2.5/tests/test_trace_processing.py`

 * *Files identical despite different names*

