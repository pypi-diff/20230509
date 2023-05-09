# Comparing `tmp/reasoner-pydantic-4.0.0.tar.gz` & `tmp/reasoner-pydantic-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner-pydantic-4.0.0.tar", last modified: Tue May  2 17:23:33 2023, max compression
+gzip compressed data, was "reasoner-pydantic-4.0.1.tar", last modified: Tue May  9 19:52:45 2023, max compression
```

## Comparing `reasoner-pydantic-4.0.0.tar` & `reasoner-pydantic-4.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:23:33.171311 reasoner-pydantic-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-02 17:23:33.171311 reasoner-pydantic-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:23:33.167310 reasoner-pydantic-4.0.0/reasoner_pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/auxgraphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/kgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/metakg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/qgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/reasoner_pydantic/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:23:33.171311 reasoner-pydantic-4.0.0/reasoner_pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-02 17:23:33.000000 reasoner-pydantic-4.0.0/reasoner_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-02 17:23:33.000000 reasoner-pydantic-4.0.0/reasoner_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:23:33.000000 reasoner-pydantic-4.0.0/reasoner_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:23:33.000000 reasoner-pydantic-4.0.0/reasoner_pydantic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 17:23:33.000000 reasoner-pydantic-4.0.0/reasoner_pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 17:23:33.000000 reasoner-pydantic-4.0.0/reasoner_pydantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:23:33.171311 reasoner-pydantic-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-02 17:23:29.000000 reasoner-pydantic-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:45.884259 reasoner-pydantic-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-09 19:52:45.884259 reasoner-pydantic-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:45.880259 reasoner-pydantic-4.0.1/reasoner_pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/auxgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/kgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/metakg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/qgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/reasoner_pydantic/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:45.880259 reasoner-pydantic-4.0.1/reasoner_pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-09 19:52:45.000000 reasoner-pydantic-4.0.1/reasoner_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-09 19:52:45.000000 reasoner-pydantic-4.0.1/reasoner_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:52:45.000000 reasoner-pydantic-4.0.1/reasoner_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:52:45.000000 reasoner-pydantic-4.0.1/reasoner_pydantic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 19:52:45.000000 reasoner-pydantic-4.0.1/reasoner_pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 19:52:45.000000 reasoner-pydantic-4.0.1/reasoner_pydantic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:52:45.884259 reasoner-pydantic-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-09 19:52:42.000000 reasoner-pydantic-4.0.1/setup.py
```

### Comparing `reasoner-pydantic-4.0.0/PKG-INFO` & `reasoner-pydantic-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.0.0
+Version: 4.0.1
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Kenneth Morton
 Author-email: kenny@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-4.0.0/README.md` & `reasoner-pydantic-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.0/reasoner_pydantic/__init__.py` & `reasoner-pydantic-4.0.1/reasoner_pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.0/reasoner_pydantic/auxgraphs.py` & `reasoner-pydantic-4.0.1/reasoner_pydantic/auxgraphs.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,26 +19,24 @@
         title = "auxiliary graph"
         extra = "allow"
 
 
 class AuxiliaryGraphs(BaseModel):
     """Auxiliary Graphs"""
 
-    __root__: Optional[HashableSet[AuxiliaryGraph]]
+    __root__: Optional[HashableMapping[str, AuxiliaryGraph]]
 
     class Config:
         title = "auxiliary graphs"
         extra = "allow"
 
-    def add(self, graph):
-        self.__root__.add(graph)
-
     def update(self, other):
         self.__root__.update(other.__root__)
 
     def parse_obj(obj):
         auxiliary_graphs = parse_obj_as(AuxiliaryGraphs, obj)
         graphs = AuxiliaryGraphs()
-        graphs.__root__ = HashableSet[AuxiliaryGraph]()
-        for graph in obj:
-            graphs.add(AuxiliaryGraph.parse_obj(graph))
-        return graphs.update(auxiliary_graphs)
+        graphs.__root__ = HashableMapping[str, AuxiliaryGraph]()
+        for id, graph in obj.items():
+            graphs.__root__[id] = AuxiliaryGraph.parse_obj(graph)
+        graphs.update(auxiliary_graphs)
+        return graphs
```

### Comparing `reasoner-pydantic-4.0.0/reasoner_pydantic/base_model.py` & `reasoner-pydantic-4.0.1/reasoner_pydantic/base_model.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.0/reasoner_pydantic/kgraph.py` & `reasoner-pydantic-4.0.1/reasoner_pydantic/kgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.0/reasoner_pydantic/message.py` & `reasoner-pydantic-4.0.1/reasoner_pydantic/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     )
     results: Optional[Results] = Field(
         None,
         title="list of results",
         nullable=True,
     )
     auxiliary_graphs: Optional[AuxiliaryGraphs] = Field(
-        None, title="list of auxiliary graphs", nullable=True
+        None, title="dict of auxiliary graphs", nullable=True
     )
 
     class Config:
         title = "message"
         extra = "forbid"
 
     def parse_obj(obj):
@@ -83,14 +83,19 @@
             # will handle concatenating properties when necessary.
             self.knowledge_graph.update(other.knowledge_graph)
         if other.results:
             if self.results:
                 self.results.update(other.results)
             else:
                 self.results = other.results
+        if other.auxiliary_graphs:
+            if self.auxiliary_graphs:
+                self.auxiliary_graphs.update(other.auxiliary_graphs)
+            else:
+                self.auxiliary_graphs = other.auxiliary_graphs
 
     def _normalize_kg_edge_ids(self):
         """
         Replace edge IDs with a hash of the edge object
         """
         self._update_kg_edge_ids(
             lambda edge: hashlib.blake2b(
@@ -112,30 +117,31 @@
             new_edge_id = update_func(edge)
 
             edge_id_mapping[edge_id] = new_edge_id
 
             # Update knowledge graph
             self.knowledge_graph.edges[new_edge_id] = edge
 
+        # Update auxiliary graphs
+        if self.auxiliary_graphs:
+            for auxiliary_graph in self.auxiliary_graphs.__root__.values():
+                if auxiliary_graph.edges:
+                    for aux_edge in auxiliary_graph.edges:
+                        auxiliary_graph.edges.discard(aux_edge)
+                        auxiliary_graph.edges.add(edge_id_mapping[aux_edge])
+
         # Update results
         if self.results:
             for result in self.results.__root__:
                 if result and result.analyses:
                     for analysis in result.analyses:
                         for edge_binding_list in analysis.edge_bindings.values():
                             for eb in edge_binding_list:
                                 eb.id = edge_id_mapping[eb.id]
 
-        # Update auxiliary graphs
-        if self.auxiliary_graphs:
-            for auxiliary_graph in self.auxiliary_graphs.__root__:
-                if auxiliary_graph.edges:
-                    for aux_edge in auxiliary_graph.edges:
-                        aux_edge = edge_id_mapping[aux_edge]
-
 
 class Query(BaseModel):
     """Request."""
 
     message: Message = Field(
         ...,
         title="message",
```

### Comparing `reasoner-pydantic-4.0.0/reasoner_pydantic/metakg.py` & `reasoner-pydantic-4.0.1/reasoner_pydantic/metakg.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.0/reasoner_pydantic/qgraph.py` & `reasoner-pydantic-4.0.1/reasoner_pydantic/qgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.0/reasoner_pydantic/results.py` & `reasoner-pydantic-4.0.1/reasoner_pydantic/results.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.0/reasoner_pydantic/shared.py` & `reasoner-pydantic-4.0.1/reasoner_pydantic/shared.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.0/reasoner_pydantic/utils.py` & `reasoner-pydantic-4.0.1/reasoner_pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.0/reasoner_pydantic/workflow.py` & `reasoner-pydantic-4.0.1/reasoner_pydantic/workflow.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.0/reasoner_pydantic.egg-info/PKG-INFO` & `reasoner-pydantic-4.0.1/reasoner_pydantic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.0.0
+Version: 4.0.1
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Kenneth Morton
 Author-email: kenny@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-4.0.0/reasoner_pydantic.egg-info/SOURCES.txt` & `reasoner-pydantic-4.0.1/reasoner_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.0/setup.py` & `reasoner-pydantic-4.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="reasoner-pydantic",
-    version="4.0.0",
+    version="4.0.1",
     author="Kenneth Morton",
     author_email="kenny@covar.com",
     url="https://github.com/TranslatorSRI/reasoner-pydantic",
     description="Pydantic models for the Reasoner API data formats",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["reasoner_pydantic"],
```

