# Comparing `tmp/mongomancy-0.0.6.tar.gz` & `tmp/mongomancy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongomancy-0.0.6.tar", last modified: Thu Apr 13 12:07:23 2023, max compression
+gzip compressed data, was "mongomancy-0.1.0.tar", last modified: Tue May  9 13:06:21 2023, max compression
```

## Comparing `mongomancy-0.0.6.tar` & `mongomancy-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-13 12:07:23.179283 mongomancy-0.0.6/
--rw-r--r--   0 trval     (1000) trval     (1000)     1112 2023-04-13 12:06:01.000000 mongomancy-0.0.6/CHANGELOG.md
--rw-rw-r--   0 trval     (1000) trval     (1000)     1329 2022-09-02 09:33:19.000000 mongomancy-0.0.6/CONTRIBUTING.md
--rw-r--r--   0 trval     (1000) trval     (1000)     1516 2023-04-04 08:06:59.000000 mongomancy-0.0.6/LICENSE
--rw-r--r--   0 trval     (1000) trval     (1000)       42 2023-04-12 12:30:41.000000 mongomancy-0.0.6/MANIFEST.in
--rw-r--r--   0 trval     (1000) trval     (1000)     4468 2023-04-13 12:07:23.179283 mongomancy-0.0.6/PKG-INFO
--rw-rw-r--   0 trval     (1000) trval     (1000)     3677 2022-09-06 10:07:16.000000 mongomancy-0.0.6/README.md
--rw-r--r--   0 trval     (1000) trval     (1000)     1368 2023-04-12 12:30:41.000000 mongomancy-0.0.6/pyproject.toml
--rw-rw-r--   0 trval     (1000) trval     (1000)       68 2022-09-02 09:38:35.000000 mongomancy-0.0.6/requirements.txt
--rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-04-13 12:07:23.179283 mongomancy-0.0.6/setup.cfg
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-13 12:07:23.175949 mongomancy-0.0.6/src/
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-13 12:07:23.179283 mongomancy-0.0.6/src/mongomancy/
--rw-r--r--   0 trval     (1000) trval     (1000)      431 2023-04-13 12:06:01.000000 mongomancy-0.0.6/src/mongomancy/__init__.py
--rw-r--r--   0 trval     (1000) trval     (1000)    13420 2023-04-12 12:30:41.000000 mongomancy-0.0.6/src/mongomancy/engine.py
--rw-rw-r--   0 trval     (1000) trval     (1000)      924 2022-08-29 12:44:42.000000 mongomancy-0.0.6/src/mongomancy/mongo_errors.py
--rw-r--r--   0 trval     (1000) trval     (1000)        0 2023-04-12 12:30:41.000000 mongomancy-0.0.6/src/mongomancy/py.typed
--rw-r--r--   0 trval     (1000) trval     (1000)    12445 2023-04-13 12:06:01.000000 mongomancy-0.0.6/src/mongomancy/schema.py
--rw-r--r--   0 trval     (1000) trval     (1000)     5603 2023-04-13 12:06:01.000000 mongomancy-0.0.6/src/mongomancy/types.py
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-04-13 12:07:23.179283 mongomancy-0.0.6/src/mongomancy.egg-info/
--rw-rw-r--   0 trval     (1000) trval     (1000)     4468 2023-04-13 12:07:23.000000 mongomancy-0.0.6/src/mongomancy.egg-info/PKG-INFO
--rw-rw-r--   0 trval     (1000) trval     (1000)      435 2023-04-13 12:07:23.000000 mongomancy-0.0.6/src/mongomancy.egg-info/SOURCES.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)        1 2023-04-13 12:07:23.000000 mongomancy-0.0.6/src/mongomancy.egg-info/dependency_links.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)       13 2023-04-13 12:07:23.000000 mongomancy-0.0.6/src/mongomancy.egg-info/requires.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)       11 2023-04-13 12:07:23.000000 mongomancy-0.0.6/src/mongomancy.egg-info/top_level.txt
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:06:21.169779 mongomancy-0.1.0/
+-rw-r--r--   0 trval     (1000) trval     (1000)     1296 2023-05-09 13:03:25.000000 mongomancy-0.1.0/CHANGELOG.md
+-rw-rw-r--   0 trval     (1000) trval     (1000)     1329 2022-09-02 09:33:19.000000 mongomancy-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0 trval     (1000) trval     (1000)     1516 2023-04-04 08:06:59.000000 mongomancy-0.1.0/LICENSE
+-rw-r--r--   0 trval     (1000) trval     (1000)       42 2023-04-12 12:30:41.000000 mongomancy-0.1.0/MANIFEST.in
+-rw-r--r--   0 trval     (1000) trval     (1000)     4468 2023-05-09 13:06:21.169779 mongomancy-0.1.0/PKG-INFO
+-rw-rw-r--   0 trval     (1000) trval     (1000)     3677 2022-09-06 10:07:16.000000 mongomancy-0.1.0/README.md
+-rw-r--r--   0 trval     (1000) trval     (1000)     1368 2023-04-12 12:30:41.000000 mongomancy-0.1.0/pyproject.toml
+-rw-rw-r--   0 trval     (1000) trval     (1000)       68 2022-09-02 09:38:35.000000 mongomancy-0.1.0/requirements.txt
+-rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-05-09 13:06:21.169779 mongomancy-0.1.0/setup.cfg
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:06:21.166446 mongomancy-0.1.0/src/
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:06:21.166446 mongomancy-0.1.0/src/mongomancy/
+-rw-r--r--   0 trval     (1000) trval     (1000)      431 2023-05-09 13:03:25.000000 mongomancy-0.1.0/src/mongomancy/__init__.py
+-rw-r--r--   0 trval     (1000) trval     (1000)    13920 2023-05-09 13:03:25.000000 mongomancy-0.1.0/src/mongomancy/engine.py
+-rw-rw-r--   0 trval     (1000) trval     (1000)      924 2022-08-29 12:44:42.000000 mongomancy-0.1.0/src/mongomancy/mongo_errors.py
+-rw-r--r--   0 trval     (1000) trval     (1000)        0 2023-04-12 12:30:41.000000 mongomancy-0.1.0/src/mongomancy/py.typed
+-rw-r--r--   0 trval     (1000) trval     (1000)    14168 2023-05-09 13:03:25.000000 mongomancy-0.1.0/src/mongomancy/schema.py
+-rw-r--r--   0 trval     (1000) trval     (1000)     5944 2023-05-09 13:03:25.000000 mongomancy-0.1.0/src/mongomancy/types.py
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 13:06:21.166446 mongomancy-0.1.0/src/mongomancy.egg-info/
+-rw-rw-r--   0 trval     (1000) trval     (1000)     4468 2023-05-09 13:06:21.000000 mongomancy-0.1.0/src/mongomancy.egg-info/PKG-INFO
+-rw-rw-r--   0 trval     (1000) trval     (1000)      435 2023-05-09 13:06:21.000000 mongomancy-0.1.0/src/mongomancy.egg-info/SOURCES.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)        1 2023-05-09 13:06:21.000000 mongomancy-0.1.0/src/mongomancy.egg-info/dependency_links.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)       13 2023-05-09 13:06:21.000000 mongomancy-0.1.0/src/mongomancy.egg-info/requires.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)       11 2023-05-09 13:06:21.000000 mongomancy-0.1.0/src/mongomancy.egg-info/top_level.txt
```

### Comparing `mongomancy-0.0.6/CHANGELOG.md` & `mongomancy-0.1.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.0] - 2023-05-09
+
+### Added
+
+- mongomancy creates `mongomancy_lock` collection to synchronize db init with master lock record
+- create all now uses multiprocess and thread log
+
 ## [0.0.6] - 2023-04-13
 
 ### Fixed
 
 - typing of required fields of index more broad
 
 ## [0.0.5] - 2023-04-12
```

### Comparing `mongomancy-0.0.6/CONTRIBUTING.md` & `mongomancy-0.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mongomancy-0.0.6/LICENSE` & `mongomancy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mongomancy-0.0.6/PKG-INFO` & `mongomancy-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomancy
-Version: 0.0.6
+Version: 0.1.0
 Summary: Pymongo based python client with data definition layer.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Ryu-CZ/mongomancy
 Project-URL: Bug Tracker, https://github.com/Ryu-CZ/mongomancy/issues
 Keywords: mongo,python,pymongo,database,nosql
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `mongomancy-0.0.6/README.md` & `mongomancy-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mongomancy-0.0.6/pyproject.toml` & `mongomancy-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mongomancy-0.0.6/src/mongomancy/engine.py` & `mongomancy-0.1.0/src/mongomancy/engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import List, Sequence, Union, Set, TypeVar, Mapping, Any, ClassVar, Type, Optional, Callable, Iterable
 
 import pymongo
 import pymongo.command_cursor
 import pymongo.database
 import pymongo.results
 import pymongo.typings
+import pymongo.client_session
 from pymongo.errors import PyMongoError
 
 from . import mongo_errors, types
 
 __all__ = ("Engine",)
 
 LoggerType = Union[logging.Logger, logging.LoggerAdapter]
@@ -50,14 +51,16 @@
         "write_retry_delay",
         "read_retry",
         "read_retry_delay",
         "retry_codes",
         "_address",
         "_connection_params",
         "reconnect_hooks",
+        "mp_semaphore",
+        "th_semaphore",
     )
 
     def __init__(
         self,
         host: str = "localhost",
         port: int = 27017,
         max_pool_size: int = 1,
@@ -255,14 +258,26 @@
                 collection = self.client[collection.database.name][collection.name]
         if _error:
             command_name_ = command_name_ or getattr(command, "__qualname__", "<unknown_command>")
             self.logger.warning(f"fatal fail - {command_name_} args={args}, kwargs={kwargs} - after {attempt}x retry")
             raise _error from _error
         return result
 
+    def start_session(
+        self,
+        causal_consistency: Optional[bool] = None,
+        default_transaction_options: Optional[pymongo.client_session.TransactionOptions] = None,
+        snapshot: Optional[bool] = False,
+    ) -> pymongo.client_session.ClientSession:
+        return self.client.start_session(
+            causal_consistency,
+            default_transaction_options,
+            snapshot,
+        )
+
     def find_one(
         self,
         collection: pymongo.collection.Collection,
         where: Optional[types.BsonDict],
         *args,
         **kwargs,
     ) -> Optional[types.BsonDict]:
```

### Comparing `mongomancy-0.0.6/src/mongomancy/mongo_errors.py` & `mongomancy-0.1.0/src/mongomancy/mongo_errors.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.0.6/src/mongomancy/schema.py` & `mongomancy-0.1.0/src/mongomancy/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import logging
+import multiprocessing
+import threading
 import time
 import traceback
 from dataclasses import dataclass
 from typing import (
     List,
     Tuple,
     Union,
     TypeVar,
     Mapping,
     Any,
     Optional,
     Dict,
     Iterable,
+    ClassVar,
 )
 
 import pymongo
 import pymongo.command_cursor
 import pymongo.database
 import pymongo.results
 import pymongo.typings
@@ -31,14 +34,23 @@
     "DocumentType",
 )
 
 LoggerType = Union[logging.Logger, logging.LoggerAdapter]
 DocumentType = TypeVar("DocumentType", bound=Mapping[str, Any])
 
 
+def define_lock_collection(name: str):
+    return types.CollectionDefinition(
+        name,
+        default_docs=[
+            types.Document(unique_key={"_id": "master"}, data={"_id": "master", "locked": False}),
+        ],
+    )
+
+
 @dataclass(slots=True)
 class Collection:
     """
     Abstraction of existing collection.
     Wraps `pymongo.collection.Collection` for easier reconnect.
     """
 
@@ -150,31 +162,38 @@
 
     """
 
     engine: types.Executor
     topology: List[types.CollectionDefinition]
     _database: pymongo.database.Database
     _collections: Dict[str, Collection]
+    mp_semaphore: multiprocessing.Semaphore
+    th_semaphore: threading.Semaphore
     logger: LoggerType
+    LOCK_COLLECTION: ClassVar[str] = "mongomancy_lock"
 
     __slots__ = (
         "engine",
         "topology",
         "_database",
         "_collections",
+        "mp_semaphore",
+        "th_semaphore",
         "logger",
     )
 
     def __init__(
         self,
         name: str,
         logger: LoggerType,
         engine: types.Executor,
         *collections: types.CollectionDefinition,
     ) -> None:
+        self.mp_semaphore = multiprocessing.Semaphore()
+        self.th_semaphore = threading.Semaphore()
         self._collections = {}
         self.topology = []
         self.logger = logger
         self.engine = engine
         self._database = engine.get_database(name)
         for coll in collections:
             self.add_collection(coll)
@@ -228,22 +247,51 @@
         """
         Add new collection definitions into `self.topology`.
 
         :param new_definitions: add the collection definition
         """
         self.topology.append(new_definitions)
 
+    def _lock(self) -> bool:
+        self.create_collection(define_lock_collection(self.LOCK_COLLECTION))
+        doc = self.engine.find_one_and_update(
+            self._database[self.LOCK_COLLECTION],
+            where={"_id": "master", "locked": False},
+            changes={"$set": {"locked": True}},
+        )
+        if not doc:
+            return False
+        return not bool(doc.get("locked"))
+
+    def _unlock(self):
+        self.engine.find_one_and_update(
+            self._database[self.LOCK_COLLECTION],
+            where={"_id": "master"},
+            changes={"$set": {"locked": False}},
+            upsert=True,
+        )
+
     def create_all(self, skip_existing: bool = True) -> None:
         """
         Create all collections if not exists. Loads `self._collections` for use.
 
         :param skip_existing: skip collection init if collection already exists in db
         """
-        for collection_definition in self.topology:
-            _ = self.create_collection(collection_definition, skip_existing)
+        with self.mp_semaphore:
+            with self.th_semaphore:
+                if not self._lock():
+                    self.logger.debug("database is locked - this process or thread is skipping 'Database.create_all'")
+                    return
+                try:
+                    for collection_definition in self.topology:
+                        _ = self.create_collection(collection_definition, skip_existing)
+                except (Exception, KeyError, IndexError, IOError) as e:
+                    self.logger.error(f"create_all failed on {e}")
+                    self._unlock()
+                    raise e from e
 
     def create_collection(
         self,
         definition: types.CollectionDefinition,
         skip_existing: bool = True,
     ) -> Collection:
         """
```

### Comparing `mongomancy-0.0.6/src/mongomancy/types.py` & `mongomancy-0.1.0/src/mongomancy/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Any,
     Iterable,
     Callable,
 )
 from collections import OrderedDict
 import pymongo.database
 import pymongo.results
+import pymongo.client_session
 from bson import ObjectId
 from pymongo.command_cursor import CommandCursor
 
 __all__ = (
     "Bson",
     "BsonDict",
     "BsonList",
@@ -113,14 +114,23 @@
     Reconnect-able interface of MongoDB mongo_driver that allows to execute commands like:
     `find`, `insert_one`, `update_many`, `delete_one`.
     """
 
     __slots__ = ()
 
     @abc.abstractmethod
+    def start_session(
+        self,
+        causal_consistency: Optional[bool] = None,
+        default_transaction_options: Optional[pymongo.client_session.TransactionOptions] = None,
+        snapshot: Optional[bool] = False,
+    ) -> pymongo.client_session.ClientSession:
+        ...
+
+    @abc.abstractmethod
     def find_one(
         self,
         collection: pymongo.collection.Collection,
         where: Optional[BsonDict],
         *args,
         **kwargs,
     ) -> Optional[Dict[str, Any]]:
```

### Comparing `mongomancy-0.0.6/src/mongomancy.egg-info/PKG-INFO` & `mongomancy-0.1.0/src/mongomancy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomancy
-Version: 0.0.6
+Version: 0.1.0
 Summary: Pymongo based python client with data definition layer.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Ryu-CZ/mongomancy
 Project-URL: Bug Tracker, https://github.com/Ryu-CZ/mongomancy/issues
 Keywords: mongo,python,pymongo,database,nosql
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

