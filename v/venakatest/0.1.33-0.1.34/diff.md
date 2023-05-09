# Comparing `tmp/venakatest-0.1.33.tar.gz` & `tmp/venakatest-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "venakatest-0.1.33.tar", last modified: Tue May  9 04:15:39 2023, max compression
+gzip compressed data, was "venakatest-0.1.34.tar", last modified: Tue May  9 04:19:08 2023, max compression
```

## Comparing `venakatest-0.1.33.tar` & `venakatest-0.1.34.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 04:15:39.446901 venakatest-0.1.33/
--rw-rw-rw-   0        0        0       94 2023-05-09 04:15:39.445903 venakatest-0.1.33/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-04-20 09:43:51.000000 venakatest-0.1.33/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 04:15:39.446901 venakatest-0.1.33/setup.cfg
--rw-rw-rw-   0        0        0      312 2023-05-09 04:15:34.000000 venakatest-0.1.33/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 04:15:39.429901 venakatest-0.1.33/venakatest/
--rw-rw-rw-   0        0        0        0 2023-05-09 03:17:15.000000 venakatest-0.1.33/venakatest/__init__.py
--rw-rw-rw-   0        0        0     1833 2023-05-09 04:15:28.000000 venakatest-0.1.33/venakatest/test.py
-drwxrwxrwx   0        0        0        0 2023-05-09 04:15:39.444902 venakatest-0.1.33/venakatest.egg-info/
--rw-rw-rw-   0        0        0       94 2023-05-09 04:15:39.000000 venakatest-0.1.33/venakatest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-05-09 04:15:39.000000 venakatest-0.1.33/venakatest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 04:15:39.000000 venakatest-0.1.33/venakatest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-09 04:15:39.000000 venakatest-0.1.33/venakatest.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2023-05-09 04:15:39.000000 venakatest-0.1.33/venakatest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-09 04:15:39.000000 venakatest-0.1.33/venakatest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 04:19:08.947512 venakatest-0.1.34/
+-rw-rw-rw-   0        0        0       94 2023-05-09 04:19:08.947512 venakatest-0.1.34/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-04-20 09:43:51.000000 venakatest-0.1.34/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-09 04:19:08.948512 venakatest-0.1.34/setup.cfg
+-rw-rw-rw-   0        0        0      312 2023-05-09 04:18:55.000000 venakatest-0.1.34/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 04:19:08.932512 venakatest-0.1.34/venakatest/
+-rw-rw-rw-   0        0        0        0 2023-05-09 03:17:15.000000 venakatest-0.1.34/venakatest/__init__.py
+-rw-rw-rw-   0        0        0     1951 2023-05-09 04:18:48.000000 venakatest-0.1.34/venakatest/test.py
+drwxrwxrwx   0        0        0        0 2023-05-09 04:19:08.946511 venakatest-0.1.34/venakatest.egg-info/
+-rw-rw-rw-   0        0        0       94 2023-05-09 04:19:08.000000 venakatest-0.1.34/venakatest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-09 04:19:08.000000 venakatest-0.1.34/venakatest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 04:19:08.000000 venakatest-0.1.34/venakatest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-09 04:19:08.000000 venakatest-0.1.34/venakatest.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-05-09 04:19:08.000000 venakatest-0.1.34/venakatest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-09 04:19:08.000000 venakatest-0.1.34/venakatest.egg-info/top_level.txt
```

### Comparing `venakatest-0.1.33/venakatest/test.py` & `venakatest-0.1.34/venakatest/test.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,19 +19,19 @@
     return "ok"
 def exception_handler(type, value, tb):
     logging.exception("Uncaught exception: {0} {1} - Line : {2} ".format(str(value), str(type),str(tb.tb_lineno)))
 logging.basicConfig(level=logging.DEBUG)
 def check():
     
         # Additional batch-specific code here
-    if os.environ.get('COMSPEC', '').endswith('cmd.exe'):
+    if os.environ.get('COMSPEC', '').endswith('cmd.exe') and not os.path.basename(sys.executable) == 'powershell.exe':
         print("Running from batch")
         logging.exception("Running from a batch file")
         # Additional PowerShell-specific code here
-    elif 'MyInvocation' in str(globals().get('Get-Variable')):
+    elif 'MyInvocation' in str(globals().get('Get-Variable')) and os.path.basename(sys.executable) == 'powershell.exe':
         logging.exception("Running from a powershell file")
         print("Running directly from powershell")
     else:
         logging.exception("Running from python file")
 
         print("Running from a python file")
     # Code to handle other cases
```

