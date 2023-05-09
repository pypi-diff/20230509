# Comparing `tmp/mongomancy-0.1.0.tar.gz` & `tmp/mongomancy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongomancy-0.1.0.tar", last modified: Tue May  9 13:06:21 2023, max compression
+gzip compressed data, was "mongomancy-0.1.1.tar", last modified: Tue May  9 13:41:00 2023, max compression
```

## Comparing `mongomancy-0.1.0.tar` & `mongomancy-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:06:21.169779 mongomancy-0.1.0/
--rw-r--r--   0 trval     (1000) trval     (1000)     1296 2023-05-09 13:03:25.000000 mongomancy-0.1.0/CHANGELOG.md
--rw-rw-r--   0 trval     (1000) trval     (1000)     1329 2022-09-02 09:33:19.000000 mongomancy-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 trval     (1000) trval     (1000)     1516 2023-04-04 08:06:59.000000 mongomancy-0.1.0/LICENSE
--rw-r--r--   0 trval     (1000) trval     (1000)       42 2023-04-12 12:30:41.000000 mongomancy-0.1.0/MANIFEST.in
--rw-r--r--   0 trval     (1000) trval     (1000)     4468 2023-05-09 13:06:21.169779 mongomancy-0.1.0/PKG-INFO
--rw-rw-r--   0 trval     (1000) trval     (1000)     3677 2022-09-06 10:07:16.000000 mongomancy-0.1.0/README.md
--rw-r--r--   0 trval     (1000) trval     (1000)     1368 2023-04-12 12:30:41.000000 mongomancy-0.1.0/pyproject.toml
--rw-rw-r--   0 trval     (1000) trval     (1000)       68 2022-09-02 09:38:35.000000 mongomancy-0.1.0/requirements.txt
--rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-05-09 13:06:21.169779 mongomancy-0.1.0/setup.cfg
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:06:21.166446 mongomancy-0.1.0/src/
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:06:21.166446 mongomancy-0.1.0/src/mongomancy/
--rw-r--r--   0 trval     (1000) trval     (1000)      431 2023-05-09 13:03:25.000000 mongomancy-0.1.0/src/mongomancy/__init__.py
--rw-r--r--   0 trval     (1000) trval     (1000)    13920 2023-05-09 13:03:25.000000 mongomancy-0.1.0/src/mongomancy/engine.py
--rw-rw-r--   0 trval     (1000) trval     (1000)      924 2022-08-29 12:44:42.000000 mongomancy-0.1.0/src/mongomancy/mongo_errors.py
--rw-r--r--   0 trval     (1000) trval     (1000)        0 2023-04-12 12:30:41.000000 mongomancy-0.1.0/src/mongomancy/py.typed
--rw-r--r--   0 trval     (1000) trval     (1000)    14168 2023-05-09 13:03:25.000000 mongomancy-0.1.0/src/mongomancy/schema.py
--rw-r--r--   0 trval     (1000) trval     (1000)     5944 2023-05-09 13:03:25.000000 mongomancy-0.1.0/src/mongomancy/types.py
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:06:21.166446 mongomancy-0.1.0/src/mongomancy.egg-info/
--rw-rw-r--   0 trval     (1000) trval     (1000)     4468 2023-05-09 13:06:21.000000 mongomancy-0.1.0/src/mongomancy.egg-info/PKG-INFO
--rw-rw-r--   0 trval     (1000) trval     (1000)      435 2023-05-09 13:06:21.000000 mongomancy-0.1.0/src/mongomancy.egg-info/SOURCES.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)        1 2023-05-09 13:06:21.000000 mongomancy-0.1.0/src/mongomancy.egg-info/dependency_links.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)       13 2023-05-09 13:06:21.000000 mongomancy-0.1.0/src/mongomancy.egg-info/requires.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)       11 2023-05-09 13:06:21.000000 mongomancy-0.1.0/src/mongomancy.egg-info/top_level.txt
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:41:00.173271 mongomancy-0.1.1/
+-rw-r--r--   0 trval     (1000) trval     (1000)     1432 2023-05-09 13:40:27.000000 mongomancy-0.1.1/CHANGELOG.md
+-rw-rw-r--   0 trval     (1000) trval     (1000)     1329 2022-09-02 09:33:19.000000 mongomancy-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 trval     (1000) trval     (1000)     1516 2023-04-04 08:06:59.000000 mongomancy-0.1.1/LICENSE
+-rw-r--r--   0 trval     (1000) trval     (1000)       42 2023-04-12 12:30:41.000000 mongomancy-0.1.1/MANIFEST.in
+-rw-r--r--   0 trval     (1000) trval     (1000)     4468 2023-05-09 13:41:00.173271 mongomancy-0.1.1/PKG-INFO
+-rw-rw-r--   0 trval     (1000) trval     (1000)     3677 2022-09-06 10:07:16.000000 mongomancy-0.1.1/README.md
+-rw-r--r--   0 trval     (1000) trval     (1000)     1368 2023-04-12 12:30:41.000000 mongomancy-0.1.1/pyproject.toml
+-rw-rw-r--   0 trval     (1000) trval     (1000)       68 2022-09-02 09:38:35.000000 mongomancy-0.1.1/requirements.txt
+-rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-05-09 13:41:00.173271 mongomancy-0.1.1/setup.cfg
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:41:00.169937 mongomancy-0.1.1/src/
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:41:00.173271 mongomancy-0.1.1/src/mongomancy/
+-rw-r--r--   0 trval     (1000) trval     (1000)      431 2023-05-09 13:40:27.000000 mongomancy-0.1.1/src/mongomancy/__init__.py
+-rw-r--r--   0 trval     (1000) trval     (1000)    13920 2023-05-09 13:03:25.000000 mongomancy-0.1.1/src/mongomancy/engine.py
+-rw-rw-r--   0 trval     (1000) trval     (1000)      924 2022-08-29 12:44:42.000000 mongomancy-0.1.1/src/mongomancy/mongo_errors.py
+-rw-r--r--   0 trval     (1000) trval     (1000)        0 2023-04-12 12:30:41.000000 mongomancy-0.1.1/src/mongomancy/py.typed
+-rw-r--r--   0 trval     (1000) trval     (1000)    14915 2023-05-09 13:40:27.000000 mongomancy-0.1.1/src/mongomancy/schema.py
+-rw-r--r--   0 trval     (1000) trval     (1000)     5944 2023-05-09 13:03:25.000000 mongomancy-0.1.1/src/mongomancy/types.py
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:41:00.173271 mongomancy-0.1.1/src/mongomancy.egg-info/
+-rw-rw-r--   0 trval     (1000) trval     (1000)     4468 2023-05-09 13:41:00.000000 mongomancy-0.1.1/src/mongomancy.egg-info/PKG-INFO
+-rw-rw-r--   0 trval     (1000) trval     (1000)      435 2023-05-09 13:41:00.000000 mongomancy-0.1.1/src/mongomancy.egg-info/SOURCES.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)        1 2023-05-09 13:41:00.000000 mongomancy-0.1.1/src/mongomancy.egg-info/dependency_links.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)       13 2023-05-09 13:41:00.000000 mongomancy-0.1.1/src/mongomancy.egg-info/requires.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)       11 2023-05-09 13:41:00.000000 mongomancy-0.1.1/src/mongomancy.egg-info/top_level.txt
```

### Comparing `mongomancy-0.1.0/CHANGELOG.md` & `mongomancy-0.1.1/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.1] - 2023-05-09
+
+### Added
+
+- introduced lock wait timeout into `Database` init
+
+### Fixed
+
+- unlock database after first init
+
 ## [0.1.0] - 2023-05-09
 
 ### Added
 
 - mongomancy creates `mongomancy_lock` collection to synchronize db init with master lock record
 - create all now uses multiprocess and thread log
```

### Comparing `mongomancy-0.1.0/CONTRIBUTING.md` & `mongomancy-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.0/LICENSE` & `mongomancy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.0/PKG-INFO` & `mongomancy-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomancy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pymongo based python client with data definition layer.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Ryu-CZ/mongomancy
 Project-URL: Bug Tracker, https://github.com/Ryu-CZ/mongomancy/issues
 Keywords: mongo,python,pymongo,database,nosql
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `mongomancy-0.1.0/README.md` & `mongomancy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.0/pyproject.toml` & `mongomancy-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.0/src/mongomancy/engine.py` & `mongomancy-0.1.1/src/mongomancy/engine.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.0/src/mongomancy/mongo_errors.py` & `mongomancy-0.1.1/src/mongomancy/mongo_errors.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.0/src/mongomancy/schema.py` & `mongomancy-0.1.1/src/mongomancy/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -166,32 +166,40 @@
     topology: List[types.CollectionDefinition]
     _database: pymongo.database.Database
     _collections: Dict[str, Collection]
     mp_semaphore: multiprocessing.Semaphore
     th_semaphore: threading.Semaphore
     logger: LoggerType
     LOCK_COLLECTION: ClassVar[str] = "mongomancy_lock"
+    wait_step: float
+    max_wait: float
 
     __slots__ = (
         "engine",
         "topology",
         "_database",
         "_collections",
         "mp_semaphore",
         "th_semaphore",
         "logger",
+        "wait_step",
+        "max_wait",
     )
 
     def __init__(
         self,
         name: str,
         logger: LoggerType,
         engine: types.Executor,
         *collections: types.CollectionDefinition,
+        wait_step: float = 7,
+        max_wait: float = 90,
     ) -> None:
+        self.max_wait = max_wait
+        self.wait_step = wait_step
         self.mp_semaphore = multiprocessing.Semaphore()
         self.th_semaphore = threading.Semaphore()
         self._collections = {}
         self.topology = []
         self.logger = logger
         self.engine = engine
         self._database = engine.get_database(name)
@@ -248,50 +256,64 @@
         Add new collection definitions into `self.topology`.
 
         :param new_definitions: add the collection definition
         """
         self.topology.append(new_definitions)
 
     def _lock(self) -> bool:
+        """
+        Try to acquire lock or return false
+        :returns: lock acquired
+        """
         self.create_collection(define_lock_collection(self.LOCK_COLLECTION))
         doc = self.engine.find_one_and_update(
             self._database[self.LOCK_COLLECTION],
             where={"_id": "master", "locked": False},
             changes={"$set": {"locked": True}},
         )
         if not doc:
             return False
         return not bool(doc.get("locked"))
 
     def _unlock(self):
+        """
+        Update master lock to unlock state.
+        """
         self.engine.find_one_and_update(
-            self._database[self.LOCK_COLLECTION],
+            self._database.client.c[self.LOCK_COLLECTION],
             where={"_id": "master"},
             changes={"$set": {"locked": False}},
             upsert=True,
         )
 
     def create_all(self, skip_existing: bool = True) -> None:
         """
         Create all collections if not exists. Loads `self._collections` for use.
 
         :param skip_existing: skip collection init if collection already exists in db
         """
         with self.mp_semaphore:
             with self.th_semaphore:
-                if not self._lock():
-                    self.logger.debug("database is locked - this process or thread is skipping 'Database.create_all'")
-                    return
+                wait_time = 0
+                while not self._lock():
+                    self.logger.debug(f"create_all - process or thread is waiting for master lock {wait_time}sec")
+                    time.sleep(self.wait_step)
+                    wait_time += self.wait_step
+                    if wait_time > self.max_wait:
+                        self.logger.warning(f"create_all - wait timeout after {wait_time}sec and stops waiting")
+                        self._unlock()
+                        break
                 try:
                     for collection_definition in self.topology:
                         _ = self.create_collection(collection_definition, skip_existing)
                 except (Exception, KeyError, IndexError, IOError) as e:
                     self.logger.error(f"create_all failed on {e}")
                     self._unlock()
                     raise e from e
+                self._unlock()
 
     def create_collection(
         self,
         definition: types.CollectionDefinition,
         skip_existing: bool = True,
     ) -> Collection:
         """
```

### Comparing `mongomancy-0.1.0/src/mongomancy/types.py` & `mongomancy-0.1.1/src/mongomancy/types.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.0/src/mongomancy.egg-info/PKG-INFO` & `mongomancy-0.1.1/src/mongomancy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomancy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pymongo based python client with data definition layer.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Ryu-CZ/mongomancy
 Project-URL: Bug Tracker, https://github.com/Ryu-CZ/mongomancy/issues
 Keywords: mongo,python,pymongo,database,nosql
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

