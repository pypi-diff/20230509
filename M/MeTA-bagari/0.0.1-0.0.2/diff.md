# Comparing `tmp/MeTA_bagari-0.0.1.tar.gz` & `tmp/MeTA_bagari-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MeTA_bagari-0.0.1.tar", last modified: Mon May  8 22:40:30 2023, max compression
+gzip compressed data, was "MeTA_bagari-0.0.2.tar", last modified: Mon May  8 23:04:32 2023, max compression
```

## Comparing `MeTA_bagari-0.0.1.tar` & `MeTA_bagari-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 shayanjavid   (501) staff       (20)        0 2023-05-08 22:40:30.194592 MeTA_bagari-0.0.1/
--rw-r--r--   0 shayanjavid   (501) staff       (20)     1091 2023-05-08 20:47:16.000000 MeTA_bagari-0.0.1/LICENSE
-drwxr-xr-x   0 shayanjavid   (501) staff       (20)        0 2023-05-08 22:40:30.191781 MeTA_bagari-0.0.1/MeTA_bagari.egg-info/
--rw-r--r--   0 shayanjavid   (501) staff       (20)      338 2023-05-08 22:40:30.000000 MeTA_bagari-0.0.1/MeTA_bagari.egg-info/PKG-INFO
--rw-r--r--   0 shayanjavid   (501) staff       (20)      471 2023-05-08 22:40:30.000000 MeTA_bagari-0.0.1/MeTA_bagari.egg-info/SOURCES.txt
--rw-r--r--   0 shayanjavid   (501) staff       (20)        1 2023-05-08 22:40:30.000000 MeTA_bagari-0.0.1/MeTA_bagari.egg-info/dependency_links.txt
--rw-r--r--   0 shayanjavid   (501) staff       (20)      917 2023-05-08 22:40:30.000000 MeTA_bagari-0.0.1/MeTA_bagari.egg-info/requires.txt
--rw-r--r--   0 shayanjavid   (501) staff       (20)        4 2023-05-08 22:40:30.000000 MeTA_bagari-0.0.1/MeTA_bagari.egg-info/top_level.txt
--rw-r--r--   0 shayanjavid   (501) staff       (20)      338 2023-05-08 22:40:30.194689 MeTA_bagari-0.0.1/PKG-INFO
--rw-r--r--   0 shayanjavid   (501) staff       (20)      170 2023-05-08 20:51:52.000000 MeTA_bagari-0.0.1/README.md
--rw-r--r--   0 shayanjavid   (501) staff       (20)       79 2023-05-08 22:40:30.195071 MeTA_bagari-0.0.1/setup.cfg
--rw-r--r--   0 shayanjavid   (501) staff       (20)     1882 2023-05-08 22:39:29.000000 MeTA_bagari-0.0.1/setup.py
-drwxr-xr-x   0 shayanjavid   (501) staff       (20)        0 2023-05-08 22:40:30.189651 MeTA_bagari-0.0.1/src/
-drwxr-xr-x   0 shayanjavid   (501) staff       (20)        0 2023-05-08 22:40:30.194364 MeTA_bagari-0.0.1/src/MeTA/
--rw-rw-r--   0 shayanjavid   (501) staff       (20)    13729 2023-05-08 18:40:58.000000 MeTA_bagari-0.0.1/src/MeTA/Explained_AssignmentVoxelMaps.py
--rw-rw-r--   0 shayanjavid   (501) staff       (20)    28142 2023-05-08 18:40:58.000000 MeTA_bagari-0.0.1/src/MeTA/META_toolkit_v2.py
--rw-r--r--   0 shayanjavid   (501) staff       (20)        0 2023-05-08 20:36:07.000000 MeTA_bagari-0.0.1/src/MeTA/__init__.py
--rw-rw-r--   0 shayanjavid   (501) staff       (20)     3406 2023-05-08 18:40:58.000000 MeTA_bagari-0.0.1/src/MeTA/calculate_stat.py
--rw-rw-r--   0 shayanjavid   (501) staff       (20)     5298 2023-05-08 18:40:58.000000 MeTA_bagari-0.0.1/src/MeTA/create_endpoints_mask_with_clustering.py
--rw-rw-r--   0 shayanjavid   (501) staff       (20)      963 2023-05-08 18:40:58.000000 MeTA_bagari-0.0.1/src/MeTA/read_compressed.py
--rw-rw-r--   0 shayanjavid   (501) staff       (20)     1617 2023-05-08 18:40:58.000000 MeTA_bagari-0.0.1/src/MeTA/tck2trk.py
--rw-rw-r--   0 shayanjavid   (501) staff       (20)      899 2023-05-08 18:40:58.000000 MeTA_bagari-0.0.1/src/MeTA/trk2tck.py
--rw-rw-r--   0 shayanjavid   (501) staff       (20)     3609 2023-05-08 18:40:58.000000 MeTA_bagari-0.0.1/src/MeTA/trk_2_binary.py
+drwxr-xr-x   0 shayanjavid   (501) staff       (20)        0 2023-05-08 23:04:32.058920 MeTA_bagari-0.0.2/
+-rw-r--r--   0 shayanjavid   (501) staff       (20)     1091 2023-05-08 20:47:16.000000 MeTA_bagari-0.0.2/LICENSE
+drwxr-xr-x   0 shayanjavid   (501) staff       (20)        0 2023-05-08 23:04:32.055390 MeTA_bagari-0.0.2/MeTA_bagari.egg-info/
+-rw-r--r--   0 shayanjavid   (501) staff       (20)      338 2023-05-08 23:04:32.000000 MeTA_bagari-0.0.2/MeTA_bagari.egg-info/PKG-INFO
+-rw-r--r--   0 shayanjavid   (501) staff       (20)      487 2023-05-08 23:04:32.000000 MeTA_bagari-0.0.2/MeTA_bagari.egg-info/SOURCES.txt
+-rw-r--r--   0 shayanjavid   (501) staff       (20)        1 2023-05-08 23:04:32.000000 MeTA_bagari-0.0.2/MeTA_bagari.egg-info/dependency_links.txt
+-rw-r--r--   0 shayanjavid   (501) staff       (20)      917 2023-05-08 23:04:32.000000 MeTA_bagari-0.0.2/MeTA_bagari.egg-info/requires.txt
+-rw-r--r--   0 shayanjavid   (501) staff       (20)        4 2023-05-08 23:04:32.000000 MeTA_bagari-0.0.2/MeTA_bagari.egg-info/top_level.txt
+-rw-r--r--   0 shayanjavid   (501) staff       (20)      338 2023-05-08 23:04:32.059138 MeTA_bagari-0.0.2/PKG-INFO
+-rw-r--r--   0 shayanjavid   (501) staff       (20)      170 2023-05-08 20:51:52.000000 MeTA_bagari-0.0.2/README.md
+-rw-r--r--   0 shayanjavid   (501) staff       (20)       79 2023-05-08 23:04:32.059714 MeTA_bagari-0.0.2/setup.cfg
+-rw-r--r--   0 shayanjavid   (501) staff       (20)     1882 2023-05-08 23:03:46.000000 MeTA_bagari-0.0.2/setup.py
+drwxr-xr-x   0 shayanjavid   (501) staff       (20)        0 2023-05-08 23:04:32.055662 MeTA_bagari-0.0.2/src/
+drwxr-xr-x   0 shayanjavid   (501) staff       (20)        0 2023-05-08 23:04:32.058298 MeTA_bagari-0.0.2/src/MeTA/
+-rw-rw-r--   0 shayanjavid   (501) staff       (20)    13729 2023-05-08 18:40:58.000000 MeTA_bagari-0.0.2/src/MeTA/Explained_AssignmentVoxelMaps.py
+-rw-rw-r--   0 shayanjavid   (501) staff       (20)    28142 2023-05-08 18:40:58.000000 MeTA_bagari-0.0.2/src/MeTA/META_toolkit_v2.py
+-rw-r--r--   0 shayanjavid   (501) staff       (20)        0 2023-05-08 20:36:07.000000 MeTA_bagari-0.0.2/src/MeTA/__init__.py
+-rw-rw-r--   0 shayanjavid   (501) staff       (20)     3406 2023-05-08 18:40:58.000000 MeTA_bagari-0.0.2/src/MeTA/calculate_stat.py
+-rw-rw-r--   0 shayanjavid   (501) staff       (20)     5298 2023-05-08 18:40:58.000000 MeTA_bagari-0.0.2/src/MeTA/create_endpoints_mask_with_clustering.py
+-rw-rw-r--   0 shayanjavid   (501) staff       (20)      963 2023-05-08 18:40:58.000000 MeTA_bagari-0.0.2/src/MeTA/read_compressed.py
+-rw-rw-r--   0 shayanjavid   (501) staff       (20)     1617 2023-05-08 18:40:58.000000 MeTA_bagari-0.0.2/src/MeTA/tck2trk.py
+-rw-rw-r--   0 shayanjavid   (501) staff       (20)      899 2023-05-08 18:40:58.000000 MeTA_bagari-0.0.2/src/MeTA/trk2tck.py
+-rw-rw-r--   0 shayanjavid   (501) staff       (20)     3609 2023-05-08 18:40:58.000000 MeTA_bagari-0.0.2/src/MeTA/trk_2_binary.py
+-rw-r--r--   0 shayanjavid   (501) staff       (20)        0 2023-05-08 20:36:07.000000 MeTA_bagari-0.0.2/src/__init__.py
```

### Comparing `MeTA_bagari-0.0.1/LICENSE` & `MeTA_bagari-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MeTA_bagari-0.0.1/MeTA_bagari.egg-info/requires.txt` & `MeTA_bagari-0.0.2/MeTA_bagari.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `MeTA_bagari-0.0.1/setup.py` & `MeTA_bagari-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 # Define our package
 setup(
     name="MeTA_bagari",
-    version='0.0.1',
+    version='0.0.2',
     license='MIT',
     description="Medial Tractography Analysis (MeTA) for White Matter Population Analyses Across Datasets",
     author="Iyad Ba Gari, Abhinaav Ramesh, Shayan Javid,",
     author_email="bagari@usc.edu, contactabhinaav@gmail.com, javidyaz@usc.edu",
     #url="TBD",
     python_requires=">=3.9",
     packages=find_namespace_packages(),
```

### Comparing `MeTA_bagari-0.0.1/src/MeTA/Explained_AssignmentVoxelMaps.py` & `MeTA_bagari-0.0.2/src/MeTA/Explained_AssignmentVoxelMaps.py`

 * *Files identical despite different names*

### Comparing `MeTA_bagari-0.0.1/src/MeTA/META_toolkit_v2.py` & `MeTA_bagari-0.0.2/src/MeTA/META_toolkit_v2.py`

 * *Files identical despite different names*

### Comparing `MeTA_bagari-0.0.1/src/MeTA/calculate_stat.py` & `MeTA_bagari-0.0.2/src/MeTA/calculate_stat.py`

 * *Files identical despite different names*

### Comparing `MeTA_bagari-0.0.1/src/MeTA/create_endpoints_mask_with_clustering.py` & `MeTA_bagari-0.0.2/src/MeTA/create_endpoints_mask_with_clustering.py`

 * *Files identical despite different names*

### Comparing `MeTA_bagari-0.0.1/src/MeTA/read_compressed.py` & `MeTA_bagari-0.0.2/src/MeTA/read_compressed.py`

 * *Files identical despite different names*

### Comparing `MeTA_bagari-0.0.1/src/MeTA/tck2trk.py` & `MeTA_bagari-0.0.2/src/MeTA/tck2trk.py`

 * *Files identical despite different names*

### Comparing `MeTA_bagari-0.0.1/src/MeTA/trk2tck.py` & `MeTA_bagari-0.0.2/src/MeTA/trk2tck.py`

 * *Files identical despite different names*

### Comparing `MeTA_bagari-0.0.1/src/MeTA/trk_2_binary.py` & `MeTA_bagari-0.0.2/src/MeTA/trk_2_binary.py`

 * *Files identical despite different names*

