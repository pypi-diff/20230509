# Comparing `tmp/monarch_py-0.7.2.tar.gz` & `tmp/monarch_py-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monarch_py-0.7.2.tar", max compression
+gzip compressed data, was "monarch_py-0.7.3.tar", max compression
```

## Comparing `monarch_py-0.7.2.tar` & `monarch_py-0.7.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      955 2023-05-05 20:41:42.065764 monarch_py-0.7.2/pyproject.toml
--rw-r--r--   0        0        0       77 2023-05-05 20:41:42.065764 monarch_py-0.7.2/src/monarch_py/__init__.py
--rw-r--r--   0        0        0     1587 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/association_type_mappings.yaml
--rw-r--r--   0        0        0     6581 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/cli.py
--rw-r--r--   0        0        0        0 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/datamodels/__init__.py
--rw-r--r--   0        0        0     8802 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/datamodels/model.py
--rw-r--r--   0        0        0     7857 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/datamodels/model.yaml
--rw-r--r--   0        0        0     3300 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/datamodels/solr.py
--rw-r--r--   0        0        0        0 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/implementations/solr/__init__.py
--rw-r--r--   0        0        0    17565 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/implementations/solr/solr_implementation.py
--rw-r--r--   0        0        0        0 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/implementations/sql/__init__.py
--rw-r--r--   0        0        0     8909 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/implementations/sql/sql_implementation.py
--rw-r--r--   0        0        0        0 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/interfaces/__init__.py
--rw-r--r--   0        0        0     2343 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/interfaces/association_interface.py
--rw-r--r--   0        0        0      985 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/interfaces/entity_interface.py
--rw-r--r--   0        0        0      890 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/interfaces/query_interface.py
--rw-r--r--   0        0        0     3737 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/interfaces/search_interface.py
--rw-r--r--   0        0        0        0 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/service/__init__.py
--rw-r--r--   0        0        0     2052 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/service/solr_service.py
--rw-r--r--   0        0        0     8133 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/solr_cli.py
--rw-r--r--   0        0        0     3330 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/sql_cli.py
--rw-r--r--   0        0        0        0 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/utils/__init__.py
--rw-r--r--   0        0        0     4052 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/utils/association_type_utils.py
--rw-r--r--   0        0        0     3985 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/utils/solr_cli_utils.py
--rw-r--r--   0        0        0     4937 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/utils/utils.py
--rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      955 2023-05-08 22:37:25.046450 monarch_py-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/__init__.py
+-rw-r--r--   0        0        0     1587 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/association_type_mappings.yaml
+-rw-r--r--   0        0        0     6581 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/cli.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/datamodels/__init__.py
+-rw-r--r--   0        0        0     8802 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/datamodels/model.py
+-rw-r--r--   0        0        0     7913 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/datamodels/model.yaml
+-rw-r--r--   0        0        0     3300 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/datamodels/solr.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/implementations/solr/__init__.py
+-rw-r--r--   0        0        0    17565 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/implementations/solr/solr_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/implementations/sql/__init__.py
+-rw-r--r--   0        0        0     8909 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/implementations/sql/sql_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/interfaces/__init__.py
+-rw-r--r--   0        0        0     2343 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/interfaces/association_interface.py
+-rw-r--r--   0        0        0      985 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/interfaces/entity_interface.py
+-rw-r--r--   0        0        0      890 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/interfaces/query_interface.py
+-rw-r--r--   0        0        0     3737 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/interfaces/search_interface.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/service/__init__.py
+-rw-r--r--   0        0        0     2052 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/service/solr_service.py
+-rw-r--r--   0        0        0     8133 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/solr_cli.py
+-rw-r--r--   0        0        0     3330 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/sql_cli.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/utils/__init__.py
+-rw-r--r--   0        0        0     4052 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/utils/association_type_utils.py
+-rw-r--r--   0        0        0     3985 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/utils/solr_cli_utils.py
+-rw-r--r--   0        0        0     4937 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/utils/utils.py
+-rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.7.3/PKG-INFO
```

### Comparing `monarch_py-0.7.2/pyproject.toml` & `monarch_py-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monarch-py"
-version = "0.7.2"
+version = "0.7.3"
 description = "Monarch Initiative data access library"
 authors = [
     "Kevin Schaper <kevin@tislab.org>",
     "Glass Elsarboukh <glass@tislab.org>",
     "The Monarch Initiative <info@monarchinitiative.org>"
 ]
 packages = [
```

### Comparing `monarch_py-0.7.2/src/monarch_py/association_type_mappings.yaml` & `monarch_py-0.7.3/src/monarch_py/association_type_mappings.yaml`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.2/src/monarch_py/cli.py` & `monarch_py-0.7.3/src/monarch_py/cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.2/src/monarch_py/datamodels/model.py` & `monarch_py-0.7.3/src/monarch_py/datamodels/model.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.2/src/monarch_py/datamodels/model.yaml` & `monarch_py-0.7.3/src/monarch_py/datamodels/model.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,14 @@
       - highlight
       - score
     slot_usage:
       category:
         required: true
       name:
         required: true
-
   SearchResults:
     is_a: Results
     slots:
       - items
       - facet_fields
       - facet_queries
     slot_usage:
@@ -259,14 +258,15 @@
     required: true
   name:
     range: string
   negated:
     range: boolean
   object:
     range: string
+    required: true
   object_category:
     multivalued: true
   object_closure:
     multivalued: true
   object_closure_label:
     multivalued: true
   object_label:
@@ -284,14 +284,15 @@
   original_subject:
     range: string
   pathway:
     range: string
   predicate:
     multivalued: false
     range: string
+    required: true
   primary_knowledge_source:
     multivalued: true
   provided_by:
     range: string
   publications:
     multivalued: true
   qualifiers:
@@ -304,14 +305,15 @@
     range: string
   source:
     range: string
   stage_qualifier:
     range: string
   subject:
     range: string
+    required: true
   subject_category:
     multivalued: true
   subject_closure:
     multivalued: true
   subject_closure_label:
     multivalued: true
   subject_label:
```

### Comparing `monarch_py-0.7.2/src/monarch_py/datamodels/solr.py` & `monarch_py-0.7.3/src/monarch_py/datamodels/solr.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.2/src/monarch_py/implementations/solr/solr_implementation.py` & `monarch_py-0.7.3/src/monarch_py/implementations/solr/solr_implementation.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.2/src/monarch_py/implementations/sql/sql_implementation.py` & `monarch_py-0.7.3/src/monarch_py/implementations/sql/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.2/src/monarch_py/interfaces/association_interface.py` & `monarch_py-0.7.3/src/monarch_py/interfaces/association_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.2/src/monarch_py/interfaces/entity_interface.py` & `monarch_py-0.7.3/src/monarch_py/interfaces/entity_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.2/src/monarch_py/interfaces/query_interface.py` & `monarch_py-0.7.3/src/monarch_py/interfaces/query_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.2/src/monarch_py/interfaces/search_interface.py` & `monarch_py-0.7.3/src/monarch_py/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.2/src/monarch_py/service/solr_service.py` & `monarch_py-0.7.3/src/monarch_py/service/solr_service.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.2/src/monarch_py/solr_cli.py` & `monarch_py-0.7.3/src/monarch_py/solr_cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.2/src/monarch_py/sql_cli.py` & `monarch_py-0.7.3/src/monarch_py/sql_cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.2/src/monarch_py/utils/association_type_utils.py` & `monarch_py-0.7.3/src/monarch_py/utils/association_type_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.2/src/monarch_py/utils/solr_cli_utils.py` & `monarch_py-0.7.3/src/monarch_py/utils/solr_cli_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.2/src/monarch_py/utils/utils.py` & `monarch_py-0.7.3/src/monarch_py/utils/utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.2/PKG-INFO` & `monarch_py-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monarch-py
-Version: 0.7.2
+Version: 0.7.3
 Summary: Monarch Initiative data access library
 Author: Kevin Schaper
 Author-email: kevin@tislab.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

