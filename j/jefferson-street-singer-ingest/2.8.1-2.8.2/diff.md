# Comparing `tmp/jefferson-street-singer-ingest-2.8.1.tar.gz` & `tmp/jefferson-street-singer-ingest-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jefferson-street-singer-ingest-2.8.1.tar", max compression
+gzip compressed data, was "jefferson-street-singer-ingest-2.8.2.tar", max compression
```

## Comparing `jefferson-street-singer-ingest-2.8.1.tar` & `jefferson-street-singer-ingest-2.8.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-01-29 20:58:43.197928 jefferson-street-singer-ingest-2.8.1/README.md
--rw-r--r--   0        0        0      178 2023-01-29 20:58:43.198639 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/__init__.py
--rw-r--r--   0        0        0      370 2023-01-29 20:58:43.199118 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/__init__.py
--rw-r--r--   0        0        0      114 2023-01-29 20:58:43.199575 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/entry/__init__.py
--rw-r--r--   0        0        0     3026 2023-04-03 18:38:45.473683 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/entry/run_command.py
--rw-r--r--   0        0        0      863 2023-03-06 06:51:51.165998 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/state/ingest_bookmark.py
--rw-r--r--   0        0        0     3146 2023-04-11 01:01:56.530521 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/state/state_management.py
--rw-r--r--   0        0        0      186 2023-01-29 20:58:43.200092 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/stream/__init__.py
--rw-r--r--   0        0        0     4323 2023-03-06 06:51:51.166341 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/stream/base_tap_stream.py
--rw-r--r--   0        0        0     5413 2023-04-11 00:54:06.673010 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/stream/rest_stream.py
--rw-r--r--   0        0        0       88 2023-01-29 20:58:43.201272 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/tap/__init__.py
--rw-r--r--   0        0        0     7917 2023-01-29 20:58:43.201522 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/tap/base_tap.py
--rw-r--r--   0        0        0      145 2023-01-29 20:58:43.201963 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/target/__init__.py
--rw-r--r--   0        0        0     1009 2023-01-29 20:58:43.202097 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/target/avro_generator.py
--rw-r--r--   0        0        0     2111 2023-01-29 20:58:43.202352 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/target/base_google_cloud_storage_target.py
--rw-r--r--   0        0        0      632 2023-04-11 01:05:28.425111 jefferson-street-singer-ingest-2.8.1/pyproject.toml
--rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 jefferson-street-singer-ingest-2.8.1/setup.py
--rw-r--r--   0        0        0      770 1970-01-01 00:00:00.000000 jefferson-street-singer-ingest-2.8.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-01-29 20:58:43.197928 jefferson-street-singer-ingest-2.8.2/README.md
+-rw-r--r--   0        0        0      178 2023-01-29 20:58:43.198639 jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/__init__.py
+-rw-r--r--   0        0        0      370 2023-01-29 20:58:43.199118 jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/__init__.py
+-rw-r--r--   0        0        0      114 2023-01-29 20:58:43.199575 jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/entry/__init__.py
+-rw-r--r--   0        0        0     3026 2023-04-19 00:26:26.695996 jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/entry/run_command.py
+-rw-r--r--   0        0        0      863 2023-04-19 00:26:26.696220 jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/state/ingest_bookmark.py
+-rw-r--r--   0        0        0     3146 2023-04-19 00:26:26.696432 jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/state/state_management.py
+-rw-r--r--   0        0        0      186 2023-01-29 20:58:43.200092 jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/stream/__init__.py
+-rw-r--r--   0        0        0     4323 2023-04-19 00:26:26.696749 jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/stream/base_tap_stream.py
+-rw-r--r--   0        0        0     5413 2023-04-19 00:26:26.697031 jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/stream/rest_stream.py
+-rw-r--r--   0        0        0       88 2023-01-29 20:58:43.201272 jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/tap/__init__.py
+-rw-r--r--   0        0        0     7917 2023-01-29 20:58:43.201522 jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/tap/base_tap.py
+-rw-r--r--   0        0        0      145 2023-01-29 20:58:43.201963 jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/target/__init__.py
+-rw-r--r--   0        0        0     1009 2023-01-29 20:58:43.202097 jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/target/avro_generator.py
+-rw-r--r--   0        0        0     2230 2023-05-08 23:30:46.165105 jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/target/base_google_cloud_storage_target.py
+-rw-r--r--   0        0        0      632 2023-05-08 23:32:48.231361 jefferson-street-singer-ingest-2.8.2/pyproject.toml
+-rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 jefferson-street-singer-ingest-2.8.2/setup.py
+-rw-r--r--   0        0        0      770 1970-01-01 00:00:00.000000 jefferson-street-singer-ingest-2.8.2/PKG-INFO
```

### Comparing `jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/entry/run_command.py` & `jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/entry/run_command.py`

 * *Files identical despite different names*

### Comparing `jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/state/ingest_bookmark.py` & `jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/state/ingest_bookmark.py`

 * *Files identical despite different names*

### Comparing `jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/state/state_management.py` & `jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/state/state_management.py`

 * *Files identical despite different names*

### Comparing `jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/stream/base_tap_stream.py` & `jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/stream/base_tap_stream.py`

 * *Files identical despite different names*

### Comparing `jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/stream/rest_stream.py` & `jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/stream/rest_stream.py`

 * *Files identical despite different names*

### Comparing `jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/tap/base_tap.py` & `jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/tap/base_tap.py`

 * *Files identical despite different names*

### Comparing `jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/target/avro_generator.py` & `jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/target/avro_generator.py`

 * *Files identical despite different names*

### Comparing `jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/target/base_google_cloud_storage_target.py` & `jefferson-street-singer-ingest-2.8.2/jefferson_street_singer_ingest/services/target/base_google_cloud_storage_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,17 @@
             if json_line["type"] == "SCHEMA":
                 self.current_name = json_line["stream"]
                 self.current_fields = json_line["schema"]["properties"].keys()
                 self.current_avro_schema = build_avro_schema(
                     self.current_fields, self.current_name
                 )
 
+                build_avro_file(
+                    self.current_name, self.current_avro_schema, []
+                )
                 self.avro_files.append(f"{self.current_name}.avro")
             if json_line["type"] == "RECORD":
                 build_avro_file(
                     self.current_name, self.current_avro_schema, [json_line["record"]]
                 )
 
     def upload_avro_to_gcs(self, bucket_name, source_file_name):
```

### Comparing `jefferson-street-singer-ingest-2.8.1/pyproject.toml` & `jefferson-street-singer-ingest-2.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jefferson-street-singer-ingest"
-version = "2.8.1"
+version = "2.8.2"
 description = "Library holding the taps and targets for Jefferson Street Ingestion"
 authors = ["Nikolai McFall <nikolai@jeffersonst.io>"]
 readme = "README.md"
 packages = [{include = "jefferson_street_singer_ingest"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.9"
```

### Comparing `jefferson-street-singer-ingest-2.8.1/setup.py` & `jefferson-street-singer-ingest-2.8.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'pandas>=1.4.4,<2.0.0',
  'rec-avro>=0.0.4,<0.0.5',
  'requests>=2.28.1,<3.0.0',
  'singer-sdk==0.1.6']
 
 setup_kwargs = {
     'name': 'jefferson-street-singer-ingest',
-    'version': '2.8.1',
+    'version': '2.8.2',
     'description': 'Library holding the taps and targets for Jefferson Street Ingestion',
     'long_description': '',
     'author': 'Nikolai McFall',
     'author_email': 'nikolai@jeffersonst.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `jefferson-street-singer-ingest-2.8.1/PKG-INFO` & `jefferson-street-singer-ingest-2.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jefferson-street-singer-ingest
-Version: 2.8.1
+Version: 2.8.2
 Summary: Library holding the taps and targets for Jefferson Street Ingestion
 Author: Nikolai McFall
 Author-email: nikolai@jeffersonst.io
 Requires-Python: >=3.8,<3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: fastavro (>=1.6.1,<2.0.0)
```

