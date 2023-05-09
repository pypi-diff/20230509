# Comparing `tmp/nexora-0.0.2.tar.gz` & `tmp/nexora-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexora-0.0.2.tar", last modified: Tue May  9 14:44:37 2023, max compression
+gzip compressed data, was "nexora-0.0.3.tar", last modified: Tue May  9 14:47:00 2023, max compression
```

## Comparing `nexora-0.0.2.tar` & `nexora-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 alicabukel   (501) staff       (20)        0 2023-05-09 14:44:37.650276 nexora-0.0.2/
--rw-r--r--   0 alicabukel   (501) staff       (20)    11357 2023-05-04 08:59:14.000000 nexora-0.0.2/LICENSE
--rw-r--r--   0 alicabukel   (501) staff       (20)      349 2023-05-09 14:44:37.650428 nexora-0.0.2/PKG-INFO
--rw-r--r--   0 alicabukel   (501) staff       (20)       45 2023-05-09 14:29:35.000000 nexora-0.0.2/README.md
-drwxr-xr-x   0 alicabukel   (501) staff       (20)        0 2023-05-09 14:44:37.645803 nexora-0.0.2/nexora/
--rw-r--r--   0 alicabukel   (501) staff       (20)       54 2023-05-09 14:43:59.000000 nexora-0.0.2/nexora/__init__.py
--rw-r--r--   0 alicabukel   (501) staff       (20)      331 2023-05-04 23:40:22.000000 nexora-0.0.2/nexora/api.py
--rw-r--r--   0 alicabukel   (501) staff       (20)    13108 2023-05-09 14:29:37.000000 nexora-0.0.2/nexora/autotuna.py
--rw-r--r--   0 alicabukel   (501) staff       (20)    25293 2023-05-09 14:29:37.000000 nexora-0.0.2/nexora/boruta.py
-drwxr-xr-x   0 alicabukel   (501) staff       (20)        0 2023-05-09 14:44:37.648229 nexora-0.0.2/nexora/cli/
--rw-r--r--   0 alicabukel   (501) staff       (20)      305 2023-05-06 21:12:06.000000 nexora-0.0.2/nexora/cli/__init__.py
--rw-r--r--   0 alicabukel   (501) staff       (20)     1227 2023-05-09 14:29:36.000000 nexora-0.0.2/nexora/cli/autotuna.py
--rw-r--r--   0 alicabukel   (501) staff       (20)     2361 2023-05-09 14:33:32.000000 nexora-0.0.2/nexora/cli/explain.py
--rw-r--r--   0 alicabukel   (501) staff       (20)     1122 2023-05-09 14:29:36.000000 nexora-0.0.2/nexora/cli/monitor.py
--rw-r--r--   0 alicabukel   (501) staff       (20)     1332 2023-05-09 14:29:37.000000 nexora-0.0.2/nexora/cli/predict.py
--rw-r--r--   0 alicabukel   (501) staff       (20)     1668 2023-05-09 14:29:37.000000 nexora-0.0.2/nexora/cli/serve.py
--rw-r--r--   0 alicabukel   (501) staff       (20)     5648 2023-05-09 14:29:37.000000 nexora-0.0.2/nexora/cli/train.py
--rw-r--r--   0 alicabukel   (501) staff       (20)      181 2023-05-06 13:16:06.000000 nexora-0.0.2/nexora/config.py
--rw-r--r--   0 alicabukel   (501) staff       (20)     1444 2023-05-09 14:29:37.000000 nexora-0.0.2/nexora/enums.py
--rw-r--r--   0 alicabukel   (501) staff       (20)      391 2023-05-09 14:33:55.000000 nexora-0.0.2/nexora/logger.py
--rw-r--r--   0 alicabukel   (501) staff       (20)     3374 2023-05-09 14:29:37.000000 nexora-0.0.2/nexora/metrics.py
--rw-r--r--   0 alicabukel   (501) staff       (20)     2644 2023-05-09 14:29:37.000000 nexora-0.0.2/nexora/params.py
--rw-r--r--   0 alicabukel   (501) staff       (20)     4763 2023-05-09 14:29:37.000000 nexora-0.0.2/nexora/predict.py
--rw-r--r--   0 alicabukel   (501) staff       (20)      504 2023-05-09 11:12:34.000000 nexora-0.0.2/nexora/schemas.py
--rw-r--r--   0 alicabukel   (501) staff       (20)    18458 2023-05-09 14:34:09.000000 nexora-0.0.2/nexora/utils.py
-drwxr-xr-x   0 alicabukel   (501) staff       (20)        0 2023-05-09 14:44:37.649973 nexora-0.0.2/nexora.egg-info/
--rw-r--r--   0 alicabukel   (501) staff       (20)      349 2023-05-09 14:44:37.000000 nexora-0.0.2/nexora.egg-info/PKG-INFO
--rw-r--r--   0 alicabukel   (501) staff       (20)      629 2023-05-09 14:44:37.000000 nexora-0.0.2/nexora.egg-info/SOURCES.txt
--rw-r--r--   0 alicabukel   (501) staff       (20)        1 2023-05-09 14:44:37.000000 nexora-0.0.2/nexora.egg-info/dependency_links.txt
--rw-r--r--   0 alicabukel   (501) staff       (20)       52 2023-05-09 14:44:37.000000 nexora-0.0.2/nexora.egg-info/entry_points.txt
--rw-r--r--   0 alicabukel   (501) staff       (20)      234 2023-05-09 14:44:37.000000 nexora-0.0.2/nexora.egg-info/requires.txt
--rw-r--r--   0 alicabukel   (501) staff       (20)        7 2023-05-09 14:44:37.000000 nexora-0.0.2/nexora.egg-info/top_level.txt
--rw-r--r--   0 alicabukel   (501) staff       (20)      122 2023-05-04 09:39:11.000000 nexora-0.0.2/pyproject.toml
--rw-r--r--   0 alicabukel   (501) staff       (20)      972 2023-05-09 14:44:37.650951 nexora-0.0.2/setup.cfg
--rw-r--r--   0 alicabukel   (501) staff       (20)      398 2023-05-09 11:29:03.000000 nexora-0.0.2/setup.py
+drwxr-xr-x   0 alicabukel   (501) staff       (20)        0 2023-05-09 14:47:00.844604 nexora-0.0.3/
+-rw-r--r--   0 alicabukel   (501) staff       (20)    11357 2023-05-04 08:59:14.000000 nexora-0.0.3/LICENSE
+-rw-r--r--   0 alicabukel   (501) staff       (20)      349 2023-05-09 14:47:00.844770 nexora-0.0.3/PKG-INFO
+-rw-r--r--   0 alicabukel   (501) staff       (20)       45 2023-05-09 14:29:35.000000 nexora-0.0.3/README.md
+drwxr-xr-x   0 alicabukel   (501) staff       (20)        0 2023-05-09 14:47:00.836893 nexora-0.0.3/nexora/
+-rw-r--r--   0 alicabukel   (501) staff       (20)       54 2023-05-09 14:46:37.000000 nexora-0.0.3/nexora/__init__.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)      331 2023-05-04 23:40:22.000000 nexora-0.0.3/nexora/api.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)    13108 2023-05-09 14:29:37.000000 nexora-0.0.3/nexora/autotuna.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)    25293 2023-05-09 14:29:37.000000 nexora-0.0.3/nexora/boruta.py
+drwxr-xr-x   0 alicabukel   (501) staff       (20)        0 2023-05-09 14:47:00.841909 nexora-0.0.3/nexora/cli/
+-rw-r--r--   0 alicabukel   (501) staff       (20)      305 2023-05-06 21:12:06.000000 nexora-0.0.3/nexora/cli/__init__.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     1227 2023-05-09 14:29:36.000000 nexora-0.0.3/nexora/cli/autotuna.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     2361 2023-05-09 14:33:32.000000 nexora-0.0.3/nexora/cli/explain.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     1122 2023-05-09 14:29:36.000000 nexora-0.0.3/nexora/cli/monitor.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     1332 2023-05-09 14:29:37.000000 nexora-0.0.3/nexora/cli/predict.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     1668 2023-05-09 14:29:37.000000 nexora-0.0.3/nexora/cli/serve.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     5648 2023-05-09 14:29:37.000000 nexora-0.0.3/nexora/cli/train.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)      181 2023-05-06 13:16:06.000000 nexora-0.0.3/nexora/config.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     1444 2023-05-09 14:29:37.000000 nexora-0.0.3/nexora/enums.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)      391 2023-05-09 14:33:55.000000 nexora-0.0.3/nexora/logger.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     3374 2023-05-09 14:29:37.000000 nexora-0.0.3/nexora/metrics.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     2644 2023-05-09 14:29:37.000000 nexora-0.0.3/nexora/params.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     4763 2023-05-09 14:29:37.000000 nexora-0.0.3/nexora/predict.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)      504 2023-05-09 11:12:34.000000 nexora-0.0.3/nexora/schemas.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)    18458 2023-05-09 14:34:09.000000 nexora-0.0.3/nexora/utils.py
+drwxr-xr-x   0 alicabukel   (501) staff       (20)        0 2023-05-09 14:47:00.844271 nexora-0.0.3/nexora.egg-info/
+-rw-r--r--   0 alicabukel   (501) staff       (20)      349 2023-05-09 14:47:00.000000 nexora-0.0.3/nexora.egg-info/PKG-INFO
+-rw-r--r--   0 alicabukel   (501) staff       (20)      629 2023-05-09 14:47:00.000000 nexora-0.0.3/nexora.egg-info/SOURCES.txt
+-rw-r--r--   0 alicabukel   (501) staff       (20)        1 2023-05-09 14:47:00.000000 nexora-0.0.3/nexora.egg-info/dependency_links.txt
+-rw-r--r--   0 alicabukel   (501) staff       (20)       52 2023-05-09 14:47:00.000000 nexora-0.0.3/nexora.egg-info/entry_points.txt
+-rw-r--r--   0 alicabukel   (501) staff       (20)      234 2023-05-09 14:47:00.000000 nexora-0.0.3/nexora.egg-info/requires.txt
+-rw-r--r--   0 alicabukel   (501) staff       (20)        7 2023-05-09 14:47:00.000000 nexora-0.0.3/nexora.egg-info/top_level.txt
+-rw-r--r--   0 alicabukel   (501) staff       (20)      122 2023-05-04 09:39:11.000000 nexora-0.0.3/pyproject.toml
+-rw-r--r--   0 alicabukel   (501) staff       (20)      972 2023-05-09 14:47:00.845311 nexora-0.0.3/setup.cfg
+-rw-r--r--   0 alicabukel   (501) staff       (20)      398 2023-05-09 11:29:03.000000 nexora-0.0.3/setup.py
```

### Comparing `nexora-0.0.2/LICENSE` & `nexora-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nexora-0.0.2/nexora/autotuna.py` & `nexora-0.0.3/nexora/autotuna.py`

 * *Files identical despite different names*

### Comparing `nexora-0.0.2/nexora/boruta.py` & `nexora-0.0.3/nexora/boruta.py`

 * *Files identical despite different names*

### Comparing `nexora-0.0.2/nexora/cli/autotuna.py` & `nexora-0.0.3/nexora/cli/autotuna.py`

 * *Files identical despite different names*

### Comparing `nexora-0.0.2/nexora/cli/explain.py` & `nexora-0.0.3/nexora/cli/explain.py`

 * *Files identical despite different names*

### Comparing `nexora-0.0.2/nexora/cli/monitor.py` & `nexora-0.0.3/nexora/cli/monitor.py`

 * *Files identical despite different names*

### Comparing `nexora-0.0.2/nexora/cli/predict.py` & `nexora-0.0.3/nexora/cli/predict.py`

 * *Files identical despite different names*

### Comparing `nexora-0.0.2/nexora/cli/serve.py` & `nexora-0.0.3/nexora/cli/serve.py`

 * *Files identical despite different names*

### Comparing `nexora-0.0.2/nexora/cli/train.py` & `nexora-0.0.3/nexora/cli/train.py`

 * *Files identical despite different names*

### Comparing `nexora-0.0.2/nexora/enums.py` & `nexora-0.0.3/nexora/enums.py`

 * *Files identical despite different names*

### Comparing `nexora-0.0.2/nexora/metrics.py` & `nexora-0.0.3/nexora/metrics.py`

 * *Files identical despite different names*

### Comparing `nexora-0.0.2/nexora/params.py` & `nexora-0.0.3/nexora/params.py`

 * *Files identical despite different names*

### Comparing `nexora-0.0.2/nexora/predict.py` & `nexora-0.0.3/nexora/predict.py`

 * *Files identical despite different names*

### Comparing `nexora-0.0.2/nexora/utils.py` & `nexora-0.0.3/nexora/utils.py`

 * *Files identical despite different names*

### Comparing `nexora-0.0.2/nexora.egg-info/SOURCES.txt` & `nexora-0.0.3/nexora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nexora-0.0.2/setup.cfg` & `nexora-0.0.3/setup.cfg`

 * *Files identical despite different names*

