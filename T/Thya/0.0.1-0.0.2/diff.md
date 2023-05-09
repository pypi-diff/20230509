# Comparing `tmp/Thya-0.0.1.tar.gz` & `tmp/Thya-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Thya-0.0.1.tar", last modified: Thu May  4 09:02:17 2023, max compression
+gzip compressed data, was "Thya-0.0.2.tar", last modified: Tue May  9 09:12:39 2023, max compression
```

## Comparing `Thya-0.0.1.tar` & `Thya-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:02:17.564226 Thya-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-04 09:02:07.000000 Thya-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-04 09:02:07.000000 Thya-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-04 09:02:17.564226 Thya-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-04 09:02:07.000000 Thya-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:02:17.564226 Thya-0.0.1/Thya.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-04 09:02:17.000000 Thya-0.0.1/Thya.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-04 09:02:17.000000 Thya-0.0.1/Thya.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:02:17.000000 Thya-0.0.1/Thya.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 09:02:17.000000 Thya-0.0.1/Thya.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 09:02:17.000000 Thya-0.0.1/Thya.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 09:02:17.564226 Thya-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-04 09:02:07.000000 Thya-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:02:17.564226 Thya-0.0.1/thya/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-04 09:02:07.000000 Thya-0.0.1/thya/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-04 09:02:07.000000 Thya-0.0.1/thya/apis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:02:17.564226 Thya-0.0.1/thya/data/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 09:02:07.000000 Thya-0.0.1/thya/data/example.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:12:39.668153 Thya-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-09 09:12:30.000000 Thya-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-09 09:12:30.000000 Thya-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-09 09:12:39.668153 Thya-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-09 09:12:30.000000 Thya-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:12:39.668153 Thya-0.0.2/Thya.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-09 09:12:39.000000 Thya-0.0.2/Thya.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-09 09:12:39.000000 Thya-0.0.2/Thya.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:12:39.000000 Thya-0.0.2/Thya.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 09:12:39.000000 Thya-0.0.2/Thya.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 09:12:39.000000 Thya-0.0.2/Thya.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-09 09:12:39.668153 Thya-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-09 09:12:30.000000 Thya-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:12:39.668153 Thya-0.0.2/thya/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-09 09:12:30.000000 Thya-0.0.2/thya/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-09 09:12:30.000000 Thya-0.0.2/thya/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-09 09:12:30.000000 Thya-0.0.2/thya/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:12:39.668153 Thya-0.0.2/thya/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 09:12:30.000000 Thya-0.0.2/thya/data/example.json
```

### Comparing `Thya-0.0.1/LICENSE` & `Thya-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Thya-0.0.1/PKG-INFO` & `Thya-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Thya
-Version: 0.0.1
+Version: 0.0.2
 Summary: ThyaTechnology SDK
 Home-page: https://github.com/ThyaTechnology/thya
 Author: Silvio Giancola
 Author-email: silvio@thya-technology.com
 License: GNU Affero General Public License v3.0
 Keywords: Thya,Technology,SDK,Cloud,Computer Vision,Object Detection,Instance Segmentation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `Thya-0.0.1/Thya.egg-info/PKG-INFO` & `Thya-0.0.2/Thya.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Thya
-Version: 0.0.1
+Version: 0.0.2
 Summary: ThyaTechnology SDK
 Home-page: https://github.com/ThyaTechnology/thya
 Author: Silvio Giancola
 Author-email: silvio@thya-technology.com
 License: GNU Affero General Public License v3.0
 Keywords: Thya,Technology,SDK,Cloud,Computer Vision,Object Detection,Instance Segmentation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `Thya-0.0.1/setup.py` & `Thya-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import sys
 from shutil import rmtree
 from setuptools import setup, find_packages, Command
 
 from thya import __version__, __authors__, __author_email__, __github__
 
-with open('README.md') as readme_file:
+with open('PYPI.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='Thya',         # How you named your package folder (MyLib)
     packages=['thya'],   # Chose the same as "name"
     # Start with a small number and increase it with every change you make
     version=__version__,
@@ -25,15 +25,16 @@
     # download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
     keywords=['Thya', 'Technology', 'SDK', 'Cloud', 'Computer Vision', 'Object Detection', 'Instance Segmentation'],   # Keywords that define your package best
     # package_data={'SoccerNet': [
     #     'SoccerNet/data/*.json', 'SoccerNet/data/SNMOT*.txt']},
     # include_package_data=True,
     install_requires=[
         'requests',
-        # 'tqdm',
+        'tqdm',
+        'xmltodict',
         # 'opencv-python',
         'imagesize'
     ],
     classifiers=[
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Development Status :: 3 - Alpha',
         # Define that your audience are developers
```

### Comparing `Thya-0.0.1/thya/apis.py` & `Thya-0.0.2/thya/apis.py`

 * *Files identical despite different names*

