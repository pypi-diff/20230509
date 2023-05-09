# Comparing `tmp/KeyboardPaster-0.1.2.tar.gz` & `tmp/KeyboardPaster-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KeyboardPaster-0.1.2.tar", last modified: Tue May  9 09:36:28 2023, max compression
+gzip compressed data, was "KeyboardPaster-0.1.3.tar", last modified: Tue May  9 09:39:42 2023, max compression
```

## Comparing `KeyboardPaster-0.1.2.tar` & `KeyboardPaster-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 09:36:28.884662 KeyboardPaster-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-05-09 09:36:28.878157 KeyboardPaster-0.1.2/KeyboardPaster.egg-info/
--rw-rw-rw-   0        0        0     1040 2023-05-09 09:36:28.000000 KeyboardPaster-0.1.2/KeyboardPaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-05-09 09:36:28.000000 KeyboardPaster-0.1.2/KeyboardPaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 09:36:28.000000 KeyboardPaster-0.1.2/KeyboardPaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-09 09:36:28.000000 KeyboardPaster-0.1.2/KeyboardPaster.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       80 2023-05-09 09:36:28.000000 KeyboardPaster-0.1.2/KeyboardPaster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-09 09:36:28.000000 KeyboardPaster-0.1.2/KeyboardPaster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1040 2023-05-09 09:36:28.884161 KeyboardPaster-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-05-09 09:19:34.000000 KeyboardPaster-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 09:36:28.882660 KeyboardPaster-0.1.2/keyboardpaster/
--rw-rw-rw-   0        0        0        0 2023-05-09 08:14:31.000000 KeyboardPaster-0.1.2/keyboardpaster/__init__.py
--rw-rw-rw-   0        0        0     3392 2023-05-09 09:36:00.000000 KeyboardPaster-0.1.2/keyboardpaster/app.py
--rw-rw-rw-   0        0        0     2737 2023-05-09 09:15:39.000000 KeyboardPaster-0.1.2/keyboardpaster/keyboard_layout_detector.py
--rw-rw-rw-   0        0        0       42 2023-05-09 09:36:28.885162 KeyboardPaster-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1333 2023-05-09 09:36:13.000000 KeyboardPaster-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:39:42.965697 KeyboardPaster-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-05-09 09:39:42.958191 KeyboardPaster-0.1.3/KeyboardPaster.egg-info/
+-rw-rw-rw-   0        0        0     1040 2023-05-09 09:39:42.000000 KeyboardPaster-0.1.3/KeyboardPaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-05-09 09:39:42.000000 KeyboardPaster-0.1.3/KeyboardPaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 09:39:42.000000 KeyboardPaster-0.1.3/KeyboardPaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-09 09:39:42.000000 KeyboardPaster-0.1.3/KeyboardPaster.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       80 2023-05-09 09:39:42.000000 KeyboardPaster-0.1.3/KeyboardPaster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-09 09:39:42.000000 KeyboardPaster-0.1.3/KeyboardPaster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1040 2023-05-09 09:39:42.964696 KeyboardPaster-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-09 09:19:34.000000 KeyboardPaster-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 09:39:42.963194 KeyboardPaster-0.1.3/keyboardpaster/
+-rw-rw-rw-   0        0        0        0 2023-05-09 08:14:31.000000 KeyboardPaster-0.1.3/keyboardpaster/__init__.py
+-rw-rw-rw-   0        0        0     3407 2023-05-09 09:37:52.000000 KeyboardPaster-0.1.3/keyboardpaster/app.py
+-rw-rw-rw-   0        0        0     2737 2023-05-09 09:15:39.000000 KeyboardPaster-0.1.3/keyboardpaster/keyboard_layout_detector.py
+-rw-rw-rw-   0        0        0       42 2023-05-09 09:39:42.965697 KeyboardPaster-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1333 2023-05-09 09:39:16.000000 KeyboardPaster-0.1.3/setup.py
```

### Comparing `KeyboardPaster-0.1.2/KeyboardPaster.egg-info/PKG-INFO` & `KeyboardPaster-0.1.3/KeyboardPaster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyboardPaster
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package to type text using the keyboard module
 Home-page: https://github.com/KnutssonDevelopment/KeyboardPaster
 Author: Brian Knutsson
 Author-email: development@knutsson.it
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `KeyboardPaster-0.1.2/PKG-INFO` & `KeyboardPaster-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyboardPaster
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package to type text using the keyboard module
 Home-page: https://github.com/KnutssonDevelopment/KeyboardPaster
 Author: Brian Knutsson
 Author-email: development@knutsson.it
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `KeyboardPaster-0.1.2/keyboardpaster/app.py` & `KeyboardPaster-0.1.3/keyboardpaster/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 
 class KeyboardPasterApp(App):
     layout = 'EN_US'
 
     def build(self):
         self.detect_keyboard_layout()
-        return Builder.load_file("keyboardpaster.kv")
+        return Builder.load_file("KeyboardPaster/keyboardpaster.kv")
 
     def paste_text(self):
         text_to_paste = self.root.ids.input_text.text
         type_string_with_delay(text_to_paste, layout=self.layout)
 
     def set_layout(self, layout):
         self.layout = layout
```

### Comparing `KeyboardPaster-0.1.2/keyboardpaster/keyboard_layout_detector.py` & `KeyboardPaster-0.1.3/keyboardpaster/keyboard_layout_detector.py`

 * *Files identical despite different names*

### Comparing `KeyboardPaster-0.1.2/setup.py` & `KeyboardPaster-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="KeyboardPaster",
-    version="0.1.2",
+    version="0.1.3",
     author="Brian Knutsson",
     author_email="development@knutsson.it",
     description="A Python package to type text using the keyboard module",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KnutssonDevelopment/KeyboardPaster",
     packages=find_packages(),
```

