# Comparing `tmp/magma_suite-1.2.2b1.tar.gz` & `tmp/magma_suite-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magma_suite-1.2.2b1.tar", max compression
+gzip compressed data, was "magma_suite-1.3.0.tar", max compression
```

## Comparing `magma_suite-1.2.2b1.tar` & `magma_suite-1.3.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     1083 2021-12-04 12:27:49.522554 magma_suite-1.2.2b1/LICENSE.txt
--rw-r--r--   0        0        0       96 2021-12-04 12:27:49.522647 magma_suite-1.2.2b1/README.md
--rw-r--r--   0        0        0        1 2021-12-04 12:27:49.524453 magma_suite-1.2.2b1/magma/__init__.py
--rw-r--r--   0        0        0     3444 2022-06-30 15:42:36.924381 magma_suite-1.2.2b1/magma/checkstatus.py
--rw-r--r--   0        0        0    12922 2022-06-30 15:42:36.925024 magma_suite-1.2.2b1/magma/inputgenerator.py
--rw-r--r--   0        0        0    15898 2023-02-23 21:12:29.226971 magma_suite-1.2.2b1/magma/metawfl.py
--rw-r--r--   0        0        0     8908 2022-06-30 15:42:36.926246 magma_suite-1.2.2b1/magma/metawflrun.py
--rw-r--r--   0        0        0     4087 2022-06-30 15:42:36.926668 magma_suite-1.2.2b1/magma/runupdate.py
--rw-r--r--   0        0        0        0 2021-12-04 12:27:49.525213 magma_suite-1.2.2b1/magma_ff/__init__.py
--rw-r--r--   0        0        0     2391 2022-07-28 17:12:25.211617 magma_suite-1.2.2b1/magma_ff/checkstatus.py
--rw-r--r--   0        0        0    45467 2023-04-20 19:52:37.302115 magma_suite-1.2.2b1/magma_ff/create_metawfr.py
--rw-r--r--   0        0        0     6670 2022-06-30 15:42:36.928302 magma_suite-1.2.2b1/magma_ff/import_metawfr.py
--rw-r--r--   0        0        0     5097 2022-06-30 15:42:36.928742 magma_suite-1.2.2b1/magma_ff/inputgenerator.py
--rw-r--r--   0        0        0      778 2021-12-04 12:27:49.525871 magma_suite-1.2.2b1/magma_ff/metawfl.py
--rw-r--r--   0        0        0     3162 2023-03-08 16:08:26.869788 magma_suite-1.2.2b1/magma_ff/metawflrun.py
--rw-r--r--   0        0        0     5032 2022-06-30 15:42:36.929823 magma_suite-1.2.2b1/magma_ff/parser.py
--rw-r--r--   0        0        0     6915 2022-06-30 15:42:36.930301 magma_suite-1.2.2b1/magma_ff/reset_metawfr.py
--rw-r--r--   0        0        0     2465 2022-06-30 15:42:36.930893 magma_suite-1.2.2b1/magma_ff/run_metawfr.py
--rw-r--r--   0        0        0       30 2021-12-04 12:27:49.526349 magma_suite-1.2.2b1/magma_ff/runupdate.py
--rw-r--r--   0        0        0     5650 2023-03-08 16:08:26.870983 magma_suite-1.2.2b1/magma_ff/status_metawfr.py
--rw-r--r--   0        0        0     1398 2022-06-30 15:42:36.931870 magma_suite-1.2.2b1/magma_ff/update_cost_metawfr.py
--rw-r--r--   0        0        0     3021 2023-04-20 19:52:37.303019 magma_suite-1.2.2b1/magma_ff/utils.py
--rw-r--r--   0        0        0     4066 2023-03-07 22:19:37.427723 magma_suite-1.2.2b1/magma_ff/wfrutils.py
--rw-r--r--   0        0        0      857 2023-04-20 20:14:08.561130 magma_suite-1.2.2b1/pyproject.toml
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 magma_suite-1.2.2b1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2021-12-04 12:27:49.522554 magma_suite-1.3.0/LICENSE.txt
+-rw-r--r--   0        0        0       96 2021-12-04 12:27:49.522647 magma_suite-1.3.0/README.md
+-rw-r--r--   0        0        0        1 2021-12-04 12:27:49.524453 magma_suite-1.3.0/magma/__init__.py
+-rw-r--r--   0        0        0     3444 2022-06-30 15:42:36.924381 magma_suite-1.3.0/magma/checkstatus.py
+-rw-r--r--   0        0        0    12922 2022-06-30 15:42:36.925024 magma_suite-1.3.0/magma/inputgenerator.py
+-rw-r--r--   0        0        0    15898 2023-02-23 21:12:29.226971 magma_suite-1.3.0/magma/metawfl.py
+-rw-r--r--   0        0        0     8908 2022-06-30 15:42:36.926246 magma_suite-1.3.0/magma/metawflrun.py
+-rw-r--r--   0        0        0     4087 2022-06-30 15:42:36.926668 magma_suite-1.3.0/magma/runupdate.py
+-rw-r--r--   0        0        0        0 2021-12-04 12:27:49.525213 magma_suite-1.3.0/magma_ff/__init__.py
+-rw-r--r--   0        0        0     2391 2022-07-28 17:12:25.211617 magma_suite-1.3.0/magma_ff/checkstatus.py
+-rw-r--r--   0        0        0        0 2023-05-04 18:15:38.867708 magma_suite-1.3.0/magma_ff/commands/__init__.py
+-rw-r--r--   0        0        0     1229 2023-05-04 18:15:38.867954 magma_suite-1.3.0/magma_ff/commands/create_meta_workflow_run.py
+-rw-r--r--   0        0        0    48727 2023-05-09 20:54:57.585987 magma_suite-1.3.0/magma_ff/create_metawfr.py
+-rw-r--r--   0        0        0     6670 2022-06-30 15:42:36.928302 magma_suite-1.3.0/magma_ff/import_metawfr.py
+-rw-r--r--   0        0        0     5097 2022-06-30 15:42:36.928742 magma_suite-1.3.0/magma_ff/inputgenerator.py
+-rw-r--r--   0        0        0      778 2021-12-04 12:27:49.525871 magma_suite-1.3.0/magma_ff/metawfl.py
+-rw-r--r--   0        0        0     3162 2023-03-08 16:08:26.869788 magma_suite-1.3.0/magma_ff/metawflrun.py
+-rw-r--r--   0        0        0     5032 2022-06-30 15:42:36.929823 magma_suite-1.3.0/magma_ff/parser.py
+-rw-r--r--   0        0        0     6915 2022-06-30 15:42:36.930301 magma_suite-1.3.0/magma_ff/reset_metawfr.py
+-rw-r--r--   0        0        0     2465 2022-06-30 15:42:36.930893 magma_suite-1.3.0/magma_ff/run_metawfr.py
+-rw-r--r--   0        0        0       30 2021-12-04 12:27:49.526349 magma_suite-1.3.0/magma_ff/runupdate.py
+-rw-r--r--   0        0        0     5650 2023-03-08 16:08:26.870983 magma_suite-1.3.0/magma_ff/status_metawfr.py
+-rw-r--r--   0        0        0     1398 2022-06-30 15:42:36.931870 magma_suite-1.3.0/magma_ff/update_cost_metawfr.py
+-rw-r--r--   0        0        0     3843 2023-05-04 18:15:38.868373 magma_suite-1.3.0/magma_ff/utils.py
+-rw-r--r--   0        0        0     4066 2023-03-07 22:19:37.427723 magma_suite-1.3.0/magma_ff/wfrutils.py
+-rw-r--r--   0        0        0      955 2023-05-09 20:54:57.586955 magma_suite-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 magma_suite-1.3.0/PKG-INFO
```

### Comparing `magma_suite-1.2.2b1/LICENSE.txt` & `magma_suite-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2b1/magma/checkstatus.py` & `magma_suite-1.3.0/magma/checkstatus.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2b1/magma/inputgenerator.py` & `magma_suite-1.3.0/magma/inputgenerator.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2b1/magma/metawfl.py` & `magma_suite-1.3.0/magma/metawfl.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2b1/magma/metawflrun.py` & `magma_suite-1.3.0/magma/metawflrun.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2b1/magma/runupdate.py` & `magma_suite-1.3.0/magma/runupdate.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2b1/magma_ff/checkstatus.py` & `magma_suite-1.3.0/magma_ff/checkstatus.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2b1/magma_ff/create_metawfr.py` & `magma_suite-1.3.0/magma_ff/create_metawfr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,135 @@
 #!/usr/bin/env python3
 
 ################################################
 #
 #   create_metawfr
 #
 ################################################
+from __future__ import annotations
 
-################################################
-#   Libraries
-################################################
 import datetime
 import json
 import uuid
+from typing import List
 
 from dcicutils import ff_utils
 
-# magma
 from magma_ff.metawfl import MetaWorkflow
 from magma_ff.metawflrun import MetaWorkflowRun
-from magma_ff.utils import make_embed_request
+from magma_ff.utils import JsonObject, keep_last_item, make_embed_request
 
 
 FILE_FORMAT = "file_format"
+SAMPLE_PROCESSING_TYPE = "SampleProcessing"
+SAMPLE_TYPE = "Sample"
+TYPE = "@type"
 UUID = "uuid"
 
 
-################################################
-#   MetaWorkflowRunCreationError
-################################################
+def create_meta_workflow_run(
+    item_identifier: str,
+    meta_workflow_identifier: str,
+    auth_key: JsonObject,
+    post: bool = True,
+    patch: bool = True,
+) -> JsonObject:
+    """Create a MetaWorkflowRun for the given item and MetaWorkflow.
+
+    POST MetaWorkflowRun and PATCH associated item as instructed.
+
+    :param item_identfier: Identifier (e.g. UUID, @id) for item from
+        which to create the MetaWorkflowRun
+    :param meta_workflow_identifier: Identifier for the MetaWorkflow
+        from which to create the MetaWorkflowRun
+    :param auth_key: Authorization keys for C4 account
+    :param post: Whether to POST the MetaWorkflowRun created
+    :param patch: Whether to PATCH the item given by the
+        item_identifier with the created MetaWorkflowRun
+    :returns: MetaWorkflowRun created
+    """
+    item = ff_utils.get_metadata(item_identifier, key=auth_key, add_on="frame=object")
+    if _is_item_of_type(SAMPLE_TYPE, item):
+        return create_meta_workflow_run_from_sample(
+            item_identifier, meta_workflow_identifier, auth_key, post=post, patch=patch
+        )
+    if _is_item_of_type(SAMPLE_PROCESSING_TYPE, item):
+        return create_meta_workflow_run_from_sample_processing(
+            item_identifier, meta_workflow_identifier, auth_key, post=post, patch=patch
+        )
+    raise MetaWorkflowRunCreationError(
+        f"No methods available to create MetaWorkflowRun for item of type(s):"
+        f" {_get_item_types(item)}"
+    )
+
+
+def _is_item_of_type(item_type: str, item: JsonObject) -> bool:
+    item_types = _get_item_types(item)
+    if item_type in item_types:
+        return True
+    return False
+
+
+def _get_item_types(item: JsonObject) -> List[str]:
+    return item.get(TYPE, [])
+
+
+def create_meta_workflow_run_from_sample(
+    sample_identifier: str,
+    meta_workflow_identifier: str,
+    auth_key: JsonObject,
+    post: bool = True,
+    patch: bool = True,
+) -> JsonObject:
+    return _create_meta_workflow_run(
+        MetaWorkflowRunFromSample,
+        sample_identifier,
+        meta_workflow_identifier,
+        auth_key,
+        post=post,
+        patch=patch,
+    )
+
+
+def create_meta_workflow_run_from_sample_processing(
+    sample_processing_identifier: str,
+    meta_workflow_identifier: str,
+    auth_key: JsonObject,
+    post: bool = True,
+    patch: bool = True,
+) -> JsonObject:
+    return _create_meta_workflow_run(
+        MetaWorkflowRunFromSampleProcessing,
+        sample_processing_identifier,
+        meta_workflow_identifier,
+        auth_key,
+        post=post,
+        patch=patch,
+    )
+
+
+def _create_meta_workflow_run(
+    meta_workflow_run_creator_class: MetaWorkflowRunFromItem,
+    item_identifier: str,
+    meta_workflow_identifier: str,
+    auth_key: JsonObject,
+    post: bool = True,
+    patch: bool = True,
+) -> JsonObject:
+    meta_workflow_run_creator = meta_workflow_run_creator_class(
+        item_identifier, meta_workflow_identifier, auth_key
+    )
+    if post:
+        if patch:
+            meta_workflow_run_creator.post_and_patch()
+        else:
+            meta_workflow_run_creator.post_meta_workflow_run()
+    return meta_workflow_run_creator.get_meta_workflow_run()
+
+
 class MetaWorkflowRunCreationError(Exception):
     """Custom exception for error tracking."""
 
 
 class MetaWorkflowRunFromItem:
     """Base class to hold common methods required to create/POST a
     MetaWorkflowRun and PATCH the Item used to create it.
@@ -95,14 +193,17 @@
         self.input_item_uuid = self.input_item.get(self.UUID)
         self.existing_meta_workflow_runs = self.input_item.get(
             self.META_WORKFLOW_RUNS, []
         )
         self.meta_workflow_run_uuid = str(uuid.uuid4())
         self.meta_workflow_run = {}  # Overwrite in child classes
 
+    def get_meta_workflow_run(self) -> JsonObject:
+        return self.meta_workflow_run
+
     def create_workflow_runs(self, meta_workflow_run):
         """Create shards and update MetaWorkflowRun[json].
 
         :param meta_workflow_run: MetaWorkflowRun[json]
         :type meta_workflow_run: dict
         :raises MetaWorkflowRunCreationError: If input files to
             MetaWorkflowRun cannot be identified
@@ -125,15 +226,14 @@
             reformatted_file_input
         )
         meta_workflow_run[self.WORKFLOW_RUNS] = run_with_workflows[self.WORKFLOW_RUNS]
 
     def get_item_properties(self, item_identifier):
         """Retrieve item from given environment without raising
         exception if not found.
-
         :param item_identifier: Item identifier on the portal
         :type item_identifier: str
         :return: Raw view of item if found
         :rtype: dict or None
         """
         try:
             result = ff_utils.get_metadata(
@@ -1135,15 +1235,16 @@
     def input_crams(self):
         """CRAM file input."""
         return [self.get_submitted_files_for_file_format(self.CRAM_FORMAT)]
 
     @property
     def input_gvcfs(self):
         """gVCF file input."""
-        return [self.get_processed_files_for_file_format(self.GVCF_FORMAT)]
+        gvcfs = self.get_processed_files_for_file_format(self.GVCF_FORMAT)
+        return [keep_last_item(gvcfs)]
 
     @property
     def fastqs_r1(self):
         """FASTQ paired-end 1 file input."""
         return [self.get_fastqs_for_paired_end(self.PAIRED_END_1)]
 
     @property
@@ -1162,15 +1263,16 @@
             if file_format == self.FASTQ_FORMAT:
                 result.append(file_uuid)
         return [result]
 
     @property
     def input_bams(self):
         """BAM file input."""
-        return [self.get_processed_files_for_file_format(self.BAM_FORMAT)]
+        bams = self.get_processed_files_for_file_format(self.BAM_FORMAT)
+        return [keep_last_item(bams)]
 
     @property
     def rcktar_file_names(self):
         """Name for created RckTar files input."""
         return [
             sample_name + self.RCKTAR_FILE_ENDING for sample_name in self.sample_names
         ]
```

### Comparing `magma_suite-1.2.2b1/magma_ff/import_metawfr.py` & `magma_suite-1.3.0/magma_ff/import_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2b1/magma_ff/inputgenerator.py` & `magma_suite-1.3.0/magma_ff/inputgenerator.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2b1/magma_ff/metawfl.py` & `magma_suite-1.3.0/magma_ff/metawfl.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2b1/magma_ff/metawflrun.py` & `magma_suite-1.3.0/magma_ff/metawflrun.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2b1/magma_ff/parser.py` & `magma_suite-1.3.0/magma_ff/parser.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2b1/magma_ff/reset_metawfr.py` & `magma_suite-1.3.0/magma_ff/reset_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2b1/magma_ff/run_metawfr.py` & `magma_suite-1.3.0/magma_ff/run_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2b1/magma_ff/status_metawfr.py` & `magma_suite-1.3.0/magma_ff/status_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2b1/magma_ff/update_cost_metawfr.py` & `magma_suite-1.3.0/magma_ff/update_cost_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2b1/magma_ff/wfrutils.py` & `magma_suite-1.3.0/magma_ff/wfrutils.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.2.2b1/pyproject.toml` & `magma_suite-1.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magma-suite"
-version = "1.2.2-b1"
+version = "1.3.0"
 description = "Collection of tools to manage meta-workflows automation."
 authors = ["Michele Berselli <berselli.michele@gmail.com>", "Doug Rioux", "Soo Lee", "CGAP team"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbmi-bgm/magma"
 homepage = "https://github.com/dbmi-bgm/magma"
 classifiers = [
@@ -26,10 +26,14 @@
 
 
 [tool.poetry.dev-dependencies]
 mock = "*"
 pytest = "*"
 
 
+[tool.poetry.scripts]
+create-meta-workflow-run = "magma_ff.commands.create_meta_workflow_run:main"
+
+
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `magma_suite-1.2.2b1/PKG-INFO` & `magma_suite-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magma-suite
-Version: 1.2.2b1
+Version: 1.3.0
 Summary: Collection of tools to manage meta-workflows automation.
 Home-page: https://github.com/dbmi-bgm/magma
 License: MIT
 Author: Michele Berselli
 Author-email: berselli.michele@gmail.com
 Requires-Python: >=3.7,<3.9
 Classifier: License :: OSI Approved :: MIT License
```

