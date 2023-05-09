# Comparing `tmp/venakatest-0.1.11.tar.gz` & `tmp/venakatest-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "venakatest-0.1.11.tar", last modified: Tue May  9 03:40:49 2023, max compression
+gzip compressed data, was "venakatest-0.1.23.tar", last modified: Tue May  9 03:49:48 2023, max compression
```

## Comparing `venakatest-0.1.11.tar` & `venakatest-0.1.23.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 03:40:49.068161 venakatest-0.1.11/
--rw-rw-rw-   0        0        0       94 2023-05-09 03:40:49.067161 venakatest-0.1.11/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-04-20 09:43:51.000000 venakatest-0.1.11/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 03:40:49.068161 venakatest-0.1.11/setup.cfg
--rw-rw-rw-   0        0        0      225 2023-05-09 03:39:57.000000 venakatest-0.1.11/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 03:40:49.042161 venakatest-0.1.11/venakatest/
--rw-rw-rw-   0        0        0        0 2023-05-09 03:17:15.000000 venakatest-0.1.11/venakatest/__init__.py
--rw-rw-rw-   0        0        0     1795 2023-05-09 03:21:39.000000 venakatest-0.1.11/venakatest/test.py
-drwxrwxrwx   0        0        0        0 2023-05-09 03:40:49.066161 venakatest-0.1.11/venakatest.egg-info/
--rw-rw-rw-   0        0        0       94 2023-05-09 03:40:48.000000 venakatest-0.1.11/venakatest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-05-09 03:40:48.000000 venakatest-0.1.11/venakatest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 03:40:48.000000 venakatest-0.1.11/venakatest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-09 03:40:48.000000 venakatest-0.1.11/venakatest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-09 03:40:48.000000 venakatest-0.1.11/venakatest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 03:49:48.612609 venakatest-0.1.23/
+-rw-rw-rw-   0        0        0       94 2023-05-09 03:49:48.611607 venakatest-0.1.23/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-04-20 09:43:51.000000 venakatest-0.1.23/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-09 03:49:48.612609 venakatest-0.1.23/setup.cfg
+-rw-rw-rw-   0        0        0      225 2023-05-09 03:47:52.000000 venakatest-0.1.23/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:49:48.596605 venakatest-0.1.23/venakatest/
+-rw-rw-rw-   0        0        0        0 2023-05-09 03:17:15.000000 venakatest-0.1.23/venakatest/__init__.py
+-rw-rw-rw-   0        0        0     2654 2023-05-09 03:46:40.000000 venakatest-0.1.23/venakatest/test.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:49:48.608605 venakatest-0.1.23/venakatest.egg-info/
+-rw-rw-rw-   0        0        0       94 2023-05-09 03:49:48.000000 venakatest-0.1.23/venakatest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-05-09 03:49:48.000000 venakatest-0.1.23/venakatest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 03:49:48.000000 venakatest-0.1.23/venakatest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-09 03:49:48.000000 venakatest-0.1.23/venakatest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-09 03:49:48.000000 venakatest-0.1.23/venakatest.egg-info/top_level.txt
```

### Comparing `venakatest-0.1.11/venakatest/test.py` & `venakatest-0.1.23/venakatest/test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,21 @@
+
+import binascii
+import traceback
+import warnings
 import sys
+import argparse
+import subprocess
+import json
+import re
 import logging
+import os
+import threading
 import logging.config
+import datetime
 def testing():
     return "ok"
 def exception_handler(type, value, tb):
     logging.exception("Uncaught exception: {0} {1} - Line : {2} ".format(str(value), str(type),str(tb.tb_lineno)))
     
 DEBUG = True
 LOGGING_CONFIG = {
@@ -36,24 +47,50 @@
     'loggers': {
         '': {
             'level': 'INFO' if not DEBUG else 'DEBUG',
             'handlers': ['console', 'file']
         },
     }
 }
-if len(sys.argv) > 0 and sys.argv[0].endswith('.bat'):
-    logging.exception("Running from a batch file")
+def check():
+    if len(sys.argv) > 0 and sys.argv[0].endswith('.bat'):
+        logging.exception("Running from a batch file")
 
-    print("Running from a batch file")
-    # Additional batch-specific code here
-elif len(sys.argv) > 0 and sys.argv[0].endswith('.ps1'):
-    print("Running from PowerShell")
-    logging.exception("Running from a PowerShell file")
-    # Additional PowerShell-specific code here
-else:
-    logging.exception("Running from a Python file")
-    print("Running directly from Python")
+        print("Running from a batch file")
+        # Additional batch-specific code here
+    elif len(sys.argv) > 0 and sys.argv[0].endswith('.ps1'):
+        print("Running from PowerShell")
+        logging.exception("Running from a PowerShell file")
+        # Additional PowerShell-specific code here
+    else:
+        logging.exception("Running from a Python file")
+        print("Running directly from Python")
     # Code to handle other cases
 logging.config.dictConfig(LOGGING_CONFIG)
 # Install exception handler
 sys.excepthook = exception_handler
 
+def gittoappsurify():
+    logging.info('Started syncing commits to {}'.format("testubg"))
+    check()
+    logging.info('Start commit: {}'.format("start"))
+
+
+parser = argparse.ArgumentParser(description='Sync a number of commits before a specific commit')
+
+parser.add_argument('--project', type=str, required=True,
+                    help='Enter project name')
+parser.add_argument('--token', type=str, required=True,
+                    help='The API key to communicate with API')
+
+args = parser.parse_args()
+
+project = args.project
+token = args.token
+
+debug = True
+
+
+
+
+if __name__ == '__main__':
+    gittoappsurify()
```

