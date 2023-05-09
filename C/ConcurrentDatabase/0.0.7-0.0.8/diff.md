# Comparing `tmp/ConcurrentDatabase-0.0.7.tar.gz` & `tmp/ConcurrentDatabase-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ConcurrentDatabase-0.0.7.tar", last modified: Tue May  9 01:21:25 2023, max compression
+gzip compressed data, was "ConcurrentDatabase-0.0.8.tar", last modified: Tue May  9 01:46:51 2023, max compression
```

## Comparing `ConcurrentDatabase-0.0.7.tar` & `ConcurrentDatabase-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:21:25.736306 ConcurrentDatabase-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:21:25.732306 ConcurrentDatabase-0.0.7/ConcurrentDatabase/
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-09 01:21:14.000000 ConcurrentDatabase-0.0.7/ConcurrentDatabase/ColumnWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14289 2023-05-09 01:21:14.000000 ConcurrentDatabase-0.0.7/ConcurrentDatabase/Database.py
--rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-05-09 01:21:14.000000 ConcurrentDatabase-0.0.7/ConcurrentDatabase/DynamicEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)    15673 2023-05-09 01:21:14.000000 ConcurrentDatabase-0.0.7/ConcurrentDatabase/DynamicTable.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 01:21:14.000000 ConcurrentDatabase-0.0.7/ConcurrentDatabase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:21:25.732306 ConcurrentDatabase-0.0.7/ConcurrentDatabase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-09 01:21:25.000000 ConcurrentDatabase-0.0.7/ConcurrentDatabase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-09 01:21:25.000000 ConcurrentDatabase-0.0.7/ConcurrentDatabase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 01:21:25.000000 ConcurrentDatabase-0.0.7/ConcurrentDatabase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-09 01:21:25.000000 ConcurrentDatabase-0.0.7/ConcurrentDatabase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-09 01:21:25.736306 ConcurrentDatabase-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-09 01:21:14.000000 ConcurrentDatabase-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-09 01:21:14.000000 ConcurrentDatabase-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 01:21:25.736306 ConcurrentDatabase-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-09 01:21:14.000000 ConcurrentDatabase-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:46:51.781914 ConcurrentDatabase-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:46:51.781914 ConcurrentDatabase-0.0.8/ConcurrentDatabase/
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-09 01:46:40.000000 ConcurrentDatabase-0.0.8/ConcurrentDatabase/ColumnWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14406 2023-05-09 01:46:40.000000 ConcurrentDatabase-0.0.8/ConcurrentDatabase/Database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-05-09 01:46:40.000000 ConcurrentDatabase-0.0.8/ConcurrentDatabase/DynamicEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16055 2023-05-09 01:46:40.000000 ConcurrentDatabase-0.0.8/ConcurrentDatabase/DynamicTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 01:46:40.000000 ConcurrentDatabase-0.0.8/ConcurrentDatabase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:46:51.781914 ConcurrentDatabase-0.0.8/ConcurrentDatabase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-09 01:46:51.000000 ConcurrentDatabase-0.0.8/ConcurrentDatabase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-09 01:46:51.000000 ConcurrentDatabase-0.0.8/ConcurrentDatabase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 01:46:51.000000 ConcurrentDatabase-0.0.8/ConcurrentDatabase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-09 01:46:51.000000 ConcurrentDatabase-0.0.8/ConcurrentDatabase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-09 01:46:51.781914 ConcurrentDatabase-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-09 01:46:40.000000 ConcurrentDatabase-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-09 01:46:40.000000 ConcurrentDatabase-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 01:46:51.781914 ConcurrentDatabase-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-09 01:46:40.000000 ConcurrentDatabase-0.0.8/setup.py
```

### Comparing `ConcurrentDatabase-0.0.7/ConcurrentDatabase/ColumnWrapper.py` & `ConcurrentDatabase-0.0.8/ConcurrentDatabase/ColumnWrapper.py`

 * *Files identical despite different names*

### Comparing `ConcurrentDatabase-0.0.7/ConcurrentDatabase/Database.py` & `ConcurrentDatabase-0.0.8/ConcurrentDatabase/Database.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,17 +80,17 @@
     def has_link(self, table1, table2):
         return (self.parent_table.table_name == table1.table_name and
                 self.child_table.table_name == table2.table_name) or \
                (self.child_table.table_name == table1.table_name and
                 self.parent_table.table_name == table2.table_name)
 
     def get_foreign_key(self, table):
-        if table == self.parent_table:
+        if table.table_name == self.parent_table.table_name:
             return self.parent_key, self.child_key
-        elif table == self.child_table:
+        elif table.table_name == self.child_table.table_name:
             return self.child_key, self.parent_key
         else:
             raise ValueError(f"Table {table} is not linked to {self}")
 
     def __str__(self):
         return f"{self.parent_table.table_name}.{self.parent_key.name} " \
                f"{'<->' if self.on_update == 'NO ACTION' else '->'} " \
@@ -242,14 +242,16 @@
         if table_name not in self.tables:
             raise KeyError(f"Table {table_name} not found in database {self.database_name}")
         self.run(f"DROP TABLE {table_name}")
         # Remove the table from the table_versions table
         self.table_version_table.delete(table_name=table_name)
         # del self.tables[table_name]
         self.tables.pop(table_name)
+        # del self.tables[table_name]
+        self._update_table_links()
 
     def run(self, sql, *args, **kwargs) -> sqlite3.Cursor:
         """
         Run a query on the database with thread safety.
         :param sql: The SQL query to run.
         :param args: The arguments to pass to the query.
         :param kwargs: The keyword arguments to pass to the query.
```

### Comparing `ConcurrentDatabase-0.0.7/ConcurrentDatabase/DynamicEntry.py` & `ConcurrentDatabase-0.0.8/ConcurrentDatabase/DynamicEntry.py`

 * *Files 5% similar despite different names*

```diff
@@ -174,19 +174,32 @@
         self._values = {self.columns[i].name: value for i, value in enumerate(result.fetchone())}
 
     def delete(self):
         """
         Deletes the entry from the database
         :return:
         """
-        primary_key_values = [self._values[column.name] for column in self.columns if column.primary_key]
         sql = f"DELETE FROM {self.table.table_name} WHERE {self._entry_where_clause()}"
-        result = self.database.run(sql, primary_key_values)
+        self.database.run(sql)
         del self
 
+    def matches(self, **kwargs):
+        """
+        Checks if the entry matches the given criteria
+        :param kwargs: The criteria to check
+        :return: True if the entry matches the criteria, False otherwise
+        """
+        for key in kwargs:
+            if key in self.columns:
+                if self._values[key] != kwargs[key]:
+                    return False
+            else:
+                raise KeyError(f"Column {key} does not exist in table {self.table.table_name}")
+        return True
+
     def is_dirty(self):
         return self._dirty
 
     def _entry_where_clause(self):
         """
         Returns a complete WHERE clause to find this entry in the database even if the table has no primary keys
         Will contain no ?'s and will be ready to be inserted into a SQL statement
@@ -267,14 +280,16 @@
         elif isinstance(other, dict):
             for key in other:
                 if key not in self._values:
                     raise KeyError(f"Key {key} not in entry")
                 if self._values[key] != other[key]:
                     return False
             return True
+        elif other is None:
+            return False
         else:
             raise TypeError(f"Cannot compare DynamicEntry to {type(other)}")
 
     def __del__(self):
         """
         Called when the DynamicEntry object is garbage collected, flushes the entry to the database to prevent data loss
         """
```

### Comparing `ConcurrentDatabase-0.0.7/ConcurrentDatabase/DynamicTable.py` & `ConcurrentDatabase-0.0.8/ConcurrentDatabase/DynamicTable.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,29 +88,30 @@
         Get a row from the table.
         :param kwargs: The filters to apply to the query.
         :return: The row.
         """
         self._validate_columns(**kwargs)
         # self._contains_primary_keys(**kwargs)
 
-        # Check if the DynamicEntry is already loaded
-        for entry in self.entries:
-            if entry == kwargs:
-                return entry
-
         # Build the query
         sql = f"SELECT * FROM {self.table_name}"
         if len(kwargs) > 0:
             sql += " WHERE "
             for column_name in kwargs:
                 column = self.columns[self.columns.index(column_name)]
                 sql += self._create_filter(column, kwargs[column_name]) + " AND "
             sql = sql[:-5]
         result = self.database.get(sql)
         if result:
+
+            # Check if the DynamicEntry is already loaded
+            for entry in self.entries:  # TODO: Fix this hacky fix to a ghost entry bug
+                if entry.matches(**kwargs):
+                    return entry
+
             entry = DynamicEntry(self, load_tuple=result[0])
             self.entries.append(entry)
             return entry
         else:
             return None
 
     def get_rows(self, **kwargs) -> List[DynamicEntry]:
@@ -269,29 +270,34 @@
         :param kwargs: The filters to apply to the query.
         :return: None
         """
         # For each column validate that it is a valid column and that the constraints are met.
         self._validate_columns(**kwargs)
         # self._contains_primary_keys(**kwargs)
 
-        entry = self.get_row(**kwargs)
-
-        if entry:
-            self.entries.remove(entry)
+        for entry in self.entries:
+            if entry.matches(**kwargs):
+                self.entries.remove(entry)
+                del entry
 
         # Build the query
         sql = f"DELETE FROM {self.table_name}"
         if len(kwargs) > 0:
             sql += " WHERE "
             for column_name in kwargs:
                 column = self.columns[self.columns.index(column_name)]
                 sql += self._create_filter(column, kwargs[column]) + " AND "
             sql = sql[:-5]
         result = self.database.run(sql)
-        return result
+        if result.rowcount == 0:
+            raise ValueError(f"No rows were deleted from table [{self.table_name}]")
+        elif result.rowcount > 1:
+            raise ValueError(f"Multiple rows were deleted from table [{self.table_name}]")
+        else:
+            return result
 
     def delete_many(self, **kwargs):
         """
         Deletes rows with values matching the kwargs
         :param kwargs:
         :return:
         """
```

### Comparing `ConcurrentDatabase-0.0.7/ConcurrentDatabase.egg-info/PKG-INFO` & `ConcurrentDatabase-0.0.8/ConcurrentDatabase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConcurrentDatabase
-Version: 0.0.7
+Version: 0.0.8
 Summary: A SQLite wrapper that allows for object oriented database access.
 Home-page: 
 Author: Jay S
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `ConcurrentDatabase-0.0.7/PKG-INFO` & `ConcurrentDatabase-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConcurrentDatabase
-Version: 0.0.7
+Version: 0.0.8
 Summary: A SQLite wrapper that allows for object oriented database access.
 Home-page: 
 Author: Jay S
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `ConcurrentDatabase-0.0.7/README.md` & `ConcurrentDatabase-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ConcurrentDatabase-0.0.7/pyproject.toml` & `ConcurrentDatabase-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [metadata]
 name = "ConcurrentDatabase"
 author = "Jay S"
 author_email = ""
-version = "0.0.7"
+version = "0.0.8"
 description = "A simple wrapper allow for treating an SQLite database as an object oriented structure"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `ConcurrentDatabase-0.0.7/setup.py` & `ConcurrentDatabase-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ConcurrentDatabase",
-    version="0.0.7",
+    version="0.0.8",
     author="Jay S",
     author_email="",
     description="A SQLite wrapper that allows for object oriented database access.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

