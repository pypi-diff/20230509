# Comparing `tmp/kgcl-rdflib-0.3.0.tar.gz` & `tmp/kgcl_rdflib-0.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgcl-rdflib-0.3.0.tar", max compression
+gzip compressed data, was "kgcl_rdflib-0.4.0rc1.tar", max compression
```

## Comparing `kgcl-rdflib-0.3.0.tar` & `kgcl_rdflib-0.4.0rc1.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1071 2022-08-30 01:21:14.695909 kgcl-rdflib-0.3.0/LICENSE
--rw-r--r--   0        0        0      380 2022-08-30 01:21:14.695909 kgcl-rdflib-0.3.0/README.md
--rw-r--r--   0        0        0     7695 2022-08-30 01:21:14.699910 kgcl-rdflib-0.3.0/kgcl_rdflib/README.md
--rw-r--r--   0        0        0        0 2022-08-30 01:21:14.699910 kgcl-rdflib-0.3.0/kgcl_rdflib/__init__.py
--rw-r--r--   0        0        0        0 2022-08-30 01:21:14.699910 kgcl-rdflib-0.3.0/kgcl_rdflib/apply/__init__.py
--rw-r--r--   0        0        0      540 2022-08-30 01:21:14.699910 kgcl-rdflib-0.3.0/kgcl_rdflib/apply/graph_transformer.py
--rw-r--r--   0        0        0    65989 2022-08-30 01:21:14.699910 kgcl-rdflib-0.3.0/kgcl_rdflib/apply/kgcl_2_sparql.py
--rw-r--r--   0        0        0        0 2022-08-30 01:21:14.699910 kgcl-rdflib-0.3.0/kgcl_rdflib/diff/__init__.py
--rw-r--r--   0        0        0    13033 2022-08-30 01:21:14.699910 kgcl-rdflib-0.3.0/kgcl_rdflib/diff/change_detection.py
--rw-r--r--   0        0        0     5831 2022-08-30 01:21:14.699910 kgcl-rdflib-0.3.0/kgcl_rdflib/diff/diff_2_kgcl_existential.py
--rw-r--r--   0        0        0    21085 2022-08-30 01:21:14.699910 kgcl-rdflib-0.3.0/kgcl_rdflib/diff/diff_2_kgcl_single.py
--rw-r--r--   0        0        0     7591 2022-08-30 01:21:14.699910 kgcl-rdflib-0.3.0/kgcl_rdflib/diff/diff_2_kgcl_triple_annotation.py
--rw-r--r--   0        0        0     3538 2022-08-30 01:21:14.699910 kgcl-rdflib-0.3.0/kgcl_rdflib/diff/graph_diff.py
--rw-r--r--   0        0        0    11823 2022-08-30 01:21:14.699910 kgcl-rdflib-0.3.0/kgcl_rdflib/diff/owlstar_sublanguage.py
--rw-r--r--   0        0        0    12052 2022-08-30 01:21:14.699910 kgcl-rdflib-0.3.0/kgcl_rdflib/diff/pretty_print_kgcl.py
--rw-r--r--   0        0        0     8080 2022-08-30 01:21:14.699910 kgcl-rdflib-0.3.0/kgcl_rdflib/diff/render_operations.py
--rw-r--r--   0        0        0     5531 2022-08-30 01:21:14.699910 kgcl-rdflib-0.3.0/kgcl_rdflib/diff/summary_generation.py
--rw-r--r--   0        0        0     1560 2022-08-30 01:21:14.699910 kgcl-rdflib-0.3.0/kgcl_rdflib/kgcl.py
--rw-r--r--   0        0        0     7952 2022-08-30 01:21:14.699910 kgcl-rdflib-0.3.0/kgcl_rdflib/kgcl_diff.py
--rw-r--r--   0        0        0     6148 2022-08-30 01:21:14.699910 kgcl-rdflib-0.3.0/kgcl_rdflib/render_kgcl.py
--rw-r--r--   0        0        0      791 2022-08-30 01:22:18.166577 kgcl-rdflib-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1369 2022-08-30 01:22:18.923481 kgcl-rdflib-0.3.0/setup.py
--rw-r--r--   0        0        0     1046 2022-08-30 01:22:18.923827 kgcl-rdflib-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-08 22:55:06.123477 kgcl_rdflib-0.4.0rc1/LICENSE
+-rw-r--r--   0        0        0      380 2023-05-08 22:55:06.123477 kgcl_rdflib-0.4.0rc1/README.md
+-rw-r--r--   0        0        0     7695 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/apply/__init__.py
+-rw-r--r--   0        0        0      540 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/apply/graph_transformer.py
+-rw-r--r--   0        0        0    65986 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/apply/kgcl_2_sparql.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/__init__.py
+-rw-r--r--   0        0        0    13033 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/change_detection.py
+-rw-r--r--   0        0        0     5831 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/diff_2_kgcl_existential.py
+-rw-r--r--   0        0        0    21085 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/diff_2_kgcl_single.py
+-rw-r--r--   0        0        0     7591 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/diff_2_kgcl_triple_annotation.py
+-rw-r--r--   0        0        0     3538 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/graph_diff.py
+-rw-r--r--   0        0        0    11823 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/owlstar_sublanguage.py
+-rw-r--r--   0        0        0    12052 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/pretty_print_kgcl.py
+-rw-r--r--   0        0        0     8080 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/render_operations.py
+-rw-r--r--   0        0        0     5531 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/summary_generation.py
+-rw-r--r--   0        0        0     1560 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/kgcl.py
+-rw-r--r--   0        0        0     7952 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/kgcl_diff.py
+-rw-r--r--   0        0        0     6145 2023-05-08 22:55:06.127477 kgcl_rdflib-0.4.0rc1/kgcl_rdflib/render_kgcl.py
+-rw-r--r--   0        0        0      798 2023-05-08 22:55:46.003692 kgcl_rdflib-0.4.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 kgcl_rdflib-0.4.0rc1/PKG-INFO
```

### Comparing `kgcl-rdflib-0.3.0/LICENSE` & `kgcl_rdflib-0.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `kgcl-rdflib-0.3.0/kgcl_rdflib/README.md` & `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/README.md`

 * *Files identical despite different names*

### Comparing `kgcl-rdflib-0.3.0/kgcl_rdflib/apply/graph_transformer.py` & `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/apply/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `kgcl-rdflib-0.3.0/kgcl_rdflib/apply/kgcl_2_sparql.py` & `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/apply/kgcl_2_sparql.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from kgcl_schema.datamodel.kgcl import (Change, ClassCreation, EdgeCreation,
                                         EdgeDeletion, NewSynonym,
                                         NodeAnnotationChange, NodeCreation,
                                         NodeDeepening, NodeDeletion, NodeMove,
                                         NodeObsoletion, NodeRename,
                                         NodeShallowing, NodeUnobsoletion,
                                         PlaceUnder, PredicateChange,
-                                        RemovedNodeFromSubset, RemoveUnder)
+                                        RemoveNodeFromSubset, RemoveUnder)
 
 CURIE_PATTERN = re.compile(r"^(\w+):(\S+)$")
 SPARQL_COMMAND = str
 
 
 def get_prefix(curie):
     """Get prefix."""
@@ -171,15 +171,15 @@
             return new_synonym_for_label(kgcl_instance)
         if representation == "curie":
             return new_synonym_for_curie(kgcl_instance)
 
     if isinstance(kgcl_instance, PredicateChange):
         return change_predicate(kgcl_instance)
 
-    if isinstance(kgcl_instance, RemovedNodeFromSubset):
+    if isinstance(kgcl_instance, RemoveNodeFromSubset):
         if is_id(kgcl_instance.about_node) and is_id(kgcl_instance.subset):
             return remove_node_from_subset(kgcl_instance)
 
     if isinstance(kgcl_instance, PlaceUnder):
         return triple_creation(kgcl_instance)
 
     if isinstance(kgcl_instance, RemoveUnder):
@@ -268,15 +268,15 @@
     where = "WHERE {" + where__query + "}"
 
     update__query = prefix + " " + delete + " " + insert + " " + where
 
     return update__query
 
 
-def remove_node_from_subset(kgcl_instance: RemovedNodeFromSubset) -> SPARQL_COMMAND:
+def remove_node_from_subset(kgcl_instance: RemoveNodeFromSubset) -> SPARQL_COMMAND:
     """Return SPARQL query to remove node from subset."""
     about = kgcl_instance.about_node
     subset = kgcl_instance.subset
 
     update__query = (
         f"PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>"
         f"PREFIX obo: <http://purl.obolibrary.org/obo/>"
```

### Comparing `kgcl-rdflib-0.3.0/kgcl_rdflib/diff/change_detection.py` & `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/change_detection.py`

 * *Files identical despite different names*

### Comparing `kgcl-rdflib-0.3.0/kgcl_rdflib/diff/diff_2_kgcl_existential.py` & `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/diff_2_kgcl_existential.py`

 * *Files identical despite different names*

### Comparing `kgcl-rdflib-0.3.0/kgcl_rdflib/diff/diff_2_kgcl_single.py` & `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/diff_2_kgcl_single.py`

 * *Files identical despite different names*

### Comparing `kgcl-rdflib-0.3.0/kgcl_rdflib/diff/diff_2_kgcl_triple_annotation.py` & `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/diff_2_kgcl_triple_annotation.py`

 * *Files identical despite different names*

### Comparing `kgcl-rdflib-0.3.0/kgcl_rdflib/diff/graph_diff.py` & `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/graph_diff.py`

 * *Files identical despite different names*

### Comparing `kgcl-rdflib-0.3.0/kgcl_rdflib/diff/owlstar_sublanguage.py` & `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/owlstar_sublanguage.py`

 * *Files identical despite different names*

### Comparing `kgcl-rdflib-0.3.0/kgcl_rdflib/diff/pretty_print_kgcl.py` & `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/pretty_print_kgcl.py`

 * *Files identical despite different names*

### Comparing `kgcl-rdflib-0.3.0/kgcl_rdflib/diff/render_operations.py` & `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/render_operations.py`

 * *Files identical despite different names*

### Comparing `kgcl-rdflib-0.3.0/kgcl_rdflib/diff/summary_generation.py` & `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/diff/summary_generation.py`

 * *Files identical despite different names*

### Comparing `kgcl-rdflib-0.3.0/kgcl_rdflib/kgcl.py` & `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/kgcl.py`

 * *Files identical despite different names*

### Comparing `kgcl-rdflib-0.3.0/kgcl_rdflib/kgcl_diff.py` & `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/kgcl_diff.py`

 * *Files identical despite different names*

### Comparing `kgcl-rdflib-0.3.0/kgcl_rdflib/render_kgcl.py` & `kgcl_rdflib-0.4.0rc1/kgcl_rdflib/render_kgcl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Render KGCL."""
 from kgcl_schema.model.kgcl import (ClassCreation, EdgeCreation, EdgeDeletion,
                                     NewSynonym, NodeCreation, NodeDeepening,
                                     NodeDeletion, NodeMove, NodeObsoletion,
                                     NodeRename, NodeShallowing,
                                     NodeUnobsoletion, PredicateChange,
-                                    RemovedNodeFromSubset)
+                                    RemoveNodeFromSubset)
 
 
 def render(kgcl_instance):
     """Render kGCL based on instance type."""
     render = ""
     if type(kgcl_instance) is NodeRename:
         render = (
@@ -216,18 +216,18 @@
 
     # if(type(kgclInstance) is AddNodeToSubset):
     #    render = render + "AddNodeToSubset(" \
     #            + "ID=" + kgclInstance.id + ", " \
     #            + "Subset=" + kgclInstance.in_subset + ", " \
     #            + "About Node" + kgclInstance.about_node + ")"
 
-    if type(kgcl_instance) is RemovedNodeFromSubset:
+    if type(kgcl_instance) is RemoveNodeFromSubset:
         render = (
             render
-            + "RemovedNodeFromSubset("
+            + "RemoveNodeFromSubset("
             + "ID="
             + kgcl_instance.id
             + ", "
             + "Subset="
             + kgcl_instance.subset
             + ", "
             + "About Node"
```

### Comparing `kgcl-rdflib-0.3.0/pyproject.toml` & `kgcl_rdflib-0.4.0rc1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "kgcl-rdflib"
-version = "v0.3.0"
-description = "Schema fro the KGCL project."
+version = "v0.4.0-rc1"
+description = "Schema for the KGCL project."
 authors = [
     "Christian Kindermann <christian.kindermann@postgrad.manchester.ac.uk>",
     "Chris Mungall <cjmungall@lbl.gov>",
     "Harshad Hegde <hhegde@lbl.gov>"
     ]
 license = "MIT"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 linkml-runtime = "^1.1.24"
 lark = "^1.1.2"
-kgcl-schema = "^0.3.0"
+kgcl-schema = "0.4.0-rc1"
 
 [tool.poetry.dev-dependencies]
 linkml = "^1.2.15"
 mkdocs-material = "^8.2.8"
 pytest = "^7.1.2"
 
 [build-system]
```

### Comparing `kgcl-rdflib-0.3.0/PKG-INFO` & `kgcl_rdflib-0.4.0rc1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: kgcl-rdflib
-Version: 0.3.0
-Summary: Schema fro the KGCL project.
+Version: 0.4.0rc1
+Summary: Schema for the KGCL project.
 License: MIT
 Author: Christian Kindermann
 Author-email: christian.kindermann@postgrad.manchester.ac.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
-Requires-Dist: kgcl-schema (>=0.3.0,<0.4.0)
+Requires-Dist: kgcl-schema (==0.4.0-rc1)
 Requires-Dist: lark (>=1.1.2,<2.0.0)
 Requires-Dist: linkml-runtime (>=1.1.24,<2.0.0)
 Description-Content-Type: text/markdown
 
 # kgcl-rdflib
 
 An engine that applies changes or diffs specified in KGCL to an RDF graph stored using rdflib
```

