# Comparing `tmp/kalm-0.4.4.tar.gz` & `tmp/kalm-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.4.4.tar", max compression
+gzip compressed data, was "kalm-0.4.5.tar", max compression
```

## Comparing `kalm-0.4.4.tar` & `kalm-0.4.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1081 2023-05-05 20:49:24.880279 kalm-0.4.4/LICENSE.txt
--rw-r--r--   0        0        0     1832 2023-05-08 13:35:45.619909 kalm-0.4.4/pyproject.toml
--rw-r--r--   0        0        0    10663 2023-05-08 13:34:59.939641 kalm-0.4.4/src/kalm/__init__.py
--rw-r--r--   0        0        0    32308 2023-05-08 13:21:45.550993 kalm-0.4.4/src/kalm/kalm.py
--rw-r--r--   0        0        0     6484 2023-05-05 20:49:24.884279 kalm-0.4.4/src/kalm/kalm_api.py
--rw-r--r--   0        0        0     1296 2023-05-05 20:49:24.884279 kalm-0.4.4/src/kalm/netbox.py
--rw-r--r--   0        0        0        9 2023-05-05 20:49:24.884279 kalm-0.4.4/src/kalm/package_data.dat
--rw-r--r--   0        0        0      312 2023-05-05 20:49:24.884279 kalm-0.4.4/src/kalm/toolbox.py
--rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 kalm-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-05 20:49:24.880279 kalm-0.4.5/LICENSE.txt
+-rw-r--r--   0        0        0     1862 2023-05-09 12:16:22.471829 kalm-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0    10663 2023-05-08 13:34:59.939641 kalm-0.4.5/src/kalm/__init__.py
+-rw-r--r--   0        0        0    32308 2023-05-08 13:21:45.550993 kalm-0.4.5/src/kalm/kalm.py
+-rw-r--r--   0        0        0     6484 2023-05-05 20:49:24.884279 kalm-0.4.5/src/kalm/kalm_api.py
+-rw-r--r--   0        0        0     1296 2023-05-05 20:49:24.884279 kalm-0.4.5/src/kalm/netbox.py
+-rw-r--r--   0        0        0        9 2023-05-05 20:49:24.884279 kalm-0.4.5/src/kalm/package_data.dat
+-rw-r--r--   0        0        0      312 2023-05-05 20:49:24.884279 kalm-0.4.5/src/kalm/toolbox.py
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 kalm-0.4.5/PKG-INFO
```

### Comparing `kalm-0.4.4/LICENSE.txt` & `kalm-0.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.4.4/pyproject.toml` & `kalm-0.4.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "kalm"
-version = "0.4.4"
+version = "0.4.5"
 description = "Knowit Automation lifecycle management"
 authors = ["Jakob Holst <jakob.holst@knowit.dk>"]
 license = "MIT"
 homepage = "https://kalm.openknowit.com"
 repository = "https://github.com/miracle-as/openknowit_kalm.git"
 
 [tool.poetry.scripts]
 kalm = "kalm:main"
+kalm-jenkins = "jenkins:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.25"
 pytest = "^6.2"
 mypy = "^0.910"
 redis = "^4.5.3"
```

### Comparing `kalm-0.4.4/src/kalm/__init__.py` & `kalm-0.4.5/src/kalm/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.4.4/src/kalm/kalm.py` & `kalm-0.4.5/src/kalm/kalm.py`

 * *Files identical despite different names*

### Comparing `kalm-0.4.4/src/kalm/kalm_api.py` & `kalm-0.4.5/src/kalm/kalm_api.py`

 * *Files identical despite different names*

### Comparing `kalm-0.4.4/src/kalm/netbox.py` & `kalm-0.4.5/src/kalm/netbox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.4.4/PKG-INFO` & `kalm-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.4.4
+Version: 0.4.5
 Summary: Knowit Automation lifecycle management
 Home-page: https://kalm.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

