# Comparing `tmp/kgcl_schema-0.3.6.tar.gz` & `tmp/kgcl_schema-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgcl_schema-0.3.6.tar", max compression
+gzip compressed data, was "kgcl_schema-0.3.7.tar", max compression
```

## Comparing `kgcl_schema-0.3.6.tar` & `kgcl_schema-0.3.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1071 2023-04-06 03:45:59.978752 kgcl_schema-0.3.6/LICENSE
--rw-r--r--   0        0        0      330 2023-04-06 03:45:59.978752 kgcl_schema-0.3.6/README.md
--rw-r--r--   0        0        0      825 2023-04-06 03:46:36.970307 kgcl_schema-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     7695 2023-04-06 03:45:59.990752 kgcl_schema-0.3.6/src/kgcl_schema/README.md
--rw-r--r--   0        0        0        0 2023-04-06 03:45:59.990752 kgcl_schema-0.3.6/src/kgcl_schema/__init__.py
--rw-r--r--   0        0        0   125899 2023-04-06 03:45:59.990752 kgcl_schema-0.3.6/src/kgcl_schema/datamodel/kgcl.py
--rw-r--r--   0        0        0    15508 2023-04-06 03:45:59.990752 kgcl_schema-0.3.6/src/kgcl_schema/datamodel/ontology_model.py
--rw-r--r--   0        0        0        0 2023-04-06 03:45:59.990752 kgcl_schema-0.3.6/src/kgcl_schema/grammar/__init__.py
--rw-r--r--   0        0        0     4242 2023-04-06 03:45:59.990752 kgcl_schema-0.3.6/src/kgcl_schema/grammar/kgcl.lark
--rw-r--r--   0        0        0    14441 2023-04-06 03:45:59.990752 kgcl_schema-0.3.6/src/kgcl_schema/grammar/kgcl_2_rdf.py
--rw-r--r--   0        0        0    20275 2023-04-06 03:45:59.990752 kgcl_schema-0.3.6/src/kgcl_schema/grammar/parser.py
--rw-r--r--   0        0        0     9975 2023-04-06 03:45:59.990752 kgcl_schema-0.3.6/src/kgcl_schema/grammar/render_operations.py
--rw-r--r--   0        0        0      208 2023-04-06 03:45:59.990752 kgcl_schema-0.3.6/src/kgcl_schema/schema/__init__.py
--rw-r--r--   0        0        0      516 2023-04-06 03:45:59.990752 kgcl_schema-0.3.6/src/kgcl_schema/schema/basics.yaml
--rw-r--r--   0        0        0    33131 2023-04-06 03:45:59.990752 kgcl_schema-0.3.6/src/kgcl_schema/schema/kgcl.yaml
--rw-r--r--   0        0        0     4635 2023-04-06 03:45:59.990752 kgcl_schema-0.3.6/src/kgcl_schema/schema/ontology_model.yaml
--rw-r--r--   0        0        0     1485 2023-04-06 03:45:59.990752 kgcl_schema-0.3.6/src/kgcl_schema/schema/prov.yaml
--rw-r--r--   0        0        0     4415 2023-04-06 03:45:59.990752 kgcl_schema-0.3.6/src/kgcl_schema/utils.py
--rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 kgcl_schema-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-08 22:04:58.143718 kgcl_schema-0.3.7/LICENSE
+-rw-r--r--   0        0        0      330 2023-05-08 22:04:58.143718 kgcl_schema-0.3.7/README.md
+-rw-r--r--   0        0        0      828 2023-05-08 22:05:38.390241 kgcl_schema-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     7695 2023-05-08 22:04:58.155719 kgcl_schema-0.3.7/src/kgcl_schema/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 22:04:58.155719 kgcl_schema-0.3.7/src/kgcl_schema/__init__.py
+-rw-r--r--   0        0        0   125899 2023-05-08 22:04:58.155719 kgcl_schema-0.3.7/src/kgcl_schema/datamodel/kgcl.py
+-rw-r--r--   0        0        0    15508 2023-05-08 22:04:58.155719 kgcl_schema-0.3.7/src/kgcl_schema/datamodel/ontology_model.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:04:58.155719 kgcl_schema-0.3.7/src/kgcl_schema/grammar/__init__.py
+-rw-r--r--   0        0        0     4242 2023-05-08 22:04:58.155719 kgcl_schema-0.3.7/src/kgcl_schema/grammar/kgcl.lark
+-rw-r--r--   0        0        0    14441 2023-05-08 22:04:58.155719 kgcl_schema-0.3.7/src/kgcl_schema/grammar/kgcl_2_rdf.py
+-rw-r--r--   0        0        0    20275 2023-05-08 22:04:58.155719 kgcl_schema-0.3.7/src/kgcl_schema/grammar/parser.py
+-rw-r--r--   0        0        0     9975 2023-05-08 22:04:58.155719 kgcl_schema-0.3.7/src/kgcl_schema/grammar/render_operations.py
+-rw-r--r--   0        0        0      208 2023-05-08 22:04:58.155719 kgcl_schema-0.3.7/src/kgcl_schema/schema/__init__.py
+-rw-r--r--   0        0        0      516 2023-05-08 22:04:58.155719 kgcl_schema-0.3.7/src/kgcl_schema/schema/basics.yaml
+-rw-r--r--   0        0        0    33131 2023-05-08 22:04:58.155719 kgcl_schema-0.3.7/src/kgcl_schema/schema/kgcl.yaml
+-rw-r--r--   0        0        0     4635 2023-05-08 22:04:58.155719 kgcl_schema-0.3.7/src/kgcl_schema/schema/ontology_model.yaml
+-rw-r--r--   0        0        0     1485 2023-05-08 22:04:58.155719 kgcl_schema-0.3.7/src/kgcl_schema/schema/prov.yaml
+-rw-r--r--   0        0        0     4415 2023-05-08 22:04:58.155719 kgcl_schema-0.3.7/src/kgcl_schema/utils.py
+-rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 kgcl_schema-0.3.7/PKG-INFO
```

### Comparing `kgcl_schema-0.3.6/LICENSE` & `kgcl_schema-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.3.6/pyproject.toml` & `kgcl_schema-0.3.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "kgcl_schema"
-version = "v0.3.6"
+version = "v0.3.7"
 description = "Schema for the KGCL project."
 authors = [
     "Chris Mungall <cjmungall@lbl.gov>",
     "Harshad Hegde <hhegde@lbl.gov>"
     ]
 license = "MIT"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
-linkml-runtime = "^1.1.24"
-lark = "^1.1.2"
-bioregistry = "^0.6.0"
+linkml-runtime = ">=1.1.24"
+lark = ">=1.1.2"
+bioregistry = ">=0.6.0"
 
 [tool.poetry.dev-dependencies]
-linkml = ">=1.5.0"
+linkml = ">=1.5.2"
 pytest = "^7.1.2"
 mkdocs-material = "^8.2.8"
 mkdocs-mermaid2-plugin = "^0.6.0"
 
 [tool.poetry.group.dev.dependencies]
 linkml = "^1.4.3"
```

### Comparing `kgcl_schema-0.3.6/src/kgcl_schema/README.md` & `kgcl_schema-0.3.7/src/kgcl_schema/README.md`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.3.6/src/kgcl_schema/datamodel/kgcl.py` & `kgcl_schema-0.3.7/src/kgcl_schema/datamodel/kgcl.py`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.3.6/src/kgcl_schema/datamodel/ontology_model.py` & `kgcl_schema-0.3.7/src/kgcl_schema/datamodel/ontology_model.py`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.3.6/src/kgcl_schema/grammar/kgcl.lark` & `kgcl_schema-0.3.7/src/kgcl_schema/grammar/kgcl.lark`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.3.6/src/kgcl_schema/grammar/kgcl_2_rdf.py` & `kgcl_schema-0.3.7/src/kgcl_schema/grammar/kgcl_2_rdf.py`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.3.6/src/kgcl_schema/grammar/parser.py` & `kgcl_schema-0.3.7/src/kgcl_schema/grammar/parser.py`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.3.6/src/kgcl_schema/grammar/render_operations.py` & `kgcl_schema-0.3.7/src/kgcl_schema/grammar/render_operations.py`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.3.6/src/kgcl_schema/schema/basics.yaml` & `kgcl_schema-0.3.7/src/kgcl_schema/schema/basics.yaml`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.3.6/src/kgcl_schema/schema/kgcl.yaml` & `kgcl_schema-0.3.7/src/kgcl_schema/schema/kgcl.yaml`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.3.6/src/kgcl_schema/schema/ontology_model.yaml` & `kgcl_schema-0.3.7/src/kgcl_schema/schema/ontology_model.yaml`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.3.6/src/kgcl_schema/schema/prov.yaml` & `kgcl_schema-0.3.7/src/kgcl_schema/schema/prov.yaml`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.3.6/src/kgcl_schema/utils.py` & `kgcl_schema-0.3.7/src/kgcl_schema/utils.py`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.3.6/PKG-INFO` & `kgcl_schema-0.3.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: kgcl-schema
-Version: 0.3.6
+Version: 0.3.7
 Summary: Schema for the KGCL project.
 License: MIT
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
-Requires-Dist: bioregistry (>=0.6.0,<0.7.0)
-Requires-Dist: lark (>=1.1.2,<2.0.0)
-Requires-Dist: linkml-runtime (>=1.1.24,<2.0.0)
+Requires-Dist: bioregistry (>=0.6.0)
+Requires-Dist: lark (>=1.1.2)
+Requires-Dist: linkml-runtime (>=1.1.24)
 Description-Content-Type: text/markdown
 
 # KGCL: Knowledge Graph Change Language
 
 KGCL is a standard datamodel for representing changes in ontologies and knowledge graphs.
 
 This repository houses:
```

