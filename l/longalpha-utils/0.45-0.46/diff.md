# Comparing `tmp/longalpha_utils-0.45.tar.gz` & `tmp/longalpha_utils-0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.45.tar", last modified: Mon May  8 03:02:43 2023, max compression
+gzip compressed data, was "longalpha_utils-0.46.tar", last modified: Tue May  9 03:18:51 2023, max compression
```

## Comparing `longalpha_utils-0.45.tar` & `longalpha_utils-0.46.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:02:43.010789 longalpha_utils-0.45/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-08 03:02:43.010789 longalpha_utils-0.45/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:02:43.010789 longalpha_utils-0.45/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-08 03:02:28.000000 longalpha_utils-0.45/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-08 03:02:28.000000 longalpha_utils-0.45/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-08 03:02:28.000000 longalpha_utils-0.45/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-05-08 03:02:28.000000 longalpha_utils-0.45/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-08 03:02:28.000000 longalpha_utils-0.45/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-08 03:02:28.000000 longalpha_utils-0.45/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:02:43.010789 longalpha_utils-0.45/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-08 03:02:42.000000 longalpha_utils-0.45/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-08 03:02:43.000000 longalpha_utils-0.45/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 03:02:42.000000 longalpha_utils-0.45/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-08 03:02:42.000000 longalpha_utils-0.45/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 03:02:42.000000 longalpha_utils-0.45/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 03:02:43.010789 longalpha_utils-0.45/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-08 03:02:28.000000 longalpha_utils-0.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:18:51.588094 longalpha_utils-0.46/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 03:18:51.588094 longalpha_utils-0.46/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:18:51.588094 longalpha_utils-0.46/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-09 03:18:40.000000 longalpha_utils-0.46/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-09 03:18:40.000000 longalpha_utils-0.46/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-09 03:18:40.000000 longalpha_utils-0.46/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-05-09 03:18:40.000000 longalpha_utils-0.46/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-09 03:18:40.000000 longalpha_utils-0.46/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-09 03:18:40.000000 longalpha_utils-0.46/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:18:51.588094 longalpha_utils-0.46/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 03:18:51.000000 longalpha_utils-0.46/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-09 03:18:51.000000 longalpha_utils-0.46/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 03:18:51.000000 longalpha_utils-0.46/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-09 03:18:51.000000 longalpha_utils-0.46/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 03:18:51.000000 longalpha_utils-0.46/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 03:18:51.588094 longalpha_utils-0.46/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-09 03:18:40.000000 longalpha_utils-0.46/setup.py
```

### Comparing `longalpha_utils-0.45/longalpha_utils/messenger.py` & `longalpha_utils-0.46/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.45/longalpha_utils/transfers.py` & `longalpha_utils-0.46/longalpha_utils/transfers.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.45/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.46/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.45/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.46/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.45/setup.py` & `longalpha_utils-0.46/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.45",
+    version="0.46",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

