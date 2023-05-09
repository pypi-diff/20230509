# Comparing `tmp/SpatialGlue-1.0.0.tar.gz` & `tmp/SpatialGlue-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SpatialGlue-1.0.0.tar", last modified: Mon May  8 07:20:04 2023, max compression
+gzip compressed data, was "dist/SpatialGlue-1.0.1.tar", last modified: Tue May  9 01:34:29 2023, max compression
```

## Comparing `SpatialGlue-1.0.0.tar` & `SpatialGlue-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-08 07:20:04.481053 SpatialGlue-1.0.0/
--rw-rw-r--   0 yahui     (9019) yahui     (1023)    34523 2023-05-08 07:19:17.000000 SpatialGlue-1.0.0/LICENSE.md
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     1006 2023-05-08 07:20:04.477053 SpatialGlue-1.0.0/PKG-INFO
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     1671 2023-05-08 07:19:17.000000 SpatialGlue-1.0.0/README.md
--rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-08 07:19:17.000000 SpatialGlue-1.0.0/README.rst
-drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-08 07:20:04.477053 SpatialGlue-1.0.0/SpatialGlue/
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     6845 2023-05-08 07:19:17.000000 SpatialGlue-1.0.0/SpatialGlue/SpatialGlue.py
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     7620 2023-05-08 07:19:17.000000 SpatialGlue-1.0.0/SpatialGlue/model.py
--rw-rw-r--   0 yahui     (9019) yahui     (1023)    12330 2023-05-08 07:19:17.000000 SpatialGlue-1.0.0/SpatialGlue/preprocess.py
--rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-08 07:19:17.000000 SpatialGlue-1.0.0/SpatialGlue/readme.txt
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     6009 2023-05-08 07:19:17.000000 SpatialGlue-1.0.0/SpatialGlue/utils.py
-drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-08 07:20:04.477053 SpatialGlue-1.0.0/SpatialGlue.egg-info/
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     1006 2023-05-08 07:20:04.000000 SpatialGlue-1.0.0/SpatialGlue.egg-info/PKG-INFO
--rw-rw-r--   0 yahui     (9019) yahui     (1023)      409 2023-05-08 07:20:04.000000 SpatialGlue-1.0.0/SpatialGlue.egg-info/SOURCES.txt
--rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-08 07:20:04.000000 SpatialGlue-1.0.0/SpatialGlue.egg-info/dependency_links.txt
--rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-08 07:20:04.000000 SpatialGlue-1.0.0/SpatialGlue.egg-info/not-zip-safe
--rw-rw-r--   0 yahui     (9019) yahui     (1023)        9 2023-05-08 07:20:04.000000 SpatialGlue-1.0.0/SpatialGlue.egg-info/requires.txt
--rw-rw-r--   0 yahui     (9019) yahui     (1023)       12 2023-05-08 07:20:04.000000 SpatialGlue-1.0.0/SpatialGlue.egg-info/top_level.txt
--rw-rw-r--   0 yahui     (9019) yahui     (1023)   653466 2023-05-08 07:19:17.000000 SpatialGlue-1.0.0/SpatialGlue.png
--rw-rw-r--   0 yahui     (9019) yahui     (1023)      330 2023-05-08 07:19:17.000000 SpatialGlue-1.0.0/__init__.py
-drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-08 07:20:04.477053 SpatialGlue-1.0.0/data/
--rw-rw-r--   0 yahui     (9019) yahui     (1023)      628 2023-05-08 07:19:17.000000 SpatialGlue-1.0.0/data/readme.md
--rw-rw-r--   0 yahui     (9019) yahui     (1023)       38 2023-05-08 07:20:04.481053 SpatialGlue-1.0.0/setup.cfg
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     1685 2023-05-08 07:19:17.000000 SpatialGlue-1.0.0/setup.py
+drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 01:34:29.357978 SpatialGlue-1.0.1/
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)    34523 2023-05-09 01:32:57.000000 SpatialGlue-1.0.1/LICENSE.md
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     1006 2023-05-09 01:34:29.357978 SpatialGlue-1.0.1/PKG-INFO
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     1671 2023-05-09 01:32:57.000000 SpatialGlue-1.0.1/README.md
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 01:32:57.000000 SpatialGlue-1.0.1/README.rst
+drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 01:34:29.353978 SpatialGlue-1.0.1/SpatialGlue/
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     6845 2023-05-09 01:32:57.000000 SpatialGlue-1.0.1/SpatialGlue/SpatialGlue.py
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     7620 2023-05-09 01:32:57.000000 SpatialGlue-1.0.1/SpatialGlue/model.py
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)    12330 2023-05-09 01:32:57.000000 SpatialGlue-1.0.1/SpatialGlue/preprocess.py
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 01:32:57.000000 SpatialGlue-1.0.1/SpatialGlue/readme.txt
+drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 01:34:29.357978 SpatialGlue-1.0.1/SpatialGlue.egg-info/
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     1006 2023-05-09 01:34:29.000000 SpatialGlue-1.0.1/SpatialGlue.egg-info/PKG-INFO
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)      388 2023-05-09 01:34:29.000000 SpatialGlue-1.0.1/SpatialGlue.egg-info/SOURCES.txt
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 01:34:29.000000 SpatialGlue-1.0.1/SpatialGlue.egg-info/dependency_links.txt
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 01:34:29.000000 SpatialGlue-1.0.1/SpatialGlue.egg-info/not-zip-safe
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)        9 2023-05-09 01:34:29.000000 SpatialGlue-1.0.1/SpatialGlue.egg-info/requires.txt
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)       12 2023-05-09 01:34:29.000000 SpatialGlue-1.0.1/SpatialGlue.egg-info/top_level.txt
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)   653466 2023-05-09 01:32:57.000000 SpatialGlue-1.0.1/SpatialGlue.png
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)      330 2023-05-09 01:32:57.000000 SpatialGlue-1.0.1/__init__.py
+drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 01:34:29.357978 SpatialGlue-1.0.1/data/
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)      628 2023-05-09 01:32:57.000000 SpatialGlue-1.0.1/data/readme.md
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)       38 2023-05-09 01:34:29.357978 SpatialGlue-1.0.1/setup.cfg
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     1685 2023-05-09 01:32:57.000000 SpatialGlue-1.0.1/setup.py
```

### Comparing `SpatialGlue-1.0.0/LICENSE.md` & `SpatialGlue-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.0/PKG-INFO` & `SpatialGlue-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpatialGlue
-Version: 1.0.0
+Version: 1.0.1
 Summary: Integrated analysis of spatial multi-omics with SpatialGlue
 Home-page: https://github.com/JinmiaoChenLab/SpatialGlue
 Author: Yahui Long
 Author-email: longyh@immunol.a-star.edu.sg
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `SpatialGlue-1.0.0/README.md` & `SpatialGlue-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.0/SpatialGlue/SpatialGlue.py` & `SpatialGlue-1.0.1/SpatialGlue/SpatialGlue.py`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.0/SpatialGlue/model.py` & `SpatialGlue-1.0.1/SpatialGlue/model.py`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.0/SpatialGlue/preprocess.py` & `SpatialGlue-1.0.1/SpatialGlue/preprocess.py`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.0/SpatialGlue.egg-info/PKG-INFO` & `SpatialGlue-1.0.1/SpatialGlue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpatialGlue
-Version: 1.0.0
+Version: 1.0.1
 Summary: Integrated analysis of spatial multi-omics with SpatialGlue
 Home-page: https://github.com/JinmiaoChenLab/SpatialGlue
 Author: Yahui Long
 Author-email: longyh@immunol.a-star.edu.sg
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `SpatialGlue-1.0.0/SpatialGlue.png` & `SpatialGlue-1.0.1/SpatialGlue.png`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.0/data/readme.md` & `SpatialGlue-1.0.1/data/readme.md`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.0/setup.py` & `SpatialGlue-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import Command, find_packages, setup
 
 __lib_name__ = "SpatialGlue"
-__lib_version__ = "1.0.0"
+__lib_version__ = "1.0.1"
 __description__ = "Integrated analysis of spatial multi-omics with SpatialGlue"
 __url__ = "https://github.com/JinmiaoChenLab/SpatialGlue"
 __author__ = "Yahui Long"
 __author_email__ = "longyh@immunol.a-star.edu.sg"
 __license__ = "MIT"
 __keywords__ = ["Spatial multi-omics", "Cross-omics integration", "Deep learning", "Graph neural networks", "Dual attention"]
 __requires__ = ["requests",]
```

