# Comparing `tmp/model2queue-0.1.1.tar.gz` & `tmp/model2queue-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model2queue-0.1.1.tar", last modified: Wed Apr 19 20:59:49 2023, max compression
+gzip compressed data, was "model2queue-0.1.2.tar", last modified: Tue May  9 18:52:58 2023, max compression
```

## Comparing `model2queue-0.1.1.tar` & `model2queue-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:59:49.842685 model2queue-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-19 20:59:49.842685 model2queue-0.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:59:49.838685 model2queue-0.1.1/model2queue/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-19 20:59:39.000000 model2queue-0.1.1/model2queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-04-19 20:59:39.000000 model2queue-0.1.1/model2queue/api_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:59:49.842685 model2queue-0.1.1/model2queue/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:59:39.000000 model2queue-0.1.1/model2queue/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:59:49.842685 model2queue-0.1.1/model2queue/examples/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:59:39.000000 model2queue-0.1.1/model2queue/examples/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-19 20:59:39.000000 model2queue-0.1.1/model2queue/examples/fastapi/preprocess_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-19 20:59:39.000000 model2queue-0.1.1/model2queue/examples/fastapi/simple_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:59:49.842685 model2queue-0.1.1/model2queue/helper/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 20:59:39.000000 model2queue-0.1.1/model2queue/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-19 20:59:39.000000 model2queue-0.1.1/model2queue/helper/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:59:49.842685 model2queue-0.1.1/model2queue/workers/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-19 20:59:39.000000 model2queue-0.1.1/model2queue/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-19 20:59:39.000000 model2queue-0.1.1/model2queue/workers/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-19 20:59:39.000000 model2queue-0.1.1/model2queue/workers/consumer_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-19 20:59:39.000000 model2queue-0.1.1/model2queue/workers/worker_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:59:49.842685 model2queue-0.1.1/model2queue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-19 20:59:49.000000 model2queue-0.1.1/model2queue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-19 20:59:49.000000 model2queue-0.1.1/model2queue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:59:49.000000 model2queue-0.1.1/model2queue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-19 20:59:49.000000 model2queue-0.1.1/model2queue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 20:59:49.000000 model2queue-0.1.1/model2queue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:59:49.842685 model2queue-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-19 20:59:39.000000 model2queue-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:52:58.656476 model2queue-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-09 18:52:58.656476 model2queue-0.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:52:58.652476 model2queue-0.1.2/model2queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/api_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:52:58.652476 model2queue-0.1.2/model2queue/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:52:58.652476 model2queue-0.1.2/model2queue/examples/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/examples/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/examples/fastapi/preprocess_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/examples/fastapi/simple_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:52:58.652476 model2queue-0.1.2/model2queue/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/helper/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:52:58.652476 model2queue-0.1.2/model2queue/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/workers/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/workers/consumer_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/workers/worker_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:52:58.652476 model2queue-0.1.2/model2queue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-09 18:52:58.000000 model2queue-0.1.2/model2queue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-09 18:52:58.000000 model2queue-0.1.2/model2queue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 18:52:58.000000 model2queue-0.1.2/model2queue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-09 18:52:58.000000 model2queue-0.1.2/model2queue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 18:52:58.000000 model2queue-0.1.2/model2queue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 18:52:58.656476 model2queue-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-09 18:52:44.000000 model2queue-0.1.2/setup.py
```

### Comparing `model2queue-0.1.1/model2queue/api_tasks.py` & `model2queue-0.1.2/model2queue/api_tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,38 +19,42 @@
 
 def start_consumer_producer(
     connection: Connection,
     queue: Queue,
     tgt_exchange: Exchange,
     callback_function: Callable[[str], None],
     routing_key: str,
+    n_workers: int
 ):
     queue.maybe_bind(connection)
     queue.declare()
     worker = ConsumerProducerTaskWorker(
         connection=connection,
         queue=queue,
         tgt_exchange=tgt_exchange,
         callback_function=callback_function,
         routing_key=routing_key,
+        n_workers=n_workers
     )
     worker.run()
 
 
 def start_consumer(
     connection: Connection,
     queue: Queue,
     callback_function: Callable[[str], None],
+    n_workers: int
 ):
     queue.maybe_bind(connection)
     queue.declare()
     worker = ConsumerTaskWorker(
         connection=connection,
         queue=queue,
         callback_function=callback_function,
+        n_workers=n_workers
     )
     worker.run()
 
 
 def start_api_task_consumer_producer(
     func: Callable,
     conn_url: str = "memory://localhost/",
```

### Comparing `model2queue-0.1.1/model2queue/examples/fastapi/preprocess_images.py` & `model2queue-0.1.2/model2queue/examples/fastapi/preprocess_images.py`

 * *Files identical despite different names*

### Comparing `model2queue-0.1.1/model2queue/examples/fastapi/simple_model.py` & `model2queue-0.1.2/model2queue/examples/fastapi/simple_model.py`

 * *Files identical despite different names*

### Comparing `model2queue-0.1.1/model2queue/workers/consumer.py` & `model2queue-0.1.2/model2queue/workers/consumer_producer.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,34 +4,44 @@
 from kombu import Message, Consumer, Connection
 
 from model2queue.helper.logger import get_logger
 
 logger = get_logger(__name__)
 
 
-class ConsumerTaskWorker(ConsumerProducerMixin):
+class ConsumerProducerTaskWorker(ConsumerProducerMixin):
     def __init__(
         self,
         connection: Connection,
         queue: str,
+        tgt_exchange: str,
         callback_function: Callable,
+        routing_key: str,
+        n_workers: int = 1
     ):
         self.connection = connection
         self.queue = queue
+        self.tgt_exchange = tgt_exchange
         self.callback_function = callback_function
+        self.routing_key = routing_key
+        self.n_workers = n_workers
 
     def get_consumers(self, consumer: Consumer, channel: Any) -> List[Consumer]:
         return [
             consumer(
                 queues=self.queue,
                 on_message=self.handle_message,
                 prefetch_count=10,
             )
+            for _ in self.n_workers
         ]
 
     def handle_message(self, message: Message) -> None:
         logger.debug(f"received {message} from {self.queue}")
-        try:
-            self.callback_function(message.payload)
-        except Exception as e:
-            logger.error(f"error {e} while processing message {message}")
-        message.ack()
+        output = self.callback_function(message.payload)
+        self.producer.publish(
+            output,
+            exchange=self.tgt_exchange,
+            routing_key=self.routing_key,
+            retry=True,
+        )
+        logger.debug(f"published {output} to {self.tgt_exchange}")
```

### Comparing `model2queue-0.1.1/model2queue/workers/consumer_producer.py` & `model2queue-0.1.2/model2queue/workers/consumer.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,41 +4,37 @@
 from kombu import Message, Consumer, Connection
 
 from model2queue.helper.logger import get_logger
 
 logger = get_logger(__name__)
 
 
-class ConsumerProducerTaskWorker(ConsumerProducerMixin):
+class ConsumerTaskWorker(ConsumerProducerMixin):
     def __init__(
         self,
         connection: Connection,
         queue: str,
-        tgt_exchange: str,
         callback_function: Callable,
-        routing_key: str,
+        n_workers: int = 1,
     ):
         self.connection = connection
         self.queue = queue
-        self.tgt_exchange = tgt_exchange
         self.callback_function = callback_function
-        self.routing_key = routing_key
+        self.n_workers = n_workers
 
     def get_consumers(self, consumer: Consumer, channel: Any) -> List[Consumer]:
         return [
             consumer(
                 queues=self.queue,
                 on_message=self.handle_message,
                 prefetch_count=10,
             )
+            for _ in self.n_workers
         ]
 
     def handle_message(self, message: Message) -> None:
         logger.debug(f"received {message} from {self.queue}")
-        output = self.callback_function(message.payload)
-        self.producer.publish(
-            output,
-            exchange=self.tgt_exchange,
-            routing_key=self.routing_key,
-            retry=True,
-        )
-        logger.debug(f"published {output} to {self.tgt_exchange}")
+        try:
+            self.callback_function(message.payload)
+        except Exception as e:
+            logger.error(f"error {e} while processing message {message}")
+        message.ack()
```

### Comparing `model2queue-0.1.1/model2queue.egg-info/SOURCES.txt` & `model2queue-0.1.2/model2queue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `model2queue-0.1.1/setup.py` & `model2queue-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name="model2queue",
     packages=find_packages(),
-    version="0.1.1",
+    version="0.1.2",
     description="A library to expose an api with a queue for batch predictions",
     author="collective.ai",
     author_email="team.collective.ai@gmail.com",
     url="https://github.com/collectiveai-team/model2queue",
     install_requires=["kombu", "fastapi", "uvicorn", "rich"],
     package_data={"": ["*.yml", "*.yaml"]},
     include_package_data=True,
```

