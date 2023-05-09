# Comparing `tmp/licensekeygentest-0.0.1.tar.gz` & `tmp/licensekeygentest-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "licensekeygentest-0.0.1.tar", last modified: Mon May  8 15:06:12 2023, max compression
+gzip compressed data, was "licensekeygentest-0.0.2.tar", last modified: Tue May  9 08:25:50 2023, max compression
```

## Comparing `licensekeygentest-0.0.1.tar` & `licensekeygentest-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-08 15:06:12.213749 licensekeygentest-0.0.1/
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1063 2023-05-08 14:20:18.000000 licensekeygentest-0.0.1/LICENSE
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      574 2023-05-08 15:06:12.213749 licensekeygentest-0.0.1/PKG-INFO
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       30 2023-05-08 15:05:37.000000 licensekeygentest-0.0.1/README.md
-drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-08 15:06:12.209749 licensekeygentest-0.0.1/licensekeygentest/
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       43 2023-05-08 13:59:31.000000 licensekeygentest-0.0.1/licensekeygentest/__init__.py
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     2220 2023-05-08 14:14:48.000000 licensekeygentest-0.0.1/licensekeygentest/main.py
-drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-08 15:06:12.209749 licensekeygentest-0.0.1/licensekeygentest.egg-info/
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      574 2023-05-08 15:06:12.000000 licensekeygentest-0.0.1/licensekeygentest.egg-info/PKG-INFO
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      286 2023-05-08 15:06:12.000000 licensekeygentest-0.0.1/licensekeygentest.egg-info/SOURCES.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)        1 2023-05-08 15:06:12.000000 licensekeygentest-0.0.1/licensekeygentest.egg-info/dependency_links.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       22 2023-05-08 15:06:12.000000 licensekeygentest-0.0.1/licensekeygentest.egg-info/requires.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       18 2023-05-08 15:06:12.000000 licensekeygentest-0.0.1/licensekeygentest.egg-info/top_level.txt
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       38 2023-05-08 15:06:12.213749 licensekeygentest-0.0.1/setup.cfg
--rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1074 2023-05-08 15:03:53.000000 licensekeygentest-0.0.1/setup.py
+drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 08:25:50.613454 licensekeygentest-0.0.2/
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1063 2023-05-08 14:20:18.000000 licensekeygentest-0.0.2/LICENSE
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      574 2023-05-09 08:25:50.613454 licensekeygentest-0.0.2/PKG-INFO
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       30 2023-05-08 15:05:37.000000 licensekeygentest-0.0.2/README.md
+drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 08:25:50.613454 licensekeygentest-0.0.2/licensekeygentest/
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       43 2023-05-08 13:59:31.000000 licensekeygentest-0.0.2/licensekeygentest/__init__.py
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     2225 2023-05-09 08:21:05.000000 licensekeygentest-0.0.2/licensekeygentest/main.py
+drwxrwxr-x   0 jaspercyan  (1000) jaspercyan  (1000)        0 2023-05-09 08:25:50.613454 licensekeygentest-0.0.2/licensekeygentest.egg-info/
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      574 2023-05-09 08:25:50.000000 licensekeygentest-0.0.2/licensekeygentest.egg-info/PKG-INFO
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)      286 2023-05-09 08:25:50.000000 licensekeygentest-0.0.2/licensekeygentest.egg-info/SOURCES.txt
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)        1 2023-05-09 08:25:50.000000 licensekeygentest-0.0.2/licensekeygentest.egg-info/dependency_links.txt
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       22 2023-05-09 08:25:50.000000 licensekeygentest-0.0.2/licensekeygentest.egg-info/requires.txt
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       18 2023-05-09 08:25:50.000000 licensekeygentest-0.0.2/licensekeygentest.egg-info/top_level.txt
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)       38 2023-05-09 08:25:50.613454 licensekeygentest-0.0.2/setup.cfg
+-rw-rw-r--   0 jaspercyan  (1000) jaspercyan  (1000)     1074 2023-05-09 08:23:20.000000 licensekeygentest-0.0.2/setup.py
```

### Comparing `licensekeygentest-0.0.1/LICENSE` & `licensekeygentest-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `licensekeygentest-0.0.1/PKG-INFO` & `licensekeygentest-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensekeygentest
-Version: 0.0.1
+Version: 0.0.2
 Summary: POC for keygen authentication
 Author: Rahul R
 Author-email: <rahulranjan25.RR@gmail.com>
 Keywords: python,authentication,licensing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `licensekeygentest-0.0.1/licensekeygentest/main.py` & `licensekeygentest-0.0.2/licensekeygentest/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,28 +19,28 @@
           "key": license_key
         }
       })
     ).json()
 
     if "errors" in validation:
       errs = validation["errors"]
-      return False, "license validation failed: {}".format(
+      raise Exception("license validation failed: {}".format(
         map(lambda e: "{} - {}".format(e["title"], e["detail"]).lower(), errs)
-      )
+      ))
 
     if validation["meta"]["valid"]:
-      return True, "license has already been activated on this machine"
+      print("license has already been activated on this machine")
     
     validation_code = validation["meta"]["code"]
     activation_is_required = validation_code == 'FINGERPRINT_SCOPE_MISMATCH' or \
                              validation_code == 'NO_MACHINES' or \
                              validation_code == 'NO_MACHINE'
 
     if not activation_is_required:
-      return False, "license {}".format(validation["meta"]["detail"])
+      raise Exception("license {}".format(validation["meta"]["detail"]))
 
     activation = requests.post(
       "https://api.keygen.sh/v1/accounts/{}/machines".format(os.environ['KEYGEN_ACCOUNT_ID']),
       headers={
         "Authorization": "License {}".format(license_key),
         "Content-Type": "application/vnd.api+json",
         "Accept": "application/vnd.api+json"
@@ -58,12 +58,12 @@
           }
         }
       })
     ).json()
 
     if "errors" in activation:
       errs = activation["errors"]
-      return False, "license activation failed: {}".format(
+      raise Exception("license activation failed: {}".format(
         ','.join(map(lambda e: "{} - {}".format(e["title"], e["detail"]).lower(), errs))
-      )
+      ))
 
-    return True, "license activated"
+    # return True, "license activated"
```

### Comparing `licensekeygentest-0.0.1/licensekeygentest.egg-info/PKG-INFO` & `licensekeygentest-0.0.2/licensekeygentest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensekeygentest
-Version: 0.0.1
+Version: 0.0.2
 Summary: POC for keygen authentication
 Author: Rahul R
 Author-email: <rahulranjan25.RR@gmail.com>
 Keywords: python,authentication,licensing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `licensekeygentest-0.0.1/setup.py` & `licensekeygentest-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'POC for keygen authentication'
 LONG_DESCRIPTION = 'A POC package that allows lisencing of python libraries.'
 
 # Setting up
 setup(
     name="licensekeygentest",
     version=VERSION,
```

