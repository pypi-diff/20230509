# Comparing `tmp/fp_browser_sdk-0.9.tar.gz` & `tmp/fp_browser_sdk-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fp_browser_sdk-0.9.tar", last modified: Mon May  8 07:10:10 2023, max compression
+gzip compressed data, was "dist/fp_browser_sdk-0.9.1.tar", last modified: Tue May  9 07:30:21 2023, max compression
```

## Comparing `fp_browser_sdk-0.9.tar` & `fp_browser_sdk-0.9.1.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/
--rw-r--r--   0 leeyang    (501) staff       (20)      262 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/PKG-INFO
--rw-r--r--   0 leeyang    (501) staff       (20)     8453 2023-02-12 04:55:25.000000 fp_browser_sdk-0.9/README.md
-drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/fp_browser_sdk/
--rw-r--r--   0 leeyang    (501) staff       (20)    15571 2022-12-15 04:40:42.000000 fp_browser_sdk-0.9/fp_browser_sdk/__init__.py
-drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/fp_browser_sdk/data/
--rw-r--r--   0 leeyang    (501) staff       (20)        0 2022-08-05 08:21:32.000000 fp_browser_sdk-0.9/fp_browser_sdk/data/__init__.py
--rw-r--r--   0 leeyang    (501) staff       (20)   183083 2022-08-16 02:45:13.000000 fp_browser_sdk-0.9/fp_browser_sdk/data/motion.py
-drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/
--rw-r--r--   0 leeyang    (501) staff       (20)        0 2022-08-05 08:21:32.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/__init__.py
--rw-r--r--   0 leeyang    (501) staff       (20)     6386 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/basic.py
--rw-r--r--   0 leeyang    (501) staff       (20)     3212 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/battery.py
--rw-r--r--   0 leeyang    (501) staff       (20)    17258 2023-04-07 07:59:18.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/browser_enum.py
--rw-r--r--   0 leeyang    (501) staff       (20)     3357 2023-03-13 13:15:24.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/client_hints.py
--rw-r--r--   0 leeyang    (501) staff       (20)     5336 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/device_motion.py
--rw-r--r--   0 leeyang    (501) staff       (20)     2059 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/device_orientation.py
--rw-r--r--   0 leeyang    (501) staff       (20)     7142 2023-01-15 06:50:48.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/document.py
--rw-r--r--   0 leeyang    (501) staff       (20)      451 2022-08-07 03:58:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/exception.py
--rw-r--r--   0 leeyang    (501) staff       (20)     3291 2023-04-10 11:49:02.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/fingerprint_offset.py
--rw-r--r--   0 leeyang    (501) staff       (20)     1851 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/geo.py
--rw-r--r--   0 leeyang    (501) staff       (20)     3266 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/header.py
--rw-r--r--   0 leeyang    (501) staff       (20)      465 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/inject_js.py
--rw-r--r--   0 leeyang    (501) staff       (20)     2223 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/media.py
--rw-r--r--   0 leeyang    (501) staff       (20)     2539 2022-08-05 07:15:01.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/module.py
--rw-r--r--   0 leeyang    (501) staff       (20)     6966 2023-05-08 07:08:22.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/navigator.py
--rw-r--r--   0 leeyang    (501) staff       (20)     3917 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/network.py
--rw-r--r--   0 leeyang    (501) staff       (20)     9140 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/performance.py
-drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/
--rw-r--r--   0 leeyang    (501) staff       (20)      294 2022-09-18 13:15:09.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/__init__.py
--rw-r--r--   0 leeyang    (501) staff       (20)    13786 2022-12-17 12:48:42.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type.py
--rw-r--r--   0 leeyang    (501) staff       (20)    12917 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_102.py
--rw-r--r--   0 leeyang    (501) staff       (20)    12683 2022-12-17 12:48:42.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_107.py
--rw-r--r--   0 leeyang    (501) staff       (20)     9857 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_88.py
--rw-r--r--   0 leeyang    (501) staff       (20)    10280 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_90.py
--rw-r--r--   0 leeyang    (501) staff       (20)    11710 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_93.py
--rw-r--r--   0 leeyang    (501) staff       (20)     1049 2022-12-17 12:48:42.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/util.py
--rw-r--r--   0 leeyang    (501) staff       (20)     2087 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/plugin.py
--rw-r--r--   0 leeyang    (501) staff       (20)     3923 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/screen.py
--rw-r--r--   0 leeyang    (501) staff       (20)     2343 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/speech_synthesis_voice.py
--rw-r--r--   0 leeyang    (501) staff       (20)     1678 2023-02-12 04:54:23.000000 fp_browser_sdk-0.9/fp_browser_sdk/ext/webrtc.py
--rw-r--r--   0 leeyang    (501) staff       (20)      471 2022-11-11 04:36:45.000000 fp_browser_sdk-0.9/fp_browser_sdk/fp_browser_settings.py
-drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/fp_browser_sdk.egg-info/
--rw-r--r--   0 leeyang    (501) staff       (20)      262 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/fp_browser_sdk.egg-info/PKG-INFO
--rw-r--r--   0 leeyang    (501) staff       (20)     1448 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/fp_browser_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 leeyang    (501) staff       (20)        1 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/fp_browser_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 leeyang    (501) staff       (20)       15 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/fp_browser_sdk.egg-info/top_level.txt
--rw-r--r--   0 leeyang    (501) staff       (20)       38 2023-05-08 07:10:10.000000 fp_browser_sdk-0.9/setup.cfg
--rw-r--r--   0 leeyang    (501) staff       (20)      385 2023-05-08 07:10:04.000000 fp_browser_sdk-0.9/setup.py
+drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/
+-rw-r--r--   0 leeyang    (501) staff       (20)      264 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/PKG-INFO
+-rw-r--r--   0 leeyang    (501) staff       (20)     8453 2023-02-12 04:55:25.000000 fp_browser_sdk-0.9.1/README.md
+drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/
+-rw-r--r--   0 leeyang    (501) staff       (20)    15571 2022-12-15 04:40:42.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/__init__.py
+drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/data/
+-rw-r--r--   0 leeyang    (501) staff       (20)        0 2022-08-05 08:21:32.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/data/__init__.py
+-rw-r--r--   0 leeyang    (501) staff       (20)   183083 2022-08-16 02:45:13.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/data/motion.py
+drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/
+-rw-r--r--   0 leeyang    (501) staff       (20)        0 2022-08-05 08:21:32.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/__init__.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     6386 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/basic.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     3212 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/battery.py
+-rw-r--r--   0 leeyang    (501) staff       (20)    17258 2023-04-07 07:59:18.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/browser_enum.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     3357 2023-03-13 13:15:24.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/client_hints.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     5336 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/device_motion.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     2059 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/device_orientation.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     7142 2023-01-15 06:50:48.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/document.py
+-rw-r--r--   0 leeyang    (501) staff       (20)      451 2022-08-07 03:58:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/exception.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     3291 2023-04-10 11:49:02.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/fingerprint_offset.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     1851 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/geo.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     1328 2023-05-09 07:29:43.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/gl.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     3266 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/header.py
+-rw-r--r--   0 leeyang    (501) staff       (20)      465 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/inject_js.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     2223 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/media.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     2539 2022-08-05 07:15:01.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/module.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     6966 2023-05-08 07:08:22.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/navigator.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     3917 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/network.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     9140 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/performance.py
+drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/
+-rw-r--r--   0 leeyang    (501) staff       (20)      294 2022-09-18 13:15:09.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/__init__.py
+-rw-r--r--   0 leeyang    (501) staff       (20)    13786 2022-12-17 12:48:42.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type.py
+-rw-r--r--   0 leeyang    (501) staff       (20)    12917 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_102.py
+-rw-r--r--   0 leeyang    (501) staff       (20)    12683 2022-12-17 12:48:42.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_107.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     9857 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_88.py
+-rw-r--r--   0 leeyang    (501) staff       (20)    10280 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_90.py
+-rw-r--r--   0 leeyang    (501) staff       (20)    11710 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_93.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     1049 2022-12-17 12:48:42.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/util.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     2087 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/plugin.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     3923 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/screen.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     2343 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/speech_synthesis_voice.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     1678 2023-02-12 04:54:23.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/webrtc.py
+-rw-r--r--   0 leeyang    (501) staff       (20)      471 2022-11-11 04:36:45.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/fp_browser_settings.py
+drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/fp_browser_sdk.egg-info/
+-rw-r--r--   0 leeyang    (501) staff       (20)      264 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/fp_browser_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 leeyang    (501) staff       (20)     1473 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/fp_browser_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 leeyang    (501) staff       (20)        1 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/fp_browser_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 leeyang    (501) staff       (20)       15 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/fp_browser_sdk.egg-info/top_level.txt
+-rw-r--r--   0 leeyang    (501) staff       (20)       38 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/setup.cfg
+-rw-r--r--   0 leeyang    (501) staff       (20)      387 2023-05-09 07:30:11.000000 fp_browser_sdk-0.9.1/setup.py
```

### Comparing `fp_browser_sdk-0.9/README.md` & `fp_browser_sdk-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/__init__.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/data/motion.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/data/motion.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/basic.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/basic.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/battery.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/battery.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/browser_enum.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/browser_enum.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/client_hints.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/client_hints.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/device_motion.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/device_motion.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/device_orientation.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/device_orientation.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/document.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/document.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/fingerprint_offset.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/fingerprint_offset.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/geo.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/geo.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/header.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/header.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/media.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/media.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/module.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/module.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/navigator.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/navigator.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/network.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/network.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/performance.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/performance.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_102.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_102.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_107.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_107.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_88.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_88.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_90.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_90.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/permission_type_93.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_93.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/permission_types/util.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/util.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/plugin.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/plugin.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/screen.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/screen.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/speech_synthesis_voice.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/speech_synthesis_voice.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk/ext/webrtc.py` & `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/webrtc.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9/fp_browser_sdk.egg-info/SOURCES.txt` & `fp_browser_sdk-0.9.1/fp_browser_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 fp_browser_sdk/ext/client_hints.py
 fp_browser_sdk/ext/device_motion.py
 fp_browser_sdk/ext/device_orientation.py
 fp_browser_sdk/ext/document.py
 fp_browser_sdk/ext/exception.py
 fp_browser_sdk/ext/fingerprint_offset.py
 fp_browser_sdk/ext/geo.py
+fp_browser_sdk/ext/gl.py
 fp_browser_sdk/ext/header.py
 fp_browser_sdk/ext/inject_js.py
 fp_browser_sdk/ext/media.py
 fp_browser_sdk/ext/module.py
 fp_browser_sdk/ext/navigator.py
 fp_browser_sdk/ext/network.py
 fp_browser_sdk/ext/performance.py
```

