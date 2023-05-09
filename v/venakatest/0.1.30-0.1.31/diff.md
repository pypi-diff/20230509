# Comparing `tmp/venakatest-0.1.30.tar.gz` & `tmp/venakatest-0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "venakatest-0.1.30.tar", last modified: Tue May  9 04:00:30 2023, max compression
+gzip compressed data, was "venakatest-0.1.31.tar", last modified: Tue May  9 04:02:40 2023, max compression
```

## Comparing `venakatest-0.1.30.tar` & `venakatest-0.1.31.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 04:00:30.639323 venakatest-0.1.30/
--rw-rw-rw-   0        0        0       94 2023-05-09 04:00:30.638326 venakatest-0.1.30/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-04-20 09:43:51.000000 venakatest-0.1.30/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 04:00:30.639323 venakatest-0.1.30/setup.cfg
--rw-rw-rw-   0        0        0      312 2023-05-09 04:00:27.000000 venakatest-0.1.30/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 04:00:30.612321 venakatest-0.1.30/venakatest/
--rw-rw-rw-   0        0        0        0 2023-05-09 03:17:15.000000 venakatest-0.1.30/venakatest/__init__.py
--rw-rw-rw-   0        0        0     2359 2023-05-09 03:59:43.000000 venakatest-0.1.30/venakatest/test.py
-drwxrwxrwx   0        0        0        0 2023-05-09 04:00:30.637325 venakatest-0.1.30/venakatest.egg-info/
--rw-rw-rw-   0        0        0       94 2023-05-09 04:00:30.000000 venakatest-0.1.30/venakatest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-05-09 04:00:30.000000 venakatest-0.1.30/venakatest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 04:00:30.000000 venakatest-0.1.30/venakatest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-09 04:00:30.000000 venakatest-0.1.30/venakatest.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2023-05-09 04:00:30.000000 venakatest-0.1.30/venakatest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-09 04:00:30.000000 venakatest-0.1.30/venakatest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 04:02:40.177204 venakatest-0.1.31/
+-rw-rw-rw-   0        0        0       94 2023-05-09 04:02:40.176207 venakatest-0.1.31/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-04-20 09:43:51.000000 venakatest-0.1.31/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-09 04:02:40.177204 venakatest-0.1.31/setup.cfg
+-rw-rw-rw-   0        0        0      312 2023-05-09 04:02:37.000000 venakatest-0.1.31/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 04:02:40.159205 venakatest-0.1.31/venakatest/
+-rw-rw-rw-   0        0        0        0 2023-05-09 03:17:15.000000 venakatest-0.1.31/venakatest/__init__.py
+-rw-rw-rw-   0        0        0     1722 2023-05-09 04:02:27.000000 venakatest-0.1.31/venakatest/test.py
+drwxrwxrwx   0        0        0        0 2023-05-09 04:02:40.175207 venakatest-0.1.31/venakatest.egg-info/
+-rw-rw-rw-   0        0        0       94 2023-05-09 04:02:40.000000 venakatest-0.1.31/venakatest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-09 04:02:40.000000 venakatest-0.1.31/venakatest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 04:02:40.000000 venakatest-0.1.31/venakatest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-09 04:02:40.000000 venakatest-0.1.31/venakatest.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-05-09 04:02:40.000000 venakatest-0.1.31/venakatest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-09 04:02:40.000000 venakatest-0.1.31/venakatest.egg-info/top_level.txt
```

### Comparing `venakatest-0.1.30/venakatest/test.py` & `venakatest-0.1.31/venakatest/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,57 +12,30 @@
 import threading
 import logging.config
 import datetime
 def testing():
     return "ok"
 def exception_handler(type, value, tb):
     logging.exception("Uncaught exception: {0} {1} - Line : {2} ".format(str(value), str(type),str(tb.tb_lineno)))
-    
-DEBUG = True
-LOGGING_CONFIG = {
-    'version': 1,
-    'disable_existing_loggers': True,
-
-    'formatters': {
-        'default': {
-            'format': '[%(asctime)s] %(levelname)-8s [%(funcName)s:%(lineno)d] %(message)s',
-            'datefmt': '%Y-%m-%d %H:%M:%S'
-        },
-
-    },
-    'handlers': {
-        'console': {
-            'level': 'INFO',
-            'class': 'logging.StreamHandler',
-            'formatter': 'default'
-        },
-   
-    },
-    'loggers': {
-        '': {
-            'level': 'INFO' if not DEBUG else 'DEBUG',
-            'handlers': ['console', 'file']
-        },
-    }
-}
+logging.basicConfig(level=logging.DEBUG)
 def check():
     if len(sys.argv) > 0 and sys.argv[0].endswith('.bat'):
         logging.exception("Running from a batch file")
 
         print("Running from a batch file")
         # Additional batch-specific code here
     elif len(sys.argv) > 0 and sys.argv[0].endswith('.ps1'):
         print("Running from PowerShell")
         logging.exception("Running from a PowerShell file")
         # Additional PowerShell-specific code here
     else:
         logging.exception("Running from a Python file")
         print("Running directly from Python")
     # Code to handle other cases
-logging.config.dictConfig(LOGGING_CONFIG)
+
 # Install exception handler
 sys.excepthook = exception_handler
 
 def tobe():
     logging.info('Started syncing commits to {}'.format("testubg"))
     check()
     logging.info('Start commit: {}'.format("start"))
```

