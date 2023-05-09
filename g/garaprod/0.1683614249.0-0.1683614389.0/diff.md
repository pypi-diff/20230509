# Comparing `tmp/garaprod-0.1683614249.0.tar.gz` & `tmp/garaprod-0.1683614389.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garaprod-0.1683614249.0.tar", last modified: Tue May  9 06:37:29 2023, max compression
+gzip compressed data, was "garaprod-0.1683614389.0.tar", last modified: Tue May  9 06:39:50 2023, max compression
```

## Comparing `garaprod-0.1683614249.0.tar` & `garaprod-0.1683614389.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 06:37:29.666000 garaprod-0.1683614249.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 06:37:29.665653 garaprod-0.1683614249.0/PKG-INFO
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 06:37:29.662607 garaprod-0.1683614249.0/garaprod/
--rw-r--r--   0 curlyz     (501) staff       (20)     4839 2023-05-09 06:36:28.000000 garaprod-0.1683614249.0/garaprod/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 03:35:00.000000 garaprod-0.1683614249.0/garaprod/modules.py
--rw-r--r--   0 curlyz     (501) staff       (20)       26 2023-05-09 06:37:29.000000 garaprod-0.1683614249.0/garaprod/version.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 06:37:29.665122 garaprod-0.1683614249.0/garaprod.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 06:37:29.000000 garaprod-0.1683614249.0/garaprod.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      228 2023-05-09 06:37:29.000000 garaprod-0.1683614249.0/garaprod.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 06:37:29.000000 garaprod-0.1683614249.0/garaprod.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       36 2023-05-09 06:37:29.000000 garaprod-0.1683614249.0/garaprod.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 06:37:29.000000 garaprod-0.1683614249.0/garaprod.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 06:37:29.666238 garaprod-0.1683614249.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1106 2023-05-09 03:43:37.000000 garaprod-0.1683614249.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 06:39:50.108193 garaprod-0.1683614389.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 06:39:50.106710 garaprod-0.1683614389.0/PKG-INFO
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 06:39:50.101782 garaprod-0.1683614389.0/garaprod/
+-rw-r--r--   0 curlyz     (501) staff       (20)     4871 2023-05-09 06:39:43.000000 garaprod-0.1683614389.0/garaprod/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 03:35:00.000000 garaprod-0.1683614389.0/garaprod/modules.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       26 2023-05-09 06:39:49.000000 garaprod-0.1683614389.0/garaprod/version.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 06:39:50.105857 garaprod-0.1683614389.0/garaprod.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 06:39:50.000000 garaprod-0.1683614389.0/garaprod.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      228 2023-05-09 06:39:50.000000 garaprod-0.1683614389.0/garaprod.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 06:39:50.000000 garaprod-0.1683614389.0/garaprod.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       45 2023-05-09 06:39:50.000000 garaprod-0.1683614389.0/garaprod.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 06:39:50.000000 garaprod-0.1683614389.0/garaprod.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 06:39:50.108530 garaprod-0.1683614389.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1122 2023-05-09 06:39:47.000000 garaprod-0.1683614389.0/setup.py
```

### Comparing `garaprod-0.1683614249.0/garaprod/__init__.py` & `garaprod-0.1683614389.0/garaprod/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 from dataclasses import dataclass, asdict, field
 
 
 import requests
 from enum import Enum
 from termcolor import colored
 
+import colorama
+colorama.init()
 
 
 # try:
 #     import requests
 #     req = requests.get('https://pypi.org/pypi/garaprod/json')
 #     package_info = req.json()
 #     latest_version = package_info['info']['version']
```

### Comparing `garaprod-0.1683614249.0/setup.py` & `garaprod-0.1683614389.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     download_url='https://pypi.org/project/garaprod/'
 )
 
 install_requires = [
     'termcolor',
     'requests',
     'umsgpack',
+    'colorama',
     'esptool'
 ]
 
 print("find_packages()", find_packages())
 
 import os
 if __name__ == '__main__':
```

