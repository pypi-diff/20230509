# Comparing `tmp/stackmanager-1.4.2.tar.gz` & `tmp/stackmanager-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackmanager-1.4.2.tar", last modified: Mon May  1 15:39:43 2023, max compression
+gzip compressed data, was "stackmanager-1.4.3.tar", last modified: Tue May  9 16:44:00 2023, max compression
```

## Comparing `stackmanager-1.4.2.tar` & `stackmanager-1.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:39:43.613295 stackmanager-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-01 15:39:32.000000 stackmanager-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16207 2023-05-01 15:39:43.613295 stackmanager-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15788 2023-05-01 15:39:32.000000 stackmanager-1.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 15:39:43.613295 stackmanager-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-01 15:39:32.000000 stackmanager-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:39:43.613295 stackmanager-1.4.2/stackmanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12981 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/packager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21376 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:39:43.613295 stackmanager-1.4.2/stackmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16207 2023-05-01 15:39:43.000000 stackmanager-1.4.2/stackmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-01 15:39:43.000000 stackmanager-1.4.2/stackmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:39:43.000000 stackmanager-1.4.2/stackmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-01 15:39:43.000000 stackmanager-1.4.2/stackmanager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-01 15:39:43.000000 stackmanager-1.4.2/stackmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-01 15:39:43.000000 stackmanager-1.4.2/stackmanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:44:00.142841 stackmanager-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-09 16:43:42.000000 stackmanager-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16207 2023-05-09 16:44:00.142841 stackmanager-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15788 2023-05-09 16:43:42.000000 stackmanager-1.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 16:44:00.142841 stackmanager-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-09 16:43:42.000000 stackmanager-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:44:00.138841 stackmanager-1.4.3/stackmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:43:42.000000 stackmanager-1.4.3/stackmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12981 2023-05-09 16:43:43.000000 stackmanager-1.4.3/stackmanager/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-05-09 16:43:43.000000 stackmanager-1.4.3/stackmanager/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-09 16:43:43.000000 stackmanager-1.4.3/stackmanager/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-09 16:43:43.000000 stackmanager-1.4.3/stackmanager/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-09 16:43:43.000000 stackmanager-1.4.3/stackmanager/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-09 16:43:43.000000 stackmanager-1.4.3/stackmanager/packager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21376 2023-05-09 16:43:43.000000 stackmanager-1.4.3/stackmanager/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-09 16:43:43.000000 stackmanager-1.4.3/stackmanager/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-09 16:43:43.000000 stackmanager-1.4.3/stackmanager/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:44:00.142841 stackmanager-1.4.3/stackmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16207 2023-05-09 16:44:00.000000 stackmanager-1.4.3/stackmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-09 16:44:00.000000 stackmanager-1.4.3/stackmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:44:00.000000 stackmanager-1.4.3/stackmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-09 16:44:00.000000 stackmanager-1.4.3/stackmanager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-09 16:44:00.000000 stackmanager-1.4.3/stackmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 16:44:00.000000 stackmanager-1.4.3/stackmanager.egg-info/top_level.txt
```

### Comparing `stackmanager-1.4.2/LICENSE` & `stackmanager-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.2/PKG-INFO` & `stackmanager-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackmanager
-Version: 1.4.2
+Version: 1.4.3
 Summary: Utility to manage CloudFormation stacks using YAML configuration file
 Home-page: https://github.com/LeadingEDJE/stackmanager
 Author: Andrew May
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `stackmanager-1.4.2/README.md` & `stackmanager-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.2/setup.py` & `stackmanager-1.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.2/stackmanager/cli.py` & `stackmanager-1.4.3/stackmanager/cli.py`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.2/stackmanager/config.py` & `stackmanager-1.4.3/stackmanager/config.py`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.2/stackmanager/loader.py` & `stackmanager-1.4.3/stackmanager/loader.py`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.2/stackmanager/messages.py` & `stackmanager-1.4.3/stackmanager/messages.py`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.2/stackmanager/packager.py` & `stackmanager-1.4.3/stackmanager/packager.py`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.2/stackmanager/runner.py` & `stackmanager-1.4.3/stackmanager/runner.py`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.2/stackmanager/status.py` & `stackmanager-1.4.3/stackmanager/status.py`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.2/stackmanager/uploader.py` & `stackmanager-1.4.3/stackmanager/uploader.py`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.2/stackmanager.egg-info/PKG-INFO` & `stackmanager-1.4.3/stackmanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackmanager
-Version: 1.4.2
+Version: 1.4.3
 Summary: Utility to manage CloudFormation stacks using YAML configuration file
 Home-page: https://github.com/LeadingEDJE/stackmanager
 Author: Andrew May
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

