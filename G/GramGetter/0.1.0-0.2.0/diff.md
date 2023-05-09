# Comparing `tmp/GramGetter-0.1.0.tar.gz` & `tmp/GramGetter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GramGetter-0.1.0.tar", last modified: Tue May  9 11:49:53 2023, max compression
+gzip compressed data, was "GramGetter-0.2.0.tar", last modified: Tue May  9 12:30:45 2023, max compression
```

## Comparing `GramGetter-0.1.0.tar` & `GramGetter-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 11:49:53.564686 GramGetter-0.1.0/
-drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 11:49:53.564686 GramGetter-0.1.0/GramGetter/
--rw-rw-r--   0 msaid     (1043) msaid     (1044)    14444 2023-05-09 11:27:34.000000 GramGetter-0.1.0/GramGetter/GramGetter.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)       34 2023-05-09 11:24:37.000000 GramGetter-0.1.0/GramGetter/__init__.py
-drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 11:49:53.564686 GramGetter-0.1.0/GramGetter/instaloader/
--rw-rw-r--   0 msaid     (1043) msaid     (1044)      853 2023-05-09 11:27:32.000000 GramGetter-0.1.0/GramGetter/instaloader/__init__.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)    32011 2023-05-09 11:27:32.000000 GramGetter-0.1.0/GramGetter/instaloader/__main__.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)     1611 2023-05-09 11:27:32.000000 GramGetter-0.1.0/GramGetter/instaloader/exceptions.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)    82489 2023-05-09 11:27:32.000000 GramGetter-0.1.0/GramGetter/instaloader/instaloader.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)    38435 2023-05-09 11:27:32.000000 GramGetter-0.1.0/GramGetter/instaloader/instaloadercontext.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)     4934 2023-05-09 11:27:32.000000 GramGetter-0.1.0/GramGetter/instaloader/lateststamps.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)    14877 2023-05-09 11:27:32.000000 GramGetter-0.1.0/GramGetter/instaloader/nodeiterator.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)     1940 2023-05-09 11:27:32.000000 GramGetter-0.1.0/GramGetter/instaloader/sectioniterator.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)    79877 2023-05-09 11:27:32.000000 GramGetter-0.1.0/GramGetter/instaloader/structures.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)      107 2023-05-09 11:27:34.000000 GramGetter-0.1.0/GramGetter/instaloader.py
--rw-rw-r--   0 msaid     (1043) msaid     (1044)     2288 2023-05-09 11:27:36.000000 GramGetter-0.1.0/GramGetter/setup.py
-drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 11:49:53.564686 GramGetter-0.1.0/GramGetter.egg-info/
--rw-r-----   0 msaid     (1043) msaid     (1044)      432 2023-05-09 11:49:53.000000 GramGetter-0.1.0/GramGetter.egg-info/PKG-INFO
--rw-r-----   0 msaid     (1043) msaid     (1044)      625 2023-05-09 11:49:53.000000 GramGetter-0.1.0/GramGetter.egg-info/SOURCES.txt
--rw-r-----   0 msaid     (1043) msaid     (1044)        1 2023-05-09 11:49:53.000000 GramGetter-0.1.0/GramGetter.egg-info/dependency_links.txt
--rw-r-----   0 msaid     (1043) msaid     (1044)       14 2023-05-09 11:49:53.000000 GramGetter-0.1.0/GramGetter.egg-info/requires.txt
--rw-r-----   0 msaid     (1043) msaid     (1044)       11 2023-05-09 11:49:53.000000 GramGetter-0.1.0/GramGetter.egg-info/top_level.txt
--rw-r-----   0 msaid     (1043) msaid     (1044)      432 2023-05-09 11:49:53.564686 GramGetter-0.1.0/PKG-INFO
--rw-rw-r--   0 msaid     (1043) msaid     (1044)        0 2023-05-09 11:33:47.000000 GramGetter-0.1.0/README
--rw-r-----   0 msaid     (1043) msaid     (1044)       38 2023-05-09 11:49:53.564686 GramGetter-0.1.0/setup.cfg
--rw-rw-r--   0 msaid     (1043) msaid     (1044)      656 2023-05-09 11:39:56.000000 GramGetter-0.1.0/setup.py
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 12:30:45.293532 GramGetter-0.2.0/
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 12:30:45.293532 GramGetter-0.2.0/GramGetter/
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    14462 2023-05-09 12:30:13.000000 GramGetter-0.2.0/GramGetter/GramGetter.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)       34 2023-05-09 12:04:03.000000 GramGetter-0.2.0/GramGetter/__init__.py
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 12:30:45.293532 GramGetter-0.2.0/GramGetter/instaloader/
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      853 2023-05-09 11:27:32.000000 GramGetter-0.2.0/GramGetter/instaloader/__init__.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    32011 2023-05-09 11:27:32.000000 GramGetter-0.2.0/GramGetter/instaloader/__main__.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     1611 2023-05-09 11:27:32.000000 GramGetter-0.2.0/GramGetter/instaloader/exceptions.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    82489 2023-05-09 11:27:32.000000 GramGetter-0.2.0/GramGetter/instaloader/instaloader.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    38435 2023-05-09 11:27:32.000000 GramGetter-0.2.0/GramGetter/instaloader/instaloadercontext.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     4934 2023-05-09 11:27:32.000000 GramGetter-0.2.0/GramGetter/instaloader/lateststamps.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    14877 2023-05-09 11:27:32.000000 GramGetter-0.2.0/GramGetter/instaloader/nodeiterator.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     1940 2023-05-09 11:27:32.000000 GramGetter-0.2.0/GramGetter/instaloader/sectioniterator.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)    79877 2023-05-09 11:27:32.000000 GramGetter-0.2.0/GramGetter/instaloader/structures.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      107 2023-05-09 11:27:34.000000 GramGetter-0.2.0/GramGetter/my_instaloader.py
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)     2288 2023-05-09 11:27:36.000000 GramGetter-0.2.0/GramGetter/setup.py
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-05-09 12:30:45.293532 GramGetter-0.2.0/GramGetter.egg-info/
+-rw-r-----   0 msaid     (1043) msaid     (1044)      432 2023-05-09 12:30:45.000000 GramGetter-0.2.0/GramGetter.egg-info/PKG-INFO
+-rw-r-----   0 msaid     (1043) msaid     (1044)      628 2023-05-09 12:30:45.000000 GramGetter-0.2.0/GramGetter.egg-info/SOURCES.txt
+-rw-r-----   0 msaid     (1043) msaid     (1044)        1 2023-05-09 12:30:45.000000 GramGetter-0.2.0/GramGetter.egg-info/dependency_links.txt
+-rw-r-----   0 msaid     (1043) msaid     (1044)       14 2023-05-09 12:30:45.000000 GramGetter-0.2.0/GramGetter.egg-info/requires.txt
+-rw-r-----   0 msaid     (1043) msaid     (1044)       11 2023-05-09 12:30:45.000000 GramGetter-0.2.0/GramGetter.egg-info/top_level.txt
+-rw-r-----   0 msaid     (1043) msaid     (1044)      432 2023-05-09 12:30:45.293532 GramGetter-0.2.0/PKG-INFO
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)        0 2023-05-09 11:33:47.000000 GramGetter-0.2.0/README
+-rw-r-----   0 msaid     (1043) msaid     (1044)       38 2023-05-09 12:30:45.293532 GramGetter-0.2.0/setup.cfg
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)      656 2023-05-09 12:30:41.000000 GramGetter-0.2.0/setup.py
```

### Comparing `GramGetter-0.1.0/GramGetter/GramGetter.py` & `GramGetter-0.2.0/GramGetter/GramGetter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import instaloader
+import my_instaloader as instaloader
 import time
 from datetime import datetime, timedelta
 import warnings
 warnings.filterwarnings("ignore")
 
 class GramGetter:
     def __init__(self, username, cookie_dict):
```

### Comparing `GramGetter-0.1.0/GramGetter/instaloader/__init__.py` & `GramGetter-0.2.0/GramGetter/instaloader/__init__.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.1.0/GramGetter/instaloader/__main__.py` & `GramGetter-0.2.0/GramGetter/instaloader/__main__.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.1.0/GramGetter/instaloader/exceptions.py` & `GramGetter-0.2.0/GramGetter/instaloader/exceptions.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.1.0/GramGetter/instaloader/instaloader.py` & `GramGetter-0.2.0/GramGetter/instaloader/instaloader.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.1.0/GramGetter/instaloader/instaloadercontext.py` & `GramGetter-0.2.0/GramGetter/instaloader/instaloadercontext.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.1.0/GramGetter/instaloader/lateststamps.py` & `GramGetter-0.2.0/GramGetter/instaloader/lateststamps.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.1.0/GramGetter/instaloader/nodeiterator.py` & `GramGetter-0.2.0/GramGetter/instaloader/nodeiterator.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.1.0/GramGetter/instaloader/sectioniterator.py` & `GramGetter-0.2.0/GramGetter/instaloader/sectioniterator.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.1.0/GramGetter/instaloader/structures.py` & `GramGetter-0.2.0/GramGetter/instaloader/structures.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.1.0/GramGetter/setup.py` & `GramGetter-0.2.0/GramGetter/setup.py`

 * *Files identical despite different names*

### Comparing `GramGetter-0.1.0/GramGetter.egg-info/SOURCES.txt` & `GramGetter-0.2.0/GramGetter.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 README
 setup.py
 GramGetter/GramGetter.py
 GramGetter/__init__.py
-GramGetter/instaloader.py
+GramGetter/my_instaloader.py
 GramGetter/setup.py
 GramGetter.egg-info/PKG-INFO
 GramGetter.egg-info/SOURCES.txt
 GramGetter.egg-info/dependency_links.txt
 GramGetter.egg-info/requires.txt
 GramGetter.egg-info/top_level.txt
 GramGetter/instaloader/__init__.py
```

### Comparing `GramGetter-0.1.0/setup.py` & `GramGetter-0.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 requirements = ['requests>=2.4']
 setup(
     name='GramGetter',
-    version='0.1.0',    # Update this for new versions
+    version='0.2.0',    # Update this for new versions
     description='A crawler for scraping instagram content',
     author='Mohamed Amine Said',
     author_email='amine8said@gmail.com',
     url='https://github.com/instaloader/instaloader',
     packages=find_packages(),
     python_requires='>=3.8',
     install_requires=requirements,
```

