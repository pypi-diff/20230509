# Comparing `tmp/garaprod-0.1683617694.0.tar.gz` & `tmp/garaprod-0.1683617809.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garaprod-0.1683617694.0.tar", last modified: Tue May  9 07:34:54 2023, max compression
+gzip compressed data, was "garaprod-0.1683617809.0.tar", last modified: Tue May  9 07:36:49 2023, max compression
```

## Comparing `garaprod-0.1683617694.0.tar` & `garaprod-0.1683617809.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:34:54.814003 garaprod-0.1683617694.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 07:34:54.813708 garaprod-0.1683617694.0/PKG-INFO
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:34:54.810746 garaprod-0.1683617694.0/garaprod/
--rw-r--r--   0 curlyz     (501) staff       (20)     4949 2023-05-09 07:26:45.000000 garaprod-0.1683617694.0/garaprod/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 03:35:00.000000 garaprod-0.1683617694.0/garaprod/modules.py
--rw-r--r--   0 curlyz     (501) staff       (20)       26 2023-05-09 07:34:54.000000 garaprod-0.1683617694.0/garaprod/version.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:34:54.813125 garaprod-0.1683617694.0/garaprod.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 07:34:54.000000 garaprod-0.1683617694.0/garaprod.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      228 2023-05-09 07:34:54.000000 garaprod-0.1683617694.0/garaprod.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 07:34:54.000000 garaprod-0.1683617694.0/garaprod.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       45 2023-05-09 07:34:54.000000 garaprod-0.1683617694.0/garaprod.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 07:34:54.000000 garaprod-0.1683617694.0/garaprod.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 07:34:54.814112 garaprod-0.1683617694.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1122 2023-05-09 06:39:47.000000 garaprod-0.1683617694.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:36:49.992348 garaprod-0.1683617809.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 07:36:49.992061 garaprod-0.1683617809.0/PKG-INFO
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:36:49.989319 garaprod-0.1683617809.0/garaprod/
+-rw-r--r--   0 curlyz     (501) staff       (20)     4949 2023-05-09 07:36:47.000000 garaprod-0.1683617809.0/garaprod/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 03:35:00.000000 garaprod-0.1683617809.0/garaprod/modules.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       26 2023-05-09 07:36:49.000000 garaprod-0.1683617809.0/garaprod/version.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 07:36:49.991585 garaprod-0.1683617809.0/garaprod.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 07:36:49.000000 garaprod-0.1683617809.0/garaprod.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      228 2023-05-09 07:36:49.000000 garaprod-0.1683617809.0/garaprod.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 07:36:49.000000 garaprod-0.1683617809.0/garaprod.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       45 2023-05-09 07:36:49.000000 garaprod-0.1683617809.0/garaprod.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 07:36:49.000000 garaprod-0.1683617809.0/garaprod.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 07:36:49.992460 garaprod-0.1683617809.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1122 2023-05-09 06:39:47.000000 garaprod-0.1683617809.0/setup.py
```

### Comparing `garaprod-0.1683617694.0/garaprod/__init__.py` & `garaprod-0.1683617809.0/garaprod/__init__.py`

 * *Files identical despite different names*

### Comparing `garaprod-0.1683617694.0/setup.py` & `garaprod-0.1683617809.0/setup.py`

 * *Files identical despite different names*

