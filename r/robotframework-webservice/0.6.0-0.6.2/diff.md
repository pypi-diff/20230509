# Comparing `tmp/robotframework-webservice-0.6.0.tar.gz` & `tmp/robotframework-webservice-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-webservice-0.6.0.tar", last modified: Tue May  9 20:42:34 2023, max compression
+gzip compressed data, was "robotframework-webservice-0.6.2.tar", last modified: Tue May  9 20:45:05 2023, max compression
```

## Comparing `robotframework-webservice-0.6.0.tar` & `robotframework-webservice-0.6.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:42:34.672921 robotframework-webservice-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-05-09 20:42:19.000000 robotframework-webservice-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-09 20:42:34.672921 robotframework-webservice-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-09 20:42:19.000000 robotframework-webservice-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:42:34.668920 robotframework-webservice-0.6.0/RobotFrameworkService/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-09 20:42:19.000000 robotframework-webservice-0.6.0/RobotFrameworkService/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-09 20:42:19.000000 robotframework-webservice-0.6.0/RobotFrameworkService/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-09 20:42:19.000000 robotframework-webservice-0.6.0/RobotFrameworkService/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-09 20:42:19.000000 robotframework-webservice-0.6.0/RobotFrameworkService/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:42:34.668920 robotframework-webservice-0.6.0/RobotFrameworkService/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 20:42:19.000000 robotframework-webservice-0.6.0/RobotFrameworkService/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-09 20:42:19.000000 robotframework-webservice-0.6.0/RobotFrameworkService/routers/robotframework.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-09 20:42:19.000000 robotframework-webservice-0.6.0/RobotFrameworkService/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:42:34.672921 robotframework-webservice-0.6.0/robotframework_webservice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-09 20:42:34.000000 robotframework-webservice-0.6.0/robotframework_webservice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-09 20:42:34.000000 robotframework-webservice-0.6.0/robotframework_webservice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:42:34.000000 robotframework-webservice-0.6.0/robotframework_webservice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:42:34.000000 robotframework-webservice-0.6.0/robotframework_webservice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 20:42:34.000000 robotframework-webservice-0.6.0/robotframework_webservice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 20:42:34.000000 robotframework-webservice-0.6.0/robotframework_webservice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 20:42:34.672921 robotframework-webservice-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-09 20:42:19.000000 robotframework-webservice-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:45:05.510676 robotframework-webservice-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-09 20:45:05.510676 robotframework-webservice-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:45:05.510676 robotframework-webservice-0.6.2/RobotFrameworkService/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/RobotFrameworkService/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/RobotFrameworkService/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/RobotFrameworkService/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/RobotFrameworkService/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:45:05.510676 robotframework-webservice-0.6.2/RobotFrameworkService/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/RobotFrameworkService/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/RobotFrameworkService/routers/robotframework.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/RobotFrameworkService/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:45:05.510676 robotframework-webservice-0.6.2/robotframework_webservice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-09 20:45:05.000000 robotframework-webservice-0.6.2/robotframework_webservice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-09 20:45:05.000000 robotframework-webservice-0.6.2/robotframework_webservice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:45:05.000000 robotframework-webservice-0.6.2/robotframework_webservice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:45:05.000000 robotframework-webservice-0.6.2/robotframework_webservice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 20:45:05.000000 robotframework-webservice-0.6.2/robotframework_webservice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 20:45:05.000000 robotframework-webservice-0.6.2/robotframework_webservice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 20:45:05.510676 robotframework-webservice-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-09 20:44:48.000000 robotframework-webservice-0.6.2/setup.py
```

### Comparing `robotframework-webservice-0.6.0/LICENSE` & `robotframework-webservice-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-webservice-0.6.0/PKG-INFO` & `robotframework-webservice-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-webservice
-Version: 0.6.0
+Version: 0.6.2
 Summary: Webservice for running Robot Framework tasks
 Home-page: https://github.com/MarketSquare/robotframework-webservice
 Author: Markus Stahl
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: FastAPI
```

### Comparing `robotframework-webservice-0.6.0/README.md` & `robotframework-webservice-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-webservice-0.6.0/RobotFrameworkService/Config.py` & `robotframework-webservice-0.6.2/RobotFrameworkService/Config.py`

 * *Files identical despite different names*

### Comparing `robotframework-webservice-0.6.0/RobotFrameworkService/main.py` & `robotframework-webservice-0.6.2/RobotFrameworkService/main.py`

 * *Files identical despite different names*

### Comparing `robotframework-webservice-0.6.0/RobotFrameworkService/routers/robotframework.py` & `robotframework-webservice-0.6.2/RobotFrameworkService/routers/robotframework.py`

 * *Files identical despite different names*

### Comparing `robotframework-webservice-0.6.0/robotframework_webservice.egg-info/PKG-INFO` & `robotframework-webservice-0.6.2/robotframework_webservice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-webservice
-Version: 0.6.0
+Version: 0.6.2
 Summary: Webservice for running Robot Framework tasks
 Home-page: https://github.com/MarketSquare/robotframework-webservice
 Author: Markus Stahl
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: FastAPI
```

### Comparing `robotframework-webservice-0.6.0/robotframework_webservice.egg-info/SOURCES.txt` & `robotframework-webservice-0.6.2/robotframework_webservice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-webservice-0.6.0/setup.py` & `robotframework-webservice-0.6.2/setup.py`

 * *Files identical despite different names*

