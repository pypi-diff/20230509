# Comparing `tmp/garatool-0.1683650517.0.tar.gz` & `tmp/garatool-0.1683650648.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garatool-0.1683650517.0.tar", last modified: Tue May  9 16:41:57 2023, max compression
+gzip compressed data, was "garatool-0.1683650648.0.tar", last modified: Tue May  9 16:44:08 2023, max compression
```

## Comparing `garatool-0.1683650517.0.tar` & `garatool-0.1683650648.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:41:57.623834 garatool-0.1683650517.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 16:41:57.623528 garatool-0.1683650517.0/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683650517.0/README.md
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:41:57.620911 garatool-0.1683650517.0/garatool/
--rw-r--r--   0 curlyz     (501) staff       (20)     5742 2023-05-09 16:35:34.000000 garatool-0.1683650517.0/garatool/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 14:05:11.000000 garatool-0.1683650517.0/garatool/garatool.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:41:57.623104 garatool-0.1683650517.0/garatool.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 16:41:57.000000 garatool-0.1683650517.0/garatool.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 16:41:57.000000 garatool-0.1683650517.0/garatool.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 16:41:57.000000 garatool-0.1683650517.0/garatool.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 16:41:57.000000 garatool-0.1683650517.0/garatool.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 16:41:57.000000 garatool-0.1683650517.0/garatool.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 16:41:57.623922 garatool-0.1683650517.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683650517.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:44:08.849339 garatool-0.1683650648.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 16:44:08.848932 garatool-0.1683650648.0/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683650648.0/README.md
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:44:08.843804 garatool-0.1683650648.0/garatool/
+-rw-r--r--   0 curlyz     (501) staff       (20)     5742 2023-05-09 16:35:34.000000 garatool-0.1683650648.0/garatool/__init__.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:44:08.848312 garatool-0.1683650648.0/garatool.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 16:44:08.000000 garatool-0.1683650648.0/garatool.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      198 2023-05-09 16:44:08.000000 garatool-0.1683650648.0/garatool.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 16:44:08.000000 garatool-0.1683650648.0/garatool.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 16:44:08.000000 garatool-0.1683650648.0/garatool.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 16:44:08.000000 garatool-0.1683650648.0/garatool.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 16:44:08.849439 garatool-0.1683650648.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683650648.0/setup.py
```

### Comparing `garatool-0.1683650517.0/garatool/__init__.py` & `garatool-0.1683650648.0/garatool/__init__.py`

 * *Files identical despite different names*

### Comparing `garatool-0.1683650517.0/setup.py` & `garatool-0.1683650648.0/setup.py`

 * *Files identical despite different names*

