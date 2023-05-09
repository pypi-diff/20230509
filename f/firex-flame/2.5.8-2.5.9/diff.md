# Comparing `tmp/firex_flame-2.5.8.tar.gz` & `tmp/firex_flame-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/firex_flame-2.5.8.tar", last modified: Tue Feb  2 20:39:03 2021, max compression
+gzip compressed data, was "dist/firex_flame-2.5.9.tar", last modified: Tue Feb  2 20:57:45 2021, max compression
```

## Comparing `firex_flame-2.5.8.tar` & `firex_flame-2.5.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 firex      (100) nogroup  (65533)        0 2021-02-02 20:39:03.000000 firex_flame-2.5.8/
--rw-rw-rw-   0 firex      (100) nogroup  (65533)     1505 2021-02-02 20:38:49.000000 firex_flame-2.5.8/LICENSE
--rw-rw-rw-   0 firex      (100) nogroup  (65533)      103 2021-02-02 20:38:49.000000 firex_flame-2.5.8/MANIFEST.in
--rw-r--r--   0 firex      (100) nogroup  (65533)      274 2021-02-02 20:39:03.000000 firex_flame-2.5.8/PKG-INFO
--rw-rw-rw-   0 firex      (100) nogroup  (65533)     1624 2021-02-02 20:38:49.000000 firex_flame-2.5.8/README.md
--rw-rw-rw-   0 firex      (100) nogroup  (65533)     4042 2021-02-02 20:38:49.000000 firex_flame-2.5.8/fastentrypoints.py
-drwxr-xr-x   0 firex      (100) nogroup  (65533)        0 2021-02-02 20:39:03.000000 firex_flame-2.5.8/firex_flame/
--rw-rw-rw-   0 firex      (100) nogroup  (65533)       92 2021-02-02 20:38:49.000000 firex_flame-2.5.8/firex_flame/__init__.py
--rw-rw-rw-   0 firex      (100) nogroup  (65533)     7656 2021-02-02 20:38:49.000000 firex_flame-2.5.8/firex_flame/__main__.py
--rw-r--r--   0 firex      (100) nogroup  (65533)      497 2021-02-02 20:39:03.000000 firex_flame-2.5.8/firex_flame/_version.py
--rw-rw-rw-   0 firex      (100) nogroup  (65533)    12609 2021-02-02 20:38:49.000000 firex_flame-2.5.8/firex_flame/api.py
--rw-rw-rw-   0 firex      (100) nogroup  (65533)     3237 2021-02-02 20:38:49.000000 firex_flame-2.5.8/firex_flame/controller.py
--rw-rw-rw-   0 firex      (100) nogroup  (65533)    11490 2021-02-02 20:38:49.000000 firex_flame-2.5.8/firex_flame/event_aggregator.py
--rw-rw-rw-   0 firex      (100) nogroup  (65533)     5211 2021-02-02 20:38:49.000000 firex_flame-2.5.8/firex_flame/event_broker_processor.py
--rw-rw-rw-   0 firex      (100) nogroup  (65533)     3814 2021-02-02 20:38:49.000000 firex_flame-2.5.8/firex_flame/event_file_processor.py
--rw-rw-rw-   0 firex      (100) nogroup  (65533)    16850 2021-02-02 20:38:49.000000 firex_flame-2.5.8/firex_flame/flame_helper.py
--rw-rw-rw-   0 firex      (100) nogroup  (65533)     7062 2021-02-02 20:38:49.000000 firex_flame-2.5.8/firex_flame/launcher.py
--rw-rw-rw-   0 firex      (100) nogroup  (65533)     2512 2021-02-02 20:38:49.000000 firex_flame-2.5.8/firex_flame/main_app.py
--rw-rw-rw-   0 firex      (100) nogroup  (65533)     9228 2021-02-02 20:38:49.000000 firex_flame-2.5.8/firex_flame/model_dumper.py
-drwxr-xr-x   0 firex      (100) nogroup  (65533)        0 2021-02-02 20:39:03.000000 firex_flame-2.5.8/firex_flame/templates/
--rw-rw-rw-   0 firex      (100) nogroup  (65533)     2530 2021-02-02 20:38:49.000000 firex_flame-2.5.8/firex_flame/templates/index.html
--rw-rw-rw-   0 firex      (100) nogroup  (65533)     7895 2021-02-02 20:38:49.000000 firex_flame-2.5.8/firex_flame/web_app.py
-drwxr-xr-x   0 firex      (100) nogroup  (65533)        0 2021-02-02 20:39:03.000000 firex_flame-2.5.8/firex_flame.egg-info/
--rw-r--r--   0 firex      (100) nogroup  (65533)      274 2021-02-02 20:39:02.000000 firex_flame-2.5.8/firex_flame.egg-info/PKG-INFO
--rw-r--r--   0 firex      (100) nogroup  (65533)      706 2021-02-02 20:39:02.000000 firex_flame-2.5.8/firex_flame.egg-info/SOURCES.txt
--rw-r--r--   0 firex      (100) nogroup  (65533)        1 2021-02-02 20:39:02.000000 firex_flame-2.5.8/firex_flame.egg-info/dependency_links.txt
--rw-r--r--   0 firex      (100) nogroup  (65533)      195 2021-02-02 20:39:02.000000 firex_flame-2.5.8/firex_flame.egg-info/entry_points.txt
--rw-r--r--   0 firex      (100) nogroup  (65533)      239 2021-02-02 20:39:02.000000 firex_flame-2.5.8/firex_flame.egg-info/requires.txt
--rw-r--r--   0 firex      (100) nogroup  (65533)       12 2021-02-02 20:39:02.000000 firex_flame-2.5.8/firex_flame.egg-info/top_level.txt
--rw-r--r--   0 firex      (100) nogroup  (65533)        1 2021-02-02 20:39:02.000000 firex_flame-2.5.8/firex_flame.egg-info/zip-safe
--rw-rw-rw-   0 firex      (100) nogroup  (65533)      276 2021-02-02 20:39:03.000000 firex_flame-2.5.8/setup.cfg
--rw-rw-rw-   0 firex      (100) nogroup  (65533)     1832 2021-02-02 20:38:49.000000 firex_flame-2.5.8/setup.py
--rw-rw-rw-   0 firex      (100) nogroup  (65533)    70144 2021-02-02 20:38:49.000000 firex_flame-2.5.8/versioneer.py
+drwxr-xr-x   0 firex      (100) nogroup  (65533)        0 2021-02-02 20:57:45.000000 firex_flame-2.5.9/
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)     1505 2021-02-02 20:57:32.000000 firex_flame-2.5.9/LICENSE
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)      103 2021-02-02 20:57:32.000000 firex_flame-2.5.9/MANIFEST.in
+-rw-r--r--   0 firex      (100) nogroup  (65533)      274 2021-02-02 20:57:45.000000 firex_flame-2.5.9/PKG-INFO
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)     1624 2021-02-02 20:57:32.000000 firex_flame-2.5.9/README.md
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)     4042 2021-02-02 20:57:32.000000 firex_flame-2.5.9/fastentrypoints.py
+drwxr-xr-x   0 firex      (100) nogroup  (65533)        0 2021-02-02 20:57:45.000000 firex_flame-2.5.9/firex_flame/
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)       92 2021-02-02 20:57:32.000000 firex_flame-2.5.9/firex_flame/__init__.py
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)     7656 2021-02-02 20:57:32.000000 firex_flame-2.5.9/firex_flame/__main__.py
+-rw-r--r--   0 firex      (100) nogroup  (65533)      497 2021-02-02 20:57:45.000000 firex_flame-2.5.9/firex_flame/_version.py
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)    12609 2021-02-02 20:57:32.000000 firex_flame-2.5.9/firex_flame/api.py
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)     3237 2021-02-02 20:57:32.000000 firex_flame-2.5.9/firex_flame/controller.py
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)    11490 2021-02-02 20:57:32.000000 firex_flame-2.5.9/firex_flame/event_aggregator.py
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)     5211 2021-02-02 20:57:32.000000 firex_flame-2.5.9/firex_flame/event_broker_processor.py
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)     3814 2021-02-02 20:57:32.000000 firex_flame-2.5.9/firex_flame/event_file_processor.py
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)    16850 2021-02-02 20:57:32.000000 firex_flame-2.5.9/firex_flame/flame_helper.py
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)     7062 2021-02-02 20:57:32.000000 firex_flame-2.5.9/firex_flame/launcher.py
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)     2512 2021-02-02 20:57:32.000000 firex_flame-2.5.9/firex_flame/main_app.py
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)     9228 2021-02-02 20:57:32.000000 firex_flame-2.5.9/firex_flame/model_dumper.py
+drwxr-xr-x   0 firex      (100) nogroup  (65533)        0 2021-02-02 20:57:45.000000 firex_flame-2.5.9/firex_flame/templates/
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)     2530 2021-02-02 20:57:32.000000 firex_flame-2.5.9/firex_flame/templates/index.html
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)     7895 2021-02-02 20:57:32.000000 firex_flame-2.5.9/firex_flame/web_app.py
+drwxr-xr-x   0 firex      (100) nogroup  (65533)        0 2021-02-02 20:57:45.000000 firex_flame-2.5.9/firex_flame.egg-info/
+-rw-r--r--   0 firex      (100) nogroup  (65533)      274 2021-02-02 20:57:45.000000 firex_flame-2.5.9/firex_flame.egg-info/PKG-INFO
+-rw-r--r--   0 firex      (100) nogroup  (65533)      706 2021-02-02 20:57:45.000000 firex_flame-2.5.9/firex_flame.egg-info/SOURCES.txt
+-rw-r--r--   0 firex      (100) nogroup  (65533)        1 2021-02-02 20:57:45.000000 firex_flame-2.5.9/firex_flame.egg-info/dependency_links.txt
+-rw-r--r--   0 firex      (100) nogroup  (65533)      195 2021-02-02 20:57:45.000000 firex_flame-2.5.9/firex_flame.egg-info/entry_points.txt
+-rw-r--r--   0 firex      (100) nogroup  (65533)      239 2021-02-02 20:57:45.000000 firex_flame-2.5.9/firex_flame.egg-info/requires.txt
+-rw-r--r--   0 firex      (100) nogroup  (65533)       12 2021-02-02 20:57:45.000000 firex_flame-2.5.9/firex_flame.egg-info/top_level.txt
+-rw-r--r--   0 firex      (100) nogroup  (65533)        1 2021-02-02 20:57:45.000000 firex_flame-2.5.9/firex_flame.egg-info/zip-safe
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)      276 2021-02-02 20:57:45.000000 firex_flame-2.5.9/setup.cfg
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)     1832 2021-02-02 20:57:32.000000 firex_flame-2.5.9/setup.py
+-rw-rw-rw-   0 firex      (100) nogroup  (65533)    70144 2021-02-02 20:57:32.000000 firex_flame-2.5.9/versioneer.py
```

### Comparing `firex_flame-2.5.8/LICENSE` & `firex_flame-2.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `firex_flame-2.5.8/README.md` & `firex_flame-2.5.9/README.md`

 * *Files identical despite different names*

### Comparing `firex_flame-2.5.8/fastentrypoints.py` & `firex_flame-2.5.9/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.5.8/firex_flame/__main__.py` & `firex_flame-2.5.9/firex_flame/__main__.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.5.8/firex_flame/api.py` & `firex_flame-2.5.9/firex_flame/api.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.5.8/firex_flame/controller.py` & `firex_flame-2.5.9/firex_flame/controller.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.5.8/firex_flame/event_aggregator.py` & `firex_flame-2.5.9/firex_flame/event_aggregator.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.5.8/firex_flame/event_broker_processor.py` & `firex_flame-2.5.9/firex_flame/event_broker_processor.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.5.8/firex_flame/event_file_processor.py` & `firex_flame-2.5.9/firex_flame/event_file_processor.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.5.8/firex_flame/flame_helper.py` & `firex_flame-2.5.9/firex_flame/flame_helper.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.5.8/firex_flame/launcher.py` & `firex_flame-2.5.9/firex_flame/launcher.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.5.8/firex_flame/main_app.py` & `firex_flame-2.5.9/firex_flame/main_app.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.5.8/firex_flame/model_dumper.py` & `firex_flame-2.5.9/firex_flame/model_dumper.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.5.8/firex_flame/templates/index.html` & `firex_flame-2.5.9/firex_flame/templates/index.html`

 * *Files identical despite different names*

### Comparing `firex_flame-2.5.8/firex_flame/web_app.py` & `firex_flame-2.5.9/firex_flame/web_app.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.5.8/firex_flame.egg-info/SOURCES.txt` & `firex_flame-2.5.9/firex_flame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firex_flame-2.5.8/setup.py` & `firex_flame-2.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.5.8/versioneer.py` & `firex_flame-2.5.9/versioneer.py`

 * *Files identical despite different names*

