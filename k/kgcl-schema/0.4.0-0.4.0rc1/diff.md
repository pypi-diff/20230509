# Comparing `tmp/kgcl_schema-0.4.0.tar.gz` & `tmp/kgcl_schema-0.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgcl_schema-0.4.0.tar", max compression
+gzip compressed data, was "kgcl_schema-0.4.0rc1.tar", max compression
```

## Comparing `kgcl_schema-0.4.0.tar` & `kgcl_schema-0.4.0rc1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1071 2023-05-09 00:18:18.029991 kgcl_schema-0.4.0/LICENSE
--rw-r--r--   0        0        0      330 2023-05-09 00:18:18.029991 kgcl_schema-0.4.0/README.md
--rw-r--r--   0        0        0      828 2023-05-09 00:18:52.817662 kgcl_schema-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7695 2023-05-09 00:18:18.041991 kgcl_schema-0.4.0/src/kgcl_schema/README.md
--rw-r--r--   0        0        0        0 2023-05-09 00:18:18.041991 kgcl_schema-0.4.0/src/kgcl_schema/__init__.py
--rw-r--r--   0        0        0   125899 2023-05-09 00:18:18.041991 kgcl_schema-0.4.0/src/kgcl_schema/datamodel/kgcl.py
--rw-r--r--   0        0        0    15508 2023-05-09 00:18:18.041991 kgcl_schema-0.4.0/src/kgcl_schema/datamodel/ontology_model.py
--rw-r--r--   0        0        0        0 2023-05-09 00:18:18.041991 kgcl_schema-0.4.0/src/kgcl_schema/grammar/__init__.py
--rw-r--r--   0        0        0     4242 2023-05-09 00:18:18.041991 kgcl_schema-0.4.0/src/kgcl_schema/grammar/kgcl.lark
--rw-r--r--   0        0        0    14441 2023-05-09 00:18:18.041991 kgcl_schema-0.4.0/src/kgcl_schema/grammar/kgcl_2_rdf.py
--rw-r--r--   0        0        0    20275 2023-05-09 00:18:18.041991 kgcl_schema-0.4.0/src/kgcl_schema/grammar/parser.py
--rw-r--r--   0        0        0     9975 2023-05-09 00:18:18.041991 kgcl_schema-0.4.0/src/kgcl_schema/grammar/render_operations.py
--rw-r--r--   0        0        0      208 2023-05-09 00:18:18.041991 kgcl_schema-0.4.0/src/kgcl_schema/schema/__init__.py
--rw-r--r--   0        0        0      516 2023-05-09 00:18:18.041991 kgcl_schema-0.4.0/src/kgcl_schema/schema/basics.yaml
--rw-r--r--   0        0        0    33131 2023-05-09 00:18:18.041991 kgcl_schema-0.4.0/src/kgcl_schema/schema/kgcl.yaml
--rw-r--r--   0        0        0     4635 2023-05-09 00:18:18.041991 kgcl_schema-0.4.0/src/kgcl_schema/schema/ontology_model.yaml
--rw-r--r--   0        0        0     1485 2023-05-09 00:18:18.041991 kgcl_schema-0.4.0/src/kgcl_schema/schema/prov.yaml
--rw-r--r--   0        0        0     4415 2023-05-09 00:18:18.041991 kgcl_schema-0.4.0/src/kgcl_schema/utils.py
--rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 kgcl_schema-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-08 22:38:21.140303 kgcl_schema-0.4.0rc1/LICENSE
+-rw-r--r--   0        0        0      330 2023-05-08 22:38:21.140303 kgcl_schema-0.4.0rc1/README.md
+-rw-r--r--   0        0        0      832 2023-05-08 22:39:02.963143 kgcl_schema-0.4.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     7695 2023-05-08 22:38:21.156304 kgcl_schema-0.4.0rc1/src/kgcl_schema/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 22:38:21.156304 kgcl_schema-0.4.0rc1/src/kgcl_schema/__init__.py
+-rw-r--r--   0        0        0   137919 2023-05-08 22:38:21.156304 kgcl_schema-0.4.0rc1/src/kgcl_schema/datamodel/kgcl.py
+-rw-r--r--   0        0        0    15269 2023-05-08 22:38:21.156304 kgcl_schema-0.4.0rc1/src/kgcl_schema/datamodel/ontology_model.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:38:21.156304 kgcl_schema-0.4.0rc1/src/kgcl_schema/grammar/__init__.py
+-rw-r--r--   0        0        0     4242 2023-05-08 22:38:21.156304 kgcl_schema-0.4.0rc1/src/kgcl_schema/grammar/kgcl.lark
+-rw-r--r--   0        0        0    14441 2023-05-08 22:38:21.156304 kgcl_schema-0.4.0rc1/src/kgcl_schema/grammar/kgcl_2_rdf.py
+-rw-r--r--   0        0        0    20274 2023-05-08 22:38:21.156304 kgcl_schema-0.4.0rc1/src/kgcl_schema/grammar/parser.py
+-rw-r--r--   0        0        0     9975 2023-05-08 22:38:21.156304 kgcl_schema-0.4.0rc1/src/kgcl_schema/grammar/render_operations.py
+-rw-r--r--   0        0        0      208 2023-05-08 22:38:21.156304 kgcl_schema-0.4.0rc1/src/kgcl_schema/schema/__init__.py
+-rw-r--r--   0        0        0      501 2023-05-08 22:38:21.156304 kgcl_schema-0.4.0rc1/src/kgcl_schema/schema/basics.yaml
+-rw-r--r--   0        0        0    32080 2023-05-08 22:38:21.156304 kgcl_schema-0.4.0rc1/src/kgcl_schema/schema/kgcl.yaml
+-rw-r--r--   0        0        0     4414 2023-05-08 22:38:21.156304 kgcl_schema-0.4.0rc1/src/kgcl_schema/schema/ontology_model.yaml
+-rw-r--r--   0        0        0     1544 2023-05-08 22:38:21.156304 kgcl_schema-0.4.0rc1/src/kgcl_schema/schema/prov.yaml
+-rw-r--r--   0        0        0     4415 2023-05-08 22:38:21.156304 kgcl_schema-0.4.0rc1/src/kgcl_schema/utils.py
+-rw-r--r--   0        0        0      993 1970-01-01 00:00:00.000000 kgcl_schema-0.4.0rc1/PKG-INFO
```

### Comparing `kgcl_schema-0.4.0/LICENSE` & `kgcl_schema-0.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.4.0/pyproject.toml` & `kgcl_schema-0.4.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kgcl_schema"
-version = "v0.4.0"
+version = "v0.4.0-rc1"
 description = "Schema for the KGCL project."
 authors = [
     "Chris Mungall <cjmungall@lbl.gov>",
     "Harshad Hegde <hhegde@lbl.gov>"
     ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `kgcl_schema-0.4.0/src/kgcl_schema/README.md` & `kgcl_schema-0.4.0rc1/src/kgcl_schema/README.md`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.4.0/src/kgcl_schema/datamodel/kgcl.py` & `kgcl_schema-0.4.0rc1/src/kgcl_schema/datamodel/kgcl.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,74 @@
 # Auto generated from kgcl.yaml by pythongen.py version: 0.9.0
-# Generation date: 2022-12-02T07:39:37
+# Generation date: 2023-05-08T15:27:55
 # Schema: kgcl_schema
 #
-# id: https://w3id.org/kgcl_schema
-# description: A data model for describing change operations at a high level on an ontology or ontology-like
-#              artefact, such as a Knowledge Graph. * [Browse
-#              Schema](https://cmungall.github.io/knowledge-graph-change-language/) *
-#              [GitHub](https://github.com/cmungall/knowledge-graph-change-language)
+# id: https://w3id.org/kgcl
+# description: A data model for describing change operations at a high level on an ontology or ontology-like artefact, such as a Knowledge Graph.
+#   * [Browse Schema](https://cmungall.github.io/knowledge-graph-change-language/)
+#   * [GitHub](https://github.com/cmungall/knowledge-graph-change-language)
 # license: https://creativecommons.org/publicdomain/zero/1.0/
 
 import dataclasses
-import sys
 import re
 from jsonasobj2 import JsonObj, as_dict
 from typing import Optional, List, Union, Dict, ClassVar, Any
 from dataclasses import dataclass
-from linkml_runtime.linkml_model.meta import (
-    EnumDefinition,
-    PermissibleValue,
-    PvFormulaOptions,
-)
+from linkml_runtime.linkml_model.meta import EnumDefinition, PermissibleValue, PvFormulaOptions
 
 from linkml_runtime.utils.slot import Slot
 from linkml_runtime.utils.metamodelcore import empty_list, empty_dict, bnode
-from linkml_runtime.utils.yamlutils import (
-    YAMLRoot,
-    extended_str,
-    extended_float,
-    extended_int,
-)
-from linkml_runtime.utils.dataclass_extensions_376 import (
-    dataclasses_init_fn_with_kwargs,
-)
+from linkml_runtime.utils.yamlutils import YAMLRoot, extended_str, extended_float, extended_int
+from linkml_runtime.utils.dataclass_extensions_376 import dataclasses_init_fn_with_kwargs
 from linkml_runtime.utils.formatutils import camelcase, underscore, sfx
 from linkml_runtime.utils.enumerations import EnumDefinitionImpl
 from rdflib import Namespace, URIRef
 from linkml_runtime.utils.curienamespace import CurieNamespace
 from linkml_runtime.linkml_model.types import Integer, String, Uriorcurie
 from linkml_runtime.utils.metamodelcore import URIorCURIE
 
 metamodel_version = "1.7.0"
 version = "0.0.1"
 
 # Overwrite dataclasses _init_fn to add **kwargs in __init__
 dataclasses._init_fn = dataclasses_init_fn_with_kwargs
 
 # Namespaces
-IAO = CurieNamespace("IAO", "http://purl.obolibrary.org/obo/IAO_")
-BASICS = CurieNamespace("basics", "https://w3id.org/kgcl_schema/basics/")
-DCTERMS = CurieNamespace("dcterms", "http://purl.org/dc/terms/")
-KGCL = CurieNamespace("kgcl", "http://w3id.org/kgcl_schema/")
-LINKML = CurieNamespace("linkml", "https://w3id.org/linkml/")
-OIO = CurieNamespace("oio", "http://www.geneontology.org/formats/oboInOwl#")
-OM = CurieNamespace("om", "http://w3id.org/kgcl_schema/om/")
-OWL = CurieNamespace("owl", "http://www.w3.org/2002/07/owl#")
-PROV = CurieNamespace("prov", "http://www.w3.org/ns/prov#")
-RDF = CurieNamespace("rdf", "http://www.w3.org/1999/02/22-rdf-syntax-ns#")
-RDFS = CurieNamespace("rdfs", "http://www.w3.org/2000/01/rdf-schema#")
-XML = CurieNamespace("xml", "http://www.w3.org/XML/1998/namespace#")
-XSD = CurieNamespace("xsd", "http://www.w3.org/2001/XMLSchema#")
+IAO = CurieNamespace('IAO', 'http://purl.obolibrary.org/obo/IAO_')
+BASICS = CurieNamespace('basics', 'https://w3id.org/kgcl_schema/basics/')
+DCTERMS = CurieNamespace('dcterms', 'http://purl.org/dc/terms/')
+KGCL = CurieNamespace('kgcl', 'http://w3id.org/kgcl/')
+LINKML = CurieNamespace('linkml', 'https://w3id.org/linkml/')
+OIO = CurieNamespace('oio', 'http://www.geneontology.org/formats/oboInOwl#')
+OM = CurieNamespace('om', 'http://w3id.org/kgcl_schema/om/')
+OWL = CurieNamespace('owl', 'http://www.w3.org/2002/07/owl#')
+PROV = CurieNamespace('prov', 'http://www.w3.org/ns/prov#')
+RDF = CurieNamespace('rdf', 'http://www.w3.org/1999/02/22-rdf-syntax-ns#')
+RDFS = CurieNamespace('rdfs', 'http://www.w3.org/2000/01/rdf-schema#')
+XML = CurieNamespace('xml', 'http://www.w3.org/XML/1998/namespace#')
+XSD = CurieNamespace('xsd', 'http://www.w3.org/2001/XMLSchema#')
 DEFAULT_ = KGCL
 
 
 # Types
-class ChangeClassType(Uriorcurie):
-    """CURIE for a class within this datamodel. E.g. kgcl:NodeObsoletion"""
-
-    type_class_uri = XSD.anyURI
-    type_class_curie = "xsd:anyURI"
-    type_name = "change class type"
-    type_model_uri = KGCL.ChangeClassType
-
-
 class LanguageTag(str):
     type_class_uri = XML.lang
     type_class_curie = "xml:lang"
-    type_name = "language tag"
+    type_name = "LanguageTag"
     type_model_uri = KGCL.LanguageTag
 
 
+class ChangeClassType(Uriorcurie):
+    """ CURIE for a class within this data model. E.g. kgcl:NodeObsoletion """
+    type_class_uri = XSD.anyURI
+    type_class_curie = "xsd:anyURI"
+    type_name = "ChangeClassType"
+    type_model_uri = KGCL.ChangeClassType
+
+
 # Class references
 class ChangeId(extended_str):
     pass
 
 
 class SimpleChangeId(ChangeId):
     pass
@@ -196,14 +182,54 @@
     pass
 
 
 class SynonymPredicateChangeId(NodeSynonymChangeId):
     pass
 
 
+class NodeMappingChangeId(NodeChangeId):
+    pass
+
+
+class NewMappingId(NodeMappingChangeId):
+    pass
+
+
+class RemoveMappingId(NodeMappingChangeId):
+    pass
+
+
+class MappingReplacementId(NodeMappingChangeId):
+    pass
+
+
+class MappingPredicateChangeId(NodeMappingChangeId):
+    pass
+
+
+class NodeMetadataAssertionChangeId(NodeChangeId):
+    pass
+
+
+class NewMetadataAssertionId(NodeMetadataAssertionChangeId):
+    pass
+
+
+class RemoveMetadataAssertionId(NodeMetadataAssertionChangeId):
+    pass
+
+
+class MetadataAssertionReplacementId(NodeMetadataAssertionChangeId):
+    pass
+
+
+class MetadataAssertionPredicateChangeId(NodeMetadataAssertionChangeId):
+    pass
+
+
 class NodeTextDefinitionChangeId(NodeChangeId):
     pass
 
 
 class NewTextDefinitionId(NodeTextDefinitionChangeId):
     pass
 
@@ -216,15 +242,15 @@
     pass
 
 
 class AddNodeToSubsetId(NodeChangeId):
     pass
 
 
-class RemovedNodeFromSubsetId(NodeChangeId):
+class RemoveNodeFromSubsetId(NodeChangeId):
     pass
 
 
 class NodeObsoletionId(NodeChangeId):
     pass
 
 
@@ -236,14 +262,18 @@
     pass
 
 
 class ClassCreationId(NodeCreationId):
     pass
 
 
+class ObjectPropertyCreationId(NodeCreationId):
+    pass
+
+
 class NodeDeletionId(NodeChangeId):
     pass
 
 
 class NodeDirectMergeId(NodeObsoletionId):
     pass
 
@@ -272,49 +302,59 @@
     pass
 
 
 class AgentId(extended_str):
     pass
 
 
+class ChangeLanguageElement(YAMLRoot):
+    """
+    A broad grouping for all elements of the change language
+    """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = KGCL.ChangeLanguageElement
+    class_class_curie: ClassVar[str] = "kgcl:ChangeLanguageElement"
+    class_name: ClassVar[str] = "ChangeLanguageElement"
+    class_model_uri: ClassVar[URIRef] = KGCL.ChangeLanguageElement
+
+
 @dataclass
-class Change(YAMLRoot):
+class Change(ChangeLanguageElement):
     """
     Any change perform on an ontology or knowledge graph
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.Change
     class_class_curie: ClassVar[str] = "kgcl:Change"
-    class_name: ClassVar[str] = "change"
+    class_name: ClassVar[str] = "Change"
     class_model_uri: ClassVar[URIRef] = KGCL.Change
 
     id: Union[str, ChangeId] = None
     type: Optional[str] = None
     was_generated_by: Optional[Union[str, ActivityId]] = None
     see_also: Optional[str] = None
     pull_request: Optional[str] = None
     creator: Optional[str] = None
     change_date: Optional[str] = None
     contributor: Optional[str] = None
     has_undo: Optional[Union[str, ChangeId]] = None
+    term_tracker_issue: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, ChangeId):
             self.id = ChangeId(self.id)
 
         if self.type is not None and not isinstance(self.type, str):
             self.type = str(self.type)
 
-        if self.was_generated_by is not None and not isinstance(
-            self.was_generated_by, ActivityId
-        ):
+        if self.was_generated_by is not None and not isinstance(self.was_generated_by, ActivityId):
             self.was_generated_by = ActivityId(self.was_generated_by)
 
         if self.see_also is not None and not isinstance(self.see_also, str):
             self.see_also = str(self.see_also)
 
         if self.pull_request is not None and not isinstance(self.pull_request, str):
             self.pull_request = str(self.pull_request)
@@ -327,28 +367,30 @@
 
         if self.contributor is not None and not isinstance(self.contributor, str):
             self.contributor = str(self.contributor)
 
         if self.has_undo is not None and not isinstance(self.has_undo, ChangeId):
             self.has_undo = ChangeId(self.has_undo)
 
+        if self.term_tracker_issue is not None and not isinstance(self.term_tracker_issue, str):
+            self.term_tracker_issue = str(self.term_tracker_issue)
+
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class SimpleChange(Change):
     """
     A change that is about a single ontology element
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.SimpleChange
     class_class_curie: ClassVar[str] = "kgcl:SimpleChange"
-    class_name: ClassVar[str] = "simple change"
+    class_name: ClassVar[str] = "SimpleChange"
     class_model_uri: ClassVar[URIRef] = KGCL.SimpleChange
 
     id: Union[str, SimpleChangeId] = None
     old_value: Optional[str] = None
     new_value: Optional[str] = None
     old_value_type: Optional[str] = None
     new_value_type: Optional[str] = None
@@ -386,187 +428,142 @@
 
 
 @dataclass
 class ComplexChange(Change):
     """
     A change that is is a composition of other changes
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.ComplexChange
     class_class_curie: ClassVar[str] = "kgcl:ComplexChange"
-    class_name: ClassVar[str] = "complex change"
+    class_name: ClassVar[str] = "ComplexChange"
     class_model_uri: ClassVar[URIRef] = KGCL.ComplexChange
 
     id: Union[str, ComplexChangeId] = None
-    change_set: Optional[
-        Union[
-            Dict[Union[str, ChangeId], Union[dict, Change]], List[Union[dict, Change]]
-        ]
-    ] = empty_dict()
+    change_set: Optional[Union[Dict[Union[str, ChangeId], Union[dict, Change]], List[Union[dict, Change]]]] = empty_dict()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        self._normalize_inlined_as_list(
-            slot_name="change_set", slot_type=Change, key_name="id", keyed=True
-        )
+        self._normalize_inlined_as_list(slot_name="change_set", slot_type=Change, key_name="id", keyed=True)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class MultiNodeObsoletion(ComplexChange):
     """
     A complex change consisting of multiple obsoletions.
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.MultiNodeObsoletion
     class_class_curie: ClassVar[str] = "kgcl:MultiNodeObsoletion"
-    class_name: ClassVar[str] = "multi node obsoletion"
+    class_name: ClassVar[str] = "MultiNodeObsoletion"
     class_model_uri: ClassVar[URIRef] = KGCL.MultiNodeObsoletion
 
     id: Union[str, MultiNodeObsoletionId] = None
-    change_set: Optional[
-        Union[
-            Dict[Union[str, NodeObsoletionId], Union[dict, "NodeObsoletion"]],
-            List[Union[dict, "NodeObsoletion"]],
-        ]
-    ] = empty_dict()
-    change_description: Optional[str] = None
-    associated_change_set: Optional[
-        Union[
-            Dict[Union[str, ChangeId], Union[dict, Change]], List[Union[dict, Change]]
-        ]
-    ] = empty_dict()
+    change_set: Optional[Union[Dict[Union[str, NodeObsoletionId], Union[dict, "NodeObsoletion"]], List[Union[dict, "NodeObsoletion"]]]] = empty_dict()
+    change_description: Optional[str] = None
+    associated_change_set: Optional[Union[Dict[Union[str, ChangeId], Union[dict, Change]], List[Union[dict, Change]]]] = empty_dict()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, MultiNodeObsoletionId):
             self.id = MultiNodeObsoletionId(self.id)
 
-        self._normalize_inlined_as_list(
-            slot_name="change_set", slot_type=NodeObsoletion, key_name="id", keyed=True
-        )
-
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        self._normalize_inlined_as_list(slot_name="change_set", slot_type=NodeObsoletion, key_name="id", keyed=True)
+
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
-        self._normalize_inlined_as_list(
-            slot_name="associated_change_set",
-            slot_type=Change,
-            key_name="id",
-            keyed=True,
-        )
+        self._normalize_inlined_as_list(slot_name="associated_change_set", slot_type=Change, key_name="id", keyed=True)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class Transaction(Change):
     """
     A change that is a composition of a set of changes, where those changes are treated as a single unit. Could be a
     single change, or the results of an ontology diff
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.Transaction
     class_class_curie: ClassVar[str] = "kgcl:Transaction"
-    class_name: ClassVar[str] = "transaction"
+    class_name: ClassVar[str] = "Transaction"
     class_model_uri: ClassVar[URIRef] = KGCL.Transaction
 
     id: Union[str, TransactionId] = None
-    change_set: Optional[
-        Union[
-            Dict[Union[str, ChangeId], Union[dict, Change]], List[Union[dict, Change]]
-        ]
-    ] = empty_dict()
+    change_set: Optional[Union[Dict[Union[str, ChangeId], Union[dict, Change]], List[Union[dict, Change]]]] = empty_dict()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, TransactionId):
             self.id = TransactionId(self.id)
 
-        self._normalize_inlined_as_list(
-            slot_name="change_set", slot_type=Change, key_name="id", keyed=True
-        )
+        self._normalize_inlined_as_list(slot_name="change_set", slot_type=Change, key_name="id", keyed=True)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
-class ChangeSetSummaryStatistic(YAMLRoot):
+class ChangeSetSummaryStatistic(ChangeLanguageElement):
     """
     A summary statistic for a set of changes of the same type, grouped by zero or more node properties
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.ChangeSetSummaryStatistic
     class_class_curie: ClassVar[str] = "kgcl:ChangeSetSummaryStatistic"
-    class_name: ClassVar[str] = "change set summary statistic"
+    class_name: ClassVar[str] = "ChangeSetSummaryStatistic"
     class_model_uri: ClassVar[URIRef] = KGCL.ChangeSetSummaryStatistic
 
     change_type: Optional[Union[str, ChangeClassType]] = None
     count: Optional[int] = None
-    property_value_set: Optional[
-        Union[Union[dict, "PropertyValue"], List[Union[dict, "PropertyValue"]]]
-    ] = empty_list()
+    property_value_set: Optional[Union[Union[dict, "PropertyValue"], List[Union[dict, "PropertyValue"]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self.change_type is not None and not isinstance(
-            self.change_type, ChangeClassType
-        ):
+        if self.change_type is not None and not isinstance(self.change_type, ChangeClassType):
             self.change_type = ChangeClassType(self.change_type)
 
         if self.count is not None and not isinstance(self.count, int):
             self.count = int(self.count)
 
         if not isinstance(self.property_value_set, list):
-            self.property_value_set = (
-                [self.property_value_set] if self.property_value_set is not None else []
-            )
-        self.property_value_set = [
-            v if isinstance(v, PropertyValue) else PropertyValue(**as_dict(v))
-            for v in self.property_value_set
-        ]
+            self.property_value_set = [self.property_value_set] if self.property_value_set is not None else []
+        self.property_value_set = [v if isinstance(v, PropertyValue) else PropertyValue(**as_dict(v)) for v in self.property_value_set]
 
         super().__post_init__(**kwargs)
 
 
 class ChangeMixin(YAMLRoot):
     """
     root class for all change mixins
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.ChangeMixin
     class_class_curie: ClassVar[str] = "kgcl:ChangeMixin"
-    class_name: ClassVar[str] = "change mixin"
+    class_name: ClassVar[str] = "ChangeMixin"
     class_model_uri: ClassVar[URIRef] = KGCL.ChangeMixin
 
 
 @dataclass
 class Obsoletion(ChangeMixin):
     """
     Obsoletion of an element deprecates usage of that element, but does not delete that element.
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.Obsoletion
     class_class_curie: ClassVar[str] = "kgcl:Obsoletion"
-    class_name: ClassVar[str] = "obsoletion"
+    class_name: ClassVar[str] = "Obsoletion"
     class_model_uri: ClassVar[URIRef] = KGCL.Obsoletion
 
     about: Optional[Union[dict, "OntologyElement"]] = None
     has_undo: Optional[Union[dict, "Obsoletion"]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.about is not None and not isinstance(self.about, OntologyElement):
@@ -578,30 +575,29 @@
         super().__post_init__(**kwargs)
 
 
 class DatatypeOrLanguageTagChange(ChangeMixin):
     """
     A change in a value assertion where the value remain unchanged but either the datatype or language changes
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.DatatypeOrLanguageTagChange
     class_class_curie: ClassVar[str] = "kgcl:DatatypeOrLanguageTagChange"
-    class_name: ClassVar[str] = "datatype or language tag change"
+    class_name: ClassVar[str] = "DatatypeOrLanguageTagChange"
     class_model_uri: ClassVar[URIRef] = KGCL.DatatypeOrLanguageTagChange
 
 
 @dataclass
 class LanguageTagChange(DatatypeOrLanguageTagChange):
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.LanguageTagChange
     class_class_curie: ClassVar[str] = "kgcl:LanguageTagChange"
-    class_name: ClassVar[str] = "language tag change"
+    class_name: ClassVar[str] = "LanguageTagChange"
     class_model_uri: ClassVar[URIRef] = KGCL.LanguageTagChange
 
     old_value: Optional[str] = None
     new_value: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.old_value is not None and not isinstance(self.old_value, str):
@@ -614,43 +610,41 @@
 
 
 class DatatypeChange(DatatypeOrLanguageTagChange):
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.DatatypeChange
     class_class_curie: ClassVar[str] = "kgcl:DatatypeChange"
-    class_name: ClassVar[str] = "datatype change"
+    class_name: ClassVar[str] = "DatatypeChange"
     class_model_uri: ClassVar[URIRef] = KGCL.DatatypeChange
 
 
 class AllowsAutomaticReplacementOfEdges(Obsoletion):
     """
     Applies to an obsoletion in which annotations or edges pointing at the obsoleted node can be automatically rewired
     to point to a target
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.AllowsAutomaticReplacementOfEdges
     class_class_curie: ClassVar[str] = "kgcl:AllowsAutomaticReplacementOfEdges"
-    class_name: ClassVar[str] = "allows automatic replacement of edges"
+    class_name: ClassVar[str] = "AllowsAutomaticReplacementOfEdges"
     class_model_uri: ClassVar[URIRef] = KGCL.AllowsAutomaticReplacementOfEdges
 
 
 @dataclass
 class Unobsoletion(ChangeMixin):
     """
     Opposite operation of obsoletion. Rarely performed.
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.Unobsoletion
     class_class_curie: ClassVar[str] = "kgcl:Unobsoletion"
-    class_name: ClassVar[str] = "unobsoletion"
+    class_name: ClassVar[str] = "Unobsoletion"
     class_model_uri: ClassVar[URIRef] = KGCL.Unobsoletion
 
     has_undo: Optional[Union[dict, Obsoletion]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.has_undo is not None and not isinstance(self.has_undo, Obsoletion):
             self.has_undo = Obsoletion(**as_dict(self.has_undo))
@@ -658,34 +652,32 @@
         super().__post_init__(**kwargs)
 
 
 class Deletion(ChangeMixin):
     """
     Removal of an element.
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.Deletion
     class_class_curie: ClassVar[str] = "kgcl:Deletion"
-    class_name: ClassVar[str] = "deletion"
+    class_name: ClassVar[str] = "Deletion"
     class_model_uri: ClassVar[URIRef] = KGCL.Deletion
 
 
 @dataclass
 class Creation(ChangeMixin):
     """
     Creation of an element.
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.Creation
     class_class_curie: ClassVar[str] = "kgcl:Creation"
-    class_name: ClassVar[str] = "creation"
+    class_name: ClassVar[str] = "Creation"
     class_model_uri: ClassVar[URIRef] = KGCL.Creation
 
     has_undo: Optional[Union[dict, Deletion]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.has_undo is not None and not isinstance(self.has_undo, Deletion):
             self.has_undo = Deletion()
@@ -694,96 +686,86 @@
 
 
 @dataclass
 class SubsetMembershipChange(ChangeMixin):
     """
     A change in the membership status of a node with respect to a subset (view)
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.SubsetMembershipChange
     class_class_curie: ClassVar[str] = "kgcl:SubsetMembershipChange"
-    class_name: ClassVar[str] = "subset membership change"
+    class_name: ClassVar[str] = "SubsetMembershipChange"
     class_model_uri: ClassVar[URIRef] = KGCL.SubsetMembershipChange
 
     in_subset: Optional[Union[dict, "OntologySubset"]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self.in_subset is not None and not isinstance(
-            self.in_subset, OntologySubset
-        ):
+        if self.in_subset is not None and not isinstance(self.in_subset, OntologySubset):
             self.in_subset = OntologySubset()
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class AddToSubset(SubsetMembershipChange):
     """
     placing an element inside a subset
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.AddToSubset
     class_class_curie: ClassVar[str] = "kgcl:AddToSubset"
-    class_name: ClassVar[str] = "add to subset"
+    class_name: ClassVar[str] = "AddToSubset"
     class_model_uri: ClassVar[URIRef] = KGCL.AddToSubset
 
     in_subset: Optional[Union[dict, "OntologySubset"]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self.in_subset is not None and not isinstance(
-            self.in_subset, OntologySubset
-        ):
+        if self.in_subset is not None and not isinstance(self.in_subset, OntologySubset):
             self.in_subset = OntologySubset()
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class RemoveFromSubset(SubsetMembershipChange):
     """
     removing an element from a subset
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.RemoveFromSubset
     class_class_curie: ClassVar[str] = "kgcl:RemoveFromSubset"
-    class_name: ClassVar[str] = "remove from subset"
+    class_name: ClassVar[str] = "RemoveFromSubset"
     class_model_uri: ClassVar[URIRef] = KGCL.RemoveFromSubset
 
     in_subset: Optional[Union[dict, "OntologySubset"]] = None
     has_undo: Optional[Union[dict, AddToSubset]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self.in_subset is not None and not isinstance(
-            self.in_subset, OntologySubset
-        ):
+        if self.in_subset is not None and not isinstance(self.in_subset, OntologySubset):
             self.in_subset = OntologySubset()
 
         if self.has_undo is not None and not isinstance(self.has_undo, AddToSubset):
             self.has_undo = AddToSubset(**as_dict(self.has_undo))
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class EdgeChange(SimpleChange):
     """
     A change in which the element that is the focus of the change is an edge.
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.EdgeChange
     class_class_curie: ClassVar[str] = "kgcl:EdgeChange"
-    class_name: ClassVar[str] = "edge change"
+    class_name: ClassVar[str] = "EdgeChange"
     class_model_uri: ClassVar[URIRef] = KGCL.EdgeChange
 
     id: Union[str, EdgeChangeId] = None
     about_edge: Optional[Union[dict, "Edge"]] = None
     object_type: Optional[str] = None
     language: Optional[str] = None
     datatype: Optional[str] = None
@@ -809,20 +791,19 @@
 
 
 @dataclass
 class EdgeCreation(EdgeChange):
     """
     An edge change in which a de-novo edge is created. The edge is potentially annotated in the same action.
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.EdgeCreation
     class_class_curie: ClassVar[str] = "kgcl:EdgeCreation"
-    class_name: ClassVar[str] = "edge creation"
+    class_name: ClassVar[str] = "EdgeCreation"
     class_model_uri: ClassVar[URIRef] = KGCL.EdgeCreation
 
     id: Union[str, EdgeCreationId] = None
     subject: Optional[Union[str, NodeId]] = None
     predicate: Optional[Union[str, NodeId]] = None
     object: Optional[Union[str, NodeId]] = None
     subject_type: Optional[str] = None
@@ -851,38 +832,33 @@
 
         if self.predicate_type is not None and not isinstance(self.predicate_type, str):
             self.predicate_type = str(self.predicate_type)
 
         if self.object_type is not None and not isinstance(self.object_type, str):
             self.object_type = str(self.object_type)
 
-        if self.annotation_set is not None and not isinstance(
-            self.annotation_set, Annotation
-        ):
+        if self.annotation_set is not None and not isinstance(self.annotation_set, Annotation):
             self.annotation_set = Annotation(**as_dict(self.annotation_set))
 
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class PlaceUnder(EdgeCreation):
     """
     An edge creation where the predicate is owl:subClassOf
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.PlaceUnder
     class_class_curie: ClassVar[str] = "kgcl:PlaceUnder"
-    class_name: ClassVar[str] = "place under"
+    class_name: ClassVar[str] = "PlaceUnder"
     class_model_uri: ClassVar[URIRef] = KGCL.PlaceUnder
 
     id: Union[str, PlaceUnderId] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
@@ -893,20 +869,19 @@
 
 
 @dataclass
 class EdgeDeletion(EdgeChange):
     """
     An edge change in which an edge is removed. All edge annotations/properies are removed in the same action.
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.EdgeDeletion
     class_class_curie: ClassVar[str] = "kgcl:EdgeDeletion"
-    class_name: ClassVar[str] = "edge deletion"
+    class_name: ClassVar[str] = "EdgeDeletion"
     class_model_uri: ClassVar[URIRef] = KGCL.EdgeDeletion
 
     id: Union[str, EdgeDeletionId] = None
     subject: Optional[Union[str, NodeId]] = None
     predicate: Optional[Union[str, NodeId]] = None
     object: Optional[Union[str, NodeId]] = None
     subject_type: Optional[str] = None
@@ -935,38 +910,33 @@
 
         if self.predicate_type is not None and not isinstance(self.predicate_type, str):
             self.predicate_type = str(self.predicate_type)
 
         if self.object_type is not None and not isinstance(self.object_type, str):
             self.object_type = str(self.object_type)
 
-        if self.annotation_set is not None and not isinstance(
-            self.annotation_set, Annotation
-        ):
+        if self.annotation_set is not None and not isinstance(self.annotation_set, Annotation):
             self.annotation_set = Annotation(**as_dict(self.annotation_set))
 
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class RemoveUnder(EdgeDeletion):
     """
     An edge deletion where the predicate is owl:subClassOf
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.RemoveUnder
     class_class_curie: ClassVar[str] = "kgcl:RemoveUnder"
-    class_name: ClassVar[str] = "remove under"
+    class_name: ClassVar[str] = "RemoveUnder"
     class_model_uri: ClassVar[URIRef] = KGCL.RemoveUnder
 
     id: Union[str, RemoveUnderId] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
@@ -977,20 +947,19 @@
 
 
 @dataclass
 class EdgeObsoletion(EdgeChange):
     """
     An edge change in which an edge is obsoleted.
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.EdgeObsoletion
     class_class_curie: ClassVar[str] = "kgcl:EdgeObsoletion"
-    class_name: ClassVar[str] = "edge obsoletion"
+    class_name: ClassVar[str] = "EdgeObsoletion"
     class_model_uri: ClassVar[URIRef] = KGCL.EdgeObsoletion
 
     id: Union[str, EdgeObsoletionId] = None
     subject: Optional[Union[str, NodeId]] = None
     predicate: Optional[Union[str, NodeId]] = None
     object: Optional[Union[str, NodeId]] = None
     annotation_set: Optional[Union[dict, "Annotation"]] = None
@@ -1008,41 +977,36 @@
 
         if self.predicate is not None and not isinstance(self.predicate, NodeId):
             self.predicate = NodeId(self.predicate)
 
         if self.object is not None and not isinstance(self.object, NodeId):
             self.object = NodeId(self.object)
 
-        if self.annotation_set is not None and not isinstance(
-            self.annotation_set, Annotation
-        ):
+        if self.annotation_set is not None and not isinstance(self.annotation_set, Annotation):
             self.annotation_set = Annotation(**as_dict(self.annotation_set))
 
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
         if self.about is not None and not isinstance(self.about, OntologyElement):
             self.about = OntologyElement()
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class EdgeRewiring(EdgeChange):
     """
     An edge change where one node is replaced with another, as in the case of obsoletion with replacement
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.EdgeRewiring
     class_class_curie: ClassVar[str] = "kgcl:EdgeRewiring"
-    class_name: ClassVar[str] = "edge rewiring"
+    class_name: ClassVar[str] = "EdgeRewiring"
     class_model_uri: ClassVar[URIRef] = KGCL.EdgeRewiring
 
     id: Union[str, EdgeRewiringId] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
@@ -1053,20 +1017,19 @@
 
 
 @dataclass
 class MappingCreation(EdgeCreation):
     """
     A specific kind of edge creation in which the created edge is a mapping.
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.MappingCreation
     class_class_curie: ClassVar[str] = "kgcl:MappingCreation"
-    class_name: ClassVar[str] = "mapping creation"
+    class_name: ClassVar[str] = "MappingCreation"
     class_model_uri: ClassVar[URIRef] = KGCL.MappingCreation
 
     id: Union[str, MappingCreationId] = None
     subject: Optional[Union[str, NodeId]] = None
     predicate: Optional[Union[str, NodeId]] = None
     object: Optional[Union[str, NodeId]] = None
     annotation_set: Optional[Union[dict, "Annotation"]] = None
@@ -1083,172 +1046,151 @@
 
         if self.predicate is not None and not isinstance(self.predicate, NodeId):
             self.predicate = NodeId(self.predicate)
 
         if self.object is not None and not isinstance(self.object, NodeId):
             self.object = NodeId(self.object)
 
-        if self.annotation_set is not None and not isinstance(
-            self.annotation_set, Annotation
-        ):
+        if self.annotation_set is not None and not isinstance(self.annotation_set, Annotation):
             self.annotation_set = Annotation(**as_dict(self.annotation_set))
 
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class NodeMove(EdgeChange):
     """
     A node move is a combination of deleting a parent edge and adding a parent edge, where the predicate is preserved
     and the object/parent node changes
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.NodeMove
     class_class_curie: ClassVar[str] = "kgcl:NodeMove"
-    class_name: ClassVar[str] = "node move"
+    class_name: ClassVar[str] = "NodeMove"
     class_model_uri: ClassVar[URIRef] = KGCL.NodeMove
 
     id: Union[str, NodeMoveId] = None
     old_object_type: Optional[str] = None
     new_object_type: Optional[str] = None
     change_description: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, NodeMoveId):
             self.id = NodeMoveId(self.id)
 
-        if self.old_object_type is not None and not isinstance(
-            self.old_object_type, str
-        ):
+        if self.old_object_type is not None and not isinstance(self.old_object_type, str):
             self.old_object_type = str(self.old_object_type)
 
-        if self.new_object_type is not None and not isinstance(
-            self.new_object_type, str
-        ):
+        if self.new_object_type is not None and not isinstance(self.new_object_type, str):
             self.new_object_type = str(self.new_object_type)
 
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class NodeDeepening(NodeMove):
     """
     A node move in which a node where the destination is a proper descendant of the original location. Note that here
     descendant applied not just to subclass, but edges of any predicate in the relational graph
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.NodeDeepening
     class_class_curie: ClassVar[str] = "kgcl:NodeDeepening"
-    class_name: ClassVar[str] = "node deepening"
+    class_name: ClassVar[str] = "NodeDeepening"
     class_model_uri: ClassVar[URIRef] = KGCL.NodeDeepening
 
     id: Union[str, NodeDeepeningId] = None
     change_description: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, NodeDeepeningId):
             self.id = NodeDeepeningId(self.id)
 
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class NodeShallowing(NodeMove):
     """
     The opposite of node deepening
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.NodeShallowing
     class_class_curie: ClassVar[str] = "kgcl:NodeShallowing"
-    class_name: ClassVar[str] = "node shallowing"
+    class_name: ClassVar[str] = "NodeShallowing"
     class_model_uri: ClassVar[URIRef] = KGCL.NodeShallowing
 
     id: Union[str, NodeShallowingId] = None
     change_description: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, NodeShallowingId):
             self.id = NodeShallowingId(self.id)
 
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class PredicateChange(EdgeChange):
     """
     An edge change where the predicate (relationship type) is modified.
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.PredicateChange
     class_class_curie: ClassVar[str] = "kgcl:PredicateChange"
-    class_name: ClassVar[str] = "predicate change"
+    class_name: ClassVar[str] = "PredicateChange"
     class_model_uri: ClassVar[URIRef] = KGCL.PredicateChange
 
     id: Union[str, PredicateChangeId] = None
     change_description: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, PredicateChangeId):
             self.id = PredicateChangeId(self.id)
 
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class EdgeLogicalInterpretationChange(EdgeChange):
     """
-    An edge change where the subjet, object, and predicate are unchanged, but the logical interpretation changes
+    An edge change where the subject, object, and predicate are unchanged, but the logical interpretation changes
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.EdgeLogicalInterpretationChange
     class_class_curie: ClassVar[str] = "kgcl:EdgeLogicalInterpretationChange"
-    class_name: ClassVar[str] = "edge logical interpretation change"
+    class_name: ClassVar[str] = "EdgeLogicalInterpretationChange"
     class_model_uri: ClassVar[URIRef] = KGCL.EdgeLogicalInterpretationChange
 
     id: Union[str, EdgeLogicalInterpretationChangeId] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
@@ -1259,20 +1201,19 @@
 
 
 @dataclass
 class LogicalAxiomChange(SimpleChange):
     """
     A simple change where a logical axiom is changed, where the logical axiom cannot be represented as an edge
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.LogicalAxiomChange
     class_class_curie: ClassVar[str] = "kgcl:LogicalAxiomChange"
-    class_name: ClassVar[str] = "logical axiom change"
+    class_name: ClassVar[str] = "LogicalAxiomChange"
     class_model_uri: ClassVar[URIRef] = KGCL.LogicalAxiomChange
 
     id: Union[str, LogicalAxiomChangeId] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
@@ -1283,53 +1224,49 @@
 
 
 @dataclass
 class NodeChange(SimpleChange):
     """
     A simple change where the change is about a node
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.NodeChange
     class_class_curie: ClassVar[str] = "kgcl:NodeChange"
-    class_name: ClassVar[str] = "node change"
+    class_name: ClassVar[str] = "NodeChange"
     class_model_uri: ClassVar[URIRef] = KGCL.NodeChange
 
     id: Union[str, NodeChangeId] = None
     about_node: Optional[Union[str, NodeId]] = None
     about_node_representation: Optional[str] = None
     language: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.about_node is not None and not isinstance(self.about_node, NodeId):
             self.about_node = NodeId(self.about_node)
 
-        if self.about_node_representation is not None and not isinstance(
-            self.about_node_representation, str
-        ):
+        if self.about_node_representation is not None and not isinstance(self.about_node_representation, str):
             self.about_node_representation = str(self.about_node_representation)
 
         if self.language is not None and not isinstance(self.language, str):
             self.language = str(self.language)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class NodeRename(NodeChange):
     """
     A node change where the name (aka rdfs:label) of the node changes
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.NodeRename
     class_class_curie: ClassVar[str] = "kgcl:NodeRename"
-    class_name: ClassVar[str] = "node rename"
+    class_name: ClassVar[str] = "NodeRename"
     class_model_uri: ClassVar[URIRef] = KGCL.NodeRename
 
     id: Union[str, NodeRenameId] = None
     old_value: Optional[str] = None
     new_value: Optional[str] = None
     has_textual_diff: Optional[Union[dict, "TextualDiff"]] = None
     new_language: Optional[str] = None
@@ -1344,44 +1281,39 @@
 
         if self.old_value is not None and not isinstance(self.old_value, str):
             self.old_value = str(self.old_value)
 
         if self.new_value is not None and not isinstance(self.new_value, str):
             self.new_value = str(self.new_value)
 
-        if self.has_textual_diff is not None and not isinstance(
-            self.has_textual_diff, TextualDiff
-        ):
+        if self.has_textual_diff is not None and not isinstance(self.has_textual_diff, TextualDiff):
             self.has_textual_diff = TextualDiff()
 
         if self.new_language is not None and not isinstance(self.new_language, str):
             self.new_language = str(self.new_language)
 
         if self.old_language is not None and not isinstance(self.old_language, str):
             self.old_language = str(self.old_language)
 
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class SetLanguageForName(NodeChange):
     """
     A node change where the string value for the name is unchanged but the language tag is set
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.SetLanguageForName
     class_class_curie: ClassVar[str] = "kgcl:SetLanguageForName"
-    class_name: ClassVar[str] = "set language for name"
+    class_name: ClassVar[str] = "SetLanguageForName"
     class_model_uri: ClassVar[URIRef] = KGCL.SetLanguageForName
 
     id: Union[str, SetLanguageForNameId] = None
     old_value: Optional[str] = None
     new_value: Optional[str] = None
     change_description: Optional[str] = None
 
@@ -1393,69 +1325,61 @@
 
         if self.old_value is not None and not isinstance(self.old_value, str):
             self.old_value = str(self.old_value)
 
         if self.new_value is not None and not isinstance(self.new_value, str):
             self.new_value = str(self.new_value)
 
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class NodeAnnotationChange(NodeChange):
     """
     A node change where the change alters node properties/annotations. TODO
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.NodeAnnotationChange
     class_class_curie: ClassVar[str] = "kgcl:NodeAnnotationChange"
-    class_name: ClassVar[str] = "node annotation change"
+    class_name: ClassVar[str] = "NodeAnnotationChange"
     class_model_uri: ClassVar[URIRef] = KGCL.NodeAnnotationChange
 
     id: Union[str, NodeAnnotationChangeId] = None
     annotation_property: Optional[str] = None
     annotation_property_type: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, NodeAnnotationChangeId):
             self.id = NodeAnnotationChangeId(self.id)
 
-        if self.annotation_property is not None and not isinstance(
-            self.annotation_property, str
-        ):
+        if self.annotation_property is not None and not isinstance(self.annotation_property, str):
             self.annotation_property = str(self.annotation_property)
 
-        if self.annotation_property_type is not None and not isinstance(
-            self.annotation_property_type, str
-        ):
+        if self.annotation_property_type is not None and not isinstance(self.annotation_property_type, str):
             self.annotation_property_type = str(self.annotation_property_type)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class NodeAnnotationReplacement(NodeAnnotationChange):
     """
     A node annotation change where the change replaces a particular property value. TODO
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.NodeAnnotationReplacement
     class_class_curie: ClassVar[str] = "kgcl:NodeAnnotationReplacement"
-    class_name: ClassVar[str] = "node annotation replacement"
+    class_name: ClassVar[str] = "NodeAnnotationReplacement"
     class_model_uri: ClassVar[URIRef] = KGCL.NodeAnnotationReplacement
 
     id: Union[str, NodeAnnotationReplacementId] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
@@ -1467,15 +1391,15 @@
 
 @dataclass
 class NodeSynonymChange(NodeChange):
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.NodeSynonymChange
     class_class_curie: ClassVar[str] = "kgcl:NodeSynonymChange"
-    class_name: ClassVar[str] = "node synonym change"
+    class_name: ClassVar[str] = "NodeSynonymChange"
     class_model_uri: ClassVar[URIRef] = KGCL.NodeSynonymChange
 
     id: Union[str, NodeSynonymChangeId] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
@@ -1486,20 +1410,19 @@
 
 
 @dataclass
 class NewSynonym(NodeSynonymChange):
     """
     A node synonym change where a de-novo synonym is created
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.NewSynonym
     class_class_curie: ClassVar[str] = "kgcl:NewSynonym"
-    class_name: ClassVar[str] = "new synonym"
+    class_name: ClassVar[str] = "NewSynonym"
     class_model_uri: ClassVar[URIRef] = KGCL.NewSynonym
 
     id: Union[str, NewSynonymId] = None
     new_value: Optional[str] = None
     language: Optional[str] = None
     qualifier: Optional[str] = None
 
@@ -1523,20 +1446,19 @@
 
 @dataclass
 class NameBecomesSynonym(NodeSynonymChange):
     """
     A node synonym where the name NAME of an node NODE moves to a synonym, and NODE receives a new name. This change
     consists of compose of (1) a node rename where NAME is replaced by a different name (2) a new synonym
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.NameBecomesSynonym
     class_class_curie: ClassVar[str] = "kgcl:NameBecomesSynonym"
-    class_name: ClassVar[str] = "name becomes synonym"
+    class_name: ClassVar[str] = "NameBecomesSynonym"
     class_model_uri: ClassVar[URIRef] = KGCL.NameBecomesSynonym
 
     id: Union[str, NameBecomesSynonymId] = None
     change_1: Optional[Union[str, NodeRenameId]] = None
     change_2: Optional[Union[str, NewSynonymId]] = None
     change_description: Optional[str] = None
 
@@ -1548,33 +1470,30 @@
 
         if self.change_1 is not None and not isinstance(self.change_1, NodeRenameId):
             self.change_1 = NodeRenameId(self.change_1)
 
         if self.change_2 is not None and not isinstance(self.change_2, NewSynonymId):
             self.change_2 = NewSynonymId(self.change_2)
 
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class RemoveSynonym(NodeSynonymChange):
     """
     A node synonym change where a synonym is deleted
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.RemoveSynonym
     class_class_curie: ClassVar[str] = "kgcl:RemoveSynonym"
-    class_name: ClassVar[str] = "remove synonym"
+    class_name: ClassVar[str] = "RemoveSynonym"
     class_model_uri: ClassVar[URIRef] = KGCL.RemoveSynonym
 
     id: Union[str, RemoveSynonymId] = None
     old_value: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
@@ -1589,20 +1508,19 @@
 
 
 @dataclass
 class SynonymReplacement(NodeSynonymChange):
     """
     A node synonym change where the text of a synonym is changed
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.SynonymReplacement
     class_class_curie: ClassVar[str] = "kgcl:SynonymReplacement"
-    class_name: ClassVar[str] = "synonym replacement"
+    class_name: ClassVar[str] = "SynonymReplacement"
     class_model_uri: ClassVar[URIRef] = KGCL.SynonymReplacement
 
     id: Union[str, SynonymReplacementId] = None
     old_value: Optional[str] = None
     new_value: Optional[str] = None
     has_textual_diff: Optional[Union[dict, "TextualDiff"]] = None
 
@@ -1614,35 +1532,32 @@
 
         if self.old_value is not None and not isinstance(self.old_value, str):
             self.old_value = str(self.old_value)
 
         if self.new_value is not None and not isinstance(self.new_value, str):
             self.new_value = str(self.new_value)
 
-        if self.has_textual_diff is not None and not isinstance(
-            self.has_textual_diff, TextualDiff
-        ):
+        if self.has_textual_diff is not None and not isinstance(self.has_textual_diff, TextualDiff):
             self.has_textual_diff = TextualDiff()
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class SynonymPredicateChange(NodeSynonymChange):
     """
     A node synonym change where the predicate of a synonym is changed. Background: synonyms can be represented by a
     variety of predicates. For example, many OBO ontologies make use of predicates such as oio:hasExactSynonym,
     oio:hasRelatedSynonym, etc
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.SynonymPredicateChange
     class_class_curie: ClassVar[str] = "kgcl:SynonymPredicateChange"
-    class_name: ClassVar[str] = "synonym predicate change"
+    class_name: ClassVar[str] = "SynonymPredicateChange"
     class_model_uri: ClassVar[URIRef] = KGCL.SynonymPredicateChange
 
     id: Union[str, SynonymPredicateChangeId] = None
     old_value: Optional[str] = None
     new_value: Optional[str] = None
     has_textual_diff: Optional[Union[dict, "TextualDiff"]] = None
 
@@ -1654,61 +1569,338 @@
 
         if self.old_value is not None and not isinstance(self.old_value, str):
             self.old_value = str(self.old_value)
 
         if self.new_value is not None and not isinstance(self.new_value, str):
             self.new_value = str(self.new_value)
 
-        if self.has_textual_diff is not None and not isinstance(
-            self.has_textual_diff, TextualDiff
-        ):
+        if self.has_textual_diff is not None and not isinstance(self.has_textual_diff, TextualDiff):
             self.has_textual_diff = TextualDiff()
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
-class NodeTextDefinitionChange(NodeChange):
+class NodeMappingChange(NodeChange):
     """
-    A node change where the text definition is changed
+    A node change where the mappings for that node are altered
     """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = KGCL.NodeMappingChange
+    class_class_curie: ClassVar[str] = "kgcl:NodeMappingChange"
+    class_name: ClassVar[str] = "NodeMappingChange"
+    class_model_uri: ClassVar[URIRef] = KGCL.NodeMappingChange
+
+    id: Union[str, NodeMappingChangeId] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, NodeMappingChangeId):
+            self.id = NodeMappingChangeId(self.id)
 
+        super().__post_init__(**kwargs)
+
+
+@dataclass
+class NewMapping(NodeMappingChange):
+    """
+    A node mapping change where a mapping is added to a node
+    """
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = KGCL.NodeTextDefinitionChange
-    class_class_curie: ClassVar[str] = "kgcl:NodeTextDefinitionChange"
-    class_name: ClassVar[str] = "node text definition change"
-    class_model_uri: ClassVar[URIRef] = KGCL.NodeTextDefinitionChange
+    class_class_uri: ClassVar[URIRef] = KGCL.NewMapping
+    class_class_curie: ClassVar[str] = "kgcl:NewMapping"
+    class_name: ClassVar[str] = "NewMapping"
+    class_model_uri: ClassVar[URIRef] = KGCL.NewMapping
 
-    id: Union[str, NodeTextDefinitionChangeId] = None
+    id: Union[str, NewMappingId] = None
+    object: Optional[Union[str, NodeId]] = None
+    predicate: Optional[Union[str, NodeId]] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, NewMappingId):
+            self.id = NewMappingId(self.id)
+
+        if self.object is not None and not isinstance(self.object, NodeId):
+            self.object = NodeId(self.object)
+
+        if self.predicate is not None and not isinstance(self.predicate, NodeId):
+            self.predicate = NodeId(self.predicate)
+
+        super().__post_init__(**kwargs)
+
+
+@dataclass
+class RemoveMapping(NodeMappingChange):
+    """
+    A node mapping change where a mapping is deleted
+    """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = KGCL.RemoveMapping
+    class_class_curie: ClassVar[str] = "kgcl:RemoveMapping"
+    class_name: ClassVar[str] = "RemoveMapping"
+    class_model_uri: ClassVar[URIRef] = KGCL.RemoveMapping
+
+    id: Union[str, RemoveMappingId] = None
+    object: Optional[Union[str, NodeId]] = None
+    predicate: Optional[Union[str, NodeId]] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, RemoveMappingId):
+            self.id = RemoveMappingId(self.id)
+
+        if self.object is not None and not isinstance(self.object, NodeId):
+            self.object = NodeId(self.object)
+
+        if self.predicate is not None and not isinstance(self.predicate, NodeId):
+            self.predicate = NodeId(self.predicate)
+
+        super().__post_init__(**kwargs)
+
+
+@dataclass
+class MappingReplacement(NodeMappingChange):
+    """
+    A node mapping change where the object of a mapping is changed
+    """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = KGCL.MappingReplacement
+    class_class_curie: ClassVar[str] = "kgcl:MappingReplacement"
+    class_name: ClassVar[str] = "MappingReplacement"
+    class_model_uri: ClassVar[URIRef] = KGCL.MappingReplacement
+
+    id: Union[str, MappingReplacementId] = None
+    old_value: Optional[str] = None
+    new_value: Optional[str] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, MappingReplacementId):
+            self.id = MappingReplacementId(self.id)
+
+        if self.old_value is not None and not isinstance(self.old_value, str):
+            self.old_value = str(self.old_value)
+
+        if self.new_value is not None and not isinstance(self.new_value, str):
+            self.new_value = str(self.new_value)
+
+        super().__post_init__(**kwargs)
+
+
+@dataclass
+class MappingPredicateChange(NodeMappingChange):
+    """
+    A node mapping change where the predicate of a mapping is changed.
+    """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = KGCL.MappingPredicateChange
+    class_class_curie: ClassVar[str] = "kgcl:MappingPredicateChange"
+    class_name: ClassVar[str] = "MappingPredicateChange"
+    class_model_uri: ClassVar[URIRef] = KGCL.MappingPredicateChange
+
+    id: Union[str, MappingPredicateChangeId] = None
+    old_value: Optional[str] = None
+    new_value: Optional[str] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, MappingPredicateChangeId):
+            self.id = MappingPredicateChangeId(self.id)
+
+        if self.old_value is not None and not isinstance(self.old_value, str):
+            self.old_value = str(self.old_value)
+
+        if self.new_value is not None and not isinstance(self.new_value, str):
+            self.new_value = str(self.new_value)
+
+        super().__post_init__(**kwargs)
+
+
+@dataclass
+class NodeMetadataAssertionChange(NodeChange):
+    """
+    A node change where the metadata assertion (OWL annotations) for that node are altered
+    """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = KGCL.NodeMetadataAssertionChange
+    class_class_curie: ClassVar[str] = "kgcl:NodeMetadataAssertionChange"
+    class_name: ClassVar[str] = "NodeMetadataAssertionChange"
+    class_model_uri: ClassVar[URIRef] = KGCL.NodeMetadataAssertionChange
+
+    id: Union[str, NodeMetadataAssertionChangeId] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, NodeMetadataAssertionChangeId):
+            self.id = NodeMetadataAssertionChangeId(self.id)
+
+        super().__post_init__(**kwargs)
+
+
+@dataclass
+class NewMetadataAssertion(NodeMetadataAssertionChange):
+    """
+    A node metadata assertion change where a metadata assertion is added to a node
+    """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = KGCL.NewMetadataAssertion
+    class_class_curie: ClassVar[str] = "kgcl:NewMetadataAssertion"
+    class_name: ClassVar[str] = "NewMetadataAssertion"
+    class_model_uri: ClassVar[URIRef] = KGCL.NewMetadataAssertion
+
+    id: Union[str, NewMetadataAssertionId] = None
+    object: Optional[Union[str, NodeId]] = None
+    predicate: Optional[Union[str, NodeId]] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, NewMetadataAssertionId):
+            self.id = NewMetadataAssertionId(self.id)
+
+        if self.object is not None and not isinstance(self.object, NodeId):
+            self.object = NodeId(self.object)
+
+        if self.predicate is not None and not isinstance(self.predicate, NodeId):
+            self.predicate = NodeId(self.predicate)
+
+        super().__post_init__(**kwargs)
+
+
+@dataclass
+class RemoveMetadataAssertion(NodeMetadataAssertionChange):
+    """
+    A node metadata assertion change where a metadata assertion is deleted
+    """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = KGCL.RemoveMetadataAssertion
+    class_class_curie: ClassVar[str] = "kgcl:RemoveMetadataAssertion"
+    class_name: ClassVar[str] = "RemoveMetadataAssertion"
+    class_model_uri: ClassVar[URIRef] = KGCL.RemoveMetadataAssertion
+
+    id: Union[str, RemoveMetadataAssertionId] = None
+    object: Optional[Union[str, NodeId]] = None
+    predicate: Optional[Union[str, NodeId]] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, RemoveMetadataAssertionId):
+            self.id = RemoveMetadataAssertionId(self.id)
+
+        if self.object is not None and not isinstance(self.object, NodeId):
+            self.object = NodeId(self.object)
+
+        if self.predicate is not None and not isinstance(self.predicate, NodeId):
+            self.predicate = NodeId(self.predicate)
+
+        super().__post_init__(**kwargs)
+
+
+@dataclass
+class MetadataAssertionReplacement(NodeMetadataAssertionChange):
+    """
+    A node metadata assertion change where the object of a metadata assertion is changed
+    """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = KGCL.MetadataAssertionReplacement
+    class_class_curie: ClassVar[str] = "kgcl:MetadataAssertionReplacement"
+    class_name: ClassVar[str] = "MetadataAssertionReplacement"
+    class_model_uri: ClassVar[URIRef] = KGCL.MetadataAssertionReplacement
+
+    id: Union[str, MetadataAssertionReplacementId] = None
+    old_value: Optional[str] = None
+    new_value: Optional[str] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, MetadataAssertionReplacementId):
+            self.id = MetadataAssertionReplacementId(self.id)
+
+        if self.old_value is not None and not isinstance(self.old_value, str):
+            self.old_value = str(self.old_value)
+
+        if self.new_value is not None and not isinstance(self.new_value, str):
+            self.new_value = str(self.new_value)
+
+        super().__post_init__(**kwargs)
+
+
+@dataclass
+class MetadataAssertionPredicateChange(NodeMetadataAssertionChange):
+    """
+    A node metadata assertion change where the predicate of a metadata assertion is changed.
+    """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = KGCL.MetadataAssertionPredicateChange
+    class_class_curie: ClassVar[str] = "kgcl:MetadataAssertionPredicateChange"
+    class_name: ClassVar[str] = "MetadataAssertionPredicateChange"
+    class_model_uri: ClassVar[URIRef] = KGCL.MetadataAssertionPredicateChange
+
+    id: Union[str, MetadataAssertionPredicateChangeId] = None
+    old_value: Optional[str] = None
+    new_value: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
-        if not isinstance(self.id, NodeTextDefinitionChangeId):
-            self.id = NodeTextDefinitionChangeId(self.id)
+        if not isinstance(self.id, MetadataAssertionPredicateChangeId):
+            self.id = MetadataAssertionPredicateChangeId(self.id)
+
         if self.old_value is not None and not isinstance(self.old_value, str):
             self.old_value = str(self.old_value)
+
         if self.new_value is not None and not isinstance(self.new_value, str):
             self.new_value = str(self.new_value)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
+class NodeTextDefinitionChange(NodeChange):
+    """
+    A node change where the text definition is changed
+    """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = KGCL.NodeTextDefinitionChange
+    class_class_curie: ClassVar[str] = "kgcl:NodeTextDefinitionChange"
+    class_name: ClassVar[str] = "NodeTextDefinitionChange"
+    class_model_uri: ClassVar[URIRef] = KGCL.NodeTextDefinitionChange
+
+    id: Union[str, NodeTextDefinitionChangeId] = None
+
+@dataclass
 class NewTextDefinition(NodeTextDefinitionChange):
     """
     A node change where a de-novo text definition is created
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.NewTextDefinition
     class_class_curie: ClassVar[str] = "kgcl:NewTextDefinition"
-    class_name: ClassVar[str] = "new text definition"
+    class_name: ClassVar[str] = "NewTextDefinition"
     class_model_uri: ClassVar[URIRef] = KGCL.NewTextDefinition
 
     id: Union[str, NewTextDefinitionId] = None
     new_value: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
@@ -1723,20 +1915,19 @@
 
 
 @dataclass
 class RemoveTextDefinition(NodeTextDefinitionChange):
     """
     A node change where a text definition is deleted
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.RemoveTextDefinition
     class_class_curie: ClassVar[str] = "kgcl:RemoveTextDefinition"
-    class_name: ClassVar[str] = "remove text definition"
+    class_name: ClassVar[str] = "RemoveTextDefinition"
     class_model_uri: ClassVar[URIRef] = KGCL.RemoveTextDefinition
 
     id: Union[str, RemoveTextDefinitionId] = None
     old_value: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
@@ -1751,20 +1942,19 @@
 
 
 @dataclass
 class TextDefinitionReplacement(NodeTextDefinitionChange):
     """
     A node change where a text definition is modified
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.TextDefinitionReplacement
     class_class_curie: ClassVar[str] = "kgcl:TextDefinitionReplacement"
-    class_name: ClassVar[str] = "text definition replacement"
+    class_name: ClassVar[str] = "TextDefinitionReplacement"
     class_model_uri: ClassVar[URIRef] = KGCL.TextDefinitionReplacement
 
     id: Union[str, TextDefinitionReplacementId] = None
     old_value: Optional[str] = None
     new_value: Optional[str] = None
     has_textual_diff: Optional[Union[dict, "TextualDiff"]] = None
 
@@ -1776,189 +1966,153 @@
 
         if self.old_value is not None and not isinstance(self.old_value, str):
             self.old_value = str(self.old_value)
 
         if self.new_value is not None and not isinstance(self.new_value, str):
             self.new_value = str(self.new_value)
 
-        if self.has_textual_diff is not None and not isinstance(
-            self.has_textual_diff, TextualDiff
-        ):
+        if self.has_textual_diff is not None and not isinstance(self.has_textual_diff, TextualDiff):
             self.has_textual_diff = TextualDiff()
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class AddNodeToSubset(NodeChange):
     """
     Places a node inside a subset, by annotating that node
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.AddNodeToSubset
     class_class_curie: ClassVar[str] = "kgcl:AddNodeToSubset"
-    class_name: ClassVar[str] = "add node to subset"
+    class_name: ClassVar[str] = "AddNodeToSubset"
     class_model_uri: ClassVar[URIRef] = KGCL.AddNodeToSubset
 
     id: Union[str, AddNodeToSubsetId] = None
     in_subset: Optional[Union[dict, "OntologySubset"]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, AddNodeToSubsetId):
             self.id = AddNodeToSubsetId(self.id)
 
-        if self.in_subset is not None and not isinstance(
-            self.in_subset, OntologySubset
-        ):
+        if self.in_subset is not None and not isinstance(self.in_subset, OntologySubset):
             self.in_subset = OntologySubset()
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
-class RemovedNodeFromSubset(NodeChange):
+class RemoveNodeFromSubset(NodeChange):
     """
     Removes a node from a subset, by removing an annotation
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = KGCL.RemovedNodeFromSubset
-    class_class_curie: ClassVar[str] = "kgcl:RemovedNodeFromSubset"
-    class_name: ClassVar[str] = "removed node from subset"
-    class_model_uri: ClassVar[URIRef] = KGCL.RemovedNodeFromSubset
+    class_class_uri: ClassVar[URIRef] = KGCL.RemoveNodeFromSubset
+    class_class_curie: ClassVar[str] = "kgcl:RemoveNodeFromSubset"
+    class_name: ClassVar[str] = "RemoveNodeFromSubset"
+    class_model_uri: ClassVar[URIRef] = KGCL.RemoveNodeFromSubset
 
-    id: Union[str, RemovedNodeFromSubsetId] = None
+    id: Union[str, RemoveNodeFromSubsetId] = None
     change_description: Optional[str] = None
     about_node: Optional[Union[str, NodeId]] = None
     subset: Optional[str] = None
     in_subset: Optional[Union[dict, "OntologySubset"]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
-        if not isinstance(self.id, RemovedNodeFromSubsetId):
-            self.id = RemovedNodeFromSubsetId(self.id)
+        if not isinstance(self.id, RemoveNodeFromSubsetId):
+            self.id = RemoveNodeFromSubsetId(self.id)
 
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
         if self.about_node is not None and not isinstance(self.about_node, NodeId):
             self.about_node = NodeId(self.about_node)
 
         if self.subset is not None and not isinstance(self.subset, str):
             self.subset = str(self.subset)
 
-        if self.in_subset is not None and not isinstance(
-            self.in_subset, OntologySubset
-        ):
+        if self.in_subset is not None and not isinstance(self.in_subset, OntologySubset):
             self.in_subset = OntologySubset()
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class NodeObsoletion(NodeChange):
     """
     Obsoletion of a node deprecates usage of that node, but does not delete it.
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.NodeObsoletion
     class_class_curie: ClassVar[str] = "kgcl:NodeObsoletion"
-    class_name: ClassVar[str] = "node obsoletion"
+    class_name: ClassVar[str] = "NodeObsoletion"
     class_model_uri: ClassVar[URIRef] = KGCL.NodeObsoletion
 
     id: Union[str, NodeObsoletionId] = None
     has_direct_replacement: Optional[Union[str, NodeId]] = None
-    has_nondirect_replacement: Optional[
-        Union[Union[str, NodeId], List[Union[str, NodeId]]]
-    ] = empty_list()
-    change_description: Optional[str] = None
-    associated_change_set: Optional[
-        Union[
-            Dict[Union[str, ChangeId], Union[dict, Change]], List[Union[dict, Change]]
-        ]
-    ] = empty_dict()
+    has_nondirect_replacement: Optional[Union[Union[str, NodeId], List[Union[str, NodeId]]]] = empty_list()
+    change_description: Optional[str] = None
+    associated_change_set: Optional[Union[Dict[Union[str, ChangeId], Union[dict, Change]], List[Union[dict, Change]]]] = empty_dict()
     about: Optional[Union[dict, "OntologyElement"]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, NodeObsoletionId):
             self.id = NodeObsoletionId(self.id)
 
-        if self.has_direct_replacement is not None and not isinstance(
-            self.has_direct_replacement, NodeId
-        ):
+        if self.has_direct_replacement is not None and not isinstance(self.has_direct_replacement, NodeId):
             self.has_direct_replacement = NodeId(self.has_direct_replacement)
 
         if not isinstance(self.has_nondirect_replacement, list):
-            self.has_nondirect_replacement = (
-                [self.has_nondirect_replacement]
-                if self.has_nondirect_replacement is not None
-                else []
-            )
-        self.has_nondirect_replacement = [
-            v if isinstance(v, NodeId) else NodeId(v)
-            for v in self.has_nondirect_replacement
-        ]
-
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
-            self.change_description = str(self.change_description)
-
-        self._normalize_inlined_as_list(
-            slot_name="associated_change_set",
-            slot_type=Change,
-            key_name="id",
-            keyed=True,
-        )
+            self.has_nondirect_replacement = [self.has_nondirect_replacement] if self.has_nondirect_replacement is not None else []
+        self.has_nondirect_replacement = [v if isinstance(v, NodeId) else NodeId(v) for v in self.has_nondirect_replacement]
+
+        if self.change_description is not None and not isinstance(self.change_description, str):
+            self.change_description = str(self.change_description)
+
+        self._normalize_inlined_as_list(slot_name="associated_change_set", slot_type=Change, key_name="id", keyed=True)
 
         if self.about is not None and not isinstance(self.about, OntologyElement):
             self.about = OntologyElement()
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class NodeUnobsoletion(NodeChange):
     """
     unobsoletion of a node deprecates usage of that node. Rarely applied.
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.NodeUnobsoletion
     class_class_curie: ClassVar[str] = "kgcl:NodeUnobsoletion"
-    class_name: ClassVar[str] = "node unobsoletion"
+    class_name: ClassVar[str] = "NodeUnobsoletion"
     class_model_uri: ClassVar[URIRef] = KGCL.NodeUnobsoletion
 
     id: Union[str, NodeUnobsoletionId] = None
     change_description: Optional[str] = None
     replaced_by: Optional[Union[str, NodeId]] = None
     consider: Optional[Union[str, NodeId]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, NodeUnobsoletionId):
             self.id = NodeUnobsoletionId(self.id)
 
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
         if self.replaced_by is not None and not isinstance(self.replaced_by, NodeId):
             self.replaced_by = NodeId(self.replaced_by)
 
         if self.consider is not None and not isinstance(self.consider, NodeId):
             self.consider = NodeId(self.consider)
@@ -1967,20 +2121,19 @@
 
 
 @dataclass
 class NodeCreation(NodeChange):
     """
     a node change in which a new node is created
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.NodeCreation
     class_class_curie: ClassVar[str] = "kgcl:NodeCreation"
-    class_name: ClassVar[str] = "node creation"
+    class_name: ClassVar[str] = "NodeCreation"
     class_model_uri: ClassVar[URIRef] = KGCL.NodeCreation
 
     id: Union[str, NodeCreationId] = None
     node_id: Optional[Union[str, NodeId]] = None
     name: Optional[str] = None
     owl_type: Optional[Union[str, "OwlTypeEnum"]] = None
     annotation_set: Optional[Union[dict, "Annotation"]] = None
@@ -1998,41 +2151,36 @@
 
         if self.name is not None and not isinstance(self.name, str):
             self.name = str(self.name)
 
         if self.owl_type is not None and not isinstance(self.owl_type, OwlTypeEnum):
             self.owl_type = OwlTypeEnum(self.owl_type)
 
-        if self.annotation_set is not None and not isinstance(
-            self.annotation_set, Annotation
-        ):
+        if self.annotation_set is not None and not isinstance(self.annotation_set, Annotation):
             self.annotation_set = Annotation(**as_dict(self.annotation_set))
 
         if self.language is not None and not isinstance(self.language, str):
             self.language = str(self.language)
 
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class ClassCreation(NodeCreation):
     """
-    A node creation where the owl type is 'class'
+    A node creation where the owl type is 'owl:Class'
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.ClassCreation
     class_class_curie: ClassVar[str] = "kgcl:ClassCreation"
-    class_name: ClassVar[str] = "class creation"
+    class_name: ClassVar[str] = "ClassCreation"
     class_model_uri: ClassVar[URIRef] = KGCL.ClassCreation
 
     id: Union[str, ClassCreationId] = None
     superclass: Optional[Union[str, NodeId]] = None
     change_description: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
@@ -2040,65 +2188,86 @@
             self.MissingRequiredField("id")
         if not isinstance(self.id, ClassCreationId):
             self.id = ClassCreationId(self.id)
 
         if self.superclass is not None and not isinstance(self.superclass, NodeId):
             self.superclass = NodeId(self.superclass)
 
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        if self.change_description is not None and not isinstance(self.change_description, str):
+            self.change_description = str(self.change_description)
+
+        super().__post_init__(**kwargs)
+
+
+@dataclass
+class ObjectPropertyCreation(NodeCreation):
+    """
+    A node creation where the owl type is 'ObjectProperty'
+    """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = KGCL.ObjectPropertyCreation
+    class_class_curie: ClassVar[str] = "kgcl:ObjectPropertyCreation"
+    class_name: ClassVar[str] = "ObjectPropertyCreation"
+    class_model_uri: ClassVar[URIRef] = KGCL.ObjectPropertyCreation
+
+    id: Union[str, ObjectPropertyCreationId] = None
+    change_description: Optional[str] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, ObjectPropertyCreationId):
+            self.id = ObjectPropertyCreationId(self.id)
+
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class NodeDeletion(NodeChange):
     """
     Deletion of a node from the graph. Note it is recommended nodes are obsoleted and never merged, but this operation
     exists to represent deletions in ontologies, accidental or otherwise
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.NodeDeletion
     class_class_curie: ClassVar[str] = "kgcl:NodeDeletion"
-    class_name: ClassVar[str] = "node deletion"
+    class_name: ClassVar[str] = "NodeDeletion"
     class_model_uri: ClassVar[URIRef] = KGCL.NodeDeletion
 
     id: Union[str, NodeDeletionId] = None
     change_description: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, NodeDeletionId):
             self.id = NodeDeletionId(self.id)
 
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class NodeDirectMerge(NodeObsoletion):
     """
     An obsoletion change in which all metadata (including name/label) from the source node is deleted and added to the
     target node, and edges can automatically be rewired to point to the target node
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.NodeDirectMerge
     class_class_curie: ClassVar[str] = "kgcl:NodeDirectMerge"
-    class_name: ClassVar[str] = "node direct merge"
+    class_name: ClassVar[str] = "NodeDirectMerge"
     class_model_uri: ClassVar[URIRef] = KGCL.NodeDirectMerge
 
     id: Union[str, NodeDirectMergeId] = None
     has_direct_replacement: Union[str, NodeId] = None
     about_node: Optional[Union[str, NodeId]] = None
     change_description: Optional[str] = None
 
@@ -2112,34 +2281,31 @@
             self.MissingRequiredField("has_direct_replacement")
         if not isinstance(self.has_direct_replacement, NodeId):
             self.has_direct_replacement = NodeId(self.has_direct_replacement)
 
         if self.about_node is not None and not isinstance(self.about_node, NodeId):
             self.about_node = NodeId(self.about_node)
 
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class NodeObsoletionWithDirectReplacement(NodeObsoletion):
     """
     An obsoletion change in which information from the obsoleted node is selectively copied to a single target, and
     edges can automatically be rewired to point to the target node
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.NodeObsoletionWithDirectReplacement
     class_class_curie: ClassVar[str] = "kgcl:NodeObsoletionWithDirectReplacement"
-    class_name: ClassVar[str] = "node obsoletion with direct replacement"
+    class_name: ClassVar[str] = "NodeObsoletionWithDirectReplacement"
     class_model_uri: ClassVar[URIRef] = KGCL.NodeObsoletionWithDirectReplacement
 
     id: Union[str, NodeObsoletionWithDirectReplacementId] = None
     has_direct_replacement: Union[str, NodeId] = None
     change_description: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
@@ -2149,206 +2315,169 @@
             self.id = NodeObsoletionWithDirectReplacementId(self.id)
 
         if self._is_empty(self.has_direct_replacement):
             self.MissingRequiredField("has_direct_replacement")
         if not isinstance(self.has_direct_replacement, NodeId):
             self.has_direct_replacement = NodeId(self.has_direct_replacement)
 
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class NodeObsoletionWithNoDirectReplacement(NodeObsoletion):
     """
     An obsoletion change in which there is no direct replacement
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.NodeObsoletionWithNoDirectReplacement
     class_class_curie: ClassVar[str] = "kgcl:NodeObsoletionWithNoDirectReplacement"
-    class_name: ClassVar[str] = "node obsoletion with no direct replacement"
+    class_name: ClassVar[str] = "NodeObsoletionWithNoDirectReplacement"
     class_model_uri: ClassVar[URIRef] = KGCL.NodeObsoletionWithNoDirectReplacement
 
     id: Union[str, NodeObsoletionWithNoDirectReplacementId] = None
-    has_nondirect_replacement: Union[
-        Union[str, NodeId], List[Union[str, NodeId]]
-    ] = None
+    has_nondirect_replacement: Union[Union[str, NodeId], List[Union[str, NodeId]]] = None
     change_description: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, NodeObsoletionWithNoDirectReplacementId):
             self.id = NodeObsoletionWithNoDirectReplacementId(self.id)
 
         if self._is_empty(self.has_nondirect_replacement):
             self.MissingRequiredField("has_nondirect_replacement")
         if not isinstance(self.has_nondirect_replacement, list):
-            self.has_nondirect_replacement = (
-                [self.has_nondirect_replacement]
-                if self.has_nondirect_replacement is not None
-                else []
-            )
-        self.has_nondirect_replacement = [
-            v if isinstance(v, NodeId) else NodeId(v)
-            for v in self.has_nondirect_replacement
-        ]
+            self.has_nondirect_replacement = [self.has_nondirect_replacement] if self.has_nondirect_replacement is not None else []
+        self.has_nondirect_replacement = [v if isinstance(v, NodeId) else NodeId(v) for v in self.has_nondirect_replacement]
 
-        if self.change_description is not None and not isinstance(
-            self.change_description, str
-        ):
+        if self.change_description is not None and not isinstance(self.change_description, str):
             self.change_description = str(self.change_description)
 
         super().__post_init__(**kwargs)
 
 
-class TextualDiff(YAMLRoot):
+class TextualDiff(ChangeLanguageElement):
     """
     A summarizing of a change on a piece of text. This could be rendered in a number of different ways
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.TextualDiff
     class_class_curie: ClassVar[str] = "kgcl:TextualDiff"
-    class_name: ClassVar[str] = "textual diff"
+    class_name: ClassVar[str] = "TextualDiff"
     class_model_uri: ClassVar[URIRef] = KGCL.TextualDiff
 
 
 @dataclass
-class Configuration(YAMLRoot):
+class Configuration(ChangeLanguageElement):
     """
     The meaning of operations can be configured
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.Configuration
     class_class_curie: ClassVar[str] = "kgcl:Configuration"
-    class_name: ClassVar[str] = "configuration"
+    class_name: ClassVar[str] = "Configuration"
     class_model_uri: ClassVar[URIRef] = KGCL.Configuration
 
     name_predicate: Optional[str] = None
     definition_predicate: Optional[str] = None
     main_synonym_predicate: Optional[str] = None
     synonym_predicates: Optional[str] = None
     creator_predicate: Optional[str] = None
     contributor_predicate: Optional[str] = None
+    obsolete_node_label_prefix: Optional[str] = None
     obsoletion_workflow: Optional[str] = None
-    obsoletion_policy: Optional[str] = None
+    obsoletion_policies: Optional[Union[Union[str, "ObsoletionPolicyEnum"], List[Union[str, "ObsoletionPolicyEnum"]]]] = empty_list()
+    obsolete_subclass_of_shadow_property: Optional[Union[str, URIorCURIE]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.name_predicate is not None and not isinstance(self.name_predicate, str):
             self.name_predicate = str(self.name_predicate)
 
-        if self.definition_predicate is not None and not isinstance(
-            self.definition_predicate, str
-        ):
+        if self.definition_predicate is not None and not isinstance(self.definition_predicate, str):
             self.definition_predicate = str(self.definition_predicate)
 
-        if self.main_synonym_predicate is not None and not isinstance(
-            self.main_synonym_predicate, str
-        ):
+        if self.main_synonym_predicate is not None and not isinstance(self.main_synonym_predicate, str):
             self.main_synonym_predicate = str(self.main_synonym_predicate)
 
-        if self.synonym_predicates is not None and not isinstance(
-            self.synonym_predicates, str
-        ):
+        if self.synonym_predicates is not None and not isinstance(self.synonym_predicates, str):
             self.synonym_predicates = str(self.synonym_predicates)
 
-        if self.creator_predicate is not None and not isinstance(
-            self.creator_predicate, str
-        ):
+        if self.creator_predicate is not None and not isinstance(self.creator_predicate, str):
             self.creator_predicate = str(self.creator_predicate)
 
-        if self.contributor_predicate is not None and not isinstance(
-            self.contributor_predicate, str
-        ):
+        if self.contributor_predicate is not None and not isinstance(self.contributor_predicate, str):
             self.contributor_predicate = str(self.contributor_predicate)
 
-        if self.obsoletion_workflow is not None and not isinstance(
-            self.obsoletion_workflow, str
-        ):
+        if self.obsolete_node_label_prefix is not None and not isinstance(self.obsolete_node_label_prefix, str):
+            self.obsolete_node_label_prefix = str(self.obsolete_node_label_prefix)
+
+        if self.obsoletion_workflow is not None and not isinstance(self.obsoletion_workflow, str):
             self.obsoletion_workflow = str(self.obsoletion_workflow)
 
-        if self.obsoletion_policy is not None and not isinstance(
-            self.obsoletion_policy, str
-        ):
-            self.obsoletion_policy = str(self.obsoletion_policy)
+        if not isinstance(self.obsoletion_policies, list):
+            self.obsoletion_policies = [self.obsoletion_policies] if self.obsoletion_policies is not None else []
+        self.obsoletion_policies = [v if isinstance(v, ObsoletionPolicyEnum) else ObsoletionPolicyEnum(v) for v in self.obsoletion_policies]
+
+        if self.obsolete_subclass_of_shadow_property is not None and not isinstance(self.obsolete_subclass_of_shadow_property, URIorCURIE):
+            self.obsolete_subclass_of_shadow_property = URIorCURIE(self.obsolete_subclass_of_shadow_property)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
-class Session(YAMLRoot):
+class Session(ChangeLanguageElement):
     """
     A session consists of a set of change sets bundled with the activities that generated those change sets
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = KGCL.Session
     class_class_curie: ClassVar[str] = "kgcl:Session"
-    class_name: ClassVar[str] = "session"
+    class_name: ClassVar[str] = "Session"
     class_model_uri: ClassVar[URIRef] = KGCL.Session
 
-    change_set: Optional[
-        Union[
-            Dict[Union[str, ChangeId], Union[dict, Change]], List[Union[dict, Change]]
-        ]
-    ] = empty_dict()
-    activity_set: Optional[
-        Union[
-            Dict[Union[str, ActivityId], Union[dict, "Activity"]],
-            List[Union[dict, "Activity"]],
-        ]
-    ] = empty_dict()
-
-    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        self._normalize_inlined_as_list(
-            slot_name="change_set", slot_type=Change, key_name="id", keyed=True
-        )
-
-        self._normalize_inlined_as_list(
-            slot_name="activity_set", slot_type=Activity, key_name="id", keyed=True
-        )
+    change_set: Optional[Union[Dict[Union[str, ChangeId], Union[dict, Change]], List[Union[dict, Change]]]] = empty_dict()
+    activity_set: Optional[Union[Dict[Union[str, ActivityId], Union[dict, "Activity"]], List[Union[dict, "Activity"]]]] = empty_dict()
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        self._normalize_inlined_as_list(slot_name="change_set", slot_type=Change, key_name="id", keyed=True)
+
+        self._normalize_inlined_as_list(slot_name="activity_set", slot_type=Activity, key_name="id", keyed=True)
 
         super().__post_init__(**kwargs)
 
 
 class OntologyElement(YAMLRoot):
     """
     Any component of an ontology or knowledge graph
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = OM.OntologyElement
     class_class_curie: ClassVar[str] = "om:OntologyElement"
-    class_name: ClassVar[str] = "ontology element"
+    class_name: ClassVar[str] = "OntologyElement"
     class_model_uri: ClassVar[URIRef] = KGCL.OntologyElement
 
 
 @dataclass
 class PropertyValue(OntologyElement):
     """
     a property-value pair
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = OM.PropertyValue
     class_class_curie: ClassVar[str] = "om:PropertyValue"
-    class_name: ClassVar[str] = "property value"
+    class_name: ClassVar[str] = "PropertyValue"
     class_model_uri: ClassVar[URIRef] = KGCL.PropertyValue
 
     property: Optional[Union[str, NodeId]] = None
     filler: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.property is not None and not isinstance(self.property, NodeId):
@@ -2361,20 +2490,19 @@
 
 
 @dataclass
 class Annotation(PropertyValue):
     """
     owl annotations. Not to be confused with annotations sensu GO
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = OM.Annotation
     class_class_curie: ClassVar[str] = "om:Annotation"
-    class_name: ClassVar[str] = "annotation"
+    class_name: ClassVar[str] = "Annotation"
     class_model_uri: ClassVar[URIRef] = KGCL.Annotation
 
     property: Optional[Union[str, NodeId]] = None
     filler: Optional[str] = None
     annotation_set: Optional[Union[dict, "Annotation"]] = None
     property_type: Optional[str] = None
     filler_type: Optional[str] = None
@@ -2382,17 +2510,15 @@
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.property is not None and not isinstance(self.property, NodeId):
             self.property = NodeId(self.property)
 
         if self.filler is not None and not isinstance(self.filler, str):
             self.filler = str(self.filler)
 
-        if self.annotation_set is not None and not isinstance(
-            self.annotation_set, Annotation
-        ):
+        if self.annotation_set is not None and not isinstance(self.annotation_set, Annotation):
             self.annotation_set = Annotation(**as_dict(self.annotation_set))
 
         if self.property_type is not None and not isinstance(self.property_type, str):
             self.property_type = str(self.property_type)
 
         if self.filler_type is not None and not isinstance(self.filler_type, str):
             self.filler_type = str(self.filler_type)
@@ -2401,20 +2527,19 @@
 
 
 @dataclass
 class Node(OntologyElement):
     """
     Any named entity in an ontology. May be a class, individual, property
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = OM.Node
     class_class_curie: ClassVar[str] = "om:Node"
-    class_name: ClassVar[str] = "node"
+    class_name: ClassVar[str] = "Node"
     class_model_uri: ClassVar[URIRef] = KGCL.Node
 
     id: Union[str, NodeId] = None
     name: Optional[str] = None
     annotation_set: Optional[Union[dict, Annotation]] = None
     owl_type: Optional[Union[str, "OwlTypeEnum"]] = None
 
@@ -2423,36 +2548,33 @@
             self.MissingRequiredField("id")
         if not isinstance(self.id, NodeId):
             self.id = NodeId(self.id)
 
         if self.name is not None and not isinstance(self.name, str):
             self.name = str(self.name)
 
-        if self.annotation_set is not None and not isinstance(
-            self.annotation_set, Annotation
-        ):
+        if self.annotation_set is not None and not isinstance(self.annotation_set, Annotation):
             self.annotation_set = Annotation(**as_dict(self.annotation_set))
 
         if self.owl_type is not None and not isinstance(self.owl_type, OwlTypeEnum):
             self.owl_type = OwlTypeEnum(self.owl_type)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class ClassNode(Node):
     """
     A node that is a class
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = OWL.Class
     class_class_curie: ClassVar[str] = "owl:Class"
-    class_name: ClassVar[str] = "class node"
+    class_name: ClassVar[str] = "ClassNode"
     class_model_uri: ClassVar[URIRef] = KGCL.ClassNode
 
     id: Union[str, ClassNodeId] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
@@ -2463,20 +2585,19 @@
 
 
 @dataclass
 class InstanceNode(Node):
     """
     A node that is an individual
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = OWL.NamedIndividual
     class_class_curie: ClassVar[str] = "owl:NamedIndividual"
-    class_name: ClassVar[str] = "instance node"
+    class_name: ClassVar[str] = "InstanceNode"
     class_model_uri: ClassVar[URIRef] = KGCL.InstanceNode
 
     id: Union[str, InstanceNodeId] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
@@ -2494,32 +2615,30 @@
 
     * A subClassOf B <==> Edge(subject=A, predicate=owl:subClassOf, object=B)
     * A subClassOf P some B <==> Edge(subject=A, predicate=P, object=B)
     * P subPropertyOf Q <==> Edge(subject=P, predicate=owl:subPropertyOf, object=Q)
 
     These represent the most common kind of pairwise relationship between classes, and classes are the dominant node
     type in ontologies.
-
     In future a wider variety of OWL axiom types will be supportedn through the use of an additional edge
     property/slot to indicate the interpretation of the axiom, following owlstar
     (https://github.com/cmungall/owlstar).
     For example:
     * `A subClassOf R only B <==> Edge(subject=A, predicate=P, object=B, interpretation=AllOnly)`
     * `A Annotation(P,B) <==> Edge(subject=A, predicate=P, object=B, interpretation=annotationAssertion)`
 
     Note that not all axioms are intended to map to edges. Axioms/triples where the object is a literal would be
     represented as node properties. Complex OWL axioms involving nesting would have their own dedicated construct, or
     may be represented generically. These are out of scope for the current version of KGCL
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = OM.Edge
     class_class_curie: ClassVar[str] = "om:Edge"
-    class_name: ClassVar[str] = "edge"
+    class_name: ClassVar[str] = "Edge"
     class_model_uri: ClassVar[URIRef] = KGCL.Edge
 
     subject: Optional[Union[str, NodeId]] = None
     predicate: Optional[Union[str, NodeId]] = None
     object: Optional[Union[str, NodeId]] = None
     subject_representation: Optional[str] = None
     predicate_representation: Optional[str] = None
@@ -2532,66 +2651,69 @@
 
         if self.predicate is not None and not isinstance(self.predicate, NodeId):
             self.predicate = NodeId(self.predicate)
 
         if self.object is not None and not isinstance(self.object, NodeId):
             self.object = NodeId(self.object)
 
-        if self.subject_representation is not None and not isinstance(
-            self.subject_representation, str
-        ):
+        if self.subject_representation is not None and not isinstance(self.subject_representation, str):
             self.subject_representation = str(self.subject_representation)
 
-        if self.predicate_representation is not None and not isinstance(
-            self.predicate_representation, str
-        ):
+        if self.predicate_representation is not None and not isinstance(self.predicate_representation, str):
             self.predicate_representation = str(self.predicate_representation)
 
-        if self.object_representation is not None and not isinstance(
-            self.object_representation, str
-        ):
+        if self.object_representation is not None and not isinstance(self.object_representation, str):
             self.object_representation = str(self.object_representation)
 
-        if self.annotation_set is not None and not isinstance(
-            self.annotation_set, Annotation
-        ):
+        if self.annotation_set is not None and not isinstance(self.annotation_set, Annotation):
             self.annotation_set = Annotation(**as_dict(self.annotation_set))
 
         super().__post_init__(**kwargs)
 
 
 class LogicalDefinition(OntologyElement):
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = OM.LogicalDefinition
     class_class_curie: ClassVar[str] = "om:LogicalDefinition"
-    class_name: ClassVar[str] = "logical definition"
+    class_name: ClassVar[str] = "LogicalDefinition"
     class_model_uri: ClassVar[URIRef] = KGCL.LogicalDefinition
 
 
 class OntologySubset(OntologyElement):
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = OM.OntologySubset
     class_class_curie: ClassVar[str] = "om:OntologySubset"
-    class_name: ClassVar[str] = "ontology subset"
+    class_name: ClassVar[str] = "OntologySubset"
     class_model_uri: ClassVar[URIRef] = KGCL.OntologySubset
 
 
+class ProvElement(YAMLRoot):
+    """
+    A grouping for prov elements
+    """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = PROV.ProvElement
+    class_class_curie: ClassVar[str] = "prov:ProvElement"
+    class_name: ClassVar[str] = "ProvElement"
+    class_model_uri: ClassVar[URIRef] = KGCL.ProvElement
+
+
 @dataclass
-class Activity(YAMLRoot):
+class Activity(ProvElement):
     """
     a provence-generating activity
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = PROV.Activity
     class_class_curie: ClassVar[str] = "prov:Activity"
-    class_name: ClassVar[str] = "activity"
+    class_name: ClassVar[str] = "Activity"
     class_model_uri: ClassVar[URIRef] = KGCL.Activity
 
     id: Union[str, ActivityId] = None
     started_at_time: Optional[str] = None
     ended_at_time: Optional[str] = None
     was_informed_by: Optional[Union[str, ActivityId]] = None
     was_associated_with: Optional[Union[str, AgentId]] = None
@@ -2600,1419 +2722,555 @@
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, ActivityId):
             self.id = ActivityId(self.id)
 
-        if self.started_at_time is not None and not isinstance(
-            self.started_at_time, str
-        ):
+        if self.started_at_time is not None and not isinstance(self.started_at_time, str):
             self.started_at_time = str(self.started_at_time)
 
         if self.ended_at_time is not None and not isinstance(self.ended_at_time, str):
             self.ended_at_time = str(self.ended_at_time)
 
-        if self.was_informed_by is not None and not isinstance(
-            self.was_informed_by, ActivityId
-        ):
+        if self.was_informed_by is not None and not isinstance(self.was_informed_by, ActivityId):
             self.was_informed_by = ActivityId(self.was_informed_by)
 
-        if self.was_associated_with is not None and not isinstance(
-            self.was_associated_with, AgentId
-        ):
+        if self.was_associated_with is not None and not isinstance(self.was_associated_with, AgentId):
             self.was_associated_with = AgentId(self.was_associated_with)
 
         if self.used is not None and not isinstance(self.used, str):
             self.used = str(self.used)
 
         if self.description is not None and not isinstance(self.description, str):
             self.description = str(self.description)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
-class Agent(YAMLRoot):
+class Agent(ProvElement):
     """
     a provence-generating agent
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = PROV.Agent
     class_class_curie: ClassVar[str] = "prov:Agent"
-    class_name: ClassVar[str] = "agent"
+    class_name: ClassVar[str] = "Agent"
     class_model_uri: ClassVar[URIRef] = KGCL.Agent
 
     id: Union[str, AgentId] = None
     acted_on_behalf_of: Optional[Union[str, AgentId]] = None
     was_informed_by: Optional[Union[str, ActivityId]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, AgentId):
             self.id = AgentId(self.id)
 
-        if self.acted_on_behalf_of is not None and not isinstance(
-            self.acted_on_behalf_of, AgentId
-        ):
+        if self.acted_on_behalf_of is not None and not isinstance(self.acted_on_behalf_of, AgentId):
             self.acted_on_behalf_of = AgentId(self.acted_on_behalf_of)
 
-        if self.was_informed_by is not None and not isinstance(
-            self.was_informed_by, ActivityId
-        ):
+        if self.was_informed_by is not None and not isinstance(self.was_informed_by, ActivityId):
             self.was_informed_by = ActivityId(self.was_informed_by)
 
         super().__post_init__(**kwargs)
 
 
 # Enumerations
+class ObsoletionPolicyEnum(EnumDefinitionImpl):
+
+    NoLogicalAxiomsOnObsoletes = PermissibleValue(
+        text="NoLogicalAxiomsOnObsoletes",
+        description="The obsoletion policy is that there MUST NOT be logical axioms about an obsolete node")
+    ObsoleteLabelsArePrefixed = PermissibleValue(
+        text="ObsoleteLabelsArePrefixed",
+        description="""The obsoletion policy is that any label on an obsolete node MUST be prefixed with 'obsolete' or similar""")
+
+    _defn = EnumDefinition(
+        name="ObsoletionPolicyEnum",
+    )
+
 class OwlTypeEnum(EnumDefinitionImpl):
 
-    CLASS = PermissibleValue(text="CLASS", meaning=OWL.Class)
+    CLASS = PermissibleValue(
+        text="CLASS",
+        meaning=OWL.Class)
     OBJECT_PROPERTY = PermissibleValue(
-        text="OBJECT_PROPERTY", meaning=OWL.ObjectProperty
-    )
+        text="OBJECT_PROPERTY",
+        meaning=OWL.ObjectProperty)
     NAMED_INDIVIDUAL = PermissibleValue(
-        text="NAMED_INDIVIDUAL", meaning=OWL.NamedIndividual
-    )
+        text="NAMED_INDIVIDUAL",
+        meaning=OWL.NamedIndividual)
 
     _defn = EnumDefinition(
         name="OwlTypeEnum",
     )
 
-
 class SynonymScopeEnum(EnumDefinitionImpl):
 
-    related = PermissibleValue(text="related", meaning=OIO.hasNarrowSynonym)
-    broad = PermissibleValue(text="broad", meaning=OIO.hasBroadSynonym)
-    narrow = PermissibleValue(text="narrow", meaning=OIO.hasNarrowSynonym)
-    exact = PermissibleValue(text="exact", meaning=OIO.hasExactSynonym)
+    related = PermissibleValue(
+        text="related",
+        meaning=OIO.hasNarrowSynonym)
+    broad = PermissibleValue(
+        text="broad",
+        meaning=OIO.hasBroadSynonym)
+    narrow = PermissibleValue(
+        text="narrow",
+        meaning=OIO.hasNarrowSynonym)
+    exact = PermissibleValue(
+        text="exact",
+        meaning=OIO.hasExactSynonym)
 
     _defn = EnumDefinition(
         name="SynonymScopeEnum",
     )
 
-
 # Slots
 class slots:
     pass
 
+slots.type = Slot(uri=RDF.type, name="type", curie=RDF.curie('type'),
+                   model_uri=KGCL.type, domain=None, range=Optional[str])
+
+slots.pull_request = Slot(uri=KGCL.pull_request, name="pull_request", curie=KGCL.curie('pull_request'),
+                   model_uri=KGCL.pull_request, domain=None, range=Optional[str])
+
+slots.see_also = Slot(uri=RDFS.seeAlso, name="see_also", curie=RDFS.curie('seeAlso'),
+                   model_uri=KGCL.see_also, domain=None, range=Optional[str])
+
+slots.creator = Slot(uri=DCTERMS.creator, name="creator", curie=DCTERMS.curie('creator'),
+                   model_uri=KGCL.creator, domain=None, range=Optional[str])
+
+slots.contributor = Slot(uri=DCTERMS.creator, name="contributor", curie=DCTERMS.curie('creator'),
+                   model_uri=KGCL.contributor, domain=None, range=Optional[str])
+
+slots.change_date = Slot(uri=DCTERMS.date, name="change_date", curie=DCTERMS.curie('date'),
+                   model_uri=KGCL.change_date, domain=None, range=Optional[str])
+
+slots.has_undo = Slot(uri=KGCL.has_undo, name="has_undo", curie=KGCL.curie('has_undo'),
+                   model_uri=KGCL.has_undo, domain=Change, range=Optional[Union[str, ChangeId]])
+
+slots.node_id = Slot(uri=KGCL.node_id, name="node_id", curie=KGCL.curie('node_id'),
+                   model_uri=KGCL.node_id, domain=None, range=Optional[Union[str, NodeId]])
+
+slots.superclass = Slot(uri=KGCL.superclass, name="superclass", curie=KGCL.curie('superclass'),
+                   model_uri=KGCL.superclass, domain=None, range=Optional[Union[str, NodeId]])
+
+slots.language = Slot(uri=KGCL.language, name="language", curie=KGCL.curie('language'),
+                   model_uri=KGCL.language, domain=None, range=Optional[str])
+
+slots.about = Slot(uri=KGCL.about, name="about", curie=KGCL.curie('about'),
+                   model_uri=KGCL.about, domain=None, range=Optional[Union[dict, OntologyElement]])
+
+slots.about_node = Slot(uri=KGCL.about_node, name="about_node", curie=KGCL.curie('about_node'),
+                   model_uri=KGCL.about_node, domain=None, range=Optional[Union[str, NodeId]])
+
+slots.about_edge = Slot(uri=KGCL.about_edge, name="about_edge", curie=KGCL.curie('about_edge'),
+                   model_uri=KGCL.about_edge, domain=None, range=Optional[Union[dict, Edge]])
+
+slots.about_node_representation = Slot(uri=KGCL.about_node_representation, name="about_node_representation", curie=KGCL.curie('about_node_representation'),
+                   model_uri=KGCL.about_node_representation, domain=None, range=Optional[str])
+
+slots.target = Slot(uri=KGCL.target, name="target", curie=KGCL.curie('target'),
+                   model_uri=KGCL.target, domain=None, range=Optional[str])
+
+slots.old_value = Slot(uri=KGCL.old_value, name="old_value", curie=KGCL.curie('old_value'),
+                   model_uri=KGCL.old_value, domain=None, range=Optional[str])
+
+slots.new_value = Slot(uri=KGCL.new_value, name="new_value", curie=KGCL.curie('new_value'),
+                   model_uri=KGCL.new_value, domain=None, range=Optional[str])
+
+slots.datatype = Slot(uri=KGCL.datatype, name="datatype", curie=KGCL.curie('datatype'),
+                   model_uri=KGCL.datatype, domain=None, range=Optional[str])
+
+slots.new_datatype = Slot(uri=KGCL.new_datatype, name="new_datatype", curie=KGCL.curie('new_datatype'),
+                   model_uri=KGCL.new_datatype, domain=None, range=Optional[str])
+
+slots.old_datatype = Slot(uri=KGCL.old_datatype, name="old_datatype", curie=KGCL.curie('old_datatype'),
+                   model_uri=KGCL.old_datatype, domain=None, range=Optional[str])
+
+slots.new_language = Slot(uri=KGCL.new_language, name="new_language", curie=KGCL.curie('new_language'),
+                   model_uri=KGCL.new_language, domain=None, range=Optional[str])
+
+slots.old_language = Slot(uri=KGCL.old_language, name="old_language", curie=KGCL.curie('old_language'),
+                   model_uri=KGCL.old_language, domain=None, range=Optional[str])
+
+slots.qualifier = Slot(uri=KGCL.qualifier, name="qualifier", curie=KGCL.curie('qualifier'),
+                   model_uri=KGCL.qualifier, domain=None, range=Optional[str])
+
+slots.subclass = Slot(uri=KGCL.subclass, name="subclass", curie=KGCL.curie('subclass'),
+                   model_uri=KGCL.subclass, domain=None, range=Optional[str])
+
+slots.new_subclass = Slot(uri=KGCL.new_subclass, name="new_subclass", curie=KGCL.curie('new_subclass'),
+                   model_uri=KGCL.new_subclass, domain=None, range=Optional[str])
+
+slots.new_property = Slot(uri=KGCL.new_property, name="new_property", curie=KGCL.curie('new_property'),
+                   model_uri=KGCL.new_property, domain=None, range=Optional[str])
+
+slots.new_filler = Slot(uri=KGCL.new_filler, name="new_filler", curie=KGCL.curie('new_filler'),
+                   model_uri=KGCL.new_filler, domain=None, range=Optional[str])
+
+slots.object_type = Slot(uri=KGCL.object_type, name="object_type", curie=KGCL.curie('object_type'),
+                   model_uri=KGCL.object_type, domain=None, range=Optional[str])
+
+slots.new_object_type = Slot(uri=KGCL.new_object_type, name="new_object_type", curie=KGCL.curie('new_object_type'),
+                   model_uri=KGCL.new_object_type, domain=None, range=Optional[str])
+
+slots.old_object_type = Slot(uri=KGCL.old_object_type, name="old_object_type", curie=KGCL.curie('old_object_type'),
+                   model_uri=KGCL.old_object_type, domain=None, range=Optional[str])
+
+slots.new_value_type = Slot(uri=KGCL.new_value_type, name="new_value_type", curie=KGCL.curie('new_value_type'),
+                   model_uri=KGCL.new_value_type, domain=None, range=Optional[str])
+
+slots.old_value_type = Slot(uri=KGCL.old_value_type, name="old_value_type", curie=KGCL.curie('old_value_type'),
+                   model_uri=KGCL.old_value_type, domain=None, range=Optional[str])
+
+slots.subject_type = Slot(uri=KGCL.subject_type, name="subject_type", curie=KGCL.curie('subject_type'),
+                   model_uri=KGCL.subject_type, domain=None, range=Optional[str])
+
+slots.subclass_type = Slot(uri=KGCL.subclass_type, name="subclass_type", curie=KGCL.curie('subclass_type'),
+                   model_uri=KGCL.subclass_type, domain=None, range=Optional[str])
+
+slots.superclass_type = Slot(uri=KGCL.superclass_type, name="superclass_type", curie=KGCL.curie('superclass_type'),
+                   model_uri=KGCL.superclass_type, domain=None, range=Optional[str])
+
+slots.predicate_type = Slot(uri=KGCL.predicate_type, name="predicate_type", curie=KGCL.curie('predicate_type'),
+                   model_uri=KGCL.predicate_type, domain=None, range=Optional[str])
+
+slots.in_subset = Slot(uri=KGCL.in_subset, name="in_subset", curie=KGCL.curie('in_subset'),
+                   model_uri=KGCL.in_subset, domain=None, range=Optional[Union[dict, OntologySubset]])
+
+slots.annotation_property = Slot(uri=KGCL.annotation_property, name="annotation_property", curie=KGCL.curie('annotation_property'),
+                   model_uri=KGCL.annotation_property, domain=None, range=Optional[str])
+
+slots.annotation_property_type = Slot(uri=KGCL.annotation_property_type, name="annotation_property_type", curie=KGCL.curie('annotation_property_type'),
+                   model_uri=KGCL.annotation_property_type, domain=None, range=Optional[str])
+
+slots.change_description = Slot(uri=KGCL.change_description, name="change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.change_description, domain=None, range=Optional[str])
+
+slots.has_textual_diff = Slot(uri=KGCL.has_textual_diff, name="has_textual_diff", curie=KGCL.curie('has_textual_diff'),
+                   model_uri=KGCL.has_textual_diff, domain=Change, range=Optional[Union[dict, "TextualDiff"]])
+
+slots.change_set = Slot(uri=KGCL.change_set, name="change_set", curie=KGCL.curie('change_set'),
+                   model_uri=KGCL.change_set, domain=None, range=Optional[Union[Dict[Union[str, ChangeId], Union[dict, Change]], List[Union[dict, Change]]]])
+
+slots.has_replacement = Slot(uri=KGCL.has_replacement, name="has_replacement", curie=KGCL.curie('has_replacement'),
+                   model_uri=KGCL.has_replacement, domain=NodeObsoletion, range=Optional[Union[str, NodeId]])
+
+slots.has_direct_replacement = Slot(uri=KGCL.has_direct_replacement, name="has_direct_replacement", curie=KGCL.curie('has_direct_replacement'),
+                   model_uri=KGCL.has_direct_replacement, domain=None, range=Optional[Union[str, NodeId]])
+
+slots.has_nondirect_replacement = Slot(uri=KGCL.has_nondirect_replacement, name="has_nondirect_replacement", curie=KGCL.curie('has_nondirect_replacement'),
+                   model_uri=KGCL.has_nondirect_replacement, domain=None, range=Optional[Union[Union[str, NodeId], List[Union[str, NodeId]]]])
+
+slots.owl_type = Slot(uri=OM.owl_type, name="owl_type", curie=OM.curie('owl_type'),
+                   model_uri=KGCL.owl_type, domain=None, range=Optional[Union[str, "OwlTypeEnum"]])
+
+slots.name = Slot(uri=OM.name, name="name", curie=OM.curie('name'),
+                   model_uri=KGCL.name, domain=None, range=Optional[str])
+
+slots.subject = Slot(uri=OM.subject, name="subject", curie=OM.curie('subject'),
+                   model_uri=KGCL.subject, domain=None, range=Optional[Union[str, NodeId]])
+
+slots.object = Slot(uri=OM.object, name="object", curie=OM.curie('object'),
+                   model_uri=KGCL.object, domain=None, range=Optional[Union[str, NodeId]])
+
+slots.predicate = Slot(uri=OM.predicate, name="predicate", curie=OM.curie('predicate'),
+                   model_uri=KGCL.predicate, domain=None, range=Optional[Union[str, NodeId]])
+
+slots.annotation_set = Slot(uri=OM.annotation_set, name="annotation_set", curie=OM.curie('annotation_set'),
+                   model_uri=KGCL.annotation_set, domain=None, range=Optional[Union[dict, Annotation]])
+
+slots.property = Slot(uri=OM.property, name="property", curie=OM.curie('property'),
+                   model_uri=KGCL.property, domain=None, range=Optional[Union[str, NodeId]])
+
+slots.filler = Slot(uri=OM.filler, name="filler", curie=OM.curie('filler'),
+                   model_uri=KGCL.filler, domain=None, range=Optional[str])
+
+slots.property_type = Slot(uri=OM.property_type, name="property_type", curie=OM.curie('property_type'),
+                   model_uri=KGCL.property_type, domain=None, range=Optional[str])
+
+slots.filler_type = Slot(uri=OM.filler_type, name="filler_type", curie=OM.curie('filler_type'),
+                   model_uri=KGCL.filler_type, domain=None, range=Optional[str])
+
+slots.subject_representation = Slot(uri=OM.subject_representation, name="subject_representation", curie=OM.curie('subject_representation'),
+                   model_uri=KGCL.subject_representation, domain=None, range=Optional[str])
+
+slots.predicate_representation = Slot(uri=OM.predicate_representation, name="predicate_representation", curie=OM.curie('predicate_representation'),
+                   model_uri=KGCL.predicate_representation, domain=None, range=Optional[str])
+
+slots.object_representation = Slot(uri=OM.object_representation, name="object_representation", curie=OM.curie('object_representation'),
+                   model_uri=KGCL.object_representation, domain=None, range=Optional[str])
+
+slots.property_value_set = Slot(uri=OM.property_value_set, name="property_value_set", curie=OM.curie('property_value_set'),
+                   model_uri=KGCL.property_value_set, domain=None, range=Optional[Union[Union[dict, PropertyValue], List[Union[dict, PropertyValue]]]])
+
+slots.started_at_time = Slot(uri=PROV.startedAtTime, name="started_at_time", curie=PROV.curie('startedAtTime'),
+                   model_uri=KGCL.started_at_time, domain=None, range=Optional[str])
+
+slots.ended_at_time = Slot(uri=PROV.endedAtTime, name="ended_at_time", curie=PROV.curie('endedAtTime'),
+                   model_uri=KGCL.ended_at_time, domain=None, range=Optional[str])
+
+slots.was_informed_by = Slot(uri=PROV.wasInformedBy, name="was_informed_by", curie=PROV.curie('wasInformedBy'),
+                   model_uri=KGCL.was_informed_by, domain=None, range=Optional[Union[str, ActivityId]])
+
+slots.was_associated_with = Slot(uri=PROV.wasAssociatedWith, name="was_associated_with", curie=PROV.curie('wasAssociatedWith'),
+                   model_uri=KGCL.was_associated_with, domain=None, range=Optional[Union[str, AgentId]])
+
+slots.acted_on_behalf_of = Slot(uri=PROV.actedOnBehalfOf, name="acted_on_behalf_of", curie=PROV.curie('actedOnBehalfOf'),
+                   model_uri=KGCL.acted_on_behalf_of, domain=None, range=Optional[Union[str, AgentId]])
+
+slots.was_generated_by = Slot(uri=PROV.wasGeneratedBy, name="was_generated_by", curie=PROV.curie('wasGeneratedBy'),
+                   model_uri=KGCL.was_generated_by, domain=None, range=Optional[Union[str, ActivityId]])
+
+slots.used = Slot(uri=PROV.used, name="used", curie=PROV.curie('used'),
+                   model_uri=KGCL.used, domain=Activity, range=Optional[str])
+
+slots.activity_set = Slot(uri=PROV.activity_set, name="activity_set", curie=PROV.curie('activity_set'),
+                   model_uri=KGCL.activity_set, domain=None, range=Optional[Union[Dict[Union[str, ActivityId], Union[dict, Activity]], List[Union[dict, Activity]]]])
+
+slots.agent_set = Slot(uri=PROV.agent_set, name="agent_set", curie=PROV.curie('agent_set'),
+                   model_uri=KGCL.agent_set, domain=None, range=Optional[Union[Dict[Union[str, AgentId], Union[dict, Agent]], List[Union[dict, Agent]]]])
+
+slots.id = Slot(uri=BASICS.id, name="id", curie=BASICS.curie('id'),
+                   model_uri=KGCL.id, domain=None, range=URIRef)
+
+slots.description = Slot(uri=DCTERMS.description, name="description", curie=DCTERMS.curie('description'),
+                   model_uri=KGCL.description, domain=None, range=Optional[str])
+
+slots.configuration__name_predicate = Slot(uri=KGCL.name_predicate, name="configuration__name_predicate", curie=KGCL.curie('name_predicate'),
+                   model_uri=KGCL.configuration__name_predicate, domain=None, range=Optional[str])
+
+slots.configuration__definition_predicate = Slot(uri=KGCL.definition_predicate, name="configuration__definition_predicate", curie=KGCL.curie('definition_predicate'),
+                   model_uri=KGCL.configuration__definition_predicate, domain=None, range=Optional[str])
+
+slots.configuration__main_synonym_predicate = Slot(uri=KGCL.main_synonym_predicate, name="configuration__main_synonym_predicate", curie=KGCL.curie('main_synonym_predicate'),
+                   model_uri=KGCL.configuration__main_synonym_predicate, domain=None, range=Optional[str])
+
+slots.configuration__synonym_predicates = Slot(uri=KGCL.synonym_predicates, name="configuration__synonym_predicates", curie=KGCL.curie('synonym_predicates'),
+                   model_uri=KGCL.configuration__synonym_predicates, domain=None, range=Optional[str])
+
+slots.configuration__creator_predicate = Slot(uri=KGCL.creator_predicate, name="configuration__creator_predicate", curie=KGCL.curie('creator_predicate'),
+                   model_uri=KGCL.configuration__creator_predicate, domain=None, range=Optional[str])
+
+slots.configuration__contributor_predicate = Slot(uri=KGCL.contributor_predicate, name="configuration__contributor_predicate", curie=KGCL.curie('contributor_predicate'),
+                   model_uri=KGCL.configuration__contributor_predicate, domain=None, range=Optional[str])
+
+slots.configuration__obsolete_node_label_prefix = Slot(uri=KGCL.obsolete_node_label_prefix, name="configuration__obsolete_node_label_prefix", curie=KGCL.curie('obsolete_node_label_prefix'),
+                   model_uri=KGCL.configuration__obsolete_node_label_prefix, domain=None, range=Optional[str])
+
+slots.configuration__obsoletion_workflow = Slot(uri=KGCL.obsoletion_workflow, name="configuration__obsoletion_workflow", curie=KGCL.curie('obsoletion_workflow'),
+                   model_uri=KGCL.configuration__obsoletion_workflow, domain=None, range=Optional[str])
+
+slots.configuration__obsoletion_policies = Slot(uri=KGCL.obsoletion_policies, name="configuration__obsoletion_policies", curie=KGCL.curie('obsoletion_policies'),
+                   model_uri=KGCL.configuration__obsoletion_policies, domain=None, range=Optional[Union[Union[str, "ObsoletionPolicyEnum"], List[Union[str, "ObsoletionPolicyEnum"]]]])
+
+slots.configuration__obsolete_subclass_of_shadow_property = Slot(uri=KGCL.obsolete_subclass_of_shadow_property, name="configuration__obsolete_subclass_of_shadow_property", curie=KGCL.curie('obsolete_subclass_of_shadow_property'),
+                   model_uri=KGCL.configuration__obsolete_subclass_of_shadow_property, domain=None, range=Optional[Union[str, URIorCURIE]])
+
+slots.term_tracker_issue = Slot(uri=KGCL.term_tracker_issue, name="term_tracker_issue", curie=KGCL.curie('term_tracker_issue'),
+                   model_uri=KGCL.term_tracker_issue, domain=None, range=Optional[str])
+
+slots.associated_change_set = Slot(uri=KGCL.associated_change_set, name="associated change set", curie=KGCL.curie('associated_change_set'),
+                   model_uri=KGCL.associated_change_set, domain=None, range=Optional[Union[Dict[Union[str, ChangeId], Union[dict, Change]], List[Union[dict, Change]]]])
+
+slots.change_type = Slot(uri=KGCL.change_type, name="change type", curie=KGCL.curie('change_type'),
+                   model_uri=KGCL.change_type, domain=None, range=Optional[Union[str, ChangeClassType]])
+
+slots.count = Slot(uri=KGCL.count, name="count", curie=KGCL.curie('count'),
+                   model_uri=KGCL.count, domain=None, range=Optional[int])
+
+slots.change_1 = Slot(uri=KGCL.change_1, name="change 1", curie=KGCL.curie('change_1'),
+                   model_uri=KGCL.change_1, domain=None, range=Optional[Union[str, NodeRenameId]])
+
+slots.change_2 = Slot(uri=KGCL.change_2, name="change 2", curie=KGCL.curie('change_2'),
+                   model_uri=KGCL.change_2, domain=None, range=Optional[Union[str, NewSynonymId]])
+
+slots.subset = Slot(uri=KGCL.subset, name="subset", curie=KGCL.curie('subset'),
+                   model_uri=KGCL.subset, domain=None, range=Optional[str])
+
+slots.replaced_by = Slot(uri=KGCL.replaced_by, name="replaced by", curie=KGCL.curie('replaced_by'),
+                   model_uri=KGCL.replaced_by, domain=None, range=Optional[Union[str, NodeId]])
+
+slots.consider = Slot(uri=KGCL.consider, name="consider", curie=KGCL.curie('consider'),
+                   model_uri=KGCL.consider, domain=None, range=Optional[Union[str, NodeId]])
+
+slots.Change_was_generated_by = Slot(uri=PROV.wasGeneratedBy, name="Change_was_generated_by", curie=PROV.curie('wasGeneratedBy'),
+                   model_uri=KGCL.Change_was_generated_by, domain=Change, range=Optional[Union[str, ActivityId]])
+
+slots.Change_see_also = Slot(uri=RDFS.seeAlso, name="Change_see_also", curie=RDFS.curie('seeAlso'),
+                   model_uri=KGCL.Change_see_also, domain=Change, range=Optional[str])
+
+slots.Change_pull_request = Slot(uri=KGCL.pull_request, name="Change_pull_request", curie=KGCL.curie('pull_request'),
+                   model_uri=KGCL.Change_pull_request, domain=Change, range=Optional[str])
+
+slots.Change_term_tracker_issue = Slot(uri=KGCL.term_tracker_issue, name="Change_term_tracker_issue", curie=KGCL.curie('term_tracker_issue'),
+                   model_uri=KGCL.Change_term_tracker_issue, domain=Change, range=Optional[str])
+
+slots.Change_creator = Slot(uri=DCTERMS.creator, name="Change_creator", curie=DCTERMS.curie('creator'),
+                   model_uri=KGCL.Change_creator, domain=Change, range=Optional[str])
+
+slots.Change_change_date = Slot(uri=DCTERMS.date, name="Change_change_date", curie=DCTERMS.curie('date'),
+                   model_uri=KGCL.Change_change_date, domain=Change, range=Optional[str])
+
+slots.MultiNodeObsoletion_change_set = Slot(uri=KGCL.change_set, name="MultiNodeObsoletion_change_set", curie=KGCL.curie('change_set'),
+                   model_uri=KGCL.MultiNodeObsoletion_change_set, domain=MultiNodeObsoletion, range=Optional[Union[Dict[Union[str, NodeObsoletionId], Union[dict, "NodeObsoletion"]], List[Union[dict, "NodeObsoletion"]]]])
+
+slots.MultiNodeObsoletion_change_description = Slot(uri=KGCL.change_description, name="MultiNodeObsoletion_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.MultiNodeObsoletion_change_description, domain=MultiNodeObsoletion, range=Optional[str])
+
+slots.MultiNodeObsoletion_associated_change_set = Slot(uri=KGCL.associated_change_set, name="MultiNodeObsoletion_associated change set", curie=KGCL.curie('associated_change_set'),
+                   model_uri=KGCL.MultiNodeObsoletion_associated_change_set, domain=MultiNodeObsoletion, range=Optional[Union[Dict[Union[str, ChangeId], Union[dict, Change]], List[Union[dict, Change]]]])
+
+slots.ChangeSetSummaryStatistic_change_type = Slot(uri=KGCL.change_type, name="ChangeSetSummaryStatistic_change type", curie=KGCL.curie('change_type'),
+                   model_uri=KGCL.ChangeSetSummaryStatistic_change_type, domain=ChangeSetSummaryStatistic, range=Optional[Union[str, ChangeClassType]])
+
+slots.ChangeSetSummaryStatistic_count = Slot(uri=KGCL.count, name="ChangeSetSummaryStatistic_count", curie=KGCL.curie('count'),
+                   model_uri=KGCL.ChangeSetSummaryStatistic_count, domain=ChangeSetSummaryStatistic, range=Optional[int])
+
+slots.ChangeSetSummaryStatistic_property_value_set = Slot(uri=OM.property_value_set, name="ChangeSetSummaryStatistic_property_value_set", curie=OM.curie('property_value_set'),
+                   model_uri=KGCL.ChangeSetSummaryStatistic_property_value_set, domain=ChangeSetSummaryStatistic, range=Optional[Union[Union[dict, "PropertyValue"], List[Union[dict, "PropertyValue"]]]])
+
+slots.Obsoletion_about = Slot(uri=KGCL.about, name="Obsoletion_about", curie=KGCL.curie('about'),
+                   model_uri=KGCL.Obsoletion_about, domain=None, range=Optional[Union[dict, "OntologyElement"]])
+
+slots.Obsoletion_has_undo = Slot(uri=KGCL.has_undo, name="Obsoletion_has_undo", curie=KGCL.curie('has_undo'),
+                   model_uri=KGCL.Obsoletion_has_undo, domain=None, range=Optional[Union[dict, "Obsoletion"]])
+
+slots.LanguageTagChange_old_value = Slot(uri=KGCL.old_value, name="LanguageTagChange_old_value", curie=KGCL.curie('old_value'),
+                   model_uri=KGCL.LanguageTagChange_old_value, domain=LanguageTagChange, range=Optional[str])
+
+slots.LanguageTagChange_new_value = Slot(uri=KGCL.new_value, name="LanguageTagChange_new_value", curie=KGCL.curie('new_value'),
+                   model_uri=KGCL.LanguageTagChange_new_value, domain=LanguageTagChange, range=Optional[str])
+
+slots.Unobsoletion_has_undo = Slot(uri=KGCL.has_undo, name="Unobsoletion_has_undo", curie=KGCL.curie('has_undo'),
+                   model_uri=KGCL.Unobsoletion_has_undo, domain=None, range=Optional[Union[dict, Obsoletion]])
+
+slots.Creation_has_undo = Slot(uri=KGCL.has_undo, name="Creation_has_undo", curie=KGCL.curie('has_undo'),
+                   model_uri=KGCL.Creation_has_undo, domain=None, range=Optional[Union[dict, Deletion]])
+
+slots.AddToSubset_in_subset = Slot(uri=KGCL.in_subset, name="AddToSubset_in_subset", curie=KGCL.curie('in_subset'),
+                   model_uri=KGCL.AddToSubset_in_subset, domain=None, range=Optional[Union[dict, "OntologySubset"]])
+
+slots.RemoveFromSubset_in_subset = Slot(uri=KGCL.in_subset, name="RemoveFromSubset_in_subset", curie=KGCL.curie('in_subset'),
+                   model_uri=KGCL.RemoveFromSubset_in_subset, domain=None, range=Optional[Union[dict, "OntologySubset"]])
+
+slots.RemoveFromSubset_has_undo = Slot(uri=KGCL.has_undo, name="RemoveFromSubset_has_undo", curie=KGCL.curie('has_undo'),
+                   model_uri=KGCL.RemoveFromSubset_has_undo, domain=None, range=Optional[Union[dict, AddToSubset]])
+
+slots.EdgeChange_subject = Slot(uri=OM.subject, name="EdgeChange_subject", curie=OM.curie('subject'),
+                   model_uri=KGCL.EdgeChange_subject, domain=EdgeChange, range=Optional[Union[str, NodeId]])
+
+slots.EdgeCreation_change_description = Slot(uri=KGCL.change_description, name="EdgeCreation_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.EdgeCreation_change_description, domain=EdgeCreation, range=Optional[str])
+
+slots.EdgeDeletion_change_description = Slot(uri=KGCL.change_description, name="EdgeDeletion_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.EdgeDeletion_change_description, domain=EdgeDeletion, range=Optional[str])
+
+slots.EdgeObsoletion_change_description = Slot(uri=KGCL.change_description, name="EdgeObsoletion_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.EdgeObsoletion_change_description, domain=EdgeObsoletion, range=Optional[str])
+
+slots.MappingCreation_change_description = Slot(uri=KGCL.change_description, name="MappingCreation_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.MappingCreation_change_description, domain=MappingCreation, range=Optional[str])
+
+slots.MappingCreation_subject = Slot(uri=OM.subject, name="MappingCreation_subject", curie=OM.curie('subject'),
+                   model_uri=KGCL.MappingCreation_subject, domain=MappingCreation, range=Optional[Union[str, NodeId]])
+
+slots.MappingCreation_predicate = Slot(uri=OM.predicate, name="MappingCreation_predicate", curie=OM.curie('predicate'),
+                   model_uri=KGCL.MappingCreation_predicate, domain=MappingCreation, range=Optional[Union[str, NodeId]])
+
+slots.MappingCreation_object = Slot(uri=OM.object, name="MappingCreation_object", curie=OM.curie('object'),
+                   model_uri=KGCL.MappingCreation_object, domain=MappingCreation, range=Optional[Union[str, NodeId]])
+
+slots.NodeMove_change_description = Slot(uri=KGCL.change_description, name="NodeMove_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.NodeMove_change_description, domain=NodeMove, range=Optional[str])
+
+slots.NodeDeepening_change_description = Slot(uri=KGCL.change_description, name="NodeDeepening_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.NodeDeepening_change_description, domain=NodeDeepening, range=Optional[str])
+
+slots.NodeShallowing_change_description = Slot(uri=KGCL.change_description, name="NodeShallowing_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.NodeShallowing_change_description, domain=NodeShallowing, range=Optional[str])
+
+slots.PredicateChange_change_description = Slot(uri=KGCL.change_description, name="PredicateChange_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.PredicateChange_change_description, domain=PredicateChange, range=Optional[str])
+
+slots.NodeRename_old_value = Slot(uri=KGCL.old_value, name="NodeRename_old_value", curie=KGCL.curie('old_value'),
+                   model_uri=KGCL.NodeRename_old_value, domain=NodeRename, range=Optional[str])
+
+slots.NodeRename_new_value = Slot(uri=KGCL.new_value, name="NodeRename_new_value", curie=KGCL.curie('new_value'),
+                   model_uri=KGCL.NodeRename_new_value, domain=NodeRename, range=Optional[str])
+
+slots.NodeRename_change_description = Slot(uri=KGCL.change_description, name="NodeRename_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.NodeRename_change_description, domain=NodeRename, range=Optional[str])
+
+slots.SetLanguageForName_change_description = Slot(uri=KGCL.change_description, name="SetLanguageForName_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.SetLanguageForName_change_description, domain=SetLanguageForName, range=Optional[str])
+
+slots.NameBecomesSynonym_change_1 = Slot(uri=KGCL.change_1, name="NameBecomesSynonym_change 1", curie=KGCL.curie('change_1'),
+                   model_uri=KGCL.NameBecomesSynonym_change_1, domain=NameBecomesSynonym, range=Optional[Union[str, NodeRenameId]])
+
+slots.NameBecomesSynonym_change_2 = Slot(uri=KGCL.change_2, name="NameBecomesSynonym_change 2", curie=KGCL.curie('change_2'),
+                   model_uri=KGCL.NameBecomesSynonym_change_2, domain=NameBecomesSynonym, range=Optional[Union[str, NewSynonymId]])
+
+slots.NameBecomesSynonym_change_description = Slot(uri=KGCL.change_description, name="NameBecomesSynonym_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.NameBecomesSynonym_change_description, domain=NameBecomesSynonym, range=Optional[str])
+
+slots.RemoveNodeFromSubset_change_description = Slot(uri=KGCL.change_description, name="RemoveNodeFromSubset_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.RemoveNodeFromSubset_change_description, domain=RemoveNodeFromSubset, range=Optional[str])
+
+slots.RemoveNodeFromSubset_about_node = Slot(uri=KGCL.about_node, name="RemoveNodeFromSubset_about_node", curie=KGCL.curie('about_node'),
+                   model_uri=KGCL.RemoveNodeFromSubset_about_node, domain=RemoveNodeFromSubset, range=Optional[Union[str, NodeId]])
+
+slots.RemoveNodeFromSubset_subset = Slot(uri=KGCL.subset, name="RemoveNodeFromSubset_subset", curie=KGCL.curie('subset'),
+                   model_uri=KGCL.RemoveNodeFromSubset_subset, domain=RemoveNodeFromSubset, range=Optional[str])
+
+slots.NodeObsoletion_change_description = Slot(uri=KGCL.change_description, name="NodeObsoletion_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.NodeObsoletion_change_description, domain=NodeObsoletion, range=Optional[str])
+
+slots.NodeObsoletion_associated_change_set = Slot(uri=KGCL.associated_change_set, name="NodeObsoletion_associated change set", curie=KGCL.curie('associated_change_set'),
+                   model_uri=KGCL.NodeObsoletion_associated_change_set, domain=NodeObsoletion, range=Optional[Union[Dict[Union[str, ChangeId], Union[dict, Change]], List[Union[dict, Change]]]])
+
+slots.NodeUnobsoletion_change_description = Slot(uri=KGCL.change_description, name="NodeUnobsoletion_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.NodeUnobsoletion_change_description, domain=NodeUnobsoletion, range=Optional[str])
+
+slots.NodeUnobsoletion_replaced_by = Slot(uri=KGCL.replaced_by, name="NodeUnobsoletion_replaced by", curie=KGCL.curie('replaced_by'),
+                   model_uri=KGCL.NodeUnobsoletion_replaced_by, domain=NodeUnobsoletion, range=Optional[Union[str, NodeId]])
+
+slots.NodeUnobsoletion_consider = Slot(uri=KGCL.consider, name="NodeUnobsoletion_consider", curie=KGCL.curie('consider'),
+                   model_uri=KGCL.NodeUnobsoletion_consider, domain=NodeUnobsoletion, range=Optional[Union[str, NodeId]])
+
+slots.NodeCreation_change_description = Slot(uri=KGCL.change_description, name="NodeCreation_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.NodeCreation_change_description, domain=NodeCreation, range=Optional[str])
+
+slots.ClassCreation_change_description = Slot(uri=KGCL.change_description, name="ClassCreation_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.ClassCreation_change_description, domain=ClassCreation, range=Optional[str])
+
+slots.ObjectPropertyCreation_change_description = Slot(uri=KGCL.change_description, name="ObjectPropertyCreation_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.ObjectPropertyCreation_change_description, domain=ObjectPropertyCreation, range=Optional[str])
+
+slots.NodeDeletion_change_description = Slot(uri=KGCL.change_description, name="NodeDeletion_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.NodeDeletion_change_description, domain=NodeDeletion, range=Optional[str])
+
+slots.NodeDirectMerge_has_direct_replacement = Slot(uri=KGCL.has_direct_replacement, name="NodeDirectMerge_has_direct_replacement", curie=KGCL.curie('has_direct_replacement'),
+                   model_uri=KGCL.NodeDirectMerge_has_direct_replacement, domain=NodeDirectMerge, range=Union[str, NodeId])
+
+slots.NodeDirectMerge_about_node = Slot(uri=KGCL.about_node, name="NodeDirectMerge_about_node", curie=KGCL.curie('about_node'),
+                   model_uri=KGCL.NodeDirectMerge_about_node, domain=NodeDirectMerge, range=Optional[Union[str, NodeId]])
+
+slots.NodeDirectMerge_change_description = Slot(uri=KGCL.change_description, name="NodeDirectMerge_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.NodeDirectMerge_change_description, domain=NodeDirectMerge, range=Optional[str])
+
+slots.NodeObsoletionWithDirectReplacement_has_direct_replacement = Slot(uri=KGCL.has_direct_replacement, name="NodeObsoletionWithDirectReplacement_has_direct_replacement", curie=KGCL.curie('has_direct_replacement'),
+                   model_uri=KGCL.NodeObsoletionWithDirectReplacement_has_direct_replacement, domain=NodeObsoletionWithDirectReplacement, range=Union[str, NodeId])
+
+slots.NodeObsoletionWithDirectReplacement_change_description = Slot(uri=KGCL.change_description, name="NodeObsoletionWithDirectReplacement_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.NodeObsoletionWithDirectReplacement_change_description, domain=NodeObsoletionWithDirectReplacement, range=Optional[str])
+
+slots.NodeObsoletionWithNoDirectReplacement_has_nondirect_replacement = Slot(uri=KGCL.has_nondirect_replacement, name="NodeObsoletionWithNoDirectReplacement_has_nondirect_replacement", curie=KGCL.curie('has_nondirect_replacement'),
+                   model_uri=KGCL.NodeObsoletionWithNoDirectReplacement_has_nondirect_replacement, domain=NodeObsoletionWithNoDirectReplacement, range=Union[Union[str, NodeId], List[Union[str, NodeId]]])
 
-slots.type = Slot(
-    uri=RDF.type,
-    name="type",
-    curie=RDF.curie("type"),
-    model_uri=KGCL.type,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.pull_request = Slot(
-    uri=KGCL.pull_request,
-    name="pull request",
-    curie=KGCL.curie("pull_request"),
-    model_uri=KGCL.pull_request,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.see_also = Slot(
-    uri=RDFS.seeAlso,
-    name="see also",
-    curie=RDFS.curie("seeAlso"),
-    model_uri=KGCL.see_also,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.creator = Slot(
-    uri=DCTERMS.creator,
-    name="creator",
-    curie=DCTERMS.curie("creator"),
-    model_uri=KGCL.creator,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.contributor = Slot(
-    uri=DCTERMS.creator,
-    name="contributor",
-    curie=DCTERMS.curie("creator"),
-    model_uri=KGCL.contributor,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.change_date = Slot(
-    uri=DCTERMS.date,
-    name="change date",
-    curie=DCTERMS.curie("date"),
-    model_uri=KGCL.change_date,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.has_undo = Slot(
-    uri=KGCL.has_undo,
-    name="has undo",
-    curie=KGCL.curie("has_undo"),
-    model_uri=KGCL.has_undo,
-    domain=Change,
-    range=Optional[Union[str, ChangeId]],
-)
-
-slots.node_id = Slot(
-    uri=KGCL.node_id,
-    name="node id",
-    curie=KGCL.curie("node_id"),
-    model_uri=KGCL.node_id,
-    domain=None,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.superclass = Slot(
-    uri=KGCL.superclass,
-    name="superclass",
-    curie=KGCL.curie("superclass"),
-    model_uri=KGCL.superclass,
-    domain=None,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.language = Slot(
-    uri=KGCL.language,
-    name="language",
-    curie=KGCL.curie("language"),
-    model_uri=KGCL.language,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.about = Slot(
-    uri=KGCL.about,
-    name="about",
-    curie=KGCL.curie("about"),
-    model_uri=KGCL.about,
-    domain=None,
-    range=Optional[Union[dict, OntologyElement]],
-)
-
-slots.about_node = Slot(
-    uri=KGCL.about_node,
-    name="about node",
-    curie=KGCL.curie("about_node"),
-    model_uri=KGCL.about_node,
-    domain=None,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.about_edge = Slot(
-    uri=KGCL.about_edge,
-    name="about edge",
-    curie=KGCL.curie("about_edge"),
-    model_uri=KGCL.about_edge,
-    domain=None,
-    range=Optional[Union[dict, Edge]],
-)
-
-slots.about_node_representation = Slot(
-    uri=KGCL.about_node_representation,
-    name="about node representation",
-    curie=KGCL.curie("about_node_representation"),
-    model_uri=KGCL.about_node_representation,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.target = Slot(
-    uri=KGCL.target,
-    name="target",
-    curie=KGCL.curie("target"),
-    model_uri=KGCL.target,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.old_value = Slot(
-    uri=KGCL.old_value,
-    name="old value",
-    curie=KGCL.curie("old_value"),
-    model_uri=KGCL.old_value,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.new_value = Slot(
-    uri=KGCL.new_value,
-    name="new value",
-    curie=KGCL.curie("new_value"),
-    model_uri=KGCL.new_value,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.datatype = Slot(
-    uri=KGCL.datatype,
-    name="datatype",
-    curie=KGCL.curie("datatype"),
-    model_uri=KGCL.datatype,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.new_datatype = Slot(
-    uri=KGCL.new_datatype,
-    name="new datatype",
-    curie=KGCL.curie("new_datatype"),
-    model_uri=KGCL.new_datatype,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.old_datatype = Slot(
-    uri=KGCL.old_datatype,
-    name="old datatype",
-    curie=KGCL.curie("old_datatype"),
-    model_uri=KGCL.old_datatype,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.new_language = Slot(
-    uri=KGCL.new_language,
-    name="new language",
-    curie=KGCL.curie("new_language"),
-    model_uri=KGCL.new_language,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.old_language = Slot(
-    uri=KGCL.old_language,
-    name="old language",
-    curie=KGCL.curie("old_language"),
-    model_uri=KGCL.old_language,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.qualifier = Slot(
-    uri=KGCL.qualifier,
-    name="qualifier",
-    curie=KGCL.curie("qualifier"),
-    model_uri=KGCL.qualifier,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.subclass = Slot(
-    uri=KGCL.subclass,
-    name="subclass",
-    curie=KGCL.curie("subclass"),
-    model_uri=KGCL.subclass,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.new_subclass = Slot(
-    uri=KGCL.new_subclass,
-    name="new subclass",
-    curie=KGCL.curie("new_subclass"),
-    model_uri=KGCL.new_subclass,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.new_property = Slot(
-    uri=KGCL.new_property,
-    name="new property",
-    curie=KGCL.curie("new_property"),
-    model_uri=KGCL.new_property,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.new_filler = Slot(
-    uri=KGCL.new_filler,
-    name="new filler",
-    curie=KGCL.curie("new_filler"),
-    model_uri=KGCL.new_filler,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.object_type = Slot(
-    uri=KGCL.object_type,
-    name="object type",
-    curie=KGCL.curie("object_type"),
-    model_uri=KGCL.object_type,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.new_object_type = Slot(
-    uri=KGCL.new_object_type,
-    name="new object type",
-    curie=KGCL.curie("new_object_type"),
-    model_uri=KGCL.new_object_type,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.old_object_type = Slot(
-    uri=KGCL.old_object_type,
-    name="old object type",
-    curie=KGCL.curie("old_object_type"),
-    model_uri=KGCL.old_object_type,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.new_value_type = Slot(
-    uri=KGCL.new_value_type,
-    name="new value type",
-    curie=KGCL.curie("new_value_type"),
-    model_uri=KGCL.new_value_type,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.old_value_type = Slot(
-    uri=KGCL.old_value_type,
-    name="old value type",
-    curie=KGCL.curie("old_value_type"),
-    model_uri=KGCL.old_value_type,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.subject_type = Slot(
-    uri=KGCL.subject_type,
-    name="subject type",
-    curie=KGCL.curie("subject_type"),
-    model_uri=KGCL.subject_type,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.subclass_type = Slot(
-    uri=KGCL.subclass_type,
-    name="subclass type",
-    curie=KGCL.curie("subclass_type"),
-    model_uri=KGCL.subclass_type,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.superclass_type = Slot(
-    uri=KGCL.superclass_type,
-    name="superclass type",
-    curie=KGCL.curie("superclass_type"),
-    model_uri=KGCL.superclass_type,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.predicate_type = Slot(
-    uri=KGCL.predicate_type,
-    name="predicate type",
-    curie=KGCL.curie("predicate_type"),
-    model_uri=KGCL.predicate_type,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.in_subset = Slot(
-    uri=KGCL.in_subset,
-    name="in subset",
-    curie=KGCL.curie("in_subset"),
-    model_uri=KGCL.in_subset,
-    domain=None,
-    range=Optional[Union[dict, OntologySubset]],
-)
-
-slots.annotation_property = Slot(
-    uri=KGCL.annotation_property,
-    name="annotation property",
-    curie=KGCL.curie("annotation_property"),
-    model_uri=KGCL.annotation_property,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.annotation_property_type = Slot(
-    uri=KGCL.annotation_property_type,
-    name="annotation property type",
-    curie=KGCL.curie("annotation_property_type"),
-    model_uri=KGCL.annotation_property_type,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.change_description = Slot(
-    uri=KGCL.change_description,
-    name="change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.change_description,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.has_textual_diff = Slot(
-    uri=KGCL.has_textual_diff,
-    name="has textual diff",
-    curie=KGCL.curie("has_textual_diff"),
-    model_uri=KGCL.has_textual_diff,
-    domain=Change,
-    range=Optional[Union[dict, "TextualDiff"]],
-)
-
-slots.change_set = Slot(
-    uri=KGCL.change_set,
-    name="change set",
-    curie=KGCL.curie("change_set"),
-    model_uri=KGCL.change_set,
-    domain=None,
-    range=Optional[
-        Union[
-            Dict[Union[str, ChangeId], Union[dict, Change]], List[Union[dict, Change]]
-        ]
-    ],
-)
-
-slots.has_replacement = Slot(
-    uri=KGCL.has_replacement,
-    name="has replacement",
-    curie=KGCL.curie("has_replacement"),
-    model_uri=KGCL.has_replacement,
-    domain=NodeObsoletion,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.has_direct_replacement = Slot(
-    uri=KGCL.has_direct_replacement,
-    name="has direct replacement",
-    curie=KGCL.curie("has_direct_replacement"),
-    model_uri=KGCL.has_direct_replacement,
-    domain=None,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.has_nondirect_replacement = Slot(
-    uri=KGCL.has_nondirect_replacement,
-    name="has nondirect replacement",
-    curie=KGCL.curie("has_nondirect_replacement"),
-    model_uri=KGCL.has_nondirect_replacement,
-    domain=None,
-    range=Optional[Union[Union[str, NodeId], List[Union[str, NodeId]]]],
-)
-
-slots.owl_type = Slot(
-    uri=OM.owl_type,
-    name="owl type",
-    curie=OM.curie("owl_type"),
-    model_uri=KGCL.owl_type,
-    domain=None,
-    range=Optional[Union[str, "OwlTypeEnum"]],
-)
-
-slots.name = Slot(
-    uri=OM.name,
-    name="name",
-    curie=OM.curie("name"),
-    model_uri=KGCL.name,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.subject = Slot(
-    uri=OM.subject,
-    name="subject",
-    curie=OM.curie("subject"),
-    model_uri=KGCL.subject,
-    domain=None,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.object = Slot(
-    uri=OM.object,
-    name="object",
-    curie=OM.curie("object"),
-    model_uri=KGCL.object,
-    domain=None,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.predicate = Slot(
-    uri=OM.predicate,
-    name="predicate",
-    curie=OM.curie("predicate"),
-    model_uri=KGCL.predicate,
-    domain=None,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.annotation_set = Slot(
-    uri=OM.annotation_set,
-    name="annotation set",
-    curie=OM.curie("annotation_set"),
-    model_uri=KGCL.annotation_set,
-    domain=None,
-    range=Optional[Union[dict, Annotation]],
-)
-
-slots.property = Slot(
-    uri=OM.property,
-    name="property",
-    curie=OM.curie("property"),
-    model_uri=KGCL.property,
-    domain=None,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.filler = Slot(
-    uri=OM.filler,
-    name="filler",
-    curie=OM.curie("filler"),
-    model_uri=KGCL.filler,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.property_type = Slot(
-    uri=OM.property_type,
-    name="property type",
-    curie=OM.curie("property_type"),
-    model_uri=KGCL.property_type,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.filler_type = Slot(
-    uri=OM.filler_type,
-    name="filler type",
-    curie=OM.curie("filler_type"),
-    model_uri=KGCL.filler_type,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.subject_representation = Slot(
-    uri=OM.subject_representation,
-    name="subject representation",
-    curie=OM.curie("subject_representation"),
-    model_uri=KGCL.subject_representation,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.predicate_representation = Slot(
-    uri=OM.predicate_representation,
-    name="predicate representation",
-    curie=OM.curie("predicate_representation"),
-    model_uri=KGCL.predicate_representation,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.object_representation = Slot(
-    uri=OM.object_representation,
-    name="object representation",
-    curie=OM.curie("object_representation"),
-    model_uri=KGCL.object_representation,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.property_value_set = Slot(
-    uri=OM.property_value_set,
-    name="property value set",
-    curie=OM.curie("property_value_set"),
-    model_uri=KGCL.property_value_set,
-    domain=None,
-    range=Optional[Union[Union[dict, PropertyValue], List[Union[dict, PropertyValue]]]],
-)
-
-slots.started_at_time = Slot(
-    uri=PROV.startedAtTime,
-    name="started at time",
-    curie=PROV.curie("startedAtTime"),
-    model_uri=KGCL.started_at_time,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.ended_at_time = Slot(
-    uri=PROV.endedAtTime,
-    name="ended at time",
-    curie=PROV.curie("endedAtTime"),
-    model_uri=KGCL.ended_at_time,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.was_informed_by = Slot(
-    uri=PROV.wasInformedBy,
-    name="was informed by",
-    curie=PROV.curie("wasInformedBy"),
-    model_uri=KGCL.was_informed_by,
-    domain=None,
-    range=Optional[Union[str, ActivityId]],
-)
-
-slots.was_associated_with = Slot(
-    uri=PROV.wasAssociatedWith,
-    name="was associated with",
-    curie=PROV.curie("wasAssociatedWith"),
-    model_uri=KGCL.was_associated_with,
-    domain=None,
-    range=Optional[Union[str, AgentId]],
-)
-
-slots.acted_on_behalf_of = Slot(
-    uri=PROV.actedOnBehalfOf,
-    name="acted on behalf of",
-    curie=PROV.curie("actedOnBehalfOf"),
-    model_uri=KGCL.acted_on_behalf_of,
-    domain=None,
-    range=Optional[Union[str, AgentId]],
-)
-
-slots.was_generated_by = Slot(
-    uri=PROV.wasGeneratedBy,
-    name="was generated by",
-    curie=PROV.curie("wasGeneratedBy"),
-    model_uri=KGCL.was_generated_by,
-    domain=None,
-    range=Optional[Union[str, ActivityId]],
-)
-
-slots.used = Slot(
-    uri=PROV.used,
-    name="used",
-    curie=PROV.curie("used"),
-    model_uri=KGCL.used,
-    domain=Activity,
-    range=Optional[str],
-)
-
-slots.activity_set = Slot(
-    uri=PROV.activity_set,
-    name="activity set",
-    curie=PROV.curie("activity_set"),
-    model_uri=KGCL.activity_set,
-    domain=None,
-    range=Optional[
-        Union[
-            Dict[Union[str, ActivityId], Union[dict, Activity]],
-            List[Union[dict, Activity]],
-        ]
-    ],
-)
-
-slots.agent_set = Slot(
-    uri=PROV.agent_set,
-    name="agent set",
-    curie=PROV.curie("agent_set"),
-    model_uri=KGCL.agent_set,
-    domain=None,
-    range=Optional[
-        Union[Dict[Union[str, AgentId], Union[dict, Agent]], List[Union[dict, Agent]]]
-    ],
-)
-
-slots.id = Slot(
-    uri=BASICS.id,
-    name="id",
-    curie=BASICS.curie("id"),
-    model_uri=KGCL.id,
-    domain=None,
-    range=URIRef,
-)
-
-slots.description = Slot(
-    uri=DCTERMS.description,
-    name="description",
-    curie=DCTERMS.curie("description"),
-    model_uri=KGCL.description,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.configuration__name_predicate = Slot(
-    uri=KGCL.name_predicate,
-    name="configuration__name_predicate",
-    curie=KGCL.curie("name_predicate"),
-    model_uri=KGCL.configuration__name_predicate,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.configuration__definition_predicate = Slot(
-    uri=KGCL.definition_predicate,
-    name="configuration__definition_predicate",
-    curie=KGCL.curie("definition_predicate"),
-    model_uri=KGCL.configuration__definition_predicate,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.configuration__main_synonym_predicate = Slot(
-    uri=KGCL.main_synonym_predicate,
-    name="configuration__main_synonym_predicate",
-    curie=KGCL.curie("main_synonym_predicate"),
-    model_uri=KGCL.configuration__main_synonym_predicate,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.configuration__synonym_predicates = Slot(
-    uri=KGCL.synonym_predicates,
-    name="configuration__synonym_predicates",
-    curie=KGCL.curie("synonym_predicates"),
-    model_uri=KGCL.configuration__synonym_predicates,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.configuration__creator_predicate = Slot(
-    uri=KGCL.creator_predicate,
-    name="configuration__creator_predicate",
-    curie=KGCL.curie("creator_predicate"),
-    model_uri=KGCL.configuration__creator_predicate,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.configuration__contributor_predicate = Slot(
-    uri=KGCL.contributor_predicate,
-    name="configuration__contributor_predicate",
-    curie=KGCL.curie("contributor_predicate"),
-    model_uri=KGCL.configuration__contributor_predicate,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.configuration__obsoletion_workflow = Slot(
-    uri=KGCL.obsoletion_workflow,
-    name="configuration__obsoletion_workflow",
-    curie=KGCL.curie("obsoletion_workflow"),
-    model_uri=KGCL.configuration__obsoletion_workflow,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.configuration__obsoletion_policy = Slot(
-    uri=KGCL.obsoletion_policy,
-    name="configuration__obsoletion_policy",
-    curie=KGCL.curie("obsoletion_policy"),
-    model_uri=KGCL.configuration__obsoletion_policy,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.associated_change_set = Slot(
-    uri=KGCL.associated_change_set,
-    name="associated change set",
-    curie=KGCL.curie("associated_change_set"),
-    model_uri=KGCL.associated_change_set,
-    domain=None,
-    range=Optional[
-        Union[
-            Dict[Union[str, ChangeId], Union[dict, Change]], List[Union[dict, Change]]
-        ]
-    ],
-)
-
-slots.change_type = Slot(
-    uri=KGCL.change_type,
-    name="change type",
-    curie=KGCL.curie("change_type"),
-    model_uri=KGCL.change_type,
-    domain=None,
-    range=Optional[Union[str, ChangeClassType]],
-)
-
-slots.count = Slot(
-    uri=KGCL.count,
-    name="count",
-    curie=KGCL.curie("count"),
-    model_uri=KGCL.count,
-    domain=None,
-    range=Optional[int],
-)
-
-slots.change_1 = Slot(
-    uri=KGCL.change_1,
-    name="change 1",
-    curie=KGCL.curie("change_1"),
-    model_uri=KGCL.change_1,
-    domain=None,
-    range=Optional[Union[str, NodeRenameId]],
-)
-
-slots.change_2 = Slot(
-    uri=KGCL.change_2,
-    name="change 2",
-    curie=KGCL.curie("change_2"),
-    model_uri=KGCL.change_2,
-    domain=None,
-    range=Optional[Union[str, NewSynonymId]],
-)
-
-slots.subset = Slot(
-    uri=KGCL.subset,
-    name="subset",
-    curie=KGCL.curie("subset"),
-    model_uri=KGCL.subset,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.replaced_by = Slot(
-    uri=KGCL.replaced_by,
-    name="replaced by",
-    curie=KGCL.curie("replaced_by"),
-    model_uri=KGCL.replaced_by,
-    domain=None,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.consider = Slot(
-    uri=KGCL.consider,
-    name="consider",
-    curie=KGCL.curie("consider"),
-    model_uri=KGCL.consider,
-    domain=None,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.change_was_generated_by = Slot(
-    uri=PROV.wasGeneratedBy,
-    name="change_was generated by",
-    curie=PROV.curie("wasGeneratedBy"),
-    model_uri=KGCL.change_was_generated_by,
-    domain=Change,
-    range=Optional[Union[str, ActivityId]],
-)
-
-slots.change_see_also = Slot(
-    uri=RDFS.seeAlso,
-    name="change_see also",
-    curie=RDFS.curie("seeAlso"),
-    model_uri=KGCL.change_see_also,
-    domain=Change,
-    range=Optional[str],
-)
-
-slots.change_pull_request = Slot(
-    uri=KGCL.pull_request,
-    name="change_pull request",
-    curie=KGCL.curie("pull_request"),
-    model_uri=KGCL.change_pull_request,
-    domain=Change,
-    range=Optional[str],
-)
-
-slots.change_creator = Slot(
-    uri=DCTERMS.creator,
-    name="change_creator",
-    curie=DCTERMS.curie("creator"),
-    model_uri=KGCL.change_creator,
-    domain=Change,
-    range=Optional[str],
-)
-
-slots.change_change_date = Slot(
-    uri=DCTERMS.date,
-    name="change_change date",
-    curie=DCTERMS.curie("date"),
-    model_uri=KGCL.change_change_date,
-    domain=Change,
-    range=Optional[str],
-)
-
-slots.multi_node_obsoletion_change_set = Slot(
-    uri=KGCL.change_set,
-    name="multi node obsoletion_change set",
-    curie=KGCL.curie("change_set"),
-    model_uri=KGCL.multi_node_obsoletion_change_set,
-    domain=MultiNodeObsoletion,
-    range=Optional[
-        Union[
-            Dict[Union[str, NodeObsoletionId], Union[dict, "NodeObsoletion"]],
-            List[Union[dict, "NodeObsoletion"]],
-        ]
-    ],
-)
-
-slots.multi_node_obsoletion_change_description = Slot(
-    uri=KGCL.change_description,
-    name="multi node obsoletion_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.multi_node_obsoletion_change_description,
-    domain=MultiNodeObsoletion,
-    range=Optional[str],
-)
-
-slots.multi_node_obsoletion_associated_change_set = Slot(
-    uri=KGCL.associated_change_set,
-    name="multi node obsoletion_associated change set",
-    curie=KGCL.curie("associated_change_set"),
-    model_uri=KGCL.multi_node_obsoletion_associated_change_set,
-    domain=MultiNodeObsoletion,
-    range=Optional[
-        Union[
-            Dict[Union[str, ChangeId], Union[dict, Change]], List[Union[dict, Change]]
-        ]
-    ],
-)
-
-slots.change_set_summary_statistic_change_type = Slot(
-    uri=KGCL.change_type,
-    name="change set summary statistic_change type",
-    curie=KGCL.curie("change_type"),
-    model_uri=KGCL.change_set_summary_statistic_change_type,
-    domain=ChangeSetSummaryStatistic,
-    range=Optional[Union[str, ChangeClassType]],
-)
-
-slots.change_set_summary_statistic_count = Slot(
-    uri=KGCL.count,
-    name="change set summary statistic_count",
-    curie=KGCL.curie("count"),
-    model_uri=KGCL.change_set_summary_statistic_count,
-    domain=ChangeSetSummaryStatistic,
-    range=Optional[int],
-)
-
-slots.change_set_summary_statistic_property_value_set = Slot(
-    uri=OM.property_value_set,
-    name="change set summary statistic_property value set",
-    curie=OM.curie("property_value_set"),
-    model_uri=KGCL.change_set_summary_statistic_property_value_set,
-    domain=ChangeSetSummaryStatistic,
-    range=Optional[
-        Union[Union[dict, "PropertyValue"], List[Union[dict, "PropertyValue"]]]
-    ],
-)
-
-slots.obsoletion_about = Slot(
-    uri=KGCL.about,
-    name="obsoletion_about",
-    curie=KGCL.curie("about"),
-    model_uri=KGCL.obsoletion_about,
-    domain=None,
-    range=Optional[Union[dict, "OntologyElement"]],
-)
-
-slots.obsoletion_has_undo = Slot(
-    uri=KGCL.has_undo,
-    name="obsoletion_has undo",
-    curie=KGCL.curie("has_undo"),
-    model_uri=KGCL.obsoletion_has_undo,
-    domain=None,
-    range=Optional[Union[dict, "Obsoletion"]],
-)
-
-slots.language_tag_change_old_value = Slot(
-    uri=KGCL.old_value,
-    name="language tag change_old value",
-    curie=KGCL.curie("old_value"),
-    model_uri=KGCL.language_tag_change_old_value,
-    domain=LanguageTagChange,
-    range=Optional[str],
-)
-
-slots.language_tag_change_new_value = Slot(
-    uri=KGCL.new_value,
-    name="language tag change_new value",
-    curie=KGCL.curie("new_value"),
-    model_uri=KGCL.language_tag_change_new_value,
-    domain=LanguageTagChange,
-    range=Optional[str],
-)
-
-slots.unobsoletion_has_undo = Slot(
-    uri=KGCL.has_undo,
-    name="unobsoletion_has undo",
-    curie=KGCL.curie("has_undo"),
-    model_uri=KGCL.unobsoletion_has_undo,
-    domain=None,
-    range=Optional[Union[dict, Obsoletion]],
-)
-
-slots.creation_has_undo = Slot(
-    uri=KGCL.has_undo,
-    name="creation_has undo",
-    curie=KGCL.curie("has_undo"),
-    model_uri=KGCL.creation_has_undo,
-    domain=None,
-    range=Optional[Union[dict, Deletion]],
-)
-
-slots.add_to_subset_in_subset = Slot(
-    uri=KGCL.in_subset,
-    name="add to subset_in subset",
-    curie=KGCL.curie("in_subset"),
-    model_uri=KGCL.add_to_subset_in_subset,
-    domain=None,
-    range=Optional[Union[dict, "OntologySubset"]],
-)
-
-slots.remove_from_subset_in_subset = Slot(
-    uri=KGCL.in_subset,
-    name="remove from subset_in subset",
-    curie=KGCL.curie("in_subset"),
-    model_uri=KGCL.remove_from_subset_in_subset,
-    domain=None,
-    range=Optional[Union[dict, "OntologySubset"]],
-)
-
-slots.remove_from_subset_has_undo = Slot(
-    uri=KGCL.has_undo,
-    name="remove from subset_has undo",
-    curie=KGCL.curie("has_undo"),
-    model_uri=KGCL.remove_from_subset_has_undo,
-    domain=None,
-    range=Optional[Union[dict, AddToSubset]],
-)
-
-slots.edge_change_subject = Slot(
-    uri=OM.subject,
-    name="edge change_subject",
-    curie=OM.curie("subject"),
-    model_uri=KGCL.edge_change_subject,
-    domain=EdgeChange,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.edge_creation_change_description = Slot(
-    uri=KGCL.change_description,
-    name="edge creation_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.edge_creation_change_description,
-    domain=EdgeCreation,
-    range=Optional[str],
-)
-
-slots.edge_deletion_change_description = Slot(
-    uri=KGCL.change_description,
-    name="edge deletion_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.edge_deletion_change_description,
-    domain=EdgeDeletion,
-    range=Optional[str],
-)
-
-slots.edge_obsoletion_change_description = Slot(
-    uri=KGCL.change_description,
-    name="edge obsoletion_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.edge_obsoletion_change_description,
-    domain=EdgeObsoletion,
-    range=Optional[str],
-)
-
-slots.mapping_creation_change_description = Slot(
-    uri=KGCL.change_description,
-    name="mapping creation_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.mapping_creation_change_description,
-    domain=MappingCreation,
-    range=Optional[str],
-)
-
-slots.mapping_creation_subject = Slot(
-    uri=OM.subject,
-    name="mapping creation_subject",
-    curie=OM.curie("subject"),
-    model_uri=KGCL.mapping_creation_subject,
-    domain=MappingCreation,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.mapping_creation_predicate = Slot(
-    uri=OM.predicate,
-    name="mapping creation_predicate",
-    curie=OM.curie("predicate"),
-    model_uri=KGCL.mapping_creation_predicate,
-    domain=MappingCreation,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.mapping_creation_object = Slot(
-    uri=OM.object,
-    name="mapping creation_object",
-    curie=OM.curie("object"),
-    model_uri=KGCL.mapping_creation_object,
-    domain=MappingCreation,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.node_move_change_description = Slot(
-    uri=KGCL.change_description,
-    name="node move_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.node_move_change_description,
-    domain=NodeMove,
-    range=Optional[str],
-)
-
-slots.node_deepening_change_description = Slot(
-    uri=KGCL.change_description,
-    name="node deepening_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.node_deepening_change_description,
-    domain=NodeDeepening,
-    range=Optional[str],
-)
-
-slots.node_shallowing_change_description = Slot(
-    uri=KGCL.change_description,
-    name="node shallowing_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.node_shallowing_change_description,
-    domain=NodeShallowing,
-    range=Optional[str],
-)
-
-slots.predicate_change_change_description = Slot(
-    uri=KGCL.change_description,
-    name="predicate change_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.predicate_change_change_description,
-    domain=PredicateChange,
-    range=Optional[str],
-)
-
-slots.node_rename_old_value = Slot(
-    uri=KGCL.old_value,
-    name="node rename_old value",
-    curie=KGCL.curie("old_value"),
-    model_uri=KGCL.node_rename_old_value,
-    domain=NodeRename,
-    range=Optional[str],
-)
-
-slots.node_rename_new_value = Slot(
-    uri=KGCL.new_value,
-    name="node rename_new value",
-    curie=KGCL.curie("new_value"),
-    model_uri=KGCL.node_rename_new_value,
-    domain=NodeRename,
-    range=Optional[str],
-)
-
-slots.node_rename_change_description = Slot(
-    uri=KGCL.change_description,
-    name="node rename_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.node_rename_change_description,
-    domain=NodeRename,
-    range=Optional[str],
-)
-
-slots.set_language_for_name_change_description = Slot(
-    uri=KGCL.change_description,
-    name="set language for name_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.set_language_for_name_change_description,
-    domain=SetLanguageForName,
-    range=Optional[str],
-)
-
-slots.name_becomes_synonym_change_1 = Slot(
-    uri=KGCL.change_1,
-    name="name becomes synonym_change 1",
-    curie=KGCL.curie("change_1"),
-    model_uri=KGCL.name_becomes_synonym_change_1,
-    domain=NameBecomesSynonym,
-    range=Optional[Union[str, NodeRenameId]],
-)
-
-slots.name_becomes_synonym_change_2 = Slot(
-    uri=KGCL.change_2,
-    name="name becomes synonym_change 2",
-    curie=KGCL.curie("change_2"),
-    model_uri=KGCL.name_becomes_synonym_change_2,
-    domain=NameBecomesSynonym,
-    range=Optional[Union[str, NewSynonymId]],
-)
-
-slots.name_becomes_synonym_change_description = Slot(
-    uri=KGCL.change_description,
-    name="name becomes synonym_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.name_becomes_synonym_change_description,
-    domain=NameBecomesSynonym,
-    range=Optional[str],
-)
-
-slots.removed_node_from_subset_change_description = Slot(
-    uri=KGCL.change_description,
-    name="removed node from subset_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.removed_node_from_subset_change_description,
-    domain=RemovedNodeFromSubset,
-    range=Optional[str],
-)
-
-slots.removed_node_from_subset_about_node = Slot(
-    uri=KGCL.about_node,
-    name="removed node from subset_about node",
-    curie=KGCL.curie("about_node"),
-    model_uri=KGCL.removed_node_from_subset_about_node,
-    domain=RemovedNodeFromSubset,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.removed_node_from_subset_subset = Slot(
-    uri=KGCL.subset,
-    name="removed node from subset_subset",
-    curie=KGCL.curie("subset"),
-    model_uri=KGCL.removed_node_from_subset_subset,
-    domain=RemovedNodeFromSubset,
-    range=Optional[str],
-)
-
-slots.node_obsoletion_change_description = Slot(
-    uri=KGCL.change_description,
-    name="node obsoletion_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.node_obsoletion_change_description,
-    domain=NodeObsoletion,
-    range=Optional[str],
-)
-
-slots.node_obsoletion_associated_change_set = Slot(
-    uri=KGCL.associated_change_set,
-    name="node obsoletion_associated change set",
-    curie=KGCL.curie("associated_change_set"),
-    model_uri=KGCL.node_obsoletion_associated_change_set,
-    domain=NodeObsoletion,
-    range=Optional[
-        Union[
-            Dict[Union[str, ChangeId], Union[dict, Change]], List[Union[dict, Change]]
-        ]
-    ],
-)
-
-slots.node_unobsoletion_change_description = Slot(
-    uri=KGCL.change_description,
-    name="node unobsoletion_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.node_unobsoletion_change_description,
-    domain=NodeUnobsoletion,
-    range=Optional[str],
-)
-
-slots.node_unobsoletion_replaced_by = Slot(
-    uri=KGCL.replaced_by,
-    name="node unobsoletion_replaced by",
-    curie=KGCL.curie("replaced_by"),
-    model_uri=KGCL.node_unobsoletion_replaced_by,
-    domain=NodeUnobsoletion,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.node_unobsoletion_consider = Slot(
-    uri=KGCL.consider,
-    name="node unobsoletion_consider",
-    curie=KGCL.curie("consider"),
-    model_uri=KGCL.node_unobsoletion_consider,
-    domain=NodeUnobsoletion,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.node_creation_change_description = Slot(
-    uri=KGCL.change_description,
-    name="node creation_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.node_creation_change_description,
-    domain=NodeCreation,
-    range=Optional[str],
-)
-
-slots.class_creation_change_description = Slot(
-    uri=KGCL.change_description,
-    name="class creation_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.class_creation_change_description,
-    domain=ClassCreation,
-    range=Optional[str],
-)
-
-slots.node_deletion_change_description = Slot(
-    uri=KGCL.change_description,
-    name="node deletion_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.node_deletion_change_description,
-    domain=NodeDeletion,
-    range=Optional[str],
-)
-
-slots.node_direct_merge_has_direct_replacement = Slot(
-    uri=KGCL.has_direct_replacement,
-    name="node direct merge_has direct replacement",
-    curie=KGCL.curie("has_direct_replacement"),
-    model_uri=KGCL.node_direct_merge_has_direct_replacement,
-    domain=NodeDirectMerge,
-    range=Union[str, NodeId],
-)
-
-slots.node_direct_merge_about_node = Slot(
-    uri=KGCL.about_node,
-    name="node direct merge_about node",
-    curie=KGCL.curie("about_node"),
-    model_uri=KGCL.node_direct_merge_about_node,
-    domain=NodeDirectMerge,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.node_direct_merge_change_description = Slot(
-    uri=KGCL.change_description,
-    name="node direct merge_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.node_direct_merge_change_description,
-    domain=NodeDirectMerge,
-    range=Optional[str],
-)
-
-slots.node_obsoletion_with_direct_replacement_has_direct_replacement = Slot(
-    uri=KGCL.has_direct_replacement,
-    name="node obsoletion with direct replacement_has direct replacement",
-    curie=KGCL.curie("has_direct_replacement"),
-    model_uri=KGCL.node_obsoletion_with_direct_replacement_has_direct_replacement,
-    domain=NodeObsoletionWithDirectReplacement,
-    range=Union[str, NodeId],
-)
-
-slots.node_obsoletion_with_direct_replacement_change_description = Slot(
-    uri=KGCL.change_description,
-    name="node obsoletion with direct replacement_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.node_obsoletion_with_direct_replacement_change_description,
-    domain=NodeObsoletionWithDirectReplacement,
-    range=Optional[str],
-)
-
-slots.node_obsoletion_with_no_direct_replacement_has_nondirect_replacement = Slot(
-    uri=KGCL.has_nondirect_replacement,
-    name="node obsoletion with no direct replacement_has nondirect replacement",
-    curie=KGCL.curie("has_nondirect_replacement"),
-    model_uri=KGCL.node_obsoletion_with_no_direct_replacement_has_nondirect_replacement,
-    domain=NodeObsoletionWithNoDirectReplacement,
-    range=Union[Union[str, NodeId], List[Union[str, NodeId]]],
-)
-
-slots.node_obsoletion_with_no_direct_replacement_change_description = Slot(
-    uri=KGCL.change_description,
-    name="node obsoletion with no direct replacement_change description",
-    curie=KGCL.curie("change_description"),
-    model_uri=KGCL.node_obsoletion_with_no_direct_replacement_change_description,
-    domain=NodeObsoletionWithNoDirectReplacement,
-    range=Optional[str],
-)
+slots.NodeObsoletionWithNoDirectReplacement_change_description = Slot(uri=KGCL.change_description, name="NodeObsoletionWithNoDirectReplacement_change_description", curie=KGCL.curie('change_description'),
+                   model_uri=KGCL.NodeObsoletionWithNoDirectReplacement_change_description, domain=NodeObsoletionWithNoDirectReplacement, range=Optional[str])
```

### Comparing `kgcl_schema-0.4.0/src/kgcl_schema/datamodel/ontology_model.py` & `kgcl_schema-0.4.0rc1/src/kgcl_schema/datamodel/ontology_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,55 @@
 # Auto generated from ontology_model.yaml by pythongen.py version: 0.9.0
-# Generation date: 2022-06-30T15:03:19
+# Generation date: 2023-05-08T15:28:23
 # Schema: kgcl_schema-ontology-model
 #
-# id: https://w3id.org/kgcl/ontology
-# description: A basic bare-bones model of an ontology or ontology-like structure. The purpose is not to provide a
-#              complete model, rather just sufficient structure for domain and range constraints in the ocl model
+# id: https://w3id.org/kgcl_schema/ontology
+# description: A basic bare-bones model of an ontology or ontology-like structure. The purpose is not to provide a complete model, rather just sufficient structure for domain and range constraints in the ocl model
 # license: https://creativecommons.org/publicdomain/zero/1.0/
 
 import dataclasses
-import sys
 import re
 from jsonasobj2 import JsonObj, as_dict
 from typing import Optional, List, Union, Dict, ClassVar, Any
 from dataclasses import dataclass
-from linkml_runtime.linkml_model.meta import (
-    EnumDefinition,
-    PermissibleValue,
-    PvFormulaOptions,
-)
+from linkml_runtime.linkml_model.meta import EnumDefinition, PermissibleValue, PvFormulaOptions
 
 from linkml_runtime.utils.slot import Slot
 from linkml_runtime.utils.metamodelcore import empty_list, empty_dict, bnode
-from linkml_runtime.utils.yamlutils import (
-    YAMLRoot,
-    extended_str,
-    extended_float,
-    extended_int,
-)
-from linkml_runtime.utils.dataclass_extensions_376 import (
-    dataclasses_init_fn_with_kwargs,
-)
+from linkml_runtime.utils.yamlutils import YAMLRoot, extended_str, extended_float, extended_int
+from linkml_runtime.utils.dataclass_extensions_376 import dataclasses_init_fn_with_kwargs
 from linkml_runtime.utils.formatutils import camelcase, underscore, sfx
 from linkml_runtime.utils.enumerations import EnumDefinitionImpl
 from rdflib import Namespace, URIRef
 from linkml_runtime.utils.curienamespace import CurieNamespace
 from linkml_runtime.linkml_model.types import String
 
 metamodel_version = "1.7.0"
 version = "0.0.1"
 
 # Overwrite dataclasses _init_fn to add **kwargs in __init__
 dataclasses._init_fn = dataclasses_init_fn_with_kwargs
 
 # Namespaces
-BASICS = CurieNamespace("basics", "https://w3id.org/kgcl/basics/")
-DCTERMS = CurieNamespace("dcterms", "http://purl.org/dc/terms/")
-LINKML = CurieNamespace("linkml", "https://w3id.org/linkml/")
-OIO = CurieNamespace("oio", "http://www.geneontology.org/formats/oboInOwl#")
-OM = CurieNamespace("om", "http://w3id.org/kgcl/om/")
-OWL = CurieNamespace("owl", "http://www.w3.org/2002/07/owl#")
-RDF = CurieNamespace("rdf", "http://www.w3.org/1999/02/22-rdf-syntax-ns#")
-XML = CurieNamespace("xml", "http://example.org/UNKNOWN/xml/")
+BASICS = CurieNamespace('basics', 'https://w3id.org/kgcl_schema/basics/')
+DCTERMS = CurieNamespace('dcterms', 'http://purl.org/dc/terms/')
+LINKML = CurieNamespace('linkml', 'https://w3id.org/linkml/')
+OIO = CurieNamespace('oio', 'http://www.geneontology.org/formats/oboInOwl#')
+OM = CurieNamespace('om', 'http://w3id.org/kgcl_schema/om/')
+OWL = CurieNamespace('owl', 'http://www.w3.org/2002/07/owl#')
+RDF = CurieNamespace('rdf', 'http://www.w3.org/1999/02/22-rdf-syntax-ns#')
+XML = CurieNamespace('xml', 'http://example.org/UNKNOWN/xml/')
 DEFAULT_ = OM
 
 
 # Types
 class LanguageTag(str):
     type_class_uri = XML.lang
     type_class_curie = "xml:lang"
-    type_name = "language tag"
+    type_name = "LanguageTag"
     type_model_uri = OM.LanguageTag
 
 
 # Class references
 class NodeId(extended_str):
     pass
 
@@ -75,34 +62,32 @@
     pass
 
 
 class OntologyElement(YAMLRoot):
     """
     Any component of an ontology or knowledge graph
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = OM.OntologyElement
     class_class_curie: ClassVar[str] = "om:OntologyElement"
-    class_name: ClassVar[str] = "ontology element"
+    class_name: ClassVar[str] = "OntologyElement"
     class_model_uri: ClassVar[URIRef] = OM.OntologyElement
 
 
 @dataclass
 class PropertyValue(OntologyElement):
     """
     a property-value pair
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = OM.PropertyValue
     class_class_curie: ClassVar[str] = "om:PropertyValue"
-    class_name: ClassVar[str] = "property value"
+    class_name: ClassVar[str] = "PropertyValue"
     class_model_uri: ClassVar[URIRef] = OM.PropertyValue
 
     property: Optional[Union[str, NodeId]] = None
     filler: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.property is not None and not isinstance(self.property, NodeId):
@@ -115,20 +100,19 @@
 
 
 @dataclass
 class Annotation(PropertyValue):
     """
     owl annotations. Not to be confused with annotations sensu GO
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = OM.Annotation
     class_class_curie: ClassVar[str] = "om:Annotation"
-    class_name: ClassVar[str] = "annotation"
+    class_name: ClassVar[str] = "Annotation"
     class_model_uri: ClassVar[URIRef] = OM.Annotation
 
     property: Optional[Union[str, NodeId]] = None
     filler: Optional[str] = None
     annotation_set: Optional[Union[dict, "Annotation"]] = None
     property_type: Optional[str] = None
     filler_type: Optional[str] = None
@@ -136,17 +120,15 @@
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.property is not None and not isinstance(self.property, NodeId):
             self.property = NodeId(self.property)
 
         if self.filler is not None and not isinstance(self.filler, str):
             self.filler = str(self.filler)
 
-        if self.annotation_set is not None and not isinstance(
-            self.annotation_set, Annotation
-        ):
+        if self.annotation_set is not None and not isinstance(self.annotation_set, Annotation):
             self.annotation_set = Annotation(**as_dict(self.annotation_set))
 
         if self.property_type is not None and not isinstance(self.property_type, str):
             self.property_type = str(self.property_type)
 
         if self.filler_type is not None and not isinstance(self.filler_type, str):
             self.filler_type = str(self.filler_type)
@@ -155,20 +137,19 @@
 
 
 @dataclass
 class Node(OntologyElement):
     """
     Any named entity in an ontology. May be a class, individual, property
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = OM.Node
     class_class_curie: ClassVar[str] = "om:Node"
-    class_name: ClassVar[str] = "node"
+    class_name: ClassVar[str] = "Node"
     class_model_uri: ClassVar[URIRef] = OM.Node
 
     id: Union[str, NodeId] = None
     name: Optional[str] = None
     annotation_set: Optional[Union[dict, Annotation]] = None
     owl_type: Optional[Union[str, "OwlTypeEnum"]] = None
 
@@ -177,36 +158,33 @@
             self.MissingRequiredField("id")
         if not isinstance(self.id, NodeId):
             self.id = NodeId(self.id)
 
         if self.name is not None and not isinstance(self.name, str):
             self.name = str(self.name)
 
-        if self.annotation_set is not None and not isinstance(
-            self.annotation_set, Annotation
-        ):
+        if self.annotation_set is not None and not isinstance(self.annotation_set, Annotation):
             self.annotation_set = Annotation(**as_dict(self.annotation_set))
 
         if self.owl_type is not None and not isinstance(self.owl_type, OwlTypeEnum):
             self.owl_type = OwlTypeEnum(self.owl_type)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class ClassNode(Node):
     """
     A node that is a class
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = OWL.Class
     class_class_curie: ClassVar[str] = "owl:Class"
-    class_name: ClassVar[str] = "class node"
+    class_name: ClassVar[str] = "ClassNode"
     class_model_uri: ClassVar[URIRef] = OM.ClassNode
 
     id: Union[str, ClassNodeId] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
@@ -217,20 +195,19 @@
 
 
 @dataclass
 class InstanceNode(Node):
     """
     A node that is an individual
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = OWL.NamedIndividual
     class_class_curie: ClassVar[str] = "owl:NamedIndividual"
-    class_name: ClassVar[str] = "instance node"
+    class_name: ClassVar[str] = "InstanceNode"
     class_model_uri: ClassVar[URIRef] = OM.InstanceNode
 
     id: Union[str, InstanceNodeId] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
@@ -248,32 +225,30 @@
 
     * A subClassOf B <==> Edge(subject=A, predicate=owl:subClassOf, object=B)
     * A subClassOf P some B <==> Edge(subject=A, predicate=P, object=B)
     * P subPropertyOf Q <==> Edge(subject=P, predicate=owl:subPropertyOf, object=Q)
 
     These represent the most common kind of pairwise relationship between classes, and classes are the dominant node
     type in ontologies.
-
     In future a wider variety of OWL axiom types will be supportedn through the use of an additional edge
     property/slot to indicate the interpretation of the axiom, following owlstar
     (https://github.com/cmungall/owlstar).
     For example:
     * `A subClassOf R only B <==> Edge(subject=A, predicate=P, object=B, interpretation=AllOnly)`
     * `A Annotation(P,B) <==> Edge(subject=A, predicate=P, object=B, interpretation=annotationAssertion)`
 
     Note that not all axioms are intended to map to edges. Axioms/triples where the object is a literal would be
     represented as node properties. Complex OWL axioms involving nesting would have their own dedicated construct, or
     may be represented generically. These are out of scope for the current version of KGCL
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = OM.Edge
     class_class_curie: ClassVar[str] = "om:Edge"
-    class_name: ClassVar[str] = "edge"
+    class_name: ClassVar[str] = "Edge"
     class_model_uri: ClassVar[URIRef] = OM.Edge
 
     subject: Optional[Union[str, NodeId]] = None
     predicate: Optional[Union[str, NodeId]] = None
     object: Optional[Union[str, NodeId]] = None
     subject_representation: Optional[str] = None
     predicate_representation: Optional[str] = None
@@ -286,224 +261,127 @@
 
         if self.predicate is not None and not isinstance(self.predicate, NodeId):
             self.predicate = NodeId(self.predicate)
 
         if self.object is not None and not isinstance(self.object, NodeId):
             self.object = NodeId(self.object)
 
-        if self.subject_representation is not None and not isinstance(
-            self.subject_representation, str
-        ):
+        if self.subject_representation is not None and not isinstance(self.subject_representation, str):
             self.subject_representation = str(self.subject_representation)
 
-        if self.predicate_representation is not None and not isinstance(
-            self.predicate_representation, str
-        ):
+        if self.predicate_representation is not None and not isinstance(self.predicate_representation, str):
             self.predicate_representation = str(self.predicate_representation)
 
-        if self.object_representation is not None and not isinstance(
-            self.object_representation, str
-        ):
+        if self.object_representation is not None and not isinstance(self.object_representation, str):
             self.object_representation = str(self.object_representation)
 
-        if self.annotation_set is not None and not isinstance(
-            self.annotation_set, Annotation
-        ):
+        if self.annotation_set is not None and not isinstance(self.annotation_set, Annotation):
             self.annotation_set = Annotation(**as_dict(self.annotation_set))
 
         super().__post_init__(**kwargs)
 
 
 class LogicalDefinition(OntologyElement):
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = OM.LogicalDefinition
     class_class_curie: ClassVar[str] = "om:LogicalDefinition"
-    class_name: ClassVar[str] = "logical definition"
+    class_name: ClassVar[str] = "LogicalDefinition"
     class_model_uri: ClassVar[URIRef] = OM.LogicalDefinition
 
 
 class OntologySubset(OntologyElement):
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = OM.OntologySubset
     class_class_curie: ClassVar[str] = "om:OntologySubset"
-    class_name: ClassVar[str] = "ontology subset"
+    class_name: ClassVar[str] = "OntologySubset"
     class_model_uri: ClassVar[URIRef] = OM.OntologySubset
 
 
 # Enumerations
 class OwlTypeEnum(EnumDefinitionImpl):
 
-    CLASS = PermissibleValue(text="CLASS", meaning=OWL.Class)
+    CLASS = PermissibleValue(
+        text="CLASS",
+        meaning=OWL.Class)
     OBJECT_PROPERTY = PermissibleValue(
-        text="OBJECT_PROPERTY", meaning=OWL.ObjectProperty
-    )
+        text="OBJECT_PROPERTY",
+        meaning=OWL.ObjectProperty)
     NAMED_INDIVIDUAL = PermissibleValue(
-        text="NAMED_INDIVIDUAL", meaning=OWL.NamedIndividual
-    )
+        text="NAMED_INDIVIDUAL",
+        meaning=OWL.NamedIndividual)
 
     _defn = EnumDefinition(
         name="OwlTypeEnum",
     )
 
-
 class SynonymScopeEnum(EnumDefinitionImpl):
 
-    related = PermissibleValue(text="related", meaning=OIO.hasNarrowSynonym)
-    broad = PermissibleValue(text="broad", meaning=OIO.hasBroadSynonym)
-    narrow = PermissibleValue(text="narrow", meaning=OIO.hasNarrowSynonym)
-    exact = PermissibleValue(text="exact", meaning=OIO.hasExactSynonym)
+    related = PermissibleValue(
+        text="related",
+        meaning=OIO.hasNarrowSynonym)
+    broad = PermissibleValue(
+        text="broad",
+        meaning=OIO.hasBroadSynonym)
+    narrow = PermissibleValue(
+        text="narrow",
+        meaning=OIO.hasNarrowSynonym)
+    exact = PermissibleValue(
+        text="exact",
+        meaning=OIO.hasExactSynonym)
 
     _defn = EnumDefinition(
         name="SynonymScopeEnum",
     )
 
-
 # Slots
 class slots:
     pass
 
+slots.owl_type = Slot(uri=OM.owl_type, name="owl_type", curie=OM.curie('owl_type'),
+                   model_uri=OM.owl_type, domain=None, range=Optional[Union[str, "OwlTypeEnum"]])
+
+slots.name = Slot(uri=OM.name, name="name", curie=OM.curie('name'),
+                   model_uri=OM.name, domain=None, range=Optional[str])
+
+slots.subject = Slot(uri=OM.subject, name="subject", curie=OM.curie('subject'),
+                   model_uri=OM.subject, domain=None, range=Optional[Union[str, NodeId]])
+
+slots.object = Slot(uri=OM.object, name="object", curie=OM.curie('object'),
+                   model_uri=OM.object, domain=None, range=Optional[Union[str, NodeId]])
+
+slots.predicate = Slot(uri=OM.predicate, name="predicate", curie=OM.curie('predicate'),
+                   model_uri=OM.predicate, domain=None, range=Optional[Union[str, NodeId]])
+
+slots.annotation_set = Slot(uri=OM.annotation_set, name="annotation_set", curie=OM.curie('annotation_set'),
+                   model_uri=OM.annotation_set, domain=None, range=Optional[Union[dict, Annotation]])
+
+slots.property = Slot(uri=OM.property, name="property", curie=OM.curie('property'),
+                   model_uri=OM.property, domain=None, range=Optional[Union[str, NodeId]])
+
+slots.filler = Slot(uri=OM.filler, name="filler", curie=OM.curie('filler'),
+                   model_uri=OM.filler, domain=None, range=Optional[str])
+
+slots.property_type = Slot(uri=OM.property_type, name="property_type", curie=OM.curie('property_type'),
+                   model_uri=OM.property_type, domain=None, range=Optional[str])
+
+slots.filler_type = Slot(uri=OM.filler_type, name="filler_type", curie=OM.curie('filler_type'),
+                   model_uri=OM.filler_type, domain=None, range=Optional[str])
+
+slots.subject_representation = Slot(uri=OM.subject_representation, name="subject_representation", curie=OM.curie('subject_representation'),
+                   model_uri=OM.subject_representation, domain=None, range=Optional[str])
+
+slots.predicate_representation = Slot(uri=OM.predicate_representation, name="predicate_representation", curie=OM.curie('predicate_representation'),
+                   model_uri=OM.predicate_representation, domain=None, range=Optional[str])
+
+slots.object_representation = Slot(uri=OM.object_representation, name="object_representation", curie=OM.curie('object_representation'),
+                   model_uri=OM.object_representation, domain=None, range=Optional[str])
+
+slots.property_value_set = Slot(uri=OM.property_value_set, name="property_value_set", curie=OM.curie('property_value_set'),
+                   model_uri=OM.property_value_set, domain=None, range=Optional[Union[Union[dict, PropertyValue], List[Union[dict, PropertyValue]]]])
+
+slots.id = Slot(uri=BASICS.id, name="id", curie=BASICS.curie('id'),
+                   model_uri=OM.id, domain=None, range=URIRef)
 
-slots.owl_type = Slot(
-    uri=OM.owl_type,
-    name="owl type",
-    curie=OM.curie("owl_type"),
-    model_uri=OM.owl_type,
-    domain=None,
-    range=Optional[Union[str, "OwlTypeEnum"]],
-)
-
-slots.name = Slot(
-    uri=OM.name,
-    name="name",
-    curie=OM.curie("name"),
-    model_uri=OM.name,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.subject = Slot(
-    uri=OM.subject,
-    name="subject",
-    curie=OM.curie("subject"),
-    model_uri=OM.subject,
-    domain=None,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.object = Slot(
-    uri=OM.object,
-    name="object",
-    curie=OM.curie("object"),
-    model_uri=OM.object,
-    domain=None,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.predicate = Slot(
-    uri=OM.predicate,
-    name="predicate",
-    curie=OM.curie("predicate"),
-    model_uri=OM.predicate,
-    domain=None,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.annotation_set = Slot(
-    uri=OM.annotation_set,
-    name="annotation set",
-    curie=OM.curie("annotation_set"),
-    model_uri=OM.annotation_set,
-    domain=None,
-    range=Optional[Union[dict, Annotation]],
-)
-
-slots.property = Slot(
-    uri=OM.property,
-    name="property",
-    curie=OM.curie("property"),
-    model_uri=OM.property,
-    domain=None,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.filler = Slot(
-    uri=OM.filler,
-    name="filler",
-    curie=OM.curie("filler"),
-    model_uri=OM.filler,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.property_type = Slot(
-    uri=OM.property_type,
-    name="property type",
-    curie=OM.curie("property_type"),
-    model_uri=OM.property_type,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.filler_type = Slot(
-    uri=OM.filler_type,
-    name="filler type",
-    curie=OM.curie("filler_type"),
-    model_uri=OM.filler_type,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.subject_representation = Slot(
-    uri=OM.subject_representation,
-    name="subject representation",
-    curie=OM.curie("subject_representation"),
-    model_uri=OM.subject_representation,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.predicate_representation = Slot(
-    uri=OM.predicate_representation,
-    name="predicate representation",
-    curie=OM.curie("predicate_representation"),
-    model_uri=OM.predicate_representation,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.object_representation = Slot(
-    uri=OM.object_representation,
-    name="object representation",
-    curie=OM.curie("object_representation"),
-    model_uri=OM.object_representation,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.property_value_set = Slot(
-    uri=OM.property_value_set,
-    name="property value set",
-    curie=OM.curie("property_value_set"),
-    model_uri=OM.property_value_set,
-    domain=None,
-    range=Optional[Union[Union[dict, PropertyValue], List[Union[dict, PropertyValue]]]],
-)
-
-slots.id = Slot(
-    uri=BASICS.id,
-    name="id",
-    curie=BASICS.curie("id"),
-    model_uri=OM.id,
-    domain=None,
-    range=URIRef,
-)
-
-slots.description = Slot(
-    uri=DCTERMS.description,
-    name="description",
-    curie=DCTERMS.curie("description"),
-    model_uri=OM.description,
-    domain=None,
-    range=Optional[str],
-)
+slots.description = Slot(uri=DCTERMS.description, name="description", curie=DCTERMS.curie('description'),
+                   model_uri=OM.description, domain=None, range=Optional[str])
```

### Comparing `kgcl_schema-0.4.0/src/kgcl_schema/grammar/kgcl.lark` & `kgcl_schema-0.4.0rc1/src/kgcl_schema/grammar/kgcl.lark`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.4.0/src/kgcl_schema/grammar/kgcl_2_rdf.py` & `kgcl_schema-0.4.0rc1/src/kgcl_schema/grammar/kgcl_2_rdf.py`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.4.0/src/kgcl_schema/grammar/parser.py` & `kgcl_schema-0.4.0rc1/src/kgcl_schema/grammar/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     NodeRename,
     NodeShallowing,
     NodeTextDefinitionChange,
     NodeUnobsoletion,
     PlaceUnder,
     PredicateChange,
     RemoveSynonym,
-    RemovedNodeFromSubset,
+    RemoveNodeFromSubset,
     RemoveUnder,
     Session,
     RemoveTextDefinition,
 )
 from kgcl_schema.datamodel.ontology_model import Edge
 from kgcl_schema.utils import to_json, to_rdf, to_yaml
 from lark import Lark, Token
```

### Comparing `kgcl_schema-0.4.0/src/kgcl_schema/grammar/render_operations.py` & `kgcl_schema-0.4.0rc1/src/kgcl_schema/grammar/render_operations.py`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.4.0/src/kgcl_schema/schema/ontology_model.yaml` & `kgcl_schema-0.4.0rc1/src/kgcl_schema/schema/ontology_model.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,196 +1,158 @@
 id: https://w3id.org/kgcl_schema/ontology
 name: kgcl_schema-ontology-model
 title: knowledge graph change language ontology model
-description: >-
-  A basic bare-bones model of an ontology or ontology-like structure. The purpose is not to provide a complete model,
-  rather just sufficient structure for domain and range constraints in the ocl model
-
+description: A basic bare-bones model of an ontology or ontology-like structure. The
+  purpose is not to provide a complete model, rather just sufficient structure for
+  domain and range constraints in the ocl model
 license: https://creativecommons.org/publicdomain/zero/1.0/
 version: 0.0.1
-
 prefixes:
   om: http://w3id.org/kgcl_schema/om/
   dcterms: http://purl.org/dc/terms/
   linkml: https://w3id.org/linkml/
   oio: http://www.geneontology.org/formats/oboInOwl#
-  
 default_prefix: om
 default_range: string
-
 imports:
-  - linkml:types
-  - basics
-  
+- linkml:types
+- basics
 classes:
-
-  ontology element:
+  OntologyElement:
     aliases:
-      - entity
-    description: >-
-      Any component of an ontology or knowledge graph
-
-  property value:
-    is_a: ontology element
-    description: >-
-      a property-value pair
+    - entity
+    description: Any component of an ontology or knowledge graph
+  PropertyValue:
+    is_a: OntologyElement
+    description: a property-value pair
     slots:
-      - property
-      - filler
-      
-  annotation:
-    is_a: property value
-    description: >-
-      owl annotations. Not to be confused with annotations sensu GO
+    - property
+    - filler
+  Annotation:
+    is_a: PropertyValue
+    description: owl annotations. Not to be confused with annotations sensu GO
     slots:
-      - property
-      - filler
-      - annotation set
-      - property type
-      - filler type
+    - property
+    - filler
+    - annotation_set
+    - property_type
+    - filler_type
     mappings:
-      - owl:Annotation
-      
-  node:
+    - owl:Annotation
+  Node:
     aliases:
-      - entity
-      - term
-    is_a: ontology element
-    description: >-
-      Any named entity in an ontology. May be a class, individual, property
+    - entity
+    - term
+    is_a: OntologyElement
+    description: Any named entity in an ontology. May be a class, individual, property
     slots:
-      - id
-      - name
-      - annotation set
-      - owl type
-
-  class node:
+    - id
+    - name
+    - annotation_set
+    - owl_type
+  ClassNode:
     aliases:
-      - concept
-    is_a: node
-    description: >-
-      A node that is a class
+    - concept
+    is_a: Node
+    description: A node that is a class
     class_uri: owl:Class
-
-  instance node:
+  InstanceNode:
     aliases:
-      - named individual
-    is_a: node
-    description: >-
-      A node that is an individual
+    - named individual
+    is_a: Node
+    description: A node that is an individual
     class_uri: owl:NamedIndividual
-
-  edge:
+  Edge:
     aliases:
-      - triple
-      - axiom
-      - relationship
-    is_a: ontology element
+    - triple
+    - axiom
+    - relationship
+    is_a: OntologyElement
     description: >-
       A relationship between two nodes.
-      
+
       Currently the only kinds of edges supported in KGCL:
 
         * A subClassOf B <==> Edge(subject=A, predicate=owl:subClassOf, object=B)
         * A subClassOf P some B <==> Edge(subject=A, predicate=P, object=B)
         * P subPropertyOf Q <==> Edge(subject=P, predicate=owl:subPropertyOf, object=Q)
 
       These represent the most common kind of pairwise relationship between classes,
       and classes are the dominant node type in ontologies.
-        
+
       In future a wider variety of OWL axiom types will be supportedn through the use
       of an additional edge property/slot to indicate the interpretation of the axiom,
       following owlstar (https://github.com/cmungall/owlstar).
 
       For example:
        * `A subClassOf R only B <==> Edge(subject=A, predicate=P, object=B, interpretation=AllOnly)`
        * `A Annotation(P,B) <==> Edge(subject=A, predicate=P, object=B, interpretation=annotationAssertion)`
 
       Note that not all axioms are intended to map to edges. Axioms/triples where the object is a literal
       would be represented as node properties. Complex OWL axioms involving nesting would have their own
       dedicated construct, or may be represented generically. These are out of scope for the current
       version of KGCL
+      
     mappings:
-      - owl:Axiom
-      - rdf:Statement
+    - owl:Axiom
+    - rdf:Statement
     slots:
-      - subject
-      - predicate
-      - object
-      - subject representation
-      - predicate representation
-      - object representation
-      - annotation set
-
-  logical definition:
-    is_a: ontology element
-  
-  ontology subset:
-    is_a: ontology element
-  
-
+    - subject
+    - predicate
+    - object
+    - subject_representation
+    - predicate_representation
+    - object_representation
+    - annotation_set
+  LogicalDefinition:
+    is_a: OntologyElement
+  OntologySubset:
+    is_a: OntologyElement
 slots:
-
-  owl type:
-    range: owl_type_enum
-    
+  owl_type:
+    range: OwlTypeEnum
   name: {}
-
   subject:
-    range: node
-
+    range: Node
   object:
-    range: node
-    
+    range: Node
   predicate:
-    range: node    
-    
-  annotation set:
-    range: annotation    
-
+    range: Node
+  annotation_set:
+    range: Annotation
   property:
-    range: node
-
-  filler:
-
-  property type:
+    range: Node
+  filler: null
+  property_type:
     deprecated: no longer required
-
-  filler type:
+  filler_type:
     deprecated: no longer required
-
-  subject representation:
+  subject_representation:
     deprecated: no longer required
-
-  predicate representation:
+  predicate_representation:
     deprecated: no longer required
-
-  object representation:
+  object_representation:
     deprecated: no longer required
-
-  property value set:
-    range: property value
+  property_value_set:
+    range: PropertyValue
     multivalued: true
     inlined: true
-
 enums:
-
-  owl_type_enum:
+  OwlTypeEnum:
     permissible_values:
       CLASS:
         meaning: owl:Class
       OBJECT_PROPERTY:
         meaning: owl:ObjectProperty
       NAMED_INDIVIDUAL:
         meaning: owl:NamedIndividual
-
-  synonym_scope_enum:
+  SynonymScopeEnum:
     permissible_values:
       related:
         meaning: oio:hasNarrowSynonym
       broad:
         meaning: oio:hasBroadSynonym
       narrow:
         meaning: oio:hasNarrowSynonym
       exact:
         meaning: oio:hasExactSynonym
-        
+
```

### Comparing `kgcl_schema-0.4.0/src/kgcl_schema/schema/prov.yaml` & `kgcl_schema-0.4.0rc1/src/kgcl_schema/schema/prov.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,82 +1,72 @@
 id: https://w3id.org/kgcl_schema/prov
 name: KGCL-PROV
 title: KGCL Rendering of prov schema
-description: >-
-  See https://www.w3.org/TR/prov-o/
+description: See https://www.w3.org/TR/prov-o/
 license: https://creativecommons.org/publicdomain/zero/1.0/
-
 prefixes:
   prov: http://www.w3.org/ns/prov#
   linkml: https://w3id.org/linkml/
-  
 default_prefix: prov
 default_range: string
-
 default_curi_maps:
-  - semweb_context
-
+- semweb_context
 imports:
-  - linkml:types
-  - basics
-
+- linkml:types
+- basics
 classes:
 
-  activity:
-    description: "a provence-generating activity"
+  ProvElement:
+    abstract: true
+    description: A grouping for prov elements
+
+  Activity:
+    is_a: ProvElement
+    description: a provence-generating activity
     slots:
-      - id
-      - started at time
-      - ended at time
-      - was informed by
-      - was associated with
-      - used
-      - description
+    - id
+    - started_at_time
+    - ended_at_time
+    - was_informed_by
+    - was_associated_with
+    - used
+    - description
     mappings:
-      - prov:Activity
-      
-  agent:
-    description: "a provence-generating agent"
+    - prov:Activity
+  Agent:
+    is_a: ProvElement
+    description: a provence-generating agent
     slots:
-      - id
-      - acted on behalf of
-      - was informed by
+    - id
+    - acted_on_behalf_of
+    - was_informed_by
     class_uri: prov:Agent
-      
 slots:
-
-  started at time:
+  started_at_time:
     slot_uri: prov:startedAtTime
-
-  ended at time:
+  ended_at_time:
     slot_uri: prov:endedAtTime
-
-  was informed by:
-    range: activity
+  was_informed_by:
+    range: Activity
     slot_uri: prov:wasInformedBy
-
-  was associated with:
-    range: agent
+  was_associated_with:
+    range: Agent
     slot_uri: prov:wasAssociatedWith
     inlined: false
-
-  acted on behalf of:
-    range: agent
+  acted_on_behalf_of:
+    range: Agent
     slot_uri: prov:actedOnBehalfOf
-
-  was generated by:
-    range: activity
+  was_generated_by:
+    range: Activity
     slot_uri: prov:wasGeneratedBy
-
   used:
-    domain: activity
+    domain: Activity
     slot_uri: prov:used
-
-  activity set:
-    range: activity
+  activity_set:
+    range: Activity
     multivalued: true
     inlined_as_list: true
-
-  agent set:
-    range: agent
+  agent_set:
+    range: Agent
     multivalued: true
     inlined_as_list: true
+
```

### Comparing `kgcl_schema-0.4.0/src/kgcl_schema/utils.py` & `kgcl_schema-0.4.0rc1/src/kgcl_schema/utils.py`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.4.0/PKG-INFO` & `kgcl_schema-0.4.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgcl-schema
-Version: 0.4.0
+Version: 0.4.0rc1
 Summary: Schema for the KGCL project.
 License: MIT
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

