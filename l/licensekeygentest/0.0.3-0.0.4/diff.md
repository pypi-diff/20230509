# Comparing `tmp/licensekeygentest-0.0.3.tar.gz` & `tmp/licensekeygentest-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "licensekeygentest-0.0.3.tar", last modified: Tue May  9 09:17:16 2023, max compression
+gzip compressed data, was "licensekeygentest-0.0.4.tar", last modified: Tue May  9 09:23:26 2023, max compression
```

## Comparing `licensekeygentest-0.0.3.tar` & `licensekeygentest-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 09:17:16.431305 licensekeygentest-0.0.3/
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1063 2023-05-08 14:20:18.000000 licensekeygentest-0.0.3/LICENSE
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      574 2023-05-09 09:17:16.431305 licensekeygentest-0.0.3/PKG-INFO
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       30 2023-05-08 15:05:37.000000 licensekeygentest-0.0.3/README.md
-drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 09:17:16.427305 licensekeygentest-0.0.3/licensekeygentest/
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       43 2023-05-08 13:59:31.000000 licensekeygentest-0.0.3/licensekeygentest/__init__.py
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     2225 2023-05-09 09:11:39.000000 licensekeygentest-0.0.3/licensekeygentest/main.py
-drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 09:17:16.431305 licensekeygentest-0.0.3/licensekeygentest.egg-info/
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      574 2023-05-09 09:17:16.000000 licensekeygentest-0.0.3/licensekeygentest.egg-info/PKG-INFO
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      286 2023-05-09 09:17:16.000000 licensekeygentest-0.0.3/licensekeygentest.egg-info/SOURCES.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)        1 2023-05-09 09:17:16.000000 licensekeygentest-0.0.3/licensekeygentest.egg-info/dependency_links.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       22 2023-05-09 09:17:16.000000 licensekeygentest-0.0.3/licensekeygentest.egg-info/requires.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       18 2023-05-09 09:17:16.000000 licensekeygentest-0.0.3/licensekeygentest.egg-info/top_level.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       38 2023-05-09 09:17:16.431305 licensekeygentest-0.0.3/setup.cfg
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1074 2023-05-09 09:16:42.000000 licensekeygentest-0.0.3/setup.py
+drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 09:23:26.163446 licensekeygentest-0.0.4/
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1063 2023-05-08 14:20:18.000000 licensekeygentest-0.0.4/LICENSE
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      636 2023-05-09 09:23:26.163446 licensekeygentest-0.0.4/PKG-INFO
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       92 2023-05-09 09:18:34.000000 licensekeygentest-0.0.4/README.md
+drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 09:23:26.159446 licensekeygentest-0.0.4/licensekeygentest/
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       43 2023-05-08 13:59:31.000000 licensekeygentest-0.0.4/licensekeygentest/__init__.py
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     2191 2023-05-09 09:22:40.000000 licensekeygentest-0.0.4/licensekeygentest/main.py
+drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 09:23:26.163446 licensekeygentest-0.0.4/licensekeygentest.egg-info/
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      636 2023-05-09 09:23:26.000000 licensekeygentest-0.0.4/licensekeygentest.egg-info/PKG-INFO
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      286 2023-05-09 09:23:26.000000 licensekeygentest-0.0.4/licensekeygentest.egg-info/SOURCES.txt
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)        1 2023-05-09 09:23:26.000000 licensekeygentest-0.0.4/licensekeygentest.egg-info/dependency_links.txt
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       22 2023-05-09 09:23:26.000000 licensekeygentest-0.0.4/licensekeygentest.egg-info/requires.txt
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       18 2023-05-09 09:23:26.000000 licensekeygentest-0.0.4/licensekeygentest.egg-info/top_level.txt
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       38 2023-05-09 09:23:26.163446 licensekeygentest-0.0.4/setup.cfg
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1074 2023-05-09 09:23:15.000000 licensekeygentest-0.0.4/setup.py
```

### Comparing `licensekeygentest-0.0.3/LICENSE` & `licensekeygentest-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `licensekeygentest-0.0.3/PKG-INFO` & `licensekeygentest-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensekeygentest
-Version: 0.0.3
+Version: 0.0.4
 Summary: POC for keygen authentication
 Author: Rahul R
 Author-email: <rahulranjan25.RR@gmail.com>
 Keywords: python,authentication,licensing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,7 +12,10 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Licensed Library KeyGen test
+
+This is test environment for lisenced libraries over PyPi.
+
```

### Comparing `licensekeygentest-0.0.3/licensekeygentest/main.py` & `licensekeygentest-0.0.4/licensekeygentest/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
       data=json.dumps({
         "meta": {
           "scope": { "fingerprint": machine_fingerprint },
           "key": license_key
         }
       })
     ).json()
-    # print(validation)
     if "errors" in validation:
       errs = validation["errors"]
       raise Exception("license validation failed: {}".format(
         map(lambda e: "{} - {}".format(e["title"], e["detail"]).lower(), errs)
       ))
 
     if validation["meta"]["valid"]:
@@ -31,15 +30,15 @@
     
     validation_code = validation["meta"]["code"]
     activation_is_required = validation_code == 'FINGERPRINT_SCOPE_MISMATCH' or \
                              validation_code == 'NO_MACHINES' or \
                              validation_code == 'NO_MACHINE'
     print(validation_code)
     if not activation_is_required:
-      raise Exception("license {}".format(validation["meta"]["detail"]))
+      print("license {}".format(validation["meta"]["detail"]))
 
     activation = requests.post(
       "https://api.keygen.sh/v1/accounts/{}/machines".format(os.environ['KEYGEN_ACCOUNT_ID']),
       headers={
         "Authorization": "License {}".format(license_key),
         "Content-Type": "application/vnd.api+json",
         "Accept": "application/vnd.api+json"
```

### Comparing `licensekeygentest-0.0.3/licensekeygentest.egg-info/PKG-INFO` & `licensekeygentest-0.0.4/licensekeygentest.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensekeygentest
-Version: 0.0.3
+Version: 0.0.4
 Summary: POC for keygen authentication
 Author: Rahul R
 Author-email: <rahulranjan25.RR@gmail.com>
 Keywords: python,authentication,licensing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,7 +12,10 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Licensed Library KeyGen test
+
+This is test environment for lisenced libraries over PyPi.
+
```

### Comparing `licensekeygentest-0.0.3/setup.py` & `licensekeygentest-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'POC for keygen authentication'
 LONG_DESCRIPTION = 'A POC package that allows lisencing of python libraries.'
 
 # Setting up
 setup(
     name="licensekeygentest",
     version=VERSION,
```

