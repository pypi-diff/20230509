# Comparing `tmp/mongomancy-0.1.1.tar.gz` & `tmp/mongomancy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongomancy-0.1.1.tar", last modified: Tue May  9 13:41:00 2023, max compression
+gzip compressed data, was "mongomancy-0.1.2.tar", last modified: Tue May  9 13:58:19 2023, max compression
```

## Comparing `mongomancy-0.1.1.tar` & `mongomancy-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:41:00.173271 mongomancy-0.1.1/
--rw-r--r--   0 trval     (1000) trval     (1000)     1432 2023-05-09 13:40:27.000000 mongomancy-0.1.1/CHANGELOG.md
--rw-rw-r--   0 trval     (1000) trval     (1000)     1329 2022-09-02 09:33:19.000000 mongomancy-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 trval     (1000) trval     (1000)     1516 2023-04-04 08:06:59.000000 mongomancy-0.1.1/LICENSE
--rw-r--r--   0 trval     (1000) trval     (1000)       42 2023-04-12 12:30:41.000000 mongomancy-0.1.1/MANIFEST.in
--rw-r--r--   0 trval     (1000) trval     (1000)     4468 2023-05-09 13:41:00.173271 mongomancy-0.1.1/PKG-INFO
--rw-rw-r--   0 trval     (1000) trval     (1000)     3677 2022-09-06 10:07:16.000000 mongomancy-0.1.1/README.md
--rw-r--r--   0 trval     (1000) trval     (1000)     1368 2023-04-12 12:30:41.000000 mongomancy-0.1.1/pyproject.toml
--rw-rw-r--   0 trval     (1000) trval     (1000)       68 2022-09-02 09:38:35.000000 mongomancy-0.1.1/requirements.txt
--rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-05-09 13:41:00.173271 mongomancy-0.1.1/setup.cfg
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:41:00.169937 mongomancy-0.1.1/src/
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:41:00.173271 mongomancy-0.1.1/src/mongomancy/
--rw-r--r--   0 trval     (1000) trval     (1000)      431 2023-05-09 13:40:27.000000 mongomancy-0.1.1/src/mongomancy/__init__.py
--rw-r--r--   0 trval     (1000) trval     (1000)    13920 2023-05-09 13:03:25.000000 mongomancy-0.1.1/src/mongomancy/engine.py
--rw-rw-r--   0 trval     (1000) trval     (1000)      924 2022-08-29 12:44:42.000000 mongomancy-0.1.1/src/mongomancy/mongo_errors.py
--rw-r--r--   0 trval     (1000) trval     (1000)        0 2023-04-12 12:30:41.000000 mongomancy-0.1.1/src/mongomancy/py.typed
--rw-r--r--   0 trval     (1000) trval     (1000)    14915 2023-05-09 13:40:27.000000 mongomancy-0.1.1/src/mongomancy/schema.py
--rw-r--r--   0 trval     (1000) trval     (1000)     5944 2023-05-09 13:03:25.000000 mongomancy-0.1.1/src/mongomancy/types.py
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:41:00.173271 mongomancy-0.1.1/src/mongomancy.egg-info/
--rw-rw-r--   0 trval     (1000) trval     (1000)     4468 2023-05-09 13:41:00.000000 mongomancy-0.1.1/src/mongomancy.egg-info/PKG-INFO
--rw-rw-r--   0 trval     (1000) trval     (1000)      435 2023-05-09 13:41:00.000000 mongomancy-0.1.1/src/mongomancy.egg-info/SOURCES.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)        1 2023-05-09 13:41:00.000000 mongomancy-0.1.1/src/mongomancy.egg-info/dependency_links.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)       13 2023-05-09 13:41:00.000000 mongomancy-0.1.1/src/mongomancy.egg-info/requires.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)       11 2023-05-09 13:41:00.000000 mongomancy-0.1.1/src/mongomancy.egg-info/top_level.txt
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:58:19.575607 mongomancy-0.1.2/
+-rw-r--r--   0 trval     (1000) trval     (1000)     1500 2023-05-09 13:57:53.000000 mongomancy-0.1.2/CHANGELOG.md
+-rw-rw-r--   0 trval     (1000) trval     (1000)     1329 2022-09-02 09:33:19.000000 mongomancy-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 trval     (1000) trval     (1000)     1516 2023-04-04 08:06:59.000000 mongomancy-0.1.2/LICENSE
+-rw-r--r--   0 trval     (1000) trval     (1000)       42 2023-04-12 12:30:41.000000 mongomancy-0.1.2/MANIFEST.in
+-rw-r--r--   0 trval     (1000) trval     (1000)     4468 2023-05-09 13:58:19.575607 mongomancy-0.1.2/PKG-INFO
+-rw-rw-r--   0 trval     (1000) trval     (1000)     3677 2022-09-06 10:07:16.000000 mongomancy-0.1.2/README.md
+-rw-r--r--   0 trval     (1000) trval     (1000)     1368 2023-04-12 12:30:41.000000 mongomancy-0.1.2/pyproject.toml
+-rw-rw-r--   0 trval     (1000) trval     (1000)       68 2022-09-02 09:38:35.000000 mongomancy-0.1.2/requirements.txt
+-rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-05-09 13:58:19.575607 mongomancy-0.1.2/setup.cfg
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:58:19.572274 mongomancy-0.1.2/src/
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:58:19.575607 mongomancy-0.1.2/src/mongomancy/
+-rw-r--r--   0 trval     (1000) trval     (1000)      431 2023-05-09 13:57:53.000000 mongomancy-0.1.2/src/mongomancy/__init__.py
+-rw-r--r--   0 trval     (1000) trval     (1000)    13920 2023-05-09 13:03:25.000000 mongomancy-0.1.2/src/mongomancy/engine.py
+-rw-rw-r--   0 trval     (1000) trval     (1000)      924 2022-08-29 12:44:42.000000 mongomancy-0.1.2/src/mongomancy/mongo_errors.py
+-rw-r--r--   0 trval     (1000) trval     (1000)        0 2023-04-12 12:30:41.000000 mongomancy-0.1.2/src/mongomancy/py.typed
+-rw-r--r--   0 trval     (1000) trval     (1000)    14906 2023-05-09 13:50:56.000000 mongomancy-0.1.2/src/mongomancy/schema.py
+-rw-r--r--   0 trval     (1000) trval     (1000)     5944 2023-05-09 13:03:25.000000 mongomancy-0.1.2/src/mongomancy/types.py
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:58:19.575607 mongomancy-0.1.2/src/mongomancy.egg-info/
+-rw-rw-r--   0 trval     (1000) trval     (1000)     4468 2023-05-09 13:58:19.000000 mongomancy-0.1.2/src/mongomancy.egg-info/PKG-INFO
+-rw-rw-r--   0 trval     (1000) trval     (1000)      435 2023-05-09 13:58:19.000000 mongomancy-0.1.2/src/mongomancy.egg-info/SOURCES.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)        1 2023-05-09 13:58:19.000000 mongomancy-0.1.2/src/mongomancy.egg-info/dependency_links.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)       13 2023-05-09 13:58:19.000000 mongomancy-0.1.2/src/mongomancy.egg-info/requires.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)       11 2023-05-09 13:58:19.000000 mongomancy-0.1.2/src/mongomancy.egg-info/top_level.txt
```

### Comparing `mongomancy-0.1.1/CHANGELOG.md` & `mongomancy-0.1.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.2] - 2023-05-09
+
+### Fixed
+
+- unlock called bad collection
+
 ## [0.1.1] - 2023-05-09
 
 ### Added
 
 - introduced lock wait timeout into `Database` init
 
 ### Fixed
```

### Comparing `mongomancy-0.1.1/CONTRIBUTING.md` & `mongomancy-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.1/LICENSE` & `mongomancy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.1/PKG-INFO` & `mongomancy-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomancy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pymongo based python client with data definition layer.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Ryu-CZ/mongomancy
 Project-URL: Bug Tracker, https://github.com/Ryu-CZ/mongomancy/issues
 Keywords: mongo,python,pymongo,database,nosql
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `mongomancy-0.1.1/README.md` & `mongomancy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.1/pyproject.toml` & `mongomancy-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.1/src/mongomancy/engine.py` & `mongomancy-0.1.2/src/mongomancy/engine.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.1/src/mongomancy/mongo_errors.py` & `mongomancy-0.1.2/src/mongomancy/mongo_errors.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.1/src/mongomancy/schema.py` & `mongomancy-0.1.2/src/mongomancy/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,15 @@
         return not bool(doc.get("locked"))
 
     def _unlock(self):
         """
         Update master lock to unlock state.
         """
         self.engine.find_one_and_update(
-            self._database.client.c[self.LOCK_COLLECTION],
+            self._database[self.LOCK_COLLECTION],
             where={"_id": "master"},
             changes={"$set": {"locked": False}},
             upsert=True,
         )
 
     def create_all(self, skip_existing: bool = True) -> None:
         """
```

### Comparing `mongomancy-0.1.1/src/mongomancy/types.py` & `mongomancy-0.1.2/src/mongomancy/types.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.1/src/mongomancy.egg-info/PKG-INFO` & `mongomancy-0.1.2/src/mongomancy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomancy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pymongo based python client with data definition layer.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Ryu-CZ/mongomancy
 Project-URL: Bug Tracker, https://github.com/Ryu-CZ/mongomancy/issues
 Keywords: mongo,python,pymongo,database,nosql
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

