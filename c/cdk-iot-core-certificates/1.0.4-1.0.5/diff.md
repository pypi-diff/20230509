# Comparing `tmp/cdk-iot-core-certificates-1.0.4.tar.gz` & `tmp/cdk-iot-core-certificates-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-iot-core-certificates-1.0.4.tar", last modified: Mon May  8 08:29:14 2023, max compression
+gzip compressed data, was "cdk-iot-core-certificates-1.0.5.tar", last modified: Tue May  9 00:10:50 2023, max compression
```

## Comparing `cdk-iot-core-certificates-1.0.4.tar` & `cdk-iot-core-certificates-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:14.070136 cdk-iot-core-certificates-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-08 08:29:02.000000 cdk-iot-core-certificates-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 08:29:02.000000 cdk-iot-core-certificates-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-08 08:29:14.070136 cdk-iot-core-certificates-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-08 08:29:02.000000 cdk-iot-core-certificates-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-08 08:29:02.000000 cdk-iot-core-certificates-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:29:14.070136 cdk-iot-core-certificates-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-08 08:29:02.000000 cdk-iot-core-certificates-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:14.070136 cdk-iot-core-certificates-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:14.070136 cdk-iot-core-certificates-1.0.4/src/cdk_iot_core_certficates/
--rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-05-08 08:29:02.000000 cdk-iot-core-certificates-1.0.4/src/cdk_iot_core_certficates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:14.070136 cdk-iot-core-certificates-1.0.4/src/cdk_iot_core_certficates/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-08 08:29:02.000000 cdk-iot-core-certificates-1.0.4/src/cdk_iot_core_certficates/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24073 2023-05-08 08:29:02.000000 cdk-iot-core-certificates-1.0.4/src/cdk_iot_core_certficates/_jsii/cdk-iot-core-certificates@1.0.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:29:02.000000 cdk-iot-core-certificates-1.0.4/src/cdk_iot_core_certficates/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:29:14.070136 cdk-iot-core-certificates-1.0.4/src/cdk_iot_core_certificates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-08 08:29:14.000000 cdk-iot-core-certificates-1.0.4/src/cdk_iot_core_certificates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-08 08:29:14.000000 cdk-iot-core-certificates-1.0.4/src/cdk_iot_core_certificates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:29:14.000000 cdk-iot-core-certificates-1.0.4/src/cdk_iot_core_certificates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-08 08:29:14.000000 cdk-iot-core-certificates-1.0.4/src/cdk_iot_core_certificates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 08:29:14.000000 cdk-iot-core-certificates-1.0.4/src/cdk_iot_core_certificates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:10:50.969016 cdk-iot-core-certificates-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-09 00:10:38.000000 cdk-iot-core-certificates-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 00:10:38.000000 cdk-iot-core-certificates-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-09 00:10:50.969016 cdk-iot-core-certificates-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-09 00:10:38.000000 cdk-iot-core-certificates-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-09 00:10:38.000000 cdk-iot-core-certificates-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:10:50.969016 cdk-iot-core-certificates-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-09 00:10:38.000000 cdk-iot-core-certificates-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:10:50.965016 cdk-iot-core-certificates-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:10:50.965016 cdk-iot-core-certificates-1.0.5/src/cdk_iot_core_certficates/
+-rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-05-09 00:10:38.000000 cdk-iot-core-certificates-1.0.5/src/cdk_iot_core_certficates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:10:50.965016 cdk-iot-core-certificates-1.0.5/src/cdk_iot_core_certficates/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-09 00:10:38.000000 cdk-iot-core-certificates-1.0.5/src/cdk_iot_core_certficates/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24070 2023-05-09 00:10:38.000000 cdk-iot-core-certificates-1.0.5/src/cdk_iot_core_certficates/_jsii/cdk-iot-core-certificates@1.0.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:10:38.000000 cdk-iot-core-certificates-1.0.5/src/cdk_iot_core_certficates/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:10:50.969016 cdk-iot-core-certificates-1.0.5/src/cdk_iot_core_certificates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-09 00:10:50.000000 cdk-iot-core-certificates-1.0.5/src/cdk_iot_core_certificates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-09 00:10:50.000000 cdk-iot-core-certificates-1.0.5/src/cdk_iot_core_certificates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:10:50.000000 cdk-iot-core-certificates-1.0.5/src/cdk_iot_core_certificates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-09 00:10:50.000000 cdk-iot-core-certificates-1.0.5/src/cdk_iot_core_certificates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 00:10:50.000000 cdk-iot-core-certificates-1.0.5/src/cdk_iot_core_certificates.egg-info/top_level.txt
```

### Comparing `cdk-iot-core-certificates-1.0.4/LICENSE` & `cdk-iot-core-certificates-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-iot-core-certificates-1.0.4/PKG-INFO` & `cdk-iot-core-certificates-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-iot-core-certificates
-Version: 1.0.4
+Version: 1.0.5
 Summary: cdk-iot-core-certificates
 Home-page: https://github.com/polyperception/cdk-iot-core-certificates
 Author: DevOps@Home<devops.at.home@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/polyperception/cdk-iot-core-certificates
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-iot-core-certificates-1.0.4/README.md` & `cdk-iot-core-certificates-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cdk-iot-core-certificates-1.0.4/setup.py` & `cdk-iot-core-certificates-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-iot-core-certificates",
-    "version": "1.0.4",
+    "version": "1.0.5",
     "description": "cdk-iot-core-certificates",
     "license": "MIT",
     "url": "https://github.com/polyperception/cdk-iot-core-certificates",
     "long_description_content_type": "text/markdown",
     "author": "DevOps@Home<devops.at.home@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_iot_core_certficates",
         "cdk_iot_core_certficates._jsii"
     ],
     "package_data": {
         "cdk_iot_core_certficates._jsii": [
-            "cdk-iot-core-certificates@1.0.4.jsii.tgz"
+            "cdk-iot-core-certificates@1.0.5.jsii.tgz"
         ],
         "cdk_iot_core_certficates": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-iot-core-certificates-1.0.4/src/cdk_iot_core_certficates/__init__.py` & `cdk-iot-core-certificates-1.0.5/src/cdk_iot_core_certficates/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-iot-core-certificates-1.0.4/src/cdk_iot_core_certificates.egg-info/PKG-INFO` & `cdk-iot-core-certificates-1.0.5/src/cdk_iot_core_certificates.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-iot-core-certificates
-Version: 1.0.4
+Version: 1.0.5
 Summary: cdk-iot-core-certificates
 Home-page: https://github.com/polyperception/cdk-iot-core-certificates
 Author: DevOps@Home<devops.at.home@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/polyperception/cdk-iot-core-certificates
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-iot-core-certificates-1.0.4/src/cdk_iot_core_certificates.egg-info/SOURCES.txt` & `cdk-iot-core-certificates-1.0.5/src/cdk_iot_core_certificates.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/cdk_iot_core_certficates/__init__.py
 src/cdk_iot_core_certficates/py.typed
 src/cdk_iot_core_certficates/_jsii/__init__.py
-src/cdk_iot_core_certficates/_jsii/cdk-iot-core-certificates@1.0.4.jsii.tgz
+src/cdk_iot_core_certficates/_jsii/cdk-iot-core-certificates@1.0.5.jsii.tgz
 src/cdk_iot_core_certificates.egg-info/PKG-INFO
 src/cdk_iot_core_certificates.egg-info/SOURCES.txt
 src/cdk_iot_core_certificates.egg-info/dependency_links.txt
 src/cdk_iot_core_certificates.egg-info/requires.txt
 src/cdk_iot_core_certificates.egg-info/top_level.txt
```

