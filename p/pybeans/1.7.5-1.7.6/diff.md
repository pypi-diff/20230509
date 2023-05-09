# Comparing `tmp/pybeans-1.7.5.tar.gz` & `tmp/pybeans-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybeans-1.7.5.tar", last modified: Mon May  8 12:21:06 2023, max compression
+gzip compressed data, was "dist/pybeans-1.7.6.tar", last modified: Tue May  9 13:01:06 2023, max compression
```

## Comparing `pybeans-1.7.5.tar` & `pybeans-1.7.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:21:06.000000 pybeans-1.7.5/
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-08 12:21:06.000000 pybeans-1.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-05-08 12:20:54.000000 pybeans-1.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:21:06.000000 pybeans-1.7.5/pybeans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-08 12:21:05.000000 pybeans-1.7.5/pybeans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-08 12:21:05.000000 pybeans-1.7.5/pybeans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 12:21:05.000000 pybeans-1.7.5/pybeans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-08 12:21:05.000000 pybeans-1.7.5/pybeans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      332 2023-05-08 12:21:06.000000 pybeans-1.7.5/pybeans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      802 2023-05-08 12:20:54.000000 pybeans-1.7.5/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-08 12:21:06.000000 pybeans-1.7.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:21:06.000000 pybeans-1.7.5/pybeans/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-08 12:20:54.000000 pybeans-1.7.5/pybeans/exception.py
--rw-r--r--   0 runner    (1001) docker     (122)    15361 2023-05-08 12:20:54.000000 pybeans-1.7.5/pybeans/app_tool.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-08 12:20:54.000000 pybeans-1.7.5/pybeans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-05-08 12:20:54.000000 pybeans-1.7.5/pybeans/ColorfulFormatter.py
--rw-r--r--   0 runner    (1001) docker     (122)      970 2023-05-08 12:20:54.000000 pybeans-1.7.5/pybeans/get_ch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-05-08 12:20:54.000000 pybeans-1.7.5/pybeans/config_sample.py
--rw-r--r--   0 runner    (1001) docker     (122)    21969 2023-05-08 12:20:54.000000 pybeans-1.7.5/pybeans/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:01:06.000000 pybeans-1.7.6/
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-09 13:01:06.000000 pybeans-1.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-05-09 13:00:42.000000 pybeans-1.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:01:06.000000 pybeans-1.7.6/pybeans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-09 13:01:05.000000 pybeans-1.7.6/pybeans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-09 13:01:05.000000 pybeans-1.7.6/pybeans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 13:01:05.000000 pybeans-1.7.6/pybeans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-09 13:01:05.000000 pybeans-1.7.6/pybeans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-05-09 13:01:05.000000 pybeans-1.7.6/pybeans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2023-05-09 13:00:42.000000 pybeans-1.7.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 13:01:06.000000 pybeans-1.7.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:01:06.000000 pybeans-1.7.6/pybeans/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-09 13:00:42.000000 pybeans-1.7.6/pybeans/exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15384 2023-05-09 13:00:42.000000 pybeans-1.7.6/pybeans/app_tool.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-09 13:00:42.000000 pybeans-1.7.6/pybeans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-05-09 13:00:42.000000 pybeans-1.7.6/pybeans/ColorfulFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      970 2023-05-09 13:00:42.000000 pybeans-1.7.6/pybeans/get_ch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-05-09 13:00:42.000000 pybeans-1.7.6/pybeans/config_sample.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21969 2023-05-09 13:00:42.000000 pybeans-1.7.6/pybeans/utils.py
```

### Comparing `pybeans-1.7.5/PKG-INFO` & `pybeans-1.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybeans
-Version: 1.7.5
+Version: 1.7.6
 Summary: Common toolkit for python.
 Home-page: https://github.com/chariothy/pybeans.git
 Author: Henry TIAN
 Author-email: chariothy@gmail.com
 License: MIT
 Description: # pybeans
         Common toolkit for python.
```

### Comparing `pybeans-1.7.5/setup.py` & `pybeans-1.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 NAME = 'pybeans'
 DESCRIPTION = 'Common toolkit for python.'
 PY_MODULES = ['pybeans']
 PACKAGES = ['pybeans']
 URL = 'https://github.com/chariothy/pybeans.git'
 EMAIL = 'chariothy@gmail.com'
 AUTHOR = 'Henry TIAN'
-VERSION = '1.7.5'
+VERSION = '1.7.6'
 
 LONG_DESCRIPTION = '''
 This is a helper which includes common methods and classes.
 
 '''
 
 # What packages are required for this module to be executed?
```

### Comparing `pybeans-1.7.5/pybeans.egg-info/PKG-INFO` & `pybeans-1.7.6/pybeans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybeans
-Version: 1.7.5
+Version: 1.7.6
 Summary: Common toolkit for python.
 Home-page: https://github.com/chariothy/pybeans.git
 Author: Henry TIAN
 Author-email: chariothy@gmail.com
 License: MIT
 Description: # pybeans
         Common toolkit for python.
```

### Comparing `pybeans-1.7.5/README.md` & `pybeans-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `pybeans-1.7.5/pybeans/app_tool.py` & `pybeans-1.7.6/pybeans/app_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,27 +148,26 @@
             [logger] -- Initialized logger.
         """
         
         smtp = self._config.get('smtp')
         mail = self._config.get('mail')
         logConfig = self._config.get('log', {})
 
-        logs_path = path.join(self._app_path, 'logs')
-        if not os.path.exists(logs_path):
-            os.mkdir(logs_path)
-
         logger = logging.getLogger(self._app_name)
         logLevel = logConfig.get('level', logging.DEBUG)
         logger.setLevel(logLevel)
 
         logDst = logConfig.get('dest', {})
 
         fileDest = logDst.get('file')
         if fileDest is not None:
             if not fileDest: # Empty
+                logs_path = path.join(self._app_path, 'logs')
+                if not os.path.exists(logs_path):
+                    os.mkdir(logs_path)
                 regular_log_name = re.sub(r'\W+', '_', self._app_name.lower())
                 fileDest = path.join(logs_path, f'{regular_log_name}.log')
             regular_log_name = re.sub(r'\W+', '_', self._app_name.lower())
             rf_handler = handlers.TimedRotatingFileHandler(fileDest, when='D', interval=1, backupCount=7, encoding='utf-8')
             rf_handler.suffix = "%Y-%m-%d_%H-%M-%S.log"
             rf_handler.level = logging.INFO
             rf_handler.setFormatter(logging.Formatter("%(asctime)s - %(levelname)s - %(message)s"))
```

### Comparing `pybeans-1.7.5/pybeans/ColorfulFormatter.py` & `pybeans-1.7.6/pybeans/ColorfulFormatter.py`

 * *Files identical despite different names*

### Comparing `pybeans-1.7.5/pybeans/get_ch.py` & `pybeans-1.7.6/pybeans/get_ch.py`

 * *Files identical despite different names*

### Comparing `pybeans-1.7.5/pybeans/config_sample.py` & `pybeans-1.7.6/pybeans/config_sample.py`

 * *Files identical despite different names*

### Comparing `pybeans-1.7.5/pybeans/utils.py` & `pybeans-1.7.6/pybeans/utils.py`

 * *Files identical despite different names*

