# Comparing `tmp/macrometa-source-collection-0.0.26.tar.gz` & `tmp/macrometa-source-collection-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.26.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.27.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.26.tar` & `macrometa-source-collection-0.0.27.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     8346 2023-05-02 07:14:48.605730 macrometa-source-collection-0.0.26/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     7978 2023-05-02 07:14:48.605730 macrometa-source-collection-0.0.26/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1623 2023-05-02 07:14:48.877739 macrometa-source-collection-0.0.26/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.26/setup.py
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.26/PKG-INFO
+-rw-r--r--   0        0        0     8346 2023-05-09 05:59:02.788937 macrometa-source-collection-0.0.27/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     8025 2023-05-09 05:59:02.788937 macrometa-source-collection-0.0.27/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1623 2023-05-09 05:59:03.028937 macrometa-source-collection-0.0.27/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.27/setup.py
+-rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.27/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.26/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.27/macrometa_source_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.26/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.27/macrometa_source_collection/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,15 @@
                             for key in j.keys()
                         ):
                             j['_sdc_deleted_at'] = None
                             singer_record = self.msg_to_singer_message(stream, j, None, utils.now())
                             singer.write_message(singer_record)
                     elif props["op"] == "DELETE":
                         # Currently, we don't have a way to validate schema here
+                        j.pop('_delete', None)
                         j['_sdc_deleted_at'] = singer.utils.strftime(utils.now())
                         singer_record = self.msg_to_singer_message(stream, j, None, utils.now())
                         singer.write_message(singer_record)
                     self.exported_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(data))
                     self.exported_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                     time = datetime.fromtimestamp(msg.publish_timestamp()/1000)
                     time_str = time.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
```

### Comparing `macrometa-source-collection-0.0.26/pyproject.toml` & `macrometa-source-collection-0.0.27/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.26'
+version='0.0.27'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.26/setup.py` & `macrometa-source-collection-0.0.27/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.26',
+    'version': '0.0.27',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.26/PKG-INFO` & `macrometa-source-collection-0.0.27/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.26
+Version: 0.0.27
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Tap
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

