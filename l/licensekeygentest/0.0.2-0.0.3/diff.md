# Comparing `tmp/licensekeygentest-0.0.2.tar.gz` & `tmp/licensekeygentest-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "licensekeygentest-0.0.2.tar", last modified: Tue May  9 08:25:50 2023, max compression
+gzip compressed data, was "licensekeygentest-0.0.3.tar", last modified: Tue May  9 09:17:16 2023, max compression
```

## Comparing `licensekeygentest-0.0.2.tar` & `licensekeygentest-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 08:25:50.613454 licensekeygentest-0.0.2/
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1063 2023-05-08 14:20:18.000000 licensekeygentest-0.0.2/LICENSE
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      574 2023-05-09 08:25:50.613454 licensekeygentest-0.0.2/PKG-INFO
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       30 2023-05-08 15:05:37.000000 licensekeygentest-0.0.2/README.md
-drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 08:25:50.613454 licensekeygentest-0.0.2/licensekeygentest/
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       43 2023-05-08 13:59:31.000000 licensekeygentest-0.0.2/licensekeygentest/__init__.py
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     2225 2023-05-09 08:21:05.000000 licensekeygentest-0.0.2/licensekeygentest/main.py
-drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 08:25:50.613454 licensekeygentest-0.0.2/licensekeygentest.egg-info/
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      574 2023-05-09 08:25:50.000000 licensekeygentest-0.0.2/licensekeygentest.egg-info/PKG-INFO
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      286 2023-05-09 08:25:50.000000 licensekeygentest-0.0.2/licensekeygentest.egg-info/SOURCES.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)        1 2023-05-09 08:25:50.000000 licensekeygentest-0.0.2/licensekeygentest.egg-info/dependency_links.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       22 2023-05-09 08:25:50.000000 licensekeygentest-0.0.2/licensekeygentest.egg-info/requires.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       18 2023-05-09 08:25:50.000000 licensekeygentest-0.0.2/licensekeygentest.egg-info/top_level.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       38 2023-05-09 08:25:50.613454 licensekeygentest-0.0.2/setup.cfg
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1074 2023-05-09 08:23:20.000000 licensekeygentest-0.0.2/setup.py
+drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 09:17:16.431305 licensekeygentest-0.0.3/
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1063 2023-05-08 14:20:18.000000 licensekeygentest-0.0.3/LICENSE
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      574 2023-05-09 09:17:16.431305 licensekeygentest-0.0.3/PKG-INFO
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       30 2023-05-08 15:05:37.000000 licensekeygentest-0.0.3/README.md
+drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 09:17:16.427305 licensekeygentest-0.0.3/licensekeygentest/
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       43 2023-05-08 13:59:31.000000 licensekeygentest-0.0.3/licensekeygentest/__init__.py
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     2225 2023-05-09 09:11:39.000000 licensekeygentest-0.0.3/licensekeygentest/main.py
+drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 09:17:16.431305 licensekeygentest-0.0.3/licensekeygentest.egg-info/
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      574 2023-05-09 09:17:16.000000 licensekeygentest-0.0.3/licensekeygentest.egg-info/PKG-INFO
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      286 2023-05-09 09:17:16.000000 licensekeygentest-0.0.3/licensekeygentest.egg-info/SOURCES.txt
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)        1 2023-05-09 09:17:16.000000 licensekeygentest-0.0.3/licensekeygentest.egg-info/dependency_links.txt
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       22 2023-05-09 09:17:16.000000 licensekeygentest-0.0.3/licensekeygentest.egg-info/requires.txt
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       18 2023-05-09 09:17:16.000000 licensekeygentest-0.0.3/licensekeygentest.egg-info/top_level.txt
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       38 2023-05-09 09:17:16.431305 licensekeygentest-0.0.3/setup.cfg
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1074 2023-05-09 09:16:42.000000 licensekeygentest-0.0.3/setup.py
```

### Comparing `licensekeygentest-0.0.2/LICENSE` & `licensekeygentest-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `licensekeygentest-0.0.2/PKG-INFO` & `licensekeygentest-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensekeygentest
-Version: 0.0.2
+Version: 0.0.3
 Summary: POC for keygen authentication
 Author: Rahul R
 Author-email: <rahulranjan25.RR@gmail.com>
 Keywords: python,authentication,licensing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `licensekeygentest-0.0.2/licensekeygentest/main.py` & `licensekeygentest-0.0.3/licensekeygentest/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import machineid
 import requests
 import json
-import sys
 import os
 
 class library():
   def __init__(self, license_key):
     machine_fingerprint = machineid.hashed_id('example-app')
     validation = requests.post(
       "https://api.keygen.sh/v1/accounts/{}/licenses/actions/validate-key".format(os.environ['KEYGEN_ACCOUNT_ID']),
@@ -16,29 +15,29 @@
       data=json.dumps({
         "meta": {
           "scope": { "fingerprint": machine_fingerprint },
           "key": license_key
         }
       })
     ).json()
-
+    # print(validation)
     if "errors" in validation:
       errs = validation["errors"]
       raise Exception("license validation failed: {}".format(
         map(lambda e: "{} - {}".format(e["title"], e["detail"]).lower(), errs)
       ))
 
     if validation["meta"]["valid"]:
       print("license has already been activated on this machine")
     
     validation_code = validation["meta"]["code"]
     activation_is_required = validation_code == 'FINGERPRINT_SCOPE_MISMATCH' or \
                              validation_code == 'NO_MACHINES' or \
                              validation_code == 'NO_MACHINE'
-
+    print(validation_code)
     if not activation_is_required:
       raise Exception("license {}".format(validation["meta"]["detail"]))
 
     activation = requests.post(
       "https://api.keygen.sh/v1/accounts/{}/machines".format(os.environ['KEYGEN_ACCOUNT_ID']),
       headers={
         "Authorization": "License {}".format(license_key),
@@ -62,8 +61,7 @@
 
     if "errors" in activation:
       errs = activation["errors"]
       raise Exception("license activation failed: {}".format(
         ','.join(map(lambda e: "{} - {}".format(e["title"], e["detail"]).lower(), errs))
       ))
 
-    # return True, "license activated"
```

### Comparing `licensekeygentest-0.0.2/licensekeygentest.egg-info/PKG-INFO` & `licensekeygentest-0.0.3/licensekeygentest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensekeygentest
-Version: 0.0.2
+Version: 0.0.3
 Summary: POC for keygen authentication
 Author: Rahul R
 Author-email: <rahulranjan25.RR@gmail.com>
 Keywords: python,authentication,licensing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `licensekeygentest-0.0.2/setup.py` & `licensekeygentest-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'POC for keygen authentication'
 LONG_DESCRIPTION = 'A POC package that allows lisencing of python libraries.'
 
 # Setting up
 setup(
     name="licensekeygentest",
     version=VERSION,
```

