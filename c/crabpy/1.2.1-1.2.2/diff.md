# Comparing `tmp/crabpy-1.2.1.tar.gz` & `tmp/crabpy-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crabpy-1.2.1.tar", last modified: Thu May  4 13:36:33 2023, max compression
+gzip compressed data, was "crabpy-1.2.2.tar", last modified: Tue May  9 05:25:35 2023, max compression
```

## Comparing `crabpy-1.2.1.tar` & `crabpy-1.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-04 13:36:33.274009 crabpy-1.2.1/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6641 2023-05-04 13:36:14.000000 crabpy-1.2.1/CHANGES.rst
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 12:57:29.000000 crabpy-1.2.1/LICENSE
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       76 2023-04-13 12:57:29.000000 crabpy-1.2.1/MANIFEST.in
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     8292 2023-05-04 13:36:33.274009 crabpy-1.2.1/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      941 2023-04-13 12:57:29.000000 crabpy-1.2.1/README.rst
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-04 13:36:33.270009 crabpy-1.2.1/crabpy/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.2.1/crabpy/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7372 2023-04-13 12:57:29.000000 crabpy-1.2.1/crabpy/client.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-04 13:36:33.274009 crabpy-1.2.1/crabpy/data/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)   238209 2023-05-03 12:29:06.000000 crabpy-1.2.1/crabpy/data/deelgemeenten.json
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)   167480 2023-05-03 12:29:06.000000 crabpy-1.2.1/crabpy/data/gemeenten.json
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      547 2023-05-03 12:29:06.000000 crabpy-1.2.1/crabpy/data/gewesten.json
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      803 2023-05-04 09:43:10.000000 crabpy-1.2.1/crabpy/data/provincies.json
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-04 13:36:33.274009 crabpy-1.2.1/crabpy/gateway/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.2.1/crabpy/gateway/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    30229 2023-05-04 13:36:14.000000 crabpy-1.2.1/crabpy/gateway/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    28420 2023-04-13 12:57:29.000000 crabpy-1.2.1/crabpy/gateway/capakey.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    85501 2023-04-13 12:57:29.000000 crabpy-1.2.1/crabpy/gateway/crab.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      991 2023-04-13 12:57:29.000000 crabpy-1.2.1/crabpy/gateway/exception.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1083 2023-04-13 12:57:29.000000 crabpy-1.2.1/crabpy/wsa.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2719 2023-04-13 12:57:29.000000 crabpy-1.2.1/crabpy/wsse.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-04 13:36:33.274009 crabpy-1.2.1/crabpy.egg-info/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     8292 2023-05-04 13:36:33.000000 crabpy-1.2.1/crabpy.egg-info/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      578 2023-05-04 13:36:33.000000 crabpy-1.2.1/crabpy.egg-info/SOURCES.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-05-04 13:36:33.000000 crabpy-1.2.1/crabpy.egg-info/dependency_links.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-05-04 13:36:33.000000 crabpy-1.2.1/crabpy.egg-info/entry_points.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 12:57:59.000000 crabpy-1.2.1/crabpy.egg-info/not-zip-safe
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       41 2023-05-04 13:36:33.000000 crabpy-1.2.1/crabpy.egg-info/requires.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        7 2023-05-04 13:36:33.000000 crabpy-1.2.1/crabpy.egg-info/top_level.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       38 2023-05-04 13:36:33.274009 crabpy-1.2.1/setup.cfg
--rwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)     1278 2023-05-04 13:36:14.000000 crabpy-1.2.1/setup.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-09 05:25:35.587619 crabpy-1.2.2/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6711 2023-05-09 05:25:15.000000 crabpy-1.2.2/CHANGES.rst
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 12:57:29.000000 crabpy-1.2.2/LICENSE
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       76 2023-04-13 12:57:29.000000 crabpy-1.2.2/MANIFEST.in
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     8362 2023-05-09 05:25:35.587619 crabpy-1.2.2/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      941 2023-04-13 12:57:29.000000 crabpy-1.2.2/README.rst
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-09 05:25:35.587619 crabpy-1.2.2/crabpy/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.2.2/crabpy/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7379 2023-05-09 05:25:15.000000 crabpy-1.2.2/crabpy/client.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-09 05:25:35.587619 crabpy-1.2.2/crabpy/data/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)   238209 2023-05-03 12:29:06.000000 crabpy-1.2.2/crabpy/data/deelgemeenten.json
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)   167480 2023-05-03 12:29:06.000000 crabpy-1.2.2/crabpy/data/gemeenten.json
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      547 2023-05-03 12:29:06.000000 crabpy-1.2.2/crabpy/data/gewesten.json
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      803 2023-05-04 09:43:10.000000 crabpy-1.2.2/crabpy/data/provincies.json
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-09 05:25:35.587619 crabpy-1.2.2/crabpy/gateway/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.2.2/crabpy/gateway/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    30229 2023-05-04 13:36:14.000000 crabpy-1.2.2/crabpy/gateway/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    28420 2023-04-13 12:57:29.000000 crabpy-1.2.2/crabpy/gateway/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    85501 2023-04-13 12:57:29.000000 crabpy-1.2.2/crabpy/gateway/crab.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      991 2023-04-13 12:57:29.000000 crabpy-1.2.2/crabpy/gateway/exception.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1083 2023-04-13 12:57:29.000000 crabpy-1.2.2/crabpy/wsa.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2719 2023-04-13 12:57:29.000000 crabpy-1.2.2/crabpy/wsse.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-09 05:25:35.587619 crabpy-1.2.2/crabpy.egg-info/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     8362 2023-05-09 05:25:35.000000 crabpy-1.2.2/crabpy.egg-info/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      578 2023-05-09 05:25:35.000000 crabpy-1.2.2/crabpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-05-09 05:25:35.000000 crabpy-1.2.2/crabpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-05-09 05:25:35.000000 crabpy-1.2.2/crabpy.egg-info/entry_points.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 12:57:59.000000 crabpy-1.2.2/crabpy.egg-info/not-zip-safe
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       41 2023-05-09 05:25:35.000000 crabpy-1.2.2/crabpy.egg-info/requires.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        7 2023-05-09 05:25:35.000000 crabpy-1.2.2/crabpy.egg-info/top_level.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       38 2023-05-09 05:25:35.587619 crabpy-1.2.2/setup.cfg
+-rwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)     1278 2023-05-09 05:25:15.000000 crabpy-1.2.2/setup.py
```

### Comparing `crabpy-1.2.1/CHANGES.rst` & `crabpy-1.2.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+1.2.2 (09-05-2023)
+------------------
+
+- get percelen timeout (#217)
+
 1.2.1 (04-05-2023)
 ------------------
 
 - Adressenregister bugfixes
 
 1.2.0 (04-05-2023)
 ------------------
```

### Comparing `crabpy-1.2.1/LICENSE` & `crabpy-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.1/PKG-INFO` & `crabpy-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crabpy
-Version: 1.2.1
+Version: 1.2.2
 Summary: Interact with geographical webservices by Informatie Vlaanderen.
 Home-page: http://github.com/onroerenderfgoed/crabpy
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,19 @@
         :target: https://travis-ci.org/OnroerendErfgoed/crabpy
 .. image:: https://coveralls.io/repos/OnroerendErfgoed/crabpy/badge.png?branch=master
         :target: https://coveralls.io/r/OnroerendErfgoed/crabpy?branch=master
 .. image:: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/badges/quality-score.png?b=master
         :target: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/?branch=master
 
 
+1.2.2 (09-05-2023)
+------------------
+
+- get percelen timeout (#217)
+
 1.2.1 (04-05-2023)
 ------------------
 
 - Adressenregister bugfixes
 
 1.2.0 (04-05-2023)
 ------------------
```

### Comparing `crabpy-1.2.1/README.rst` & `crabpy-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.1/crabpy/client.py` & `crabpy-1.2.2/crabpy/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
     def get_gemeenten(self, gemeentenaam=None, status=None):
         params = {}
         if gemeentenaam is not None:
             params["gemeentenaam"] = gemeentenaam
         if status is not None:
             params["status"] = status
-        return self._get_list("/v2/gemeenten", "gemeenten", params)
+        return self._get_list("/v2/gemeenten", "gemeenten", params=params)
 
     def get_postinfo(self, postinfo_id):
         return self._get(f"/v2/postinfo/{postinfo_id}")
 
     def get_postinfos(self, gemeentenaam=None, postnaam=None):
         params = {}
         if gemeentenaam is not None:
@@ -201,15 +201,15 @@
         return self._get(f"/v2/percelen/{perceel_id}")
 
     def get_percelen(self, status=None, adresObjectId=None):
         params = {}
         if status is not None:
             params["status"] = status
         if adresObjectId is not None:
-            params["adresOjbectId"] = adresObjectId
+            params["adresObjectId"] = adresObjectId
         return self._get_list("/v2/percelen", "percelen", params=params)
 
     def get_gebouw(self, gebouw_id):
         return self._get(f"/v2/gebouwen/{gebouw_id}")
 
     def get_gebouwen(self, status=None):
         params = {}
```

### Comparing `crabpy-1.2.1/crabpy/data/deelgemeenten.json` & `crabpy-1.2.2/crabpy/data/deelgemeenten.json`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.1/crabpy/data/gemeenten.json` & `crabpy-1.2.2/crabpy/data/gemeenten.json`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.1/crabpy/data/gewesten.json` & `crabpy-1.2.2/crabpy/data/gewesten.json`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.1/crabpy/data/provincies.json` & `crabpy-1.2.2/crabpy/data/provincies.json`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.1/crabpy/gateway/adressenregister.py` & `crabpy-1.2.2/crabpy/gateway/adressenregister.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.1/crabpy/gateway/capakey.py` & `crabpy-1.2.2/crabpy/gateway/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.1/crabpy/gateway/crab.py` & `crabpy-1.2.2/crabpy/gateway/crab.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.1/crabpy/gateway/exception.py` & `crabpy-1.2.2/crabpy/gateway/exception.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.1/crabpy/wsa.py` & `crabpy-1.2.2/crabpy/wsa.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.1/crabpy/wsse.py` & `crabpy-1.2.2/crabpy/wsse.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.1/crabpy.egg-info/PKG-INFO` & `crabpy-1.2.2/crabpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crabpy
-Version: 1.2.1
+Version: 1.2.2
 Summary: Interact with geographical webservices by Informatie Vlaanderen.
 Home-page: http://github.com/onroerenderfgoed/crabpy
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,19 @@
         :target: https://travis-ci.org/OnroerendErfgoed/crabpy
 .. image:: https://coveralls.io/repos/OnroerendErfgoed/crabpy/badge.png?branch=master
         :target: https://coveralls.io/r/OnroerendErfgoed/crabpy?branch=master
 .. image:: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/badges/quality-score.png?b=master
         :target: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/?branch=master
 
 
+1.2.2 (09-05-2023)
+------------------
+
+- get percelen timeout (#217)
+
 1.2.1 (04-05-2023)
 ------------------
 
 - Adressenregister bugfixes
 
 1.2.0 (04-05-2023)
 ------------------
```

### Comparing `crabpy-1.2.1/crabpy.egg-info/SOURCES.txt` & `crabpy-1.2.2/crabpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.1/setup.py` & `crabpy-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "crabpy",
 ]
 
 requires = ["suds-py3>=1.4.4.1", "dogpile.cache", "requests"]
 
 setup(
     name="crabpy",
-    version="1.2.1",
+    version="1.2.2",
     description="Interact with geographical webservices by Informatie Vlaanderen.",
     long_description=open("README.rst").read() + "\n\n" + open("CHANGES.rst").read(),
     author="Onroerend Erfgoed",
     author_email="ict@onroerenderfgoed.be",
     url="http://github.com/onroerenderfgoed/crabpy",
     packages=find_packages(exclude=["tests*"]),
     package_data={"": ["LICENSE"]},
```

