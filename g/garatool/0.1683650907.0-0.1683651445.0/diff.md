# Comparing `tmp/garatool-0.1683650907.0.tar.gz` & `tmp/garatool-0.1683651445.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garatool-0.1683650907.0.tar", last modified: Tue May  9 16:48:27 2023, max compression
+gzip compressed data, was "garatool-0.1683651445.0.tar", last modified: Tue May  9 16:57:25 2023, max compression
```

## Comparing `garatool-0.1683650907.0.tar` & `garatool-0.1683651445.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:48:27.442038 garatool-0.1683650907.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 16:48:27.441700 garatool-0.1683650907.0/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683650907.0/README.md
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:48:27.438640 garatool-0.1683650907.0/garatool/
--rw-r--r--   0 curlyz     (501) staff       (20)     5845 2023-05-09 16:48:09.000000 garatool-0.1683650907.0/garatool/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683650907.0/garatool/__main__.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:48:27.441165 garatool-0.1683650907.0/garatool.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 16:48:27.000000 garatool-0.1683650907.0/garatool.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 16:48:27.000000 garatool-0.1683650907.0/garatool.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 16:48:27.000000 garatool-0.1683650907.0/garatool.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 16:48:27.000000 garatool-0.1683650907.0/garatool.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 16:48:27.000000 garatool-0.1683650907.0/garatool.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 16:48:27.442140 garatool-0.1683650907.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683650907.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:57:25.630902 garatool-0.1683651445.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 16:57:25.630626 garatool-0.1683651445.0/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683651445.0/README.md
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:57:25.628195 garatool-0.1683651445.0/garatool/
+-rw-r--r--   0 curlyz     (501) staff       (20)     5650 2023-05-09 16:57:18.000000 garatool-0.1683651445.0/garatool/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683651445.0/garatool/__main__.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:57:25.630114 garatool-0.1683651445.0/garatool.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 16:57:25.000000 garatool-0.1683651445.0/garatool.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 16:57:25.000000 garatool-0.1683651445.0/garatool.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 16:57:25.000000 garatool-0.1683651445.0/garatool.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 16:57:25.000000 garatool-0.1683651445.0/garatool.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 16:57:25.000000 garatool-0.1683651445.0/garatool.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 16:57:25.630985 garatool-0.1683651445.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683651445.0/setup.py
```

### Comparing `garatool-0.1683650907.0/garatool/__init__.py` & `garatool-0.1683651445.0/garatool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 import shutil
 import esptool
 import serial
 import subprocess
 import requests
 import uuid
 import platform
+import tempfile
+
+
 import dacite
 import os
 
 
 from dataclasses import dataclass, asdict, field
 from enum import Enum
 from termcolor import colored
@@ -119,24 +122,18 @@
     if req.status_code != 200:
         raise Exception('Problem: ' + req.text)
     response = dacite.from_dict(BuildRequest, msgpack.loads(req.content, raw=False))
     # print('Response', flag(response))
     return response
 
 
-def publish_tag(tag: str, key: str):
-    print(step('publishing tag'), flag(tag))
-    br.event = 'publish_firmware'
-    req = requests.post(
-        url = 'https://api.garastem.com/api/v1/toolchain/garatool',
-        data = msgpack.dumps(asdict(br))
-    )
 
 def program_device(br: BuildRequest):
     for parti in br.partitions:
+        parti['file'] = tempfile.mkstemp()
         print(parti['file'], parti['offset'], len(parti['data']))
         with open(parti['file'], 'wb') as f:
             f.write(parti['data'])
 
 
 
     partition_params = ' '.join([
```

### Comparing `garatool-0.1683650907.0/setup.py` & `garatool-0.1683651445.0/setup.py`

 * *Files identical despite different names*

