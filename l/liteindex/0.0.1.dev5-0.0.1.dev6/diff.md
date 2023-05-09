# Comparing `tmp/liteindex-0.0.1.dev5.tar.gz` & `tmp/liteindex-0.0.1.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteindex-0.0.1.dev5.tar", last modified: Wed May  3 10:21:32 2023, max compression
+gzip compressed data, was "liteindex-0.0.1.dev6.tar", last modified: Tue May  9 03:55:59 2023, max compression
```

## Comparing `liteindex-0.0.1.dev5.tar` & `liteindex-0.0.1.dev6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:21:32.071393 liteindex-0.0.1.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-03 10:21:17.000000 liteindex-0.0.1.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-03 10:21:32.071393 liteindex-0.0.1.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 10:21:17.000000 liteindex-0.0.1.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:21:32.071393 liteindex-0.0.1.dev5/liteindex/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 10:21:17.000000 liteindex-0.0.1.dev5/liteindex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-05-03 10:21:17.000000 liteindex-0.0.1.dev5/liteindex/any_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    18737 2023-05-03 10:21:17.000000 liteindex-0.0.1.dev5/liteindex/defined_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-03 10:21:17.000000 liteindex-0.0.1.dev5/liteindex/dict_index_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-03 10:21:17.000000 liteindex-0.0.1.dev5/liteindex/file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-03 10:21:17.000000 liteindex-0.0.1.dev5/liteindex/number_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:21:32.071393 liteindex-0.0.1.dev5/liteindex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-03 10:21:32.000000 liteindex-0.0.1.dev5/liteindex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-03 10:21:32.000000 liteindex-0.0.1.dev5/liteindex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:21:32.000000 liteindex-0.0.1.dev5/liteindex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-03 10:21:32.000000 liteindex-0.0.1.dev5/liteindex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 10:21:32.000000 liteindex-0.0.1.dev5/liteindex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 10:21:32.071393 liteindex-0.0.1.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-03 10:21:17.000000 liteindex-0.0.1.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:59.237019 liteindex-0.0.1.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-09 03:55:48.000000 liteindex-0.0.1.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-09 03:55:59.237019 liteindex-0.0.1.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-09 03:55:48.000000 liteindex-0.0.1.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:59.233019 liteindex-0.0.1.dev6/liteindex/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-09 03:55:48.000000 liteindex-0.0.1.dev6/liteindex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-09 03:55:48.000000 liteindex-0.0.1.dev6/liteindex/any_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11256 2023-05-09 03:55:48.000000 liteindex-0.0.1.dev6/liteindex/defined_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-09 03:55:48.000000 liteindex-0.0.1.dev6/liteindex/dict_index_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-09 03:55:48.000000 liteindex-0.0.1.dev6/liteindex/file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-09 03:55:48.000000 liteindex-0.0.1.dev6/liteindex/number_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:55:59.237019 liteindex-0.0.1.dev6/liteindex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-09 03:55:59.000000 liteindex-0.0.1.dev6/liteindex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-09 03:55:59.000000 liteindex-0.0.1.dev6/liteindex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 03:55:59.000000 liteindex-0.0.1.dev6/liteindex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-09 03:55:59.000000 liteindex-0.0.1.dev6/liteindex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 03:55:59.000000 liteindex-0.0.1.dev6/liteindex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 03:55:59.237019 liteindex-0.0.1.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-09 03:55:48.000000 liteindex-0.0.1.dev6/setup.py
```

### Comparing `liteindex-0.0.1.dev5/LICENSE` & `liteindex-0.0.1.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev5/liteindex/any_index.py` & `liteindex-0.0.1.dev6/liteindex/any_index.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -381,8 +381,8 @@
 
     print("search results:", d.search_by_value(["number"], 2))
 
     # d.create_number_index(["number"])
 
     # print(d.list_indexes())
 
-    print("All tests passed!")
+    print("All tests passed!")
```

### Comparing `liteindex-0.0.1.dev5/liteindex/dict_index_helpers.py` & `liteindex-0.0.1.dev6/liteindex/dict_index_helpers.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev5/liteindex/file_index.py` & `liteindex-0.0.1.dev6/liteindex/file_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import sqlite3
 import tempfile
 import os
 from typing import Optional, Dict, Iterator
 from contextlib import contextmanager
 from threading import Lock
 
+
 class FileIndex:
     def __init__(self, name: str, db_path: str = ":memory:"):
         self.name = name
         self.db_path = db_path
-        self._connection = sqlite3.connect(self.db_path, uri=True, check_same_thread=False)
+        self._connection = sqlite3.connect(
+            self.db_path, uri=True, check_same_thread=False
+        )
         self._lock = Lock()
         self._create_table()
 
     @contextmanager
     def _locked_cursor(self):
         with self._lock:
             cursor = self._connection.cursor()
@@ -24,47 +27,58 @@
                 cursor.close()
 
     def _create_table(self):
         with self._locked_cursor() as cursor:
             cursor.execute(
                 f"CREATE TABLE IF NOT EXISTS {self.name} (id INTEGER PRIMARY KEY AUTOINCREMENT, key TEXT, file_name TEXT, value BLOB)"
             )
-            cursor.execute(f"CREATE INDEX IF NOT EXISTS idx_file_name ON {self.name} (file_name)")
+            cursor.execute(
+                f"CREATE INDEX IF NOT EXISTS idx_file_name ON {self.name} (file_name)"
+            )
 
     def __setitem__(self, key: str, value: Dict[str, bytes]):
         with self._locked_cursor() as cursor:
-            data = [(key, file_name, file_content) for file_name, file_content in value.items()]
+            data = [
+                (key, file_name, file_content)
+                for file_name, file_content in value.items()
+            ]
             cursor.executemany(
                 f"INSERT OR REPLACE INTO {self.name} (key, file_name, value) VALUES (?, ?, ?)",
-                data
+                data,
             )
 
     def __getitem__(self, key: str) -> Dict[str, bytes]:
         with self._connection.cursor() as cursor:
-            cursor.execute(f"SELECT file_name, value FROM {self.name} WHERE key=?", (key,))
+            cursor.execute(
+                f"SELECT file_name, value FROM {self.name} WHERE key=?", (key,)
+            )
             results = cursor.fetchall()
 
         if not results:
             raise KeyError(f"Key '{key}' not found in {self.name}")
 
         return {file_name: file_data for file_name, file_data in results}
 
     def get_file_paths(self, key: str) -> Iterator[str]:
         with self._connection.cursor() as cursor:
             temp_dir = tempfile.mkdtemp()
-            cursor.execute(f"SELECT file_name, value FROM {self.name} WHERE key=?", (key,))
+            cursor.execute(
+                f"SELECT file_name, value FROM {self.name} WHERE key=?", (key,)
+            )
             for file_name, file_data in cursor:
                 temp_path = os.path.join(temp_dir, file_name)
                 with open(temp_path, "wb") as temp_file:
                     temp_file.write(file_data)
                 yield temp_path
 
     def __delitem__(self, key: str):
         with self._locked_cursor() as cursor:
             cursor.execute(f"DELETE FROM {self.name} WHERE key=?", (key,))
+
+
 if __name__ == "__main__":
     # Initialize the FileIndex
     file_index = FileIndex("my_files")
 
     # Add multiple files to the FileIndex
     file_key = "key_1"
     files = {
@@ -80,8 +94,7 @@
     # Get the file paths of the files stored in memory
     file_paths_iterator = file_index.get_file_paths(file_key)
     for file_path in file_paths_iterator:
         print(f"File path in memory: {file_path}")
         with open(file_path, "rb") as f:
             file_data = f.read()
             print(f"File content from file path: {file_data}")
-
```

### Comparing `liteindex-0.0.1.dev5/liteindex/number_index.py` & `liteindex-0.0.1.dev6/liteindex/number_index.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev5/setup.py` & `liteindex-0.0.1.dev6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "liteindex"
 DESCRIPTION = "SQLite based queryable python indexes for dicts and lists"
 URL = "https://github.com/notAI-tech/liteindex"
 EMAIL = "praneeth@bpraneeth.com"
 AUTHOR = "BEDAPUDI PRANEETH"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.1.dev5"
+VERSION = "0.0.1.dev6"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
 ]
 
 # What packages are optional?
 EXTRAS = {
```

