# Comparing `tmp/garaprod-0.1683603820.0.tar.gz` & `tmp/garaprod-0.1683613799.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garaprod-0.1683603820.0.tar", last modified: Tue May  9 03:43:40 2023, max compression
+gzip compressed data, was "garaprod-0.1683613799.0.tar", last modified: Tue May  9 06:29:59 2023, max compression
```

## Comparing `garaprod-0.1683603820.0.tar` & `garaprod-0.1683613799.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 03:43:40.340776 garaprod-0.1683603820.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 03:43:40.340435 garaprod-0.1683603820.0/PKG-INFO
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 03:43:40.333199 garaprod-0.1683603820.0/garaprod/
--rw-r--r--   0 curlyz     (501) staff       (20)      578 2023-05-09 03:43:30.000000 garaprod-0.1683603820.0/garaprod/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 03:35:00.000000 garaprod-0.1683603820.0/garaprod/modules.py
--rw-r--r--   0 curlyz     (501) staff       (20)       26 2023-05-09 03:43:40.000000 garaprod-0.1683603820.0/garaprod/version.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 03:43:40.339760 garaprod-0.1683603820.0/garaprod.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 03:43:40.000000 garaprod-0.1683603820.0/garaprod.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      228 2023-05-09 03:43:40.000000 garaprod-0.1683603820.0/garaprod.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 03:43:40.000000 garaprod-0.1683603820.0/garaprod.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       36 2023-05-09 03:43:40.000000 garaprod-0.1683603820.0/garaprod.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 03:43:40.000000 garaprod-0.1683603820.0/garaprod.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 03:43:40.340923 garaprod-0.1683603820.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1106 2023-05-09 03:43:37.000000 garaprod-0.1683603820.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 06:29:59.208024 garaprod-0.1683613799.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 06:29:59.207705 garaprod-0.1683613799.0/PKG-INFO
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 06:29:59.204730 garaprod-0.1683613799.0/garaprod/
+-rw-r--r--   0 curlyz     (501) staff       (20)     3692 2023-05-09 05:51:48.000000 garaprod-0.1683613799.0/garaprod/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 03:35:00.000000 garaprod-0.1683613799.0/garaprod/modules.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       26 2023-05-09 06:29:59.000000 garaprod-0.1683613799.0/garaprod/version.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 06:29:59.207089 garaprod-0.1683613799.0/garaprod.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 06:29:59.000000 garaprod-0.1683613799.0/garaprod.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      228 2023-05-09 06:29:59.000000 garaprod-0.1683613799.0/garaprod.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 06:29:59.000000 garaprod-0.1683613799.0/garaprod.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       36 2023-05-09 06:29:59.000000 garaprod-0.1683613799.0/garaprod.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 06:29:59.000000 garaprod-0.1683613799.0/garaprod.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 06:29:59.208117 garaprod-0.1683613799.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1106 2023-05-09 03:43:37.000000 garaprod-0.1683613799.0/setup.py
```

### Comparing `garaprod-0.1683603820.0/setup.py` & `garaprod-0.1683613799.0/setup.py`

 * *Files identical despite different names*

