# Comparing `tmp/jobbergate-api-3.5.0a2.tar.gz` & `tmp/jobbergate_api-3.5.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate-api-3.5.0a2.tar", max compression
+gzip compressed data, was "jobbergate_api-3.5.0a3.tar", max compression
```

## Comparing `jobbergate-api-3.5.0a2.tar` & `jobbergate_api-3.5.0a3.tar`

### file list

```diff
@@ -1,62 +1,61 @@
--rw-r--r--   0        0        0     1082 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/LICENSE
--rw-r--r--   0        0        0      738 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/README.rst
--rw-r--r--   0        0        0      169 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/__init__.py
--rw-r--r--   0        0        0       30 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/__init__.py
--rw-r--r--   0        0        0       41 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/__init__.py
--rw-r--r--   0        0        0     5655 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/application_files.py
--rw-r--r--   0        0        0      234 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/constants.py
--rw-r--r--   0        0        0     9408 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/file_validation.py
--rw-r--r--   0        0        0     1404 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/models.py
--rw-r--r--   0        0        0    13548 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/routers.py
--rw-r--r--   0        0        0     7239 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/schemas.py
--rw-r--r--   0        0        0       40 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_scripts/__init__.py
--rw-r--r--   0        0        0    12157 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_scripts/job_script_files.py
--rw-r--r--   0        0        0     1185 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_scripts/models.py
--rw-r--r--   0        0        0    11747 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_scripts/routers.py
--rw-r--r--   0        0        0     3890 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_scripts/schemas.py
--rw-r--r--   0        0        0       44 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/__init__.py
--rw-r--r--   0        0        0      529 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/constants.py
--rw-r--r--   0        0        0     1910 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/models.py
--rw-r--r--   0        0        0    12331 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/properties_parser.py
--rw-r--r--   0        0        0    18431 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/routers.py
--rw-r--r--   0        0        0    14894 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/schemas.py
--rw-r--r--   0        0        0      554 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/apps/permissions.py
--rw-r--r--   0        0        0     3621 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/config.py
--rw-r--r--   0        0        0     2466 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/email_notification.py
--rw-r--r--   0        0        0     3268 2023-04-27 21:34:03.604115 jobbergate-api-3.5.0a2/jobbergate_api/main.py
--rw-r--r--   0        0        0     3433 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/meta_mapper.py
--rw-r--r--   0        0        0       96 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/metadata.py
--rw-r--r--   0        0        0     3470 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/pagination.py
--rw-r--r--   0        0        0     2284 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/s3_manager.py
--rw-r--r--   0        0        0     2166 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/security.py
--rw-r--r--   0        0        0     5580 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/storage.py
--rw-r--r--   0        0        0       40 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/__init__.py
--rw-r--r--   0        0        0       28 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/__init__.py
--rw-r--r--   0        0        0       44 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/applications/__init__.py
--rw-r--r--   0        0        0    10634 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/applications/test_application_files.py
--rw-r--r--   0        0        0     1967 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/applications/test_file_validation.py
--rw-r--r--   0        0        0    41708 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/applications/test_routers.py
--rw-r--r--   0        0        0     5180 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/applications/test_schemas.py
--rw-r--r--   0        0        0     2756 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/conftest.py
--rw-r--r--   0        0        0       42 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_scripts/__init__.py
--rw-r--r--   0        0        0     1376 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_scripts/conftest.py
--rw-r--r--   0        0        0    11518 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py
--rw-r--r--   0        0        0    42583 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_scripts/test_routers.py
--rw-r--r--   0        0        0       46 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_submissions/__init__.py
--rw-r--r--   0        0        0    23970 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py
--rw-r--r--   0        0        0    78149 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_submissions/test_routers.py
--rw-r--r--   0        0        0      511 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/test_main.py
--rw-r--r--   0        0        0     8900 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/conftest.py
--rw-r--r--   0        0        0     4503 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py
--rw-r--r--   0        0        0     3215 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/test_config.py
--rw-r--r--   0        0        0     4974 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/test_email_notification.py
--rw-r--r--   0        0        0     3177 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/test_meta_mapper.py
--rw-r--r--   0        0        0     3959 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/test_pagination.py
--rw-r--r--   0        0        0     1146 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/test_s3_manager.py
--rw-r--r--   0        0        0     2718 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/test_security.py
--rw-r--r--   0        0        0     4512 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/test_storage.py
--rw-r--r--   0        0        0     2777 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/tests/test_version.py
--rw-r--r--   0        0        0     1102 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/jobbergate_api/version.py
--rw-r--r--   0        0        0     2904 2023-04-27 21:34:03.608115 jobbergate-api-3.5.0a2/pyproject.toml
--rw-r--r--   0        0        0     2488 2023-04-27 21:34:22.967130 jobbergate-api-3.5.0a2/setup.py
--rw-r--r--   0        0        0     2657 2023-04-27 21:34:22.967521 jobbergate-api-3.5.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-09 14:04:29.803973 jobbergate_api-3.5.0a3/LICENSE
+-rw-r--r--   0        0        0      738 2023-05-09 14:04:29.803973 jobbergate_api-3.5.0a3/README.rst
+-rw-r--r--   0        0        0      169 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/__init__.py
+-rw-r--r--   0        0        0       30 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/__init__.py
+-rw-r--r--   0        0        0     5655 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/application_files.py
+-rw-r--r--   0        0        0      234 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/constants.py
+-rw-r--r--   0        0        0     9408 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/file_validation.py
+-rw-r--r--   0        0        0     1474 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/models.py
+-rw-r--r--   0        0        0    14123 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/routers.py
+-rw-r--r--   0        0        0     7421 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/schemas.py
+-rw-r--r--   0        0        0       40 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_scripts/__init__.py
+-rw-r--r--   0        0        0    12157 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_scripts/job_script_files.py
+-rw-r--r--   0        0        0     1287 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_scripts/models.py
+-rw-r--r--   0        0        0    15623 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_scripts/routers.py
+-rw-r--r--   0        0        0     4088 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_scripts/schemas.py
+-rw-r--r--   0        0        0       44 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/__init__.py
+-rw-r--r--   0        0        0      529 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/constants.py
+-rw-r--r--   0        0        0     1909 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/models.py
+-rw-r--r--   0        0        0    12331 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/properties_parser.py
+-rw-r--r--   0        0        0    18431 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/routers.py
+-rw-r--r--   0        0        0    14904 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/schemas.py
+-rw-r--r--   0        0        0      554 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/permissions.py
+-rw-r--r--   0        0        0     3621 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/config.py
+-rw-r--r--   0        0        0     2466 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/email_notification.py
+-rw-r--r--   0        0        0     3268 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/main.py
+-rw-r--r--   0        0        0     3433 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/meta_mapper.py
+-rw-r--r--   0        0        0       96 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/metadata.py
+-rw-r--r--   0        0        0     3470 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/pagination.py
+-rw-r--r--   0        0        0     2284 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/s3_manager.py
+-rw-r--r--   0        0        0     2166 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/security.py
+-rw-r--r--   0        0        0     5580 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/storage.py
+-rw-r--r--   0        0        0       40 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/__init__.py
+-rw-r--r--   0        0        0       44 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/applications/__init__.py
+-rw-r--r--   0        0        0    10634 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/applications/test_application_files.py
+-rw-r--r--   0        0        0     1967 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/applications/test_file_validation.py
+-rw-r--r--   0        0        0    44032 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/applications/test_routers.py
+-rw-r--r--   0        0        0     5180 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/applications/test_schemas.py
+-rw-r--r--   0        0        0     2756 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/conftest.py
+-rw-r--r--   0        0        0       42 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_scripts/__init__.py
+-rw-r--r--   0        0        0     1376 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_scripts/conftest.py
+-rw-r--r--   0        0        0    11518 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py
+-rw-r--r--   0        0        0    52389 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_scripts/test_routers.py
+-rw-r--r--   0        0        0       46 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_submissions/__init__.py
+-rw-r--r--   0        0        0    23970 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py
+-rw-r--r--   0        0        0    78149 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_submissions/test_routers.py
+-rw-r--r--   0        0        0      511 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/test_main.py
+-rw-r--r--   0        0        0     8900 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/conftest.py
+-rw-r--r--   0        0        0     4503 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py
+-rw-r--r--   0        0        0     3215 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/test_config.py
+-rw-r--r--   0        0        0     4974 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/test_email_notification.py
+-rw-r--r--   0        0        0     3177 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/test_meta_mapper.py
+-rw-r--r--   0        0        0     3959 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/test_pagination.py
+-rw-r--r--   0        0        0     1146 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/test_s3_manager.py
+-rw-r--r--   0        0        0     2718 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/test_security.py
+-rw-r--r--   0        0        0     4512 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/test_storage.py
+-rw-r--r--   0        0        0     2777 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/test_version.py
+-rw-r--r--   0        0        0     1102 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/version.py
+-rw-r--r--   0        0        0     2904 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/pyproject.toml
+-rw-r--r--   0        0        0     2756 1970-01-01 00:00:00.000000 jobbergate_api-3.5.0a3/PKG-INFO
```

### Comparing `jobbergate-api-3.5.0a2/LICENSE` & `jobbergate_api-3.5.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/README.rst` & `jobbergate_api-3.5.0a3/README.rst`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/application_files.py` & `jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/application_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/file_validation.py` & `jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/file_validation.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/models.py` & `jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Column("application_name", String, nullable=False, index=True),
     Column("application_identifier", String, unique=True, index=True),
     Column("application_description", String, default=""),
     Column("application_owner_email", String, nullable=False, index=True),
     Column("application_uploaded", Boolean, nullable=False, default=False_()),
     Column("created_at", DateTime, nullable=False, default=func.now()),
     Column("updated_at", DateTime, nullable=False, default=func.now(), onupdate=func.now()),
+    Column("is_archived", Boolean, nullable=False, default=False_()),
 )
 
 searchable_fields = [
     applications_table.c.application_name,
     applications_table.c.application_identifier,
     applications_table.c.application_description,
     applications_table.c.application_owner_email,
```

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/routers.py` & `jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/routers.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from jobbergate_api.apps.applications.models import applications_table, searchable_fields, sortable_fields
 from jobbergate_api.apps.applications.schemas import (
     ApplicationCreateRequest,
     ApplicationPartialResponse,
     ApplicationResponse,
     ApplicationUpdateRequest,
 )
+from jobbergate_api.apps.job_scripts.models import job_scripts_table
 from jobbergate_api.apps.permissions import Permissions
 from jobbergate_api.config import settings
 from jobbergate_api.pagination import Pagination, ok_response, package_response
 from jobbergate_api.security import IdentityClaims, guard
 from jobbergate_api.storage import (
     INTEGRITY_CHECK_EXCEPTIONS,
     database,
@@ -183,16 +184,26 @@
     description="Endpoint to delete application",
     dependencies=[Depends(guard.lockdown(Permissions.APPLICATIONS_EDIT))],
 )
 async def application_delete(
     application_id: int = Query(..., description="id of the application to delete"),
 ):
     """
-    Delete application from the database and S3 given it's id.
+    Delete application from the database and S3 given its id.
     """
+    logger.debug(f"Orphaning job_scripts rendered from application {application_id=}")
+    update_query = (
+        job_scripts_table.update()
+        .where(job_scripts_table.c.application_id == application_id)
+        .values(dict(application_id=None))
+    )
+
+    logger.trace(f"update_query = {render_sql(update_query)}")
+    await database.execute(update_query)
+
     logger.debug(f"Preparing to delete {application_id=} from the database and S3")
 
     where_stmt = applications_table.c.id == application_id
     get_query = applications_table.select().where(where_stmt)
     logger.trace(f"get_query = {render_sql(get_query)}")
 
     raw_application = await database.fetch_one(get_query)
@@ -256,14 +267,15 @@
     "/applications",
     description="Endpoint to list applications",
     responses=ok_response(ApplicationPartialResponse),
 )
 async def applications_list(
     user: bool = Query(False),
     all: bool = Query(False),
+    include_archived: bool = Query(False),
     search: Optional[str] = Query(None),
     sort_field: Optional[str] = Query(None),
     sort_ascending: bool = Query(True),
     pagination: Pagination = Depends(),
     token_payload: TokenPayload = Depends(guard.lockdown(Permissions.APPLICATIONS_VIEW)),
 ):
     """
@@ -273,14 +285,16 @@
 
     identity_claims = IdentityClaims.from_token_payload(token_payload)
     query = applications_table.select()
     if user:
         query = query.where(applications_table.c.application_owner_email == identity_claims.email)
     if not all:
         query = query.where(not_(applications_table.c.application_identifier.is_(None)))
+    if not include_archived:
+        query = query.where(not_(applications_table.c.is_archived))
     if search is not None:
         query = query.where(search_clause(search, searchable_fields))
     if sort_field is not None:
         query = query.order_by(sort_clause(sort_field, sortable_fields, sort_ascending))
 
     logger.trace(f"query = {render_sql(query)}")
     return await package_response(ApplicationPartialResponse, query, pagination)
```

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/apps/applications/schemas.py` & `jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,18 @@
             """
         ).strip(),
     ),
     application_uploaded=MetaField(
         description="Indicates if the application file zip has been uploaded yet.",
         example=True,
     ),
+    is_archived=MetaField(
+        description="Indicates if the application has been archived.",
+        example=False,
+    ),
 )
 
 
 class JobbergateConfig(BaseModel):
     """
     Model for Jobbergate configuration (subsection at the yaml file).
     """
@@ -183,14 +187,15 @@
     Request model for updating Application instances.
     """
 
     application_name: Optional[str]
     application_identifier: Optional[str]
     application_description: Optional[str]
     application_config: Optional[str]
+    is_archived: Optional[bool]
 
     class Config:
         schema_extra = application_meta_mapper
 
 
 class ApplicationPartialResponse(BaseModel):
     """
@@ -201,14 +206,15 @@
     created_at: Optional[datetime] = datetime.utcnow()
     updated_at: Optional[datetime] = datetime.utcnow()
     application_name: str
     application_identifier: Optional[str]
     application_description: Optional[str]
     application_owner_email: str
     application_uploaded: bool
+    is_archived: bool
 
     class Config:
         orm_mode = True
         schema_extra = application_meta_mapper
 
 
 class ApplicationResponse(ApplicationPartialResponse):
```

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/apps/job_scripts/job_script_files.py` & `jobbergate_api-3.5.0a3/jobbergate_api/apps/job_scripts/job_script_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/apps/job_scripts/models.py` & `jobbergate_api-3.5.0a3/jobbergate_api/apps/job_scripts/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """
 Database model for the JobScript resource.
 """
-from sqlalchemy import DateTime, ForeignKey, Integer, String, Table
-from sqlalchemy.sql import func
+from sqlalchemy import Boolean, DateTime, ForeignKey, Integer, String, Table
+from sqlalchemy.sql import False_, func
 from sqlalchemy.sql.schema import Column
 
 from jobbergate_api.metadata import metadata
 
 job_scripts_table = Table(
     "job_scripts",
     metadata,
     Column("id", Integer, primary_key=True),
     Column("job_script_name", String, nullable=False, index=True),
     Column("job_script_description", String, default=""),
     Column("job_script_owner_email", String, nullable=False, index=True),
-    Column("application_id", ForeignKey("applications.id")),
+    Column("application_id", ForeignKey("applications.id"), nullable=True),
     Column("created_at", DateTime, nullable=False, default=func.now()),
     Column("updated_at", DateTime, nullable=False, default=func.now(), onupdate=func.now()),
+    Column("is_archived", Boolean, nullable=False, default=False_()),
 )
 
 searchable_fields = [
     job_scripts_table.c.job_script_name,
     job_scripts_table.c.job_script_description,
     job_scripts_table.c.job_script_owner_email,
 ]
```

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/apps/job_scripts/routers.py` & `jobbergate_api-3.5.0a3/jobbergate_api/apps/job_scripts/routers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-"""
-Router for the JobScript resource.
-"""
+"""Router for the JobScript resource."""
 from typing import Optional
 
 from armasec import TokenPayload
-from fastapi import APIRouter, Depends, HTTPException, Query, status
+from fastapi import APIRouter, Depends, File, HTTPException, Query, UploadFile, status
+from fastapi.responses import PlainTextResponse
 from loguru import logger
-from sqlalchemy import join, select
+from sqlalchemy import join, not_, select
+from sqlalchemy.sql import func
 
 from jobbergate_api.apps.applications.application_files import ApplicationFiles
 from jobbergate_api.apps.applications.models import applications_table
 from jobbergate_api.apps.applications.schemas import ApplicationResponse
-from jobbergate_api.apps.job_scripts.job_script_files import JobScriptCreationError, JobScriptFiles
+from jobbergate_api.apps.job_scripts.job_script_files import (
+    JOBSCRIPTS_MAIN_FILE_FOLDER,
+    JobScriptCreationError,
+    JobScriptFiles,
+)
 from jobbergate_api.apps.job_scripts.models import job_scripts_table, searchable_fields, sortable_fields
 from jobbergate_api.apps.job_scripts.schemas import (
     JobScriptCreateRequest,
     JobScriptPartialResponse,
     JobScriptResponse,
     JobScriptUpdateRequest,
 )
+from jobbergate_api.apps.job_submissions.models import job_submissions_table
 from jobbergate_api.apps.permissions import Permissions
 from jobbergate_api.pagination import Pagination, ok_response, package_response
 from jobbergate_api.security import IdentityClaims, guard
 from jobbergate_api.storage import (
     INTEGRITY_CHECK_EXCEPTIONS,
     database,
     render_sql,
@@ -171,22 +176,99 @@
         )
 
     logger.debug(f"Job-script data: {response}")
 
     return response
 
 
+@router.patch(
+    "/job-scripts/{job_script_id}/upload",
+    status_code=status.HTTP_204_NO_CONTENT,
+    description="Endpoint to replace a job script file.",
+    dependencies=[Depends(guard.lockdown(Permissions.JOB_SCRIPTS_EDIT))],
+)
+async def job_script_replace_file_content(
+    job_script_id: int = Query(...),
+    job_script_file: UploadFile = File(...),
+):
+    """Replace the content on a job script file."""
+    logger.debug(f"Replacing the main file from {job_script_id=}")
+
+    query = job_scripts_table.select().where(job_scripts_table.c.id == job_script_id)
+    logger.trace(f"get_query = {render_sql(query)}")
+    job_script = await database.fetch_one(query)
+
+    if not job_script:
+        message = f"JobScript with id={job_script_id} was not found."
+        logger.warning(message)
+        raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=message)
+
+    file_manager = JobScriptFiles.file_manager_factory(job_script_id)
+    file_content = job_script_file.file.read().decode("utf-8")
+
+    for s3_path in file_manager.keys():
+        root_dir = s3_path.parts[0]
+        if root_dir == JOBSCRIPTS_MAIN_FILE_FOLDER:
+            file_manager[s3_path] = file_content
+            update_query = (
+                job_scripts_table.update()
+                .where(job_scripts_table.c.id == job_script["id"])
+                .values(updated_at=func.now())
+            )
+            await database.execute(update_query)
+            logger.debug(f"Success replacing the main file from {job_script_id=}")
+            return None
+
+    message = f"Main file from {job_script_id=} was not found."
+    logger.warning(message)
+    raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=message)
+
+
+@router.get(
+    "/job-scripts/{job_script_id}/download",
+    status_code=status.HTTP_200_OK,
+    description="Endpoint to download a job script file.",
+    dependencies=[Depends(guard.lockdown(Permissions.JOB_SCRIPTS_VIEW))],
+)
+async def job_script_download_file(job_script_id: int = Query(...)):
+    """Download the job script file."""
+    logger.debug(f"Downloading main file from {job_script_id=}")
+
+    query = job_scripts_table.select().where(job_scripts_table.c.id == job_script_id)
+    logger.trace(f"get_query = {render_sql(query)}")
+    job_script = await database.fetch_one(query)
+
+    if not job_script:
+        message = f"JobScript with id={job_script_id} was not found."
+        logger.warning(message)
+        raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=message)
+
+    file_manager = JobScriptFiles.file_manager_factory(job_script_id)
+
+    for s3_path in file_manager.keys():
+        root_dir = s3_path.parts[0]
+        if root_dir == JOBSCRIPTS_MAIN_FILE_FOLDER:
+            file_content = file_manager[s3_path]
+            filename = s3_path.relative_to(JOBSCRIPTS_MAIN_FILE_FOLDER).as_posix()
+            return PlainTextResponse(file_content, media_type="text/plain", headers={"filename": filename})
+
+    message = f"Main file from {job_script_id=} was not found."
+    logger.warning(message)
+    raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=message)
+
+
 @router.get(
     "/job-scripts",
     description="Endpoint to list job_scripts",
     responses=ok_response(JobScriptPartialResponse),
 )
 async def job_script_list(
     pagination: Pagination = Depends(),
     all: Optional[bool] = Query(False),
+    include_archived: bool = Query(False),
     search: Optional[str] = Query(None),
     sort_field: Optional[str] = Query(None),
     from_application_id: Optional[int] = Query(
         None,
         description="Filter job-scripts by the application-id they were created from.",
     ),
     sort_ascending: bool = Query(True),
@@ -209,14 +291,16 @@
             applications_table,
             applications_table.c.id == job_scripts_table.c.application_id,
         )
     )
     identity_claims = IdentityClaims.from_token_payload(token_payload)
     if not all:
         query = query.where(job_scripts_table.c.job_script_owner_email == identity_claims.email)
+    if not include_archived:
+        query = query.where(not_(job_scripts_table.c.is_archived))
     if from_application_id is not None:
         query = query.where(job_scripts_table.c.application_id == from_application_id)
     if search is not None:
         query = query.where(search_clause(search, searchable_fields))
     if sort_field is not None:
         query = query.order_by(sort_clause(sort_field, sortable_fields, sort_ascending))
     else:
@@ -232,14 +316,23 @@
     description="Endpoint to delete job script",
     dependencies=[Depends(guard.lockdown(Permissions.JOB_SCRIPTS_EDIT))],
 )
 async def job_script_delete(job_script_id: int = Query(..., description="id of the job script to delete")):
     """
     Delete job_script given its id.
     """
+    logger.debug(f"Orphaning job_submissions submitted from job_script {job_script_id=}")
+    update_query = (
+        job_submissions_table.update()
+        .where(job_submissions_table.c.job_script_id == job_script_id)
+        .values(dict(job_script_id=None))
+    )
+    logger.trace(f"update_query = {render_sql(update_query)}")
+    await database.execute(update_query)
+
     logger.debug(f"Preparing to delete {job_script_id=}")
     where_stmt = job_scripts_table.c.id == job_script_id
 
     get_query = job_scripts_table.select().where(where_stmt)
     logger.trace(f"get_query = {render_sql(get_query)}")
 
     raw_job_script = await database.fetch_one(get_query)
```

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/apps/job_scripts/schemas.py` & `jobbergate_api-3.5.0a3/jobbergate_api/apps/job_scripts/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,18 @@
         description="SBATCH parameters to inject into the job_script",
         example=["alpha", "beta", "delta"],
     ),
     param_dict=MetaField(
         description="Parameters to use when rendering the job_script jinja2 template",
         example={"param1": 7, "param2": 13},
     ),
+    is_archived=MetaField(
+        description="Indicates if the job_script has been archived.",
+        example=False,
+    ),
 )
 
 
 class JobScriptCreateRequest(BaseModel):
     """
     Request model for creating JobScript instances.
     """
@@ -81,14 +85,15 @@
     """
 
     job_script_name: Optional[str]
     job_script_description: Optional[str]
     job_script_files: Optional[JobScriptFiles]
     sbatch_params: Optional[List[str]]
     param_dict: Optional[str]
+    is_archived: Optional[bool]
 
     class Config:
         schema_extra = job_script_meta_mapper
 
 
 class JobScriptPartialResponse(BaseModel):
     """
@@ -99,16 +104,17 @@
 
     id: Optional[int] = None
     created_at: Optional[datetime] = None
     updated_at: Optional[datetime] = None
     job_script_name: str
     job_script_description: Optional[str] = None
     job_script_owner_email: str
-    application_id: int
     application_name: Optional[str] = None
+    application_id: Optional[int] = None
+    is_archived: bool
 
     class Config:
         orm_mode = True
         schema_extra = job_script_meta_mapper
 
 
 class JobScriptResponse(JobScriptPartialResponse):
```

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/constants.py` & `jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/constants.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/models.py` & `jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 job_submissions_table = Table(
     "job_submissions",
     metadata,
     Column("id", Integer, primary_key=True),
     Column("job_submission_name", String, nullable=False, index=True),
     Column("job_submission_description", String, default=""),
     Column("job_submission_owner_email", String, nullable=False, index=True),
-    Column("job_script_id", ForeignKey("job_scripts.id"), nullable=False),
+    Column("job_script_id", ForeignKey("job_scripts.id"), nullable=True),
     Column("execution_directory", String),
     Column("slurm_job_id", Integer, default=None),
     Column("client_id", String, nullable=False, index=True),
     Column("status", Enum(JobSubmissionStatus), nullable=False, index=True),
     Column("report_message", String, nullable=True),
     Column("created_at", DateTime, nullable=False, default=func.now()),
     Column("updated_at", DateTime, nullable=False, default=func.now(), onupdate=func.now()),
```

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/properties_parser.py` & `jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/properties_parser.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/routers.py` & `jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/apps/job_submissions/schemas.py` & `jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
 
     id: Optional[int] = Field(None)
     created_at: Optional[datetime]
     updated_at: Optional[datetime]
     job_submission_name: str
     job_submission_description: Optional[str]
     job_submission_owner_email: str
-    job_script_id: int
+    job_script_id: Optional[int]
     execution_directory: Optional[Path]
     slurm_job_id: Optional[int]
     client_id: Optional[str]
     status: JobSubmissionStatus
     report_message: Optional[str]
     execution_parameters: Optional[JobProperties]
     job_script_name: Optional[str] = None
```

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/apps/permissions.py` & `jobbergate_api-3.5.0a3/jobbergate_api/apps/permissions.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/config.py` & `jobbergate_api-3.5.0a3/jobbergate_api/config.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/email_notification.py` & `jobbergate_api-3.5.0a3/jobbergate_api/email_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/main.py` & `jobbergate_api-3.5.0a3/jobbergate_api/main.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/meta_mapper.py` & `jobbergate_api-3.5.0a3/jobbergate_api/meta_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/pagination.py` & `jobbergate_api-3.5.0a3/jobbergate_api/pagination.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/s3_manager.py` & `jobbergate_api-3.5.0a3/jobbergate_api/s3_manager.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/security.py` & `jobbergate_api-3.5.0a3/jobbergate_api/security.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/storage.py` & `jobbergate_api-3.5.0a3/jobbergate_api/storage.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/applications/test_application_files.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/applications/test_application_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/applications/test_file_validation.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/applications/test_file_validation.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/applications/test_routers.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/applications/test_routers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """
 Tests for the /applications/ endpoint.
 """
-import json
 from unittest import mock
 
-import asyncpg
 import pytest
 from fastapi import status
 
 from jobbergate_api.apps.applications.application_files import ApplicationFiles
 from jobbergate_api.apps.applications.models import applications_table
 from jobbergate_api.apps.applications.schemas import ApplicationPartialResponse
+from jobbergate_api.apps.job_scripts.models import job_scripts_table
 from jobbergate_api.apps.permissions import Permissions
 from jobbergate_api.storage import database, fetch_instance
 
 # Force the async event loop at the app to begin.
 # Since this is a time consuming fixture, it is just used where strict necessary.
 pytestmark = pytest.mark.usefixtures("startup_event_force")
 
@@ -241,48 +240,60 @@
     """
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_EDIT)
     response = await client.delete("/jobbergate/applications/999")
     assert response.status_code == status.HTTP_404_NOT_FOUND
 
 
 @pytest.mark.asyncio
-async def test_delete_application__fk_error(
+@mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.delete_from_s3")
+async def test_delete_application__unlinks_job_scripts(
+    mocked_application_deleter,
     client,
     application_data,
+    job_script_data,
     inject_security_header,
 ):
     """
-    Test DELETE /applications/<id> correctly returns a 409 when a foreign-key error occurs.
+    Test DELETE /applications/<id> correctly deletes an application linked to a job_script.
 
-    Test that a helpful message when a delete is blocked by a foreign-key constraint.
+    Test that a the application_id field for connected job_scripts is set to null.
     """
     inserted_id = await database.execute(
         query=applications_table.insert(),
         values=application_data,
     )
     count = await database.fetch_all("SELECT COUNT(*) FROM applications")
     assert count[0][0] == 1
 
+    await database.execute(
+        query=job_scripts_table.insert(),
+        values=dict(
+            **job_script_data,
+            application_id=inserted_id,
+        ),
+    )
+    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
+    assert count[0][0] == 1
+    count = await database.fetch_all(
+        "SELECT COUNT(*) FROM job_scripts where application_id=:inserted_id",
+        values=dict(inserted_id=inserted_id),
+    )
+    assert count[0][0] == 1
+
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_EDIT)
-    with mock.patch(
-        "jobbergate_api.storage.database.execute",
-        side_effect=asyncpg.exceptions.ForeignKeyViolationError(
-            f"""
-            update or delete on table "applications" violates foreign key constraint
-            "job_scripts_application_id_fkey" on table "job_scripts"
-            DETAIL:  Key (id)=({inserted_id}) is still referenced from table "job_scripts".
-            """
-        ),
-    ):
-        response = await client.delete(f"/jobbergate/applications/{inserted_id}")
-    assert response.status_code == status.HTTP_409_CONFLICT
-    error_data = json.loads(response.text)["detail"]
-    assert error_data["message"] == "Delete failed due to foreign-key constraint"
-    assert error_data["table"] == "job_scripts"
-    assert error_data["pk_id"] == f"{inserted_id}"
+    response = await client.delete(f"/jobbergate/applications/{inserted_id}")
+    assert response.status_code == status.HTTP_204_NO_CONTENT
+    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
+    assert count[0][0] == 0
+
+    count = await database.fetch_all(
+        "SELECT COUNT(*) FROM job_scripts where application_id=:inserted_id",
+        values=dict(inserted_id=inserted_id),
+    )
+    assert count[0][0] == 0
 
 
 @pytest.mark.asyncio
 async def test_get_application_by_id__files_not_uploaded(
     client,
     fill_application_data,
     inject_security_header,
@@ -415,26 +426,28 @@
     inject_security_header,
 ):
     """
     Test GET /applications returns only applications owned by the user making the request.
 
     This test proves that GET /applications returns the correct applications for the user making
     the request. We show this by asserting that the applications returned in the response are
-    only applications owned by the user making the request.
+    only applications owned by the user making the request. This test also ensures that archived
+    applications are not included by default.
     """
     await database.execute_many(
         applications_table.insert(),
         values=fill_all_application_data(
             dict(application_identifier="app1"),
             dict(application_identifier="app2"),
             dict(application_identifier="app3"),
+            dict(application_identifier="app4", is_archived=True),
         ),
     )
     count = await database.fetch_all("SELECT COUNT(*) FROM applications")
-    assert count[0][0] == 3
+    assert count[0][0] == 4
 
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_VIEW)
     response = await client.get("/jobbergate/applications/")
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
     results = data.get("results")
@@ -490,15 +503,15 @@
 ):
     """
     Test applications list doesn't include applications owned by other users with `user` param.
 
     This test proves that the user making the request cannot see applications owned by other users.
     We show this by creating applications that are owned by another user id and assert that
     the user making the request to list applications doesn't see any of the other user's
-    applications in the response
+    applications in the response.
     """
     await database.execute_many(
         query=applications_table.insert(),
         values=fill_all_application_data(
             dict(
                 application_identifier="app1",
                 application_owner_email="owner1@org.com",
@@ -597,14 +610,67 @@
         total=3,
         start=None,
         limit=None,
     )
 
 
 @pytest.mark.asyncio
+async def test_get_applications__with_include_archived_param(
+    client,
+    fill_all_application_data,
+    inject_security_header,
+):
+    """
+    Test that listing applications, when include_archived=True, contains archived applications.
+
+    This test proves that the user making the request can see archived applications.
+    We show this by creating three applications, two that are normal, and one that is archived.
+    Assert that the response to GET /applications/?include_archived=True includes all three applications.
+    """
+    await database.execute_many(
+        query=applications_table.insert(),
+        values=fill_all_application_data(
+            dict(application_identifier="app1"),
+            dict(application_identifier="app2", is_archived=True),
+            dict(application_identifier="app3"),
+        ),
+    )
+    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
+    assert count[0][0] == 3
+
+    inject_security_header("owner1@org.com", Permissions.APPLICATIONS_VIEW)
+
+    response = await client.get("/jobbergate/applications")
+    assert response.status_code == status.HTTP_200_OK
+
+    data = response.json()
+    results = data.get("results")
+    assert [d["application_identifier"] for d in results] == ["app1", "app3"]
+
+    pagination = data.get("pagination")
+    assert pagination == dict(
+        total=2,
+        start=None,
+        limit=None,
+    )
+
+    response = await client.get("/jobbergate/applications/?include_archived=True")
+    assert response.status_code == status.HTTP_200_OK
+
+    data = response.json()
+    results = data.get("results")
+    pagination = data.get("pagination")
+    assert pagination == dict(
+        total=3,
+        start=None,
+        limit=None,
+    )
+
+
+@pytest.mark.asyncio
 async def test_get_applications__with_search_param(
     client,
     fill_all_application_data,
     inject_security_header,
 ):
     """
     Test that listing applications, when search=<search terms>, returns matches.
@@ -823,31 +889,34 @@
     with time_frame() as window:
         response = await client.put(
             f"/jobbergate/applications/{id}",
             json=dict(
                 application_name="new_name",
                 application_identifier="new_identifier",
                 application_description="new_description",
+                is_archived=True,
             ),
         )
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
     assert data["application_name"] == "new_name"
     assert data["application_identifier"] == "new_identifier"
     assert data["application_description"] == "new_description"
+    assert data["is_archived"] is True
 
     query = applications_table.select(applications_table.c.id == id)
     result = await database.fetch_one(query)
 
     assert result is not None
     assert result["application_name"] == "new_name"
     assert result["application_identifier"] == "new_identifier"
     assert result["application_owner_email"] == "owner1@org.com"
     assert result["application_description"] == "new_description"
+    assert result["is_archived"] is True
     assert result["updated_at"] in window
 
 
 @pytest.mark.asyncio
 async def test_update_application_bad_permission(
     client,
     fill_application_data,
```

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/applications/test_schemas.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/applications/test_schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/conftest.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_scripts/conftest.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_scripts/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_scripts/test_routers.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_scripts/test_routers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """
 Tests for the /job-scripts/ endpoint.
 """
-import json
 import pathlib
 from textwrap import dedent
 from unittest import mock
 
-import asyncpg
 import pytest
 from fastapi import status
 
 from jobbergate_api.apps.applications.application_files import ApplicationFiles
 from jobbergate_api.apps.applications.models import applications_table
 from jobbergate_api.apps.job_scripts.job_script_files import JobScriptFiles
 from jobbergate_api.apps.job_scripts.models import job_scripts_table
 from jobbergate_api.apps.job_scripts.schemas import JobScriptPartialResponse, JobScriptResponse
+from jobbergate_api.apps.job_submissions.models import job_submissions_table
 from jobbergate_api.apps.permissions import Permissions
 from jobbergate_api.storage import database
 
 # Force the async event loop at the app to begin.
 # Since this is a time consuming fixture, it is just used where strict necessary.
 pytestmark = pytest.mark.usefixtures("startup_event_force")
 
@@ -390,14 +389,208 @@
     assert data["job_script_owner_email"] == "owner1@org.com"
     assert data["application_id"] == inserted_application_id
     assert JobScriptFiles(**data["job_script_files"]) == dummy_job_script_files
 
 
 @pytest.mark.asyncio
 @database.transaction(force_rollback=True)
+async def test_download_job_script_file_by_id__success(
+    client,
+    fill_job_script_data,
+    inject_security_header,
+    mocked_file_manager_factory,
+):
+    """Test that a job script file can be downloaded."""
+    inserted_job_script_id = await database.execute(
+        query=job_scripts_table.insert(),
+        values=fill_job_script_data(),
+    )
+
+    main_file_path = pathlib.Path("jobbergate.py")
+    expected_file_content = "print(__name__)"
+
+    dummy_job_script_files = JobScriptFiles(
+        main_file_path=main_file_path, files={main_file_path: expected_file_content}
+    )
+    dummy_job_script_files.write_to_s3(inserted_job_script_id)
+
+    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
+    assert count[0][0] == 1
+
+    inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_VIEW)
+    response = await client.get(f"/jobbergate/job-scripts/{inserted_job_script_id}/download")
+
+    assert response.status_code == status.HTTP_200_OK
+
+    assert response.read() == expected_file_content.encode()
+    assert response.headers["filename"] == main_file_path.as_posix()
+
+
+@pytest.mark.asyncio
+@database.transaction(force_rollback=True)
+async def test_download_job_script_file_by_id__job_script_not_found(
+    client,
+    inject_security_header,
+):
+    """Test that a job script file can not be downloaded when its id is not found at the database."""
+    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
+    assert count[0][0] == 0
+
+    inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_VIEW)
+    response = await client.get("/jobbergate/job-scripts/1/download")
+
+    assert response.status_code == status.HTTP_404_NOT_FOUND
+    assert "JobScript with id=1 was not found." in response.text
+
+
+@pytest.mark.asyncio
+@database.transaction(force_rollback=True)
+async def test_download_job_script_file_by_id__job_script_file_not_found(
+    client,
+    fill_job_script_data,
+    inject_security_header,
+    mocked_file_manager_factory,
+):
+    """Test that a job script file can not be downloaded when its not found at s3."""
+    inserted_job_script_id = await database.execute(
+        query=job_scripts_table.insert(),
+        values=fill_job_script_data(),
+    )
+
+    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
+    assert count[0][0] == 1
+
+    inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_VIEW)
+    response = await client.get(f"/jobbergate/job-scripts/{inserted_job_script_id}/download")
+
+    assert response.status_code == status.HTTP_404_NOT_FOUND
+    assert f"Main file from job_script_id={inserted_job_script_id} was not found." in response.text
+
+
+@pytest.mark.asyncio
+@database.transaction(force_rollback=True)
+async def test_upload_job_script_file_by_id__success(
+    client,
+    fill_job_script_data,
+    inject_security_header,
+    make_dummy_file,
+    time_frame,
+    mocked_file_manager_factory,
+):
+    """Test that a job script file can be uploaded."""
+    inserted_job_script_id = await database.execute(
+        query=job_scripts_table.insert(),
+        values=fill_job_script_data(),
+    )
+
+    main_file_path = pathlib.Path("jobbergate.py")
+
+    old_file_content = "I'm going to be replaced"
+    new_file_content = "I'm the new content"
+
+    dummy_job_script_files = JobScriptFiles(
+        main_file_path=main_file_path, files={main_file_path: old_file_content}
+    )
+    dummy_job_script_files.write_to_s3(inserted_job_script_id)
+
+    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
+    assert count[0][0] == 1
+
+    new_job_script_file = make_dummy_file(main_file_path, content=new_file_content)
+
+    inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_EDIT)
+
+    with time_frame() as window:
+        response = await client.patch(
+            f"/jobbergate/job-scripts/{inserted_job_script_id}/upload",
+            files={"job_script_file": open(new_job_script_file, "rb")},
+        )
+
+    assert response.status_code == status.HTTP_204_NO_CONTENT
+
+    expected_job_script_files = JobScriptFiles(
+        main_file_path=main_file_path, files={main_file_path: new_file_content}
+    )
+    actual_job_script_files = JobScriptFiles.get_from_s3(inserted_job_script_id)
+
+    assert actual_job_script_files == expected_job_script_files
+
+    query = job_scripts_table.select(job_scripts_table.c.id == inserted_job_script_id)
+    job_script = JobScriptPartialResponse.parse_obj(await database.fetch_one(query))
+
+    assert job_script.updated_at in window
+
+
+@pytest.mark.asyncio
+@database.transaction(force_rollback=True)
+async def test_upload_job_script_file_by_id__job_script_not_found(
+    client,
+    inject_security_header,
+    make_dummy_file,
+):
+    """Test that a job script file can be uploaded when its id is not found at the database."""
+    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
+    assert count[0][0] == 0
+
+    main_file_path = pathlib.Path("jobbergate.py")
+    main_file_content = "I'm going to be replaced"
+
+    new_job_script_file = make_dummy_file(main_file_path, content=main_file_content)
+
+    inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_EDIT)
+
+    response = await client.patch(
+        "/jobbergate/job-scripts/1/upload",
+        files={"job_script_file": open(new_job_script_file, "rb")},
+    )
+
+    assert response.status_code == status.HTTP_404_NOT_FOUND
+    assert "JobScript with id=1 was not found." in response.text
+
+
+@pytest.mark.asyncio
+@database.transaction(force_rollback=True)
+async def test_upload_job_script_file_by_id__job_script_file_not_found(
+    client,
+    fill_job_script_data,
+    inject_security_header,
+    make_dummy_file,
+    mocked_file_manager_factory,
+):
+    """Test that a job script file can not be uploaded when its not found at s3."""
+    inserted_job_script_id = await database.execute(
+        query=job_scripts_table.insert(),
+        values=fill_job_script_data(),
+    )
+
+    main_file_path = pathlib.Path("jobbergate.py")
+
+    main_file_path = pathlib.Path("jobbergate.py")
+    new_file_content = "I'm going to be replaced"
+
+    new_job_script_file = make_dummy_file(main_file_path, content=new_file_content)
+
+    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
+    assert count[0][0] == 1
+
+    new_job_script_file = make_dummy_file(main_file_path, content=new_file_content)
+
+    inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_EDIT)
+
+    response = await client.patch(
+        f"/jobbergate/job-scripts/{inserted_job_script_id}/upload",
+        files={"job_script_file": open(new_job_script_file, "rb")},
+    )
+
+    assert response.status_code == status.HTTP_404_NOT_FOUND
+    assert f"Main file from job_script_id={inserted_job_script_id} was not found." in response.text
+
+
+@pytest.mark.asyncio
+@database.transaction(force_rollback=True)
 async def test_get_job_script_by_id_file_not_found_at_s3(
     client,
     fill_application_data,
     fill_job_script_data,
     inject_security_header,
     mocked_file_manager_factory,
 ):
@@ -473,15 +666,16 @@
     inject_security_header,
 ):
     """
     Test GET /job-scripts/ returns only job_scripts owned by the user making the request.
 
     This test proves that GET /job-scripts/ returns the correct job_scripts for the user making
     the request. We show this by asserting that the job_scripts returned in the response are
-    only job_scripts owned by the user making the request.
+    only job_scripts owned by the user making the request. This test also ensures that archived
+    job_scripts are not included by default.
     """
     inserted_application_id = await database.execute(
         query=applications_table.insert(),
         values=fill_application_data(application_owner_email="owner1@org.com"),
     )
     await database.execute_many(
         query=job_scripts_table.insert(),
@@ -497,19 +691,25 @@
                 application_id=inserted_application_id,
             ),
             dict(
                 job_script_name="js3",
                 job_script_owner_email="owner1@org.com",
                 application_id=inserted_application_id,
             ),
+            dict(
+                job_script_name="js4",
+                job_script_owner_email="owner1@org.com",
+                application_id=inserted_application_id,
+                is_archived=True,
+            ),
         ),
     )
 
     count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
-    assert count[0][0] == 3
+    assert count[0][0] == 4
 
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_VIEW)
     response = await client.get("/jobbergate/job-scripts/")
     assert response.status_code == status.HTTP_200_OK
 
     data = response.json()
     results = data.get("results")
@@ -614,14 +814,75 @@
         start=None,
         limit=None,
     )
 
 
 @pytest.mark.asyncio
 @database.transaction(force_rollback=True)
+async def test_get_job_scripts__with_include_archived_param(
+    client,
+    fill_application_data,
+    fill_all_job_script_data,
+    inject_security_header,
+):
+    """
+    Test that listing job_scripts, when include_archived=True, contains archived job_scripts.
+
+    This test proves that the user making the request can see archived job_scripts.
+    We show this by creating three job_scripts, one that is archived, and two that are not.
+    Assert that the response to GET /job-scripts/?include_archived=True includes all three job_scripts.
+    """
+    inserted_application_id = await database.execute(
+        query=applications_table.insert(),
+        values=fill_application_data(application_owner_email="owner1@org.com"),
+    )
+    await database.execute_many(
+        query=job_scripts_table.insert(),
+        values=fill_all_job_script_data(
+            {
+                "job_script_name": "script1",
+                "job_script_owner_email": "owner1@org.com",
+                "application_id": inserted_application_id,
+            },
+            {
+                "job_script_name": "script2",
+                "job_script_owner_email": "owner1@org.com",
+                "application_id": inserted_application_id,
+                "is_archived": True,
+            },
+            {
+                "job_script_name": "script3",
+                "job_script_owner_email": "owner1@org.com",
+                "application_id": inserted_application_id,
+            },
+        ),
+    )
+
+    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
+    assert count[0][0] == 3
+
+    inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_VIEW)
+    response = await client.get("/jobbergate/job-scripts/?include_archived=True")
+    assert response.status_code == status.HTTP_200_OK
+
+    data = response.json()
+    results = data.get("results")
+    assert results
+    assert [d["job_script_name"] for d in results] == ["script1", "script2", "script3"]
+
+    pagination = data.get("pagination")
+    assert pagination == dict(
+        total=3,
+        start=None,
+        limit=None,
+    )
+
+
+@pytest.mark.asyncio
+@database.transaction(force_rollback=True)
 async def test_get_job_scripts__with_search_param(client, inject_security_header, fill_application_data):
     """
     Test that listing job scripts, when search=<search terms>, returns matches.
 
     This test proves that the user making the request will be shown job scripts that match the search string.
     We show this by creating job scripts and using various search queries to match against them.
 
@@ -917,33 +1178,36 @@
             json={
                 "job_script_name": "new name",
                 "job_script_description": "new description",
                 "job_script_files": {
                     "main_file_path": main_file_path,
                     "files": {main_file_path: main_file_content},
                 },
+                "is_archived": True,
             },
         )
 
     assert response.status_code == status.HTTP_200_OK
     data = response.json()
 
     assert data["job_script_name"] == "new name"
     assert data["job_script_description"] == "new description"
     assert JobScriptFiles(**data["job_script_files"]) == dummy_job_script_files
     assert JobScriptFiles.get_from_s3(inserted_job_script_id) == dummy_job_script_files
     assert data["id"] == inserted_job_script_id
+    assert data["is_archived"] is True
 
     query = job_scripts_table.select(job_scripts_table.c.id == inserted_job_script_id)
     job_script = JobScriptPartialResponse.parse_obj(await database.fetch_one(query))
 
     assert job_script is not None
     assert job_script.job_script_name == "new name"
     assert job_script.job_script_description == "new description"
     assert job_script.updated_at in window
+    assert job_script.is_archived
 
 
 @pytest.mark.asyncio
 @database.transaction(force_rollback=True)
 async def test_update_job_script_not_found(
     client,
     inject_security_header,
@@ -1135,45 +1399,56 @@
 
     count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
     assert count[0][0] == 1
 
 
 @pytest.mark.asyncio
 @database.transaction(force_rollback=True)
-async def test_delete_job_script__fk_error(
+async def test_delete_job_script__unlinks_job_submissions(
     client,
     fill_application_data,
     fill_job_script_data,
+    fill_job_submission_data,
     inject_security_header,
 ):
     """
-    Test DELETE /job_script/<id> correctly returns a 409 on a foreign-key constraint error.
+    Test DELETE /job_scripts/<id> correctly deletes a job_script linked to a job_submission.
+
+    Test that a the job_script_id field for connected job_submissions is set to null.
     """
     inserted_application_id = await database.execute(
         query=applications_table.insert(),
         values=fill_application_data(),
     )
     inserted_job_script_id = await database.execute(
         query=job_scripts_table.insert(),
         values=fill_job_script_data(application_id=inserted_application_id),
     )
 
     count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
     assert count[0][0] == 1
 
+    await database.execute(
+        query=job_submissions_table.insert(),
+        values=fill_job_submission_data(job_script_id=inserted_job_script_id),
+    )
+    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
+    assert count[0][0] == 1
+    count = await database.fetch_all(
+        "SELECT COUNT(*) FROM job_submissions where job_script_id=:inserted_id",
+        values=dict(inserted_id=inserted_job_script_id),
+    )
+    assert count[0][0] == 1
+
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_EDIT)
-    with mock.patch(
-        "jobbergate_api.storage.database.execute",
-        side_effect=asyncpg.exceptions.ForeignKeyViolationError(
-            f"""
-            update or delete on table "job_scripts" violates foreign key constraint
-            "job_submissions_job_script_id_fkey" on table "job_submissions"
-            DETAIL:  Key (id)=({inserted_job_script_id}) is still referenced from table "job_submissions".
-            """
-        ),
-    ):
+    with mock.patch("jobbergate_api.apps.job_scripts.job_script_files.JobScriptFiles.delete_from_s3"):
         response = await client.delete(f"/jobbergate/job-scripts/{inserted_job_script_id}")
-    assert response.status_code == status.HTTP_409_CONFLICT
-    error_data = json.loads(response.text)["detail"]
-    assert error_data["message"] == "Delete failed due to foreign-key constraint"
-    assert error_data["table"] == "job_submissions"
-    assert error_data["pk_id"] == f"{inserted_job_script_id}"
+        assert response.status_code == status.HTTP_204_NO_CONTENT
+
+    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
+    assert count[0][0] == 0
+
+    count = await database.fetch_all(
+        "SELECT COUNT(*) FROM job_submissions where job_script_id=:inserted_id",
+        values=dict(inserted_id=inserted_job_script_id),
+    )
+    assert count[0][0] == 0
```

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/apps/job_submissions/test_routers.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_submissions/test_routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/conftest.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/test_config.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/test_email_notification.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/test_email_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/test_meta_mapper.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/test_meta_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/test_pagination.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/test_s3_manager.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/test_s3_manager.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/test_security.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/test_storage.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/tests/test_version.py` & `jobbergate_api-3.5.0a3/jobbergate_api/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/jobbergate_api/version.py` & `jobbergate_api-3.5.0a3/jobbergate_api/version.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a2/pyproject.toml` & `jobbergate_api-3.5.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-api"
-version = "3.5.0-alpha.2"
+version = "3.5.0-alpha.3"
 description = "Jobbergate API"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `jobbergate-api-3.5.0a2/PKG-INFO` & `jobbergate_api-3.5.0a3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: jobbergate-api
-Version: 3.5.0a2
+Version: 3.5.0a3
 Summary: Jobbergate API
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: FastAPI
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: Jinja2 (>=3.0.3,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: alembic (>=1.7.5,<2.0.0)
 Requires-Dist: armasec (>=0.11.0,<0.12.0)
 Requires-Dist: asyncpg (>=0.22.0,<0.23.0)
 Requires-Dist: bidict (>=0.22.0,<0.23.0)
```

