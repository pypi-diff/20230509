# Comparing `tmp/ediff-0.0.4.tar.gz` & `tmp/ediff-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ediff-0.0.4.tar", last modified: Sat Oct  1 22:22:21 2022, max compression
+gzip compressed data, was "ediff-0.1.0.tar", last modified: Tue May  9 16:20:15 2023, max compression
```

## Comparing `ediff-0.0.4.tar` & `ediff-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-10-01 22:22:21.340240 ediff-0.0.4/
--rw-rw-rw-   0        0        0     1093 2021-12-06 08:05:53.000000 ediff-0.0.4/LICENCE
--rw-rw-rw-   0        0        0     1235 2022-10-01 22:22:21.340240 ediff-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      697 2022-09-30 17:45:30.000000 ediff-0.0.4/README.md
--rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 ediff-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-10-01 22:22:21.340240 ediff-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1258 2021-12-09 19:47:58.000000 ediff-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-01 22:22:21.313465 ediff-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2022-10-01 22:22:21.332662 ediff-0.0.4/src/ediff/
--rw-rw-rw-   0        0        0      173 2022-09-29 14:34:58.000000 ediff-0.0.4/src/ediff/__init__.py
--rw-rw-rw-   0        0        0      888 2022-09-12 12:23:02.000000 ediff-0.0.4/src/ediff/background.py
--rw-rw-rw-   0        0        0      710 2022-08-28 07:50:46.000000 ediff-0.0.4/src/ediff/io.py
--rw-rw-rw-   0        0        0    28913 2022-10-01 22:10:26.000000 ediff-0.0.4/src/ediff/pxrd.py
-drwxrwxrwx   0        0        0        0 2022-10-01 22:22:21.338957 ediff-0.0.4/src/ediff.egg-info/
--rw-rw-rw-   0        0        0     1235 2022-10-01 22:22:21.000000 ediff-0.0.4/src/ediff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2022-10-01 22:22:21.000000 ediff-0.0.4/src/ediff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-01 22:22:21.000000 ediff-0.0.4/src/ediff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-10-01 22:22:21.000000 ediff-0.0.4/src/ediff.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 16:20:15.346619 ediff-0.1.0/
+-rw-rw-rw-   0        0        0     1093 2021-12-06 08:05:54.000000 ediff-0.1.0/LICENCE
+-rw-rw-rw-   0        0        0     2010 2023-05-09 16:20:15.345621 ediff-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1472 2023-05-09 15:48:32.000000 ediff-0.1.0/README.md
+-rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 ediff-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 16:20:15.346619 ediff-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1258 2021-12-09 19:48:00.000000 ediff-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:20:15.308198 ediff-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 16:20:15.337655 ediff-0.1.0/src/ediff/
+-rw-rw-rw-   0        0        0      173 2023-05-09 06:50:36.000000 ediff-0.1.0/src/ediff/__init__.py
+-rw-rw-rw-   0        0        0      888 2022-09-12 12:23:00.000000 ediff-0.1.0/src/ediff/background.py
+-rw-rw-rw-   0        0        0     2570 2023-05-09 07:17:18.000000 ediff-0.1.0/src/ediff/center.py
+-rw-rw-rw-   0        0        0      718 2023-04-21 18:14:14.000000 ediff-0.1.0/src/ediff/io.py
+-rw-rw-rw-   0        0        0    28913 2022-10-01 22:10:28.000000 ediff-0.1.0/src/ediff/pxrd.py
+-rw-rw-rw-   0        0        0     4956 2023-04-21 18:14:46.000000 ediff-0.1.0/src/ediff/radial.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:20:15.344624 ediff-0.1.0/src/ediff.egg-info/
+-rw-rw-rw-   0        0        0     2010 2023-05-09 16:20:15.000000 ediff-0.1.0/src/ediff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-09 16:20:15.000000 ediff-0.1.0/src/ediff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 16:20:15.000000 ediff-0.1.0/src/ediff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-09 16:20:15.000000 ediff-0.1.0/src/ediff.egg-info/top_level.txt
```

### Comparing `ediff-0.0.4/LICENCE` & `ediff-0.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ediff-0.0.4/setup.py` & `ediff-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `ediff-0.0.4/src/ediff/background.py` & `ediff-0.1.0/src/ediff/background.py`

 * *Files identical despite different names*

### Comparing `ediff-0.0.4/src/ediff/io.py` & `ediff-0.1.0/src/ediff/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
-stemdiff.io
------------
+Module ediff.io
+---------------
 Input/output functions for package ediff.    
 '''
 
 import numpy as np
 from PIL import Image
 
 def read_image(image_name, itype='8bit'):
```

### Comparing `ediff-0.0.4/src/ediff/pxrd.py` & `ediff-0.1.0/src/ediff/pxrd.py`

 * *Files identical despite different names*

