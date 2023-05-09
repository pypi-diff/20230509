# Comparing `tmp/dequeai-0.772.tar.gz` & `tmp/dequeai-0.774.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.772.tar", last modified: Fri Apr 28 14:37:12 2023, max compression
+gzip compressed data, was "dequeai-0.774.tar", last modified: Tue May  9 17:23:28 2023, max compression
```

## Comparing `dequeai-0.772.tar` & `dequeai-0.774.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:37:12.671929 dequeai-0.772/
--rw-r--r--   0 root         (0) root         (0)      319 2023-04-28 14:37:12.671929 dequeai-0.772/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:37:12.671929 dequeai-0.772/dequeai/
--rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.772/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.772/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.772/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.772/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.772/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    29568 2023-04-28 14:36:44.000000 dequeai-0.772/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.772/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.772/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.772/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.772/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:37:12.671929 dequeai-0.772/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      319 2023-04-28 14:37:12.000000 dequeai-0.772/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-28 14:37:12.000000 dequeai-0.772/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 14:37:12.000000 dequeai-0.772/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-28 14:37:12.000000 dequeai-0.772/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-28 14:37:12.000000 dequeai-0.772/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 14:37:12.671929 dequeai-0.772/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      494 2023-04-28 14:36:57.000000 dequeai-0.772/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:23:28.317091 dequeai-0.774/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-09 17:23:28.317091 dequeai-0.774/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:23:28.317091 dequeai-0.774/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.774/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.774/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.774/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.774/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.774/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    29652 2023-05-09 17:23:12.000000 dequeai-0.774/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.774/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.774/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.774/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.774/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:23:28.317091 dequeai-0.774/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-09 17:23:27.000000 dequeai-0.774/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-05-09 17:23:28.000000 dequeai-0.774/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 17:23:27.000000 dequeai-0.774/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-05-09 17:23:28.000000 dequeai-0.774/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-09 17:23:28.000000 dequeai-0.774/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 17:23:28.317091 dequeai-0.774/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      583 2023-05-03 22:42:09.000000 dequeai-0.774/setup.py
```

### Comparing `dequeai-0.772/dequeai/datatypes.py` & `dequeai-0.774/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.772/dequeai/dequeai.py` & `dequeai-0.774/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.772/dequeai/dequeai_run.py` & `dequeai-0.774/dequeai/dequeai_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,14 +372,17 @@
             file_name = os.path.basename(artifact_uri)
             with open(file_name, "wb") as f:
                 f.write(http_response.content)
             print(f"Downloaded artifact '{file_name}'")
 
     def _validate_data(self, data):
         for key, value in data.items():
+            if key is None:
+                raise ValueError("Key cannot be None")
+
             if type(value) is dict:
                 self._validate_data(value)
             else:
                 if type(value) in [Audio, BoundingBox2D, Histogram, Table,
                                    Image] or type(value) in types.__builtins__.values():
                     pass
                 else:
```

### Comparing `dequeai-0.772/dequeai/parsing_service.py` & `dequeai-0.774/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.772/dequeai/rest_connect.py` & `dequeai-0.774/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.772/dequeai/util.py` & `dequeai-0.774/dequeai/util.py`

 * *Files identical despite different names*

