# Comparing `tmp/pybeans-1.7.6.tar.gz` & `tmp/pybeans-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybeans-1.7.6.tar", last modified: Tue May  9 13:01:06 2023, max compression
+gzip compressed data, was "dist/pybeans-1.8.0.tar", last modified: Tue May  9 16:04:00 2023, max compression
```

## Comparing `pybeans-1.7.6.tar` & `pybeans-1.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:01:06.000000 pybeans-1.7.6/
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-09 13:01:06.000000 pybeans-1.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-05-09 13:00:42.000000 pybeans-1.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:01:06.000000 pybeans-1.7.6/pybeans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-09 13:01:05.000000 pybeans-1.7.6/pybeans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-09 13:01:05.000000 pybeans-1.7.6/pybeans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 13:01:05.000000 pybeans-1.7.6/pybeans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-09 13:01:05.000000 pybeans-1.7.6/pybeans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      332 2023-05-09 13:01:05.000000 pybeans-1.7.6/pybeans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      802 2023-05-09 13:00:42.000000 pybeans-1.7.6/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 13:01:06.000000 pybeans-1.7.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:01:06.000000 pybeans-1.7.6/pybeans/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-09 13:00:42.000000 pybeans-1.7.6/pybeans/exception.py
--rw-r--r--   0 runner    (1001) docker     (122)    15384 2023-05-09 13:00:42.000000 pybeans-1.7.6/pybeans/app_tool.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-09 13:00:42.000000 pybeans-1.7.6/pybeans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-05-09 13:00:42.000000 pybeans-1.7.6/pybeans/ColorfulFormatter.py
--rw-r--r--   0 runner    (1001) docker     (122)      970 2023-05-09 13:00:42.000000 pybeans-1.7.6/pybeans/get_ch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-05-09 13:00:42.000000 pybeans-1.7.6/pybeans/config_sample.py
--rw-r--r--   0 runner    (1001) docker     (122)    21969 2023-05-09 13:00:42.000000 pybeans-1.7.6/pybeans/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:04:00.000000 pybeans-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-09 16:04:00.000000 pybeans-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-05-09 16:03:45.000000 pybeans-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:04:00.000000 pybeans-1.8.0/pybeans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-09 16:03:59.000000 pybeans-1.8.0/pybeans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-09 16:03:59.000000 pybeans-1.8.0/pybeans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 16:03:59.000000 pybeans-1.8.0/pybeans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-09 16:03:59.000000 pybeans-1.8.0/pybeans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-05-09 16:04:00.000000 pybeans-1.8.0/pybeans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2023-05-09 16:03:45.000000 pybeans-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 16:04:00.000000 pybeans-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 16:04:00.000000 pybeans-1.8.0/pybeans/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-09 16:03:45.000000 pybeans-1.8.0/pybeans/exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15457 2023-05-09 16:03:45.000000 pybeans-1.8.0/pybeans/app_tool.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-09 16:03:45.000000 pybeans-1.8.0/pybeans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-05-09 16:03:45.000000 pybeans-1.8.0/pybeans/ColorfulFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      970 2023-05-09 16:03:45.000000 pybeans-1.8.0/pybeans/get_ch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-05-09 16:03:45.000000 pybeans-1.8.0/pybeans/config_sample.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21969 2023-05-09 16:03:45.000000 pybeans-1.8.0/pybeans/utils.py
```

### Comparing `pybeans-1.7.6/PKG-INFO` & `pybeans-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybeans
-Version: 1.7.6
+Version: 1.8.0
 Summary: Common toolkit for python.
 Home-page: https://github.com/chariothy/pybeans.git
 Author: Henry TIAN
 Author-email: chariothy@gmail.com
 License: MIT
 Description: # pybeans
         Common toolkit for python.
```

### Comparing `pybeans-1.7.6/setup.py` & `pybeans-1.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 NAME = 'pybeans'
 DESCRIPTION = 'Common toolkit for python.'
 PY_MODULES = ['pybeans']
 PACKAGES = ['pybeans']
 URL = 'https://github.com/chariothy/pybeans.git'
 EMAIL = 'chariothy@gmail.com'
 AUTHOR = 'Henry TIAN'
-VERSION = '1.7.6'
+VERSION = '1.8.0'
 
 LONG_DESCRIPTION = '''
 This is a helper which includes common methods and classes.
 
 '''
 
 # What packages are required for this module to be executed?
```

### Comparing `pybeans-1.7.6/pybeans.egg-info/PKG-INFO` & `pybeans-1.8.0/pybeans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybeans
-Version: 1.7.6
+Version: 1.8.0
 Summary: Common toolkit for python.
 Home-page: https://github.com/chariothy/pybeans.git
 Author: Henry TIAN
 Author-email: chariothy@gmail.com
 License: MIT
 Description: # pybeans
         Common toolkit for python.
```

### Comparing `pybeans-1.7.6/README.md` & `pybeans-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pybeans-1.7.6/pybeans/app_tool.py` & `pybeans-1.8.0/pybeans/app_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         #all_formatter = logging.Formatter(fmt='%(name)s - %(levelno)s - %(levelname)s - %(pathname)s - %(filename)s - %(module)s - %(lineno)d - %(funcName)s - %(created)f - %(asctime)s - %(msecs)d  %(relativeCreated)d - %(thread)d -  %(threadName)s -  %(process)d - %(message)s ')        
         #print('Ex. >>> ',all_formatter.formatMessage(record))
 
         #help(record)
         #help(formatter)
         
         formatter = logging.Formatter(fmt=self.subject)
+        record.message = record.msg # To be compatible with Python 3.10 to avoid KeyError in formatMessage
         return formatter.formatMessage(record)
 
 
 class AppTool(object):
     def __init__(self, app_name: str, app_path: str='', local_config_dir: str='', config_name: str='config', ignore_env:bool=False):
         self._app_name = app_name
         self._app_path = app_path if app_path else os.getcwd()
@@ -171,24 +172,23 @@
             rf_handler.suffix = "%Y-%m-%d_%H-%M-%S.log"
             rf_handler.level = logging.INFO
             rf_handler.setFormatter(logging.Formatter("%(asctime)s - %(levelname)s - %(message)s"))
             logger.addHandler(rf_handler)
 
         mailDest = logDst.get('mail')
         if smtp and mailDest is not None:
-            from_addr = mail.get('from')
             #TODO: Use schema to validate smtp
             if not mailDest:    # Empty
                 to_addrs = mail.get('to')
             else:   # Ex. 'Henry TIAN <chariothy@gmail.com>'
                 to_addrs = mailDest
 
             mail_handler = MySMTPHandler(
                     mailhost = (smtp['host'], smtp['port']),
-                    fromaddr = from_addr,
+                    fromaddr = mail.get('from'),
                     toaddrs = to_addrs,
                     subject = '%(name)s - %(levelname)s - %(message)s',
                     credentials = (smtp['user'], smtp['pwd']))
             mail_handler.setLevel(logging.ERROR)
             logger.addHandler(mail_handler)
 
         stdoutDest = logDst.get('stdout')
```

### Comparing `pybeans-1.7.6/pybeans/ColorfulFormatter.py` & `pybeans-1.8.0/pybeans/ColorfulFormatter.py`

 * *Files identical despite different names*

### Comparing `pybeans-1.7.6/pybeans/get_ch.py` & `pybeans-1.8.0/pybeans/get_ch.py`

 * *Files identical despite different names*

### Comparing `pybeans-1.7.6/pybeans/config_sample.py` & `pybeans-1.8.0/pybeans/config_sample.py`

 * *Files identical despite different names*

### Comparing `pybeans-1.7.6/pybeans/utils.py` & `pybeans-1.8.0/pybeans/utils.py`

 * *Files identical despite different names*

