# Comparing `tmp/polars-streaming-0.2.0.tar.gz` & `tmp/polars-streaming-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/alchemist/Desktop/OpenSource/polars-streaming/dist/.tmp-_lveyz49/polars-streaming-0.2.0.tar", last modified: Sun Apr 30 14:08:08 2023, max compression
+gzip compressed data, was "/home/alchemist/Desktop/OpenSource/polars-streaming/dist/.tmp-hiizhq42/polars-streaming-0.3.0.tar", last modified: Tue May  9 15:04:16 2023, max compression
```

## Comparing `polars-streaming-0.2.0.tar` & `polars-streaming-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    11357 2023-04-19 18:26:51.000000 polars-streaming-0.2.0/LICENSE
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    14448 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/PKG-INFO
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      901 2023-04-30 14:07:46.000000 polars-streaming-0.2.0/README.md
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/polars_streaming/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      210 2023-04-30 13:56:54.000000 polars-streaming-0.2.0/polars_streaming/__init__.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1240 2023-04-30 12:55:14.000000 polars-streaming-0.2.0/polars_streaming/core.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      436 2023-04-26 17:25:44.000000 polars-streaming-0.2.0/polars_streaming/exceptions.py
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/polars_streaming/processors/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        0 2023-04-30 12:45:56.000000 polars-streaming-0.2.0/polars_streaming/processors/__init__.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     2138 2023-04-30 12:41:43.000000 polars-streaming-0.2.0/polars_streaming/processors/fileProcessor.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     2823 2023-04-30 12:41:36.000000 polars-streaming-0.2.0/polars_streaming/processors/kafkaProcessor.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1790 2023-04-30 13:55:05.000000 polars-streaming-0.2.0/polars_streaming/processors/socketProcessor.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      919 2023-04-30 12:41:23.000000 polars-streaming-0.2.0/polars_streaming/processors/utils.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1715 2023-04-26 13:32:40.000000 polars-streaming-0.2.0/polars_streaming/readwriter.py
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/polars_streaming/sinks/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        0 2023-04-30 11:14:10.000000 polars-streaming-0.2.0/polars_streaming/sinks/__init__.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1015 2023-04-29 07:01:54.000000 polars-streaming-0.2.0/polars_streaming/sinks/esWriter.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      586 2023-04-29 06:50:31.000000 polars-streaming-0.2.0/polars_streaming/sinks/mongoWriter.py
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/polars_streaming.egg-info/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    14448 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/polars_streaming.egg-info/PKG-INFO
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      670 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/polars_streaming.egg-info/SOURCES.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        1 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/polars_streaming.egg-info/dependency_links.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      128 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/polars_streaming.egg-info/requires.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       17 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/polars_streaming.egg-info/top_level.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1228 2023-04-30 13:56:54.000000 polars-streaming-0.2.0/pyproject.toml
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       38 2023-04-30 14:08:08.000000 polars-streaming-0.2.0/setup.cfg
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-05-09 15:04:16.000000 polars-streaming-0.3.0/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    11357 2023-04-19 18:26:51.000000 polars-streaming-0.3.0/LICENSE
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    15895 2023-05-09 15:04:16.000000 polars-streaming-0.3.0/PKG-INFO
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     2348 2023-05-09 12:34:29.000000 polars-streaming-0.3.0/README.md
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-05-09 15:04:16.000000 polars-streaming-0.3.0/polars_streaming/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      210 2023-05-09 15:04:01.000000 polars-streaming-0.3.0/polars_streaming/__init__.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1240 2023-04-30 12:55:14.000000 polars-streaming-0.3.0/polars_streaming/core.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      436 2023-04-26 17:25:44.000000 polars-streaming-0.3.0/polars_streaming/exceptions.py
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-05-09 15:04:16.000000 polars-streaming-0.3.0/polars_streaming/processors/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        0 2023-04-30 12:45:56.000000 polars-streaming-0.3.0/polars_streaming/processors/__init__.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     2476 2023-05-09 08:23:32.000000 polars-streaming-0.3.0/polars_streaming/processors/fileProcessor.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     3421 2023-05-09 08:16:30.000000 polars-streaming-0.3.0/polars_streaming/processors/kafkaProcessor.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     2050 2023-05-09 08:20:05.000000 polars-streaming-0.3.0/polars_streaming/processors/socketProcessor.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      919 2023-04-30 12:41:23.000000 polars-streaming-0.3.0/polars_streaming/processors/utils.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1715 2023-04-26 13:32:40.000000 polars-streaming-0.3.0/polars_streaming/readwriter.py
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-05-09 15:04:16.000000 polars-streaming-0.3.0/polars_streaming/sinks/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        0 2023-04-30 11:14:10.000000 polars-streaming-0.3.0/polars_streaming/sinks/__init__.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1004 2023-05-09 14:57:45.000000 polars-streaming-0.3.0/polars_streaming/sinks/esWriter.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      650 2023-05-09 15:00:09.000000 polars-streaming-0.3.0/polars_streaming/sinks/mongoWriter.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      839 2023-05-09 08:15:30.000000 polars-streaming-0.3.0/polars_streaming/sinks/sink_utils.py
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-05-09 15:04:16.000000 polars-streaming-0.3.0/polars_streaming.egg-info/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    15895 2023-05-09 15:04:16.000000 polars-streaming-0.3.0/polars_streaming.egg-info/PKG-INFO
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      707 2023-05-09 15:04:16.000000 polars-streaming-0.3.0/polars_streaming.egg-info/SOURCES.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        1 2023-05-09 15:04:16.000000 polars-streaming-0.3.0/polars_streaming.egg-info/dependency_links.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      128 2023-05-09 15:04:16.000000 polars-streaming-0.3.0/polars_streaming.egg-info/requires.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       17 2023-05-09 15:04:16.000000 polars-streaming-0.3.0/polars_streaming.egg-info/top_level.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1228 2023-05-09 15:04:01.000000 polars-streaming-0.3.0/pyproject.toml
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       38 2023-05-09 15:04:16.000000 polars-streaming-0.3.0/setup.cfg
```

### Comparing `polars-streaming-0.2.0/LICENSE` & `polars-streaming-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polars-streaming-0.2.0/PKG-INFO` & `polars-streaming-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars-streaming
-Version: 0.2.0
+Version: 0.3.0
 Summary: Stream Processing Library using Polars
 Author-email: Vinish M <vinishuchiha@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -233,14 +233,15 @@
 Alternatively, you can also clone the latest version from the [repository](https://github.com/VinishUchiha/polars-streaming) and install it directly from the source code:
 
 ```bash
 pip install -e .
 ```
 
 ## Quick tour
+### Socket
 ```python
 >>> from polars_streaming import StreamProcessor
 
 >>> s = StreamProcessor()
 >>> s.readStream.format('socket').options({'host':'localhost','port':12345}).load()
 
 >>> def transformation(df):
@@ -249,7 +250,61 @@
 >>>     return df # Return the transformed dataframe
 
 >>> s.add_transform(transformation)
 >>> s.writeStream.format('console').trigger('3 seconds')
 
 >>> s.start()
 ```
+### Kafka
+```python
+>>> from polars_streaming import StreamProcessor
+
+>>> s = StreamProcessor()
+>>> s.readStream.format('kafka').options({'kafka.bootstrap.servers':'localhost','subscribe': 'topic_name',
+                                          'startingOffsets': 'earliest',
+                                          'kafka.group.id': 'g1'}).load()
+
+>>> def transformation(df):
+>>>     # Add your transformation code here
+>>>     df = df.sum() # For example purpose, I am calculating the sum.
+>>>     return df # Return the transformed dataframe
+
+>>> s.add_transform(transformation)
+>>> s.writeStream.format('console').trigger('10 seconds')
+
+>>> s.start()
+```
+### File Sources
+```python
+>>> from polars_streaming import StreamProcessor
+
+>>> s = StreamProcessor()
+>>> s.readStream.format('csv').load('read_path_of_file_source') # Reads the csv file from the path once it is created
+
+>>> def transformation(df):
+>>>     # Add your transformation code here
+>>>     df = df.sum() # For example purpose, I am calculating the sum.
+>>>     return df # Return the transformed dataframe
+
+>>> s.add_transform(transformation)
+>>> s.writeStream.option('path','write_path').format('avro') # Write the processed data to the write path in avro format
+
+>>> s.start()
+```
+## Sources
+- Socket
+- File Sources
+  - CSV
+  - JSON
+  - AVRO
+  - PARQUET
+- Kafka
+
+## Sinks
+- Console
+- File Sources
+  - CSV
+  - JSON
+  - AVRO
+  - PARQUET
+- MongoDB
+- ElasticSearch
```

### Comparing `polars-streaming-0.2.0/README.md` & `polars-streaming-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 Alternatively, you can also clone the latest version from the [repository](https://github.com/VinishUchiha/polars-streaming) and install it directly from the source code:
 
 ```bash
 pip install -e .
 ```
 
 ## Quick tour
+### Socket
 ```python
 >>> from polars_streaming import StreamProcessor
 
 >>> s = StreamProcessor()
 >>> s.readStream.format('socket').options({'host':'localhost','port':12345}).load()
 
 >>> def transformation(df):
@@ -31,7 +32,61 @@
 >>>     return df # Return the transformed dataframe
 
 >>> s.add_transform(transformation)
 >>> s.writeStream.format('console').trigger('3 seconds')
 
 >>> s.start()
 ```
+### Kafka
+```python
+>>> from polars_streaming import StreamProcessor
+
+>>> s = StreamProcessor()
+>>> s.readStream.format('kafka').options({'kafka.bootstrap.servers':'localhost','subscribe': 'topic_name',
+                                          'startingOffsets': 'earliest',
+                                          'kafka.group.id': 'g1'}).load()
+
+>>> def transformation(df):
+>>>     # Add your transformation code here
+>>>     df = df.sum() # For example purpose, I am calculating the sum.
+>>>     return df # Return the transformed dataframe
+
+>>> s.add_transform(transformation)
+>>> s.writeStream.format('console').trigger('10 seconds')
+
+>>> s.start()
+```
+### File Sources
+```python
+>>> from polars_streaming import StreamProcessor
+
+>>> s = StreamProcessor()
+>>> s.readStream.format('csv').load('read_path_of_file_source') # Reads the csv file from the path once it is created
+
+>>> def transformation(df):
+>>>     # Add your transformation code here
+>>>     df = df.sum() # For example purpose, I am calculating the sum.
+>>>     return df # Return the transformed dataframe
+
+>>> s.add_transform(transformation)
+>>> s.writeStream.option('path','write_path').format('avro') # Write the processed data to the write path in avro format
+
+>>> s.start()
+```
+## Sources
+- Socket
+- File Sources
+  - CSV
+  - JSON
+  - AVRO
+  - PARQUET
+- Kafka
+
+## Sinks
+- Console
+- File Sources
+  - CSV
+  - JSON
+  - AVRO
+  - PARQUET
+- MongoDB
+- ElasticSearch
```

### Comparing `polars-streaming-0.2.0/polars_streaming/core.py` & `polars-streaming-0.3.0/polars_streaming/core.py`

 * *Files identical despite different names*

### Comparing `polars-streaming-0.2.0/polars_streaming/processors/fileProcessor.py` & `polars-streaming-0.3.0/polars_streaming/processors/fileProcessor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 from watchdog.events import PatternMatchingEventHandler
 from watchdog.observers import Observer
 from ..exceptions import FileSourcePathMissingException, FileExtensionNotSupportedException
 import polars as pl
 import time
 from pathlib import Path
 from .utils import _writer, READERS, SUPPORTED_FILE_WRITERS
+from ..sinks import sink_utils
 
 class FileHandler(PatternMatchingEventHandler):
-    def __init__(self, reader, transform, writer) -> None:
+    def __init__(self, reader, transform, writer, sink) -> None:
         self.reader = reader
         self.transform = transform
         self.writer = writer
+        self.sink = sink
         PatternMatchingEventHandler.__init__(self, patterns=[f'*.{self.reader.source}'], ignore_directories=True, case_sensitive=False)
 
     def on_created(self, event):
         #print(f"New {self.source} file created", event.src_path)
         try:
             df = READERS[self.reader.source](event.src_path)
             df = self.transform(df.lazy())
             if self.writer.source=='console':
                 print(df.collect())
             elif self.writer.source in SUPPORTED_FILE_WRITERS:
                 path = self.writer._options['path'].rstrip('/')
                 filename = Path(event.src_path).stem
                 fullpath = f"{path}/{filename}.{self.writer.source}"
                 _writer(df.collect(), fullpath, self.writer.source)
+            elif self.writer.source in ['mongo','elasticsearch']:
+                self.sink.write_dataframe(df.collect())
         except Exception as e:
             print(e)
 
 class FileProcessor():
     def __init__(self, reader, transform, writer) -> None:
         self.reader = reader
         self.transform = transform
         self.writer = writer
 
     def start(self):
-        event_handler = FileHandler(self.reader, self.transform, self.writer)
+        if self.writer.source in ['mongo','elasticsearch']:
+            sink = sink_utils.sinker(self.writer)
+        else:
+            sink = None
+        event_handler = FileHandler(self.reader, self.transform, self.writer, sink)
         observer = Observer()
         if self.reader.file_source_path:
             path = self.reader.file_source_path
         elif 'path' in self.reader._options:
             path = self.reader._options['path']
         else:
             raise FileSourcePathMissingException("file source path not mentioned")
```

### Comparing `polars-streaming-0.2.0/polars_streaming/processors/kafkaProcessor.py` & `polars-streaming-0.3.0/polars_streaming/processors/kafkaProcessor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import polars as pl
 import schedule
 from .utils import _writer, SUPPORTED_FILE_WRITERS, trigger_time_extracter
 from ..exceptions import ModuleNotFoundException
+import json
+from ..sinks import sink_utils
 
 options_mapper = {'kafka.bootstrap.servers':'bootstrap.servers',
                 #'subscribe': 'subscribe',
                 #'includeHeaders': 'includeHeaders',
                 'startingOffsets': 'auto.offset.reset',
                 #'endingOffsets': 'endingOffsets',
                 #'subscribePattern': 'subscribePattern',
@@ -36,36 +38,47 @@
             print(f"Batch: {self.batch_count}")
             print(df.collect())
         elif self.writer.source in SUPPORTED_FILE_WRITERS:
             path = self.writer._options['path'].rstrip('/')
             filename = f"batch_{self.batch_count}"
             fullpath = f"{path}/{filename}.{self.writer.source}"
             _writer(df.collect(), fullpath, self.writer.source)
+        elif self.writer.source in ['mongo','elasticsearch']:
+            self.sink.write_dataframe(df.collect())
         self.batch_count+=1
         self.mini_batch.clear()
 
     def start(self):
         from confluent_kafka import Consumer, KafkaException
         self._kafka_option_mapper()
         consumer = Consumer(self.kafka_config)
         topics = self.reader._options['subscribe'].split(',')
+        if 'serializer' in self.reader._options:
+            serializer = self.reader._options['serializer']
+        else:
+            serializer = 'string'
         consumer.subscribe(topics)
+        if self.writer.source in ['mongo','elasticsearch']:
+            self.sink = sink_utils.sinker(self.writer)
         self.mini_batch = []
         ptime = trigger_time_extracter(self.writer.processing_time)
         schedule.every(ptime).seconds.do(self.apply_transform, transformation = self.transform)
         self.batch_count = 0
         try:
             while True:
                 event = consumer.poll(1.0)
                 if event is None:
                     continue
                 if event.error():
                     raise KafkaException(event.error())
                 else:
-                    val = event.value().decode('utf8')
+                    if serializer ==' string':
+                        val = event.value().decode('utf8')
+                    elif serializer == 'json':
+                        val = json.loads(event.value().decode('utf8'))
                     consumer.commit(event)
                 self.mini_batch.append(val)
                 schedule.run_pending()
         except KeyboardInterrupt:
             print('Canceled by user.')
         finally:
             consumer.close()
```

### Comparing `polars-streaming-0.2.0/polars_streaming/processors/socketProcessor.py` & `polars-streaming-0.3.0/polars_streaming/processors/socketProcessor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import polars as pl
 import socket
 import schedule
 from .utils import _writer, SUPPORTED_FILE_WRITERS, trigger_time_extracter
+from ..sinks import sink_utils
 
 class SocketProcessor():
     def __init__(self, reader, transform, writer):
         self.reader = reader
         self.writer = writer
         self.transform = transform
 
@@ -16,26 +17,30 @@
             print(f"Batch: {self.batch_count}")
             print(df.collect())
         elif self.writer.source in SUPPORTED_FILE_WRITERS:
             path = self.writer._options['path'].rstrip('/')
             filename = f"batch_{self.batch_count}"
             fullpath = f"{path}/{filename}.{self.writer.source}"
             _writer(df.collect(), fullpath, self.writer.source)
+        elif self.writer.source in ['mongo','elasticsearch']:
+            self.sink.write_dataframe(df.collect())
         self.batch_count+=1
         self.mini_batch.clear()
 
     def start(self):
         host = self.reader._options['host']
         port = self.reader._options['port']
         if 'bufferSize' in self.reader._options:
             buffer = self.reader._options['bufferSize']
         else:
             buffer = 1024
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         s.connect((host, port))
+        if self.writer.source in ['mongo','elasticsearch']:
+            self.sink = sink_utils.sinker(self.writer)
         self.mini_batch = []
         ptime = trigger_time_extracter(self.writer.processing_time)
         schedule.every(ptime).seconds.do(self.apply_transform, transformation = self.transform)
         self.batch_count = 0
         try:
             while True:
                 msg = s.recv(buffer)
```

### Comparing `polars-streaming-0.2.0/polars_streaming/processors/utils.py` & `polars-streaming-0.3.0/polars_streaming/processors/utils.py`

 * *Files identical despite different names*

### Comparing `polars-streaming-0.2.0/polars_streaming/readwriter.py` & `polars-streaming-0.3.0/polars_streaming/readwriter.py`

 * *Files identical despite different names*

### Comparing `polars-streaming-0.2.0/polars_streaming/sinks/esWriter.py` & `polars-streaming-0.3.0/polars_streaming/sinks/esWriter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from ..exceptions import ModuleNotFoundException
 
-class ElasticSearch():
+class ESWriter():
     def __init__(self, host: str, index: str, username: str =None, password: str =None, api_key: str = None) -> None:
         try:
             from elasticsearch import Elasticsearch
         except ImportError:
             raise ModuleNotFoundException("elasticsearch not installed. try `pip install elasticsearch`.")
         if username is not None and password is not None:
-            self.es = ElasticSearch([host], basic_auth=(username, password))
+            self.es = Elasticsearch([host], basic_auth=(username, password))
         elif api_key is not None:
-            self.es = ElasticSearch([host], api_key=api_key)
+            self.es = Elasticsearch([host], api_key=api_key)
         else:
-            self.es = ElasticSearch([host])
+            self.es = Elasticsearch([host])
         self.index = index
 
-    def write_dataframe(self, df, index):
+    def write_dataframe(self, df):
         from elasticsearch.helpers import bulk
-        records = df.to_dict()
+        records = df.to_dicts()
         actions = [
             {
                 "_index": self.index,
                 "_source": doc
             }
             for doc in records
         ]
```

### Comparing `polars-streaming-0.2.0/polars_streaming/sinks/mongoWriter.py` & `polars-streaming-0.3.0/polars_streaming/sinks/mongoWriter.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,12 +5,14 @@
         try:
             from pymongo import MongoClient
         except ImportError:
             raise ModuleNotFoundException("pymongo not installed. try `pip install pymongo`.")
         self.mdb = MongoClient(conn_str)
         self.collection = collection
         self.database = database
+        self.mongo = self.mdb[self.database][self.collection]
 
     def write_dataframe(self, df):
-        records = df.to_dict()
-        self.mdb[self.database][self.collection].insert_many(records)
+        records = df.to_dicts()
+        if len(records)>0:
+            self.mongo.insert_many(records)
```

### Comparing `polars-streaming-0.2.0/polars_streaming.egg-info/PKG-INFO` & `polars-streaming-0.3.0/polars_streaming.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars-streaming
-Version: 0.2.0
+Version: 0.3.0
 Summary: Stream Processing Library using Polars
 Author-email: Vinish M <vinishuchiha@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -233,14 +233,15 @@
 Alternatively, you can also clone the latest version from the [repository](https://github.com/VinishUchiha/polars-streaming) and install it directly from the source code:
 
 ```bash
 pip install -e .
 ```
 
 ## Quick tour
+### Socket
 ```python
 >>> from polars_streaming import StreamProcessor
 
 >>> s = StreamProcessor()
 >>> s.readStream.format('socket').options({'host':'localhost','port':12345}).load()
 
 >>> def transformation(df):
@@ -249,7 +250,61 @@
 >>>     return df # Return the transformed dataframe
 
 >>> s.add_transform(transformation)
 >>> s.writeStream.format('console').trigger('3 seconds')
 
 >>> s.start()
 ```
+### Kafka
+```python
+>>> from polars_streaming import StreamProcessor
+
+>>> s = StreamProcessor()
+>>> s.readStream.format('kafka').options({'kafka.bootstrap.servers':'localhost','subscribe': 'topic_name',
+                                          'startingOffsets': 'earliest',
+                                          'kafka.group.id': 'g1'}).load()
+
+>>> def transformation(df):
+>>>     # Add your transformation code here
+>>>     df = df.sum() # For example purpose, I am calculating the sum.
+>>>     return df # Return the transformed dataframe
+
+>>> s.add_transform(transformation)
+>>> s.writeStream.format('console').trigger('10 seconds')
+
+>>> s.start()
+```
+### File Sources
+```python
+>>> from polars_streaming import StreamProcessor
+
+>>> s = StreamProcessor()
+>>> s.readStream.format('csv').load('read_path_of_file_source') # Reads the csv file from the path once it is created
+
+>>> def transformation(df):
+>>>     # Add your transformation code here
+>>>     df = df.sum() # For example purpose, I am calculating the sum.
+>>>     return df # Return the transformed dataframe
+
+>>> s.add_transform(transformation)
+>>> s.writeStream.option('path','write_path').format('avro') # Write the processed data to the write path in avro format
+
+>>> s.start()
+```
+## Sources
+- Socket
+- File Sources
+  - CSV
+  - JSON
+  - AVRO
+  - PARQUET
+- Kafka
+
+## Sinks
+- Console
+- File Sources
+  - CSV
+  - JSON
+  - AVRO
+  - PARQUET
+- MongoDB
+- ElasticSearch
```

### Comparing `polars-streaming-0.2.0/polars_streaming.egg-info/SOURCES.txt` & `polars-streaming-0.3.0/polars_streaming.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 polars_streaming/processors/__init__.py
 polars_streaming/processors/fileProcessor.py
 polars_streaming/processors/kafkaProcessor.py
 polars_streaming/processors/socketProcessor.py
 polars_streaming/processors/utils.py
 polars_streaming/sinks/__init__.py
 polars_streaming/sinks/esWriter.py
-polars_streaming/sinks/mongoWriter.py
+polars_streaming/sinks/mongoWriter.py
+polars_streaming/sinks/sink_utils.py
```

### Comparing `polars-streaming-0.2.0/pyproject.toml` & `polars-streaming-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "polars-streaming"
-version = "0.2.0"
+version = "0.3.0"
 description = "Stream Processing Library using Polars"
 readme = "README.md"
 authors = [{ name = "Vinish M", email = "vinishuchiha@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
@@ -27,15 +27,15 @@
 kafka = ["confluent-kafka"]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/VinishUchiha/polars-streaming"
 
 [tool.bumpver]
-current_version = "0.2.0"
+current_version = "0.3.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

