# Comparing `tmp/dbis-er-diagram-1.0.6.tar.gz` & `tmp/dbis-er-diagram-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis-er-diagram-1.0.6.tar", last modified: Mon May  8 16:16:32 2023, max compression
+gzip compressed data, was "dbis-er-diagram-1.0.7.tar", last modified: Tue May  9 14:16:37 2023, max compression
```

## Comparing `dbis-er-diagram-1.0.6.tar` & `dbis-er-diagram-1.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-08 16:16:32.493008 dbis-er-diagram-1.0.6/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/LICENSE
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-05-08 16:16:32.493008 dbis-er-diagram-1.0.6/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15133 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/README.md
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-08 16:16:32.492008 dbis-er-diagram-1.0.6/dbis_er_diagram.egg-info/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-05-08 16:16:32.000000 dbis-er-diagram-1.0.6/dbis_er_diagram.egg-info/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      565 2023-05-08 16:16:32.000000 dbis-er-diagram-1.0.6/dbis_er_diagram.egg-info/SOURCES.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-05-08 16:16:32.000000 dbis-er-diagram-1.0.6/dbis_er_diagram.egg-info/dependency_links.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       48 2023-05-08 16:16:32.000000 dbis-er-diagram-1.0.6/dbis_er_diagram.egg-info/requires.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       10 2023-05-08 16:16:32.000000 dbis-er-diagram-1.0.6/dbis_er_diagram.egg-info/top_level.txt
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-08 16:16:32.493008 dbis-er-diagram-1.0.6/erdiagram/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      246 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/erdiagram/__init__.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7697 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/erdiagram/drawing.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    38914 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/erdiagram/er.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    30589 2023-05-08 16:14:48.000000 dbis-er-diagram-1.0.6/erdiagram/grading.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6591 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/erdiagram/merging.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      306 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/erdiagram/node_type.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      881 2023-05-08 16:14:48.000000 dbis-er-diagram-1.0.6/pyproject.toml
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-05-08 16:16:32.493008 dbis-er-diagram-1.0.6/setup.cfg
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-08 16:16:32.493008 dbis-er-diagram-1.0.6/tests/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     5117 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/tests/test_adders.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1728 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/tests/test_drawing.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11855 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/tests/test_getters.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1916 2023-05-04 14:27:55.000000 dbis-er-diagram-1.0.6/tests/test_grading_components.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7118 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/tests/test_grading_diagrams.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    10304 2023-05-08 16:14:48.000000 dbis-er-diagram-1.0.6/tests/test_grading_special_cases.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1148 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/tests/test_merging.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1035 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/tests/test_other_methods.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-09 14:16:37.567646 dbis-er-diagram-1.0.7/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/LICENSE
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-05-09 14:16:37.567646 dbis-er-diagram-1.0.7/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15133 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/README.md
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-09 14:16:37.555646 dbis-er-diagram-1.0.7/dbis_er_diagram.egg-info/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-05-09 14:16:37.000000 dbis-er-diagram-1.0.7/dbis_er_diagram.egg-info/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      565 2023-05-09 14:16:37.000000 dbis-er-diagram-1.0.7/dbis_er_diagram.egg-info/SOURCES.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-05-09 14:16:37.000000 dbis-er-diagram-1.0.7/dbis_er_diagram.egg-info/dependency_links.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       48 2023-05-09 14:16:37.000000 dbis-er-diagram-1.0.7/dbis_er_diagram.egg-info/requires.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       10 2023-05-09 14:16:37.000000 dbis-er-diagram-1.0.7/dbis_er_diagram.egg-info/top_level.txt
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-09 14:16:37.555646 dbis-er-diagram-1.0.7/erdiagram/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      246 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/erdiagram/__init__.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7697 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/erdiagram/drawing.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    38914 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/erdiagram/er.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    30923 2023-05-09 14:16:07.000000 dbis-er-diagram-1.0.7/erdiagram/grading.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6591 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/erdiagram/merging.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      306 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/erdiagram/node_type.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      881 2023-05-09 14:16:07.000000 dbis-er-diagram-1.0.7/pyproject.toml
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-05-09 14:16:37.567646 dbis-er-diagram-1.0.7/setup.cfg
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-09 14:16:37.567646 dbis-er-diagram-1.0.7/tests/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     5117 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/tests/test_adders.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1728 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/tests/test_drawing.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11855 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/tests/test_getters.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1916 2023-05-04 14:27:55.000000 dbis-er-diagram-1.0.7/tests/test_grading_components.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7118 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/tests/test_grading_diagrams.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11835 2023-05-09 14:16:07.000000 dbis-er-diagram-1.0.7/tests/test_grading_special_cases.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1148 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/tests/test_merging.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1035 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/tests/test_other_methods.py
```

### Comparing `dbis-er-diagram-1.0.6/LICENSE` & `dbis-er-diagram-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.6/PKG-INFO` & `dbis-er-diagram-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-er-diagram
-Version: 1.0.6
+Version: 1.0.7
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Michal Slupczynski <slupczynski@dbis.rwth-aachen.de>, Beyza Akyüz <beyza.akyuez@rwth-aachen.de>, Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-er-diagram
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-er-diagram-1.0.6/README.md` & `dbis-er-diagram-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.6/dbis_er_diagram.egg-info/PKG-INFO` & `dbis-er-diagram-1.0.7/dbis_er_diagram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-er-diagram
-Version: 1.0.6
+Version: 1.0.7
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Michal Slupczynski <slupczynski@dbis.rwth-aachen.de>, Beyza Akyüz <beyza.akyuez@rwth-aachen.de>, Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-er-diagram
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-er-diagram-1.0.6/dbis_er_diagram.egg-info/SOURCES.txt` & `dbis-er-diagram-1.0.7/dbis_er_diagram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.6/erdiagram/drawing.py` & `dbis-er-diagram-1.0.7/erdiagram/drawing.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.6/erdiagram/er.py` & `dbis-er-diagram-1.0.7/erdiagram/er.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.6/erdiagram/grading.py` & `dbis-er-diagram-1.0.7/erdiagram/grading.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,24 +301,28 @@
     )
     to_entities_solution = transform_dict_to_list(solution_relation["to_entities"])
     to_entities_submission = transform_dict_to_list(submission_relation["to_entities"])
 
     entities_solution = from_entities_solution + to_entities_solution
     entities_submission = from_entities_submission + to_entities_submission
 
+    # for each entity in either list, add a ID (so make it tuple(ID, entity))
+    entities_solution = [(i, entity) for i, entity in enumerate(entities_solution)]
+    entities_submission = [(i, entity) for i, entity in enumerate(entities_submission)]
+
     entity_pairs_dict = (
         list()
     )  # from solution entity find all possible submission entities
     for solution_entity in entities_solution:
         candidates = []
         for submission_entity in entities_submission:
             if (
                 ratio(
-                    sanitize(solution_entity["label"]),
-                    sanitize(submission_entity["label"]),
+                    sanitize(solution_entity[1]["label"]),
+                    sanitize(submission_entity[1]["label"]),
                 )
                 > 0.8
             ):
                 candidates.append(submission_entity)
         entity_pairs_dict.append((solution_entity, candidates))
 
     # sort above dictionary by length of value list, ascending, to a list of tuple(key, list)
@@ -388,66 +392,68 @@
         if solution_entity_is_weak != submission_entity_is_weak:
             score += scores["missing_relation_property"]
             log += f"\t✗ Relation '{original_solution_label}' should be connected to entity '{original_solution_entity_label}' {'weak' if solution_entity_is_weak else 'not weak'}, but is {'weak' if submission_entity_is_weak else 'not weak'}. ({scores['missing_relation_property']})\n"
 
         return ((score, log), cardinality_letter_map)
 
     def grade_all_relation_entity_pairs(
-        entity_pairs: list[tuple[dict[str, Any], list[dict[str, Any]]]],
-        already_matched_submission_entities: list[dict[str, Any]],
+        entity_pairs: list[
+            tuple[tuple[int, dict[str, Any]], list[tuple[int, dict[str, Any]]]]
+        ],
+        already_matched_submission_entities: list[int],
         cardinality_letter_map: dict[str, str],
     ) -> tuple[float, str]:
         entity_pairs = copy.deepcopy(entity_pairs)
         already_matched_submission_entities = copy.deepcopy(
             already_matched_submission_entities
         )
         score = 0.0
         log = ""
         cardinality_letter_map = copy.deepcopy(cardinality_letter_map)
 
         if len(entity_pairs) == 0:
             return (score, log)
 
         # pop first pair
-        solution_entity, submission_entities = entity_pairs.pop(0)
+        (_, solution_entity), submission_entities = entity_pairs.pop(0)
         original_solution_entity_label = solution_entity["label"]
 
         # remove alrady matched entities from submission_entities
         submission_entities = [
-            entity
-            for entity in submission_entities
-            if entity not in already_matched_submission_entities
+            (id, entity)
+            for id, entity in submission_entities
+            if id not in already_matched_submission_entities
         ]
 
         if len(submission_entities) == 0:
             score += scores["missing_relation_property"] * 3
             log += f"\t✗ Relation '{original_solution_label}' should have an entity '{original_solution_entity_label}'. ({scores['missing_relation_property'] * 3})\n"
             remaining_score, remaining_log = grade_all_relation_entity_pairs(
                 entity_pairs,
                 already_matched_submission_entities,
                 cardinality_letter_map,
             )
             return (score + remaining_score, log + remaining_log)
 
         branches = []
-        for submission_entity in submission_entities:
+        for submission_entity_id, submission_entity in submission_entities:
             branch = grade_relation_entity_pair(
                 solution_entity, submission_entity, cardinality_letter_map
             )
-            branches.append((branch, submission_entity))
+            branches.append((branch, submission_entity_id))
 
         # grade remaining entity pairs recursively
         graded_branches = []
         for (
             (current_score, current_log),
             current_cardinality_letter_map,
-        ), submission_entity in list(branches):
+        ), submission_entity_id in list(branches):
             remaining_score, remaining_log = grade_all_relation_entity_pairs(
                 entity_pairs,
-                already_matched_submission_entities + [submission_entity],
+                already_matched_submission_entities + [submission_entity_id],
                 current_cardinality_letter_map,
             )
             graded_branches.append(
                 (current_score + remaining_score, current_log + remaining_log)
             )
 
         # get best branch by min score
```

### Comparing `dbis-er-diagram-1.0.6/erdiagram/merging.py` & `dbis-er-diagram-1.0.7/erdiagram/merging.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.6/pyproject.toml` & `dbis-er-diagram-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbis-er-diagram"
-version = "1.0.6"
+version = "1.0.7"
 description = "RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
 authors = [
 	{ name = "Michal Slupczynski", email = "slupczynski@dbis.rwth-aachen.de" },
 	{ name = "Beyza Akyüz", email = "beyza.akyuez@rwth-aachen.de" },
 	{ name = "Til Mohr", email = "til.mohr@rwth-aachen.de" },
 ]
 readme = "README.md"
```

### Comparing `dbis-er-diagram-1.0.6/tests/test_adders.py` & `dbis-er-diagram-1.0.7/tests/test_adders.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.6/tests/test_drawing.py` & `dbis-er-diagram-1.0.7/tests/test_drawing.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.6/tests/test_getters.py` & `dbis-er-diagram-1.0.7/tests/test_getters.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.6/tests/test_grading_components.py` & `dbis-er-diagram-1.0.7/tests/test_grading_components.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.6/tests/test_grading_diagrams.py` & `dbis-er-diagram-1.0.7/tests/test_grading_diagrams.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.6/tests/test_grading_special_cases.py` & `dbis-er-diagram-1.0.7/tests/test_grading_special_cases.py`

 * *Files 17% similar despite different names*

```diff
@@ -232,7 +232,36 @@
     solution = ER()
     solution.add_relation({"A": "1"}, "R1", {"A": "m", "B": "n"})
     submission = ER()
     submission.add_relation({"A": "1"}, "R1", {"B": "n"})
 
     score, log = grade_submission(solution, submission)
     assert score > 0.0
+
+
+def test_self_relation_same_cardinality():
+    solution = ER()
+    solution.add_relation({"A": "1"}, "R1", {"A": "1"})
+    solution.add_relation({"B": "n"}, "R2", {"B": "n"})
+    solution.add_relation({"C": "(1,2)"}, "R3", {"C": "(1,2)"})
+    solution.add_relation({"D": "(1,n)"}, "R4", {"D": "(1,n)"})
+    solution.add_relation({"E": "(n,m)"}, "R5", {"E": "(n,m)"})
+    solution.add_relation({"F": "1"}, "R6", {"F": "1", "G": "n"})
+    solution.add_relation({"G": "n"}, "R7", {"F": "1", "G": "n"})
+    solution.add_relation({"H": "(1,2)"}, "R8", {"H": "(1,2)", "I": "(1,2)"})
+    solution.add_relation({"I": "(1,n)"}, "R9", {"H": "(1,n)", "I": "(1,n)"})
+    solution.add_relation({"J": "(n,m)"}, "R10", {"J": "(n,m)", "K": "(n,m)"})
+
+    submission = ER()
+    submission.add_relation({"A": "1"}, "R1", {"A": "1"})
+    submission.add_relation({"B": "n"}, "R2", {"B": "n"})
+    submission.add_relation({"C": "(1,2)"}, "R3", {"C": "(1,2)"})
+    submission.add_relation({"D": "(1,n)"}, "R4", {"D": "(1,n)"})
+    submission.add_relation({"E": "(n,m)"}, "R5", {"E": "(n,m)"})
+    submission.add_relation({"F": "1"}, "R6", {"F": "1", "G": "n"})
+    submission.add_relation({"G": "n"}, "R7", {"F": "1", "G": "n"})
+    submission.add_relation({"H": "(1,2)"}, "R8", {"H": "(1,2)", "I": "(1,2)"})
+    submission.add_relation({"I": "(1,n)"}, "R9", {"H": "(1,n)", "I": "(1,n)"})
+    submission.add_relation({"J": "(n,m)"}, "R10", {"J": "(n,m)", "K": "(n,m)"})
+
+    score, log = grade_submission(solution, submission)
+    assert score == 0.0
```

### Comparing `dbis-er-diagram-1.0.6/tests/test_merging.py` & `dbis-er-diagram-1.0.7/tests/test_merging.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.6/tests/test_other_methods.py` & `dbis-er-diagram-1.0.7/tests/test_other_methods.py`

 * *Files identical despite different names*

