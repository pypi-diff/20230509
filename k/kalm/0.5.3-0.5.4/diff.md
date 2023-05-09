# Comparing `tmp/kalm-0.5.3.tar.gz` & `tmp/kalm-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.5.3.tar", max compression
+gzip compressed data, was "kalm-0.5.4.tar", max compression
```

## Comparing `kalm-0.5.3.tar` & `kalm-0.5.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.5.3/LICENSE.txt
--rw-r--r--   0        0        0     1876 2023-05-09 13:11:15.106909 kalm-0.5.3/pyproject.toml
--rw-r--r--   0        0        0    10421 2023-05-09 12:32:33.321460 kalm-0.5.3/src/kalm/__init__.py
--rw-r--r--   0        0        0    32279 2023-05-09 12:32:33.321460 kalm-0.5.3/src/kalm/kalm.py
--rw-r--r--   0        0        0     1296 2023-05-09 12:32:33.321460 kalm-0.5.3/src/kalm/netbox.py
--rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.5.3/src/kalm/package_data.dat
--rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.5.3/src/kalm/toolbox.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.5.4/LICENSE.txt
+-rw-r--r--   0        0        0     1890 2023-05-09 13:14:10.207922 kalm-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0    10421 2023-05-09 12:32:33.321460 kalm-0.5.4/src/kalm/__init__.py
+-rw-r--r--   0        0        0    32279 2023-05-09 12:32:33.321460 kalm-0.5.4/src/kalm/kalm.py
+-rw-r--r--   0        0        0     1296 2023-05-09 12:32:33.321460 kalm-0.5.4/src/kalm/netbox.py
+-rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.5.4/src/kalm/package_data.dat
+-rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.5.4/src/kalm/toolbox.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.5.4/PKG-INFO
```

### Comparing `kalm-0.5.3/LICENSE.txt` & `kalm-0.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.5.3/pyproject.toml` & `kalm-0.5.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "kalm"
-version = "0.5.3"
+version = "0.5.4"
 description = "Knowit Automation lifecycle management"
 authors = ["Jakob Holst <jakob.holst@knowit.dk>"]
 license = "MIT"
 homepage = "https://kalm.openknowit.com"
 repository = "https://github.com/miracle-as/openknowit_kalm.git"
 
 [tool.poetry.scripts]
-kalm_jenkins = 'kalm.jenkins:main'
+kalm = 'kalm:main'
+kalm_jenkins = 'kalm:jenkins'
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.25"
 pytest = "^6.2"
 mypy = "^0.910"
```

### Comparing `kalm-0.5.3/src/kalm/__init__.py` & `kalm-0.5.4/src/kalm/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.5.3/src/kalm/kalm.py` & `kalm-0.5.4/src/kalm/kalm.py`

 * *Files identical despite different names*

### Comparing `kalm-0.5.3/src/kalm/netbox.py` & `kalm-0.5.4/src/kalm/netbox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.5.3/PKG-INFO` & `kalm-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.5.3
+Version: 0.5.4
 Summary: Knowit Automation lifecycle management
 Home-page: https://kalm.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

