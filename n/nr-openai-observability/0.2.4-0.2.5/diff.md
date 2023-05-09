# Comparing `tmp/nr_openai_observability-0.2.4.tar.gz` & `tmp/nr_openai_observability-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nr_openai_observability-0.2.4.tar", max compression
+gzip compressed data, was "nr_openai_observability-0.2.5.tar", max compression
```

## Comparing `nr_openai_observability-0.2.4.tar` & `nr_openai_observability-0.2.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-03-14 22:23:29.505803 nr_openai_observability-0.2.4/LICENSE
--rw-r--r--   0        0        0     3996 2023-03-14 22:23:29.505803 nr_openai_observability-0.2.4/README.md
--rw-r--r--   0        0        0      687 2023-03-14 22:23:47.241745 nr_openai_observability-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-14 22:23:29.509803 nr_openai_observability-0.2.4/src/nr_openai_observability/__init__.py
--rw-r--r--   0        0        0     4820 2023-03-14 22:23:29.509803 nr_openai_observability-0.2.4/src/nr_openai_observability/monitor.py
--rw-r--r--   0        0        0     4811 1970-01-01 00:00:00.000000 nr_openai_observability-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-09 07:46:55.066403 nr_openai_observability-0.2.5/LICENSE
+-rw-r--r--   0        0        0     4227 2023-05-09 07:46:55.066403 nr_openai_observability-0.2.5/README.md
+-rw-r--r--   0        0        0      687 2023-05-09 07:47:11.122630 nr_openai_observability-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 07:46:55.066403 nr_openai_observability-0.2.5/src/nr_openai_observability/__init__.py
+-rw-r--r--   0        0        0     5257 2023-05-09 07:46:55.066403 nr_openai_observability-0.2.5/src/nr_openai_observability/monitor.py
+-rw-r--r--   0        0        0     5042 1970-01-01 00:00:00.000000 nr_openai_observability-0.2.5/PKG-INFO
```

### Comparing `nr_openai_observability-0.2.4/LICENSE` & `nr_openai_observability-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nr_openai_observability-0.2.4/README.md` & `nr_openai_observability-0.2.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -38,16 +38,14 @@
 #### STEP 2: Add the following two lines to your code
 
 ```python
 from nr_openai_observability import monitor
 monitor.initialization()
 ```
 
-#### STEP 3: Follow the instruction to add the dashboard to your New Relic account.
-
 #### Code example:
 
 ```python
 
 import os
 
 import openai
@@ -60,14 +58,16 @@
     model="text-davinci-003",
     prompt="What is Observability?",
     max_tokens=20,
     temperature=0 
 )
 ```
 
+#### STEP 3: Follow the instruction [here](https://one.newrelic.com/launcher/catalog-pack-details.launcher/?pane=eyJuZXJkbGV0SWQiOiJjYXRhbG9nLXBhY2stZGV0YWlscy5jYXRhbG9nLXBhY2stY29udGVudHMiLCJxdWlja3N0YXJ0SWQiOiI1ZGIyNWRiZC1hNmU5LTQ2ZmMtYTcyOC00Njk3ZjY3N2ZiYzYifQ==) to add the dashboard to your New Relic account.
+
 ### EU Account Users:
 
 If you are using an EU region account, you should also set your `EVENT_CLIENT_HOST`:
 
 **`Bash`**
 
 ```bash
```

### Comparing `nr_openai_observability-0.2.4/pyproject.toml` & `nr_openai_observability-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nr-openai-observability"
-version = "0.2.4"
+version = "0.2.5"
 description = "A lightweight tool to monitor your OpenAI workload."
 authors = ["AIR <air-opensource@newrelic.com>"]
 repository = "https://github.com/newrelic/nr-openai-observability"
 readme = "README.md"
 homepage = "https://newrelic.com/instant-observability/openai"
 keywords = ["newrelic", "observability", "openai", "gpt", "chatGPT", "GPT-4", "monitor", "generative", "ai"]
```

### Comparing `nr_openai_observability-0.2.4/src/nr_openai_observability/monitor.py` & `nr_openai_observability-0.2.5/src/nr_openai_observability/monitor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import atexit
 import logging
 import os
 import time
-from typing import Optional
+from typing import Any, Dict, Optional
 
 import openai
 from newrelic_telemetry_sdk import Event, EventBatch, EventClient, Harvester
 
 logger = logging.getLogger("nr_openai_observability")
 
 EventName = "OpenAICompletion"
@@ -53,26 +53,37 @@
         if not isinstance(event_client_host, str) and event_client_host is not None:
             raise TypeError("event_client_host instance type must be str or None")
 
         self.event_client_host = event_client_host or os.getenv(
             "EVENT_CLIENT_HOST", EventClient.HOST
         )
 
+    def _set_metadata(
+        self,
+        metadata: Dict[str, Any] = {},
+    ): 
+        self.metadata = metadata
+
+        if not isinstance(metadata, Dict) and metadata is not None:
+            raise TypeError("metadata instance type must be Dict[str, Any]")
+
     def _log(self, msg: str):
         if self.use_logger:
             logger.info(msg)
         else:
             print(msg)
 
     def start(
         self,
         license_key: Optional[str] = None,
+        metadata: Dict[str, Any] = {},
         event_client_host: Optional[str] = None,
     ):
         self._set_license_key(license_key)
+        self._set_metadata(metadata)
         self._set_client_host(event_client_host)
         self._start()
 
     # initialize event thread
     def _start(self):
         self.event_client = EventClient(
             self.license_key,
@@ -87,14 +98,15 @@
         self.event_harvester.start()
 
         # When the process exits, run the harvester.stop() method before terminating the process
         # Why? To send the remaining data...
         atexit.register(self.event_harvester.stop)
 
     def record_event(self, event_dict: dict, table: str = EventName):
+        event_dict.update(self.metadata)
         event = Event(table, event_dict)
         self.event_batch.record(event)
 
 
 def patcher_create(original_fn, *args, **kwargs):
     def flatten_dict(dd, separator=".", prefix="", index=""):
         if len(index):
@@ -146,17 +158,18 @@
 
 
 monitor = OpenAIMonitoring()
 
 
 def initialization(
     license_key: Optional[str] = None,
+    metadata: Dict[str, Any] = {},
     event_client_host: Optional[str] = None,
 ):
-    monitor.start(license_key, event_client_host)
+    monitor.start(license_key, metadata, event_client_host)
     perform_patch()
 
 
 def perform_patch():
     try:
         openai.Completion.create = _patched_call(
             openai.Completion.create, patcher_create
```

### Comparing `nr_openai_observability-0.2.4/PKG-INFO` & `nr_openai_observability-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nr-openai-observability
-Version: 0.2.4
+Version: 0.2.5
 Summary: A lightweight tool to monitor your OpenAI workload.
 Home-page: https://newrelic.com/instant-observability/openai
 Keywords: newrelic,observability,openai,gpt,chatGPT,GPT-4,monitor,generative,ai
 Author: AIR
 Author-email: air-opensource@newrelic.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
@@ -57,16 +57,14 @@
 #### STEP 2: Add the following two lines to your code
 
 ```python
 from nr_openai_observability import monitor
 monitor.initialization()
 ```
 
-#### STEP 3: Follow the instruction to add the dashboard to your New Relic account.
-
 #### Code example:
 
 ```python
 
 import os
 
 import openai
@@ -79,14 +77,16 @@
     model="text-davinci-003",
     prompt="What is Observability?",
     max_tokens=20,
     temperature=0 
 )
 ```
 
+#### STEP 3: Follow the instruction [here](https://one.newrelic.com/launcher/catalog-pack-details.launcher/?pane=eyJuZXJkbGV0SWQiOiJjYXRhbG9nLXBhY2stZGV0YWlscy5jYXRhbG9nLXBhY2stY29udGVudHMiLCJxdWlja3N0YXJ0SWQiOiI1ZGIyNWRiZC1hNmU5LTQ2ZmMtYTcyOC00Njk3ZjY3N2ZiYzYifQ==) to add the dashboard to your New Relic account.
+
 ### EU Account Users:
 
 If you are using an EU region account, you should also set your `EVENT_CLIENT_HOST`:
 
 **`Bash`**
 
 ```bash
```

