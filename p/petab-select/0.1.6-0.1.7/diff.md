# Comparing `tmp/petab_select-0.1.6.tar.gz` & `tmp/petab_select-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petab_select-0.1.6.tar", last modified: Tue May  9 10:57:11 2023, max compression
+gzip compressed data, was "petab_select-0.1.7.tar", last modified: Tue May  9 18:46:03 2023, max compression
```

## Comparing `petab_select-0.1.6.tar` & `petab_select-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-05-09 10:57:11.921579 petab_select-0.1.6/
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     1602 2021-08-31 13:20:42.000000 petab_select-0.1.6/LICENSE
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-05-09 10:57:11.917579 petab_select-0.1.6/PKG-INFO
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     9256 2023-04-13 16:12:57.000000 petab_select-0.1.6/README.md
-drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-05-09 10:57:11.917579 petab_select-0.1.6/petab_select/
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      263 2023-04-13 08:28:52.000000 petab_select-0.1.6/petab_select/__init__.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    51676 2022-09-30 16:40:04.000000 petab_select-0.1.6/petab_select/candidate_space.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    13247 2022-09-30 16:40:04.000000 petab_select-0.1.6/petab_select/cli.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     4460 2022-09-30 16:40:04.000000 petab_select-0.1.6/petab_select/constants.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     7225 2022-09-30 16:40:04.000000 petab_select-0.1.6/petab_select/criteria.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2443 2021-11-02 20:14:39.000000 petab_select-0.1.6/petab_select/descriptors.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     1076 2022-09-30 16:40:04.000000 petab_select-0.1.6/petab_select/handlers.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2438 2022-09-30 16:40:04.000000 petab_select-0.1.6/petab_select/misc.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    25976 2023-05-09 10:52:56.000000 petab_select-0.1.6/petab_select/model.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    11415 2022-09-30 16:40:04.000000 petab_select-0.1.6/petab_select/model_space.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    38364 2022-09-30 16:40:04.000000 petab_select-0.1.6/petab_select/model_subspace.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2254 2022-09-30 16:40:04.000000 petab_select-0.1.6/petab_select/petab.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     8571 2023-04-13 08:28:52.000000 petab_select-0.1.6/petab_select/problem.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    10109 2023-04-13 16:12:57.000000 petab_select-0.1.6/petab_select/ui.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      295 2021-11-03 18:08:02.000000 petab_select-0.1.6/petab_select/validators.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       80 2023-05-09 10:56:44.000000 petab_select-0.1.6/petab_select/version.py
-drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-05-09 10:57:11.917579 petab_select-0.1.6/petab_select.egg-info/
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-05-09 10:57:11.000000 petab_select-0.1.6/petab_select.egg-info/PKG-INFO
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      658 2023-05-09 10:57:11.000000 petab_select-0.1.6/petab_select.egg-info/SOURCES.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)        1 2023-05-09 10:57:11.000000 petab_select-0.1.6/petab_select.egg-info/dependency_links.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       54 2023-05-09 10:57:11.000000 petab_select-0.1.6/petab_select.egg-info/entry_points.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      136 2023-05-09 10:57:11.000000 petab_select-0.1.6/petab_select.egg-info/requires.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       13 2023-05-09 10:57:11.000000 petab_select-0.1.6/petab_select.egg-info/top_level.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      281 2022-09-30 16:40:04.000000 petab_select-0.1.6/pyproject.toml
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       38 2023-05-09 10:57:11.921579 petab_select-0.1.6/setup.cfg
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2961 2023-04-13 16:12:57.000000 petab_select-0.1.6/setup.py
+drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-05-09 18:46:03.076553 petab_select-0.1.7/
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     1602 2021-08-31 13:20:42.000000 petab_select-0.1.7/LICENSE
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-05-09 18:46:03.076553 petab_select-0.1.7/PKG-INFO
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     9256 2023-04-13 16:12:57.000000 petab_select-0.1.7/README.md
+drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-05-09 18:46:03.076553 petab_select-0.1.7/petab_select/
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      263 2023-04-13 08:28:52.000000 petab_select-0.1.7/petab_select/__init__.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    51673 2023-05-09 18:43:32.000000 petab_select-0.1.7/petab_select/candidate_space.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    13247 2022-09-30 16:40:04.000000 petab_select-0.1.7/petab_select/cli.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     4460 2022-09-30 16:40:04.000000 petab_select-0.1.7/petab_select/constants.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     7225 2022-09-30 16:40:04.000000 petab_select-0.1.7/petab_select/criteria.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2443 2021-11-02 20:14:39.000000 petab_select-0.1.7/petab_select/descriptors.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     1076 2022-09-30 16:40:04.000000 petab_select-0.1.7/petab_select/handlers.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2438 2022-09-30 16:40:04.000000 petab_select-0.1.7/petab_select/misc.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    25976 2023-05-09 10:52:56.000000 petab_select-0.1.7/petab_select/model.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    11415 2022-09-30 16:40:04.000000 petab_select-0.1.7/petab_select/model_space.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    38364 2022-09-30 16:40:04.000000 petab_select-0.1.7/petab_select/model_subspace.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2254 2022-09-30 16:40:04.000000 petab_select-0.1.7/petab_select/petab.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     8571 2023-04-13 08:28:52.000000 petab_select-0.1.7/petab_select/problem.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    10246 2023-05-09 18:43:32.000000 petab_select-0.1.7/petab_select/ui.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      295 2021-11-03 18:08:02.000000 petab_select-0.1.7/petab_select/validators.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       80 2023-05-09 18:45:22.000000 petab_select-0.1.7/petab_select/version.py
+drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-05-09 18:46:03.076553 petab_select-0.1.7/petab_select.egg-info/
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-05-09 18:46:03.000000 petab_select-0.1.7/petab_select.egg-info/PKG-INFO
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      658 2023-05-09 18:46:03.000000 petab_select-0.1.7/petab_select.egg-info/SOURCES.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)        1 2023-05-09 18:46:03.000000 petab_select-0.1.7/petab_select.egg-info/dependency_links.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       54 2023-05-09 18:46:03.000000 petab_select-0.1.7/petab_select.egg-info/entry_points.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      136 2023-05-09 18:46:03.000000 petab_select-0.1.7/petab_select.egg-info/requires.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       13 2023-05-09 18:46:03.000000 petab_select-0.1.7/petab_select.egg-info/top_level.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      281 2022-09-30 16:40:04.000000 petab_select-0.1.7/pyproject.toml
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       38 2023-05-09 18:46:03.076553 petab_select-0.1.7/setup.cfg
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2961 2023-04-13 16:12:57.000000 petab_select-0.1.7/setup.py
```

### Comparing `petab_select-0.1.6/LICENSE` & `petab_select-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.6/PKG-INFO` & `petab_select-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petab_select
-Version: 0.1.6
+Version: 0.1.7
 Summary: PEtab Select: an extension to PEtab for model selection.
 Home-page: https://github.com/PEtab-dev/petab_select
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `petab_select-0.1.6/README.md` & `petab_select-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.6/petab_select/candidate_space.py` & `petab_select-0.1.7/petab_select/candidate_space.py`

 * *Files 0% similar despite different names*

```diff
@@ -1090,15 +1090,15 @@
                 if len(critical_set) > 1
             ]
             and not self.swap_parameter_sets
         ):
             if self.n_reattempts:
                 self.jump_to_most_distant(calibrated_models=calibrated_models)
                 return
-            raise StopIteration(
+            raise ValueError(
                 f"The next method is {next_method}, but there are no critical or swap parameters sets. Terminating."
             )
         if previous_method == Method.LATERAL:
             self.swap_done_successfully = False
         self.update_method(method=next_method)
 
     def update_method(self, method: Method):
```

### Comparing `petab_select-0.1.6/petab_select/cli.py` & `petab_select-0.1.7/petab_select/cli.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.6/petab_select/constants.py` & `petab_select-0.1.7/petab_select/constants.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.6/petab_select/criteria.py` & `petab_select-0.1.7/petab_select/criteria.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.6/petab_select/descriptors.py` & `petab_select-0.1.7/petab_select/descriptors.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.6/petab_select/handlers.py` & `petab_select-0.1.7/petab_select/handlers.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.6/petab_select/misc.py` & `petab_select-0.1.7/petab_select/misc.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.6/petab_select/model.py` & `petab_select-0.1.7/petab_select/model.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.6/petab_select/model_space.py` & `petab_select-0.1.7/petab_select/model_space.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.6/petab_select/model_subspace.py` & `petab_select-0.1.7/petab_select/model_subspace.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.6/petab_select/petab.py` & `petab_select-0.1.7/petab_select/petab.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.6/petab_select/problem.py` & `petab_select-0.1.7/petab_select/problem.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.6/petab_select/ui.py` & `petab_select-0.1.7/petab_select/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         criterion:
             The criterion by which models will be compared. Defaults to the criterion
             defined in the PEtab Select problem.
 
     Returns:
         The candidate space, which contains the candidate models.
     """
+    do_search = True
     # FIXME might be difficult for a CLI tool to specify a specific predecessor
     #       model if their candidate space has models. Need a way to empty
     #       the candidate space of models... might be difficult with pickled
     #       candidate space objects/arguments?
     if excluded_models is None:
         excluded_models = []
     if excluded_model_hashes is None:
@@ -104,19 +105,23 @@
         if not default_compare(
             model0=previous_predecessor_model,
             model1=predecessor_model,
             criterion=criterion,
         ):
             predecessor_model = previous_predecessor_model
 
-        candidate_space.update_after_calibration(
-            calibrated_models=calibrated_models,
-            newly_calibrated_models=newly_calibrated_models,
-            criterion=criterion,
-        )
+        try:
+            candidate_space.update_after_calibration(
+                calibrated_models=calibrated_models,
+                newly_calibrated_models=newly_calibrated_models,
+                criterion=criterion,
+            )
+        except StopIteration:
+            do_search = False
+
         # If candidate space not Famos then ignored.
         # Else, in case we jumped to most distant in this iteration, go into
         # calibration with only the model we've jumped to.
         if (
             candidate_space.governing_method == Method.FAMOS
             and candidate_space.jumped_to_most_distant
         ):
@@ -138,15 +143,16 @@
     #      - duplicate model IDs among multiple model subspaces
     #      - perhaps less portable if model IDs are generated differently on different
     #        computers
     problem.model_space.exclude_models(models=excluded_models)
     problem.model_space.exclude_model_hashes(
         model_hashes=excluded_model_hashes
     )
-    problem.model_space.search(candidate_space, limit=limit_sent)
+    if do_search:
+        problem.model_space.search(candidate_space, limit=limit_sent)
 
     write_summary_tsv(
         problem=problem,
         candidate_space=candidate_space,
         previous_predecessor_model=previous_predecessor_model,
         predecessor_model=predecessor_model,
     )
```

### Comparing `petab_select-0.1.6/petab_select.egg-info/PKG-INFO` & `petab_select-0.1.7/petab_select.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petab-select
-Version: 0.1.6
+Version: 0.1.7
 Summary: PEtab Select: an extension to PEtab for model selection.
 Home-page: https://github.com/PEtab-dev/petab_select
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `petab_select-0.1.6/petab_select.egg-info/SOURCES.txt` & `petab_select-0.1.7/petab_select.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.6/setup.py` & `petab_select-0.1.7/setup.py`

 * *Files identical despite different names*

