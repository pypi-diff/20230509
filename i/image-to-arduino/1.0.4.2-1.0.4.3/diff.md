# Comparing `tmp/image-to-arduino-1.0.4.2.tar.gz` & `tmp/image-to-arduino-1.0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-to-arduino-1.0.4.2.tar", last modified: Tue May  9 16:03:21 2023, max compression
+gzip compressed data, was "image-to-arduino-1.0.4.3.tar", last modified: Tue May  9 16:11:27 2023, max compression
```

## Comparing `image-to-arduino-1.0.4.2.tar` & `image-to-arduino-1.0.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-09 16:03:21.614620 image-to-arduino-1.0.4.2/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.2/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.2/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-09 16:03:21.614620 image-to-arduino-1.0.4.2/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2324 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.2/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-09 16:03:21.614620 image-to-arduino-1.0.4.2/image_to_arduino.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-09 16:03:21.000000 image-to-arduino-1.0.4.2/image_to_arduino.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      374 2023-05-09 16:03:21.000000 image-to-arduino-1.0.4.2/image_to_arduino.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-09 16:03:21.000000 image-to-arduino-1.0.4.2/image_to_arduino.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       66 2023-05-09 16:03:21.000000 image-to-arduino-1.0.4.2/image_to_arduino.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-05-09 16:03:21.000000 image-to-arduino-1.0.4.2/image_to_arduino.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       15 2023-05-09 16:03:21.000000 image-to-arduino-1.0.4.2/image_to_arduino.egg-info/top_level.txt
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-09 16:03:21.614620 image-to-arduino-1.0.4.2/imagetoarduino/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.2/imagetoarduino/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       61 2023-05-09 15:55:50.000000 image-to-arduino-1.0.4.2/imagetoarduino/__main__.py
--rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     8265 2023-05-09 15:59:47.000000 image-to-arduino-1.0.4.2/imagetoarduino/main.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       77 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.2/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-09 16:03:21.614620 image-to-arduino-1.0.4.2/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1183 2023-05-09 16:02:25.000000 image-to-arduino-1.0.4.2/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-09 16:11:27.473312 image-to-arduino-1.0.4.3/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.3/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.3/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-09 16:11:27.473312 image-to-arduino-1.0.4.3/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2324 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.3/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-09 16:11:27.473312 image-to-arduino-1.0.4.3/image_to_arduino/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.3/image_to_arduino/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       78 2023-05-09 16:10:50.000000 image-to-arduino-1.0.4.3/image_to_arduino/__main__.py
+-rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     8265 2023-05-09 15:59:47.000000 image-to-arduino-1.0.4.3/image_to_arduino/main.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-09 16:11:27.473312 image-to-arduino-1.0.4.3/image_to_arduino.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-09 16:11:27.000000 image-to-arduino-1.0.4.3/image_to_arduino.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      380 2023-05-09 16:11:27.000000 image-to-arduino-1.0.4.3/image_to_arduino.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-09 16:11:27.000000 image-to-arduino-1.0.4.3/image_to_arduino.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       68 2023-05-09 16:11:27.000000 image-to-arduino-1.0.4.3/image_to_arduino.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-05-09 16:11:27.000000 image-to-arduino-1.0.4.3/image_to_arduino.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       17 2023-05-09 16:11:27.000000 image-to-arduino-1.0.4.3/image_to_arduino.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       77 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.3/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-09 16:11:27.473312 image-to-arduino-1.0.4.3/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      972 2023-05-09 16:10:00.000000 image-to-arduino-1.0.4.3/setup.py
```

### Comparing `image-to-arduino-1.0.4.2/LICENSE` & `image-to-arduino-1.0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `image-to-arduino-1.0.4.2/README.md` & `image-to-arduino-1.0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `image-to-arduino-1.0.4.2/imagetoarduino/main.py` & `image-to-arduino-1.0.4.3/image_to_arduino/main.py`

 * *Files identical despite different names*

