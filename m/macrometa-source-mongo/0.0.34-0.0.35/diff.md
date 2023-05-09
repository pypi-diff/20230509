# Comparing `tmp/macrometa-source-mongo-0.0.34.tar.gz` & `tmp/macrometa-source-mongo-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mongo-0.0.34.tar", max compression
+gzip compressed data, was "macrometa-source-mongo-0.0.35.tar", max compression
```

## Comparing `macrometa-source-mongo-0.0.34.tar` & `macrometa-source-mongo-0.0.35.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10765 2023-04-21 07:14:10.411421 macrometa-source-mongo-0.0.34/LICENSE
--rw-r--r--   0        0        0    21337 2023-04-21 07:14:10.411421 macrometa-source-mongo-0.0.34/macrometa_source_mongo/__init__.py
--rw-r--r--   0        0        0     6470 2023-04-21 07:14:10.411421 macrometa-source-mongo-0.0.34/macrometa_source_mongo/connection.py
--rw-r--r--   0        0        0     1151 2023-04-21 07:14:10.411421 macrometa-source-mongo-0.0.34/macrometa_source_mongo/exceptions.py
--rw-r--r--   0        0        0     8097 2023-04-21 07:14:10.411421 macrometa-source-mongo-0.0.34/macrometa_source_mongo/helper.py
--rw-r--r--   0        0        0    10251 2023-04-21 07:14:10.415421 macrometa-source-mongo-0.0.34/macrometa_source_mongo/sync_strategies/common.py
--rw-r--r--   0        0        0     3647 2023-04-21 07:14:10.415421 macrometa-source-mongo-0.0.34/macrometa_source_mongo/sync_strategies/full_table.py
--rw-r--r--   0        0        0     6267 2023-04-21 07:14:10.415421 macrometa-source-mongo-0.0.34/macrometa_source_mongo/sync_strategies/log_based.py
--rw-r--r--   0        0        0     2292 2023-04-21 07:14:10.415421 macrometa-source-mongo-0.0.34/macrometa_source_mongo/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1548 2023-04-21 07:14:10.699438 macrometa-source-mongo-0.0.34/pyproject.toml
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.34/setup.py
--rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.34/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-05-09 10:12:47.249009 macrometa-source-mongo-0.0.35/LICENSE
+-rw-r--r--   0        0        0    21337 2023-05-09 10:12:47.249009 macrometa-source-mongo-0.0.35/macrometa_source_mongo/__init__.py
+-rw-r--r--   0        0        0     6470 2023-05-09 10:12:47.249009 macrometa-source-mongo-0.0.35/macrometa_source_mongo/connection.py
+-rw-r--r--   0        0        0     1151 2023-05-09 10:12:47.249009 macrometa-source-mongo-0.0.35/macrometa_source_mongo/exceptions.py
+-rw-r--r--   0        0        0     8097 2023-05-09 10:12:47.249009 macrometa-source-mongo-0.0.35/macrometa_source_mongo/helper.py
+-rw-r--r--   0        0        0    10251 2023-05-09 10:12:47.249009 macrometa-source-mongo-0.0.35/macrometa_source_mongo/sync_strategies/common.py
+-rw-r--r--   0        0        0     3647 2023-05-09 10:12:47.249009 macrometa-source-mongo-0.0.35/macrometa_source_mongo/sync_strategies/full_table.py
+-rw-r--r--   0        0        0     6267 2023-05-09 10:12:47.249009 macrometa-source-mongo-0.0.35/macrometa_source_mongo/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     2292 2023-05-09 10:12:47.249009 macrometa-source-mongo-0.0.35/macrometa_source_mongo/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1548 2023-05-09 10:12:47.493013 macrometa-source-mongo-0.0.35/pyproject.toml
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.35/setup.py
+-rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.35/PKG-INFO
```

### Comparing `macrometa-source-mongo-0.0.34/LICENSE` & `macrometa-source-mongo-0.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.34/macrometa_source_mongo/__init__.py` & `macrometa-source-mongo-0.0.35/macrometa_source_mongo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,27 +134,27 @@
 
     def config(self) -> list[ConfigProperty]:
         """Get configuration parameters for the connector."""
         return [
             ConfigProperty('host', 'Host', ConfigAttributeType.STRING, True, False,
                            description='MongoDB host.',
                            placeholder_value='mongodb_host'),
-            ConfigProperty('port', 'Port', ConfigAttributeType.INT, True, False,
+            ConfigProperty('port', 'Port', ConfigAttributeType.INT, False, False,
                            description='MongoDB port.',
                            default_value='27017'),
             ConfigProperty('user', 'Username', ConfigAttributeType.STRING, True, False,
                            description='MongoDB user.',
                            placeholder_value='mongo'),
             ConfigProperty('password', 'Password', ConfigAttributeType.PASSWORD, True, False,
                            description='MongoDB password.',
                            placeholder_value='password'),
             ConfigProperty('auth_database', 'Auth Database', ConfigAttributeType.STRING, True, False,
                            description='MongoDB authentication database.',
                            default_value='admin'),
-            ConfigProperty('database', 'Database', ConfigAttributeType.STRING, True, False,
+            ConfigProperty('database', 'Database', ConfigAttributeType.STRING, True, True,
                            description='MongoDB database name.',
                            placeholder_value='mongo'),
             ConfigProperty('source_collection', 'Source Collection', ConfigAttributeType.STRING, True, True,
                            description="Source collection name.", placeholder_value="my_collection"),
             ConfigProperty('replication_method', 'Replication Method', ConfigAttributeType.STRING, False, False,
                            description='Choose from LOG_BASED, FULL_TABLE.',
                            default_value='FULL_TABLE'),
```

### Comparing `macrometa-source-mongo-0.0.34/macrometa_source_mongo/connection.py` & `macrometa-source-mongo-0.0.35/macrometa_source_mongo/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.34/macrometa_source_mongo/exceptions.py` & `macrometa-source-mongo-0.0.35/macrometa_source_mongo/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.34/macrometa_source_mongo/helper.py` & `macrometa-source-mongo-0.0.35/macrometa_source_mongo/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.34/macrometa_source_mongo/sync_strategies/common.py` & `macrometa-source-mongo-0.0.35/macrometa_source_mongo/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.34/macrometa_source_mongo/sync_strategies/full_table.py` & `macrometa-source-mongo-0.0.35/macrometa_source_mongo/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.34/macrometa_source_mongo/sync_strategies/log_based.py` & `macrometa-source-mongo-0.0.35/macrometa_source_mongo/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.34/macrometa_source_mongo/sync_strategies/sample_data.py` & `macrometa-source-mongo-0.0.35/macrometa_source_mongo/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.34/pyproject.toml` & `macrometa-source-mongo-0.0.35/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mongo"
-version='0.0.34'
+version='0.0.35'
 description = "Macrometa Source for extracting data from MongoDB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-mongo-0.0.34/setup.py` & `macrometa-source-mongo-0.0.35/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'tzlocal>=2.1.0,<2.2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mongo = macrometa_source_mongo:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mongo',
-    'version': '0.0.34',
+    'version': '0.0.35',
     'description': 'Macrometa Source for extracting data from MongoDB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mongo-0.0.34/PKG-INFO` & `macrometa-source-mongo-0.0.35/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mongo
-Version: 0.0.34
+Version: 0.0.35
 Summary: Macrometa Source for extracting data from MongoDB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MongoDB,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

