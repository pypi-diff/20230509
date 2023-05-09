# Comparing `tmp/nudeny-0.0.7.tar.gz` & `tmp/nudeny-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nudeny-0.0.7.tar", max compression
+gzip compressed data, was "nudeny-0.0.8.tar", max compression
```

## Comparing `nudeny-0.0.7.tar` & `nudeny-0.0.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1091 2023-03-25 16:00:24.478955 nudeny-0.0.7/LICENSE
--rw-r--r--   0        0        0      527 2023-04-24 14:14:26.977299 nudeny-0.0.7/pyproject.toml
--rw-r--r--   0        0        0       36 2023-03-25 16:00:24.478955 nudeny-0.0.7/src/nudeny/__init__.py
--rw-r--r--   0        0        0     5281 2023-04-24 14:11:42.740289 nudeny-0.0.7/src/nudeny/nudeny.py
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 nudeny-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-03-25 16:00:24.478955 nudeny-0.0.8/LICENSE
+-rw-r--r--   0        0        0      527 2023-04-24 14:48:15.180980 nudeny-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-03-25 16:00:24.478955 nudeny-0.0.8/src/nudeny/__init__.py
+-rw-r--r--   0        0        0     5377 2023-04-24 14:48:42.099182 nudeny-0.0.8/src/nudeny/nudeny.py
+-rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 nudeny-0.0.8/PKG-INFO
```

### Comparing `nudeny-0.0.7/LICENSE` & `nudeny-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nudeny-0.0.7/pyproject.toml` & `nudeny-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Nudeny"
-version = "0.0.7"
+version = "0.0.8"
 description = "Image nudity classification and detection package."
 authors = ["Nudeny <thesis.nudeny69@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/Nudeny/Nudeny-python-module"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `nudeny-0.0.7/src/nudeny/nudeny.py` & `nudeny-0.0.8/src/nudeny/nudeny.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,16 @@
             url=self.URL+"classify-url/", json=json).json()
 
         return response
 
 class Detect:
 
     def __init__(self):
-        self.URL = "http://127.0.0.1:8000/"
+        self.LOCALHOST_URL = "http://127.0.0.1:8000/"
+        self.URL = "http://ec2-18-136-200-224.ap-southeast-1.compute.amazonaws.com/"
     
     def save_to_path(self, prediction, save_path):
         """
         Downloads image url and saves it to the save path provided.
 
         Args:
             prediction (dict): List of Image URL or data URI
```

### Comparing `nudeny-0.0.7/PKG-INFO` & `nudeny-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nudeny
-Version: 0.0.7
+Version: 0.0.8
 Summary: Image nudity classification and detection package.
 Home-page: https://github.com/Nudeny/Nudeny-python-module
 License: MIT
 Author: Nudeny
 Author-email: thesis.nudeny69@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

