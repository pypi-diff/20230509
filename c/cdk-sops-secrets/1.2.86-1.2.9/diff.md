# Comparing `tmp/cdk-sops-secrets-1.2.86.tar.gz` & `tmp/cdk-sops-secrets-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-sops-secrets-1.2.86.tar", last modified: Tue May  9 00:26:08 2023, max compression
+gzip compressed data, was "cdk-sops-secrets-1.2.9.tar", last modified: Fri Mar 24 22:38:30 2023, max compression
```

## Comparing `cdk-sops-secrets-1.2.86.tar` & `cdk-sops-secrets-1.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:26:08.198985 cdk-sops-secrets-1.2.86/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-09 00:25:56.000000 cdk-sops-secrets-1.2.86/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 00:25:56.000000 cdk-sops-secrets-1.2.86/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-09 00:26:08.198985 cdk-sops-secrets-1.2.86/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-05-09 00:25:56.000000 cdk-sops-secrets-1.2.86/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-09 00:25:56.000000 cdk-sops-secrets-1.2.86/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:26:08.198985 cdk-sops-secrets-1.2.86/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-09 00:25:56.000000 cdk-sops-secrets-1.2.86/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:26:08.186985 cdk-sops-secrets-1.2.86/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:26:08.190985 cdk-sops-secrets-1.2.86/src/cdk_sops_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)    76168 2023-05-09 00:25:56.000000 cdk-sops-secrets-1.2.86/src/cdk_sops_secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:26:08.190985 cdk-sops-secrets-1.2.86/src/cdk_sops_secrets/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-09 00:25:56.000000 cdk-sops-secrets-1.2.86/src/cdk_sops_secrets/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  7059201 2023-05-09 00:25:56.000000 cdk-sops-secrets-1.2.86/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.2.86.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:25:56.000000 cdk-sops-secrets-1.2.86/src/cdk_sops_secrets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:26:08.190985 cdk-sops-secrets-1.2.86/src/cdk_sops_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-09 00:26:08.000000 cdk-sops-secrets-1.2.86/src/cdk_sops_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-09 00:26:08.000000 cdk-sops-secrets-1.2.86/src/cdk_sops_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:26:08.000000 cdk-sops-secrets-1.2.86/src/cdk_sops_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-09 00:26:08.000000 cdk-sops-secrets-1.2.86/src/cdk_sops_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-09 00:26:08.000000 cdk-sops-secrets-1.2.86/src/cdk_sops_secrets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 22:38:30.920565 cdk-sops-secrets-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-24 22:38:18.000000 cdk-sops-secrets-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-24 22:38:18.000000 cdk-sops-secrets-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-03-24 22:38:30.920565 cdk-sops-secrets-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-03-24 22:38:18.000000 cdk-sops-secrets-1.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-24 22:38:18.000000 cdk-sops-secrets-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 22:38:30.920565 cdk-sops-secrets-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-03-24 22:38:18.000000 cdk-sops-secrets-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 22:38:30.912565 cdk-sops-secrets-1.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 22:38:30.912565 cdk-sops-secrets-1.2.9/src/cdk_sops_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)    76168 2023-03-24 22:38:18.000000 cdk-sops-secrets-1.2.9/src/cdk_sops_secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 22:38:30.912565 cdk-sops-secrets-1.2.9/src/cdk_sops_secrets/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-24 22:38:18.000000 cdk-sops-secrets-1.2.9/src/cdk_sops_secrets/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7056003 2023-03-24 22:38:18.000000 cdk-sops-secrets-1.2.9/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.2.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 22:38:18.000000 cdk-sops-secrets-1.2.9/src/cdk_sops_secrets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 22:38:30.912565 cdk-sops-secrets-1.2.9/src/cdk_sops_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-03-24 22:38:30.000000 cdk-sops-secrets-1.2.9/src/cdk_sops_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-24 22:38:30.000000 cdk-sops-secrets-1.2.9/src/cdk_sops_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 22:38:30.000000 cdk-sops-secrets-1.2.9/src/cdk_sops_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-24 22:38:30.000000 cdk-sops-secrets-1.2.9/src/cdk_sops_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-24 22:38:30.000000 cdk-sops-secrets-1.2.9/src/cdk_sops_secrets.egg-info/top_level.txt
```

### Comparing `cdk-sops-secrets-1.2.86/LICENSE` & `cdk-sops-secrets-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.2.86/PKG-INFO` & `cdk-sops-secrets-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-sops-secrets
-Version: 1.2.86
+Version: 1.2.9
 Summary: CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.
 Home-page: https://constructs.dev/packages/cdk-sops-secrets
 Author: Markus Siebert<dev@markussiebert.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/markussiebert/cdk-sops-secrets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-sops-secrets-1.2.86/README.md` & `cdk-sops-secrets-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.2.86/setup.py` & `cdk-sops-secrets-1.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-sops-secrets",
-    "version": "1.2.86",
+    "version": "1.2.9",
     "description": "CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.",
     "license": "Apache-2.0",
     "url": "https://constructs.dev/packages/cdk-sops-secrets",
     "long_description_content_type": "text/markdown",
     "author": "Markus Siebert<dev@markussiebert.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_sops_secrets",
         "cdk_sops_secrets._jsii"
     ],
     "package_data": {
         "cdk_sops_secrets._jsii": [
-            "cdk-sops-secrets@1.2.86.jsii.tgz"
+            "cdk-sops-secrets@1.2.9.jsii.tgz"
         ],
         "cdk_sops_secrets": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.1.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.80.0, <2.0.0",
+        "jsii>=1.79.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-sops-secrets-1.2.86/src/cdk_sops_secrets/__init__.py` & `cdk-sops-secrets-1.2.9/src/cdk_sops_secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.2.86/src/cdk_sops_secrets.egg-info/PKG-INFO` & `cdk-sops-secrets-1.2.9/src/cdk_sops_secrets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-sops-secrets
-Version: 1.2.86
+Version: 1.2.9
 Summary: CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.
 Home-page: https://constructs.dev/packages/cdk-sops-secrets
 Author: Markus Siebert<dev@markussiebert.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/markussiebert/cdk-sops-secrets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

