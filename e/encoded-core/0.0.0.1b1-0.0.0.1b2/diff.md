# Comparing `tmp/encoded_core-0.0.0.1b1.tar.gz` & `tmp/encoded_core-0.0.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encoded_core-0.0.0.1b1.tar", max compression
+gzip compressed data, was "encoded_core-0.0.0.1b2.tar", max compression
```

## Comparing `encoded_core-0.0.0.1b1.tar` & `encoded_core-0.0.0.1b2.tar`

### file list

```diff
@@ -1,41 +1,54 @@
--rw-r--r--   0        0        0     1083 2023-04-28 13:49:44.781887 encoded_core-0.0.0.1b1/LICENSE
--rw-r--r--   0        0        0      174 2023-04-28 13:50:12.674541 encoded_core-0.0.0.1b1/README.rst
--rw-r--r--   0        0        0     3092 2023-04-28 15:30:08.225982 encoded_core-0.0.0.1b1/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-28 13:50:12.698338 encoded_core-0.0.0.1b1/src/encoded-core/__init__.py
--rw-r--r--   0        0        0     1915 2023-04-28 13:50:12.708994 encoded_core-0.0.0.1b1/src/encoded-core/schemas/document.json
--rw-r--r--   0        0        0    18553 2023-04-28 13:50:12.704726 encoded_core-0.0.0.1b1/src/encoded-core/schemas/file.json
--rw-r--r--   0        0        0     5070 2023-04-28 13:50:12.701442 encoded_core-0.0.0.1b1/src/encoded-core/schemas/file_format.json
--rw-r--r--   0        0        0     6170 2023-04-28 13:50:12.706416 encoded_core-0.0.0.1b1/src/encoded-core/schemas/file_processed.json
--rw-r--r--   0        0        0     2336 2023-04-28 13:50:12.710774 encoded_core-0.0.0.1b1/src/encoded-core/schemas/file_reference.json
--rw-r--r--   0        0        0     1331 2023-04-28 13:50:12.712368 encoded_core-0.0.0.1b1/src/encoded-core/schemas/file_submitted.json
--rw-r--r--   0        0        0     1831 2023-04-28 13:50:12.715563 encoded_core-0.0.0.1b1/src/encoded-core/schemas/higlass_view_config.json
--rw-r--r--   0        0        0     1528 2023-04-28 13:50:12.714806 encoded_core-0.0.0.1b1/src/encoded-core/schemas/image.json
--rw-r--r--   0        0        0    18352 2023-04-28 13:50:12.707283 encoded_core-0.0.0.1b1/src/encoded-core/schemas/meta_workflow.json
--rw-r--r--   0        0        0    14409 2023-04-28 13:50:12.713194 encoded_core-0.0.0.1b1/src/encoded-core/schemas/meta_workflow_run.json
--rw-r--r--   0        0        0    17295 2023-04-28 13:50:12.702288 encoded_core-0.0.0.1b1/src/encoded-core/schemas/mixins.json
--rw-r--r--   0        0        0     4581 2023-04-28 13:50:12.716243 encoded_core-0.0.0.1b1/src/encoded-core/schemas/page.json
--rw-r--r--   0        0        0     1457 2023-04-28 13:50:12.709844 encoded_core-0.0.0.1b1/src/encoded-core/schemas/quality_metric.json
--rw-r--r--   0        0        0     5715 2023-04-28 13:50:12.713992 encoded_core-0.0.0.1b1/src/encoded-core/schemas/software.json
--rw-r--r--   0        0        0     5010 2023-04-28 13:50:12.708092 encoded_core-0.0.0.1b1/src/encoded-core/schemas/static_section.json
--rw-r--r--   0        0        0    20411 2023-04-28 13:50:12.700669 encoded_core-0.0.0.1b1/src/encoded-core/schemas/tracking_item.json
--rw-r--r--   0        0        0     3749 2023-04-28 13:50:12.703052 encoded_core-0.0.0.1b1/src/encoded-core/schemas/user_content.json
--rw-r--r--   0        0        0    28267 2023-04-28 13:50:12.699926 encoded_core-0.0.0.1b1/src/encoded-core/schemas/workflow.json
--rw-r--r--   0        0        0    10502 2023-04-28 13:50:12.711544 encoded_core-0.0.0.1b1/src/encoded-core/schemas/workflow_run.json
--rw-r--r--   0        0        0     1908 2023-04-28 13:50:12.703919 encoded_core-0.0.0.1b1/src/encoded-core/schemas/workflow_run_awsem.json
--rw-r--r--   0        0        0       70 2023-04-28 13:50:12.688855 encoded_core-0.0.0.1b1/src/encoded-core/types/__init__.py
--rw-r--r--   0        0        0     1290 2023-04-28 13:50:12.692749 encoded_core-0.0.0.1b1/src/encoded-core/types/document.py
--rw-r--r--   0        0        0    41353 2023-04-28 13:50:12.690559 encoded_core-0.0.0.1b1/src/encoded-core/types/file.py
--rw-r--r--   0        0        0      870 2023-04-28 13:50:12.692030 encoded_core-0.0.0.1b1/src/encoded-core/types/file_format.py
--rw-r--r--   0        0        0     2352 2023-04-28 13:50:12.696184 encoded_core-0.0.0.1b1/src/encoded-core/types/file_processed.py
--rw-r--r--   0        0        0      517 2023-04-28 13:50:12.693465 encoded_core-0.0.0.1b1/src/encoded-core/types/file_reference.py
--rw-r--r--   0        0        0     2025 2023-04-28 13:50:12.691291 encoded_core-0.0.0.1b1/src/encoded-core/types/file_submitted.py
--rw-r--r--   0        0        0      607 2023-04-28 13:50:12.697483 encoded_core-0.0.0.1b1/src/encoded-core/types/higlass_view_config.py
--rw-r--r--   0        0        0     1046 2023-04-28 13:50:12.695219 encoded_core-0.0.0.1b1/src/encoded-core/types/image.py
--rw-r--r--   0        0        0     3191 2023-04-28 13:50:12.689732 encoded_core-0.0.0.1b1/src/encoded-core/types/meta_workflow.py
--rw-r--r--   0        0        0     5428 2023-04-28 13:50:12.687023 encoded_core-0.0.0.1b1/src/encoded-core/types/quality_metric.py
--rw-r--r--   0        0        0     2745 2023-04-28 13:50:12.696837 encoded_core-0.0.0.1b1/src/encoded-core/types/software.py
--rw-r--r--   0        0        0     3895 2023-04-28 13:50:12.687755 encoded_core-0.0.0.1b1/src/encoded-core/types/tracking_item.py
--rw-r--r--   0        0        0     5458 2023-04-28 13:50:12.686230 encoded_core-0.0.0.1b1/src/encoded-core/types/user_content.py
--rw-r--r--   0        0        0    12871 2023-04-28 13:50:12.694432 encoded_core-0.0.0.1b1/src/encoded-core/types/workflow.py
--rw-r--r--   0        0        0     1957 1970-01-01 00:00:00.000000 encoded_core-0.0.0.1b1/setup.py
--rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 encoded_core-0.0.0.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-28 13:49:44.781887 encoded_core-0.0.0.1b2/LICENSE
+-rw-r--r--   0        0        0      174 2023-04-28 13:50:12.674541 encoded_core-0.0.0.1b2/README.rst
+-rw-r--r--   0        0        0     3671 2023-05-09 14:51:36.163703 encoded_core-0.0.0.1b2/pyproject.toml
+-rw-r--r--   0        0        0     2378 2023-05-01 18:24:20.274258 encoded_core-0.0.0.1b2/src/encoded_core/__init__.py
+-rw-r--r--   0        0        0     4847 2023-04-28 17:14:35.491425 encoded_core-0.0.0.1b2/src/encoded_core/local_roles.py
+-rw-r--r--   0        0        0     1915 2023-04-28 13:50:12.708994 encoded_core-0.0.0.1b2/src/encoded_core/schemas/document.json
+-rw-r--r--   0        0        0    18925 2023-05-02 19:21:41.656041 encoded_core-0.0.0.1b2/src/encoded_core/schemas/file.json
+-rw-r--r--   0        0        0     5070 2023-04-28 13:50:12.701442 encoded_core-0.0.0.1b2/src/encoded_core/schemas/file_format.json
+-rw-r--r--   0        0        0     6170 2023-04-28 13:50:12.706416 encoded_core-0.0.0.1b2/src/encoded_core/schemas/file_processed.json
+-rw-r--r--   0        0        0     2336 2023-04-28 13:50:12.710774 encoded_core-0.0.0.1b2/src/encoded_core/schemas/file_reference.json
+-rw-r--r--   0        0        0     1331 2023-04-28 13:50:12.712368 encoded_core-0.0.0.1b2/src/encoded_core/schemas/file_submitted.json
+-rw-r--r--   0        0        0     1831 2023-04-28 13:50:12.715563 encoded_core-0.0.0.1b2/src/encoded_core/schemas/higlass_view_config.json
+-rw-r--r--   0        0        0     1528 2023-04-28 13:50:12.714806 encoded_core-0.0.0.1b2/src/encoded_core/schemas/image.json
+-rw-r--r--   0        0        0    18352 2023-04-28 13:50:12.707283 encoded_core-0.0.0.1b2/src/encoded_core/schemas/meta_workflow.json
+-rw-r--r--   0        0        0    14409 2023-04-28 13:50:12.713194 encoded_core-0.0.0.1b2/src/encoded_core/schemas/meta_workflow_run.json
+-rw-r--r--   0        0        0    17295 2023-04-28 13:50:12.702288 encoded_core-0.0.0.1b2/src/encoded_core/schemas/mixins.json
+-rw-r--r--   0        0        0     4581 2023-04-28 13:50:12.716243 encoded_core-0.0.0.1b2/src/encoded_core/schemas/page.json
+-rw-r--r--   0        0        0     1454 2023-05-05 17:13:08.190163 encoded_core-0.0.0.1b2/src/encoded_core/schemas/quality_metric.json
+-rw-r--r--   0        0        0     3228 2023-05-02 19:21:00.959543 encoded_core-0.0.0.1b2/src/encoded_core/schemas/quality_metric_generic.json
+-rw-r--r--   0        0        0     5715 2023-04-28 13:50:12.713992 encoded_core-0.0.0.1b2/src/encoded_core/schemas/software.json
+-rw-r--r--   0        0        0     5010 2023-04-28 13:50:12.708092 encoded_core-0.0.0.1b2/src/encoded_core/schemas/static_section.json
+-rw-r--r--   0        0        0    20411 2023-04-28 13:50:12.700669 encoded_core-0.0.0.1b2/src/encoded_core/schemas/tracking_item.json
+-rw-r--r--   0        0        0     3749 2023-04-28 13:50:12.703052 encoded_core-0.0.0.1b2/src/encoded_core/schemas/user_content.json
+-rw-r--r--   0        0        0    28089 2023-05-02 19:08:31.618837 encoded_core-0.0.0.1b2/src/encoded_core/schemas/workflow.json
+-rw-r--r--   0        0        0    10491 2023-05-02 19:07:38.780580 encoded_core-0.0.0.1b2/src/encoded_core/schemas/workflow_run.json
+-rw-r--r--   0        0        0     1908 2023-04-28 13:50:12.703919 encoded_core-0.0.0.1b2/src/encoded_core/schemas/workflow_run_awsem.json
+-rw-r--r--   0        0        0        0 2023-04-28 17:30:49.756296 encoded_core-0.0.0.1b2/src/encoded_core/tests/__init__.py
+-rw-r--r--   0        0        0    14046 2023-05-05 16:55:24.908128 encoded_core-0.0.0.1b2/src/encoded_core/tests/conftest.py
+-rw-r--r--   0        0        0     1873 2023-05-01 15:51:03.342243 encoded_core-0.0.0.1b2/src/encoded_core/tests/conftest_settings.py
+-rw-r--r--   0        0        0     7765 2023-05-02 19:39:48.058091 encoded_core-0.0.0.1b2/src/encoded_core/tests/datafixtures.py
+-rw-r--r--   0        0        0    10832 2023-05-02 19:39:17.806355 encoded_core-0.0.0.1b2/src/encoded_core/tests/test_types_file.py
+-rw-r--r--   0        0        0      262 2023-05-02 19:36:28.328655 encoded_core-0.0.0.1b2/src/encoded_core/tests/test_types_file_format.py
+-rw-r--r--   0        0        0      239 2023-05-02 19:39:17.802109 encoded_core-0.0.0.1b2/src/encoded_core/tests/test_types_meta_workflow.py
+-rw-r--r--   0        0        0      212 2023-05-02 19:39:17.799579 encoded_core-0.0.0.1b2/src/encoded_core/tests/test_types_software.py
+-rw-r--r--   0        0        0      502 2023-05-02 19:39:54.040945 encoded_core-0.0.0.1b2/src/encoded_core/tests/test_types_workflow.py
+-rw-r--r--   0        0        0       70 2023-04-28 13:50:12.688855 encoded_core-0.0.0.1b2/src/encoded_core/types/__init__.py
+-rw-r--r--   0        0        0     1290 2023-04-28 18:02:48.783979 encoded_core-0.0.0.1b2/src/encoded_core/types/document.py
+-rw-r--r--   0        0        0    41353 2023-04-28 18:02:48.769257 encoded_core-0.0.0.1b2/src/encoded_core/types/file.py
+-rw-r--r--   0        0        0      870 2023-04-28 18:02:48.776599 encoded_core-0.0.0.1b2/src/encoded_core/types/file_format.py
+-rw-r--r--   0        0        0     2352 2023-04-28 18:02:48.779024 encoded_core-0.0.0.1b2/src/encoded_core/types/file_processed.py
+-rw-r--r--   0        0        0      517 2023-04-28 18:02:48.786571 encoded_core-0.0.0.1b2/src/encoded_core/types/file_reference.py
+-rw-r--r--   0        0        0     2025 2023-04-28 18:02:48.765168 encoded_core-0.0.0.1b2/src/encoded_core/types/file_submitted.py
+-rw-r--r--   0        0        0      607 2023-04-28 18:02:48.793746 encoded_core-0.0.0.1b2/src/encoded_core/types/higlass_view_config.py
+-rw-r--r--   0        0        0     1046 2023-04-28 18:02:48.788942 encoded_core-0.0.0.1b2/src/encoded_core/types/image.py
+-rw-r--r--   0        0        0     3191 2023-04-28 18:02:48.781565 encoded_core-0.0.0.1b2/src/encoded_core/types/meta_workflow.py
+-rw-r--r--   0        0        0    13688 2023-05-09 14:53:19.136309 encoded_core-0.0.0.1b2/src/encoded_core/types/page.py
+-rw-r--r--   0        0        0     5824 2023-05-02 19:21:22.853435 encoded_core-0.0.0.1b2/src/encoded_core/types/quality_metric.py
+-rw-r--r--   0        0        0     2750 2023-05-01 15:51:03.333411 encoded_core-0.0.0.1b2/src/encoded_core/types/software.py
+-rw-r--r--   0        0        0     3895 2023-04-28 18:02:48.791425 encoded_core-0.0.0.1b2/src/encoded_core/types/tracking_item.py
+-rw-r--r--   0        0        0     5468 2023-05-01 15:51:03.338160 encoded_core-0.0.0.1b2/src/encoded_core/types/user_content.py
+-rw-r--r--   0        0        0    12886 2023-05-01 15:51:03.346409 encoded_core-0.0.0.1b2/src/encoded_core/types/workflow.py
+-rw-r--r--   0        0        0     1316 2023-04-28 17:00:24.678007 encoded_core-0.0.0.1b2/src/encoded_core/upgrade.py
+-rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 encoded_core-0.0.0.1b2/setup.py
+-rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 encoded_core-0.0.0.1b2/PKG-INFO
```

### Comparing `encoded_core-0.0.0.1b1/LICENSE` & `encoded_core-0.0.0.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b1/pyproject.toml` & `encoded_core-0.0.0.1b2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "encoded-core"
-version = "0.0.0.1b1"  # to become 0.0.1
+version = "0.0.0.1b2"  # to become 0.0.1
 description = "Core data models for Park Lab ENCODE based projects"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/smaht-dac/encoded-core"
 repository = "https://github.com/smaht-dac/encoded-core"
 documentation = "https://github.com/smaht-dac/encoded-core"
 packages = [
-  { include="encoded-core", from="src" }
+  { include="encoded_core", from="src" }
 ]
 classifiers = [
     # How mature is this project? Common values are
     #   3 - Alpha
     #   4 - Beta
     #   5 - Production/Stable
     'Development Status :: 3 - Alpha',
@@ -34,15 +34,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.10"
 awscli = ">=1.25.36"
 boto3 = "^1.24.36"
 botocore = "^1.27.36"
-dcicsnovault = "^8.0.1.0b1"
+dcicsnovault = "^8.0.1.0b3"
 dcicutils = "^7.0.0"
 elasticsearch = "7.13.4"
 jsonschema_serialize_fork = "^2.1.1"
 plaster-pastedeploy = "0.6"
 psycopg2-binary = "^2.9.3"
 PyJWT = "^2.6.0"
 pyramid = "1.10.4"
@@ -85,20 +85,35 @@
 # flask only for moto[server]
 flask = ">=2.0.3"
 # Upon removal of moto[server] we seem to be able to tolerate newer moto versions
 moto = "4.0.3"
 pip-licenses = "^3.3.1"
 pipdeptree = "^2.1.0"
 # TODO: Investigate whether a major version upgrade is allowable for 'pytest', which is several versions behind.
-pytest = ">=3.10,<4"
+pytest = ">=7,<8"
 pytest-cov = ">=2.2.1"
-pytest-exact-fixtures = ">=0.3"
 pytest-instafail = ">=0.3.0"
 pytest-mock = ">=0.11.0"
 pytest-timeout = ">=1.0.0"
 pytest-xdist = ">=1.14"
 wheel = ">=0.29.0"
 
+[tool.poetry.scripts]
+# dcicutils commands
+add-image-tag = "dcicutils.ecr_scripts:add_image_tag_main"
+show-global-env-bucket = "dcicutils.env_scripts:show_global_env_bucket_main"
+show-image-manifest = "dcicutils.ecr_scripts:show_image_manifest_main"
+show-image-catalog = "dcicutils.ecr_scripts:show_image_catalog_main"
+unrelease-most-recent-image = "dcicutils.ecr_scripts:unrelease_most_recent_image_main"
+
+[paste.app_factory]
+main = "encoded_core:main"
+
+[paste.composite_factory]
+indexer = "snovault.elasticsearch.es_index_listener:composite"
+
+[paste.filter_app_factory]
+memlimit = "snovault.memlimit:filter_app"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/document.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/document.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/file.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/file.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986979166666666%*

 * *Differences: {"'properties'": "{'quality_metrics': OrderedDict([('type', 'array'), ('title', 'Quality "*

 * *                 "Metrics'), ('description', 'Associated QC reports'), ('items', "*

 * *                 "OrderedDict([('type', 'string'), ('title', 'Quality Metric'), ('description', "*

 * *                 "'Associated QC report'), ('linkTo', 'QualityMetric')]))])}"}*

```diff
@@ -345,14 +345,25 @@
                 ],
                 "title": "Selected Quality Metric",
                 "type": "object"
             },
             "title": "Quality Metric Summary",
             "type": "array"
         },
+        "quality_metrics": {
+            "description": "Associated QC reports",
+            "items": {
+                "description": "Associated QC report",
+                "linkTo": "QualityMetric",
+                "title": "Quality Metric",
+                "type": "string"
+            },
+            "title": "Quality Metrics",
+            "type": "array"
+        },
         "related_files": {
             "description": "Files related to this one",
             "ff_flag": "second round",
             "items": {
                 "additionalProperties": false,
                 "properties": {
                     "file": {
```

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/file_format.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/file_format.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/file_processed.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/file_processed.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/file_reference.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/file_reference.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/file_submitted.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/file_submitted.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/higlass_view_config.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/higlass_view_config.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/image.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/image.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/meta_workflow.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/meta_workflow.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/meta_workflow_run.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/meta_workflow_run.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/mixins.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/page.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/page.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/quality_metric.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/quality_metric.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'description'": "'Schema for reporting the specific calculation of quality metrics'"}*

```diff
@@ -2,15 +2,15 @@
     "$schema": "http://json-schema.org/draft-04/schema#",
     "additionalProperties": false,
     "columns": {
         "overall_quality_status": {
             "title": "Overall Quality"
         }
     },
-    "description": "Schema for reporting the specific calculation of an quality metrics",
+    "description": "Schema for reporting the specific calculation of quality metrics",
     "facets": {
         "overall_quality_status": {
             "title": "Overall Quality"
         }
     },
     "id": "/profiles/quality_metric.json",
     "identifyingProperties": [
```

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/software.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/software.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/static_section.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/static_section.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/tracking_item.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/tracking_item.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/user_content.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/user_content.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/workflow.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/workflow.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9923076923076923%*

 * *Differences: {"'columns'": "{delete: ['experiment_types']}"}*

```diff
@@ -10,18 +10,14 @@
             "title": "App Version"
         },
         "category": {
             "colTitle": "Category",
             "default_hidden": true,
             "title": "Workflow Category"
         },
-        "experiment_types": {
-            "comment": "TODO: Update to `experiment_types.display_title` once becomes a linkTo",
-            "title": "Experiment Types"
-        },
         "workflow_language": {
             "colTitle": "Lang.",
             "default_hidden": true,
             "title": "Workflow Language"
         }
     },
     "description": "Schema for submitting a computational analysis workflow that is composed of analysis step(s).",
```

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/workflow_run.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/workflow_run.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998497596153846%*

 * *Differences: {"'properties'": "{'quality_metric': {'linkTo': 'QualityMetric'}}"}*

```diff
@@ -237,15 +237,15 @@
                 "type": "object"
             },
             "title": "parameters",
             "type": "array"
         },
         "quality_metric": {
             "description": "The associated QC reports",
-            "linkTo": "QualityMetricWorkflowrun",
+            "linkTo": "QualityMetric",
             "title": "Quality Metric",
             "type": "string"
         },
         "run_platform": {
             "enum": [
                 "SBG",
                 "AWSEM"
```

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/schemas/workflow_run_awsem.json` & `encoded_core-0.0.0.1b2/src/encoded_core/schemas/workflow_run_awsem.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/types/document.py` & `encoded_core-0.0.0.1b2/src/encoded_core/types/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         'title': 'Documents',
         'description': 'Listing of Documents',
     })
 class Document(ItemWithAttachment, Item):
     """Document class."""
 
     item_type = 'document'
-    schema = load_schema('encoded-core:schemas/document.json')
+    schema = load_schema('encoded_core:schemas/document.json')
     embedded_list = []
     mimetype_map = {'application/proband+xml': ['text/plain']}
 
     def mimetypes_are_equal(self, m1, m2):
         """ Checks that mime_type m1 and m2 are equal """
         major1 = m1.split('/')[0]
         major2 = m2.split('/')[0]
```

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/types/file.py` & `encoded_core-0.0.0.1b2/src/encoded_core/types/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         'title': 'Files',
         'description': 'Listing of Files',
     })
 class File(Item):
     """Collection for individual files."""
     item_type = 'file'
     base_types = ['File'] + Item.base_types
-    schema = load_schema('encoded-core:schemas/file.json')
+    schema = load_schema('encoded_core:schemas/file.json')
     embedded_list = _build_file_embedded_list()
     name_key = 'accession'
 
     @calculated_property(schema={
         "title": "Display Title",
         "description": "Name of this File",
         "type": "string"
```

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/types/file_format.py` & `encoded_core-0.0.0.1b2/src/encoded_core/types/file_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         'title': 'File Formats',
         'description': 'Listing of file formats used by 4DN'
     }
 )
 class FileFormat(Item, ItemWithAttachment):
     """The class to store information about 4DN file formats"""
     item_type = 'file_format'
-    schema = load_schema('encoded-core:schemas/file_format.json')
+    schema = load_schema('encoded_core:schemas/file_format.json')
     name_key = 'file_format'
 
     @calculated_property(schema={
         "title": "Display Title",
         "description": "File Format name or extension.",
         "type": "string"
     })
```

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/types/file_processed.py` & `encoded_core-0.0.0.1b2/src/encoded_core/types/file_processed.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     properties={
         'title': 'Processed Files',
         'description': 'Listing of Processed Files',
     })
 class FileProcessed(File):
     """Collection for individual processed files."""
     item_type = 'file_processed'
-    schema = load_schema('encoded-core:schemas/file_processed.json')
+    schema = load_schema('encoded_core:schemas/file_processed.json')
     embedded_list = File.embedded_list + file_workflow_run_embeds
     name_key = 'accession'
     rev = dict(File.rev, **{
         'workflow_run_inputs': ('WorkflowRun', 'input_files.value'),
         'workflow_run_outputs': ('WorkflowRun', 'output_files.value'),
     })
     aggregated_items = {
```

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/types/file_reference.py` & `encoded_core-0.0.0.1b2/src/encoded_core/types/file_reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,10 +11,10 @@
     properties={
         'title': 'Reference Files',
         'description': 'Listing of Reference Files',
         })
 class FileReference(File):
     """Collection for individual reference files."""
     item_type = 'file_reference'
-    schema = load_schema('encoded-core:schemas/file_reference.json')
+    schema = load_schema('encoded_core:schemas/file_reference.json')
     embedded_list = File.embedded_list
     name_key = 'accession'
```

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/types/file_submitted.py` & `encoded_core-0.0.0.1b2/src/encoded_core/types/file_submitted.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     properties={
         "title": "Submitted Files",
         "description": "Listing of Submitted Files",
     })
 class FileSubmitted(File):
     """Collection for individual submitted files."""
     item_type = 'file_submitted'
-    schema = load_schema('encoded-core:schemas/file_submitted.json')
+    schema = load_schema('encoded_core:schemas/file_submitted.json')
     embedded_list = _build_file_submitted_embedded_list()
     name_key = 'accession'
     rev = dict(File.rev, **{
         'workflow_run_inputs': ('WorkflowRun', 'input_files.value'),
         'workflow_run_outputs': ('WorkflowRun', 'output_files.value'),
     })
```

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/types/higlass_view_config.py` & `encoded_core-0.0.0.1b2/src/encoded_core/types/higlass_view_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,10 +12,10 @@
     })
 class HiglassViewConfig(Item):
     """
     Item type which contains a `view_config` property and other metadata.
     """
 
     item_type = 'higlass_view_config'
-    schema = load_schema('encoded-core:schemas/higlass_view_config.json')
+    schema = load_schema('encoded_core:schemas/higlass_view_config.json')
     embedded_list = []
     name_key = 'name'
```

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/types/image.py` & `encoded_core-0.0.0.1b2/src/encoded_core/types/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         'title': 'Image',
         'description': 'Listing of portal images',
     })
 class Image(ItemWithAttachment, Item):
     """Class image,defines accepted file types."""
 
     item_type = 'image'
-    schema = load_schema('encoded-core:schemas/image.json')
+    schema = load_schema('encoded_core:schemas/image.json')
     schema['properties']['attachment']['properties']['type']['enum'] = [
         'image/png',
         'image/jpeg',
         'image/gif',
     ]
     embedded_list = Item.embedded_list  # + lab_award_attribution_embed_list
```

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/types/meta_workflow.py` & `encoded_core-0.0.0.1b2/src/encoded_core/types/meta_workflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,20 +60,20 @@
     properties={
         'title': 'MetaWorkflows',
         'description': 'Listing of MetaWorkflows',
     })
 class MetaWorkflow(Item):
     item_type = 'meta_workflow'
     name_key = 'accession'
-    schema = load_schema('encoded-core:schemas/meta_workflow.json')
+    schema = load_schema('encoded_core:schemas/meta_workflow.json')
 
 
 @collection(
     name='meta-workflow-runs',
     properties={
         'title': 'MetaWorkflowRuns',
         'description': 'Listing of MetaWorkflowRuns',
     })
 class MetaWorkflowRun(Item):
     item_type = 'meta_workflow_run'
     embedded_list = _build_meta_workflow_run_embedded_list()
-    schema = load_schema('encoded-core:schemas/meta_workflow_run.json')
+    schema = load_schema('encoded_core:schemas/meta_workflow_run.json')
```

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/types/quality_metric.py` & `encoded_core-0.0.0.1b2/src/encoded_core/types/quality_metric.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,18 +90,31 @@
         'title': 'Quality Metrics',
         'description': 'Listing of quality metrics',
     })
 class QualityMetric(Item):
     """Quality metrics class."""
     item_type = 'quality_metric'
     base_types = ['QualityMetric'] + Item.base_types
-    schema = load_schema('encoded:schemas/quality_metric.json')
+    schema = load_schema('encoded_core:schemas/quality_metric.json')
     embedded_list = Item.embedded_list
 
 
+@collection(
+    name="quality-metrics-generic",
+    properties={
+        "title": "Generic Quality Metrics",
+        "description": "Listing of Generic Quality Metrics",
+    },
+)
+class QualityMetricGeneric(QualityMetric):
+    item_type = "quality_metric_generic"
+    schema = load_schema("encoded_core:schemas/quality_metric_generic.json")
+    embedded_list = QualityMetric.embedded_list
+
+
 def parse_qc_s3_url(url):
     """ Parses the given s3 URL into its pair of bucket, key
         Note that this function works the way it does because of how these
         urls end up in our database. Eventually we should clean this up.
         TODO: use version in utils
         Format:
             https://s3.amazonaws.com/cgap-devtest-main-application-cgap-devtest-wfout/GAPFI1HVXJ5F/fastqc_report.html
```

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/types/software.py` & `encoded_core-0.0.0.1b2/src/encoded_core/types/software.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     properties={
         'title': 'Softwares',
         'description': 'Listing of software for 4DN analyses',
     })
 class Software(Item):
     """The Software class that contains the software... used."""
     item_type = 'software'
-    schema = load_schema('encoded:schemas/software.json')
+    schema = load_schema('encoded_core:schemas/software.json')
     embedded_list = Item.embedded_list  # + lab_award_attribution_embed_list
 
     def _update(self, properties, sheets=None):
         # update self first to ensure 'software_relation' are stored in self.properties
         if 'version' in properties:
             properties['title'] = properties['name'].replace(' ', '-').lower() + '_' + properties['version']
         elif 'commit' in properties:
```

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/types/tracking_item.py` & `encoded_core-0.0.0.1b2/src/encoded_core/types/tracking_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         'title': 'TrackingItem',
         'description': 'For internal tracking of Fourfront events',
     })
 class TrackingItem(Item):
     """tracking-item class."""
 
     item_type = 'tracking_item'
-    schema = load_schema('encoded-core:schemas/tracking_item.json')
+    schema = load_schema('encoded_core:schemas/tracking_item.json')
     embedded_list = []
     STATUS_ACL = Item.STATUS_ACL.copy()
     STATUS_ACL.update({
         'released': ONLY_ADMIN_VIEW_ACL,
         'deleted': DELETED_ACL,
         'draft': ONLY_ADMIN_VIEW_ACL
     })
```

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/types/user_content.py` & `encoded_core-0.0.0.1b2/src/encoded_core/types/user_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     properties={
         'title': "User Content Listing",
         'description': 'Listing of all types of content which may be created by people.',
     })
 class UserContent(Item):
     item_type = 'user_content'
     base_types = ['UserContent'] + Item.base_types
-    schema = load_schema('encoded:schemas/user_content.json')
+    schema = load_schema('encoded_core:schemas/user_content.json')
     embedded_list = []
 
     @calculated_property(schema={
         "title": "Content",
         "description": "Content (unused)",
         "type": "string"
     })
@@ -82,15 +82,15 @@
     properties={
         'title': 'Static Sections',
         'description': 'Static Sections for the Portal',
     })
 class StaticSection(UserContent):
     """The Software class that contains the software... used."""
     item_type = 'static_section'
-    schema = load_schema('encoded:schemas/static_section.json')
+    schema = load_schema('encoded_core:schemas/static_section.json')
 
     @calculated_property(schema={
         "title": "Content",
         "description": "Content for the page",
         "type": "string"
     })
     def content(self, request, body=None, file=None):
```

### Comparing `encoded_core-0.0.0.1b1/src/encoded-core/types/workflow.py` & `encoded_core-0.0.0.1b2/src/encoded_core/types/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         'title': 'Workflows',
         'description': 'Listing of 4DN analysis workflows',
     })
 class Workflow(Item):
     """The Workflow class that describes a workflow and steps in it."""
 
     item_type = 'workflow'
-    schema = load_schema('encoded-core:schemas/workflow.json')
+    schema = load_schema('encoded_core:schemas/workflow.json')
     embedded_list = _build_workflows_embedded_list()
     rev = {
         'newer_versions': ('Workflow', 'previous_version')
     }
 
     @calculated_property(schema={
         "title": "Newer Versions",
@@ -137,15 +137,15 @@
             "type": "string",
             "title": "I/O Type"
         }
     }
 }
 
 
-workflow_schema = load_schema('encoded:schemas/workflow.json')
+workflow_schema = load_schema('encoded_core:schemas/workflow.json')
 workflow_steps_property_schema = workflow_schema.get('properties', {}).get('steps')
 workflow_run_steps_property_schema = copy.deepcopy(workflow_steps_property_schema)
 workflow_run_steps_property_schema['items']['properties']['inputs']['items']['properties']['run_data'] = steps_run_data_schema
 workflow_run_steps_property_schema['items']['properties']['outputs']['items']['properties']['run_data'] = steps_run_data_schema
 
 
 @collection(
@@ -154,15 +154,15 @@
         'title': 'Workflow Runs',
         'description': 'Listing of executions of 4DN analysis workflows',
     })
 class WorkflowRun(Item):
     """The WorkflowRun class that describes execution of a workflow."""
 
     item_type = 'workflow_run'
-    schema = load_schema('encoded:schemas/workflow_run.json')
+    schema = load_schema('encoded_core:schemas/workflow_run.json')
     embedded_list = _build_workflow_run_embedded_list()
 
     @calculated_property(schema=workflow_run_steps_property_schema, category='page')
     def steps(self, request):
         '''
         Extends the 'inputs' & 'outputs' (lists of dicts) properties of calculated property 'analysis_steps' (list of dicts) from
         WorkflowRun's related Workflow with additional property 'run_data', which contains references to Files, Parameters, and Reports
@@ -296,9 +296,9 @@
         'title': 'Workflow Runs AWSEM',
         'description': 'Listing of executions of 4DN analysis workflows on AWSEM platform',
     })
 class WorkflowRunAwsem(WorkflowRun):
     """The WorkflowRun class that describes execution of a workflow on AWSEM platform."""
     base_types = ['WorkflowRun'] + Item.base_types
     item_type = 'workflow_run_awsem'
-    schema = load_schema('encoded:schemas/workflow_run_awsem.json')
+    schema = load_schema('encoded_core:schemas/workflow_run_awsem.json')
     embedded_list = WorkflowRun.embedded_list
```

### Comparing `encoded_core-0.0.0.1b1/setup.py` & `encoded_core-0.0.0.1b2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src'}
 
 packages = \
-['encoded-core', 'encoded-core.types']
+['encoded_core', 'encoded_core.tests', 'encoded_core.types']
 
 package_data = \
-{'': ['*'], 'encoded-core': ['schemas/*']}
+{'': ['*'], 'encoded_core': ['schemas/*']}
 
 install_requires = \
 ['PyJWT>=2.6.0,<3.0.0',
  'SPARQLWrapper>=1.8.5,<2.0.0',
  'SQLAlchemy==1.4.41',
  'WSGIProxy2==0.4.2',
  'WebOb>=1.8.7,<2.0.0',
  'WebTest>=2.0.35,<3.0.0',
  'awscli>=1.25.36',
  'boto3>=1.24.36,<2.0.0',
  'botocore>=1.27.36,<2.0.0',
- 'dcicsnovault>=8.0.1.0b1,<9.0.0.0',
+ 'dcicsnovault>=8.0.1.0b3,<9.0.0.0',
  'dcicutils>=7.0.0,<8.0.0',
  'elasticsearch==7.13.4',
  'jsonschema_serialize_fork>=2.1.1,<3.0.0',
  'plaster-pastedeploy==0.6',
  'psycopg2-binary>=2.9.3,<3.0.0',
  'pyramid-multiauth>=0.9.0,<1',
  'pyramid-retry>=1.0,<2.0',
@@ -43,26 +43,38 @@
  'urllib3>=1.26.4,<2.0.0',
  'venusian>=1.2.0,<2.0.0',
  'waitress>=2.1.1,<3.0.0',
  'zope.deprecation>=4.4.0,<5.0.0',
  'zope.interface>=4.7.2,<5.0.0',
  'zope.sqlalchemy==1.6']
 
+entry_points = \
+{'console_scripts': ['add-image-tag = dcicutils.ecr_scripts:add_image_tag_main',
+                     'show-global-env-bucket = '
+                     'dcicutils.env_scripts:show_global_env_bucket_main',
+                     'show-image-catalog = '
+                     'dcicutils.ecr_scripts:show_image_catalog_main',
+                     'show-image-manifest = '
+                     'dcicutils.ecr_scripts:show_image_manifest_main',
+                     'unrelease-most-recent-image = '
+                     'dcicutils.ecr_scripts:unrelease_most_recent_image_main']}
+
 setup_kwargs = {
     'name': 'encoded-core',
-    'version': '0.0.0.1b1',
+    'version': '0.0.0.1b2',
     'description': 'Core data models for Park Lab ENCODE based projects',
     'long_description': '============\nencoded-core\n============\n\n\nWelcome to ``encoded-core``!\n\nThis library contains common data models used across ENCODE style projects\nimplemented by the Park Lab.',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/smaht-dac/encoded-core',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'entry_points': entry_points,
     'python_requires': '>=3.8.1,<3.10',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `encoded_core-0.0.0.1b1/PKG-INFO` & `encoded_core-0.0.0.1b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encoded-core
-Version: 0.0.0.1b1
+Version: 0.0.0.1b2
 Summary: Core data models for Park Lab ENCODE based projects
 Home-page: https://github.com/smaht-dac/encoded-core
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8.1,<3.10
 Classifier: Development Status :: 3 - Alpha
@@ -22,15 +22,15 @@
 Requires-Dist: SQLAlchemy (==1.4.41)
 Requires-Dist: WSGIProxy2 (==0.4.2)
 Requires-Dist: WebOb (>=1.8.7,<2.0.0)
 Requires-Dist: WebTest (>=2.0.35,<3.0.0)
 Requires-Dist: awscli (>=1.25.36)
 Requires-Dist: boto3 (>=1.24.36,<2.0.0)
 Requires-Dist: botocore (>=1.27.36,<2.0.0)
-Requires-Dist: dcicsnovault (>=8.0.1.0b1,<9.0.0.0)
+Requires-Dist: dcicsnovault (>=8.0.1.0b3,<9.0.0.0)
 Requires-Dist: dcicutils (>=7.0.0,<8.0.0)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: jsonschema_serialize_fork (>=2.1.1,<3.0.0)
 Requires-Dist: plaster-pastedeploy (==0.6)
 Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
 Requires-Dist: pyramid (==1.10.4)
 Requires-Dist: pyramid-multiauth (>=0.9.0,<1)
```

