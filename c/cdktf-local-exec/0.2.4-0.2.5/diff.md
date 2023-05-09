# Comparing `tmp/cdktf-local-exec-0.2.4.tar.gz` & `tmp/cdktf-local-exec-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-local-exec-0.2.4.tar", last modified: Wed Mar  8 09:58:14 2023, max compression
+gzip compressed data, was "cdktf-local-exec-0.2.5.tar", last modified: Tue May  9 10:44:50 2023, max compression
```

## Comparing `cdktf-local-exec-0.2.4.tar` & `cdktf-local-exec-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 09:58:14.406418 cdktf-local-exec-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-08 09:57:58.000000 cdktf-local-exec-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-08 09:57:58.000000 cdktf-local-exec-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-03-08 09:58:14.406418 cdktf-local-exec-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-08 09:57:58.000000 cdktf-local-exec-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-08 09:57:58.000000 cdktf-local-exec-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 09:58:14.406418 cdktf-local-exec-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-03-08 09:57:58.000000 cdktf-local-exec-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 09:58:14.406418 cdktf-local-exec-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 09:58:14.406418 cdktf-local-exec-0.2.4/src/cdktf_local_exec/
--rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-03-08 09:57:58.000000 cdktf-local-exec-0.2.4/src/cdktf_local_exec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 09:58:14.406418 cdktf-local-exec-0.2.4/src/cdktf_local_exec/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-08 09:57:58.000000 cdktf-local-exec-0.2.4/src/cdktf_local_exec/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-03-08 09:57:58.000000 cdktf-local-exec-0.2.4/src/cdktf_local_exec/_jsii/cdktf-local-exec@0.2.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 09:57:58.000000 cdktf-local-exec-0.2.4/src/cdktf_local_exec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 09:58:14.406418 cdktf-local-exec-0.2.4/src/cdktf_local_exec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-03-08 09:58:13.000000 cdktf-local-exec-0.2.4/src/cdktf_local_exec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-08 09:58:14.000000 cdktf-local-exec-0.2.4/src/cdktf_local_exec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 09:58:13.000000 cdktf-local-exec-0.2.4/src/cdktf_local_exec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-08 09:58:14.000000 cdktf-local-exec-0.2.4/src/cdktf_local_exec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-08 09:58:14.000000 cdktf-local-exec-0.2.4/src/cdktf_local_exec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:44:50.266554 cdktf-local-exec-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-09 10:44:37.000000 cdktf-local-exec-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 10:44:37.000000 cdktf-local-exec-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-09 10:44:50.266554 cdktf-local-exec-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-09 10:44:37.000000 cdktf-local-exec-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-09 10:44:37.000000 cdktf-local-exec-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 10:44:50.266554 cdktf-local-exec-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-09 10:44:37.000000 cdktf-local-exec-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:44:50.262554 cdktf-local-exec-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:44:50.266554 cdktf-local-exec-0.2.5/src/cdktf_local_exec/
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-05-09 10:44:37.000000 cdktf-local-exec-0.2.5/src/cdktf_local_exec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:44:50.266554 cdktf-local-exec-0.2.5/src/cdktf_local_exec/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-09 10:44:37.000000 cdktf-local-exec-0.2.5/src/cdktf_local_exec/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-05-09 10:44:37.000000 cdktf-local-exec-0.2.5/src/cdktf_local_exec/_jsii/cdktf-local-exec@0.2.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:44:37.000000 cdktf-local-exec-0.2.5/src/cdktf_local_exec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:44:50.266554 cdktf-local-exec-0.2.5/src/cdktf_local_exec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-09 10:44:50.000000 cdktf-local-exec-0.2.5/src/cdktf_local_exec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-09 10:44:50.000000 cdktf-local-exec-0.2.5/src/cdktf_local_exec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:44:50.000000 cdktf-local-exec-0.2.5/src/cdktf_local_exec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-09 10:44:50.000000 cdktf-local-exec-0.2.5/src/cdktf_local_exec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-09 10:44:50.000000 cdktf-local-exec-0.2.5/src/cdktf_local_exec.egg-info/top_level.txt
```

### Comparing `cdktf-local-exec-0.2.4/LICENSE` & `cdktf-local-exec-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-local-exec-0.2.4/PKG-INFO` & `cdktf-local-exec-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-local-exec
-Version: 0.2.4
+Version: 0.2.5
 Summary: A simple construct that executes a command locally. This is useful to run build steps within your CDKTF Program or to run a post action after a resource is created.
 Home-page: https://github.com/DanielMSchmidt/cdktf-local-exec.git
 Author: Daniel Schmidt<danielmschmidt92@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/DanielMSchmidt/cdktf-local-exec.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -58,9 +58,7 @@
 ```
 
 ### Options
 
 * `cwd`: The working directory to run the command in. It will be copied before execution to ensure the asset can be used in a remote execution environment.
 * `command`: The command to execute.
 * `copyBeforeRun`: If true, the command will copy the `cwd` directory into a tmp dir and run there. If false, the command will be executed in the `cwd` directory.
-
-
```

### Comparing `cdktf-local-exec-0.2.4/README.md` & `cdktf-local-exec-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-local-exec-0.2.4/setup.py` & `cdktf-local-exec-0.2.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-local-exec",
-    "version": "0.2.4",
+    "version": "0.2.5",
     "description": "A simple construct that executes a command locally. This is useful to run build steps within your CDKTF Program or to run a post action after a resource is created.",
     "license": "Apache-2.0",
     "url": "https://github.com/DanielMSchmidt/cdktf-local-exec.git",
     "long_description_content_type": "text/markdown",
     "author": "Daniel Schmidt<danielmschmidt92@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,38 +22,39 @@
     },
     "packages": [
         "cdktf_local_exec",
         "cdktf_local_exec._jsii"
     ],
     "package_data": {
         "cdktf_local_exec._jsii": [
-            "cdktf-local-exec@0.2.4.jsii.tgz"
+            "cdktf-local-exec@0.2.5.jsii.tgz"
         ],
         "cdktf_local_exec": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "cdktf-cdktf-provider-null>=5.0.0",
         "cdktf>=0.15.0",
-        "constructs>=10.0.107, <11.0.0",
-        "jsii>=1.73.0, <2.0.0",
+        "constructs>=10.0.25, <11.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdktf-local-exec-0.2.4/src/cdktf_local_exec/__init__.py` & `cdktf-local-exec-0.2.5/src/cdktf_local_exec/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-local-exec-0.2.4/src/cdktf_local_exec.egg-info/PKG-INFO` & `cdktf-local-exec-0.2.5/src/cdktf_local_exec.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-local-exec
-Version: 0.2.4
+Version: 0.2.5
 Summary: A simple construct that executes a command locally. This is useful to run build steps within your CDKTF Program or to run a post action after a resource is created.
 Home-page: https://github.com/DanielMSchmidt/cdktf-local-exec.git
 Author: Daniel Schmidt<danielmschmidt92@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/DanielMSchmidt/cdktf-local-exec.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -58,9 +58,7 @@
 ```
 
 ### Options
 
 * `cwd`: The working directory to run the command in. It will be copied before execution to ensure the asset can be used in a remote execution environment.
 * `command`: The command to execute.
 * `copyBeforeRun`: If true, the command will copy the `cwd` directory into a tmp dir and run there. If false, the command will be executed in the `cwd` directory.
-
-
```

