# Comparing `tmp/KeyboardPaster-0.1.0.tar.gz` & `tmp/KeyboardPaster-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KeyboardPaster-0.1.0.tar", last modified: Tue May  9 09:20:38 2023, max compression
+gzip compressed data, was "KeyboardPaster-0.1.1.tar", last modified: Tue May  9 09:32:11 2023, max compression
```

## Comparing `KeyboardPaster-0.1.0.tar` & `KeyboardPaster-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 09:20:38.100080 KeyboardPaster-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-05-09 09:20:38.093074 KeyboardPaster-0.1.0/KeyboardPaster.egg-info/
--rw-rw-rw-   0        0        0     1040 2023-05-09 09:20:37.000000 KeyboardPaster-0.1.0/KeyboardPaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-05-09 09:20:38.000000 KeyboardPaster-0.1.0/KeyboardPaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 09:20:37.000000 KeyboardPaster-0.1.0/KeyboardPaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-09 09:20:38.000000 KeyboardPaster-0.1.0/KeyboardPaster.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       80 2023-05-09 09:20:38.000000 KeyboardPaster-0.1.0/KeyboardPaster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-09 09:20:38.000000 KeyboardPaster-0.1.0/KeyboardPaster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1040 2023-05-09 09:20:38.099580 KeyboardPaster-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-05-09 09:19:34.000000 KeyboardPaster-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 09:20:38.097578 KeyboardPaster-0.1.0/keyboardpaster/
--rw-rw-rw-   0        0        0        0 2023-05-09 08:14:31.000000 KeyboardPaster-0.1.0/keyboardpaster/__init__.py
--rw-rw-rw-   0        0        0     3348 2023-05-09 09:00:18.000000 KeyboardPaster-0.1.0/keyboardpaster/app.py
--rw-rw-rw-   0        0        0     2737 2023-05-09 09:15:39.000000 KeyboardPaster-0.1.0/keyboardpaster/keyboard_layout_detector.py
--rw-rw-rw-   0        0        0       42 2023-05-09 09:20:38.100080 KeyboardPaster-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1333 2023-05-09 09:09:55.000000 KeyboardPaster-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:32:11.058460 KeyboardPaster-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-05-09 09:32:11.050955 KeyboardPaster-0.1.1/KeyboardPaster.egg-info/
+-rw-rw-rw-   0        0        0     1040 2023-05-09 09:32:10.000000 KeyboardPaster-0.1.1/KeyboardPaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-05-09 09:32:10.000000 KeyboardPaster-0.1.1/KeyboardPaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 09:32:10.000000 KeyboardPaster-0.1.1/KeyboardPaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-09 09:32:10.000000 KeyboardPaster-0.1.1/KeyboardPaster.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       80 2023-05-09 09:32:10.000000 KeyboardPaster-0.1.1/KeyboardPaster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-09 09:32:10.000000 KeyboardPaster-0.1.1/KeyboardPaster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1040 2023-05-09 09:32:11.057460 KeyboardPaster-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-09 09:19:34.000000 KeyboardPaster-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 09:32:11.055959 KeyboardPaster-0.1.1/keyboardpaster/
+-rw-rw-rw-   0        0        0        0 2023-05-09 08:14:31.000000 KeyboardPaster-0.1.1/keyboardpaster/__init__.py
+-rw-rw-rw-   0        0        0     3363 2023-05-09 09:29:24.000000 KeyboardPaster-0.1.1/keyboardpaster/app.py
+-rw-rw-rw-   0        0        0     2737 2023-05-09 09:15:39.000000 KeyboardPaster-0.1.1/keyboardpaster/keyboard_layout_detector.py
+-rw-rw-rw-   0        0        0       42 2023-05-09 09:32:11.058460 KeyboardPaster-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1333 2023-05-09 09:32:01.000000 KeyboardPaster-0.1.1/setup.py
```

### Comparing `KeyboardPaster-0.1.0/KeyboardPaster.egg-info/PKG-INFO` & `KeyboardPaster-0.1.1/KeyboardPaster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyboardPaster
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package to type text using the keyboard module
 Home-page: https://github.com/KnutssonDevelopment/KeyboardPaster
 Author: Brian Knutsson
 Author-email: development@knutsson.it
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `KeyboardPaster-0.1.0/PKG-INFO` & `KeyboardPaster-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyboardPaster
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package to type text using the keyboard module
 Home-page: https://github.com/KnutssonDevelopment/KeyboardPaster
 Author: Brian Knutsson
 Author-email: development@knutsson.it
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `KeyboardPaster-0.1.0/keyboardpaster/app.py` & `KeyboardPaster-0.1.1/keyboardpaster/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 import keyboard
 from kivy.app import App
 from kivy.uix.boxlayout import BoxLayout
 from kivy.lang import Builder
-from keyboard_layout_detector import get_keyboard_layout
+from keyboardpaster.keyboard_layout_detector import get_keyboard_layout
 
 SPECIAL_CHARS_SHIFT = {
     'EN_US': {
         '~': '`', '!': '1', '@': '2', '#': '3', '$': '4',
         '%': '5', '^': '6', '&': '7', '*': '8', '(': '9',
         ')': '0', '_': '-', '+': '=', '{': '[', '}': ']',
         '|': '\\', ':': ';', '"': "'", '<': ',', '>': '.',
```

### Comparing `KeyboardPaster-0.1.0/keyboardpaster/keyboard_layout_detector.py` & `KeyboardPaster-0.1.1/keyboardpaster/keyboard_layout_detector.py`

 * *Files identical despite different names*

### Comparing `KeyboardPaster-0.1.0/setup.py` & `KeyboardPaster-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="KeyboardPaster",
-    version="0.1.0",
+    version="0.1.1",
     author="Brian Knutsson",
     author_email="development@knutsson.it",
     description="A Python package to type text using the keyboard module",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KnutssonDevelopment/KeyboardPaster",
     packages=find_packages(),
```

