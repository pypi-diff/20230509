# Comparing `tmp/encord-0.1.74.tar.gz` & `tmp/encord-0.1.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encord-0.1.74.tar", max compression
+gzip compressed data, was "encord-0.1.75.tar", max compression
```

## Comparing `encord-0.1.74.tar` & `encord-0.1.75.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0    11330 2023-04-28 14:21:09.197584 encord-0.1.74/LICENSE
--rw-r--r--   0        0        0     2595 2023-04-28 14:21:09.197584 encord-0.1.74/README.md
--rw-r--r--   0        0        0       84 2023-04-28 14:21:09.197584 encord-0.1.74/cord/__init__.py
--rw-r--r--   0        0        0      158 2023-04-28 14:21:09.213585 encord-0.1.74/encord/__init__.py
--rw-r--r--   0        0        0      214 2023-04-28 14:21:09.213585 encord-0.1.74/encord/_version.py
--rw-r--r--   0        0        0    47245 2023-04-28 14:21:09.213585 encord-0.1.74/encord/client.py
--rw-r--r--   0        0        0    10825 2023-04-28 14:21:09.213585 encord-0.1.74/encord/configs.py
--rw-r--r--   0        0        0        0 2023-04-28 14:21:09.213585 encord-0.1.74/encord/constants/__init__.py
--rw-r--r--   0        0        0      810 2023-04-28 14:21:09.213585 encord-0.1.74/encord/constants/enums.py
--rw-r--r--   0        0        0     3211 2023-04-28 14:21:09.213585 encord-0.1.74/encord/constants/model.py
--rw-r--r--   0        0        0     6068 2023-04-28 14:21:09.213585 encord-0.1.74/encord/constants/model_weights.py
--rw-r--r--   0        0        0     1119 2023-04-28 14:21:09.213585 encord-0.1.74/encord/constants/string_constants.py
--rw-r--r--   0        0        0        0 2023-04-28 14:21:09.213585 encord-0.1.74/encord/constants/test/__init__.py
--rw-r--r--   0        0        0      634 2023-04-28 14:21:09.213585 encord-0.1.74/encord/constants/test/test_enums.py
--rw-r--r--   0        0        0    16035 2023-04-28 14:21:09.213585 encord-0.1.74/encord/dataset.py
--rw-r--r--   0        0        0     5621 2023-04-28 14:21:09.213585 encord-0.1.74/encord/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-28 14:21:09.213585 encord-0.1.74/encord/http/__init__.py
--rw-r--r--   0        0        0      535 2023-04-28 14:21:09.213585 encord-0.1.74/encord/http/constants.py
--rw-r--r--   0        0        0     6275 2023-04-28 14:21:09.213585 encord-0.1.74/encord/http/error_utils.py
--rw-r--r--   0        0        0     5999 2023-04-28 14:21:09.213585 encord-0.1.74/encord/http/querier.py
--rw-r--r--   0        0        0      697 2023-04-28 14:21:09.213585 encord-0.1.74/encord/http/query_methods.py
--rw-r--r--   0        0        0     1691 2023-04-28 14:21:09.213585 encord-0.1.74/encord/http/request.py
--rw-r--r--   0        0        0     5880 2023-04-28 14:21:09.213585 encord-0.1.74/encord/http/utils.py
--rw-r--r--   0        0        0      340 2023-04-28 14:21:09.213585 encord-0.1.74/encord/objects/__init__.py
--rw-r--r--   0        0        0      145 2023-04-28 14:21:09.213585 encord-0.1.74/encord/objects/classification.py
--rw-r--r--   0        0        0    29709 2023-04-28 14:21:09.213585 encord-0.1.74/encord/objects/common.py
--rw-r--r--   0        0        0      172 2023-04-28 14:21:09.213585 encord-0.1.74/encord/objects/constants.py
--rw-r--r--   0        0        0     5631 2023-04-28 14:21:09.213585 encord-0.1.74/encord/objects/coordinates.py
--rw-r--r--   0        0        0     3419 2023-04-28 14:21:09.213585 encord-0.1.74/encord/objects/frames.py
--rw-r--r--   0        0        0    21407 2023-04-28 14:21:09.217585 encord-0.1.74/encord/objects/internal_helpers.py
--rw-r--r--   0        0        0   132977 2023-04-28 14:21:09.217585 encord-0.1.74/encord/objects/ontology_labels_impl.py
--rw-r--r--   0        0        0      137 2023-04-28 14:21:09.217585 encord-0.1.74/encord/objects/ontology_object.py
--rw-r--r--   0        0        0      148 2023-04-28 14:21:09.217585 encord-0.1.74/encord/objects/ontology_structure.py
--rw-r--r--   0        0        0      549 2023-04-28 14:21:09.217585 encord-0.1.74/encord/objects/project.py
--rw-r--r--   0        0        0     1240 2023-04-28 14:21:09.217585 encord-0.1.74/encord/objects/utils.py
--rw-r--r--   0        0        0     3430 2023-04-28 14:21:09.217585 encord-0.1.74/encord/ontology.py
--rw-r--r--   0        0        0        0 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/__init__.py
--rw-r--r--   0        0        0      982 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/api_key.py
--rw-r--r--   0        0        0     5377 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/base_orm.py
--rw-r--r--   0        0        0      111 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/cloud_integration.py
--rw-r--r--   0        0        0    32206 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/dataset.py
--rw-r--r--   0        0        0      828 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/dataset_with_user_role.py
--rw-r--r--   0        0        0      201 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/formatter.py
--rw-r--r--   0        0        0     1155 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/label_log.py
--rw-r--r--   0        0        0    11122 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/label_row.py
--rw-r--r--   0        0        0     1577 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/labeling_algorithm.py
--rw-r--r--   0        0        0     6687 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/model.py
--rw-r--r--   0        0        0      745 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/ontology.py
--rw-r--r--   0        0        0     8844 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/project.py
--rw-r--r--   0        0        0      625 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/project_api_key.py
--rw-r--r--   0        0        0      828 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/project_with_user_role.py
--rw-r--r--   0        0        0        0 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/test/__init__.py
--rw-r--r--   0        0        0      570 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/test/test_dataset.py
--rw-r--r--   0        0        0    38298 2023-04-28 14:21:09.217585 encord-0.1.74/encord/project.py
--rw-r--r--   0        0        0        0 2023-04-28 14:21:09.217585 encord-0.1.74/encord/project_ontology/__init__.py
--rw-r--r--   0        0        0     1316 2023-04-28 14:21:09.217585 encord-0.1.74/encord/project_ontology/classification_attribute.py
--rw-r--r--   0        0        0      525 2023-04-28 14:21:09.217585 encord-0.1.74/encord/project_ontology/classification_option.py
--rw-r--r--   0        0        0      357 2023-04-28 14:21:09.217585 encord-0.1.74/encord/project_ontology/classification_type.py
--rw-r--r--   0        0        0      237 2023-04-28 14:21:09.217585 encord-0.1.74/encord/project_ontology/object_type.py
--rw-r--r--   0        0        0     9526 2023-04-28 14:21:09.217585 encord-0.1.74/encord/project_ontology/ontology.py
--rw-r--r--   0        0        0      630 2023-04-28 14:21:09.217585 encord-0.1.74/encord/project_ontology/ontology_classification.py
--rw-r--r--   0        0        0      683 2023-04-28 14:21:09.217585 encord-0.1.74/encord/project_ontology/ontology_object.py
--rw-r--r--   0        0        0    27801 2023-04-28 14:21:09.217585 encord-0.1.74/encord/user_client.py
--rw-r--r--   0        0        0        0 2023-04-28 14:21:09.217585 encord-0.1.74/encord/utilities/__init__.py
--rw-r--r--   0        0        0     4231 2023-04-28 14:21:09.217585 encord-0.1.74/encord/utilities/client_utilities.py
--rw-r--r--   0        0        0      253 2023-04-28 14:21:09.217585 encord-0.1.74/encord/utilities/common.py
--rw-r--r--   0        0        0     3270 2023-04-28 14:21:09.217585 encord-0.1.74/encord/utilities/label_utilities.py
--rw-r--r--   0        0        0      343 2023-04-28 14:21:09.217585 encord-0.1.74/encord/utilities/ontology_user.py
--rw-r--r--   0        0        0      578 2023-04-28 14:21:09.217585 encord-0.1.74/encord/utilities/project_user.py
--rw-r--r--   0        0        0      467 2023-04-28 14:21:09.217585 encord-0.1.74/encord/utilities/project_utilities.py
--rw-r--r--   0        0        0     1659 2023-04-28 14:21:09.217585 encord-0.1.74/pyproject.toml
--rw-r--r--   0        0        0     3728 1970-01-01 00:00:00.000000 encord-0.1.74/setup.py
--rw-r--r--   0        0        0     3774 1970-01-01 00:00:00.000000 encord-0.1.74/PKG-INFO
+-rw-r--r--   0        0        0    11330 2023-05-09 09:11:04.774966 encord-0.1.75/LICENSE
+-rw-r--r--   0        0        0     2595 2023-05-09 09:11:04.774966 encord-0.1.75/README.md
+-rw-r--r--   0        0        0       84 2023-05-09 09:11:04.774966 encord-0.1.75/cord/__init__.py
+-rw-r--r--   0        0        0      158 2023-05-09 09:11:04.794966 encord-0.1.75/encord/__init__.py
+-rw-r--r--   0        0        0      214 2023-05-09 09:11:04.794966 encord-0.1.75/encord/_version.py
+-rw-r--r--   0        0        0    47909 2023-05-09 09:11:04.794966 encord-0.1.75/encord/client.py
+-rw-r--r--   0        0        0    10825 2023-05-09 09:11:04.794966 encord-0.1.75/encord/configs.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:11:04.794966 encord-0.1.75/encord/constants/__init__.py
+-rw-r--r--   0        0        0      810 2023-05-09 09:11:04.794966 encord-0.1.75/encord/constants/enums.py
+-rw-r--r--   0        0        0     3211 2023-05-09 09:11:04.794966 encord-0.1.75/encord/constants/model.py
+-rw-r--r--   0        0        0     6068 2023-05-09 09:11:04.794966 encord-0.1.75/encord/constants/model_weights.py
+-rw-r--r--   0        0        0     1119 2023-05-09 09:11:04.794966 encord-0.1.75/encord/constants/string_constants.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:11:04.794966 encord-0.1.75/encord/constants/test/__init__.py
+-rw-r--r--   0        0        0      634 2023-05-09 09:11:04.794966 encord-0.1.75/encord/constants/test/test_enums.py
+-rw-r--r--   0        0        0    16035 2023-05-09 09:11:04.794966 encord-0.1.75/encord/dataset.py
+-rw-r--r--   0        0        0     5823 2023-05-09 09:11:04.794966 encord-0.1.75/encord/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:11:04.794966 encord-0.1.75/encord/http/__init__.py
+-rw-r--r--   0        0        0      535 2023-05-09 09:11:04.794966 encord-0.1.75/encord/http/constants.py
+-rw-r--r--   0        0        0     6607 2023-05-09 09:11:04.794966 encord-0.1.75/encord/http/error_utils.py
+-rw-r--r--   0        0        0     5999 2023-05-09 09:11:04.794966 encord-0.1.75/encord/http/querier.py
+-rw-r--r--   0        0        0      697 2023-05-09 09:11:04.794966 encord-0.1.75/encord/http/query_methods.py
+-rw-r--r--   0        0        0     1691 2023-05-09 09:11:04.794966 encord-0.1.75/encord/http/request.py
+-rw-r--r--   0        0        0     5880 2023-05-09 09:11:04.794966 encord-0.1.75/encord/http/utils.py
+-rw-r--r--   0        0        0      340 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/__init__.py
+-rw-r--r--   0        0        0      145 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/classification.py
+-rw-r--r--   0        0        0    29709 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/common.py
+-rw-r--r--   0        0        0      172 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/constants.py
+-rw-r--r--   0        0        0     5631 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/coordinates.py
+-rw-r--r--   0        0        0     3419 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/frames.py
+-rw-r--r--   0        0        0    21407 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/internal_helpers.py
+-rw-r--r--   0        0        0   135230 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/ontology_labels_impl.py
+-rw-r--r--   0        0        0      137 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/ontology_object.py
+-rw-r--r--   0        0        0      148 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/ontology_structure.py
+-rw-r--r--   0        0        0      549 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/project.py
+-rw-r--r--   0        0        0     1240 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/utils.py
+-rw-r--r--   0        0        0     3430 2023-05-09 09:11:04.794966 encord-0.1.75/encord/ontology.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/__init__.py
+-rw-r--r--   0        0        0      982 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/api_key.py
+-rw-r--r--   0        0        0     5377 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/base_orm.py
+-rw-r--r--   0        0        0      111 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/cloud_integration.py
+-rw-r--r--   0        0        0    32206 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/dataset.py
+-rw-r--r--   0        0        0      828 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/dataset_with_user_role.py
+-rw-r--r--   0        0        0      201 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/formatter.py
+-rw-r--r--   0        0        0     1155 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/label_log.py
+-rw-r--r--   0        0        0    11869 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/label_row.py
+-rw-r--r--   0        0        0     1577 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/labeling_algorithm.py
+-rw-r--r--   0        0        0     6687 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/model.py
+-rw-r--r--   0        0        0      745 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/ontology.py
+-rw-r--r--   0        0        0     8844 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/project.py
+-rw-r--r--   0        0        0      625 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/project_api_key.py
+-rw-r--r--   0        0        0      828 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/project_with_user_role.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/test/__init__.py
+-rw-r--r--   0        0        0      570 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/test/test_dataset.py
+-rw-r--r--   0        0        0    38903 2023-05-09 09:11:04.794966 encord-0.1.75/encord/project.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:11:04.798966 encord-0.1.75/encord/project_ontology/__init__.py
+-rw-r--r--   0        0        0     1316 2023-05-09 09:11:04.798966 encord-0.1.75/encord/project_ontology/classification_attribute.py
+-rw-r--r--   0        0        0      525 2023-05-09 09:11:04.798966 encord-0.1.75/encord/project_ontology/classification_option.py
+-rw-r--r--   0        0        0      357 2023-05-09 09:11:04.798966 encord-0.1.75/encord/project_ontology/classification_type.py
+-rw-r--r--   0        0        0      237 2023-05-09 09:11:04.798966 encord-0.1.75/encord/project_ontology/object_type.py
+-rw-r--r--   0        0        0     9526 2023-05-09 09:11:04.798966 encord-0.1.75/encord/project_ontology/ontology.py
+-rw-r--r--   0        0        0      630 2023-05-09 09:11:04.798966 encord-0.1.75/encord/project_ontology/ontology_classification.py
+-rw-r--r--   0        0        0      683 2023-05-09 09:11:04.798966 encord-0.1.75/encord/project_ontology/ontology_object.py
+-rw-r--r--   0        0        0    27801 2023-05-09 09:11:04.798966 encord-0.1.75/encord/user_client.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:11:04.798966 encord-0.1.75/encord/utilities/__init__.py
+-rw-r--r--   0        0        0     4231 2023-05-09 09:11:04.798966 encord-0.1.75/encord/utilities/client_utilities.py
+-rw-r--r--   0        0        0      253 2023-05-09 09:11:04.798966 encord-0.1.75/encord/utilities/common.py
+-rw-r--r--   0        0        0     3270 2023-05-09 09:11:04.798966 encord-0.1.75/encord/utilities/label_utilities.py
+-rw-r--r--   0        0        0      343 2023-05-09 09:11:04.798966 encord-0.1.75/encord/utilities/ontology_user.py
+-rw-r--r--   0        0        0      578 2023-05-09 09:11:04.798966 encord-0.1.75/encord/utilities/project_user.py
+-rw-r--r--   0        0        0      467 2023-05-09 09:11:04.798966 encord-0.1.75/encord/utilities/project_utilities.py
+-rw-r--r--   0        0        0     1659 2023-05-09 09:11:04.798966 encord-0.1.75/pyproject.toml
+-rw-r--r--   0        0        0     3728 1970-01-01 00:00:00.000000 encord-0.1.75/setup.py
+-rw-r--r--   0        0        0     3774 1970-01-01 00:00:00.000000 encord-0.1.75/PKG-INFO
```

### Comparing `encord-0.1.74/LICENSE` & `encord-0.1.75/LICENSE`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/README.md` & `encord-0.1.75/README.md`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/client.py` & `encord-0.1.75/encord/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -725,14 +725,16 @@
         shadow_data_state: Optional[ShadowDataState] = None,
         *,
         include_uninitialised_labels=False,
         label_hashes: Optional[List[str]] = None,
         data_hashes: Optional[List[str]] = None,
         data_title_eq: Optional[str] = None,
         data_title_like: Optional[str] = None,
+        workflow_graph_node_title_eq: Optional[str] = None,
+        workflow_graph_node_title_like: Optional[str] = None,
     ) -> List[LabelRowMetadata]:
         """
         This function is documented in :meth:`encord.project.Project.list_label_rows`.
         """
         if label_statuses:
             label_statuses = [label_status.value for label_status in label_statuses]
         edited_before = parse_datetime("edited_before", edited_before)
@@ -744,14 +746,16 @@
             "label_statuses": label_statuses,
             "shadow_data_state": shadow_data_state.value if shadow_data_state else None,
             "include_uninitialised_labels": include_uninitialised_labels,
             "data_hashes": data_hashes,
             "label_hashes": label_hashes,
             "data_title_eq": data_title_eq,
             "data_title_like": data_title_like,
+            "workflow_graph_node_title_eq": workflow_graph_node_title_eq,
+            "workflow_graph_node_title_like": workflow_graph_node_title_like,
         }
         return self._querier.get_multiple(LabelRowMetadata, payload=payload)
 
     def set_label_status(self, label_hash: str, label_status: LabelStatus) -> bool:
         """
         This function is documented in :meth:`encord.project.Project.set_label_status`.
         """
@@ -1241,9 +1245,20 @@
 
         Returns:
             bool
         """
         payload = {"editor": ontology.to_dict()}
         return self._querier.basic_setter(OrmProject, uid=None, payload=payload)
 
+    def workflow_reopen(self, label_hashes: list[str]) -> None:
+        """
+        This function is documented in :meth:`encord.objects.LabelRowV2.workflow_reopen`.
+        """
+
+        # Workaround to make basic_setter generate proper api call
+        class LabelWorkflowGraphNode:
+            pass
+
+        self._querier.basic_setter(LabelWorkflowGraphNode, label_hashes, payload=None)
+
 
 CordClientProject = EncordClientProject
```

### Comparing `encord-0.1.74/encord/configs.py` & `encord-0.1.75/encord/configs.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/constants/enums.py` & `encord-0.1.75/encord/constants/enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/constants/model.py` & `encord-0.1.75/encord/constants/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/constants/model_weights.py` & `encord-0.1.75/encord/constants/model_weights.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/constants/string_constants.py` & `encord-0.1.75/encord/constants/string_constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/constants/test/test_enums.py` & `encord-0.1.75/encord/constants/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/dataset.py` & `encord-0.1.75/encord/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/exceptions.py` & `encord-0.1.75/encord/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,7 +246,14 @@
     pass
 
 
 class OntologyError(EncordException):
     """An error thrown when using the ontology class with an error."""
 
     pass
+
+
+class WrongProjectTypeError(CordException):
+    """
+    An error thrown when project type does not match the operation
+    E.g. when TMS2 specific operations are attempted on non-TMS2 project
+    """
```

### Comparing `encord-0.1.74/encord/http/constants.py` & `encord-0.1.75/encord/http/constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/http/error_utils.py` & `encord-0.1.75/encord/http/error_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 DETECTION_RANGE_INVALID_ERROR = ["DETECTION_RANGE_INVALID_ERROR"]
 RESOURCE_EXISTS_ERROR = ["RESOURCE_EXISTS_ERROR"]
 INVALID_DATE_FORMAT_ERROR = ["INVALID_DATE_FORMAT_ERROR"]
 DUPLICATE_SSH_KEY_ERROR = ["DUPLICATE_SSH_KEY_ERROR"]
 SSH_KEY_NOT_FOUND_ERROR = ["SSH_KEY_NOT_FOUND_ERROR"]
 INVALID_ARGUMENTS_ERROR = ["INVALID_ARGUMENTS_ERROR"]
 MULTI_LABEL_LIMIT_ERROR = ["MULTI_LABEL_LIMIT_ERROR"]
+WRONG_PROJECT_TYPE_ERROR = ["WRONG_PROJECT_TYPE_ERROR"]
 
 
 def check_error_response(response, payload=None):
     """
     Checks server response.
     Called if HTTP response status code is an error response.
     """
@@ -127,14 +128,22 @@
         maximum_labels_allowed = payload["maximum_labels_allowed"]
         raise MultiLabelLimitError(
             f"Too many labels were requested. The limit is {maximum_labels_allowed}. Please reduce the amount "
             "of requested labels to stay under the reported limit.",
             maximum_labels_allowed=maximum_labels_allowed,
         )
 
+    if response == WRONG_PROJECT_TYPE_ERROR:
+        default_message = "Operation is not supported by the project type"
+        if payload is None:
+            message = default_message
+        else:
+            message = payload
+        raise WrongProjectTypeError(message)
+
     payload_string = ""
     if payload:
         payload_string = f" with the following payload `{payload}`"
     raise GenericServerError(
         f"The Encord server has reported an error of type `{response}`{payload_string}. Please do not parse this error "
         "programmatically, instead please upgrade the SDK to the latest version to get the exact error."
     )
```

### Comparing `encord-0.1.74/encord/http/querier.py` & `encord-0.1.75/encord/http/querier.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/http/query_methods.py` & `encord-0.1.75/encord/http/query_methods.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/http/request.py` & `encord-0.1.75/encord/http/request.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/http/utils.py` & `encord-0.1.75/encord/http/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/objects/common.py` & `encord-0.1.75/encord/objects/common.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/objects/coordinates.py` & `encord-0.1.75/encord/objects/coordinates.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/objects/frames.py` & `encord-0.1.75/encord/objects/frames.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/objects/internal_helpers.py` & `encord-0.1.75/encord/objects/internal_helpers.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/objects/ontology_labels_impl.py` & `encord-0.1.75/encord/objects/ontology_labels_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import logging
 from collections import defaultdict
 from copy import deepcopy
 from dataclasses import asdict, dataclass, field
 from datetime import datetime
 from enum import IntEnum
 from typing import (
     Any,
@@ -84,15 +85,19 @@
     check_email,
     check_type,
     does_type_match,
     filter_by_type,
     short_uuid_str,
 )
 from encord.orm.formatter import Formatter
-from encord.orm.label_row import AnnotationTaskStatus, LabelRowMetadata, LabelStatus
+from encord.orm.label_row import AnnotationTaskStatus, LabelRowMetadata, LabelStatus, WorkflowGraphNode
+from encord.exceptions import WrongProjectTypeError
+
+
+log = logging.getLogger(__name__)
 
 
 @dataclass
 class Object:
     """
     This class is currently in BETA. Its API might change in future minor version releases.
     """
@@ -905,21 +910,52 @@
 
     @property
     def data_type(self) -> DataType:
         return self._label_row_read_only_data.data_type
 
     @property
     def label_status(self) -> LabelStatus:
+        """
+        Returns the current labeling status for the label row.
+
+        **Note**: This method is not supported for workflow-based projects. Please see our
+        :ref:`workflow documentation <tutorials/workflows:Workflows>`
+        for more details.
+        """
+
+        if self.__is_tms2_project:
+            raise WrongProjectTypeError(
+                '"label"_status property returns incorrect results for workflow-based projects.\
+             Please use "workflow_graph_node" property instead.'
+            )
+
         return self._label_row_read_only_data.label_status
 
     @property
     def annotation_task_status(self) -> AnnotationTaskStatus:
+        """
+        Returns the current annotation task status for the label row.
+
+        **Note**: This method is not supported for workflow-based projects. Please see our
+        :ref:`workflow documentation <tutorials/workflows:Workflows>`
+        for more details.
+        """
+        if self.__is_tms2_project:
+            raise WrongProjectTypeError(
+                '"annotation_task_status" property returns incorrect results for workflow-based projects.\
+             Please use "workflow_graph_node" property instead.'
+            )
+
         return self._label_row_read_only_data.annotation_task_status
 
     @property
+    def workflow_graph_node(self) -> Optional[WorkflowGraphNode]:
+        return self._label_row_read_only_data.workflow_graph_node
+
+    @property
     def is_shadow_data(self) -> bool:
         return self._label_row_read_only_data.is_shadow_data
 
     @property
     def created_at(self) -> Optional[datetime]:
         """The creation date of the label row. None if the label row was not yet created."""
         return self._label_row_read_only_data.created_at
@@ -977,14 +1013,18 @@
     def is_labelling_initialised(self) -> bool:
         """
         Whether you can start labelling or not. If this is `False`, call the member `.initialise_labels()` to
         read or write specific ObjectInstances or ClassificationInstances.
         """
         return self._is_labelling_initialised
 
+    @property
+    def __is_tms2_project(self) -> bool:
+        return self.workflow_graph_node is not None
+
     def initialise_labels(
         self,
         include_object_feature_hashes: Optional[Set[str]] = None,
         include_classification_feature_hashes: Optional[Set[str]] = None,
         include_reviews: bool = False,
         overwrite: bool = False,
     ) -> None:
@@ -1343,14 +1383,27 @@
         ret["classification_answers"] = self._to_classification_answers()
         ret["object_actions"] = self._to_object_actions()
         ret["label_status"] = read_only_data.label_status.value
         ret["data_units"] = self._to_encord_data_units()
 
         return ret
 
+    def workflow_reopen(self) -> None:
+        """
+        A label row is returned to the first annotation stage for re-labeling. No data is lost during the call.
+        No data will be lost during this call.
+        This method is only relevant for the projects that use the Encord Task Management System 2,
+        and does nothing for other types of projects
+        """
+        if self.label_hash is None:
+            # Label has not yet moved from the initial state, nothing to do
+            return
+
+        self._project_client.workflow_reopen([self.label_hash])
+
     class FrameView:
         """
         This class can be used to inspect what object/classification instances are on a given frame or
         what metadata, such as a image file size, is on a given frame.
         """
 
         def __init__(
@@ -1531,15 +1584,16 @@
         created_at: Optional[datetime]
         """This is None if the label row does not have any labels and was not initialised for labelling."""
         last_edited_at: Optional[datetime]
         """This is None if the label row does not have any labels and was not initialised for labelling."""
         data_hash: str
         data_type: DataType
         label_status: LabelStatus
-        annotation_task_status: AnnotationTaskStatus
+        annotation_task_status: Optional[AnnotationTaskStatus]
+        workflow_graph_node: Optional[WorkflowGraphNode]
         is_shadow_data: bool
         number_of_frames: int
         duration: Optional[float]
         fps: Optional[float]
         dataset_hash: str
         dataset_title: str
         data_title: str
@@ -1795,14 +1849,15 @@
             data_title=label_row_metadata.data_title,
             dataset_hash=label_row_metadata.dataset_hash,
             dataset_title=label_row_metadata.dataset_title,
             data_type=data_type,
             data_link=label_row_metadata.data_link,
             label_status=label_row_metadata.label_status,
             annotation_task_status=label_row_metadata.annotation_task_status,
+            workflow_graph_node=label_row_metadata.workflow_graph_node,
             is_shadow_data=label_row_metadata.is_shadow_data,
             created_at=label_row_metadata.created_at,
             last_edited_at=label_row_metadata.last_edited_at,
             duration=label_row_metadata.duration,
             fps=label_row_metadata.frames_per_second,
             number_of_frames=label_row_metadata.number_of_frames,
             width=label_row_metadata.width,
@@ -1845,15 +1900,16 @@
             label_hash=label_row_dict["label_hash"],
             dataset_hash=label_row_dict["dataset_hash"],
             dataset_title=label_row_dict["dataset_title"],
             data_title=label_row_dict["data_title"],
             data_hash=label_row_dict["data_hash"],
             data_type=data_type,
             label_status=LabelStatus(label_row_dict["label_status"]),
-            annotation_task_status=label_row_dict["annotation_task_status"],
+            annotation_task_status=label_row_dict.get("annotation_task_status", None),
+            workflow_graph_node=label_row_dict.get("workflow_graph_node", None),
             is_shadow_data=self.is_shadow_data,
             created_at=label_row_dict["created_at"],
             last_edited_at=label_row_dict["last_edited_at"],
             frame_level_data=frame_level_data,
             image_hash_to_frame=image_hash_to_frame,
             frame_to_image_hash=frame_to_image_hash,
             duration=self.duration,
```

### Comparing `encord-0.1.74/encord/objects/project.py` & `encord-0.1.75/encord/objects/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/objects/utils.py` & `encord-0.1.75/encord/objects/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/ontology.py` & `encord-0.1.75/encord/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/orm/api_key.py` & `encord-0.1.75/encord/orm/api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/orm/base_orm.py` & `encord-0.1.75/encord/orm/base_orm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/orm/dataset.py` & `encord-0.1.75/encord/orm/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/orm/dataset_with_user_role.py` & `encord-0.1.75/encord/orm/dataset_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/orm/label_log.py` & `encord-0.1.75/encord/orm/label_log.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/orm/label_row.py` & `encord-0.1.75/encord/orm/label_row.py`

 * *Files 4% similar despite different names*

```diff
@@ -232,14 +232,26 @@
 
     @classmethod
     def _missing_(cls, value):
         return cls.MISSING_LABEL_STATUS
 
 
 @dataclass(frozen=True)
+class WorkflowGraphNode:
+    uuid: str
+    title: str
+
+    @classmethod
+    def from_optional_dict(cls, json_dict: Optional[Dict]) -> Optional[WorkflowGraphNode]:
+        if json_dict is None:
+            return None
+        return WorkflowGraphNode(uuid=json_dict["uuid"], title=json_dict["title"])
+
+
+@dataclass(frozen=True)
 class LabelRowMetadata(Formatter):
     """
     Contains helpful information about a label row.
     """
 
     label_hash: Optional[str]
     """Only present if the label row is initiated"""
@@ -252,15 +264,18 @@
     dataset_hash: str
     dataset_title: str
     data_title: str
     data_type: str
     data_link: Optional[str]
     """Can be `None` for label rows of image groups or DICOM series."""
     label_status: LabelStatus
-    annotation_task_status: AnnotationTaskStatus
+    """Can be `None` for TMS2 projects"""
+    annotation_task_status: Optional[AnnotationTaskStatus]
+    """Only available for TMS2 project"""
+    workflow_graph_node: Optional[WorkflowGraphNode]
     is_shadow_data: bool
     number_of_frames: int
     duration: Optional[float]
     """Only available for the VIDEO data_type"""
     frames_per_second: Optional[int]
     """Only available for the VIDEO data_type"""
     height: Optional[int]
@@ -271,26 +286,33 @@
         created_at = json_dict.get("created_at", None)
         if created_at is not None:
             created_at = datetime.datetime.fromisoformat(created_at)
         last_edited_at = json_dict.get("last_edited_at", None)
         if last_edited_at is not None:
             last_edited_at = datetime.datetime.fromisoformat(last_edited_at)
 
+        annotation_task_status = (
+            AnnotationTaskStatus(json_dict["annotation_task_status"])
+            if json_dict["annotation_task_status"] is not None
+            else None
+        )
+
         return LabelRowMetadata(
             label_hash=json_dict.get("label_hash", None),
             created_at=created_at,
             last_edited_at=last_edited_at,
             data_hash=json_dict["data_hash"],
             dataset_hash=json_dict["dataset_hash"],
             dataset_title=json_dict["dataset_title"],
             data_title=json_dict["data_title"],
             data_type=json_dict["data_type"],
             data_link=json_dict["data_link"],
             label_status=LabelStatus(json_dict["label_status"]),
-            annotation_task_status=AnnotationTaskStatus(json_dict["annotation_task_status"]),
+            annotation_task_status=annotation_task_status,
+            workflow_graph_node=WorkflowGraphNode.from_optional_dict(json_dict.get("workflow_graph_node")),
             is_shadow_data=json_dict.get("is_shadow_data", False),
             number_of_frames=json_dict["number_of_frames"],
             duration=json_dict.get("duration", None),
             frames_per_second=json_dict.get("frames_per_second", None),
             height=json_dict.get("height"),
             width=json_dict.get("width"),
         )
```

### Comparing `encord-0.1.74/encord/orm/labeling_algorithm.py` & `encord-0.1.75/encord/orm/labeling_algorithm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/orm/model.py` & `encord-0.1.75/encord/orm/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/orm/ontology.py` & `encord-0.1.75/encord/orm/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/orm/project.py` & `encord-0.1.75/encord/orm/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/orm/project_api_key.py` & `encord-0.1.75/encord/orm/project_api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/orm/project_with_user_role.py` & `encord-0.1.75/encord/orm/project_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/orm/test/test_dataset.py` & `encord-0.1.75/encord/orm/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/project.py` & `encord-0.1.75/encord/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,39 +156,45 @@
         label_hashes: Optional[List[str]] = None,
         edited_before: Optional[Union[str, datetime.datetime]] = None,
         edited_after: Optional[Union[str, datetime.datetime]] = None,
         label_statuses: Optional[List[AnnotationTaskStatus]] = None,
         shadow_data_state: Optional[ShadowDataState] = None,
         data_title_eq: Optional[str] = None,
         data_title_like: Optional[str] = None,
+        workflow_graph_node_title_eq: Optional[str] = None,
+        workflow_graph_node_title_like: Optional[str] = None,
     ) -> List[LabelRowV2]:
         """
         Args:
             data_hashes: List of data hashes to filter by.
             label_hashes: List of label hashes to filter by.
             edited_before: Optionally filter to only rows last edited before the specified time
             edited_after: Optionally filter to only rows last edited after the specified time
             label_statuses: Optionally filter to only those label rows that have one of the specified :class:`~encord.orm.label_row.AnnotationTaskStatus`es
             shadow_data_state: On Optionally filter by data type in Benchmark QA projects. See :class:`~encord.orm.label_row.ShadowDataState`
             data_title_eq: Optionally filter by exact title match
             data_title_like: Optionally filter by fuzzy title match; SQL syntax
+            workflow_graph_node_title_eq: Optionally filter by exact match with workflow node title
+            workflow_graph_node_title_like: Optionally filter by fuzzy match with workflow node title; SQL syntax
 
         Returns:
             A list of :class:`~encord.objects.LabelRowV2` instances for all the matching label rows
         """
         label_row_metadatas = self._client.list_label_rows(
             edited_before,
             edited_after,
             label_statuses,
             shadow_data_state,
             data_hashes=data_hashes,
             label_hashes=label_hashes,
             include_uninitialised_labels=True,
             data_title_eq=data_title_eq,
             data_title_like=data_title_like,
+            workflow_graph_node_title_eq=workflow_graph_node_title_eq,
+            workflow_graph_node_title_like=workflow_graph_node_title_like,
         )
 
         label_rows = [
             LabelRowV2(label_row_metadata, self._client, self._ontology) for label_row_metadata in label_row_metadatas
         ]
         return label_rows
 
@@ -252,14 +258,16 @@
             copy_labels=copy_labels,
         )
 
     def submit_label_row_for_review(self, uid: str):
         """
         Submit a label row for review.
 
+        **Note:** this method is not supported for the workflow-based projects. See the documentation about the workflows
+
         Args:
             uid: A label_hash (uid) string.
 
         Returns:
             Bool.
 
         Raises:
```

### Comparing `encord-0.1.74/encord/project_ontology/classification_attribute.py` & `encord-0.1.75/encord/project_ontology/classification_attribute.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/project_ontology/classification_option.py` & `encord-0.1.75/encord/project_ontology/classification_option.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/project_ontology/ontology.py` & `encord-0.1.75/encord/project_ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/project_ontology/ontology_classification.py` & `encord-0.1.75/encord/project_ontology/ontology_classification.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/project_ontology/ontology_object.py` & `encord-0.1.75/encord/project_ontology/ontology_object.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/user_client.py` & `encord-0.1.75/encord/user_client.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/utilities/client_utilities.py` & `encord-0.1.75/encord/utilities/client_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/utilities/label_utilities.py` & `encord-0.1.75/encord/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/encord/utilities/project_user.py` & `encord-0.1.75/encord/utilities/project_user.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.74/pyproject.toml` & `encord-0.1.75/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encord"
-version = "0.1.74"
+version = "0.1.75"
 description = "Encord Python SDK Client"
 authors = ["Cord Technologies Limited <hello@encord.com>"]
 license = "Apache Software License"
 keywords = ["cord", "encord"]
 packages = [
     { include = "cord"},
     { include = "encord"},
```

### Comparing `encord-0.1.74/setup.py` & `encord-0.1.75/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'tqdm>=4.32.1,<5.0.0']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib_metadata>=6.1.0,<7.0.0']}
 
 setup_kwargs = {
     'name': 'encord',
-    'version': '0.1.74',
+    'version': '0.1.75',
     'description': 'Encord Python SDK Client',
     'long_description': '<h1 align="center">\n  <p align="center">Encord Python API Client</p>\n  <a href="https://encord.com"><img src="./docs/_static/logo.svg" width="100" alt="Cord logo"/></a>\n</h1>\n\n[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n\n***The data engine for computer vision***\n\n## 💻 Features\n\n- Minimal low-level Python client that allows you to interact with Encord\'s API\n- Supports Python: `3.7`, `3.8`, `3.9`, and `3.10`\n\n## ✨ Relevant Links\n* [Encord website](https://encord.com)\n* [Encord web app](https://app.encord.com)\n* [Encord documentation](https://docs.encord.com)\n\n## 💡 Getting Started\n\nFor full documentation, please visit [Encord Python SDK](https://python.docs.encord.com/).\n\nFirst, install Encord Python API Client using the [pip](https://pip.pypa.io/en/stable/installing) package manager:\n\n```bash\npip install encord\n```\n\nThen, create an API key for authentication via the [Encord web app](https://app.encord.com). Pass the resource ID and API key as environment variables or pass them explicitly when you initialise the EncordClient object.\n\n```bash\nexport ENCORD_PROJECT_ID="<project_id>"\nexport ENCORD_API_KEY="<project_api_key>"\n```\n\nPassing the resource ID and API key as environment variables, you can initialise the Encord client directly.\n\n```python\nfrom encord.client import EncordClient\n\nclient = EncordClient.initialise()\n```\n\nIf you want to avoid setting environment variables, you can initialise the Encord client by passing the resource ID and API key as strings.\n\n```python\nfrom encord.client import EncordClient\n\nclient = EncordClient.initialise("<resource_id>", "<resource_api_key>")\n```\n\nIf you wish to instantiate several client objects and avoid passing parameters each time, you can instantiate a EncordConfig object, pass the resource ID and API key as strings, and initialise the client with the config object.\n\n```py\nfrom encord.client import EncordClient\nfrom encord.client import EncordConfig\n\nconfig = EncordConfig("<resource_id>", "<resource_api_key>")\nclient = EncordClient.initialise_with_config(config)\n```\n\nOnce you have instantiated an Encord client, it is easy to fetch information associated with the given resource ID.\n\n```py\nfrom encord.client import EncordClient\n\nclient = EncordClient.initialise()\nproject = client.get_project()\n```\n\n## 🐛 Troubleshooting\n\nPlease report bugs to [GitHub Issues](https://github.com/encord-team/encord-client-python/issues). Just make sure you read the [Encord documentation](https://docs.encord.com) and search for related issues first.\n',
     'author': 'Cord Technologies Limited',
     'author_email': 'hello@encord.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/encord-team/encord-client-python',
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['cord',
 'encord', 'encord.constants', 'encord.constants.test', 'encord.http',
 'encord.objects', 'encord.orm', 'encord.orm.test', 'encord.project_ontology',
 'encord.utilities'] package_data = \ {'': ['*']} install_requires = \
 ['cryptography>=3.4.8,<4.0.0', 'python-dateutil>=2.8.2,<3.0.0',
 'requests>=2.25.0,<3.0.0', 'tqdm>=4.32.1,<5.0.0'] extras_require = \ {':
 python_version < "3.8"': ['importlib_metadata>=6.1.0,<7.0.0']} setup_kwargs =
-{ 'name': 'encord', 'version': '0.1.74', 'description': 'Encord Python SDK
+{ 'name': 'encord', 'version': '0.1.75', 'description': 'Encord Python SDK
 Client', 'long_description': '
            ****** \nEncord Python API Client\n [Cord_logo]\n ******
 \n\n[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)]
 (https://opensource.org/licenses/Apache-2.0)\n\n***The data engine for computer
 vision***\n\n## ð» Features\n\n- Minimal low-level Python client that allows
 you to interact with Encord\'s API\n- Supports Python: `3.7`, `3.8`, `3.9`, and
 `3.10`\n\n## â¨ Relevant Links\n* [Encord website](https://encord.com)\n*
```

### Comparing `encord-0.1.74/PKG-INFO` & `encord-0.1.75/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encord
-Version: 0.1.74
+Version: 0.1.75
 Summary: Encord Python SDK Client
 Home-page: https://github.com/encord-team/encord-client-python
 License: Apache Software License
 Keywords: cord,encord
 Author: Cord Technologies Limited
 Author-email: hello@encord.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: encord Version: 0.1.74 Summary: Encord Python SDK
+Metadata-Version: 2.1 Name: encord Version: 0.1.75 Summary: Encord Python SDK
 Client Home-page: https://github.com/encord-team/encord-client-python License:
 Apache Software License Keywords: cord,encord Author: Cord Technologies Limited
 Author-email: hello@encord.com Requires-Python: >=3.7,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

