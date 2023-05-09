# Comparing `tmp/pyraisdk-0.3.1.tar.gz` & `tmp/pyraisdk-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyraisdk-0.3.1.tar", max compression
+gzip compressed data, was "pyraisdk-0.3.2.tar", max compression
```

## Comparing `pyraisdk-0.3.1.tar` & `pyraisdk-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     9487 2023-03-28 15:31:48.044783 pyraisdk-0.3.1/README.md
--rw-r--r--   0        0        0      577 2023-03-28 15:31:48.072784 pyraisdk-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       42 2023-03-28 15:31:48.072784 pyraisdk-0.3.1/pyraisdk/__init__.py
--rw-r--r--   0        0        0      156 2023-03-28 15:31:48.072784 pyraisdk-0.3.1/pyraisdk/dynbatch/__init__.py
--rw-r--r--   0        0        0     1245 2023-03-28 15:31:48.072784 pyraisdk-0.3.1/pyraisdk/dynbatch/base.py
--rw-r--r--   0        0        0    15233 2023-03-28 15:31:48.072784 pyraisdk-0.3.1/pyraisdk/dynbatch/batch.py
--rw-r--r--   0        0        0     1349 2023-03-28 15:31:48.072784 pyraisdk-0.3.1/pyraisdk/dynbatch/config.py
--rw-r--r--   0        0        0     6220 2023-03-28 15:31:48.076784 pyraisdk-0.3.1/pyraisdk/rlog/__init__.py
--rw-r--r--   0        0        0     8187 2023-03-28 15:31:48.076784 pyraisdk-0.3.1/pyraisdk/rlog/eventhub.py
--rw-r--r--   0        0        0     3659 2023-03-28 15:31:48.076784 pyraisdk-0.3.1/pyraisdk/rlog/gputil.py
--rw-r--r--   0        0        0     6497 2023-03-28 15:31:48.076784 pyraisdk-0.3.1/pyraisdk/rlog/log.py
--rw-r--r--   0        0        0     7922 2023-03-28 15:31:48.076784 pyraisdk-0.3.1/pyraisdk/rlog/logimp.py
--rw-r--r--   0        0        0     5040 2023-03-28 15:31:48.076784 pyraisdk-0.3.1/pyraisdk/rlog/reporter.py
--rw-r--r--   0        0        0    10131 1970-01-01 00:00:00.000000 pyraisdk-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    10216 2023-05-09 03:16:09.748211 pyraisdk-0.3.2/README.md
+-rw-r--r--   0        0        0      577 2023-05-09 03:16:09.772213 pyraisdk-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-05-09 03:16:09.772213 pyraisdk-0.3.2/pyraisdk/__init__.py
+-rw-r--r--   0        0        0      156 2023-05-09 03:16:09.772213 pyraisdk-0.3.2/pyraisdk/dynbatch/__init__.py
+-rw-r--r--   0        0        0     1245 2023-05-09 03:16:09.772213 pyraisdk-0.3.2/pyraisdk/dynbatch/base.py
+-rw-r--r--   0        0        0    15233 2023-05-09 03:16:09.772213 pyraisdk-0.3.2/pyraisdk/dynbatch/batch.py
+-rw-r--r--   0        0        0     1349 2023-05-09 03:16:09.772213 pyraisdk-0.3.2/pyraisdk/dynbatch/config.py
+-rw-r--r--   0        0        0     6221 2023-05-09 03:16:09.772213 pyraisdk-0.3.2/pyraisdk/rlog/__init__.py
+-rw-r--r--   0        0        0     8187 2023-05-09 03:16:09.772213 pyraisdk-0.3.2/pyraisdk/rlog/eventhub.py
+-rw-r--r--   0        0        0     4048 2023-05-09 03:16:09.772213 pyraisdk-0.3.2/pyraisdk/rlog/gputil.py
+-rw-r--r--   0        0        0     6497 2023-05-09 03:16:09.772213 pyraisdk-0.3.2/pyraisdk/rlog/log.py
+-rw-r--r--   0        0        0     8043 2023-05-09 03:16:09.776213 pyraisdk-0.3.2/pyraisdk/rlog/logimp.py
+-rw-r--r--   0        0        0     5040 2023-05-09 03:16:09.776213 pyraisdk-0.3.2/pyraisdk/rlog/reporter.py
+-rw-r--r--   0        0        0    10860 1970-01-01 00:00:00.000000 pyraisdk-0.3.2/PKG-INFO
```

### Comparing `pyraisdk-0.3.1/README.md` & `pyraisdk-0.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,29 @@
   ```
 When the CD pipeline deploys the model to an AML online deployment, it exports environment variables for each `BatchingConfig` field, which pyraisdk utilizes at process start to configure batching parameters. The CD pipeline also exports environment variables to enable pyraisdk to log to RAI's Azure Data Explorer clusters.
 
 ### Test or Deploy without RAI CD Pipeline
 
 Test or Deploy independetly outside of RAI CD Pipeline, it's required to set environment variables for `BatchingConfig` manually before object of `DynamicBatchModel` is created. Refer to [Batching Parameter](#batching-parameter-attention). 
 
+The recommended way to set these variables is calling `os.environ.setdefault` in `init()`. Like below:
+
+```python
+def init():
+    os.environ.setdefault('PYRAISDK_MAX_BATCH_SIZE', '12')
+    os.environ.setdefault('PYRAISDK_IDLE_BATCH_SIZE', '5')
+    os.environ.setdefault('PYRAISDK_MAX_BATCH_INTERVAL', '0.002')
+    ...
+    batch_model = DynamicBatchModel(malware_model)
+```
+
+This should work well independent of RAI CD Pipeline. And you don't need to specifically remove these 3 lines when switching to deploy in CD Pipeline. 
+
+But please note that this kind of code should be **Avoided**: `os.environ['PYRAISDK_MAX_BATCH_SIZE'] = '12'`. It will override the configuration from CD pipeline, which is not desirable in most cases.
+
 To enable log publishing (to eventhub), there are another several environment variables need to be set, refer to following logging part. It's optional.
 
 
 ## Dynamic Batching Support
 
 There are APIs you **must** implement in your model to support batching of inference requests for best model performance. Those APIs allow the SDK
 to distribute load efficiently to the GPU instances. The APIs are:
```

### Comparing `pyraisdk-0.3.1/pyproject.toml` & `pyraisdk-0.3.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyraisdk"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = ["Xiaodong Yang <xiaoyan@microsoft.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 azure-eventhub = "^5.10.1"
```

### Comparing `pyraisdk-0.3.1/pyraisdk/dynbatch/base.py` & `pyraisdk-0.3.2/pyraisdk/dynbatch/base.py`

 * *Files identical despite different names*

### Comparing `pyraisdk-0.3.1/pyraisdk/dynbatch/batch.py` & `pyraisdk-0.3.2/pyraisdk/dynbatch/batch.py`

 * *Files identical despite different names*

### Comparing `pyraisdk-0.3.1/pyraisdk/dynbatch/config.py` & `pyraisdk-0.3.2/pyraisdk/dynbatch/config.py`

 * *Files identical despite different names*

### Comparing `pyraisdk-0.3.1/pyraisdk/rlog/__init__.py` & `pyraisdk-0.3.2/pyraisdk/rlog/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
             _logger.add_sink_unstructured(StdoutSink())
 
             # start
             _logger.start()
 
             # system auto metrics
             if sys_metrics_enable:
-                _sys_metrics_reporter = SystemMetricsReporter(_logger, report_interval=60, measure_interval=5)
+                _sys_metrics_reporter = SystemMetricsReporter(_logger, report_interval=60, measure_interval=30)
 
             # success
             _logger_initialized = True
         
                 
 def _probably_unique_id() -> str:
 	u = str(uuid.uuid4())
```

### Comparing `pyraisdk-0.3.1/pyraisdk/rlog/eventhub.py` & `pyraisdk-0.3.2/pyraisdk/rlog/eventhub.py`

 * *Files identical despite different names*

### Comparing `pyraisdk-0.3.1/pyraisdk/rlog/gputil.py` & `pyraisdk-0.3.2/pyraisdk/rlog/gputil.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import math
 import os
 import platform
 import subprocess
 from distutils import spawn
 from typing import Dict, List, Optional
 
+import psutil
+
 
 @dataclass
 class GPUInfo:
     index: int
     uuid: str
     utilization_gpu: float
     memory_total: float
@@ -46,15 +48,28 @@
         'driver_version',
         'name',
         'gpu_serial',
         'display_active',
         'display_mode',
         'temperature.gpu',
     ]
-    proc = subprocess.Popen([nvidia_smi, f"--query-gpu={','.join(fields)}", "--format=csv,noheader,nounits"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    if psutil.POSIX:
+        # set high niceness for posix
+        proc = subprocess.Popen(
+            [nvidia_smi, f"--query-gpu={','.join(fields)}", "--format=csv,noheader,nounits"],
+            preexec_fn=lambda : os.nice(19),
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+        )
+    else:
+        proc = subprocess.Popen(
+            [nvidia_smi, f"--query-gpu={','.join(fields)}", "--format=csv,noheader,nounits"],
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+        )
     try:
         outs, errs = proc.communicate(timeout=10)
     finally:
         if proc.poll() is None:
             proc.kill()
 
     if proc.poll() != 0:
```

### Comparing `pyraisdk-0.3.1/pyraisdk/rlog/log.py` & `pyraisdk-0.3.2/pyraisdk/rlog/log.py`

 * *Files identical despite different names*

### Comparing `pyraisdk-0.3.1/pyraisdk/rlog/logimp.py` & `pyraisdk-0.3.2/pyraisdk/rlog/logimp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 
 import multiprocessing as mp
+import os
 import queue
 import sys
 import signal
 import threading
 import time
 import traceback
 
 from typing import List, Optional
 
+import psutil
+
 from .log import (
     LOGGING_QUEUE_CAPACITY,
     SINK_BATCH_MAX_IDLE_SECS,
     Event,
     EventLogger,
     EventSink,
     LogLevel,
@@ -114,14 +117,18 @@
                 return
             self.process = mp.Process(target=self.main, daemon=True)
             self.process.start()
         
     def main(self):
         ''' entrance of backend process
         '''
+        # set high niceness for posix
+        if psutil.POSIX:
+            os.nice(19)
+        
         with self.mutex:
             # set quit signal
             signal.signal(signal.SIGINT, self.handle_signal)
             signal.signal(signal.SIGTERM, self.handle_signal)
             # start sinks
             self.categories_sinks_ready = [
                 self._get_ready_sinks(sinks) for sinks in self.categories_sinks
```

### Comparing `pyraisdk-0.3.1/pyraisdk/rlog/reporter.py` & `pyraisdk-0.3.2/pyraisdk/rlog/reporter.py`

 * *Files identical despite different names*

### Comparing `pyraisdk-0.3.1/PKG-INFO` & `pyraisdk-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyraisdk
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: Xiaodong Yang
 Author-email: xiaoyan@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -73,14 +73,29 @@
   ```
 When the CD pipeline deploys the model to an AML online deployment, it exports environment variables for each `BatchingConfig` field, which pyraisdk utilizes at process start to configure batching parameters. The CD pipeline also exports environment variables to enable pyraisdk to log to RAI's Azure Data Explorer clusters.
 
 ### Test or Deploy without RAI CD Pipeline
 
 Test or Deploy independetly outside of RAI CD Pipeline, it's required to set environment variables for `BatchingConfig` manually before object of `DynamicBatchModel` is created. Refer to [Batching Parameter](#batching-parameter-attention). 
 
+The recommended way to set these variables is calling `os.environ.setdefault` in `init()`. Like below:
+
+```python
+def init():
+    os.environ.setdefault('PYRAISDK_MAX_BATCH_SIZE', '12')
+    os.environ.setdefault('PYRAISDK_IDLE_BATCH_SIZE', '5')
+    os.environ.setdefault('PYRAISDK_MAX_BATCH_INTERVAL', '0.002')
+    ...
+    batch_model = DynamicBatchModel(malware_model)
+```
+
+This should work well independent of RAI CD Pipeline. And you don't need to specifically remove these 3 lines when switching to deploy in CD Pipeline. 
+
+But please note that this kind of code should be **Avoided**: `os.environ['PYRAISDK_MAX_BATCH_SIZE'] = '12'`. It will override the configuration from CD pipeline, which is not desirable in most cases.
+
 To enable log publishing (to eventhub), there are another several environment variables need to be set, refer to following logging part. It's optional.
 
 
 ## Dynamic Batching Support
 
 There are APIs you **must** implement in your model to support batching of inference requests for best model performance. Those APIs allow the SDK
 to distribute load efficiently to the GPU instances. The APIs are:
```

