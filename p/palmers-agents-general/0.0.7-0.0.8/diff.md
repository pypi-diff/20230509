# Comparing `tmp/palmers_agents_general-0.0.7.tar.gz` & `tmp/palmers_agents_general-0.0.8.tar.gz`

## Comparing `palmers_agents_general-0.0.7.tar` & `palmers_agents_general-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/palmers_agents_general/__init__.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/palmers_agents_general/base_mq_consumer.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/palmers_agents_general/blobs_handler.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/palmers_agents_general/models_handler.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/LICENSE
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/README.md
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/palmers_agents_general/__init__.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/palmers_agents_general/base_mq_worker.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/palmers_agents_general/blobs_handler.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/palmers_agents_general/models_handler.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/LICENSE
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/README.md
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.8/PKG-INFO
```

### Comparing `palmers_agents_general-0.0.7/palmers_agents_general/base_mq_consumer.py` & `palmers_agents_general-0.0.8/palmers_agents_general/base_mq_worker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 ﻿import pika
 import sys
-
+import json
 
 START_CONSUMING = 'Waiting for messages. To exit press CTRL+C'
 
 
-class BaseMqConsumer:
-    def __init__(self, mq_username, mq_password, mq_host, mq_port, mq_virtual_host, consume_queue) -> None:
+class BaseMqWorker:
+    def __init__(self, mq_username, mq_password, mq_host, mq_port, mq_virtual_host, consume_queue, produce_queue) -> None:
         self.__connection = None
         self.__channel = None
         self._mq_username = mq_username
         self._mq_password = mq_password
         self._mq_host = mq_host
         self._mq_port = mq_port
         self._mq_virtual_host = mq_virtual_host
         self._consume_queue = consume_queue
+        self._produce_queue = produce_queue
 
         pass
 
     def start_consuming(self, message: str = START_CONSUMING):
         print(message, file=sys.stderr)
         self.__channel.start_consuming()
 
@@ -43,9 +44,17 @@
 
         self.__channel.basic_qos(prefetch_count=1)
         self.__channel.basic_consume(
             queue=self._consume_queue, on_message_callback=self.__callback)
 
         return self
 
+    
+    def publish(self, message, queue=None):
+        queue = queue or self._produce_queue
+
+        self.__channel.basic_publish(exchange='',
+                              routing_key=queue,
+                              body=json.dumps(message))
+
     def __exit__(self, exc_type, exc_value, traceback):
-        self.__connection.close()
+        self.__connection.close()
```

### Comparing `palmers_agents_general-0.0.7/palmers_agents_general/blobs_handler.py` & `palmers_agents_general-0.0.8/palmers_agents_general/blobs_handler.py`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.7/palmers_agents_general/models_handler.py` & `palmers_agents_general-0.0.8/palmers_agents_general/models_handler.py`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.7/LICENSE` & `palmers_agents_general-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.7/pyproject.toml` & `palmers_agents_general-0.0.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "palmers_agents_general"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Assaf", email="assafm@sdatta.ai" },
   { name="Roy ", email="roy@sdatta.ai" },
   { name="Guy", email="assafm@sdatta.ai" },
   { name="Oran", email="assafm@sdatta.ai" },
   { name="Yotam", email="assafm@sdatta.ai" },
 ]
```

