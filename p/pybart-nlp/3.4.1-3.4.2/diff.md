# Comparing `tmp/pybart-nlp-3.4.1.tar.gz` & `tmp/pybart-nlp-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybart-nlp-3.4.1.tar", last modified: Sun Jan  1 16:26:39 2023, max compression
+gzip compressed data, was "pybart-nlp-3.4.2.tar", last modified: Tue May  9 11:02:37 2023, max compression
```

## Comparing `pybart-nlp-3.4.1.tar` & `pybart-nlp-3.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 16:26:39.661992 pybart-nlp-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-01-01 16:26:28.000000 pybart-nlp-3.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-01-01 16:26:39.661992 pybart-nlp-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-01-01 16:26:28.000000 pybart-nlp-3.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 16:26:39.661992 pybart-nlp-3.4.1/pybart/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-01 16:26:28.000000 pybart-nlp-3.4.1/pybart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-01-01 16:26:28.000000 pybart-nlp-3.4.1/pybart/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-01-01 16:26:28.000000 pybart-nlp-3.4.1/pybart/conllu_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-01-01 16:26:28.000000 pybart-nlp-3.4.1/pybart/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    89928 2023-01-01 16:26:28.000000 pybart-nlp-3.4.1/pybart/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-01-01 16:26:28.000000 pybart-nlp-3.4.1/pybart/graph_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    17717 2023-01-01 16:26:28.000000 pybart-nlp-3.4.1/pybart/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-01-01 16:26:28.000000 pybart-nlp-3.4.1/pybart/spacy_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 16:26:39.661992 pybart-nlp-3.4.1/pybart_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-01-01 16:26:39.000000 pybart-nlp-3.4.1/pybart_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-01-01 16:26:39.000000 pybart-nlp-3.4.1/pybart_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-01 16:26:39.000000 pybart-nlp-3.4.1/pybart_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-01 16:26:39.000000 pybart-nlp-3.4.1/pybart_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-01 16:26:39.661992 pybart-nlp-3.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-01-01 16:26:28.000000 pybart-nlp-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:02:37.606593 pybart-nlp-3.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-09 11:02:21.000000 pybart-nlp-3.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-05-09 11:02:37.606593 pybart-nlp-3.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-05-09 11:02:21.000000 pybart-nlp-3.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:02:37.606593 pybart-nlp-3.4.2/pybart/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 11:02:21.000000 pybart-nlp-3.4.2/pybart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-05-09 11:02:21.000000 pybart-nlp-3.4.2/pybart/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-05-09 11:02:21.000000 pybart-nlp-3.4.2/pybart/conllu_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-05-09 11:02:21.000000 pybart-nlp-3.4.2/pybart/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90101 2023-05-09 11:02:21.000000 pybart-nlp-3.4.2/pybart/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-05-09 11:02:21.000000 pybart-nlp-3.4.2/pybart/graph_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17717 2023-05-09 11:02:21.000000 pybart-nlp-3.4.2/pybart/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-05-09 11:02:21.000000 pybart-nlp-3.4.2/pybart/spacy_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:02:37.606593 pybart-nlp-3.4.2/pybart_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-05-09 11:02:37.000000 pybart-nlp-3.4.2/pybart_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-09 11:02:37.000000 pybart-nlp-3.4.2/pybart_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:02:37.000000 pybart-nlp-3.4.2/pybart_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 11:02:37.000000 pybart-nlp-3.4.2/pybart_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 11:02:37.606593 pybart-nlp-3.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-09 11:02:21.000000 pybart-nlp-3.4.2/setup.py
```

### Comparing `pybart-nlp-3.4.1/LICENSE` & `pybart-nlp-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.1/PKG-INFO` & `pybart-nlp-3.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybart-nlp
-Version: 3.4.1
+Version: 3.4.2
 Summary: python converter from UD-tree to BART-graph representations
 Home-page: https://github.com/allenai/pybart
 Author: Aryeh Tiktinsky
 Author-email: aryehgigi@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pybart-nlp Version: 3.4.1 Summary: python converter
+Metadata-Version: 2.1 Name: pybart-nlp Version: 3.4.2 Summary: python converter
 from UD-tree to BART-graph representations Home-page: https://github.com/
 allenai/pybart Author: Aryeh Tiktinsky Author-email: aryehgigi@gmail.com
 Classifier: Programming Language :: Python :: 3.7 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7, <3.12 Description-Content-Type: text/
 markdown License-File: LICENSE ![CI](https://github.com/allenai/pybart/actions/
 workflows/ci.yml/badge.svg)
```

### Comparing `pybart-nlp-3.4.1/README.md` & `pybart-nlp-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.1/pybart/api.py` & `pybart-nlp-3.4.2/pybart/api.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.1/pybart/conllu_wrapper.py` & `pybart-nlp-3.4.2/pybart/conllu_wrapper.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.1/pybart/constraints.py` & `pybart-nlp-3.4.2/pybart/constraints.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.1/pybart/converter.py` & `pybart-nlp-3.4.2/pybart/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,16 +320,19 @@
     #   There is no nsubj of asking, but the dobj, SEC, is the extra nsubj of require.
     #   Similarly, "The law tells them when to do so"
     #   Instead of nsubj(do, law) we want nsubj(do, them)
     extra_xcomp_propagation_no_to_constraint = Full(
         tokens=[
             Token(id="gov"),
             Token(id="new_subj"),
-            Token(id="xcomp", spec=[Field(field=FieldNames.TAG, value=verb_pos + ["TO", "IN"])],
-                  outgoing_edges=[HasNoLabel(subj) for subj in subj_options] + [HasNoLabel("mark"), HasNoLabel("aux")]),
+            Token(
+                id="xcomp",
+                spec=[Field(field=FieldNames.WORD, value=["using"], in_sequence=False), Field(field=FieldNames.TAG, value=verb_pos + ["TO", "IN"])],
+                outgoing_edges=[HasNoLabel(subj) for subj in subj_options] + [HasNoLabel("mark"), HasNoLabel("aux")]
+            ),
         ],
         edges=[
             Edge(child="xcomp", parent="gov", label=[HasLabelFromList(["xcomp"])]),
             Edge(child="new_subj", parent="gov", label=[HasLabelFromList(subj_options + obj_options)]),
         ],
     )
 
@@ -502,15 +505,15 @@
 
     def extra_compound_propagation(sentence, matches, converter):
         for cur_match in matches:
             gov = cur_match.token("gov")
             compound = cur_match.token("compound")
             middle_man = cur_match.token("middle_man")
             for rel in cur_match.edge(middle_man, gov):
-                sentence[compound].add_edge(Label(rel, src="compound", src_type="NULL", uncertain=True), sentence[gov])
+                sentence[compound].add_edge(Label(f"{rel}c", src="compound", src_type="NULL", uncertain=True), sentence[gov])
 
     # here we add a subject relation for each amod relation (but in the opposite direction)
     extra_amod_propagation_constraint = Full(
         tokens=[
             Token(id="gov"),
             Token(id="amod", outgoing_edges=[HasNoLabel(arg) for arg in subj_options]),
         ],
@@ -551,28 +554,28 @@
             to = sentence[cur_match.token("to")]
             subj.add_edge(Label("nsubj", src="acl", src_type="NULL", phrase=to.get_conllu_field("form")), acl)
 
 
     # acl part2: take care of all acl's (not acl:relcl) that are not marked by 'to'
     extra_acl_propagation_constraint = Full(
         tokens=[
-            Token(id="father", spec=[Field(FieldNames.TAG, pron_pos + noun_pos)],
-                  incoming_edges=[HasNoLabel(subj_cur) for subj_cur in subj_options + ["mark"]]),
+            Token(id="father", spec=[Field(FieldNames.TAG, pron_pos + noun_pos)]),
             Token(id="acl", spec=[Field(FieldNames.TAG, verb_pos)], outgoing_edges=[HasNoLabel(subj_cur) for subj_cur in subj_options]),
         ],
         edges=[
             Edge(child="acl", parent="father", label=[HasLabelFromList(["acl"])]),
         ],
     )
 
     def extra_acl_propagation(sentence, matches, converter):
         for cur_match in matches:
             father = sentence[cur_match.token("father")]
             acl = sentence[cur_match.token("acl")]
-            father.add_edge(Label("nsubj", src="acl", src_type="NULL", phrase="REDUCED"), acl)
+            if all((r.base not in subj_options) or (r.eud is not None or r.src is not None) for _, rels in father.get_new_relations() for r in rels):
+                father.add_edge(Label("nsubj", src="acl", src_type="NULL", phrase="REDUCED"), acl)
 
     extra_subj_obj_nmod_propagation_of_nmods_constraint = Full(
         tokens=[
             Token(id="receiver"),
             Token(id="mediator", spec=[Field(FieldNames.TAG, noun_pos + pron_pos)]),
             Token(id="modifier"),
             Token(id="specifier", spec=[Field(FieldNames.WORD, ["like", "such", "including", "כמו", "כגון", "כדוגמת", "כולל"])]),  # TODO: english = like/such/including
```

### Comparing `pybart-nlp-3.4.1/pybart/graph_token.py` & `pybart-nlp-3.4.2/pybart/graph_token.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.1/pybart/matcher.py` & `pybart-nlp-3.4.2/pybart/matcher.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.1/pybart/spacy_wrapper.py` & `pybart-nlp-3.4.2/pybart/spacy_wrapper.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.1/pybart_nlp.egg-info/PKG-INFO` & `pybart-nlp-3.4.2/pybart_nlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybart-nlp
-Version: 3.4.1
+Version: 3.4.2
 Summary: python converter from UD-tree to BART-graph representations
 Home-page: https://github.com/allenai/pybart
 Author: Aryeh Tiktinsky
 Author-email: aryehgigi@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pybart-nlp Version: 3.4.1 Summary: python converter
+Metadata-Version: 2.1 Name: pybart-nlp Version: 3.4.2 Summary: python converter
 from UD-tree to BART-graph representations Home-page: https://github.com/
 allenai/pybart Author: Aryeh Tiktinsky Author-email: aryehgigi@gmail.com
 Classifier: Programming Language :: Python :: 3.7 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7, <3.12 Description-Content-Type: text/
 markdown License-File: LICENSE ![CI](https://github.com/allenai/pybart/actions/
 workflows/ci.yml/badge.svg)
```

### Comparing `pybart-nlp-3.4.1/setup.py` & `pybart-nlp-3.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pybart-nlp",
-    version="3.4.1",
+    version="3.4.2",
     author="Aryeh Tiktinsky",
     author_email="aryehgigi@gmail.com",
     description="python converter from UD-tree to BART-graph representations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/allenai/pybart",
     packages=setuptools.find_packages(),
```

