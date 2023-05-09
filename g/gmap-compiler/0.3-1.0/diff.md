# Comparing `tmp/gmap-compiler-0.3.tar.gz` & `tmp/gmap-compiler-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmap-compiler-0.3.tar", last modified: Fri Apr  7 09:38:02 2023, max compression
+gzip compressed data, was "gmap-compiler-1.0.tar", last modified: Tue May  9 19:40:56 2023, max compression
```

## Comparing `gmap-compiler-0.3.tar` & `gmap-compiler-1.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 jimmy      (501) staff       (20)        0 2023-04-07 09:38:02.621274 gmap-compiler-0.3/
--rw-r--r--   0 jimmy      (501) staff       (20)     1089 2023-03-30 02:05:47.000000 gmap-compiler-0.3/LICENSE
--rw-r--r--   0 jimmy      (501) staff       (20)      331 2023-04-07 09:38:02.620539 gmap-compiler-0.3/PKG-INFO
--rw-r--r--   0 jimmy      (501) staff       (20)     1441 2023-04-06 18:12:23.000000 gmap-compiler-0.3/README.md
-drwxr-xr-x   0 jimmy      (501) staff       (20)        0 2023-04-07 09:38:02.611229 gmap-compiler-0.3/gmap/
--rw-r--r--   0 jimmy      (501) staff       (20)     4738 2023-04-06 17:55:27.000000 gmap-compiler-0.3/gmap/Hardware.py
--rw-r--r--   0 jimmy      (501) staff       (20)        2 2023-03-31 17:03:09.000000 gmap-compiler-0.3/gmap/__init__.py
--rw-r--r--   0 jimmy      (501) staff       (20)     2514 2023-04-06 14:08:17.000000 gmap-compiler-0.3/gmap/mapping.py
--rw-r--r--   0 jimmy      (501) staff       (20)     4805 2023-04-06 14:46:51.000000 gmap-compiler-0.3/gmap/matrix_generator.py
--rw-r--r--   0 jimmy      (501) staff       (20)     2250 2023-03-31 16:18:58.000000 gmap-compiler-0.3/gmap/utils.py
-drwxr-xr-x   0 jimmy      (501) staff       (20)        0 2023-04-07 09:38:02.619707 gmap-compiler-0.3/gmap_compiler.egg-info/
--rw-r--r--   0 jimmy      (501) staff       (20)      331 2023-04-07 09:38:02.000000 gmap-compiler-0.3/gmap_compiler.egg-info/PKG-INFO
--rw-r--r--   0 jimmy      (501) staff       (20)      316 2023-04-07 09:38:02.000000 gmap-compiler-0.3/gmap_compiler.egg-info/SOURCES.txt
--rw-r--r--   0 jimmy      (501) staff       (20)        1 2023-04-07 09:38:02.000000 gmap-compiler-0.3/gmap_compiler.egg-info/dependency_links.txt
--rw-r--r--   0 jimmy      (501) staff       (20)       48 2023-04-07 09:38:02.000000 gmap-compiler-0.3/gmap_compiler.egg-info/requires.txt
--rw-r--r--   0 jimmy      (501) staff       (20)        5 2023-04-07 09:38:02.000000 gmap-compiler-0.3/gmap_compiler.egg-info/top_level.txt
--rw-r--r--   0 jimmy      (501) staff       (20)       38 2023-04-07 09:38:02.621536 gmap-compiler-0.3/setup.cfg
--rw-r--r--   0 jimmy      (501) staff       (20)      602 2023-04-07 09:37:16.000000 gmap-compiler-0.3/setup.py
+drwxr-xr-x   0 jimmyweber   (501) staff       (20)        0 2023-05-09 19:40:56.987720 gmap-compiler-1.0/
+-rw-r--r--   0 jimmyweber   (501) staff       (20)     1089 2023-04-20 10:38:31.000000 gmap-compiler-1.0/LICENSE
+-rw-r--r--   0 jimmyweber   (501) staff       (20)      376 2023-05-09 19:40:56.987629 gmap-compiler-1.0/PKG-INFO
+-rw-r--r--   0 jimmyweber   (501) staff       (20)     3101 2023-05-09 19:38:08.000000 gmap-compiler-1.0/README.md
+drwxr-xr-x   0 jimmyweber   (501) staff       (20)        0 2023-05-09 19:40:56.986264 gmap-compiler-1.0/gmap/
+-rw-r--r--   0 jimmyweber   (501) staff       (20)        2 2023-04-20 10:38:31.000000 gmap-compiler-1.0/gmap/__init__.py
+-rw-r--r--   0 jimmyweber   (501) staff       (20)    13037 2023-05-09 19:18:31.000000 gmap-compiler-1.0/gmap/compiler.py
+-rw-r--r--   0 jimmyweber   (501) staff       (20)     7043 2023-05-09 18:42:11.000000 gmap-compiler-1.0/gmap/hardware.py
+drwxr-xr-x   0 jimmyweber   (501) staff       (20)        0 2023-05-09 19:40:56.986781 gmap-compiler-1.0/gmap/matrix/
+-rw-r--r--   0 jimmyweber   (501) staff       (20)        0 2023-05-09 12:14:59.000000 gmap-compiler-1.0/gmap/matrix/__init__.py
+-rw-r--r--   0 jimmyweber   (501) staff       (20)     9010 2023-05-09 15:41:57.000000 gmap-compiler-1.0/gmap/matrix/generator.py
+-rw-r--r--   0 jimmyweber   (501) staff       (20)     4589 2023-05-09 16:12:51.000000 gmap-compiler-1.0/gmap/matrix/utils.py
+drwxr-xr-x   0 jimmyweber   (501) staff       (20)        0 2023-05-09 19:40:56.987491 gmap-compiler-1.0/gmap_compiler.egg-info/
+-rw-r--r--   0 jimmyweber   (501) staff       (20)      376 2023-05-09 19:40:56.000000 gmap-compiler-1.0/gmap_compiler.egg-info/PKG-INFO
+-rw-r--r--   0 jimmyweber   (501) staff       (20)      331 2023-05-09 19:40:56.000000 gmap-compiler-1.0/gmap_compiler.egg-info/SOURCES.txt
+-rw-r--r--   0 jimmyweber   (501) staff       (20)        1 2023-05-09 19:40:56.000000 gmap-compiler-1.0/gmap_compiler.egg-info/dependency_links.txt
+-rw-r--r--   0 jimmyweber   (501) staff       (20)       48 2023-05-09 19:40:56.000000 gmap-compiler-1.0/gmap_compiler.egg-info/requires.txt
+-rw-r--r--   0 jimmyweber   (501) staff       (20)        5 2023-05-09 19:40:56.000000 gmap-compiler-1.0/gmap_compiler.egg-info/top_level.txt
+-rw-r--r--   0 jimmyweber   (501) staff       (20)       38 2023-05-09 19:40:56.987760 gmap-compiler-1.0/setup.cfg
+-rw-r--r--   0 jimmyweber   (501) staff       (20)      658 2023-05-09 19:40:54.000000 gmap-compiler-1.0/setup.py
```

### Comparing `gmap-compiler-0.3/LICENSE` & `gmap-compiler-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gmap-compiler-0.3/setup.py` & `gmap-compiler-1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gmap-compiler',
-    version='0.3',
+    version='1.0',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'matplotlib',
         'networkx',
         'numba',
         'scipy',
@@ -14,8 +14,9 @@
     ],
     author='Jimmy Weber',
     author_email='jimmy.weber@ini.ethz.ch',
     description='A versatile, easy-to-use and open-source compiler that can efficiently map any arbitrary connectivity matrix to various hardware architectures.',
     url='https://github.com/EIS-Hub/GMap',
 )
 
-# To update the package, run "python setup.py sdist"
+# To update the package, run "python setup.py sdist"
+# twine upload dist/gmap-compiler-0.3.tar.gz --verbose
```

