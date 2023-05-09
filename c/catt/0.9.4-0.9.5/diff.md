# Comparing `tmp/catt-0.9.4.tar.gz` & `tmp/catt-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/catt-0.9.4.tar", last modified: Tue Mar 26 13:43:45 2019, max compression
+gzip compressed data, was "dist/catt-0.9.5.tar", last modified: Tue Mar 26 13:57:01 2019, max compression
```

## Comparing `catt-0.9.4.tar` & `catt-0.9.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2019-03-26 13:43:45.000000 catt-0.9.4/
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      160 2019-03-24 00:15:23.000000 catt-0.9.4/AUTHORS.rst
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      262 2016-04-24 15:56:44.000000 catt-0.9.4/MANIFEST.in
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     3172 2016-04-24 23:50:19.000000 catt-0.9.4/CONTRIBUTING.rst
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     1325 2019-03-24 00:15:23.000000 catt-0.9.4/LICENSE
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     1692 2019-03-24 00:35:34.000000 catt-0.9.4/setup.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     6126 2019-03-26 13:43:45.000000 catt-0.9.4/PKG-INFO
-drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2019-03-26 13:43:45.000000 catt-0.9.4/catt/
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     1680 2019-03-24 00:15:23.000000 catt-0.9.4/catt/error.py
--rwxrwxr-x   0 stavros   (1000) stavros   (1000)    17624 2019-03-26 13:37:27.000000 catt-0.9.4/catt/cli.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)    21175 2019-03-24 00:15:23.000000 catt-0.9.4/catt/controllers.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     2846 2019-03-24 00:15:23.000000 catt-0.9.4/catt/util.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      233 2019-03-26 13:42:01.000000 catt-0.9.4/catt/__init__.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     6859 2019-03-24 00:15:23.000000 catt-0.9.4/catt/stream_info.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     3914 2019-03-26 13:04:28.000000 catt-0.9.4/catt/http_server.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     4684 2019-03-24 00:15:23.000000 catt-0.9.4/catt/api.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     4256 2019-03-24 00:15:23.000000 catt-0.9.4/README.rst
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      429 2019-03-26 13:43:45.000000 catt-0.9.4/setup.cfg
-drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2019-03-26 13:43:45.000000 catt-0.9.4/tests/
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     1596 2018-10-24 10:00:49.000000 catt-0.9.4/tests/test_catt.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)       24 2016-04-24 15:56:44.000000 catt-0.9.4/tests/__init__.py
-drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2019-03-26 13:43:45.000000 catt-0.9.4/catt.egg-info/
--rw-rw-r--   0 stavros   (1000) stavros   (1000)        1 2019-03-26 13:43:45.000000 catt-0.9.4/catt.egg-info/not-zip-safe
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     6126 2019-03-26 13:43:45.000000 catt-0.9.4/catt.egg-info/PKG-INFO
--rw-rw-r--   0 stavros   (1000) stavros   (1000)        1 2019-03-26 13:43:45.000000 catt-0.9.4/catt.egg-info/dependency_links.txt
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      119 2019-03-26 13:43:45.000000 catt-0.9.4/catt.egg-info/requires.txt
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      440 2019-03-26 13:43:45.000000 catt-0.9.4/catt.egg-info/SOURCES.txt
--rw-rw-r--   0 stavros   (1000) stavros   (1000)       40 2019-03-26 13:43:45.000000 catt-0.9.4/catt.egg-info/entry_points.txt
--rw-rw-r--   0 stavros   (1000) stavros   (1000)        5 2019-03-26 13:43:45.000000 catt-0.9.4/catt.egg-info/top_level.txt
+drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2019-03-26 13:57:01.000000 catt-0.9.5/
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      160 2019-03-24 00:15:23.000000 catt-0.9.5/AUTHORS.rst
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      262 2016-04-24 15:56:44.000000 catt-0.9.5/MANIFEST.in
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     3172 2016-04-24 23:50:19.000000 catt-0.9.5/CONTRIBUTING.rst
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     1325 2019-03-24 00:15:23.000000 catt-0.9.5/LICENSE
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     1721 2019-03-26 13:56:01.000000 catt-0.9.5/setup.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     6149 2019-03-26 13:57:01.000000 catt-0.9.5/PKG-INFO
+drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2019-03-26 13:57:01.000000 catt-0.9.5/catt/
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     1680 2019-03-24 00:15:23.000000 catt-0.9.5/catt/error.py
+-rwxrwxr-x   0 stavros   (1000) stavros   (1000)    17624 2019-03-26 13:37:27.000000 catt-0.9.5/catt/cli.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)    21175 2019-03-24 00:15:23.000000 catt-0.9.5/catt/controllers.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     2846 2019-03-24 00:15:23.000000 catt-0.9.5/catt/util.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      233 2019-03-26 13:56:42.000000 catt-0.9.5/catt/__init__.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     6859 2019-03-24 00:15:23.000000 catt-0.9.5/catt/stream_info.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     3914 2019-03-26 13:04:28.000000 catt-0.9.5/catt/http_server.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     4684 2019-03-24 00:15:23.000000 catt-0.9.5/catt/api.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     4256 2019-03-24 00:15:23.000000 catt-0.9.5/README.rst
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      497 2019-03-26 13:57:01.000000 catt-0.9.5/setup.cfg
+drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2019-03-26 13:57:01.000000 catt-0.9.5/tests/
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     1596 2018-10-24 10:00:49.000000 catt-0.9.5/tests/test_catt.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)       24 2016-04-24 15:56:44.000000 catt-0.9.5/tests/__init__.py
+drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2019-03-26 13:57:01.000000 catt-0.9.5/catt.egg-info/
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)        1 2019-03-26 13:57:01.000000 catt-0.9.5/catt.egg-info/not-zip-safe
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     6149 2019-03-26 13:57:01.000000 catt-0.9.5/catt.egg-info/PKG-INFO
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)        1 2019-03-26 13:57:01.000000 catt-0.9.5/catt.egg-info/dependency_links.txt
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      119 2019-03-26 13:57:01.000000 catt-0.9.5/catt.egg-info/requires.txt
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      440 2019-03-26 13:57:01.000000 catt-0.9.5/catt.egg-info/SOURCES.txt
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)       40 2019-03-26 13:57:01.000000 catt-0.9.5/catt.egg-info/entry_points.txt
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)        5 2019-03-26 13:57:01.000000 catt-0.9.5/catt.egg-info/top_level.txt
```

### Comparing `catt-0.9.4/CONTRIBUTING.rst` & `catt-0.9.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `catt-0.9.4/LICENSE` & `catt-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `catt-0.9.4/setup.py` & `catt-0.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,9 +55,10 @@
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
     ],
     test_suite="tests",
     tests_require=test_requirements,
+    python_requires=">=3.4",
     entry_points={"console_scripts": ["catt=catt.cli:main"]},
 )
```

### Comparing `catt-0.9.4/PKG-INFO` & `catt-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: catt
-Version: 0.9.4
+Version: 0.9.5
 Summary: Cast All The Things allows you to send videos from many, many online sources to your Chromecast.
 Home-page: https://github.com/skorokithakis/catt
 Author: Stavros Korokithakis
 Author-email: hi@stavros.io
 License: BSD
 Description: ===============================
         Cast All The Things
@@ -149,7 +149,8 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3.4
```

### Comparing `catt-0.9.4/catt/error.py` & `catt-0.9.5/catt/error.py`

 * *Files identical despite different names*

### Comparing `catt-0.9.4/catt/cli.py` & `catt-0.9.5/catt/cli.py`

 * *Files identical despite different names*

### Comparing `catt-0.9.4/catt/controllers.py` & `catt-0.9.5/catt/controllers.py`

 * *Files identical despite different names*

### Comparing `catt-0.9.4/catt/util.py` & `catt-0.9.5/catt/util.py`

 * *Files identical despite different names*

### Comparing `catt-0.9.4/catt/stream_info.py` & `catt-0.9.5/catt/stream_info.py`

 * *Files identical despite different names*

### Comparing `catt-0.9.4/catt/http_server.py` & `catt-0.9.5/catt/http_server.py`

 * *Files identical despite different names*

### Comparing `catt-0.9.4/catt/api.py` & `catt-0.9.5/catt/api.py`

 * *Files identical despite different names*

### Comparing `catt-0.9.4/README.rst` & `catt-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `catt-0.9.4/tests/test_catt.py` & `catt-0.9.5/tests/test_catt.py`

 * *Files identical despite different names*

### Comparing `catt-0.9.4/catt.egg-info/PKG-INFO` & `catt-0.9.5/catt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: catt
-Version: 0.9.4
+Version: 0.9.5
 Summary: Cast All The Things allows you to send videos from many, many online sources to your Chromecast.
 Home-page: https://github.com/skorokithakis/catt
 Author: Stavros Korokithakis
 Author-email: hi@stavros.io
 License: BSD
 Description: ===============================
         Cast All The Things
@@ -149,7 +149,8 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3.4
```

