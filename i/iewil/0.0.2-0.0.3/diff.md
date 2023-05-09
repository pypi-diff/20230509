# Comparing `tmp/iewil-0.0.2.tar.gz` & `tmp/iewil-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iewil-0.0.2.tar", last modified: Sun Apr 30 04:39:15 2023, max compression
+gzip compressed data, was "iewil-0.0.3.tar", last modified: Tue May  9 14:41:46 2023, max compression
```

## Comparing `iewil-0.0.2.tar` & `iewil-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 04:39:15.909713 iewil-0.0.2/
--rw-rw-rw-   0        0        0      452 2023-04-30 04:39:15.907765 iewil-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-30 04:39:15.889217 iewil-0.0.2/iewil/
--rw-rw-rw-   0        0        0     3095 2023-04-30 04:38:01.000000 iewil-0.0.2/iewil/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 04:39:15.905836 iewil-0.0.2/iewil.egg-info/
--rw-rw-rw-   0        0        0      452 2023-04-30 04:39:15.000000 iewil-0.0.2/iewil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      142 2023-04-30 04:39:15.000000 iewil-0.0.2/iewil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 04:39:15.000000 iewil-0.0.2/iewil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-30 04:39:15.000000 iewil-0.0.2/iewil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 04:39:15.909713 iewil-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      666 2023-04-30 04:39:08.000000 iewil-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:41:46.228738 iewil-0.0.3/
+-rw-rw-rw-   0        0        0      436 2023-05-09 14:41:46.227745 iewil-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-09 14:41:46.209979 iewil-0.0.3/iewil/
+-rw-rw-rw-   0        0        0     4321 2023-05-09 14:41:17.000000 iewil-0.0.3/iewil/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:41:46.225792 iewil-0.0.3/iewil.egg-info/
+-rw-rw-rw-   0        0        0      436 2023-05-09 14:41:45.000000 iewil-0.0.3/iewil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2023-05-09 14:41:45.000000 iewil-0.0.3/iewil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 14:41:45.000000 iewil-0.0.3/iewil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-09 14:41:45.000000 iewil-0.0.3/iewil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 14:41:46.228738 iewil-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      650 2023-05-09 14:40:35.000000 iewil-0.0.3/setup.py
```

### Comparing `iewil-0.0.2/setup.py` & `iewil-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
-DESCRIPTION = 'Streaming video data via networks'
+VERSION = '0.0.3'
+DESCRIPTION = 'modul pribadi ygy'
 
 # Setting up
 setup(
     name="iewil",
     version=VERSION,
     author="iewilmaestro",
     author_email="<purna.iera@gmail.com>",
```

