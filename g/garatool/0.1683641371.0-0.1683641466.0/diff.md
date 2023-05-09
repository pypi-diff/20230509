# Comparing `tmp/garatool-0.1683641371.0.tar.gz` & `tmp/garatool-0.1683641466.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garatool-0.1683641371.0.tar", last modified: Tue May  9 14:09:31 2023, max compression
+gzip compressed data, was "garatool-0.1683641466.0.tar", last modified: Tue May  9 14:11:06 2023, max compression
```

## Comparing `garatool-0.1683641371.0.tar` & `garatool-0.1683641466.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 14:09:31.614883 garatool-0.1683641371.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 14:09:31.614357 garatool-0.1683641371.0/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683641371.0/README.md
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 14:09:31.604102 garatool-0.1683641371.0/garatool/
--rw-r--r--   0 curlyz     (501) staff       (20)       15 2023-05-09 14:09:29.000000 garatool-0.1683641371.0/garatool/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 14:05:11.000000 garatool-0.1683641371.0/garatool/garatool.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 14:09:31.613216 garatool-0.1683641371.0/garatool.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 14:09:31.000000 garatool-0.1683641371.0/garatool.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 14:09:31.000000 garatool-0.1683641371.0/garatool.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 14:09:31.000000 garatool-0.1683641371.0/garatool.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       35 2023-05-09 14:09:31.000000 garatool-0.1683641371.0/garatool.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 14:09:31.000000 garatool-0.1683641371.0/garatool.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 14:09:31.615067 garatool-0.1683641371.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1073 2023-05-09 14:08:14.000000 garatool-0.1683641371.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 14:11:06.952539 garatool-0.1683641466.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 14:11:06.952082 garatool-0.1683641466.0/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683641466.0/README.md
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 14:11:06.938691 garatool-0.1683641466.0/garatool/
+-rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 14:10:58.000000 garatool-0.1683641466.0/garatool/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 14:05:11.000000 garatool-0.1683641466.0/garatool/garatool.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 14:11:06.951481 garatool-0.1683641466.0/garatool.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 14:11:06.000000 garatool-0.1683641466.0/garatool.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 14:11:06.000000 garatool-0.1683641466.0/garatool.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 14:11:06.000000 garatool-0.1683641466.0/garatool.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       35 2023-05-09 14:11:06.000000 garatool-0.1683641466.0/garatool.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 14:11:06.000000 garatool-0.1683641466.0/garatool.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 14:11:06.952675 garatool-0.1683641466.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1073 2023-05-09 14:08:14.000000 garatool-0.1683641466.0/setup.py
```

### Comparing `garatool-0.1683641371.0/setup.py` & `garatool-0.1683641466.0/setup.py`

 * *Files identical despite different names*

