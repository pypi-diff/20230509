# Comparing `tmp/garatool-0.1683650143.0.tar.gz` & `tmp/garatool-0.1683650517.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garatool-0.1683650143.0.tar", last modified: Tue May  9 16:35:44 2023, max compression
+gzip compressed data, was "garatool-0.1683650517.0.tar", last modified: Tue May  9 16:41:57 2023, max compression
```

## Comparing `garatool-0.1683650143.0.tar` & `garatool-0.1683650517.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:35:44.077704 garatool-0.1683650143.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 16:35:44.077396 garatool-0.1683650143.0/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683650143.0/README.md
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:35:44.074358 garatool-0.1683650143.0/garatool/
--rw-r--r--   0 curlyz     (501) staff       (20)     5742 2023-05-09 16:35:34.000000 garatool-0.1683650143.0/garatool/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 14:05:11.000000 garatool-0.1683650143.0/garatool/garatool.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:35:44.076907 garatool-0.1683650143.0/garatool.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 16:35:44.000000 garatool-0.1683650143.0/garatool.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 16:35:44.000000 garatool-0.1683650143.0/garatool.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 16:35:44.000000 garatool-0.1683650143.0/garatool.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       42 2023-05-09 16:35:44.000000 garatool-0.1683650143.0/garatool.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 16:35:44.000000 garatool-0.1683650143.0/garatool.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 16:35:44.077795 garatool-0.1683650143.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1086 2023-05-09 14:52:37.000000 garatool-0.1683650143.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:41:57.623834 garatool-0.1683650517.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 16:41:57.623528 garatool-0.1683650517.0/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683650517.0/README.md
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:41:57.620911 garatool-0.1683650517.0/garatool/
+-rw-r--r--   0 curlyz     (501) staff       (20)     5742 2023-05-09 16:35:34.000000 garatool-0.1683650517.0/garatool/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 14:05:11.000000 garatool-0.1683650517.0/garatool/garatool.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:41:57.623104 garatool-0.1683650517.0/garatool.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 16:41:57.000000 garatool-0.1683650517.0/garatool.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 16:41:57.000000 garatool-0.1683650517.0/garatool.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 16:41:57.000000 garatool-0.1683650517.0/garatool.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 16:41:57.000000 garatool-0.1683650517.0/garatool.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 16:41:57.000000 garatool-0.1683650517.0/garatool.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 16:41:57.623922 garatool-0.1683650517.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683650517.0/setup.py
```

### Comparing `garatool-0.1683650143.0/garatool/__init__.py` & `garatool-0.1683650517.0/garatool/__init__.py`

 * *Files identical despite different names*

### Comparing `garatool-0.1683650143.0/setup.py` & `garatool-0.1683650517.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 )
 
 install_requires = [
     'termcolor',
     'requests',
     'msgpack',
     'esptool',
-    'dacite'
+    'dacite',
+    'colorama'
 ]
 
 print("find_packages()", find_packages())
 
 import os
 if __name__ == '__main__':
     os.system('rm -rf dist')
```

