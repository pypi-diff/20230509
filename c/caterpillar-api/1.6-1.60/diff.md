# Comparing `tmp/caterpillar_api-1.6.tar.gz` & `tmp/caterpillar_api-1.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caterpillar_api-1.6.tar", last modified: Mon May  8 23:59:28 2023, max compression
+gzip compressed data, was "caterpillar_api-1.60.tar", last modified: Tue May  9 00:04:13 2023, max compression
```

## Comparing `caterpillar_api-1.6.tar` & `caterpillar_api-1.60.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ldupin    (1000) ldupin    (1000)        0 2023-05-08 23:59:28.795591 caterpillar_api-1.6/
--rw-r--r--   0 ldupin    (1000) ldupin    (1000)     1067 2021-11-14 23:01:12.000000 caterpillar_api-1.6/LICENSE
--rw-r--r--   0 ldupin    (1000) ldupin    (1000)    14501 2023-05-08 23:59:28.795591 caterpillar_api-1.6/PKG-INFO
--rw-r--r--   0 ldupin    (1000) ldupin    (1000)    13488 2023-05-08 23:54:48.000000 caterpillar_api-1.6/README.md
-drwxr-xr-x   0 ldupin    (1000) ldupin    (1000)        0 2023-05-08 23:59:28.795591 caterpillar_api-1.6/caterpillar_api/
--rw-r--r--   0 ldupin    (1000) ldupin    (1000)     7270 2023-05-08 23:54:59.000000 caterpillar_api-1.6/caterpillar_api/__init__.py
--rw-r--r--   0 ldupin    (1000) ldupin    (1000)     1299 2023-05-08 23:51:25.000000 caterpillar_api-1.6/caterpillar_api/monarch.py
--rw-r--r--   0 ldupin    (1000) ldupin    (1000)     6411 2023-05-08 23:45:53.000000 caterpillar_api-1.6/caterpillar_api/util.py
-drwxr-xr-x   0 ldupin    (1000) ldupin    (1000)        0 2023-05-08 23:59:28.795591 caterpillar_api-1.6/caterpillar_api.egg-info/
--rw-r--r--   0 ldupin    (1000) ldupin    (1000)    14501 2023-05-08 23:59:28.000000 caterpillar_api-1.6/caterpillar_api.egg-info/PKG-INFO
--rw-r--r--   0 ldupin    (1000) ldupin    (1000)      338 2023-05-08 23:59:28.000000 caterpillar_api-1.6/caterpillar_api.egg-info/SOURCES.txt
--rw-r--r--   0 ldupin    (1000) ldupin    (1000)        1 2023-05-08 23:59:28.000000 caterpillar_api-1.6/caterpillar_api.egg-info/dependency_links.txt
--rw-r--r--   0 ldupin    (1000) ldupin    (1000)        7 2023-05-08 23:59:28.000000 caterpillar_api-1.6/caterpillar_api.egg-info/requires.txt
--rw-r--r--   0 ldupin    (1000) ldupin    (1000)       16 2023-05-08 23:59:28.000000 caterpillar_api-1.6/caterpillar_api.egg-info/top_level.txt
--rwxr-xr-x   0 ldupin    (1000) ldupin    (1000)      117 2021-11-16 17:07:40.000000 caterpillar_api-1.6/release.sh
--rw-r--r--   0 ldupin    (1000) ldupin    (1000)       50 2023-05-08 23:59:28.795591 caterpillar_api-1.6/setup.cfg
--rw-r--r--   0 ldupin    (1000) ldupin    (1000)     1576 2023-05-08 23:48:59.000000 caterpillar_api-1.6/setup.py
-drwxr-xr-x   0 ldupin    (1000) ldupin    (1000)        0 2023-05-08 23:59:28.795591 caterpillar_api-1.6/tests/
--rw-r--r--   0 ldupin    (1000) ldupin    (1000)      973 2021-11-15 06:33:08.000000 caterpillar_api-1.6/tests/all_test.py
+drwxr-xr-x   0 ldupin    (1000) ldupin    (1000)        0 2023-05-09 00:04:13.124382 caterpillar_api-1.60/
+-rw-r--r--   0 ldupin    (1000) ldupin    (1000)     1067 2021-11-14 23:01:12.000000 caterpillar_api-1.60/LICENSE
+-rw-r--r--   0 ldupin    (1000) ldupin    (1000)    14502 2023-05-09 00:04:13.124382 caterpillar_api-1.60/PKG-INFO
+-rw-r--r--   0 ldupin    (1000) ldupin    (1000)    13488 2023-05-08 23:54:48.000000 caterpillar_api-1.60/README.md
+drwxr-xr-x   0 ldupin    (1000) ldupin    (1000)        0 2023-05-09 00:04:13.124382 caterpillar_api-1.60/caterpillar_api/
+-rw-r--r--   0 ldupin    (1000) ldupin    (1000)     7270 2023-05-08 23:54:59.000000 caterpillar_api-1.60/caterpillar_api/__init__.py
+-rw-r--r--   0 ldupin    (1000) ldupin    (1000)     1299 2023-05-08 23:51:25.000000 caterpillar_api-1.60/caterpillar_api/monarch.py
+-rw-r--r--   0 ldupin    (1000) ldupin    (1000)     6411 2023-05-08 23:45:53.000000 caterpillar_api-1.60/caterpillar_api/util.py
+drwxr-xr-x   0 ldupin    (1000) ldupin    (1000)        0 2023-05-09 00:04:13.124382 caterpillar_api-1.60/caterpillar_api.egg-info/
+-rw-r--r--   0 ldupin    (1000) ldupin    (1000)    14502 2023-05-09 00:04:13.000000 caterpillar_api-1.60/caterpillar_api.egg-info/PKG-INFO
+-rw-r--r--   0 ldupin    (1000) ldupin    (1000)      338 2023-05-09 00:04:13.000000 caterpillar_api-1.60/caterpillar_api.egg-info/SOURCES.txt
+-rw-r--r--   0 ldupin    (1000) ldupin    (1000)        1 2023-05-09 00:04:13.000000 caterpillar_api-1.60/caterpillar_api.egg-info/dependency_links.txt
+-rw-r--r--   0 ldupin    (1000) ldupin    (1000)        7 2023-05-09 00:04:13.000000 caterpillar_api-1.60/caterpillar_api.egg-info/requires.txt
+-rw-r--r--   0 ldupin    (1000) ldupin    (1000)       16 2023-05-09 00:04:13.000000 caterpillar_api-1.60/caterpillar_api.egg-info/top_level.txt
+-rwxr-xr-x   0 ldupin    (1000) ldupin    (1000)      117 2021-11-16 17:07:40.000000 caterpillar_api-1.60/release.sh
+-rw-r--r--   0 ldupin    (1000) ldupin    (1000)       50 2023-05-09 00:04:13.124382 caterpillar_api-1.60/setup.cfg
+-rw-r--r--   0 ldupin    (1000) ldupin    (1000)     1577 2023-05-09 00:04:10.000000 caterpillar_api-1.60/setup.py
+drwxr-xr-x   0 ldupin    (1000) ldupin    (1000)        0 2023-05-09 00:04:13.124382 caterpillar_api-1.60/tests/
+-rw-r--r--   0 ldupin    (1000) ldupin    (1000)      973 2021-11-15 06:33:08.000000 caterpillar_api-1.60/tests/all_test.py
```

### Comparing `caterpillar_api-1.6/LICENSE` & `caterpillar_api-1.60/LICENSE`

 * *Files identical despite different names*

### Comparing `caterpillar_api-1.6/PKG-INFO` & `caterpillar_api-1.60/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caterpillar_api
-Version: 1.6
+Version: 1.60
 Summary: 🐛 Caterpillar Api, field management for Django without the boiler-plate.
 Home-page: https://github.com/lukedupin/caterpillar
 Author: Luke Dupin
 Author-email: lukedupin@gmail.com
 License: MIT
 Keywords: DJANGO,API,REST,JSON,JSONP,JSON-P
 Classifier: Development Status :: 4 - Beta
```

### Comparing `caterpillar_api-1.6/README.md` & `caterpillar_api-1.60/README.md`

 * *Files identical despite different names*

### Comparing `caterpillar_api-1.6/caterpillar_api/__init__.py` & `caterpillar_api-1.60/caterpillar_api/__init__.py`

 * *Files identical despite different names*

### Comparing `caterpillar_api-1.6/caterpillar_api/monarch.py` & `caterpillar_api-1.60/caterpillar_api/monarch.py`

 * *Files identical despite different names*

### Comparing `caterpillar_api-1.6/caterpillar_api/util.py` & `caterpillar_api-1.60/caterpillar_api/util.py`

 * *Files identical despite different names*

### Comparing `caterpillar_api-1.6/caterpillar_api.egg-info/PKG-INFO` & `caterpillar_api-1.60/caterpillar_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caterpillar-api
-Version: 1.6
+Version: 1.60
 Summary: 🐛 Caterpillar Api, field management for Django without the boiler-plate.
 Home-page: https://github.com/lukedupin/caterpillar
 Author: Luke Dupin
 Author-email: lukedupin@gmail.com
 License: MIT
 Keywords: DJANGO,API,REST,JSON,JSONP,JSON-P
 Classifier: Development Status :: 4 - Beta
```

### Comparing `caterpillar_api-1.6/setup.py` & `caterpillar_api-1.60/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(
     name='caterpillar_api',
-    version='1.6',
+    version='1.60',
     packages=['caterpillar_api'],
     url='https://github.com/lukedupin/caterpillar',
     # I explain this later on
     license='MIT',
     author='Luke Dupin',
     author_email='lukedupin@gmail.com',
     description='🐛 Caterpillar Api, field management for Django without the boiler-plate.',
```

### Comparing `caterpillar_api-1.6/tests/all_test.py` & `caterpillar_api-1.60/tests/all_test.py`

 * *Files identical despite different names*

