# Comparing `tmp/microgue-2.0.4.tar.gz` & `tmp/microgue-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/microgue-2.0.4.tar", last modified: Fri May  5 18:43:05 2023, max compression
+gzip compressed data, was "dist/microgue-2.0.5.tar", last modified: Tue May  9 14:30:13 2023, max compression
```

## Comparing `microgue-2.0.4.tar` & `microgue-2.0.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/
--rw-r--r--   0 mhudelso   (501) staff       (20)     3060 2023-05-05 18:43:05.000000 microgue-2.0.4/PKG-INFO
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/storages/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/storages/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     3789 2023-05-05 18:16:25.000000 microgue-2.0.4/microgue/storages/abstract_storage.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/loggers/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/loggers/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1412 2023-05-05 17:01:37.000000 microgue-2.0.4/microgue/loggers/logger.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/security/
--rw-r--r--   0 mhudelso   (501) staff       (20)      334 2023-04-30 02:18:57.000000 microgue-2.0.4/microgue/security/generic.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/security/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/secrets/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/secrets/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1065 2023-05-05 17:12:46.000000 microgue-2.0.4/microgue/secrets/secrets.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/constants/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/constants/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)      378 2022-09-21 19:29:50.000000 microgue-2.0.4/microgue/constants/error_constants.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/objects/
--rw-r--r--   0 mhudelso   (501) staff       (20)     8817 2023-05-02 02:23:16.000000 microgue-2.0.4/microgue/objects/abstract_model_object.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     2707 2023-05-05 18:41:01.000000 microgue-2.0.4/microgue/objects/object.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/objects/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1483 2023-05-02 01:54:14.000000 microgue-2.0.4/microgue/objects/abstract_expiring_model_object.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/models/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/models/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)    10632 2023-05-05 18:33:37.000000 microgue-2.0.4/microgue/models/abstract_model.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     2737 2023-05-02 02:25:32.000000 microgue-2.0.4/microgue/utils.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/queues/
--rw-r--r--   0 mhudelso   (501) staff       (20)     3155 2023-05-05 18:16:25.000000 microgue-2.0.4/microgue/queues/abstract_queue.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/queues/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/events/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-03-09 20:40:18.000000 microgue-2.0.4/microgue/events/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1947 2023-05-05 18:16:25.000000 microgue-2.0.4/microgue/events/abstract_event_bus.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     5220 2023-05-02 01:51:02.000000 microgue-2.0.4/microgue/abstract_app.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/services/
--rw-r--r--   0 mhudelso   (501) staff       (20)     4053 2023-05-05 18:26:11.000000 microgue-2.0.4/microgue/services/service.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/services/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/caches/
--rw-r--r--   0 mhudelso   (501) staff       (20)     3189 2023-05-05 18:16:25.000000 microgue-2.0.4/microgue/caches/abstract_cache.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/caches/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1907 2022-09-27 19:27:36.000000 microgue-2.0.4/README.md
--rw-r--r--   0 mhudelso   (501) staff       (20)      640 2023-05-05 18:42:45.000000 microgue-2.0.4/setup.py
--rw-r--r--   0 mhudelso   (501) staff       (20)       38 2023-05-05 18:43:05.000000 microgue-2.0.4/setup.cfg
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue.egg-info/
--rw-r--r--   0 mhudelso   (501) staff       (20)     3060 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue.egg-info/PKG-INFO
--rw-r--r--   0 mhudelso   (501) staff       (20)     1010 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue.egg-info/SOURCES.txt
--rw-r--r--   0 mhudelso   (501) staff       (20)       42 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue.egg-info/requires.txt
--rw-r--r--   0 mhudelso   (501) staff       (20)        9 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue.egg-info/top_level.txt
--rw-r--r--   0 mhudelso   (501) staff       (20)        1 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue.egg-info/dependency_links.txt
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-09 14:30:13.000000 microgue-2.0.5/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3060 2023-05-09 14:30:13.000000 microgue-2.0.5/PKG-INFO
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-09 14:30:13.000000 microgue-2.0.5/microgue/
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-09 14:30:13.000000 microgue-2.0.5/microgue/storages/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.5/microgue/storages/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3886 2023-05-09 14:20:16.000000 microgue-2.0.5/microgue/storages/abstract_storage.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-09 14:30:13.000000 microgue-2.0.5/microgue/loggers/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.5/microgue/loggers/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1412 2023-05-05 17:01:37.000000 microgue-2.0.5/microgue/loggers/logger.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-09 14:30:13.000000 microgue-2.0.5/microgue/security/
+-rw-r--r--   0 mhudelso   (501) staff       (20)      334 2023-04-30 02:18:57.000000 microgue-2.0.5/microgue/security/generic.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.5/microgue/security/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-09 14:30:13.000000 microgue-2.0.5/microgue/secrets/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.5/microgue/secrets/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1065 2023-05-05 17:12:46.000000 microgue-2.0.5/microgue/secrets/secrets.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-09 14:30:13.000000 microgue-2.0.5/microgue/constants/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.5/microgue/constants/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)      378 2022-09-21 19:29:50.000000 microgue-2.0.5/microgue/constants/error_constants.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.5/microgue/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-09 14:30:13.000000 microgue-2.0.5/microgue/objects/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     8817 2023-05-02 02:23:16.000000 microgue-2.0.5/microgue/objects/abstract_model_object.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     2707 2023-05-05 18:41:01.000000 microgue-2.0.5/microgue/objects/object.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.5/microgue/objects/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1483 2023-05-02 01:54:14.000000 microgue-2.0.5/microgue/objects/abstract_expiring_model_object.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-09 14:30:13.000000 microgue-2.0.5/microgue/models/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.5/microgue/models/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)    10735 2023-05-09 14:20:16.000000 microgue-2.0.5/microgue/models/abstract_model.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     2737 2023-05-02 02:25:32.000000 microgue-2.0.5/microgue/utils.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-09 14:30:13.000000 microgue-2.0.5/microgue/queues/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3335 2023-05-09 14:20:16.000000 microgue-2.0.5/microgue/queues/abstract_queue.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.5/microgue/queues/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-09 14:30:13.000000 microgue-2.0.5/microgue/events/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-03-09 20:40:18.000000 microgue-2.0.5/microgue/events/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     2150 2023-05-09 14:20:16.000000 microgue-2.0.5/microgue/events/abstract_event_bus.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     5214 2023-05-09 14:02:06.000000 microgue-2.0.5/microgue/abstract_app.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-09 14:30:13.000000 microgue-2.0.5/microgue/services/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     4053 2023-05-05 18:26:11.000000 microgue-2.0.5/microgue/services/service.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.5/microgue/services/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-09 14:30:13.000000 microgue-2.0.5/microgue/caches/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3289 2023-05-09 14:20:16.000000 microgue-2.0.5/microgue/caches/abstract_cache.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.5/microgue/caches/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1907 2022-09-27 19:27:36.000000 microgue-2.0.5/README.md
+-rw-r--r--   0 mhudelso   (501) staff       (20)      640 2023-05-09 14:29:44.000000 microgue-2.0.5/setup.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)       38 2023-05-09 14:30:13.000000 microgue-2.0.5/setup.cfg
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-09 14:30:13.000000 microgue-2.0.5/microgue.egg-info/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3060 2023-05-09 14:30:13.000000 microgue-2.0.5/microgue.egg-info/PKG-INFO
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1010 2023-05-09 14:30:13.000000 microgue-2.0.5/microgue.egg-info/SOURCES.txt
+-rw-r--r--   0 mhudelso   (501) staff       (20)       42 2023-05-09 14:30:13.000000 microgue-2.0.5/microgue.egg-info/requires.txt
+-rw-r--r--   0 mhudelso   (501) staff       (20)        9 2023-05-09 14:30:13.000000 microgue-2.0.5/microgue.egg-info/top_level.txt
+-rw-r--r--   0 mhudelso   (501) staff       (20)        1 2023-05-09 14:30:13.000000 microgue-2.0.5/microgue.egg-info/dependency_links.txt
```

### Comparing `microgue-2.0.4/PKG-INFO` & `microgue-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microgue
-Version: 2.0.4
+Version: 2.0.5
 Summary: This project contains bootstrap code to speed up the development of AWS based microservices
 Home-page: UNKNOWN
 Author: Michael Hudelson
 Author-email: michaelhudelson@gmail.com
 License: MIT
 Description: # AWS Microservice Bootstrap Code
```

### Comparing `microgue-2.0.4/microgue/storages/abstract_storage.py` & `microgue-2.0.5/microgue/storages/abstract_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,18 +29,19 @@
 
     def __init__(self, *args, **kwargs):
         logger.debug(f"{self.__class__.__name__}.__init__", priority=2)
         logger.debug(f"AbstractStorage.storage: {AbstractStorage.storage}")
         try:
             if AbstractStorage.storage is None:
                 # share the storage connection at the application level
-                logger.debug("connecting to s3")
+                logger.debug("connecting to s3", priority=3)
                 AbstractStorage.storage = boto3.client("s3")
+                logger.debug("successfully connected to s3", priority=3)
             else:
-                logger.debug("using existing connection to s3")
+                logger.debug("using existing connection to s3", priority=3)
         except Exception as e:
             logger.error(f"{self.__class__.__name__}.__init__ - error", priority=3)
             logger.error(f"{e.__class__.__name__}: {str(e)}")
             raise StorageConnectionFailed(str(e))
 
     def upload(self, local_file_path, remote_file_path=None):
         if remote_file_path is None:
```

### Comparing `microgue-2.0.4/microgue/loggers/logger.py` & `microgue-2.0.5/microgue/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.4/microgue/secrets/secrets.py` & `microgue-2.0.5/microgue/secrets/secrets.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.4/microgue/objects/abstract_model_object.py` & `microgue-2.0.5/microgue/objects/abstract_model_object.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.4/microgue/objects/object.py` & `microgue-2.0.5/microgue/objects/object.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.4/microgue/objects/abstract_expiring_model_object.py` & `microgue-2.0.5/microgue/objects/abstract_expiring_model_object.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.4/microgue/models/abstract_model.py` & `microgue-2.0.5/microgue/models/abstract_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,18 +51,19 @@
     mask_attributes = []
 
     def __init__(self, *args, **kwargs):
         logger.debug(f"{self.__class__.__name__}.__init__", priority=2)
         logger.debug(f"AbstractModel.database: {AbstractModel.database}")
         try:
             if AbstractModel.database is None:
-                logger.debug("connecting to dynamodb")
+                logger.debug("connecting to dynamodb", priority=3)
                 AbstractModel.database = boto3.resource("dynamodb")
+                logger.debug("successfully connected to dynamodb", priority=3)
             else:
-                logger.debug("using existing connection to dynamodb")
+                logger.debug("using existing connection to dynamodb", priority=3)
 
             self.table = AbstractModel.database.Table(self.table_name)
         except Exception as e:
             logger.error(f"{self.__class__.__name__}.__init__ - error", priority=3)
             logger.error(f"{e.__class__.__name__}: {str(e)}")
             raise DatabaseConnectionFailed(str(e))
         super().__init__(*args, **kwargs)
```

### Comparing `microgue-2.0.4/microgue/utils.py` & `microgue-2.0.5/microgue/utils.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.4/microgue/queues/abstract_queue.py` & `microgue-2.0.5/microgue/queues/abstract_queue.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,32 +18,34 @@
 
     def __init__(self, *args, **kwargs):
         logger.debug(f"{self.__class__.__name__}.__init__", priority=2)
         logger.debug(f"AbstractQueue.queue: {AbstractQueue.queue}")
         try:
             if AbstractQueue.queue is None:
                 # share the queue connection at the application level
-                logger.debug("connecting to sqs")
+                logger.debug("connecting to sqs", priority=3)
                 AbstractQueue.queue = boto3.client("sqs")
+                logger.debug("successfully connected to sqs", priority=3)
             else:
-                logger.debug("using existing connection to sqs")
+                logger.debug("using existing connection to sqs", priority=3)
         except Exception as e:
             logger.error(f"{self.__class__.__name__}.__init__ - error", priority=3)
             logger.error(f"{e.__class__.__name__}: {str(e)}")
             raise QueueConnectionFailed(str(e))
 
     def send(self, message):
         logger.debug(f"{self.__class__.__name__}.send", priority=2)
         if type(message) is dict:
             message = json.dumps(message)
         try:
             self.queue.send_message(
                 QueueUrl=self.queue_url,
                 MessageBody=message
             )
+            logger.error(f"{self.__class__.__name__}.send - success", priority=3)
         except Exception as e:
             logger.error(f"{self.__class__.__name__}.send - failed", priority=3)
             logger.error(f"{e.__class__.__name__}: {str(e)}")
             return False
         return True
 
     def receive(self, max_number_of_messages=1, visibility_timeout=1, wait_time=1):
```

### Comparing `microgue-2.0.4/microgue/events/abstract_event_bus.py` & `microgue-2.0.5/microgue/events/abstract_event_bus.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 
     def __init__(self, *args, **kwargs):
         logger.debug(f"{self.__class__.__name__}.__init__", priority=2)
         logger.debug(f"AbstractEventBus.event_bus: {AbstractEventBus.event_bus}")
         try:
             if AbstractEventBus.event_bus is None:
                 # share the event bus connection at the application level
-                logger.debug("connecting to eventbridge")
+                logger.debug("connecting to eventbridge", priority=3)
                 AbstractEventBus.event_bus = boto3.client(service_name="events", region_name=self.event_bus_region)
+                logger.debug("successfully connected to eventbridge", priority=3)
             else:
-                logger.debug("using existing connection to eventbridge")
+                logger.debug("using existing connection to eventbridge", priority=3)
         except Exception as e:
             logger.error(f"{self.__class__.__name__}.__init__ - error", priority=3)
             logger.error(f"{e.__class__.__name__}: {str(e)}")
             raise EventBusConnectionFailed(str(e))
 
     def publish(self, event_type, event_data=None):
         # defaults
@@ -46,11 +47,12 @@
                 "DetailType": event_type,
                 "Detail": json.dumps(event_data),
                 "EventBusName": self.event_bus_name
             }]
         )
 
         if response.get("ResponseMetadata", {}).get("HTTPStatusCode") == 200:
+            logger.debug(f"{self.__class__.__name__}.publish - success", priority=3)
             return True
         else:
-            logger.critical(f"{self.__class__.__name__}.publish - failed")
+            logger.critical(f"{self.__class__.__name__}.publish - failed", priority=3)
             return False
```

### Comparing `microgue-2.0.4/microgue/abstract_app.py` & `microgue-2.0.5/microgue/abstract_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import traceback
 from .constants.error_constants import ErrorConstants
-from flask import Flask, request, Response, g
+from flask import Flask, request, g
 from .loggers.logger import Logger
 from .security.generic import is_allowed_by_all
 from werkzeug.exceptions import Unauthorized, Forbidden, NotFound, MethodNotAllowed
 from .utils import JSONResponse
 
 logger = Logger()
 
@@ -75,15 +75,15 @@
 
     def register_after_request_handler(self):
         self.app.after_request(self.after_request_handler)
 
     @staticmethod
     def after_request_handler(response):
         if not g.get("authenticated") and int(response.status_code) < 400:
-            response = Response(json.dumps({"error": ErrorConstants.App.UNABLE_TO_AUTHENTICATE}), status=401)
+            response = JSONResponse(json.dumps({"error": ErrorConstants.App.UNABLE_TO_AUTHENTICATE}), status=401)
 
         logger.debug("Response Sent", priority=1)
         logger.debug(f"status: {response.status}")
         logger.debug(f"headers: {response.headers}")
         logger.debug(f"body: {response.response}")
 
         return response
```

### Comparing `microgue-2.0.4/microgue/services/service.py` & `microgue-2.0.5/microgue/services/service.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.4/microgue/caches/abstract_cache.py` & `microgue-2.0.5/microgue/caches/abstract_cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,19 +25,20 @@
 
     def __init__(self, *args, **kwargs):
         logger.debug(f"{self.__class__.__name__}.__init__", priority=2)
         logger.debug(f"self.__class__.cache: {self.__class__.cache}")
         try:
             if self.__class__.cache is None:
                 # share the cache connection at the __class__ level
-                logger.debug("connecting to redis")
+                logger.debug("connecting to redis", priority=3)
                 self.__class__.cache = redis.StrictRedis(host=self.host, port=self.port, socket_connect_timeout=self.connection_timeout)
                 self.__class__.cache.ping()
+                logger.debug("successfully connected to redis", priority=3)
             else:
-                logger.debug("using existing connection to redis")
+                logger.debug("using existing connection to redis", priority=3)
         except Exception as e:
             logger.error(f"{self.__class__.__name__}.__init__ - error", priority=3)
             logger.error(f"{e.__class__.__name__}: {str(e)}")
             if self.connection_required:
                 raise CacheConnectionFailed(str(e))
             else:
                 self.__class__.cache = None
@@ -49,16 +50,16 @@
             return key
 
     def get(self, key):
         if self.cache:
             prefixed_key = self._prefix_key(key)
             value = self.cache.get(prefixed_key)
             logger.debug(f"{self.__class__.__name__}.get", priority=2)
-            logger.debug(f"Key: {prefixed_key}")
-            logger.debug(f"Value: {value}")
+            logger.debug(f"key: {prefixed_key}")
+            logger.debug(f"value: {value}")
             try:
                 return json.loads(value)
             except:  # noqa
                 pass
             try:
                 return value.decode("ascii")
             except:  # noqa
@@ -67,24 +68,24 @@
 
     def set(self, key, value, ttl=None):
         if self.cache:
             value = value if type(value) is str else json.dumps(value)
             prefixed_key = self._prefix_key(key)
             ttl = ttl if ttl is not None else self.ttl
             logger.debug(f"{self.__class__.__name__}.set", priority=2)
-            logger.debug(f"Key: {prefixed_key}")
-            logger.debug(f"Value: {value}")
+            logger.debug(f"key: {prefixed_key}")
+            logger.debug(f"value: {value}")
             self.cache.set(prefixed_key, value, ex=ttl)
             return True
 
     def delete(self, key):
         if self.cache:
             prefixed_key = self._prefix_key(key)
             logger.debug(f"{self.__class__.__name__}.delete", priority=2)
-            logger.debug(f"Key: {prefixed_key}")
+            logger.debug(f"key: {prefixed_key}")
             return bool(self.cache.delete(prefixed_key))
 
     def expires_at(self, key):
         if self.cache:
             prefixed_key = self._prefix_key(key)
             expire_time = self.cache.ttl(prefixed_key)
             return str(datetime.timedelta(seconds=expire_time))
```

### Comparing `microgue-2.0.4/README.md` & `microgue-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `microgue-2.0.4/setup.py` & `microgue-2.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="microgue",
-    version="2.0.4",
+    version="2.0.5",
     author="Michael Hudelson",
     author_email="michaelhudelson@gmail.com",
     description="This project contains bootstrap code to speed up the development of AWS based microservices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     packages=find_packages(),
```

### Comparing `microgue-2.0.4/microgue.egg-info/PKG-INFO` & `microgue-2.0.5/microgue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microgue
-Version: 2.0.4
+Version: 2.0.5
 Summary: This project contains bootstrap code to speed up the development of AWS based microservices
 Home-page: UNKNOWN
 Author: Michael Hudelson
 Author-email: michaelhudelson@gmail.com
 License: MIT
 Description: # AWS Microservice Bootstrap Code
```

### Comparing `microgue-2.0.4/microgue.egg-info/SOURCES.txt` & `microgue-2.0.5/microgue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

