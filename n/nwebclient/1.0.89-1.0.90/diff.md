# Comparing `tmp/nwebclient-1.0.89.tar.gz` & `tmp/nwebclient-1.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.89.tar", last modified: Tue May  9 13:51:06 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.90.tar", last modified: Tue May  9 14:10:00 2023, max compression
```

## Comparing `nwebclient-1.0.89.tar` & `nwebclient-1.0.90.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-09 13:51:06.125096 nwebclient-1.0.89/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.89/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-09 13:51:06.125096 nwebclient-1.0.89/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.89/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-09 13:51:06.125096 nwebclient-1.0.89/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     6469 2023-05-07 16:18:58.000000 nwebclient-1.0.89/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.89/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-09 12:58:28.000000 nwebclient-1.0.89/nwebclient/crypt.py
--rw-r--r--   0 pi        (1000) pi        (1000)    13240 2023-05-09 13:20:07.000000 nwebclient-1.0.89/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.89/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.89/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-09 13:51:06.125096 nwebclient-1.0.89/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-09 13:51:05.000000 nwebclient-1.0.89/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-05-09 13:51:06.000000 nwebclient-1.0.89/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-09 13:51:05.000000 nwebclient-1.0.89/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-09 13:51:05.000000 nwebclient-1.0.89/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-09 13:51:05.000000 nwebclient-1.0.89/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-09 13:51:05.000000 nwebclient-1.0.89/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-09 13:51:06.125096 nwebclient-1.0.89/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-09 13:50:59.000000 nwebclient-1.0.89/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-09 14:10:00.717213 nwebclient-1.0.90/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.90/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-09 14:10:00.717213 nwebclient-1.0.90/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.90/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-09 14:10:00.717213 nwebclient-1.0.90/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6481 2023-05-09 14:09:41.000000 nwebclient-1.0.90/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.90/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-09 12:58:28.000000 nwebclient-1.0.90/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    13240 2023-05-09 13:20:07.000000 nwebclient-1.0.90/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.90/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.90/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-09 14:10:00.717213 nwebclient-1.0.90/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-09 14:10:00.000000 nwebclient-1.0.90/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-05-09 14:10:00.000000 nwebclient-1.0.90/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-09 14:10:00.000000 nwebclient-1.0.90/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-09 14:10:00.000000 nwebclient-1.0.90/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-09 14:10:00.000000 nwebclient-1.0.90/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-09 14:10:00.000000 nwebclient-1.0.90/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-09 14:10:00.717213 nwebclient-1.0.90/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-09 14:09:56.000000 nwebclient-1.0.90/setup.py
```

### Comparing `nwebclient-1.0.89/LICENSE` & `nwebclient-1.0.90/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.89/PKG-INFO` & `nwebclient-1.0.90/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.89
+Version: 1.0.90
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.89/README.md` & `nwebclient-1.0.90/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.89/nwebclient/__init__.py` & `nwebclient-1.0.90/nwebclient/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 import json
 # add .parse in python3
-import urllib
+import urllib.parse
 import sys
 import os.path
 
 #import .sdb as sdb
 
 name = "nwebclient"
 
@@ -105,15 +105,15 @@
             return self.__cfg[key]
         else:
             return "Non Existing"
     def file_get_contents(self, filename):
         with open(filename) as f:
             return f.read()
     def _appendGet(self, url, name, value):
-        v = name + '=' + urllib.quote(value)
+        v = name + '=' + urllib.parse.quote(value)
         if '?' in url:
             return url + '&' + v
         else:
             return url + '?' + v
     def reqToFile(self, path, name):
         url = self.__url + path
         url = self._appendGet(url, 'username', self.__user)
```

### Comparing `nwebclient-1.0.89/nwebclient/__main__.py` & `nwebclient-1.0.90/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.89/nwebclient/crypt.py` & `nwebclient-1.0.90/nwebclient/crypt.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.89/nwebclient/sd.py` & `nwebclient-1.0.90/nwebclient/sd.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.89/nwebclient/sdb.py` & `nwebclient-1.0.90/nwebclient/sdb.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.89/nwebclient/ticker.py` & `nwebclient-1.0.90/nwebclient/ticker.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.89/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.90/nwebclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.89
+Version: 1.0.90
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.89/setup.py` & `nwebclient-1.0.90/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.89",
+    version="1.0.90",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
```

