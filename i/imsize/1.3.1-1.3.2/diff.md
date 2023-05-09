# Comparing `tmp/imsize-1.3.1.tar.gz` & `tmp/imsize-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsize-1.3.1.tar", last modified: Mon Dec 19 13:07:19 2022, max compression
+gzip compressed data, was "imsize-1.3.2.tar", last modified: Tue May  9 10:32:46 2023, max compression
```

## Comparing `imsize-1.3.1.tar` & `imsize-1.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2022-12-19 13:07:19.100600 imsize-1.3.1/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2019-07-03 14:07:01.000000 imsize-1.3.1/LICENSE
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       59 2019-07-03 14:02:18.000000 imsize-1.3.1/MANIFEST.in
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      273 2022-12-19 13:07:19.100600 imsize-1.3.1/PKG-INFO
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      589 2022-12-19 13:04:44.000000 imsize-1.3.1/README.md
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2022-12-19 13:07:19.100600 imsize-1.3.1/imsize/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      346 2022-12-19 13:04:44.000000 imsize-1.3.1/imsize/__init__.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    15567 2022-02-02 08:35:25.000000 imsize-1.3.1/imsize/argv.py
--rwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)     3982 2022-12-19 13:04:44.000000 imsize-1.3.1/imsize/consoleapp.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     2760 2021-11-15 12:23:50.000000 imsize-1.3.1/imsize/exrhdr.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    14518 2022-12-19 13:04:44.000000 imsize-1.3.1/imsize/imsize.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     1785 2021-10-07 08:19:52.000000 imsize-1.3.1/imsize/pfmhdr.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     1733 2021-10-07 08:19:52.000000 imsize-1.3.1/imsize/pnmhdr.py
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2022-12-19 13:07:19.100600 imsize-1.3.1/imsize.egg-info/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      273 2022-12-19 13:07:19.000000 imsize-1.3.1/imsize.egg-info/PKG-INFO
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      430 2022-12-19 13:07:19.000000 imsize-1.3.1/imsize.egg-info/SOURCES.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2022-12-19 13:07:19.000000 imsize-1.3.1/imsize.egg-info/dependency_links.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       51 2022-12-19 13:07:19.000000 imsize-1.3.1/imsize.egg-info/entry_points.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       57 2022-12-19 13:07:19.000000 imsize-1.3.1/imsize.egg-info/requires.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       12 2022-12-19 13:07:19.000000 imsize-1.3.1/imsize.egg-info/top_level.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2022-12-19 13:07:19.000000 imsize-1.3.1/imsize.egg-info/zip-safe
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       65 2022-01-13 10:06:37.000000 imsize-1.3.1/requirements.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      107 2022-12-19 13:07:19.100600 imsize-1.3.1/setup.cfg
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      709 2021-10-07 08:19:52.000000 imsize-1.3.1/setup.py
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2022-12-19 13:07:19.100600 imsize-1.3.1/test/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        0 2021-10-07 08:19:52.000000 imsize-1.3.1/test/__init__.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     4919 2022-12-19 13:04:44.000000 imsize-1.3.1/test/test_read.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-09 10:32:46.482217 imsize-1.3.2/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 imsize-1.3.2/LICENSE
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       59 2023-03-13 15:45:56.000000 imsize-1.3.2/MANIFEST.in
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      284 2023-05-09 10:32:46.482217 imsize-1.3.2/PKG-INFO
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      589 2023-03-13 15:45:56.000000 imsize-1.3.2/README.md
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-09 10:32:46.482217 imsize-1.3.2/imsize/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      346 2023-05-09 10:16:43.000000 imsize-1.3.2/imsize/__init__.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    15567 2023-03-13 15:45:56.000000 imsize-1.3.2/imsize/argv.py
+-rwxr-xr-x   0 toaarnio  (1000) toaarnio  (1000)     3982 2023-04-19 12:14:31.000000 imsize-1.3.2/imsize/consoleapp.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     2760 2023-03-13 15:45:56.000000 imsize-1.3.2/imsize/exrhdr.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    14618 2023-05-09 10:22:58.000000 imsize-1.3.2/imsize/imsize.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1785 2023-03-13 15:45:56.000000 imsize-1.3.2/imsize/pfmhdr.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1733 2023-03-13 15:45:56.000000 imsize-1.3.2/imsize/pnmhdr.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-09 10:32:46.482217 imsize-1.3.2/imsize.egg-info/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      284 2023-05-09 10:32:46.000000 imsize-1.3.2/imsize.egg-info/PKG-INFO
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      430 2023-05-09 10:32:46.000000 imsize-1.3.2/imsize.egg-info/SOURCES.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-05-09 10:32:46.000000 imsize-1.3.2/imsize.egg-info/dependency_links.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       51 2023-05-09 10:32:46.000000 imsize-1.3.2/imsize.egg-info/entry_points.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       57 2023-05-09 10:32:46.000000 imsize-1.3.2/imsize.egg-info/requires.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       12 2023-05-09 10:32:46.000000 imsize-1.3.2/imsize.egg-info/top_level.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-05-09 10:32:46.000000 imsize-1.3.2/imsize.egg-info/zip-safe
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       65 2023-03-13 15:45:56.000000 imsize-1.3.2/requirements.txt
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      107 2023-05-09 10:32:46.482217 imsize-1.3.2/setup.cfg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      709 2023-03-13 15:45:56.000000 imsize-1.3.2/setup.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-09 10:32:46.482217 imsize-1.3.2/test/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)        0 2023-03-13 15:45:56.000000 imsize-1.3.2/test/__init__.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     4919 2023-03-13 15:45:57.000000 imsize-1.3.2/test/test_read.py
```

### Comparing `imsize-1.3.1/LICENSE` & `imsize-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `imsize-1.3.1/README.md` & `imsize-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `imsize-1.3.1/imsize/argv.py` & `imsize-1.3.2/imsize/argv.py`

 * *Files identical despite different names*

### Comparing `imsize-1.3.1/imsize/consoleapp.py` & `imsize-1.3.2/imsize/consoleapp.py`

 * *Files identical despite different names*

### Comparing `imsize-1.3.1/imsize/exrhdr.py` & `imsize-1.3.2/imsize/exrhdr.py`

 * *Files identical despite different names*

### Comparing `imsize-1.3.1/imsize/imsize.py` & `imsize-1.3.2/imsize/imsize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/python3 -B
-
 """
 Extracts image dimensions, bit depth, and other basic metadata.
 """
 
 import os              # built-in library
 import math            # built-in library
 import struct          # built-in library
@@ -377,35 +375,36 @@
         info = _complete(info)
     else:
         info = None
     return info
 
 
 def _read_npy(filespec):
-    info = ImageInfo()
-    info.filespec = filespec
-    info.filetype = "npy"
-    info.cfa_raw = False
     with open(filespec, "rb") as npyfile:
         magic = npyfile.read(6)
         assert magic == b"\x93NUMPY"
         _ = npyfile.read(2)  # version number; ignore
         header_size, = struct.unpack("<h", npyfile.read(2))
         header = npyfile.read(header_size)
         meta = ast.literal_eval(header.decode("utf-8"))
         dtype = np.dtype(meta["descr"])
         shape = meta["shape"]
-        info.height, info.width = shape[:2]
-        info.nchan = 1 if len(shape) < 3 else shape[2]
-        info.isfloat = np.issubdtype(dtype, np.floating)
-        info.bytedepth = dtype.itemsize
-        info.bitdepth = info.bytedepth * 8
-        info.maxval = 1.0 if info.isfloat else 2 ** info.bitdepth - 1
-        info = _complete(info)
-    return info
+        if len(shape) in [2, 3]:  # grayscale or color
+            info = ImageInfo()
+            info.filespec = filespec
+            info.filetype = "npy"
+            info.cfa_raw = False
+            info.height, info.width = shape[:2]
+            info.nchan = 1 if len(shape) < 3 else shape[2]
+            info.isfloat = np.issubdtype(dtype, np.floating)
+            info.bytedepth = dtype.itemsize
+            info.bitdepth = info.bytedepth * 8
+            info.maxval = 1.0 if info.isfloat else 2 ** info.bitdepth - 1
+            info = _complete(info)
+            return info
 
 
 def _complete(info):
     info.filesize = info.filesize or os.path.getsize(info.filespec)
     info.maxval = info.maxval or 2 ** info.bitdepth - 1
     info.bitdepth = info.bitdepth or int(math.log2(info.maxval + 1))
     info.bytedepth = info.bytedepth or (2 if info.maxval > 255 else 1)
```

### Comparing `imsize-1.3.1/imsize/pfmhdr.py` & `imsize-1.3.2/imsize/pfmhdr.py`

 * *Files identical despite different names*

### Comparing `imsize-1.3.1/imsize/pnmhdr.py` & `imsize-1.3.2/imsize/pnmhdr.py`

 * *Files identical despite different names*

### Comparing `imsize-1.3.1/setup.py` & `imsize-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `imsize-1.3.1/test/test_read.py` & `imsize-1.3.2/test/test_read.py`

 * *Files identical despite different names*

