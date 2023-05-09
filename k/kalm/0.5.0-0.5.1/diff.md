# Comparing `tmp/kalm-0.5.0.tar.gz` & `tmp/kalm-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.5.0.tar", max compression
+gzip compressed data, was "kalm-0.5.1.tar", max compression
```

## Comparing `kalm-0.5.0.tar` & `kalm-0.5.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     1817 2023-05-09 12:39:56.912035 kalm-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    10421 2023-05-09 12:32:33.321460 kalm-0.5.0/src/kalm/__init__.py
--rw-r--r--   0        0        0    32279 2023-05-09 12:32:33.321460 kalm-0.5.0/src/kalm/kalm.py
--rw-r--r--   0        0        0     1296 2023-05-09 12:32:33.321460 kalm-0.5.0/src/kalm/netbox.py
--rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.5.0/src/kalm/package_data.dat
--rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.5.0/src/kalm/toolbox.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     1879 2023-05-09 13:05:09.820797 kalm-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    10421 2023-05-09 12:32:33.321460 kalm-0.5.1/src/kalm/__init__.py
+-rw-r--r--   0        0        0    32279 2023-05-09 12:32:33.321460 kalm-0.5.1/src/kalm/kalm.py
+-rw-r--r--   0        0        0     1296 2023-05-09 12:32:33.321460 kalm-0.5.1/src/kalm/netbox.py
+-rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.5.1/src/kalm/package_data.dat
+-rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.5.1/src/kalm/toolbox.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.5.1/PKG-INFO
```

### Comparing `kalm-0.5.0/LICENSE.txt` & `kalm-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.5.0/pyproject.toml` & `kalm-0.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 [tool.poetry]
 name = "kalm"
-version = "0.5.0"
+version = "0.5.1"
 description = "Knowit Automation lifecycle management"
 authors = ["Jakob Holst <jakob.holst@knowit.dk>"]
 license = "MIT"
 homepage = "https://kalm.openknowit.com"
 repository = "https://github.com/miracle-as/openknowit_kalm.git"
 
+[tool.poetry.scripts]
+kalm_jenkins = 'jenkins.jenkins:main'
+
+
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.25"
 pytest = "^6.2"
 mypy = "^0.910"
 redis = "^4.5.3"
 pynetbox = "^6.6.2"
```

### Comparing `kalm-0.5.0/src/kalm/__init__.py` & `kalm-0.5.1/src/kalm/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.5.0/src/kalm/kalm.py` & `kalm-0.5.1/src/kalm/kalm.py`

 * *Files identical despite different names*

### Comparing `kalm-0.5.0/src/kalm/netbox.py` & `kalm-0.5.1/src/kalm/netbox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.5.0/PKG-INFO` & `kalm-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.5.0
+Version: 0.5.1
 Summary: Knowit Automation lifecycle management
 Home-page: https://kalm.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

