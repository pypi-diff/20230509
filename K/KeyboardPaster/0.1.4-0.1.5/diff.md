# Comparing `tmp/KeyboardPaster-0.1.4.tar.gz` & `tmp/KeyboardPaster-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KeyboardPaster-0.1.4.tar", last modified: Tue May  9 09:41:04 2023, max compression
+gzip compressed data, was "KeyboardPaster-0.1.5.tar", last modified: Tue May  9 11:21:57 2023, max compression
```

## Comparing `KeyboardPaster-0.1.4.tar` & `KeyboardPaster-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 09:41:04.942674 KeyboardPaster-0.1.4/
-drwxrwxrwx   0        0        0        0 2023-05-09 09:41:04.935168 KeyboardPaster-0.1.4/KeyboardPaster.egg-info/
--rw-rw-rw-   0        0        0     1040 2023-05-09 09:41:04.000000 KeyboardPaster-0.1.4/KeyboardPaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-05-09 09:41:04.000000 KeyboardPaster-0.1.4/KeyboardPaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 09:41:04.000000 KeyboardPaster-0.1.4/KeyboardPaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-09 09:41:04.000000 KeyboardPaster-0.1.4/KeyboardPaster.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       80 2023-05-09 09:41:04.000000 KeyboardPaster-0.1.4/KeyboardPaster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-09 09:41:04.000000 KeyboardPaster-0.1.4/KeyboardPaster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1040 2023-05-09 09:41:04.941674 KeyboardPaster-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-05-09 09:19:34.000000 KeyboardPaster-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 09:41:04.940172 KeyboardPaster-0.1.4/keyboardpaster/
--rw-rw-rw-   0        0        0        0 2023-05-09 08:14:31.000000 KeyboardPaster-0.1.4/keyboardpaster/__init__.py
--rw-rw-rw-   0        0        0     3407 2023-05-09 09:40:40.000000 KeyboardPaster-0.1.4/keyboardpaster/app.py
--rw-rw-rw-   0        0        0     2737 2023-05-09 09:15:39.000000 KeyboardPaster-0.1.4/keyboardpaster/keyboard_layout_detector.py
--rw-rw-rw-   0        0        0       42 2023-05-09 09:41:04.942674 KeyboardPaster-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1333 2023-05-09 09:40:50.000000 KeyboardPaster-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 11:21:57.465831 KeyboardPaster-0.1.5/
+drwxrwxrwx   0        0        0        0 2023-05-09 11:21:57.457325 KeyboardPaster-0.1.5/KeyboardPaster.egg-info/
+-rw-rw-rw-   0        0        0     1040 2023-05-09 11:21:57.000000 KeyboardPaster-0.1.5/KeyboardPaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-05-09 11:21:57.000000 KeyboardPaster-0.1.5/KeyboardPaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 11:21:57.000000 KeyboardPaster-0.1.5/KeyboardPaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-09 11:21:57.000000 KeyboardPaster-0.1.5/KeyboardPaster.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       80 2023-05-09 11:21:57.000000 KeyboardPaster-0.1.5/KeyboardPaster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-09 11:21:57.000000 KeyboardPaster-0.1.5/KeyboardPaster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1040 2023-05-09 11:21:57.465332 KeyboardPaster-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-09 09:19:34.000000 KeyboardPaster-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 11:21:57.463330 KeyboardPaster-0.1.5/keyboardpaster/
+-rw-rw-rw-   0        0        0        0 2023-05-09 08:14:31.000000 KeyboardPaster-0.1.5/keyboardpaster/__init__.py
+-rw-rw-rw-   0        0        0     3485 2023-05-09 11:08:22.000000 KeyboardPaster-0.1.5/keyboardpaster/app.py
+-rw-rw-rw-   0        0        0    10577 2023-05-09 10:59:43.000000 KeyboardPaster-0.1.5/keyboardpaster/keyboard_layout_detector.py
+-rw-rw-rw-   0        0        0      552 2023-05-09 08:59:34.000000 KeyboardPaster-0.1.5/keyboardpaster/keyboardpaster.kv
+-rw-rw-rw-   0        0        0       42 2023-05-09 11:21:57.465831 KeyboardPaster-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1411 2023-05-09 11:20:04.000000 KeyboardPaster-0.1.5/setup.py
```

### Comparing `KeyboardPaster-0.1.4/KeyboardPaster.egg-info/PKG-INFO` & `KeyboardPaster-0.1.5/KeyboardPaster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyboardPaster
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package to type text using the keyboard module
 Home-page: https://github.com/KnutssonDevelopment/KeyboardPaster
 Author: Brian Knutsson
 Author-email: development@knutsson.it
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `KeyboardPaster-0.1.4/PKG-INFO` & `KeyboardPaster-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyboardPaster
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package to type text using the keyboard module
 Home-page: https://github.com/KnutssonDevelopment/KeyboardPaster
 Author: Brian Knutsson
 Author-email: development@knutsson.it
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `KeyboardPaster-0.1.4/keyboardpaster/app.py` & `KeyboardPaster-0.1.5/keyboardpaster/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import os
 import time
+import re
 import keyboard
 from kivy.app import App
-from kivy.uix.boxlayout import BoxLayout
+import pkg_resources
 from kivy.lang import Builder
 from keyboardpaster.keyboard_layout_detector import get_keyboard_layout
 
 SPECIAL_CHARS_SHIFT = {
     'EN_US': {
         '~': '`', '!': '1', '@': '2', '#': '3', '$': '4',
         '%': '5', '^': '6', '&': '7', '*': '8', '(': '9',
@@ -64,27 +66,28 @@
 
 
 class KeyboardPasterApp(App):
     layout = 'EN_US'
 
     def build(self):
         self.detect_keyboard_layout()
-        return Builder.load_file("keyboardpaster/keyboardpaster.kv")
+        kv_file_path = pkg_resources.resource_filename(__name__, "keyboardpaster.kv")
+        return Builder.load_file(kv_file_path)
 
     def paste_text(self):
         text_to_paste = self.root.ids.input_text.text
         type_string_with_delay(text_to_paste, layout=self.layout)
 
     def set_layout(self, layout):
         self.layout = layout
 
     def detect_keyboard_layout(self):
         layout_code = get_keyboard_layout()
 
-        if layout_code.startswith('da'):  # Danish layout
+        if bool(re.match('da', layout_code, re.I)):  # Danish layout
             self.layout = 'DA_DK'
         else:  # Default to English (US) layout
             self.layout = 'EN_US'
 
 
 def main():
     KeyboardPasterApp().run()
```

