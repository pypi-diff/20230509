# Comparing `tmp/pipfontslibV2-1.0.0.tar.gz` & `tmp/pipfontslibV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipfontslibV2-1.0.0.tar", last modified: Mon May  8 22:20:30 2023, max compression
+gzip compressed data, was "pipfontslibV2-1.1.0.tar", last modified: Mon May  8 22:22:36 2023, max compression
```

## Comparing `pipfontslibV2-1.0.0.tar` & `pipfontslibV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 22:20:30.916050 pipfontslibV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      346 2023-05-08 22:20:30.916050 pipfontslibV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 22:20:30.916050 pipfontslibV2-1.0.0/pipfontslibV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-08 22:20:30.000000 pipfontslibV2-1.0.0/pipfontslibV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 22:20:30.916050 pipfontslibV2-1.0.0/pipfontslibV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      346 2023-05-08 22:20:30.000000 pipfontslibV2-1.0.0/pipfontslibV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2023-05-08 22:20:30.000000 pipfontslibV2-1.0.0/pipfontslibV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 22:20:30.000000 pipfontslibV2-1.0.0/pipfontslibV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-08 22:20:30.000000 pipfontslibV2-1.0.0/pipfontslibV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 22:20:30.916050 pipfontslibV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      559 2023-05-08 22:20:30.000000 pipfontslibV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 22:22:36.946643 pipfontslibV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      346 2023-05-08 22:22:36.946643 pipfontslibV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 22:22:36.946643 pipfontslibV2-1.1.0/pipfontslibV2/
+-rw-r--r--   0 root         (0) root         (0)    97161 2023-05-08 22:22:36.000000 pipfontslibV2-1.1.0/pipfontslibV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 22:22:36.946643 pipfontslibV2-1.1.0/pipfontslibV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      346 2023-05-08 22:22:36.000000 pipfontslibV2-1.1.0/pipfontslibV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2023-05-08 22:22:36.000000 pipfontslibV2-1.1.0/pipfontslibV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 22:22:36.000000 pipfontslibV2-1.1.0/pipfontslibV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-08 22:22:36.000000 pipfontslibV2-1.1.0/pipfontslibV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 22:22:36.946643 pipfontslibV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      559 2023-05-08 22:22:36.000000 pipfontslibV2-1.1.0/setup.py
```

### Comparing `pipfontslibV2-1.0.0/setup.py` & `pipfontslibV2-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pipfontslibV2",
     version=VERSION,
```

