# Comparing `tmp/garaprod-0.1683617603.0.tar.gz` & `tmp/garaprod-0.1683617637.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garaprod-0.1683617603.0.tar", last modified: Tue May  9 07:33:23 2023, max compression
+gzip compressed data, was "garaprod-0.1683617637.0.tar", last modified: Tue May  9 07:33:57 2023, max compression
```

## Comparing `garaprod-0.1683617603.0.tar` & `garaprod-0.1683617637.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:33:23.952053 garaprod-0.1683617603.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 07:33:23.951726 garaprod-0.1683617603.0/PKG-INFO
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:33:23.949111 garaprod-0.1683617603.0/garaprod/
--rw-r--r--   0 curlyz     (501) staff       (20)     4949 2023-05-09 07:26:45.000000 garaprod-0.1683617603.0/garaprod/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 03:35:00.000000 garaprod-0.1683617603.0/garaprod/modules.py
--rw-r--r--   0 curlyz     (501) staff       (20)       26 2023-05-09 07:33:23.000000 garaprod-0.1683617603.0/garaprod/version.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:33:23.951291 garaprod-0.1683617603.0/garaprod.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 07:33:23.000000 garaprod-0.1683617603.0/garaprod.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      228 2023-05-09 07:33:23.000000 garaprod-0.1683617603.0/garaprod.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 07:33:23.000000 garaprod-0.1683617603.0/garaprod.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       45 2023-05-09 07:33:23.000000 garaprod-0.1683617603.0/garaprod.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 07:33:23.000000 garaprod-0.1683617603.0/garaprod.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 07:33:23.952145 garaprod-0.1683617603.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1122 2023-05-09 06:39:47.000000 garaprod-0.1683617603.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:33:57.183536 garaprod-0.1683617637.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 07:33:57.182966 garaprod-0.1683617637.0/PKG-INFO
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:33:57.177111 garaprod-0.1683617637.0/garaprod/
+-rw-r--r--   0 curlyz     (501) staff       (20)     4949 2023-05-09 07:26:45.000000 garaprod-0.1683617637.0/garaprod/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 03:35:00.000000 garaprod-0.1683617637.0/garaprod/modules.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       26 2023-05-09 07:33:57.000000 garaprod-0.1683617637.0/garaprod/version.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:33:57.182058 garaprod-0.1683617637.0/garaprod.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 07:33:57.000000 garaprod-0.1683617637.0/garaprod.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      228 2023-05-09 07:33:57.000000 garaprod-0.1683617637.0/garaprod.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 07:33:57.000000 garaprod-0.1683617637.0/garaprod.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       45 2023-05-09 07:33:57.000000 garaprod-0.1683617637.0/garaprod.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 07:33:57.000000 garaprod-0.1683617637.0/garaprod.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 07:33:57.183689 garaprod-0.1683617637.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1122 2023-05-09 06:39:47.000000 garaprod-0.1683617637.0/setup.py
```

### Comparing `garaprod-0.1683617603.0/garaprod/__init__.py` & `garaprod-0.1683617637.0/garaprod/__init__.py`

 * *Files identical despite different names*

### Comparing `garaprod-0.1683617603.0/setup.py` & `garaprod-0.1683617637.0/setup.py`

 * *Files identical despite different names*

