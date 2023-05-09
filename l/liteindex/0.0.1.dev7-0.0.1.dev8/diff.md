# Comparing `tmp/liteindex-0.0.1.dev7.tar.gz` & `tmp/liteindex-0.0.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteindex-0.0.1.dev7.tar", last modified: Tue May  9 03:59:25 2023, max compression
+gzip compressed data, was "liteindex-0.0.1.dev8.tar", last modified: Tue May  9 10:18:23 2023, max compression
```

## Comparing `liteindex-0.0.1.dev7.tar` & `liteindex-0.0.1.dev8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:59:25.519761 liteindex-0.0.1.dev7/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-09 03:59:15.000000 liteindex-0.0.1.dev7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-09 03:59:25.519761 liteindex-0.0.1.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-09 03:59:15.000000 liteindex-0.0.1.dev7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:59:25.519761 liteindex-0.0.1.dev7/liteindex/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-09 03:59:15.000000 liteindex-0.0.1.dev7/liteindex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-09 03:59:15.000000 liteindex-0.0.1.dev7/liteindex/any_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    11256 2023-05-09 03:59:15.000000 liteindex-0.0.1.dev7/liteindex/defined_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-09 03:59:15.000000 liteindex-0.0.1.dev7/liteindex/dict_index_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-09 03:59:15.000000 liteindex-0.0.1.dev7/liteindex/file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-09 03:59:15.000000 liteindex-0.0.1.dev7/liteindex/number_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:59:25.519761 liteindex-0.0.1.dev7/liteindex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-09 03:59:25.000000 liteindex-0.0.1.dev7/liteindex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-09 03:59:25.000000 liteindex-0.0.1.dev7/liteindex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 03:59:25.000000 liteindex-0.0.1.dev7/liteindex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-09 03:59:25.000000 liteindex-0.0.1.dev7/liteindex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 03:59:25.000000 liteindex-0.0.1.dev7/liteindex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 03:59:25.519761 liteindex-0.0.1.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-09 03:59:15.000000 liteindex-0.0.1.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:23.664692 liteindex-0.0.1.dev8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-09 10:18:13.000000 liteindex-0.0.1.dev8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-09 10:18:23.664692 liteindex-0.0.1.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-09 10:18:13.000000 liteindex-0.0.1.dev8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:23.660692 liteindex-0.0.1.dev8/liteindex/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-09 10:18:13.000000 liteindex-0.0.1.dev8/liteindex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-09 10:18:13.000000 liteindex-0.0.1.dev8/liteindex/any_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-05-09 10:18:13.000000 liteindex-0.0.1.dev8/liteindex/defined_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-09 10:18:13.000000 liteindex-0.0.1.dev8/liteindex/dict_index_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-09 10:18:13.000000 liteindex-0.0.1.dev8/liteindex/file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-09 10:18:13.000000 liteindex-0.0.1.dev8/liteindex/number_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:23.664692 liteindex-0.0.1.dev8/liteindex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-09 10:18:23.000000 liteindex-0.0.1.dev8/liteindex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-09 10:18:23.000000 liteindex-0.0.1.dev8/liteindex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:18:23.000000 liteindex-0.0.1.dev8/liteindex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-09 10:18:23.000000 liteindex-0.0.1.dev8/liteindex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 10:18:23.000000 liteindex-0.0.1.dev8/liteindex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 10:18:23.664692 liteindex-0.0.1.dev8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-09 10:18:13.000000 liteindex-0.0.1.dev8/setup.py
```

### Comparing `liteindex-0.0.1.dev7/LICENSE` & `liteindex-0.0.1.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev7/PKG-INFO` & `liteindex-0.0.1.dev8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteindex
-Version: 0.0.1.dev7
+Version: 0.0.1.dev8
 Summary: SQLite based queryable python indexes for dicts and lists
 Home-page: https://github.com/notAI-tech/liteindex
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `liteindex-0.0.1.dev7/README.md` & `liteindex-0.0.1.dev8/README.md`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev7/liteindex/any_index.py` & `liteindex-0.0.1.dev8/liteindex/any_index.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev7/liteindex/defined_index.py` & `liteindex-0.0.1.dev8/liteindex/defined_index.py`

 * *Files 10% similar despite different names*

```diff
@@ -121,107 +121,129 @@
                 params.append(value)
 
         for key, value in query.items():
             process_nested_query(value, [key])
 
         return where_conditions, params
 
-    def set(self, id: str, item: Dict[str, Any]) -> None:
-        """Insert or update an item in the index."""
-        item["id"] = id
-        keys = []
-        values = []
-        placeholders = []
-        for key, value in item.items():
-            keys.append(key)
-
-            if isinstance(value, (list, dict)):
-                value = json.dumps(value)
-
-            values.append(value)
-            placeholders.append("?")
-        keys_str = ", ".join(keys)
-        placeholders_str = ", ".join(placeholders)
-        update_str = ", ".join([f"{key} = ?" for key in keys])
-
-        query = f"""
-        INSERT INTO {self.name} ({keys_str})
-        VALUES ({placeholders_str})
-        ON CONFLICT(id) DO UPDATE SET {update_str}
-        """
-
-        self._connection.execute(query, values * 2)
-        self._connection.commit()
-
-    def batch_set(self, items: List[Tuple[str, Dict[str, Any]]]) -> None:
-        """Insert or update multiple items in the index."""
-        if not items:
-            return
-
-        all_keys = set(self.schema.keys())
-        all_keys.add("id")
-        keys_str = ", ".join(all_keys)
-        update_str = ", ".join(
-            [f"{key} = excluded.{key}" for key in all_keys if key != "id"]
-        )
-
-        placeholders = []
-        values = []
-        for id, item in items:
+    def set(self, key: Union[str, Tuple[str, Union[str, int]]], value: Any) -> None:
+        if isinstance(key, tuple):
+            id, column, *keys = key
+
+            if not keys:
+                if isinstance(value, (list, dict)):
+                    value = json.dumps(value)
+
+                query = f"""
+                INSERT INTO {self.name} (id, {column})
+                VALUES (?, ?)
+                ON CONFLICT(id) DO UPDATE SET {column} = ?
+                """
+                self._connection.execute(query, (id, value, value))
+                self._connection.commit()
+            else:
+                json_set_path = f'$.{".".join([str(k) for k in keys])}'
+                query = f"""
+                INSERT INTO {self.name} (id, {column})
+                VALUES (?, json(?))
+                ON CONFLICT(id) DO UPDATE SET {column} = json_set({column}, ?, ?)
+                """
+                self._connection.execute(
+                    query,
+                    (
+                        id,
+                        json.dumps({keys[-1]: value}),
+                        json_set_path,
+                        json.dumps(value),
+                    ),
+                )
+                self._connection.commit()
+        else:
+            id = key
+            item = value
             item["id"] = id
-            row_values = []
-            for key in all_keys:
-                value = item.get(key, self.schema.get(key))
+            keys = []
+            values = []
+            placeholders = []
+            for key, value in item.items():
+                keys.append(key)
+
                 if isinstance(value, (list, dict)):
                     value = json.dumps(value)
-                row_values.append(value)
-            placeholders.append(f"({', '.join(['?' for _ in row_values])})")
-            values.extend(row_values)
-
-        placeholders_str = ", ".join(placeholders)
-
-        query = f"""
-        INSERT INTO {self.name} ({keys_str})
-        VALUES {placeholders_str}
-        ON CONFLICT(id) DO UPDATE SET {update_str}
-        """
 
-        self._connection.executemany(query, values)
-        self._connection.commit()
+                values.append(value)
+                placeholders.append("?")
+            keys_str = ", ".join(keys)
+            placeholders_str = ", ".join(placeholders)
+            update_str = ", ".join([f"{key} = ?" for key in keys])
+
+            query = f"""
+            INSERT INTO {self.name} ({keys_str})
+            VALUES ({placeholders_str})
+            ON CONFLICT(id) DO UPDATE SET {update_str}
+            """
+
+            self._connection.execute(query, values * 2)
+            self._connection.commit()
+
+    def get(self, id: str, *keys: Union[str, int]) -> Optional[Any]:
+        """Retrieve an item or a specific key path value from the item in the index by its id."""
+        value = None
+        if len(keys) == 1:
+            query = f"SELECT {keys[0]} FROM {self.name} WHERE id = ?"
+            cursor = self._connection.execute(query, (id,))
+            row = cursor.fetchone()
+            if row:
+                value = row[0] if row[0] is not None else None
+        elif len(keys) > 1:
+            column = keys[0]
+            key_path_parts = []
+            for key in keys[1:]:
+                if isinstance(key, int):
+                    key_path_parts.append(f"[{key}]")
+                else:
+                    key_path_parts.append(f".{key}")
+            key_path = "$" + "".join(key_path_parts)
+            query = f"SELECT json_extract({column}, ?) FROM {self.name} WHERE id = ?"
+            cursor = self._connection.execute(query, (key_path, id))
+            row = cursor.fetchone()
+            if row:
+                value = row[0] if row[0] is not None else None
+        else:
+            query = f"SELECT * FROM {self.name} WHERE id = ?"
+            cursor = self._connection.execute(query, (id,))
+            row = cursor.fetchone()
+            if row:
+                value = self.__row_to_id_and_item(row)[1]
+
+        if not value:
+            raise KeyError(f"Key {id} {keys} not found in index {self.name}")
+
+        return value
+
+    def __getitem__(
+        self, key: Union[str, Tuple[str, Union[str, int]]]
+    ) -> Optional[Any]:
+        if isinstance(key, tuple):
+            id, *keys = key
+            return self.get(id, *keys)
+        else:
+            id = key
+            return self.get(id)
 
     def __row_to_id_and_item(self, row: sqlite3.Row) -> Tuple[str, Dict[str, Any]]:
         item = dict(row)
         for k, v in item.items():
             try:
                 item[k] = json.loads(v)
             except:
                 pass
 
         return item["id"], item
 
-    def get(self, id: str, *keys: str) -> Optional[Dict[str, Any]]:
-        """Retrieve an item or a specific key path value from the item in the index by its id."""
-        if not keys:
-            query = f"SELECT * FROM {self.name} WHERE id = ?"
-            cursor = self._connection.execute(query, (id,))
-            row = cursor.fetchone()
-            if row:
-                return self.__row_to_id_and_item(row)[1]
-            else:
-                return None
-        else:
-            key_path = ".".join(keys)
-            query = f"SELECT json_extract({keys[0]}, ?) FROM {self.name} WHERE id = ?"
-            cursor = self._connection.execute(query, (key_path, id))
-            row = cursor.fetchone()
-            if row:
-                return row[0] if row[0] is not None else None
-            else:
-                return None
-
     def search(
         self,
         query: Optional[Dict],
         sort_by: Optional[str] = None,
         reversed_sort: Optional[bool] = False,
     ) -> List[Dict]:
 
@@ -279,14 +301,15 @@
 
 if __name__ == "__main__":
     # Define the schema for the index
     schema = {
         "name": "",
         "age": 0,
         "address": {"street": "", "city": "", "state": "", "country": ""},
+        "years": [1, 2, 3, 4],
     }
 
     # Create a new index with the specified schema
     index = DefinedIndex("test_index", schema=schema)
     # Set an item in the index
     item = {
         "name": "John Doe",
@@ -296,17 +319,25 @@
             "city": "New York",
             "state": "NY",
             "country": "USA",
         },
     }
     index.set("1", item)
 
-    # Get an item from the index
-    retrieved_item = index.get("1")
-    print(retrieved_item)
+    index.set(("1", "name"), "updated John Doe")
+    print(index.get("1"))
+
+    index.set(("1", "years"), [1, 2, 3])
+    print(index.get("1"))
+
+    index.set(("1", "years", 1), 4)
+    print(index.get("1"))
+
+    index.set(("1", "address", "state"), "updated NY 2")
+    print(index.get("1"))
 
     # Search for items in the index
     query = {"age": (None, 35)}
     results = index.search(query)
     for result in results:
         print("--", result)
```

### Comparing `liteindex-0.0.1.dev7/liteindex/dict_index_helpers.py` & `liteindex-0.0.1.dev8/liteindex/dict_index_helpers.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev7/liteindex/file_index.py` & `liteindex-0.0.1.dev8/liteindex/file_index.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev7/liteindex/number_index.py` & `liteindex-0.0.1.dev8/liteindex/number_index.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev7/liteindex.egg-info/PKG-INFO` & `liteindex-0.0.1.dev8/liteindex.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteindex
-Version: 0.0.1.dev7
+Version: 0.0.1.dev8
 Summary: SQLite based queryable python indexes for dicts and lists
 Home-page: https://github.com/notAI-tech/liteindex
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `liteindex-0.0.1.dev7/setup.py` & `liteindex-0.0.1.dev8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "liteindex"
 DESCRIPTION = "SQLite based queryable python indexes for dicts and lists"
 URL = "https://github.com/notAI-tech/liteindex"
 EMAIL = "praneeth@bpraneeth.com"
 AUTHOR = "BEDAPUDI PRANEETH"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.1.dev7"
+VERSION = "0.0.1.dev8"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
 ]
 
 # What packages are optional?
 EXTRAS = {
```

