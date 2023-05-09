# Comparing `tmp/python-ss-logging-tool-0.1.0.tar.gz` & `tmp/python-ss-logging-tool-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-ss-logging-tool-0.1.0.tar", last modified: Fri Mar 17 04:14:01 2023, max compression
+gzip compressed data, was "python-ss-logging-tool-0.1.1.tar", last modified: Tue May  9 06:10:31 2023, max compression
```

## Comparing `python-ss-logging-tool-0.1.0.tar` & `python-ss-logging-tool-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jimmychui   (501) staff       (20)        0 2023-03-17 04:14:01.259396 python-ss-logging-tool-0.1.0/
--rw-r--r--   0 jimmychui   (501) staff       (20)      751 2023-03-17 04:14:01.259105 python-ss-logging-tool-0.1.0/PKG-INFO
--rw-r--r--   0 jimmychui   (501) staff       (20)      187 2023-03-17 04:10:00.000000 python-ss-logging-tool-0.1.0/README.md
-drwxr-xr-x   0 jimmychui   (501) staff       (20)        0 2023-03-17 04:14:01.257592 python-ss-logging-tool-0.1.0/python_ss_logging_tool.egg-info/
--rw-r--r--   0 jimmychui   (501) staff       (20)      751 2023-03-17 04:14:00.000000 python-ss-logging-tool-0.1.0/python_ss_logging_tool.egg-info/PKG-INFO
--rw-r--r--   0 jimmychui   (501) staff       (20)      301 2023-03-17 04:14:01.000000 python-ss-logging-tool-0.1.0/python_ss_logging_tool.egg-info/SOURCES.txt
--rw-r--r--   0 jimmychui   (501) staff       (20)        1 2023-03-17 04:14:00.000000 python-ss-logging-tool-0.1.0/python_ss_logging_tool.egg-info/dependency_links.txt
--rw-r--r--   0 jimmychui   (501) staff       (20)       12 2023-03-17 04:14:00.000000 python-ss-logging-tool-0.1.0/python_ss_logging_tool.egg-info/requires.txt
--rw-r--r--   0 jimmychui   (501) staff       (20)       16 2023-03-17 04:14:00.000000 python-ss-logging-tool-0.1.0/python_ss_logging_tool.egg-info/top_level.txt
--rw-r--r--   0 jimmychui   (501) staff       (20)       38 2023-03-17 04:14:01.259507 python-ss-logging-tool-0.1.0/setup.cfg
--rw-r--r--   0 jimmychui   (501) staff       (20)      817 2023-03-17 04:13:09.000000 python-ss-logging-tool-0.1.0/setup.py
-drwxr-xr-x   0 jimmychui   (501) staff       (20)        0 2023-03-17 04:14:01.258590 python-ss-logging-tool-0.1.0/ss_logging_tool/
--rw-r--r--   0 jimmychui   (501) staff       (20)       26 2023-03-17 04:04:53.000000 python-ss-logging-tool-0.1.0/ss_logging_tool/__init__.py
--rw-r--r--   0 jimmychui   (501) staff       (20)     1546 2023-03-17 04:06:10.000000 python-ss-logging-tool-0.1.0/ss_logging_tool/logger.py
+drwxr-xr-x   0 jimmychui   (501) staff       (20)        0 2023-05-09 06:10:31.759573 python-ss-logging-tool-0.1.1/
+-rw-r--r--   0 jimmychui   (501) staff       (20)      714 2023-05-09 06:10:31.759161 python-ss-logging-tool-0.1.1/PKG-INFO
+-rw-r--r--   0 jimmychui   (501) staff       (20)      187 2023-03-17 04:10:00.000000 python-ss-logging-tool-0.1.1/README.md
+drwxr-xr-x   0 jimmychui   (501) staff       (20)        0 2023-05-09 06:10:31.756984 python-ss-logging-tool-0.1.1/python_ss_logging_tool.egg-info/
+-rw-r--r--   0 jimmychui   (501) staff       (20)      714 2023-05-09 06:10:31.000000 python-ss-logging-tool-0.1.1/python_ss_logging_tool.egg-info/PKG-INFO
+-rw-r--r--   0 jimmychui   (501) staff       (20)      301 2023-05-09 06:10:31.000000 python-ss-logging-tool-0.1.1/python_ss_logging_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 jimmychui   (501) staff       (20)        1 2023-05-09 06:10:31.000000 python-ss-logging-tool-0.1.1/python_ss_logging_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 jimmychui   (501) staff       (20)       12 2023-05-09 06:10:31.000000 python-ss-logging-tool-0.1.1/python_ss_logging_tool.egg-info/requires.txt
+-rw-r--r--   0 jimmychui   (501) staff       (20)       16 2023-05-09 06:10:31.000000 python-ss-logging-tool-0.1.1/python_ss_logging_tool.egg-info/top_level.txt
+-rw-r--r--   0 jimmychui   (501) staff       (20)       38 2023-05-09 06:10:31.759698 python-ss-logging-tool-0.1.1/setup.cfg
+-rw-r--r--   0 jimmychui   (501) staff       (20)      817 2023-05-09 06:10:22.000000 python-ss-logging-tool-0.1.1/setup.py
+drwxr-xr-x   0 jimmychui   (501) staff       (20)        0 2023-05-09 06:10:31.758327 python-ss-logging-tool-0.1.1/ss_logging_tool/
+-rw-r--r--   0 jimmychui   (501) staff       (20)       26 2023-03-17 04:04:53.000000 python-ss-logging-tool-0.1.1/ss_logging_tool/__init__.py
+-rw-r--r--   0 jimmychui   (501) staff       (20)     1795 2023-05-09 06:09:25.000000 python-ss-logging-tool-0.1.1/ss_logging_tool/logger.py
```

### Comparing `python-ss-logging-tool-0.1.0/PKG-INFO` & `python-ss-logging-tool-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: python-ss-logging-tool
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple logger package
 Home-page: https://github.com/yourusername/mypackage
 Author: Jimmy
 Author-email: jimm@xxx.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
@@ -19,9 +17,7 @@
 
 A simple modification of the pino logger
 Changes:
 - can log error as traceback in error level
 - can spawn child instance with a request_id. Useful for tracing a HTTP request
 - 
 
-
-
```

### Comparing `python-ss-logging-tool-0.1.0/python_ss_logging_tool.egg-info/PKG-INFO` & `python-ss-logging-tool-0.1.1/python_ss_logging_tool.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: python-ss-logging-tool
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple logger package
 Home-page: https://github.com/yourusername/mypackage
 Author: Jimmy
 Author-email: jimm@xxx.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
@@ -19,9 +17,7 @@
 
 A simple modification of the pino logger
 Changes:
 - can log error as traceback in error level
 - can spawn child instance with a request_id. Useful for tracing a HTTP request
 - 
 
-
-
```

### Comparing `python-ss-logging-tool-0.1.0/setup.py` & `python-ss-logging-tool-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name="python-ss-logging-tool",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[
         "pino",
         "nanoid",
         # Add other dependencies if needed
     ],
     author="Jimmy",
```

### Comparing `python-ss-logging-tool-0.1.0/ss_logging_tool/logger.py` & `python-ss-logging-tool-0.1.1/ss_logging_tool/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+import json
 from typing import Callable
 
 from pino import pino
 import nanoid
 import traceback
 
 
 class Logger:
     def __init__(self, logger: pino):
         self.logger = logger
 
     @staticmethod
     def create(app_name: str):
         logger = pino(
-            bindings={"apptype": app_name, "metas": "main"}
+            bindings={"apptype": app_name, "metas": "main"},
+            dump_function=lambda obj: json.dumps(obj, ensure_ascii=False)
         )
         return Logger(logger)
 
     def child(self, metas: dict = None):
         metas = metas or {}
         if 'request_id' not in metas:
             metas['request_id'] = nanoid.generate(size=10)
@@ -44,7 +46,14 @@
             self._call(self.logger.error, *args, **kwargs)
 
     def debug(self, *args, **kwargs):
         self._call(self.logger.debug, *args, **kwargs)
 
     def warn(self, *args, **kwargs):
         self._call(self.logger.warn, *args, **kwargs)
+
+
+logger = Logger.create("testing")
+# logger = pino(
+#     bindings={"apptype": 'testing', "metas": "main"},
+# )
+logger.info("莎士比亞是哪一年出生的")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

