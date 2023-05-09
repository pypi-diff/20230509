# Comparing `tmp/utils_easy-0.0.4.tar.gz` & `tmp/utils_easy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_easy-0.0.4.tar", last modified: Mon May  1 03:43:02 2023, max compression
+gzip compressed data, was "utils_easy-0.0.5.tar", last modified: Tue May  9 02:38:59 2023, max compression
```

## Comparing `utils_easy-0.0.4.tar` & `utils_easy-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 03:43:02.745207 utils_easy-0.0.4/
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      492 2023-05-01 03:43:02.745207 utils_easy-0.0.4/PKG-INFO
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       62 2023-04-30 15:03:42.000000 utils_easy-0.0.4/README.md
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       38 2023-05-01 03:43:02.745207 utils_easy-0.0.4/setup.cfg
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      660 2023-05-01 03:41:51.000000 utils_easy-0.0.4/setup.py
-drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 03:43:02.741207 utils_easy-0.0.4/utils_easy/
-drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 03:43:02.741207 utils_easy-0.0.4/utils_easy/easy_logger/
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       39 2023-05-01 02:47:10.000000 utils_easy-0.0.4/utils_easy/easy_logger/__init__.py
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      637 2023-05-01 02:47:34.000000 utils_easy-0.0.4/utils_easy/easy_logger/logging_config.py
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)     1228 2023-05-01 02:48:02.000000 utils_easy-0.0.4/utils_easy/easy_logger/setup_logger.py
-drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 03:43:02.741207 utils_easy-0.0.4/utils_easy/stringfyobject/
--rw-r--r--   0 cybercore  (1000) cybercore  (1000)        0 2023-04-30 01:39:44.000000 utils_easy-0.0.4/utils_easy/stringfyobject/__init__.py
--rw-r--r--   0 cybercore  (1000) cybercore  (1000)      404 2023-04-30 12:00:32.000000 utils_easy-0.0.4/utils_easy/stringfyobject/config.py
--rw-r--r--   0 cybercore  (1000) cybercore  (1000)      645 2023-04-30 14:55:26.000000 utils_easy-0.0.4/utils_easy/stringfyobject/registry.py
-drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 03:43:02.741207 utils_easy-0.0.4/utils_easy.egg-info/
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      492 2023-05-01 03:43:02.000000 utils_easy-0.0.4/utils_easy.egg-info/PKG-INFO
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      381 2023-05-01 03:43:02.000000 utils_easy-0.0.4/utils_easy.egg-info/SOURCES.txt
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)        1 2023-05-01 03:43:02.000000 utils_easy-0.0.4/utils_easy.egg-info/dependency_links.txt
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       11 2023-05-01 03:43:02.000000 utils_easy-0.0.4/utils_easy.egg-info/top_level.txt
+drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-09 02:38:59.619656 utils_easy-0.0.5/
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      492 2023-05-09 02:38:59.619656 utils_easy-0.0.5/PKG-INFO
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       62 2023-04-30 15:03:42.000000 utils_easy-0.0.5/README.md
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       38 2023-05-09 02:38:59.619656 utils_easy-0.0.5/setup.cfg
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      660 2023-05-09 02:37:55.000000 utils_easy-0.0.5/setup.py
+drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-09 02:38:59.619656 utils_easy-0.0.5/utils_easy/
+drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-09 02:38:59.619656 utils_easy-0.0.5/utils_easy/easy_logger/
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       39 2023-05-01 02:47:10.000000 utils_easy-0.0.5/utils_easy/easy_logger/__init__.py
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      637 2023-05-01 02:47:34.000000 utils_easy-0.0.5/utils_easy/easy_logger/logging_config.py
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)     1198 2023-05-09 02:34:34.000000 utils_easy-0.0.5/utils_easy/easy_logger/setup_logger.py
+drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-09 02:38:59.619656 utils_easy-0.0.5/utils_easy/stringfyobject/
+-rw-r--r--   0 cybercore  (1000) cybercore  (1000)        0 2023-04-30 01:39:44.000000 utils_easy-0.0.5/utils_easy/stringfyobject/__init__.py
+-rw-r--r--   0 cybercore  (1000) cybercore  (1000)      404 2023-04-30 12:00:32.000000 utils_easy-0.0.5/utils_easy/stringfyobject/config.py
+-rw-r--r--   0 cybercore  (1000) cybercore  (1000)      645 2023-04-30 14:55:26.000000 utils_easy-0.0.5/utils_easy/stringfyobject/registry.py
+drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-09 02:38:59.619656 utils_easy-0.0.5/utils_easy.egg-info/
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      492 2023-05-09 02:38:59.000000 utils_easy-0.0.5/utils_easy.egg-info/PKG-INFO
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      381 2023-05-09 02:38:59.000000 utils_easy-0.0.5/utils_easy.egg-info/SOURCES.txt
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)        1 2023-05-09 02:38:59.000000 utils_easy-0.0.5/utils_easy.egg-info/dependency_links.txt
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       11 2023-05-09 02:38:59.000000 utils_easy-0.0.5/utils_easy.egg-info/top_level.txt
```

### Comparing `utils_easy-0.0.4/setup.py` & `utils_easy-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="utils_easy",
-    version="0.0.4",
+    version="0.0.5",
     packages=[
          'utils_easy.easy_logger',
          'utils_easy.stringfyobject'
        ],
     install_requires=[],
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `utils_easy-0.0.4/utils_easy/easy_logger/logging_config.py` & `utils_easy-0.0.5/utils_easy/easy_logger/logging_config.py`

 * *Files identical despite different names*

### Comparing `utils_easy-0.0.4/utils_easy/easy_logger/setup_logger.py` & `utils_easy-0.0.5/utils_easy/easy_logger/setup_logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     os.makedirs(log_dir, exist_ok=True)
 
     # apply configuration
     logging.config.dictConfig(LOGGING_CONFIG)
 
     # create logger
     logger = logging.getLogger(module_name)
-    logger.setLevel(logging.DEBUG if DEBUG else logging.WARNING)
+    logger.setLevel(logging.DEBUG)
     
     if not logger.handlers:
         # # get handler from config
         console_handler = logging.StreamHandler()
         console_handler.setLevel(LOGGING_CONFIG["handlers"]["console"]["level"])
         console_handler.setFormatter(logging.Formatter(LOGGING_CONFIG["formatters"]["default"]["format"]))
```

### Comparing `utils_easy-0.0.4/utils_easy/stringfyobject/registry.py` & `utils_easy-0.0.5/utils_easy/stringfyobject/registry.py`

 * *Files identical despite different names*

