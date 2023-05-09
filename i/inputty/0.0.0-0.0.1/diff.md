# Comparing `tmp/inputty-0.0.0.tar.gz` & `tmp/inputty-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inputty-0.0.0.tar", last modified: Tue May  9 13:30:23 2023, max compression
+gzip compressed data, was "inputty-0.0.1.tar", last modified: Tue May  9 13:41:37 2023, max compression
```

## Comparing `inputty-0.0.0.tar` & `inputty-0.0.1.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:30:23.310186 inputty-0.0.0/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 inputty-0.0.0/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)      560 2023-05-09 13:30:23.310186 inputty-0.0.0/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)       96 2023-05-09 13:23:03.000000 inputty-0.0.0/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:30:23.306853 inputty-0.0.0/inputty/
--rw-r--r--   0 jeff      (1000) jeff      (1001)       94 2023-05-09 13:20:34.000000 inputty-0.0.0/inputty/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-09 13:20:46.000000 inputty-0.0.0/inputty/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:30:23.306853 inputty-0.0.0/inputty.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      560 2023-05-09 13:30:23.000000 inputty-0.0.0/inputty.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      204 2023-05-09 13:30:23.000000 inputty-0.0.0/inputty.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-09 13:30:23.000000 inputty-0.0.0/inputty.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        8 2023-05-09 13:30:23.000000 inputty-0.0.0/inputty.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-09 13:30:23.310186 inputty-0.0.0/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1157 2023-05-09 13:25:02.000000 inputty-0.0.0/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:41:37.599414 inputty-0.0.1/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 inputty-0.0.1/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      613 2023-05-09 13:41:37.599414 inputty-0.0.1/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)       96 2023-05-09 13:23:03.000000 inputty-0.0.1/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:41:37.596080 inputty-0.0.1/inputty/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      123 2023-05-09 13:38:28.000000 inputty-0.0.1/inputty/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-09 13:40:50.000000 inputty-0.0.1/inputty/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:41:37.599414 inputty-0.0.1/inputty/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 inputty-0.0.1/inputty/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     6504 2023-05-09 13:39:54.000000 inputty-0.0.1/inputty/src/input.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:41:37.599414 inputty-0.0.1/inputty.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      613 2023-05-09 13:41:37.000000 inputty-0.0.1/inputty.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      249 2023-05-09 13:41:37.000000 inputty-0.0.1/inputty.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-09 13:41:37.000000 inputty-0.0.1/inputty.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        8 2023-05-09 13:41:37.000000 inputty-0.0.1/inputty.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-09 13:41:37.599414 inputty-0.0.1/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1157 2023-05-09 13:25:02.000000 inputty-0.0.1/setup.py
```

### Comparing `inputty-0.0.0/LICENSE.txt` & `inputty-0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inputty-0.0.0/PKG-INFO` & `inputty-0.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inputty
-Version: 0.0.0
+Version: 0.0.1
 Summary: """A collection of modules that supports cCLI inputs."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: cli,input
@@ -20,12 +20,18 @@
 ```bash
 pip install inputty
 ```
 
 
 # Version History
 
+Version 0.0.1 9 May 2023
+
+1. Improve access
+
+------
+
 Version 0.0.0 9 May 2023
 
 1. Initial version
 
 ------
```

### Comparing `inputty-0.0.0/inputty.egg-info/PKG-INFO` & `inputty-0.0.1/inputty.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inputty
-Version: 0.0.0
+Version: 0.0.1
 Summary: """A collection of modules that supports cCLI inputs."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: cli,input
@@ -20,12 +20,18 @@
 ```bash
 pip install inputty
 ```
 
 
 # Version History
 
+Version 0.0.1 9 May 2023
+
+1. Improve access
+
+------
+
 Version 0.0.0 9 May 2023
 
 1. Initial version
 
 ------
```

### Comparing `inputty-0.0.0/setup.py` & `inputty-0.0.1/setup.py`

 * *Files identical despite different names*

