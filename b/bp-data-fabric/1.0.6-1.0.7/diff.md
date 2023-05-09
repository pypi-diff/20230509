# Comparing `tmp/bp_data_fabric-1.0.6.tar.gz` & `tmp/bp_data_fabric-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_data_fabric-1.0.6.tar", last modified: Thu May  4 10:06:45 2023, max compression
+gzip compressed data, was "bp_data_fabric-1.0.7.tar", last modified: Tue May  9 06:00:48 2023, max compression
```

## Comparing `bp_data_fabric-1.0.6.tar` & `bp_data_fabric-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 10:06:45.243146 bp_data_fabric-1.0.6/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-1.0.6/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-04 10:06:45.242789 bp_data_fabric-1.0.6/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-1.0.6/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 10:06:45.240739 bp_data_fabric-1.0.6/bp_data_fabric.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-04 10:06:45.000000 bp_data_fabric-1.0.6/bp_data_fabric.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      265 2023-05-04 10:06:45.000000 bp_data_fabric-1.0.6/bp_data_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-04 10:06:45.000000 bp_data_fabric-1.0.6/bp_data_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       88 2023-05-04 10:06:45.000000 bp_data_fabric-1.0.6/bp_data_fabric.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-05-04 10:06:45.000000 bp_data_fabric-1.0.6/bp_data_fabric.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 10:06:45.241728 bp_data_fabric-1.0.6/data_fabric/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1158 2023-05-04 10:06:32.000000 bp_data_fabric-1.0.6/data_fabric/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2811 2023-05-04 09:57:35.000000 bp_data_fabric-1.0.6/data_fabric/components.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-04 10:06:45.243270 bp_data_fabric-1.0.6/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      860 2023-05-04 10:06:38.000000 bp_data_fabric-1.0.6/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-09 06:00:48.020829 bp_data_fabric-1.0.7/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-1.0.7/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-09 06:00:48.020302 bp_data_fabric-1.0.7/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-1.0.7/README.md
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-09 06:00:48.015732 bp_data_fabric-1.0.7/bp_data_fabric.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-09 06:00:47.000000 bp_data_fabric-1.0.7/bp_data_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      265 2023-05-09 06:00:47.000000 bp_data_fabric-1.0.7/bp_data_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-09 06:00:47.000000 bp_data_fabric-1.0.7/bp_data_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       88 2023-05-09 06:00:47.000000 bp_data_fabric-1.0.7/bp_data_fabric.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-05-09 06:00:47.000000 bp_data_fabric-1.0.7/bp_data_fabric.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-09 06:00:48.018141 bp_data_fabric-1.0.7/data_fabric/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1158 2023-05-04 10:06:32.000000 bp_data_fabric-1.0.7/data_fabric/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2811 2023-05-04 09:57:35.000000 bp_data_fabric-1.0.7/data_fabric/components.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-09 06:00:48.021016 bp_data_fabric-1.0.7/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      860 2023-05-09 05:59:27.000000 bp_data_fabric-1.0.7/setup.py
```

### Comparing `bp_data_fabric-1.0.6/LICENSE` & `bp_data_fabric-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-1.0.6/data_fabric/__init__.py` & `bp_data_fabric-1.0.7/data_fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-1.0.6/data_fabric/components.py` & `bp_data_fabric-1.0.7/data_fabric/components.py`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-1.0.6/setup.py` & `bp_data_fabric-1.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="bp_data_fabric",
-    version="1.0.6",
+    version="1.0.7",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
     description="",    
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

