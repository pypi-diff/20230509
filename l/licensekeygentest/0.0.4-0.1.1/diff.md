# Comparing `tmp/licensekeygentest-0.0.4.tar.gz` & `tmp/licensekeygentest-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "licensekeygentest-0.0.4.tar", last modified: Tue May  9 09:23:26 2023, max compression
+gzip compressed data, was "licensekeygentest-0.1.1.tar", last modified: Tue May  9 10:43:59 2023, max compression
```

## Comparing `licensekeygentest-0.0.4.tar` & `licensekeygentest-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 09:23:26.163446 licensekeygentest-0.0.4/
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1063 2023-05-08 14:20:18.000000 licensekeygentest-0.0.4/LICENSE
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      636 2023-05-09 09:23:26.163446 licensekeygentest-0.0.4/PKG-INFO
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       92 2023-05-09 09:18:34.000000 licensekeygentest-0.0.4/README.md
-drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 09:23:26.159446 licensekeygentest-0.0.4/licensekeygentest/
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       43 2023-05-08 13:59:31.000000 licensekeygentest-0.0.4/licensekeygentest/__init__.py
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     2191 2023-05-09 09:22:40.000000 licensekeygentest-0.0.4/licensekeygentest/main.py
-drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 09:23:26.163446 licensekeygentest-0.0.4/licensekeygentest.egg-info/
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      636 2023-05-09 09:23:26.000000 licensekeygentest-0.0.4/licensekeygentest.egg-info/PKG-INFO
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      286 2023-05-09 09:23:26.000000 licensekeygentest-0.0.4/licensekeygentest.egg-info/SOURCES.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)        1 2023-05-09 09:23:26.000000 licensekeygentest-0.0.4/licensekeygentest.egg-info/dependency_links.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       22 2023-05-09 09:23:26.000000 licensekeygentest-0.0.4/licensekeygentest.egg-info/requires.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       18 2023-05-09 09:23:26.000000 licensekeygentest-0.0.4/licensekeygentest.egg-info/top_level.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       38 2023-05-09 09:23:26.163446 licensekeygentest-0.0.4/setup.cfg
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1074 2023-05-09 09:23:15.000000 licensekeygentest-0.0.4/setup.py
+drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 10:43:59.546792 licensekeygentest-0.1.1/
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1063 2023-05-08 14:20:18.000000 licensekeygentest-0.1.1/LICENSE
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      695 2023-05-09 10:43:59.546792 licensekeygentest-0.1.1/PKG-INFO
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      152 2023-05-09 09:30:18.000000 licensekeygentest-0.1.1/README.md
+drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 10:43:59.542792 licensekeygentest-0.1.1/licensekeygentest/
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       43 2023-05-08 13:59:31.000000 licensekeygentest-0.1.1/licensekeygentest/__init__.py
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1388 2023-05-09 10:41:07.000000 licensekeygentest-0.1.1/licensekeygentest/main.py
+drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 10:43:59.546792 licensekeygentest-0.1.1/licensekeygentest.egg-info/
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      695 2023-05-09 10:43:59.000000 licensekeygentest-0.1.1/licensekeygentest.egg-info/PKG-INFO
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      286 2023-05-09 10:43:59.000000 licensekeygentest-0.1.1/licensekeygentest.egg-info/SOURCES.txt
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)        1 2023-05-09 10:43:59.000000 licensekeygentest-0.1.1/licensekeygentest.egg-info/dependency_links.txt
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       22 2023-05-09 10:43:59.000000 licensekeygentest-0.1.1/licensekeygentest.egg-info/requires.txt
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       18 2023-05-09 10:43:59.000000 licensekeygentest-0.1.1/licensekeygentest.egg-info/top_level.txt
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       38 2023-05-09 10:43:59.546792 licensekeygentest-0.1.1/setup.cfg
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1074 2023-05-09 10:43:18.000000 licensekeygentest-0.1.1/setup.py
```

### Comparing `licensekeygentest-0.0.4/LICENSE` & `licensekeygentest-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `licensekeygentest-0.0.4/PKG-INFO` & `licensekeygentest-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensekeygentest
-Version: 0.0.4
+Version: 0.1.1
 Summary: POC for keygen authentication
 Author: Rahul R
 Author-email: <rahulranjan25.RR@gmail.com>
 Keywords: python,authentication,licensing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -14,8 +14,13 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Licensed Library KeyGen test
 
 This is test environment for lisenced libraries over PyPi.
- 
+
+To use this poc:
+```bash
+pip install licensekeygentest
+```
+
```

### Comparing `licensekeygentest-0.0.4/licensekeygentest/main.py` & `licensekeygentest-0.1.1/licensekeygentest/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import machineid
 import requests
 import json
-import os
 
 class library():
-  def __init__(self, license_key):
-    machine_fingerprint = machineid.hashed_id('example-app')
+  def __init__(self, keygen_account_id, license_key):
+    machine_fingerprint = machineid.hashed_id('app-name')
     validation = requests.post(
-      "https://api.keygen.sh/v1/accounts/{}/licenses/actions/validate-key".format(os.environ['KEYGEN_ACCOUNT_ID']),
+      f"https://api.keygen.sh/v1/accounts/{keygen_account_id}/licenses/actions/validate-key",
       headers={
         "Content-Type": "application/vnd.api+json",
         "Accept": "application/vnd.api+json"
       },
       data=json.dumps({
         "meta": {
           "scope": { "fingerprint": machine_fingerprint },
@@ -25,42 +24,16 @@
         map(lambda e: "{} - {}".format(e["title"], e["detail"]).lower(), errs)
       ))
 
     if validation["meta"]["valid"]:
       print("license has already been activated on this machine")
     
     validation_code = validation["meta"]["code"]
-    activation_is_required = validation_code == 'FINGERPRINT_SCOPE_MISMATCH' or \
-                             validation_code == 'NO_MACHINES' or \
-                             validation_code == 'NO_MACHINE'
-    print(validation_code)
-    if not activation_is_required:
-      print("license {}".format(validation["meta"]["detail"]))
-
-    activation = requests.post(
-      "https://api.keygen.sh/v1/accounts/{}/machines".format(os.environ['KEYGEN_ACCOUNT_ID']),
-      headers={
-        "Authorization": "License {}".format(license_key),
-        "Content-Type": "application/vnd.api+json",
-        "Accept": "application/vnd.api+json"
-      },
-      data=json.dumps({
-        "data": {
-          "type": "machines",
-          "attributes": {
-            "fingerprint": machine_fingerprint
-          },
-          "relationships": {
-            "license": {
-              "data": { "type": "licenses", "id": validation["data"]["id"] }
-            }
-          }
-        }
-      })
-    ).json()
-
-    if "errors" in activation:
-      errs = activation["errors"]
-      raise Exception("license activation failed: {}".format(
-        ','.join(map(lambda e: "{} - {}".format(e["title"], e["detail"]).lower(), errs))
-      ))
-
+    print(">> Validation Code:", validation_code)
+    invalid_code =  validation_code == "SUSPENDED" or \
+                    validation_code == "NOT_FOUND"
+    
+    if invalid_code:
+      if validation_code == "SUSPENDED":
+        raise Exception("License is suspended. Please contact the library administrator.")
+      if validation_code == "NOT_FOUND":
+        raise Exception("Invalid License Key. Please recheck license_key")
```

### Comparing `licensekeygentest-0.0.4/licensekeygentest.egg-info/PKG-INFO` & `licensekeygentest-0.1.1/licensekeygentest.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensekeygentest
-Version: 0.0.4
+Version: 0.1.1
 Summary: POC for keygen authentication
 Author: Rahul R
 Author-email: <rahulranjan25.RR@gmail.com>
 Keywords: python,authentication,licensing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -14,8 +14,13 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Licensed Library KeyGen test
 
 This is test environment for lisenced libraries over PyPi.
- 
+
+To use this poc:
+```bash
+pip install licensekeygentest
+```
+
```

### Comparing `licensekeygentest-0.0.4/setup.py` & `licensekeygentest-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.1.1'
 DESCRIPTION = 'POC for keygen authentication'
 LONG_DESCRIPTION = 'A POC package that allows lisencing of python libraries.'
 
 # Setting up
 setup(
     name="licensekeygentest",
     version=VERSION,
```

