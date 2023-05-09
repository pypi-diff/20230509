# Comparing `tmp/dequeai-0.775.tar.gz` & `tmp/dequeai-0.776.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.775.tar", last modified: Tue May  9 17:28:25 2023, max compression
+gzip compressed data, was "dequeai-0.776.tar", last modified: Tue May  9 18:24:44 2023, max compression
```

## Comparing `dequeai-0.775.tar` & `dequeai-0.776.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:28:25.956518 dequeai-0.775/
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-09 17:28:25.956518 dequeai-0.775/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:28:25.956518 dequeai-0.775/dequeai/
--rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.775/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.775/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.775/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.775/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.775/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    29683 2023-05-09 17:28:12.000000 dequeai-0.775/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.775/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.775/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.775/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.775/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:28:25.956518 dequeai-0.775/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-09 17:28:25.000000 dequeai-0.775/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-05-09 17:28:25.000000 dequeai-0.775/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 17:28:25.000000 dequeai-0.775/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-05-09 17:28:25.000000 dequeai-0.775/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-09 17:28:25.000000 dequeai-0.775/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 17:28:25.956518 dequeai-0.775/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      583 2023-05-09 17:28:12.000000 dequeai-0.775/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 18:24:44.068038 dequeai-0.776/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-09 18:24:44.068038 dequeai-0.776/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 18:24:44.064038 dequeai-0.776/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.776/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.776/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.776/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.776/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.776/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    29653 2023-05-09 18:24:30.000000 dequeai-0.776/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.776/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.776/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.776/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.776/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 18:24:44.068038 dequeai-0.776/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-09 18:24:43.000000 dequeai-0.776/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-05-09 18:24:44.000000 dequeai-0.776/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 18:24:43.000000 dequeai-0.776/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-05-09 18:24:43.000000 dequeai-0.776/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-09 18:24:43.000000 dequeai-0.776/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 18:24:44.068038 dequeai-0.776/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      583 2023-05-09 18:24:20.000000 dequeai-0.776/setup.py
```

### Comparing `dequeai-0.775/dequeai/datatypes.py` & `dequeai-0.776/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.775/dequeai/dequeai.py` & `dequeai-0.776/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.775/dequeai/dequeai_run.py` & `dequeai-0.776/dequeai/dequeai_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,16 +373,16 @@
             with open(file_name, "wb") as f:
                 f.write(http_response.content)
             print(f"Downloaded artifact '{file_name}'")
 
     def _validate_data(self, data):
         for key, value in data.items():
             if key is None:
-                del data[key]
-                #raise ValueError("Key cannot be None")
+
+                raise ValueError("Key cannot be None")
 
             if type(value) is dict:
                 self._validate_data(value)
             else:
                 if type(value) in [Audio, BoundingBox2D, Histogram, Table,
                                    Image] or type(value) in types.__builtins__.values():
                     pass
```

### Comparing `dequeai-0.775/dequeai/parsing_service.py` & `dequeai-0.776/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.775/dequeai/rest_connect.py` & `dequeai-0.776/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.775/dequeai/util.py` & `dequeai-0.776/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.775/setup.py` & `dequeai-0.776/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.00000775',
+    version='0.00000776',
     description='Python Experiment Tracking Package for Deque AI DLOps Platform',
     author="The Deque AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='deque client for experiment tracking, sweep and other deep learning tooling',
     install_requires=[
```

