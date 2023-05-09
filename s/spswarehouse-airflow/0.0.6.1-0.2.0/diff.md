# Comparing `tmp/spswarehouse_airflow-0.0.6.1.tar.gz` & `tmp/spswarehouse_airflow-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spswarehouse_airflow-0.0.6.1.tar", last modified: Fri Dec 23 15:28:05 2022, max compression
+gzip compressed data, was "spswarehouse_airflow-0.2.0.tar", last modified: Tue May  9 16:15:05 2023, max compression
```

## Comparing `spswarehouse_airflow-0.0.6.1.tar` & `spswarehouse_airflow-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-12-23 15:28:05.017222 spswarehouse_airflow-0.0.6.1/
--rw-rw-rw-   0        0        0    35823 2022-12-08 23:05:42.000000 spswarehouse_airflow-0.0.6.1/LICENSE
--rw-rw-rw-   0        0        0      448 2022-12-08 23:05:42.000000 spswarehouse_airflow-0.0.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2036 2022-12-23 15:28:05.016169 spswarehouse_airflow-0.0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     1634 2022-12-08 23:05:42.000000 spswarehouse_airflow-0.0.6.1/README.md
--rw-rw-rw-   0        0        0       42 2022-12-23 15:28:05.017222 spswarehouse_airflow-0.0.6.1/setup.cfg
--rw-rw-rw-   0        0        0      739 2022-12-23 15:27:21.000000 spswarehouse_airflow-0.0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-23 15:28:05.006671 spswarehouse_airflow-0.0.6.1/spswarehouse_airflow/
--rw-rw-rw-   0        0        0      548 2022-12-20 21:53:23.000000 spswarehouse_airflow-0.0.6.1/spswarehouse_airflow/__init__.py
--rw-rw-rw-   0        0        0     2326 2022-12-23 15:26:09.000000 spswarehouse_airflow-0.0.6.1/spswarehouse_airflow/googledrive.py
--rw-rw-rw-   0        0        0     1556 2022-12-23 15:26:16.000000 spswarehouse_airflow-0.0.6.1/spswarehouse_airflow/googlesheets.py
--rw-rw-rw-   0        0        0     1374 2022-12-23 15:26:22.000000 spswarehouse_airflow-0.0.6.1/spswarehouse_airflow/googleslides.py
--rw-rw-rw-   0        0        0     1271 2022-12-08 23:05:42.000000 spswarehouse_airflow-0.0.6.1/spswarehouse_airflow/table_names.py
--rw-rw-rw-   0        0        0     7061 2022-12-08 23:07:18.000000 spswarehouse_airflow-0.0.6.1/spswarehouse_airflow/table_utils.py
--rw-rw-rw-   0        0        0     5064 2022-12-08 23:05:42.000000 spswarehouse_airflow-0.0.6.1/spswarehouse_airflow/warehouse.py
-drwxrwxrwx   0        0        0        0 2022-12-23 15:28:05.014601 spswarehouse_airflow-0.0.6.1/spswarehouse_airflow.egg-info/
--rw-rw-rw-   0        0        0     2036 2022-12-23 15:28:04.000000 spswarehouse_airflow-0.0.6.1/spswarehouse_airflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2022-12-23 15:28:04.000000 spswarehouse_airflow-0.0.6.1/spswarehouse_airflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-23 15:28:04.000000 spswarehouse_airflow-0.0.6.1/spswarehouse_airflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2022-12-23 15:28:04.000000 spswarehouse_airflow-0.0.6.1/spswarehouse_airflow.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 16:15:05.909099 spswarehouse_airflow-0.2.0/
+-rw-rw-rw-   0        0        0    35823 2022-12-08 23:05:42.000000 spswarehouse_airflow-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      448 2022-12-08 23:05:42.000000 spswarehouse_airflow-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2034 2023-05-09 16:15:05.907088 spswarehouse_airflow-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1634 2022-12-08 23:05:42.000000 spswarehouse_airflow-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-09 16:15:05.909099 spswarehouse_airflow-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1101 2023-05-09 16:12:13.000000 spswarehouse_airflow-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:15:05.888659 spswarehouse_airflow-0.2.0/spswarehouse_airflow/
+-rw-rw-rw-   0        0        0      548 2022-12-20 21:53:23.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/__init__.py
+-rw-rw-rw-   0        0        0     1060 2023-05-09 15:37:21.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/calpads.py
+-rw-rw-rw-   0        0        0     2326 2022-12-23 15:26:09.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/googledrive.py
+-rw-rw-rw-   0        0        0     1556 2022-12-23 15:26:16.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/googlesheets.py
+-rw-rw-rw-   0        0        0     1374 2022-12-23 15:26:22.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/googleslides.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:15:05.904087 spswarehouse_airflow-0.2.0/spswarehouse_airflow/powerschool/
+-rw-rw-rw-   0        0        0        0 2023-05-09 15:51:57.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/powerschool/__init__.py
+-rw-rw-rw-   0        0        0     1112 2023-05-08 21:52:17.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/powerschool/powerschool.py
+-rw-rw-rw-   0        0        0      989 2023-05-09 15:56:21.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/powerschool/powerschool_calpads.py
+-rw-rw-rw-   0        0        0     1271 2022-12-08 23:05:42.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/table_names.py
+-rw-rw-rw-   0        0        0     7195 2023-01-05 16:34:44.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/table_utils.py
+-rw-rw-rw-   0        0        0     4978 2022-12-23 15:33:36.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow/warehouse.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:15:05.897739 spswarehouse_airflow-0.2.0/spswarehouse_airflow.egg-info/
+-rw-rw-rw-   0        0        0     2034 2023-05-09 16:15:05.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      687 2023-05-09 16:15:05.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 16:15:05.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      225 2023-05-09 16:15:05.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-09 16:15:05.000000 spswarehouse_airflow-0.2.0/spswarehouse_airflow.egg-info/top_level.txt
```

### Comparing `spswarehouse_airflow-0.0.6.1/LICENSE` & `spswarehouse_airflow-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spswarehouse_airflow-0.0.6.1/PKG-INFO` & `spswarehouse_airflow-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spswarehouse_airflow
-Version: 0.0.6.1
+Version: 0.2.0
 Summary: Summit Public Schools Snowflake warehouse for use in Airflow
 Home-page: https://github.com/SummitPublicSchools/spswarehouse_airflow
 Author: Harry Li Consulting, LLC
 Author-email: hcli.consulting@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spswarehouse_airflow-0.0.6.1/README.md` & `spswarehouse_airflow-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `spswarehouse_airflow-0.0.6.1/setup.py` & `spswarehouse_airflow-0.2.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spswarehouse_airflow",
-    version="0.0.6.1",
+    version="0.2.0",
     author="Harry Li Consulting, LLC",
     author_email="hcli.consulting@gmail.com",
     description="Summit Public Schools Snowflake warehouse for use in Airflow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SummitPublicSchools/spswarehouse_airflow",
     packages=setuptools.find_packages(),
     # This needs to be set so you get the files included by MANIFEST.in
     # when you run "pip install"
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
+    install_requires=[
+        'pandas==1.5.2',
+        'SQLAlchemy==1.4.44',
+        'snowflake-sqlalchemy==1.4.4',
+        'google-api-python-client==1.12.11',
+        'google-auth-httplib2==0.1.0',
+        'google-auth-oauthlib==0.7.1',
+        'gspread==5.7.2',
+        'PyDrive2==1.15.0',
+        'spswarehouse>=0.1.1',
+        'apache-airflow<=2.5.0',
+    ]
 )
```

### Comparing `spswarehouse_airflow-0.0.6.1/spswarehouse_airflow/__init__.py` & `spswarehouse_airflow-0.2.0/spswarehouse_airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `spswarehouse_airflow-0.0.6.1/spswarehouse_airflow/googledrive.py` & `spswarehouse_airflow-0.2.0/spswarehouse_airflow/googledrive.py`

 * *Files identical despite different names*

### Comparing `spswarehouse_airflow-0.0.6.1/spswarehouse_airflow/googlesheets.py` & `spswarehouse_airflow-0.2.0/spswarehouse_airflow/googlesheets.py`

 * *Files identical despite different names*

### Comparing `spswarehouse_airflow-0.0.6.1/spswarehouse_airflow/googleslides.py` & `spswarehouse_airflow-0.2.0/spswarehouse_airflow/googleslides.py`

 * *Files identical despite different names*

### Comparing `spswarehouse_airflow-0.0.6.1/spswarehouse_airflow/table_names.py` & `spswarehouse_airflow-0.2.0/spswarehouse_airflow/table_names.py`

 * *Files identical despite different names*

### Comparing `spswarehouse_airflow-0.0.6.1/spswarehouse_airflow/table_utils.py` & `spswarehouse_airflow-0.2.0/spswarehouse_airflow/table_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pandas as pd
 import numpy as np
 import os
+import random
+import string
 
 import logging
 
 from .warehouse import create_warehouse
 from .googledrive import GoogleDrive
 
 DEFAULT_ENCODING='utf-8'
@@ -80,15 +82,16 @@
             df = pd.DataFrame(google_sheet.get_all_records())
     elif csv_filename is not None:
         if force_string:
             df = pd.read_csv(csv_filename, encoding=encoding, dtype=str)
         else:
             df = pd.read_csv(csv_filename, encoding=encoding)
     elif google_drive_id is not None:
-        filename = pd.util.testing.rands_array(10,1)[0] + '.csv'
+        letters = string.ascii_letters
+        filename = ''.join(random.choice(letters) for i in range(10)) + '.csv'
         tempFile = GoogleDrive.CreateFile({'id': google_drive_id})
         tempFile.GetContentFile(filename)
         try:
             if force_string:
                 df = pd.read_csv(filename, encoding=encoding, dtype=str)
             else:
                 df = pd.read_csv(filename, encoding=encoding)
@@ -152,15 +155,16 @@
             df = pd.DataFrame(google_sheet.get_all_records())
     elif csv_filename is not None:
         if force_string:
             df = pd.read_csv(csv_filename, encoding=encoding, dtype=str)
         else:
             df = pd.read_csv(csv_filename, encoding=encoding)
     elif google_drive_id is not None:
-        filename = pd.util.testing.rands_array(10,1)[0] + '.csv'
+        letters = string.ascii_letters
+        filename = ''.join(random.choice(letters) for i in range(10)) + '.csv'
         tempFile = GoogleDrive.CreateFile({'id': google_drive_id})
         tempFile.GetContentFile(filename)
         try:
             if force_string:
                 df = pd.read_csv(filename, encoding=encoding, dtype=str)
             else:
                 df = pd.read_csv(filename, encoding=encoding)
```

### Comparing `spswarehouse_airflow-0.0.6.1/spswarehouse_airflow/warehouse.py` & `spswarehouse_airflow-0.2.0/spswarehouse_airflow/warehouse.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,135 +1,136 @@
-import pandas
-
-from airflow.hooks.base_hook import BaseHook
-from sqlalchemy.engine.url import URL
-from sqlalchemy import create_engine, MetaData, Table
-from sqlalchemy.engine import reflection
-from snowflake.sqlalchemy import VARIANT
-
-from datetime import date
-
-snowflake_conn_id = 'snowflake_default'
-snowflake_conn = BaseHook.get_connection(snowflake_conn_id)
-
-
-def describe(table):
-    for c in table.columns:
-        tipe = c.type
-        if isinstance(tipe, VARIANT):
-             tipe = 'VARIANT'
-        print('{}: {}'.format(c.name, tipe))
-
-class Warehouse:
-    """
-    This class is an abstraction that allows you to connect to the Snowflake Warehouse.
-    It has several methods that allow for easy access to the warehouse.
-    -- execute: run some arbitrary SQL in the warehouse. totally safe!
-    -- read_sql: execute a SELECT statement and return results as a pandas.DataFrame
-    -- reflect: return a SQLAlchemy Table object containing metadata about the table
-
-    This class also has a couple of SQLAlchemy-based instance variables
-    - engine: contains information about how to connect to the warehouse
-    - insp: a SQLAlchemy inspector object that lets query metadata about the warehouse
-            e.g., Snowflake.insp.get_table_names('wild_west')
-    """
-    def __init__(self, engine):
-        self.engine = engine
-        self.meta = MetaData(bind=engine)
-        self._insp = None
-        self._conn = None
-        self.loaded_tables = {}   # dictionary of Table objects keyed by "schema.table_name"
-
-    @property
-    def insp(self):
-        if self._insp is None:
-            self._insp = reflection.Inspector.from_engine(self.engine)
-        return self._insp
-
-    @property
-    def conn(self):
-        if self._conn is None:
-            self._conn = self.engine.connect()
-        return self._conn
-
-    # caller is responsible for closing the connection when done
-    def execute(self, sql):
-        """
-        execute: SQL statement -> (connection, proxy)
-
-        Running the execute method sends the SQL string to the warehouse using
-        this object's connection object. The return value is a tuple of the
-        connection object and the SQLAlchemy proxy object returned from executing
-        the SQL.
-        """
-        return self.conn, self.conn.execute(sql)
-
-    def read_sql(self, sql):
-        """
-        read_sql: 'SELECT ...' -> pandas.DataFrame
-        read_sql: SQLAlchemy select object -> pandas.DataFrame
-
-        The warehouse read_sql method is a minimalist wrapper around the pandas.read_sql
-        method. The sole argument to this method can either be a string (typically a SELECT statement)
-        or an object constructed using SQLAlchemy's select method.
-        """
-        return pandas.read_sql(sql, self.engine)
-
-    def reflect(self, table_or_view, schema):
-        """
-        reflect: table name, schema name (optional) -> SQLAlchemy Table object
-        reflect: view name,  schema name (optional) -> SQLAlchemy Table object
-
-        The reflect method is useful to grab the underlying metadata for a table in the warehouse.
-        Using the returned value, you can print out the column names and types using the describe method.
-
-        Note that if the table or view name has a '.' in it, then this method will try to infer the schema name
-        and ignore the passed in argument
-
-        t_table = Snowflake.reflect('users', schema='staging_scrapes')
-        describe(t_table)
-        """
-        name_with_schema = '{schema}.{table_or_view}'.format(
-            schema=schema,
-            table_or_view=table_or_view
-        )
-
-        # if it's already been loaded, why bother loading it again? just return it
-        table = self.loaded_tables.get(name_with_schema, None)
-        if table is not None:
-            return table
-
-        table = Table(table_or_view, self.meta, autoload=True, schema=schema)
-
-        # sets the column names explicitly on the instance so that tab-completion is easy
-        for c in table.columns:
-            setattr(table, 'c_{}'.format(c.name), c)
-
-        # save so we don't have to load it again later
-        self.loaded_tables[name_with_schema] = table
-
-        return table
-    
-    def close(self):
-        self.conn.close()
-
-
-extras_dict = snowflake_conn.extra_dejson
-schema = snowflake_conn.schema.lower() if isinstance(snowflake_conn.schema, str) else None
-
-def create_warehouse():
-    warehouse = Warehouse(
-        create_engine(
-            'snowflake://{user}:{password}@{account}/{db}/{schema}?warehouse={warehouse}'.format(
-                user=snowflake_conn.login,
-                password=snowflake_conn.password,
-                account=extras_dict['account'].lower(),
-                db=extras_dict['database'].lower(),
-                schema=schema,
-                warehouse=extras_dict['warehouse'].lower(),
-            ),
-            pool_size=1,
-        )
-    )
-    return warehouse
-
+import pandas
+
+from airflow.hooks.base_hook import BaseHook
+from sqlalchemy.engine.url import URL
+from sqlalchemy import create_engine, MetaData, Table
+from sqlalchemy.engine import reflection
+from snowflake.sqlalchemy import VARIANT
+
+from datetime import date
+from urllib.parse import quote_plus
+
+snowflake_conn_id = 'snowflake_default'
+snowflake_conn = BaseHook.get_connection(snowflake_conn_id)
+
+
+def describe(table):
+    for c in table.columns:
+        tipe = c.type
+        if isinstance(tipe, VARIANT):
+             tipe = 'VARIANT'
+        print('{}: {}'.format(c.name, tipe))
+
+class Warehouse:
+    """
+    This class is an abstraction that allows you to connect to the Snowflake Warehouse.
+    It has several methods that allow for easy access to the warehouse.
+    -- execute: run some arbitrary SQL in the warehouse. totally safe!
+    -- read_sql: execute a SELECT statement and return results as a pandas.DataFrame
+    -- reflect: return a SQLAlchemy Table object containing metadata about the table
+
+    This class also has a couple of SQLAlchemy-based instance variables
+    - engine: contains information about how to connect to the warehouse
+    - insp: a SQLAlchemy inspector object that lets query metadata about the warehouse
+            e.g., Snowflake.insp.get_table_names('wild_west')
+    """
+    def __init__(self, engine):
+        self.engine = engine
+        self.meta = MetaData(bind=engine)
+        self._insp = None
+        self._conn = None
+        self.loaded_tables = {}   # dictionary of Table objects keyed by "schema.table_name"
+
+    @property
+    def insp(self):
+        if self._insp is None:
+            self._insp = reflection.Inspector.from_engine(self.engine)
+        return self._insp
+
+    @property
+    def conn(self):
+        if self._conn is None:
+            self._conn = self.engine.connect()
+        return self._conn
+
+    # caller is responsible for closing the connection when done
+    def execute(self, sql):
+        """
+        execute: SQL statement -> (connection, proxy)
+
+        Running the execute method sends the SQL string to the warehouse using
+        this object's connection object. The return value is a tuple of the
+        connection object and the SQLAlchemy proxy object returned from executing
+        the SQL.
+        """
+        return self.conn, self.conn.execute(sql)
+
+    def read_sql(self, sql):
+        """
+        read_sql: 'SELECT ...' -> pandas.DataFrame
+        read_sql: SQLAlchemy select object -> pandas.DataFrame
+
+        The warehouse read_sql method is a minimalist wrapper around the pandas.read_sql
+        method. The sole argument to this method can either be a string (typically a SELECT statement)
+        or an object constructed using SQLAlchemy's select method.
+        """
+        return pandas.read_sql(sql, self.engine)
+
+    def reflect(self, table_or_view, schema):
+        """
+        reflect: table name, schema name (optional) -> SQLAlchemy Table object
+        reflect: view name,  schema name (optional) -> SQLAlchemy Table object
+
+        The reflect method is useful to grab the underlying metadata for a table in the warehouse.
+        Using the returned value, you can print out the column names and types using the describe method.
+
+        Note that if the table or view name has a '.' in it, then this method will try to infer the schema name
+        and ignore the passed in argument
+
+        t_table = Snowflake.reflect('users', schema='staging_scrapes')
+        describe(t_table)
+        """
+        name_with_schema = '{schema}.{table_or_view}'.format(
+            schema=schema,
+            table_or_view=table_or_view
+        )
+
+        # if it's already been loaded, why bother loading it again? just return it
+        table = self.loaded_tables.get(name_with_schema, None)
+        if table is not None:
+            return table
+
+        table = Table(table_or_view, self.meta, autoload=True, schema=schema)
+
+        # sets the column names explicitly on the instance so that tab-completion is easy
+        for c in table.columns:
+            setattr(table, 'c_{}'.format(c.name), c)
+
+        # save so we don't have to load it again later
+        self.loaded_tables[name_with_schema] = table
+
+        return table
+    
+    def close(self):
+        self.conn.close()
+
+
+extras_dict = snowflake_conn.extra_dejson
+schema = snowflake_conn.schema.lower() if isinstance(snowflake_conn.schema, str) else None
+
+def create_warehouse():
+    warehouse = Warehouse(
+        create_engine(
+            'snowflake://{user}:{password}@{account}/{db}/{schema}?warehouse={warehouse}'.format(
+                user=snowflake_conn.login,
+                password=quote_plus(snowflake_conn.password),
+                account=extras_dict['account'].lower(),
+                db=extras_dict['database'].lower(),
+                schema=schema,
+                warehouse=extras_dict['warehouse'].lower(),
+            ),
+            pool_size=1,
+        )
+    )
+    return warehouse
+
```

### Comparing `spswarehouse_airflow-0.0.6.1/spswarehouse_airflow.egg-info/PKG-INFO` & `spswarehouse_airflow-0.2.0/spswarehouse_airflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spswarehouse-airflow
-Version: 0.0.6.1
+Version: 0.2.0
 Summary: Summit Public Schools Snowflake warehouse for use in Airflow
 Home-page: https://github.com/SummitPublicSchools/spswarehouse_airflow
 Author: Harry Li Consulting, LLC
 Author-email: hcli.consulting@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

