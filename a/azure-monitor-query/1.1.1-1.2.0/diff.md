# Comparing `tmp/azure-monitor-query-1.1.1.zip` & `tmp/azure-monitor-query-1.2.0.zip`

## zipinfo {}

```diff
@@ -1,110 +1,116 @@
-Zip file size: 173771 bytes, number of entries: 108
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-14 01:27 azure-monitor-query-1.1.1/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-14 01:27 azure-monitor-query-1.1.1/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-14 01:27 azure-monitor-query-1.1.1/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-14 01:27 azure-monitor-query-1.1.1/azure_monitor_query.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-14 01:27 azure-monitor-query-1.1.1/tests/
--rw-rw-r--  2.0 unx    29453 b- defN 23-Feb-14 01:27 azure-monitor-query-1.1.1/PKG-INFO
--rw-rw-r--  2.0 unx     5564 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/migration_guide.md
--rw-rw-r--  2.0 unx    11307 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/TROUBLESHOOTING.md
--rw-rw-r--  2.0 unx     7635 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/migration_guide_app_insights.md
--rw-rw-r--  2.0 unx     3062 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/setup.py
--rw-rw-r--  2.0 unx      193 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/MANIFEST.in
--rw-rw-r--  2.0 unx    22405 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/README.md
--rw-rw-r--  2.0 unx     1073 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/LICENSE
--rw-rw-r--  2.0 unx     6226 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/CHANGELOG.md
--rw-rw-r--  2.0 unx       38 b- defN 23-Feb-14 01:27 azure-monitor-query-1.1.1/setup.cfg
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-14 01:27 azure-monitor-query-1.1.1/samples/async_samples/
--rw-rw-r--  2.0 unx     1768 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/samples/sample_single_log_query_without_pandas.py
--rw-rw-r--  2.0 unx     2506 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/samples/sample_batch_query.py
--rw-rw-r--  2.0 unx     1841 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/samples/sample_server_timeout.py
--rw-rw-r--  2.0 unx     1169 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/samples/sample_metric_namespaces.py
--rw-rw-r--  2.0 unx     2074 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/samples/sample_metrics_query.py
--rw-rw-r--  2.0 unx     1750 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/samples/sample_log_query_multiple_workspaces.py
--rw-rw-r--  2.0 unx     2262 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/samples/sample_logs_single_query.py
--rw-rw-r--  2.0 unx     2463 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/samples/sample_logs_single_query_partial_result.py
--rw-rw-r--  2.0 unx     1892 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/samples/sample_logs_query_key_value_form.py
--rw-rw-r--  2.0 unx     1271 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/samples/sample_metric_definitions.py
--rw-rw-r--  2.0 unx     1505 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/samples/async_samples/sample_metric_namespaces_async.py
--rw-rw-r--  2.0 unx     1917 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/samples/async_samples/sample_metrics_query_async.py
--rw-rw-r--  2.0 unx     1976 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/samples/async_samples/sample_log_query_async.py
--rw-rw-r--  2.0 unx     1580 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/samples/async_samples/sample_metric_definitions_async.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-14 01:27 azure-monitor-query-1.1.1/azure/monitor/
--rw-rw-r--  2.0 unx       65 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-14 01:27 azure-monitor-query-1.1.1/azure/monitor/query/
--rw-rw-r--  2.0 unx       65 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-14 01:27 azure-monitor-query-1.1.1/azure/monitor/query/_generated/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-14 01:27 azure-monitor-query-1.1.1/azure/monitor/query/aio/
--rw-rw-r--  2.0 unx    23559 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_models.py
--rw-rw-r--  2.0 unx     9934 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_metrics_query_client.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/py.typed
--rw-rw-r--  2.0 unx     5561 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_helpers.py
--rw-rw-r--  2.0 unx     1740 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_enums.py
--rw-rw-r--  2.0 unx      345 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_version.py
--rw-rw-r--  2.0 unx     9319 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_logs_query_client.py
--rw-rw-r--  2.0 unx     1415 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/__init__.py
--rw-rw-r--  2.0 unx     1775 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_exceptions.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-14 01:27 azure-monitor-query-1.1.1/azure/monitor/query/_generated/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-14 01:27 azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-14 01:27 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/
--rw-rw-r--  2.0 unx     3282 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/_client.py
--rw-rw-r--  2.0 unx    78699 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/_serialization.py
--rw-rw-r--  2.0 unx      976 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/_vendor.py
--rw-rw-r--  2.0 unx     2015 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/_configuration.py
--rw-rw-r--  2.0 unx      827 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/_patch.py
--rw-rw-r--  2.0 unx    84386 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/operations/_operations.py
--rw-rw-r--  2.0 unx      841 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/operations/_patch.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-14 01:27 azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/operations/
--rw-rw-r--  2.0 unx     3389 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/_client.py
--rw-rw-r--  2.0 unx     2025 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/_configuration.py
--rw-rw-r--  2.0 unx      827 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/_patch.py
--rw-rw-r--  2.0 unx    80695 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/operations/_operations.py
--rw-rw-r--  2.0 unx      841 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/operations/_patch.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-14 01:27 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-14 01:27 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/
--rw-rw-r--  2.0 unx     3728 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/_client.py
--rw-rw-r--  2.0 unx    78699 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/_serialization.py
--rw-rw-r--  2.0 unx      976 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/_vendor.py
--rw-rw-r--  2.0 unx     2023 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/_configuration.py
--rw-rw-r--  2.0 unx      831 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/_patch.py
--rw-rw-r--  2.0 unx    28014 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/operations/_operations.py
--rw-rw-r--  2.0 unx      949 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/operations/_patch.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-14 01:27 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/operations/
--rw-rw-r--  2.0 unx     3839 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/_client.py
--rw-rw-r--  2.0 unx     2033 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/_configuration.py
--rw-rw-r--  2.0 unx      831 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/_patch.py
--rw-rw-r--  2.0 unx    23558 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/operations/_operations.py
--rw-rw-r--  2.0 unx      949 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/operations/_patch.py
--rw-rw-r--  2.0 unx     1662 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/aio/_helpers_async.py
--rw-rw-r--  2.0 unx     8431 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/aio/_logs_query_client_async.py
--rw-rw-r--  2.0 unx      492 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/aio/__init__.py
--rw-rw-r--  2.0 unx     9300 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/azure/monitor/query/aio/_metrics_query_client_async.py
--rw-rw-r--  2.0 unx    29453 b- defN 23-Feb-14 01:27 azure-monitor-query-1.1.1/azure_monitor_query.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx     3646 b- defN 23-Feb-14 01:27 azure-monitor-query-1.1.1/azure_monitor_query.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Feb-14 01:27 azure-monitor-query-1.1.1/azure_monitor_query.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Feb-14 01:27 azure-monitor-query-1.1.1/azure_monitor_query.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx       66 b- defN 23-Feb-14 01:27 azure-monitor-query-1.1.1/azure_monitor_query.egg-info/requires.txt
--rw-rw-r--  2.0 unx        6 b- defN 23-Feb-14 01:27 azure-monitor-query-1.1.1/azure_monitor_query.egg-info/top_level.txt
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-14 01:27 azure-monitor-query-1.1.1/tests/perfstress_tests/
--rw-rw-r--  2.0 unx     3835 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/tests/test_logs_timespans.py
--rw-rw-r--  2.0 unx    11086 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/tests/test_logs_client.py
--rw-rw-r--  2.0 unx     4936 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/tests/test_exceptions_async.py
--rw-rw-r--  2.0 unx     4588 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/tests/test_metrics_client.py
--rw-rw-r--  2.0 unx     2138 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/tests/conftest.py
--rw-rw-r--  2.0 unx     5657 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/tests/test_exceptions.py
--rw-rw-r--  2.0 unx     3142 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/tests/test_logs_response.py
--rw-rw-r--  2.0 unx     5648 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/tests/test_metrics_client_async.py
--rw-rw-r--  2.0 unx     9784 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/tests/test_logs_client_async.py
--rw-rw-r--  2.0 unx     2803 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/tests/perfstress_tests/single_query.py
--rw-rw-r--  2.0 unx     3270 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/tests/perfstress_tests/batch_query.py
--rw-rw-r--  2.0 unx     2552 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/tests/perfstress_tests/metric_query.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Feb-14 01:26 azure-monitor-query-1.1.1/tests/perfstress_tests/__init__.py
-108 files, 689830 bytes uncompressed, 151789 bytes compressed:  78.0%
+Zip file size: 185223 bytes, number of entries: 114
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 18:39 azure-monitor-query-1.2.0/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 18:39 azure-monitor-query-1.2.0/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 18:39 azure-monitor-query-1.2.0/azure_monitor_query.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 18:39 azure-monitor-query-1.2.0/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 18:39 azure-monitor-query-1.2.0/tests/
+-rw-rw-r--  2.0 unx    24213 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/README.md
+-rw-rw-r--  2.0 unx     3062 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/setup.py
+-rw-rw-r--  2.0 unx     5564 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/migration_guide.md
+-rw-rw-r--  2.0 unx       38 b- defN 23-May-09 18:39 azure-monitor-query-1.2.0/setup.cfg
+-rw-rw-r--  2.0 unx     7635 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/migration_guide_app_insights.md
+-rw-rw-r--  2.0 unx    11307 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/TROUBLESHOOTING.md
+-rw-rw-r--  2.0 unx    32045 b- defN 23-May-09 18:39 azure-monitor-query-1.2.0/PKG-INFO
+-rw-rw-r--  2.0 unx       50 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/pyproject.toml
+-rw-rw-r--  2.0 unx      193 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/MANIFEST.in
+-rw-rw-r--  2.0 unx     1073 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/LICENSE
+-rw-rw-r--  2.0 unx     7010 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/CHANGELOG.md
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 18:39 azure-monitor-query-1.2.0/samples/async_samples/
+-rw-rw-r--  2.0 unx     1841 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/samples/sample_server_timeout.py
+-rw-rw-r--  2.0 unx     2262 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/samples/sample_logs_single_query.py
+-rw-rw-r--  2.0 unx     1768 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/samples/sample_single_log_query_without_pandas.py
+-rw-rw-r--  2.0 unx     3477 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/samples/sample_logs_query_visualization.py
+-rw-rw-r--  2.0 unx     1892 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/samples/sample_logs_query_key_value_form.py
+-rw-rw-r--  2.0 unx     2074 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/samples/sample_metrics_query.py
+-rw-rw-r--  2.0 unx     2036 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/samples/sample_resource_logs_query.py
+-rw-rw-r--  2.0 unx     1271 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/samples/sample_metric_definitions.py
+-rw-rw-r--  2.0 unx     1750 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/samples/sample_log_query_multiple_workspaces.py
+-rw-rw-r--  2.0 unx     1169 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/samples/sample_metric_namespaces.py
+-rw-rw-r--  2.0 unx     2463 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/samples/sample_logs_single_query_partial_result.py
+-rw-rw-r--  2.0 unx     2506 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/samples/sample_batch_query.py
+-rw-rw-r--  2.0 unx     1505 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/samples/async_samples/sample_metric_namespaces_async.py
+-rw-rw-r--  2.0 unx     1917 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/samples/async_samples/sample_metrics_query_async.py
+-rw-rw-r--  2.0 unx     1976 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/samples/async_samples/sample_log_query_async.py
+-rw-rw-r--  2.0 unx     2387 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/samples/async_samples/sample_resource_logs_query_async.py
+-rw-rw-r--  2.0 unx     4017 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/samples/async_samples/sample_logs_query_visualization_async.py
+-rw-rw-r--  2.0 unx     1580 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/samples/async_samples/sample_metric_definitions_async.py
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-09 18:39 azure-monitor-query-1.2.0/azure_monitor_query.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx        6 b- defN 23-May-09 18:39 azure-monitor-query-1.2.0/azure_monitor_query.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx     3886 b- defN 23-May-09 18:39 azure-monitor-query-1.2.0/azure_monitor_query.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx    32045 b- defN 23-May-09 18:39 azure-monitor-query-1.2.0/azure_monitor_query.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-09 18:39 azure-monitor-query-1.2.0/azure_monitor_query.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx       66 b- defN 23-May-09 18:39 azure-monitor-query-1.2.0/azure_monitor_query.egg-info/requires.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 18:39 azure-monitor-query-1.2.0/azure/monitor/
+-rw-rw-r--  2.0 unx       65 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 18:39 azure-monitor-query-1.2.0/azure/monitor/query/
+-rw-rw-r--  2.0 unx       65 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 18:39 azure-monitor-query-1.2.0/azure/monitor/query/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 18:39 azure-monitor-query-1.2.0/azure/monitor/query/_generated/
+-rw-rw-r--  2.0 unx     1415 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/__init__.py
+-rw-rw-r--  2.0 unx     1775 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_exceptions.py
+-rw-rw-r--  2.0 unx    13192 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_logs_query_client.py
+-rw-rw-r--  2.0 unx     1740 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_enums.py
+-rw-rw-r--  2.0 unx     4675 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_helpers.py
+-rw-rw-r--  2.0 unx     9766 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_metrics_query_client.py
+-rw-rw-r--  2.0 unx      345 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_version.py
+-rw-rw-r--  2.0 unx    23463 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_models.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/py.typed
+-rw-rw-r--  2.0 unx      492 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/aio/__init__.py
+-rw-rw-r--  2.0 unx      917 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/aio/_helpers_async.py
+-rw-rw-r--  2.0 unx     9090 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/aio/_metrics_query_client_async.py
+-rw-rw-r--  2.0 unx    12528 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/aio/_logs_query_client_async.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 18:39 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 18:39 azure-monitor-query-1.2.0/azure/monitor/query/_generated/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 18:39 azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/
+-rw-rw-r--  2.0 unx      827 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/__init__.py
+-rw-rw-r--  2.0 unx     2010 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/_configuration.py
+-rw-rw-r--  2.0 unx     3303 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/_patch.py
+-rw-rw-r--  2.0 unx      976 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/_vendor.py
+-rw-rw-r--  2.0 unx    78836 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/_serialization.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 18:39 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 18:39 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/
+-rw-rw-r--  2.0 unx      831 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/__init__.py
+-rw-rw-r--  2.0 unx     2016 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/_configuration.py
+-rw-rw-r--  2.0 unx     3749 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/_patch.py
+-rw-rw-r--  2.0 unx      976 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/_vendor.py
+-rw-rw-r--  2.0 unx    78836 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/_serialization.py
+-rw-rw-r--  2.0 unx      949 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/operations/__init__.py
+-rw-rw-r--  2.0 unx    27721 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/operations/_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/operations/_patch.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 18:39 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/operations/
+-rw-rw-r--  2.0 unx      831 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/__init__.py
+-rw-rw-r--  2.0 unx     2026 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/_configuration.py
+-rw-rw-r--  2.0 unx     3865 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/_patch.py
+-rw-rw-r--  2.0 unx      949 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    23341 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      841 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/operations/__init__.py
+-rw-rw-r--  2.0 unx   130598 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/operations/_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/operations/_patch.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 18:39 azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/operations/
+-rw-rw-r--  2.0 unx      827 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/__init__.py
+-rw-rw-r--  2.0 unx     2020 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/_configuration.py
+-rw-rw-r--  2.0 unx     3415 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/_patch.py
+-rw-rw-r--  2.0 unx      841 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx   123123 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/operations/_patch.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 18:39 azure-monitor-query-1.2.0/tests/perfstress_tests/
+-rw-rw-r--  2.0 unx     2138 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/tests/conftest.py
+-rw-rw-r--  2.0 unx     3116 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/tests/test_logs_response.py
+-rw-rw-r--  2.0 unx    11265 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/tests/test_logs_client_async.py
+-rw-rw-r--  2.0 unx     6094 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/tests/test_exceptions_async.py
+-rw-rw-r--  2.0 unx    12201 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/tests/test_logs_client.py
+-rw-rw-r--  2.0 unx     6176 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/tests/test_metrics_client_async.py
+-rw-rw-r--  2.0 unx     1428 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/tests/base_testcase.py
+-rw-rw-r--  2.0 unx     3771 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/tests/test_logs_timespans.py
+-rw-rw-r--  2.0 unx     5068 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/tests/test_metrics_client.py
+-rw-rw-r--  2.0 unx     6679 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/tests/test_exceptions.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/tests/perfstress_tests/__init__.py
+-rw-rw-r--  2.0 unx     2803 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/tests/perfstress_tests/single_query.py
+-rw-rw-r--  2.0 unx     3270 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/tests/perfstress_tests/batch_query.py
+-rw-rw-r--  2.0 unx     2552 b- defN 23-May-09 18:38 azure-monitor-query-1.2.0/tests/perfstress_tests/metric_query.py
+114 files, 811274 bytes uncompressed, 162005 bytes compressed:  80.0%
```

## zipnote {}

```diff
@@ -1,325 +1,343 @@
-Filename: azure-monitor-query-1.1.1/
+Filename: azure-monitor-query-1.2.0/
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/samples/
+Filename: azure-monitor-query-1.2.0/samples/
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/
+Filename: azure-monitor-query-1.2.0/azure_monitor_query.egg-info/
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure_monitor_query.egg-info/
+Filename: azure-monitor-query-1.2.0/azure/
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/tests/
+Filename: azure-monitor-query-1.2.0/tests/
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/PKG-INFO
+Filename: azure-monitor-query-1.2.0/README.md
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/migration_guide.md
+Filename: azure-monitor-query-1.2.0/setup.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/TROUBLESHOOTING.md
+Filename: azure-monitor-query-1.2.0/migration_guide.md
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/migration_guide_app_insights.md
+Filename: azure-monitor-query-1.2.0/setup.cfg
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/setup.py
+Filename: azure-monitor-query-1.2.0/migration_guide_app_insights.md
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/MANIFEST.in
+Filename: azure-monitor-query-1.2.0/TROUBLESHOOTING.md
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/README.md
+Filename: azure-monitor-query-1.2.0/PKG-INFO
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/LICENSE
+Filename: azure-monitor-query-1.2.0/pyproject.toml
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/CHANGELOG.md
+Filename: azure-monitor-query-1.2.0/MANIFEST.in
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/setup.cfg
+Filename: azure-monitor-query-1.2.0/LICENSE
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/samples/async_samples/
+Filename: azure-monitor-query-1.2.0/CHANGELOG.md
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/samples/sample_single_log_query_without_pandas.py
+Filename: azure-monitor-query-1.2.0/samples/async_samples/
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/samples/sample_batch_query.py
+Filename: azure-monitor-query-1.2.0/samples/sample_server_timeout.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/samples/sample_server_timeout.py
+Filename: azure-monitor-query-1.2.0/samples/sample_logs_single_query.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/samples/sample_metric_namespaces.py
+Filename: azure-monitor-query-1.2.0/samples/sample_single_log_query_without_pandas.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/samples/sample_metrics_query.py
+Filename: azure-monitor-query-1.2.0/samples/sample_logs_query_visualization.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/samples/sample_log_query_multiple_workspaces.py
+Filename: azure-monitor-query-1.2.0/samples/sample_logs_query_key_value_form.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/samples/sample_logs_single_query.py
+Filename: azure-monitor-query-1.2.0/samples/sample_metrics_query.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/samples/sample_logs_single_query_partial_result.py
+Filename: azure-monitor-query-1.2.0/samples/sample_resource_logs_query.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/samples/sample_logs_query_key_value_form.py
+Filename: azure-monitor-query-1.2.0/samples/sample_metric_definitions.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/samples/sample_metric_definitions.py
+Filename: azure-monitor-query-1.2.0/samples/sample_log_query_multiple_workspaces.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/samples/async_samples/sample_metric_namespaces_async.py
+Filename: azure-monitor-query-1.2.0/samples/sample_metric_namespaces.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/samples/async_samples/sample_metrics_query_async.py
+Filename: azure-monitor-query-1.2.0/samples/sample_logs_single_query_partial_result.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/samples/async_samples/sample_log_query_async.py
+Filename: azure-monitor-query-1.2.0/samples/sample_batch_query.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/samples/async_samples/sample_metric_definitions_async.py
+Filename: azure-monitor-query-1.2.0/samples/async_samples/sample_metric_namespaces_async.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/
+Filename: azure-monitor-query-1.2.0/samples/async_samples/sample_metrics_query_async.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/__init__.py
+Filename: azure-monitor-query-1.2.0/samples/async_samples/sample_log_query_async.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/
+Filename: azure-monitor-query-1.2.0/samples/async_samples/sample_resource_logs_query_async.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/__init__.py
+Filename: azure-monitor-query-1.2.0/samples/async_samples/sample_logs_query_visualization_async.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/
+Filename: azure-monitor-query-1.2.0/samples/async_samples/sample_metric_definitions_async.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/aio/
+Filename: azure-monitor-query-1.2.0/azure_monitor_query.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_models.py
+Filename: azure-monitor-query-1.2.0/azure_monitor_query.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_metrics_query_client.py
+Filename: azure-monitor-query-1.2.0/azure_monitor_query.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/py.typed
+Filename: azure-monitor-query-1.2.0/azure_monitor_query.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_helpers.py
+Filename: azure-monitor-query-1.2.0/azure_monitor_query.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_enums.py
+Filename: azure-monitor-query-1.2.0/azure_monitor_query.egg-info/requires.txt
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_version.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_logs_query_client.py
+Filename: azure-monitor-query-1.2.0/azure/__init__.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/__init__.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_exceptions.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/__init__.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/operations/
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/aio/
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/__init__.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/_client.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_exceptions.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/_serialization.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_logs_query_client.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/_vendor.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_enums.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/_configuration.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_helpers.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/__init__.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_metrics_query_client.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/_patch.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_version.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/operations/_operations.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_models.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/operations/__init__.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/py.typed
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/operations/_patch.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/aio/__init__.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/operations/
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/aio/_helpers_async.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/_client.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/aio/_metrics_query_client_async.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/_configuration.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/aio/_logs_query_client_async.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/__init__.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/_patch.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/operations/
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/operations/_operations.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/operations/__init__.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/__init__.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/operations/_patch.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/_configuration.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/operations/
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/_client.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/_patch.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/_client.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/_vendor.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/_serialization.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/_serialization.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/_vendor.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/operations/
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/_configuration.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/__init__.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/__init__.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/_patch.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/_configuration.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/operations/_operations.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/_client.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/operations/__init__.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/_patch.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/operations/_patch.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/_vendor.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/operations/
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/_serialization.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/_client.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/operations/__init__.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/_configuration.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/operations/_operations.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/__init__.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/operations/_patch.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/_patch.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/operations/
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/operations/_operations.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/__init__.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/operations/__init__.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/_configuration.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/operations/_patch.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/_client.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/aio/_helpers_async.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/_patch.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/aio/_logs_query_client_async.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/aio/__init__.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure/monitor/query/aio/_metrics_query_client_async.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure_monitor_query.egg-info/PKG-INFO
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/operations/__init__.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure_monitor_query.egg-info/SOURCES.txt
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/operations/_operations.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure_monitor_query.egg-info/dependency_links.txt
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/operations/_patch.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure_monitor_query.egg-info/not-zip-safe
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/operations/
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure_monitor_query.egg-info/requires.txt
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/__init__.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/azure_monitor_query.egg-info/top_level.txt
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/_configuration.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/tests/perfstress_tests/
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/_client.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/tests/test_logs_timespans.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/_patch.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/tests/test_logs_client.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/tests/test_exceptions_async.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/tests/test_metrics_client.py
+Filename: azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/tests/conftest.py
+Filename: azure-monitor-query-1.2.0/tests/perfstress_tests/
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/tests/test_exceptions.py
+Filename: azure-monitor-query-1.2.0/tests/conftest.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/tests/test_logs_response.py
+Filename: azure-monitor-query-1.2.0/tests/test_logs_response.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/tests/test_metrics_client_async.py
+Filename: azure-monitor-query-1.2.0/tests/test_logs_client_async.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/tests/test_logs_client_async.py
+Filename: azure-monitor-query-1.2.0/tests/test_exceptions_async.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/tests/perfstress_tests/single_query.py
+Filename: azure-monitor-query-1.2.0/tests/test_logs_client.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/tests/perfstress_tests/batch_query.py
+Filename: azure-monitor-query-1.2.0/tests/test_metrics_client_async.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/tests/perfstress_tests/metric_query.py
+Filename: azure-monitor-query-1.2.0/tests/base_testcase.py
 Comment: 
 
-Filename: azure-monitor-query-1.1.1/tests/perfstress_tests/__init__.py
+Filename: azure-monitor-query-1.2.0/tests/test_logs_timespans.py
+Comment: 
+
+Filename: azure-monitor-query-1.2.0/tests/test_metrics_client.py
+Comment: 
+
+Filename: azure-monitor-query-1.2.0/tests/test_exceptions.py
+Comment: 
+
+Filename: azure-monitor-query-1.2.0/tests/perfstress_tests/__init__.py
+Comment: 
+
+Filename: azure-monitor-query-1.2.0/tests/perfstress_tests/single_query.py
+Comment: 
+
+Filename: azure-monitor-query-1.2.0/tests/perfstress_tests/batch_query.py
+Comment: 
+
+Filename: azure-monitor-query-1.2.0/tests/perfstress_tests/metric_query.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-monitor-query-1.1.1/PKG-INFO` & `azure-monitor-query-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-monitor-query
-Version: 1.1.1
+Version: 1.2.0
 Summary: Microsoft Azure Monitor Query Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -26,14 +26,15 @@
 - [Logs](https://learn.microsoft.com/azure/azure-monitor/logs/data-platform-logs) - Collects and organizes log and performance data from monitored resources. Data from different sources such as platform logs from Azure services, log and performance data from virtual machines agents, and usage and performance data from apps can be consolidated into a single [Azure Log Analytics workspace](https://learn.microsoft.com/azure/azure-monitor/logs/data-platform-logs#log-analytics-and-workspaces). The various data types can be analyzed together using the [Kusto Query Language][kusto_query_language].
 - [Metrics](https://learn.microsoft.com/azure/azure-monitor/essentials/data-platform-metrics) - Collects numeric data from monitored resources into a time series database. Metrics are numerical values that are collected at regular intervals and describe some aspect of a system at a particular time. Metrics are lightweight and capable of supporting near real-time scenarios, making them useful for alerting and fast detection of issues.
 
 **Resources:**
 
 - [Source code][source]
 - [Package (PyPI)][package]
+- [Package (Conda)](https://anaconda.org/microsoft/azure-monitor-query/)
 - [API reference documentation][python-query-ref-docs]
 - [Service documentation][azure_monitor_overview]
 - [Samples][samples]
 - [Change log][changelog]
 
 ## Getting started
 
@@ -79,14 +80,25 @@
 from azure.monitor.query.aio import LogsQueryClient, MetricsQueryClient
 
 credential = DefaultAzureCredential()
 async_logs_client = LogsQueryClient(credential)
 async_metrics_client = MetricsQueryClient(credential)
 ```
 
+#### Configure clients for non-public Azure clouds
+
+By default, `LogsQueryClient` and `MetricsQueryClient` are configured to connect to the public Azure cloud. These can be configured to connect to non-public Azure clouds by passing in the correct `endpoint` argument: For example:
+
+```python
+logs_client = LogsQueryClient(credential, endpoint="https://api.loganalytics.azure.cn/v1")
+metrics_client = MetricsQueryClient(credential, endpoint="https://management.chinacloudapi.cn")
+```
+
+**Note**: Currently, `MetricsQueryClient` uses the Azure Resource Manager (ARM) endpoint for querying metrics, so you will need the corresponding management endpoint for your cloud when using this client. This is subject to change in the future.
+
 ### Execute the query
 
 For examples of Logs and Metrics queries, see the [Examples](#examples) section.
 
 ## Key concepts
 
 ### Logs query rate limits and throttling
@@ -108,26 +120,27 @@
 
 ## Examples
 
 - [Logs query](#logs-query)
   - [Specify timespan](#specify-timespan)
   - [Handle logs query response](#handle-logs-query-response)
 - [Batch logs query](#batch-logs-query)
+- [Resource logs query](#resource-logs-query)
 - [Advanced logs query scenarios](#advanced-logs-query-scenarios)
   - [Set logs query timeout](#set-logs-query-timeout)
   - [Query multiple workspaces](#query-multiple-workspaces)
   - [Include statistics](#include-statistics)
   - [Include visualization](#include-visualization)
 - [Metrics query](#metrics-query)
   - [Handle metrics query response](#handle-metrics-query-response)
   - [Example of handling response](#example-of-handling-response)
 
 ### Logs query
 
-This example shows getting a logs query. To handle the response and view it in a tabular form, the [pandas](https://pypi.org/project/pandas/) library is used. See the [samples][samples] if you choose not to use pandas.
+This example shows how to query a Log Analytics workspace. To handle the response and view it in a tabular form, the [pandas](https://pypi.org/project/pandas/) library is used. See the [samples][samples] if you choose not to use pandas.
 
 #### Specify timespan
 
 The `timespan` parameter specifies the time duration for which to query the data. This value can be one of the following:
 
 - a `timedelta`
 - a `timedelta` and a start datetime
@@ -164,44 +177,44 @@
     elif response.status == LogsQueryStatus.SUCCESS:
         data = response.tables
     for table in data:
         df = pd.DataFrame(data=table.rows, columns=table.columns)
         print(df)
 except HttpResponseError as err:
     print("something fatal happened")
-    print (err)
+    print(err)
 ```
 
 #### Handle logs query response
 
 The `query_workspace` API returns either a `LogsQueryResult` or a `LogsQueryPartialResult` object. The `batch_query` API returns a list that may contain `LogsQueryResult`, `LogsQueryPartialResult`, and `LogsQueryError` objects. Here's a hierarchy of the response:
 
 ```
 LogsQueryResult
 |---statistics
 |---visualization
 |---tables (list of `LogsTable` objects)
     |---name
     |---rows
     |---columns
-    |---column_types
+    |---columns_types
 
 LogsQueryPartialResult
 |---statistics
 |---visualization
 |---partial_error (a `LogsQueryError` object)
     |---code
     |---message
     |---details
     |---status
 |---partial_data (list of `LogsTable` objects)
     |---name
     |---rows
     |---columns
-    |---column_types
+    |---columns_types
 ```
 
 The `LogsQueryResult` directly iterates over the table as a convenience. For example, to handle a logs query response with tables and display it using pandas:
 
 ```python
 response = client.query(...)
 for table in response:
@@ -235,26 +248,26 @@
 
 credential = DefaultAzureCredential()
 client = LogsQueryClient(credential)
 requests = [
     LogsBatchQuery(
         query="AzureActivity | summarize count()",
         timespan=timedelta(hours=1),
-        workspace_id= os.environ['LOG_WORKSPACE_ID']
+        workspace_id=os.environ['LOG_WORKSPACE_ID']
     ),
     LogsBatchQuery(
         query= """bad query""",
         timespan=timedelta(days=1),
-        workspace_id= os.environ['LOG_WORKSPACE_ID']
+        workspace_id=os.environ['LOG_WORKSPACE_ID']
     ),
     LogsBatchQuery(
         query= """let Weight = 92233720368547758;
         range x from 1 to 3 step 1
         | summarize percentilesw(x, Weight * 100, 50)""",
-        workspace_id= os.environ['LOG_WORKSPACE_ID'],
+        workspace_id=os.environ['LOG_WORKSPACE_ID'],
         timespan=(datetime(2021, 6, 2, tzinfo=timezone.utc), datetime(2021, 6, 5, tzinfo=timezone.utc)), # (start, end)
         include_statistics=True
     ),
 ]
 results = client.query_batch(requests)
 
 for res in results:
@@ -271,14 +284,47 @@
         ## this will be a LogsQueryResult
         table = res.tables[0]
         df = pd.DataFrame(table.rows, columns=table.columns)
         print(df)
 
 ```
 
+### Resource logs query
+
+The following example demonstrates how to query logs directly from an Azure resource without the use of a Log Analytics workspace. Here, the `query_resource` method is used instead of `query_workspace`, and instead of a workspace ID, an Azure resource identifier is passed in (e.g. `/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}/providers/{resource-provider}/{resource-type}/{resource-name}`).
+
+```python
+import os
+import pandas as pd
+from datetime import timedelta
+from azure.monitor.query import LogsQueryClient, LogsQueryStatus
+from azure.core.exceptions import HttpResponseError
+from azure.identity import DefaultAzureCredential
+
+credential  = DefaultAzureCredential()
+client = LogsQueryClient(credential)
+
+query = """AzureActivity | take 5"""
+
+try:
+    response = client.query_resource(os.environ['LOGS_RESOURCE_ID'], query, timespan=timedelta(days=1))
+    if response.status == LogsQueryStatus.PARTIAL:
+        error = response.partial_error
+        data = response.partial_data
+        print(error)
+    elif response.status == LogsQueryStatus.SUCCESS:
+        data = response.tables
+    for table in data:
+        df = pd.DataFrame(data=table.rows, columns=table.columns)
+        print(df)
+except HttpResponseError as err:
+    print("something fatal happened")
+    print(err)
+```
+
 ### Advanced logs query scenarios
 
 #### Set logs query timeout
 
 The following example shows setting a server timeout in seconds. A gateway timeout is raised if the query takes more time than the mentioned timeout. The default is 180 seconds and can be set up to 10 minutes (600 seconds).
 
 ```python
@@ -492,27 +538,15 @@
                         metric_value.time_stamp
                     )
                 )
 ```
 
 ## Troubleshooting
 
-Enable the `azure.monitor.query` logger to collect traces from the library.
-
-### General
-
-Monitor Query client library will raise exceptions defined in [Azure Core][azure_core_exceptions].
-
-### Logging
-
-This library uses the standard [logging][python_logging] library for logging. Basic information about HTTP sessions, such as URLs and headers, is logged at the `INFO` level.
-
-### Optional configuration
-
-Optional keyword arguments can be passed in at the client and per-operation level. The `azure-core` [reference documentation][azure_core_ref_docs] describes available configurations for retries, logging, transport protocols, and more.
+See our [troubleshooting guide][troubleshooting_guide] for details on how to diagnose various failure scenarios.
 
 ## Next steps
 
 To learn more about Azure Monitor, see the [Azure Monitor service documentation][azure_monitor_overview].
 
 ### Samples
 
@@ -552,23 +586,38 @@
 [kusto_query_language]: https://learn.microsoft.com/azure/data-explorer/kusto/query/
 [package]: https://aka.ms/azsdk-python-monitor-query-pypi
 [pip]: https://pypi.org/project/pip/
 [python_logging]: https://docs.python.org/3/library/logging.html
 [python-query-ref-docs]: https://aka.ms/azsdk/python/monitor-query/docs
 [samples]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-query/samples
 [source]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-query/
+[troubleshooting_guide]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-query/TROUBLESHOOTING.md
 
 [cla]: https://cla.microsoft.com
 [code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
 [coc_faq]: https://opensource.microsoft.com/codeofconduct/faq/
 [coc_contact]: mailto:opencode@microsoft.com
 
 
 # Release History
 
+## 1.2.0 (2023-05-09)
+
+### Features Added
+
+- Add the `query_resource` method to `LogsQueryClient` to allow users to query Azure resources directly without the context of a workspace. ([#29365](https://github.com/Azure/azure-sdk-for-python/pull/29365))
+
+### Bugs Fixed
+
+- Fixed an inconsistent keyword argument name in the `LogsTable` constructor, changing `column_types` to `columns_types`. Note that this is a class that is typically only instantiated internally, and not by users. ([#29076](https://github.com/Azure/azure-sdk-for-python/pull/29076))
+
+### Other Changes
+
+- Improved client configuration logic for non-public Azure clouds where credential scope will be determined based on the configured endpoint. ([#29602](https://github.com/Azure/azure-sdk-for-python/pull/29602))
+
 ## 1.1.1 (2023-02-13)
 
 ### Bugs Fixed
 
 - Fixed a bug where the incorrect key `time_stamp` (should be `timeStamp`) was used in the creation of `MetricValue` objects (thanks @jamespic).  ([#28777](https://github.com/Azure/azure-sdk-for-python/pull/28777))
 
 ## 1.1.0 (2023-02-07)
```

## Comparing `azure-monitor-query-1.1.1/migration_guide.md` & `azure-monitor-query-1.2.0/migration_guide.md`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/TROUBLESHOOTING.md` & `azure-monitor-query-1.2.0/TROUBLESHOOTING.md`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/migration_guide_app_insights.md` & `azure-monitor-query-1.2.0/migration_guide_app_insights.md`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/setup.py` & `azure-monitor-query-1.2.0/setup.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/README.md` & `azure-monitor-query-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 - [Logs](https://learn.microsoft.com/azure/azure-monitor/logs/data-platform-logs) - Collects and organizes log and performance data from monitored resources. Data from different sources such as platform logs from Azure services, log and performance data from virtual machines agents, and usage and performance data from apps can be consolidated into a single [Azure Log Analytics workspace](https://learn.microsoft.com/azure/azure-monitor/logs/data-platform-logs#log-analytics-and-workspaces). The various data types can be analyzed together using the [Kusto Query Language][kusto_query_language].
 - [Metrics](https://learn.microsoft.com/azure/azure-monitor/essentials/data-platform-metrics) - Collects numeric data from monitored resources into a time series database. Metrics are numerical values that are collected at regular intervals and describe some aspect of a system at a particular time. Metrics are lightweight and capable of supporting near real-time scenarios, making them useful for alerting and fast detection of issues.
 
 **Resources:**
 
 - [Source code][source]
 - [Package (PyPI)][package]
+- [Package (Conda)](https://anaconda.org/microsoft/azure-monitor-query/)
 - [API reference documentation][python-query-ref-docs]
 - [Service documentation][azure_monitor_overview]
 - [Samples][samples]
 - [Change log][changelog]
 
 ## Getting started
 
@@ -58,14 +59,25 @@
 from azure.monitor.query.aio import LogsQueryClient, MetricsQueryClient
 
 credential = DefaultAzureCredential()
 async_logs_client = LogsQueryClient(credential)
 async_metrics_client = MetricsQueryClient(credential)
 ```
 
+#### Configure clients for non-public Azure clouds
+
+By default, `LogsQueryClient` and `MetricsQueryClient` are configured to connect to the public Azure cloud. These can be configured to connect to non-public Azure clouds by passing in the correct `endpoint` argument: For example:
+
+```python
+logs_client = LogsQueryClient(credential, endpoint="https://api.loganalytics.azure.cn/v1")
+metrics_client = MetricsQueryClient(credential, endpoint="https://management.chinacloudapi.cn")
+```
+
+**Note**: Currently, `MetricsQueryClient` uses the Azure Resource Manager (ARM) endpoint for querying metrics, so you will need the corresponding management endpoint for your cloud when using this client. This is subject to change in the future.
+
 ### Execute the query
 
 For examples of Logs and Metrics queries, see the [Examples](#examples) section.
 
 ## Key concepts
 
 ### Logs query rate limits and throttling
@@ -87,26 +99,27 @@
 
 ## Examples
 
 - [Logs query](#logs-query)
   - [Specify timespan](#specify-timespan)
   - [Handle logs query response](#handle-logs-query-response)
 - [Batch logs query](#batch-logs-query)
+- [Resource logs query](#resource-logs-query)
 - [Advanced logs query scenarios](#advanced-logs-query-scenarios)
   - [Set logs query timeout](#set-logs-query-timeout)
   - [Query multiple workspaces](#query-multiple-workspaces)
   - [Include statistics](#include-statistics)
   - [Include visualization](#include-visualization)
 - [Metrics query](#metrics-query)
   - [Handle metrics query response](#handle-metrics-query-response)
   - [Example of handling response](#example-of-handling-response)
 
 ### Logs query
 
-This example shows getting a logs query. To handle the response and view it in a tabular form, the [pandas](https://pypi.org/project/pandas/) library is used. See the [samples][samples] if you choose not to use pandas.
+This example shows how to query a Log Analytics workspace. To handle the response and view it in a tabular form, the [pandas](https://pypi.org/project/pandas/) library is used. See the [samples][samples] if you choose not to use pandas.
 
 #### Specify timespan
 
 The `timespan` parameter specifies the time duration for which to query the data. This value can be one of the following:
 
 - a `timedelta`
 - a `timedelta` and a start datetime
@@ -143,44 +156,44 @@
     elif response.status == LogsQueryStatus.SUCCESS:
         data = response.tables
     for table in data:
         df = pd.DataFrame(data=table.rows, columns=table.columns)
         print(df)
 except HttpResponseError as err:
     print("something fatal happened")
-    print (err)
+    print(err)
 ```
 
 #### Handle logs query response
 
 The `query_workspace` API returns either a `LogsQueryResult` or a `LogsQueryPartialResult` object. The `batch_query` API returns a list that may contain `LogsQueryResult`, `LogsQueryPartialResult`, and `LogsQueryError` objects. Here's a hierarchy of the response:
 
 ```
 LogsQueryResult
 |---statistics
 |---visualization
 |---tables (list of `LogsTable` objects)
     |---name
     |---rows
     |---columns
-    |---column_types
+    |---columns_types
 
 LogsQueryPartialResult
 |---statistics
 |---visualization
 |---partial_error (a `LogsQueryError` object)
     |---code
     |---message
     |---details
     |---status
 |---partial_data (list of `LogsTable` objects)
     |---name
     |---rows
     |---columns
-    |---column_types
+    |---columns_types
 ```
 
 The `LogsQueryResult` directly iterates over the table as a convenience. For example, to handle a logs query response with tables and display it using pandas:
 
 ```python
 response = client.query(...)
 for table in response:
@@ -214,26 +227,26 @@
 
 credential = DefaultAzureCredential()
 client = LogsQueryClient(credential)
 requests = [
     LogsBatchQuery(
         query="AzureActivity | summarize count()",
         timespan=timedelta(hours=1),
-        workspace_id= os.environ['LOG_WORKSPACE_ID']
+        workspace_id=os.environ['LOG_WORKSPACE_ID']
     ),
     LogsBatchQuery(
         query= """bad query""",
         timespan=timedelta(days=1),
-        workspace_id= os.environ['LOG_WORKSPACE_ID']
+        workspace_id=os.environ['LOG_WORKSPACE_ID']
     ),
     LogsBatchQuery(
         query= """let Weight = 92233720368547758;
         range x from 1 to 3 step 1
         | summarize percentilesw(x, Weight * 100, 50)""",
-        workspace_id= os.environ['LOG_WORKSPACE_ID'],
+        workspace_id=os.environ['LOG_WORKSPACE_ID'],
         timespan=(datetime(2021, 6, 2, tzinfo=timezone.utc), datetime(2021, 6, 5, tzinfo=timezone.utc)), # (start, end)
         include_statistics=True
     ),
 ]
 results = client.query_batch(requests)
 
 for res in results:
@@ -250,14 +263,47 @@
         ## this will be a LogsQueryResult
         table = res.tables[0]
         df = pd.DataFrame(table.rows, columns=table.columns)
         print(df)
 
 ```
 
+### Resource logs query
+
+The following example demonstrates how to query logs directly from an Azure resource without the use of a Log Analytics workspace. Here, the `query_resource` method is used instead of `query_workspace`, and instead of a workspace ID, an Azure resource identifier is passed in (e.g. `/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}/providers/{resource-provider}/{resource-type}/{resource-name}`).
+
+```python
+import os
+import pandas as pd
+from datetime import timedelta
+from azure.monitor.query import LogsQueryClient, LogsQueryStatus
+from azure.core.exceptions import HttpResponseError
+from azure.identity import DefaultAzureCredential
+
+credential  = DefaultAzureCredential()
+client = LogsQueryClient(credential)
+
+query = """AzureActivity | take 5"""
+
+try:
+    response = client.query_resource(os.environ['LOGS_RESOURCE_ID'], query, timespan=timedelta(days=1))
+    if response.status == LogsQueryStatus.PARTIAL:
+        error = response.partial_error
+        data = response.partial_data
+        print(error)
+    elif response.status == LogsQueryStatus.SUCCESS:
+        data = response.tables
+    for table in data:
+        df = pd.DataFrame(data=table.rows, columns=table.columns)
+        print(df)
+except HttpResponseError as err:
+    print("something fatal happened")
+    print(err)
+```
+
 ### Advanced logs query scenarios
 
 #### Set logs query timeout
 
 The following example shows setting a server timeout in seconds. A gateway timeout is raised if the query takes more time than the mentioned timeout. The default is 180 seconds and can be set up to 10 minutes (600 seconds).
 
 ```python
@@ -471,27 +517,15 @@
                         metric_value.time_stamp
                     )
                 )
 ```
 
 ## Troubleshooting
 
-Enable the `azure.monitor.query` logger to collect traces from the library.
-
-### General
-
-Monitor Query client library will raise exceptions defined in [Azure Core][azure_core_exceptions].
-
-### Logging
-
-This library uses the standard [logging][python_logging] library for logging. Basic information about HTTP sessions, such as URLs and headers, is logged at the `INFO` level.
-
-### Optional configuration
-
-Optional keyword arguments can be passed in at the client and per-operation level. The `azure-core` [reference documentation][azure_core_ref_docs] describes available configurations for retries, logging, transport protocols, and more.
+See our [troubleshooting guide][troubleshooting_guide] for details on how to diagnose various failure scenarios.
 
 ## Next steps
 
 To learn more about Azure Monitor, see the [Azure Monitor service documentation][azure_monitor_overview].
 
 ### Samples
 
@@ -531,12 +565,13 @@
 [kusto_query_language]: https://learn.microsoft.com/azure/data-explorer/kusto/query/
 [package]: https://aka.ms/azsdk-python-monitor-query-pypi
 [pip]: https://pypi.org/project/pip/
 [python_logging]: https://docs.python.org/3/library/logging.html
 [python-query-ref-docs]: https://aka.ms/azsdk/python/monitor-query/docs
 [samples]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-query/samples
 [source]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-query/
+[troubleshooting_guide]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-query/TROUBLESHOOTING.md
 
 [cla]: https://cla.microsoft.com
 [code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
 [coc_faq]: https://opensource.microsoft.com/codeofconduct/faq/
 [coc_contact]: mailto:opencode@microsoft.com
```

## Comparing `azure-monitor-query-1.1.1/LICENSE` & `azure-monitor-query-1.2.0/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/CHANGELOG.md` & `azure-monitor-query-1.2.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,23 @@
 # Release History
 
+## 1.2.0 (2023-05-09)
+
+### Features Added
+
+- Add the `query_resource` method to `LogsQueryClient` to allow users to query Azure resources directly without the context of a workspace. ([#29365](https://github.com/Azure/azure-sdk-for-python/pull/29365))
+
+### Bugs Fixed
+
+- Fixed an inconsistent keyword argument name in the `LogsTable` constructor, changing `column_types` to `columns_types`. Note that this is a class that is typically only instantiated internally, and not by users. ([#29076](https://github.com/Azure/azure-sdk-for-python/pull/29076))
+
+### Other Changes
+
+- Improved client configuration logic for non-public Azure clouds where credential scope will be determined based on the configured endpoint. ([#29602](https://github.com/Azure/azure-sdk-for-python/pull/29602))
+
 ## 1.1.1 (2023-02-13)
 
 ### Bugs Fixed
 
 - Fixed a bug where the incorrect key `time_stamp` (should be `timeStamp`) was used in the creation of `MetricValue` objects (thanks @jamespic).  ([#28777](https://github.com/Azure/azure-sdk-for-python/pull/28777))
 
 ## 1.1.0 (2023-02-07)
```

## Comparing `azure-monitor-query-1.1.1/samples/sample_single_log_query_without_pandas.py` & `azure-monitor-query-1.2.0/samples/sample_single_log_query_without_pandas.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/samples/sample_batch_query.py` & `azure-monitor-query-1.2.0/samples/sample_batch_query.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/samples/sample_server_timeout.py` & `azure-monitor-query-1.2.0/samples/sample_server_timeout.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/samples/sample_metric_namespaces.py` & `azure-monitor-query-1.2.0/samples/sample_metric_namespaces.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/samples/sample_metrics_query.py` & `azure-monitor-query-1.2.0/samples/sample_metrics_query.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/samples/sample_log_query_multiple_workspaces.py` & `azure-monitor-query-1.2.0/samples/sample_log_query_multiple_workspaces.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/samples/sample_logs_single_query.py` & `azure-monitor-query-1.2.0/samples/sample_logs_single_query.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/samples/sample_logs_single_query_partial_result.py` & `azure-monitor-query-1.2.0/samples/sample_logs_single_query_partial_result.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/samples/sample_logs_query_key_value_form.py` & `azure-monitor-query-1.2.0/samples/sample_logs_query_key_value_form.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/samples/sample_metric_definitions.py` & `azure-monitor-query-1.2.0/samples/sample_metric_definitions.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/samples/async_samples/sample_metric_namespaces_async.py` & `azure-monitor-query-1.2.0/samples/async_samples/sample_metric_namespaces_async.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/samples/async_samples/sample_metrics_query_async.py` & `azure-monitor-query-1.2.0/samples/async_samples/sample_metrics_query_async.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/samples/async_samples/sample_log_query_async.py` & `azure-monitor-query-1.2.0/samples/async_samples/sample_log_query_async.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/samples/async_samples/sample_metric_definitions_async.py` & `azure-monitor-query-1.2.0/samples/async_samples/sample_metric_definitions_async.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_models.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     """Required. The labels of columns in this table."""
     columns_types: List[str]
     """Required. The types of columns in this table."""
 
     def __init__(self, **kwargs: Any) -> None:
         self.name = kwargs.pop("name", "")
         self.columns = kwargs.pop("columns", [])
-        self.columns_types = kwargs.pop("column_types", [])
+        self.columns_types = kwargs.pop("columns_types", [])
         _rows = kwargs.pop("rows", [])
         self.rows: List[LogsTableRow] = [
             LogsTableRow(
                 row=row,
                 row_index=ind,
                 col_types=self.columns_types,
                 columns=self.columns,
@@ -95,15 +95,15 @@
         ]
 
     @classmethod
     def _from_generated(cls, generated) -> "LogsTable":
         return cls(
             name=generated.get("name"),
             columns=[col["name"] for col in generated.get("columns", [])],
-            column_types=[col["type"] for col in generated.get("columns", [])],
+            columns_types=[col["type"] for col in generated.get("columns", [])],
             rows=generated.get("rows"),
         )
 
 
 class MetricValue:
     """Represents a metric value."""
 
@@ -117,15 +117,14 @@
     """The greatest value in the time range."""
     total: Optional[float] = None
     """The sum of all of the values in the time range."""
     count: Optional[float] = None
     """The number of samples in the time range. Can be used to determine the number of values that
     contributed to the average value."""
 
-
     def __init__(self, **kwargs: Any) -> None:
         self.timestamp = kwargs["timestamp"]
         self.average = kwargs.get("average", None)
         self.minimum = kwargs.get("minimum", None)
         self.maximum = kwargs.get("maximum", None)
         self.total = kwargs.get("total", None)
         self.count = kwargs.get("count", None)
@@ -158,19 +157,18 @@
         self.data = kwargs.get("data", [])
 
     @classmethod
     def _from_generated(cls, generated) -> "TimeSeriesElement":
         if not generated:
             return cls()
         return cls(
-            metadata_values={
-                obj["name"]["value"]: obj.get("value") for obj in generated.get("metadatavalues", [])
-            },
+            metadata_values={obj["name"]["value"]: obj.get("value") for obj in generated.get("metadatavalues", [])},
             data=[
-                MetricValue._from_generated(val) for val in generated.get("data", []) # pylint: disable=protected-access
+                MetricValue._from_generated(val)  # pylint: disable=protected-access
+                for val in generated.get("data", [])
             ],
         )
 
 
 class Metric:
     """The result data of a single metric name."""
 
@@ -203,15 +201,15 @@
             return cls()
         return cls(
             id=generated.get("id"),
             type=generated.get("type"),
             name=generated.get("name", {}).get("value"),
             unit=generated.get("unit"),
             timeseries=[
-                TimeSeriesElement._from_generated(t) # pylint: disable=protected-access
+                TimeSeriesElement._from_generated(t)  # pylint: disable=protected-access
                 for t in generated.get("timeseries", [])
             ],
             display_description=generated.get("displayDescription"),
         )
 
 
 class MetricsQueryResult:
@@ -230,18 +228,17 @@
     namespace: Optional[str] = None
     """The namespace of the metrics that has been queried."""
     resource_region: Optional[str] = None
     """The region of the resource that has been queried for metrics."""
     cost: Optional[int] = None
     """The integer value representing the cost of the query, for data case."""
 
-
     def __init__(self, **kwargs: Any) -> None:
         self.timespan = kwargs["timespan"]
-        self.metrics= kwargs["metrics"]
+        self.metrics = kwargs["metrics"]
         self.granularity = kwargs.get("granularity", None)
         self.namespace = kwargs.get("namespace", None)
         self.resource_region = kwargs.get("resource_region", None)
         self.cost = kwargs.get("cost", None)
 
     @classmethod
     def _from_generated(cls, generated) -> "MetricsQueryResult":
@@ -252,40 +249,42 @@
             granularity = Deserializer.deserialize_duration(generated.get("interval"))
         return cls(
             cost=generated.get("cost"),
             timespan=generated.get("timespan"),
             granularity=granularity,
             namespace=generated.get("namespace"),
             resource_region=generated.get("resourceregion"),
-            metrics=MetricsList(metrics=[
-                Metric._from_generated(m) for m in generated.get("value", []) # pylint: disable=protected-access
-            ]),
+            metrics=MetricsList(
+                metrics=[
+                    Metric._from_generated(m) for m in generated.get("value", [])  # pylint: disable=protected-access
+                ]
+            ),
         )
 
 
 class MetricsList(list):
     """Custom list for metrics."""
 
-    def __init__(self, **kwargs: Any) -> None: # pylint: disable=super-init-not-called
-        self._metrics = kwargs['metrics']
+    def __init__(self, **kwargs: Any) -> None:  # pylint: disable=super-init-not-called
+        self._metrics = kwargs["metrics"]
         self._metric_names = {val.name: ind for ind, val in enumerate(self._metrics)}
 
     def __iter__(self):
         return iter(self._metrics)
 
     def __len__(self):
         return len(self._metrics)
 
     def __repr__(self):
         return repr(self._metrics)
 
     def __getitem__(self, metric):
         try:
             return self._metrics[metric]
-        except TypeError: # TypeError: list indices must be integers or slices, not str
+        except TypeError:  # TypeError: list indices must be integers or slices, not str
             return self._metrics[self._metric_names[metric]]
 
 
 class LogsBatchQuery:
     """A single request in a batch. The batch query API accepts a list of these objects.
 
     :param workspace_id: Workspace ID to be included in the query.
@@ -313,17 +312,15 @@
     """
 
     def __init__(
         self,
         workspace_id: str,
         query: str,
         *,
-        timespan: Optional[Union[
-            timedelta, Tuple[datetime, timedelta], Tuple[datetime, datetime]
-        ]],
+        timespan: Optional[Union[timedelta, Tuple[datetime, timedelta], Tuple[datetime, datetime]]],
         **kwargs: Any
     ) -> None:  # pylint: disable=super-init-not-called
         include_statistics = kwargs.pop("include_statistics", False)
         include_visualization = kwargs.pop("include_visualization", False)
         server_timeout = kwargs.pop("server_timeout", None)
         prefer = ""
         if server_timeout:
@@ -352,15 +349,15 @@
     def _to_generated(self) -> Dict[str, Any]:
         return {
             "id": self.id,
             "body": self.body,
             "headers": self.headers,
             "workspace": self.workspace,
             "path": "/query",
-            "method": "POST"
+            "method": "POST",
         }
 
 
 class LogsQueryResult:
     """The LogsQueryResult type is returned when the response of a query is a success."""
 
     tables: List[LogsTable]
@@ -388,16 +385,15 @@
         if not generated:
             return cls()
         tables = []
         if "body" in generated:
             generated = generated["body"]
         if generated.get("tables"):
             tables = [
-                LogsTable._from_generated(table)  # pylint: disable=protected-access
-                for table in generated["tables"]
+                LogsTable._from_generated(table) for table in generated["tables"]  # pylint: disable=protected-access
             ]
         return cls(
             tables=tables,
             statistics=generated.get("statistics"),
             visualization=generated.get("render"),
         )
 
@@ -412,15 +408,14 @@
     name: Optional[str] = None
     """The name of the namespace."""
     fully_qualified_namespace: Optional[str] = None
     """The fully qualified namespace name."""
     namespace_classification: Optional[Union[str, MetricNamespaceClassification]] = None
     """Kind of namespace. Possible values include "Platform", "Custom", "Qos"."""
 
-
     def __init__(self, **kwargs: Any) -> None:
         self.id = kwargs.get("id", None)
         self.type = kwargs.get("type", None)
         self.name = kwargs.get("name", None)
         self.fully_qualified_namespace = kwargs.get("fully_qualified_namespace", None)
         self.namespace_classification = kwargs.get("namespace_classification", None)
 
@@ -459,18 +454,15 @@
         if not generated:
             return cls()
         granularity, retention = None, None
         if generated.get("timeGrain"):
             granularity = Deserializer.deserialize_duration(generated["timeGrain"])
         if generated.get("retention"):
             retention = Deserializer.deserialize_duration(generated["retention"])
-        return cls(
-            granularity=granularity,
-            retention=retention
-        )
+        return cls(granularity=granularity, retention=retention)
 
 
 class MetricDefinition:  # pylint: disable=too-many-instance-attributes
     """Metric definition class specifies the metadata for a metric."""
 
     dimension_required: Optional[bool] = None
     """Flag to indicate whether the dimension is required."""
@@ -495,23 +487,22 @@
     metric_availabilities: Optional[List[MetricAvailability]] = None
     """The collection of what aggregation intervals are available to be queried."""
     id: Optional[str] = None
     """The resource identifier of the metric definition."""
     dimensions: Optional[List[str]] = None
     """The name and the display name of the dimension, i.e. it is a localizable string."""
 
-
     def __init__(self, **kwargs: Any) -> None:
         self.dimension_required = kwargs.get("dimension_required", None)
         self.resource_id = kwargs.get("resource_id", None)
         self.namespace = kwargs.get("namespace", None)
         self.name = kwargs.get("name", None)
         self.unit = kwargs.get("unit", None)
         self.primary_aggregation_type = kwargs.get("primary_aggregation_type", None)
-        self.supported_aggregation_types =kwargs.get("supported_aggregation_types", None)
+        self.supported_aggregation_types = kwargs.get("supported_aggregation_types", None)
         self.metric_availabilities = kwargs.get("metric_availabilities", None)
         self.id = kwargs.get("id", None)
         self.dimensions = kwargs.get("dimensions", None)
         self.metric_class = kwargs.get("metric_class", None)
 
     @classmethod
     def _from_generated(cls, generated) -> "MetricDefinition":
@@ -528,17 +519,15 @@
             namespace=generated.get("namespace"),
             name=generated.get("name", {}).get("value"),
             unit=generated.get("unit"),
             primary_aggregation_type=generated.get("primaryAggregationType"),
             supported_aggregation_types=generated.get("supportedAggregationTypes"),
             metric_class=metric_class,
             metric_availabilities=[
-                MetricAvailability._from_generated(  # pylint: disable=protected-access
-                    val
-                )
+                MetricAvailability._from_generated(val)  # pylint: disable=protected-access
                 for val in generated.get("metricAvailabilities", [])
             ],
             id=generated.get("id"),
             dimensions=dimensions,
         )
 
 
@@ -556,15 +545,14 @@
     """This will include a visualization property in the response that specifies the type of visualization
     selected by the query and any properties for that visualization."""
     partial_error: Optional[LogsQueryError] = None
     """The partial error info."""
     status: LogsQueryStatus
     """The status of the result. Always 'PartialError' for an instance of a LogsQueryPartialResult."""
 
-
     def __init__(self, **kwargs: Any) -> None:
         self.partial_data = kwargs.get("partial_data", [])
         self.partial_error = kwargs.get("partial_error", None)
         self.statistics = kwargs.get("statistics", None)
         self.visualization = kwargs.get("visualization", None)
         self.status = LogsQueryStatus.PARTIAL
 
@@ -576,16 +564,15 @@
         if not generated:
             return cls()
         partial_data = None
         if "body" in generated:
             generated = generated["body"]
         if generated.get("tables"):
             partial_data = [
-                LogsTable._from_generated(table)  # pylint: disable=protected-access
-                for table in generated["tables"]
+                LogsTable._from_generated(table) for table in generated["tables"]  # pylint: disable=protected-access
             ]
         return cls(
             partial_data=partial_data,
-            partial_error=error._from_generated(generated.get("error")), # pylint: disable=protected-access
+            partial_error=error._from_generated(generated.get("error")),  # pylint: disable=protected-access
             statistics=generated.get("statistics"),
             visualization=generated.get("render"),
         )
```

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_metrics_query_client.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_metrics_query_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from azure.core.credentials import TokenCredential
 from azure.core.paging import ItemPaged
 from azure.core.tracing.decorator import distributed_trace
 
 from ._generated._serialization import Serializer
 from ._generated.metrics._client import MonitorMetricsClient
 from ._models import MetricsQueryResult, MetricDefinition, MetricNamespace
-from ._helpers import get_metrics_authentication_policy, construct_iso8601
+from ._helpers import get_authentication_policy, construct_iso8601
 
 
-class MetricsQueryClient(object): # pylint: disable=client-accepts-api-version-keyword
+class MetricsQueryClient(object):  # pylint: disable=client-accepts-api-version-keyword
     """MetricsQueryClient should be used to collect numeric data from monitored resources into a
     time series database. Metrics are numerical values that are collected at regular intervals and
     describe some aspect of a system at a particular time. Metrics are lightweight and capable of
     supporting near real-time scenarios, making them particularly useful for alerting and
     fast detection of issues.
 
     .. admonition:: Example:
@@ -36,24 +36,24 @@
     :param credential: The credential to authenticate the client.
     :type credential: ~azure.core.credentials.TokenCredential
     :keyword endpoint: The endpoint to connect to. Defaults to 'https://management.azure.com'.
     :paramtype endpoint: Optional[str]
     """
 
     def __init__(self, credential: TokenCredential, **kwargs: Any) -> None:
-        audience = kwargs.pop("audience", None)
         endpoint = kwargs.pop("endpoint", "https://management.azure.com")
+        audience = kwargs.pop("audience", endpoint)
         if not endpoint.startswith("https://") and not endpoint.startswith("http://"):
             endpoint = "https://" + endpoint
         self._endpoint = endpoint
         auth_policy = kwargs.pop("authentication_policy", None)
         self._client = MonitorMetricsClient(
             credential=credential,
             endpoint=self._endpoint,
-            authentication_policy=auth_policy or get_metrics_authentication_policy(credential, audience),
+            authentication_policy=auth_policy or get_authentication_policy(credential, audience),
             **kwargs
         )
         self._metrics_op = self._client.metrics
         self._namespace_op = self._client.metric_namespaces
         self._definitions_op = self._client.metric_definitions
 
     @distributed_trace
@@ -118,20 +118,16 @@
         metric_names = [x.replace(",", "%2") for x in metric_names]
         kwargs.setdefault("metricnames", ",".join(metric_names))
         kwargs.setdefault("timespan", timespan)
         kwargs.setdefault("top", kwargs.pop("max_results", None))
         kwargs.setdefault("interval", kwargs.pop("granularity", None))
         kwargs.setdefault("orderby", kwargs.pop("order_by", None))
         kwargs.setdefault("metricnamespace", kwargs.pop("metric_namespace", None))
-        generated = self._metrics_op.list(
-            resource_uri, connection_verify=False, **kwargs
-        )
-        return MetricsQueryResult._from_generated( # pylint: disable=protected-access
-            generated
-        )
+        generated = self._metrics_op.list(resource_uri, connection_verify=False, **kwargs)
+        return MetricsQueryResult._from_generated(generated)  # pylint: disable=protected-access
 
     @distributed_trace
     def list_metric_namespaces(self, resource_uri: str, **kwargs: Any) -> ItemPaged[MetricNamespace]:
         """Lists the metric namespaces for the resource.
 
         :param resource_uri: The identifier of the resource.
         :type resource_uri: str
@@ -146,18 +142,15 @@
         if start_time:
             start_time = Serializer.serialize_iso(start_time)
         res = self._namespace_op.list(
             resource_uri,
             start_time=start_time,
             cls=kwargs.pop(
                 "cls",
-                lambda objs: [
-                    MetricNamespace._from_generated(x) # pylint: disable=protected-access
-                    for x in objs
-                ],
+                lambda objs: [MetricNamespace._from_generated(x) for x in objs],  # pylint: disable=protected-access
             ),
             **kwargs
         )
         return cast(ItemPaged[MetricNamespace], res)
 
     @distributed_trace
     def list_metric_definitions(self, resource_uri: str, **kwargs: Any) -> ItemPaged[MetricDefinition]:
@@ -173,18 +166,15 @@
         """
         metric_namespace = kwargs.pop("namespace", None)
         res = self._definitions_op.list(
             resource_uri,
             metricnamespace=metric_namespace,
             cls=kwargs.pop(
                 "cls",
-                lambda objs: [
-                    MetricDefinition._from_generated(x) # pylint: disable=protected-access
-                    for x in objs
-                ],
+                lambda objs: [MetricDefinition._from_generated(x) for x in objs],  # pylint: disable=protected-access
             ),
             **kwargs
         )
         return cast(ItemPaged[MetricDefinition], res)
 
     def close(self) -> None:
         """Close the :class:`~azure.monitor.query.MetricsQueryClient` session."""
```

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_helpers.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,93 +10,60 @@
 from azure.core.credentials import TokenCredential
 from azure.core.exceptions import HttpResponseError
 from azure.core.pipeline.policies import BearerTokenCredentialPolicy
 
 from ._generated._serialization import Serializer, Deserializer
 
 
-def get_authentication_policy(
-    credential: TokenCredential,
-    audience: Optional[str] = None
-) -> BearerTokenCredentialPolicy:
+def get_authentication_policy(credential: TokenCredential, audience: str) -> BearerTokenCredentialPolicy:
     """Returns the correct authentication policy"""
-    if not audience:
-        audience = "https://api.loganalytics.io/"
-    scope = audience.rstrip('/') + "/.default"
     if credential is None:
         raise ValueError("Parameter 'credential' must not be None.")
+    scope = audience.rstrip("/") + "/.default"
     if hasattr(credential, "get_token"):
-        return BearerTokenCredentialPolicy(
-            credential, scope
-        )
-
-    raise TypeError("Unsupported credential")
-
-
-def get_metrics_authentication_policy(
-    credential: TokenCredential,
-    audience: Optional[str] = None
-) -> BearerTokenCredentialPolicy:
-    """Returns the correct authentication policy"""
-    if not audience:
-        audience = "https://management.azure.com/"
-    scope = audience.rstrip('/') + "/.default"
-    if credential is None:
-        raise ValueError("Parameter 'credential' must not be None.")
-    if hasattr(credential, "get_token"):
-        return BearerTokenCredentialPolicy(
-            credential, scope
-        )
+        return BearerTokenCredentialPolicy(credential, scope)
 
     raise TypeError("Unsupported credential")
 
 
 def order_results(request_order: List, mapping: Dict[str, Any], **kwargs: Any) -> List:
     ordered = [mapping[id] for id in request_order]
     results = []
     for item in ordered:
         if not item["body"].get("error"):
             result_obj = kwargs.get("obj")
             if result_obj:
-                results.append(
-                    result_obj._from_generated(item["body"]) # pylint: disable=protected-access
-                )
+                results.append(result_obj._from_generated(item["body"]))  # pylint: disable=protected-access
         else:
             error = item["body"]["error"]
             if error.get("code") == "PartialError":
                 partial_err = kwargs.get("partial_err")
                 if partial_err:
                     res = partial_err._from_generated(  # pylint: disable=protected-access
                         item["body"], kwargs.get("raise_with")
                     )
                     results.append(res)
             else:
                 err = kwargs.get("err")
                 if err:
-                    results.append(
-                        err._from_generated(error) # pylint: disable=protected-access
-                    )
+                    results.append(err._from_generated(error))  # pylint: disable=protected-access
     return results
 
 
 def construct_iso8601(timespan=None) -> Optional[str]:
     if not timespan:
         return None
     start, end, duration = None, None, None
     try:
         if isinstance(timespan[1], datetime):  # we treat thi as start_time, end_time
             start, end = timespan[0], timespan[1]
-        elif isinstance(
-            timespan[1], timedelta
-        ):  # we treat this as start_time, duration
+        elif isinstance(timespan[1], timedelta):  # we treat this as start_time, duration
             start, duration = timespan[0], timespan[1]
         else:
-            raise ValueError(
-                "Tuple must be a start datetime with a timedelta or an end datetime."
-            )
+            raise ValueError("Tuple must be a start datetime with a timedelta or an end datetime.")
     except TypeError:
         duration = timespan  # it means only duration (timedelta) is provideds
     duration_str = ""
     if duration:
         try:
             duration_str = "PT{}S".format(duration.total_seconds())
         except AttributeError:
@@ -106,44 +73,40 @@
         start = Serializer.serialize_iso(start)
         if end is not None:
             end = Serializer.serialize_iso(end)
             iso_str = f"{start}/{end}"
         elif duration_str:
             iso_str = f"{start}/{duration_str}"
         else:  # means that an invalid value None that is provided with start_time
-            raise ValueError(
-                "Duration or end_time cannot be None when provided with start_time."
-            )
+            raise ValueError("Duration or end_time cannot be None when provided with start_time.")
     else:
         iso_str = duration_str
     return iso_str
 
 
 def native_col_type(col_type, value):
     if col_type == "datetime":
         try:
             value = Deserializer.deserialize_iso(value)
-        except Exception: # pylint: disable=broad-except
+        except Exception:  # pylint: disable=broad-except
             # if there is any exception in deserializing the iso,
             # return the value to the user
             pass
     elif col_type in ("timespan", "guid"):
         value = str(value)
     return value
 
 
 def process_row(col_types, row) -> List[Any]:
     return [native_col_type(col_types[ind], val) for ind, val in enumerate(row)]
 
 
 def process_error(error, model):
     try:
-        model = model._from_generated( # pylint: disable=protected-access
-            error.model.error
-        )
+        model = model._from_generated(error.model.error)  # pylint: disable=protected-access
     except AttributeError:  # model can be none
         pass
     raise HttpResponseError(message=error.message, response=error.response, model=model)
 
 
 def process_prefer(server_timeout, include_statistics, include_visualization):
     prefer = ""
```

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_enums.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_enums.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_logs_query_client.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_logs_query_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
-from typing import Any, Union, Sequence, Dict, List, cast, Tuple, Optional
 from datetime import timedelta, datetime
+from typing import Any, Union, Sequence, Dict, List, cast, Tuple, Optional
+from urllib.parse import urlparse
 
 from azure.core.credentials import TokenCredential
 from azure.core.exceptions import HttpResponseError
 from azure.core.tracing.decorator import distributed_trace
 
 from ._generated._client import MonitorQueryClient
 from ._helpers import (
@@ -19,15 +20,15 @@
     process_error,
     process_prefer,
 )
 from ._models import LogsBatchQuery, LogsQueryResult, LogsQueryPartialResult
 from ._exceptions import LogsQueryError
 
 
-class LogsQueryClient(object): # pylint: disable=client-accepts-api-version-keyword
+class LogsQueryClient(object):  # pylint: disable=client-accepts-api-version-keyword
     """LogsQueryClient. Use this client to collect and organize log and performance data from
     monitored resources. Data from different sources such as platform logs from Azure services,
     log and performance data from virtual machines agents, and usage and performance data from
     apps can be consolidated into a single Azure Log Analytics workspace.
 
     The various data types can be analyzed together using the
     [Kusto Query Language](https://docs.microsoft.com/azure/data-explorer/kusto/query/)
@@ -39,43 +40,43 @@
         :end-before: [END client_auth_with_token_cred]
         :language: python
         :dedent: 0
         :caption: Creating the LogsQueryClient with a TokenCredential.
 
     :param credential: The credential to authenticate the client.
     :type credential: ~azure.core.credentials.TokenCredential
-    :keyword endpoint: The endpoint to connect to. Defaults to 'https://api.loganalytics.io'.
+    :keyword endpoint: The endpoint to connect to. Defaults to 'https://api.loganalytics.io/v1'.
     :paramtype endpoint: Optional[str]
     """
 
     def __init__(self, credential: TokenCredential, **kwargs: Any) -> None:
-        endpoint = kwargs.pop("endpoint", "https://api.loganalytics.io")
+        endpoint = kwargs.pop("endpoint", "https://api.loganalytics.io/v1")
         if not endpoint.startswith("https://") and not endpoint.startswith("http://"):
             endpoint = "https://" + endpoint
+        parsed_endpoint = urlparse(endpoint)
+        audience = kwargs.pop("audience", f"{parsed_endpoint.scheme}://{parsed_endpoint.netloc}")
         self._endpoint = endpoint
         auth_policy = kwargs.pop("authentication_policy", None)
         self._client = MonitorQueryClient(
             credential=credential,
-            authentication_policy=auth_policy or get_authentication_policy(credential, endpoint),
-            endpoint=self._endpoint.rstrip('/') + "/v1",
-            **kwargs
+            authentication_policy=auth_policy or get_authentication_policy(credential, audience),
+            endpoint=self._endpoint,
+            **kwargs,
         )
         self._query_op = self._client.query
 
     @distributed_trace
     def query_workspace(
         self,
         workspace_id: str,
         query: str,
         *,
-        timespan: Optional[Union[
-            timedelta, Tuple[datetime, timedelta], Tuple[datetime, datetime]]
-        ],
-        **kwargs: Any
-        ) -> Union[LogsQueryResult, LogsQueryPartialResult]:
+        timespan: Optional[Union[timedelta, Tuple[datetime, timedelta], Tuple[datetime, datetime]]],
+        **kwargs: Any,
+    ) -> Union[LogsQueryResult, LogsQueryPartialResult]:
         """Execute a Kusto query.
 
         Executes a Kusto query for data.
 
         :param workspace_id: ID of the workspace. This is Workspace ID from the Properties blade in the
          Azure portal.
         :type workspace_id: str
@@ -88,17 +89,17 @@
         :paramtype timespan: ~datetime.timedelta or tuple[~datetime.datetime, ~datetime.timedelta]
          or tuple[~datetime.datetime, ~datetime.datetime] or None
         :keyword int server_timeout: the server timeout in seconds. The default timeout is 3 minutes,
          and the maximum timeout is 10 minutes.
         :keyword bool include_statistics: To get information about query statistics.
         :keyword bool include_visualization: In the query language, it is possible to specify different
          visualization options. By default, the API does not return information regarding the type of
-         visualization to show. If your client requires this information, specify the preference
+         visualization to show. If your client requires this information, specify the preference.
         :keyword additional_workspaces: A list of workspaces that are included in the query.
-         These can be qualified workspace names, workspace Ids, or Azure resource Ids.
+         These can be qualified workspace names, workspace IDs, or Azure resource IDs.
         :paramtype additional_workspaces: Optional[list[str]]
         :return: LogsQueryResult if there is a success or LogsQueryPartialResult when there is a partial success.
         :rtype: Union[~azure.monitor.query.LogsQueryResult, ~azure.monitor.query.LogsQueryPartialResult]
         :raises: ~azure.core.exceptions.HttpResponseError
 
         .. admonition:: Example:
 
@@ -111,49 +112,37 @@
         """
         timespan_iso = construct_iso8601(timespan)
         include_statistics = kwargs.pop("include_statistics", False)
         include_visualization = kwargs.pop("include_visualization", False)
         server_timeout = kwargs.pop("server_timeout", None)
         additional_workspaces = kwargs.pop("additional_workspaces", None)
 
-        prefer = process_prefer(
-            server_timeout, include_statistics, include_visualization
-        )
+        prefer = process_prefer(server_timeout, include_statistics, include_visualization)
 
-        body = {
-            "query": query,
-            "timespan": timespan_iso,
-            "workspaces": additional_workspaces
-        }
+        body = {"query": query, "timespan": timespan_iso, "workspaces": additional_workspaces}
 
         try:
-            generated_response = (
-                self._query_op.execute(  # pylint: disable=protected-access
-                    workspace_id=workspace_id, body=body, prefer=prefer, **kwargs
-                )
+            generated_response = self._query_op.execute(  # pylint: disable=protected-access
+                workspace_id=workspace_id, body=body, prefer=prefer, **kwargs
             )
         except HttpResponseError as err:
             process_error(err, LogsQueryError)
 
         response: Union[LogsQueryResult, LogsQueryPartialResult]
         if not generated_response.get("error"):
-            response = LogsQueryResult._from_generated( # pylint: disable=protected-access
-                generated_response
-            )
+            response = LogsQueryResult._from_generated(generated_response)  # pylint: disable=protected-access
         else:
-            response = LogsQueryPartialResult._from_generated( # pylint: disable=protected-access
+            response = LogsQueryPartialResult._from_generated(  # pylint: disable=protected-access
                 generated_response, LogsQueryError
             )
         return response
 
     @distributed_trace
     def query_batch(
-        self,
-        queries: Union[Sequence[Dict], Sequence[LogsBatchQuery]],
-        **kwargs: Any
+        self, queries: Union[Sequence[Dict], Sequence[LogsBatchQuery]], **kwargs: Any
     ) -> List[Union[LogsQueryResult, LogsQueryError, LogsQueryPartialResult]]:
         """Execute a list of Kusto queries. Each request can be either a LogsBatchQuery
         object or an equivalent serialized model.
 
         **NOTE**: The response is returned in the same order as that of the requests sent.
 
         :param queries: The list of Kusto queries to execute.
@@ -175,30 +164,100 @@
             :dedent: 0
             :caption: Get a response for multiple Log Queries.
         """
         try:
             queries = [LogsBatchQuery(**cast(Dict, q)) for q in queries]
         except (KeyError, TypeError):
             pass
-        queries = [
-            cast(LogsBatchQuery, q)._to_generated() for q in queries # pylint: disable=protected-access
-        ]
+        queries = [cast(LogsBatchQuery, q)._to_generated() for q in queries]  # pylint: disable=protected-access
         request_order = [req["id"] for req in queries]
         batch = {"requests": queries}
         generated = self._query_op.batch(batch, **kwargs)
         mapping = {item["id"]: item for item in generated["responses"]}
         return order_results(
             request_order,
             mapping,
             obj=LogsQueryResult,
             err=LogsQueryError,
             partial_err=LogsQueryPartialResult,
             raise_with=LogsQueryError,
         )
 
+    @distributed_trace
+    def query_resource(
+        self,
+        resource_id: str,
+        query: str,
+        *,
+        timespan: Optional[Union[timedelta, Tuple[datetime, timedelta], Tuple[datetime, datetime]]],
+        **kwargs: Any,
+    ) -> Union[LogsQueryResult, LogsQueryPartialResult]:
+        """Execute a Kusto query on a resource.
+
+        Returns all the Azure Monitor logs matching the given Kusto query for an Azure resource.
+
+        :param resource_id: The identifier of the resource. The expected format is
+         '/subscriptions/<sid>/resourceGroups/<rg>/providers/<providerName>/<resourceType>/<resourceName>'.
+        :type resource_id: str
+        :param query: The Kusto query. Learn more about the `Kusto query syntax
+         <https://docs.microsoft.com/azure/data-explorer/kusto/query/>`_.
+        :type query: str
+        :keyword timespan: Required. The timespan for which to query the data. This can be a timedelta,
+         a timedelta and a start datetime, or a start datetime/end datetime. Set to None to not constrain
+         the query to a timespan.
+        :paramtype timespan: ~datetime.timedelta or tuple[~datetime.datetime, ~datetime.timedelta]
+         or tuple[~datetime.datetime, ~datetime.datetime] or None
+        :keyword int server_timeout: the server timeout in seconds. The default timeout is 3 minutes,
+         and the maximum timeout is 10 minutes.
+        :keyword bool include_statistics: To get information about query statistics.
+        :keyword bool include_visualization: In the query language, it is possible to specify different
+         visualization options. By default, the API does not return information regarding the type of
+         visualization to show. If your client requires this information, specify the preference.
+        :keyword additional_workspaces: A list of workspaces that are included in the query.
+         These can be qualified workspace names, workspace IDs, or Azure resource IDs.
+        :paramtype additional_workspaces: Optional[list[str]]
+        :return: LogsQueryResult if there is a success or LogsQueryPartialResult when there is a partial success.
+        :rtype: Union[~azure.monitor.query.LogsQueryResult, ~azure.monitor.query.LogsQueryPartialResult]
+        :raises: ~azure.core.exceptions.HttpResponseError
+
+        .. admonition:: Example:
+
+        .. literalinclude:: ../samples/sample_resource_logs_query.py
+            :start-after: [START resource_logs_query]
+            :end-before: [END resource_logs_query]
+            :language: python
+            :dedent: 0
+            :caption: Get a response for a single query on a resource's logs.
+        """
+        timespan_iso = construct_iso8601(timespan)
+        include_statistics = kwargs.pop("include_statistics", False)
+        include_visualization = kwargs.pop("include_visualization", False)
+        server_timeout = kwargs.pop("server_timeout", None)
+        additional_workspaces = kwargs.pop("additional_workspaces", None)
+
+        prefer = process_prefer(server_timeout, include_statistics, include_visualization)
+
+        body = {"query": query, "timespan": timespan_iso, "workspaces": additional_workspaces}
+
+        try:
+            generated_response = self._query_op.resource_execute(  # pylint: disable=protected-access
+                resource_id=resource_id, body=body, prefer=prefer, **kwargs
+            )
+        except HttpResponseError as err:
+            process_error(err, LogsQueryError)
+
+        response: Union[LogsQueryResult, LogsQueryPartialResult]
+        if not generated_response.get("error"):
+            response = LogsQueryResult._from_generated(generated_response)  # pylint: disable=protected-access
+        else:
+            response = LogsQueryPartialResult._from_generated(  # pylint: disable=protected-access
+                generated_response, LogsQueryError
+            )
+        return response
+
     def close(self) -> None:
         """Close the :class:`~azure.monitor.query.LogsQueryClient` session."""
         return self._client.close()
 
     def __enter__(self) -> "LogsQueryClient":
         self._client.__enter__()  # pylint:disable=no-member
         return self
```

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/__init__.py` & `azure-monitor-query-1.2.0/azure/monitor/query/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_exceptions.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_exceptions.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/_client.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     :paramtype endpoint: str
     """
 
     def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
         self, *, endpoint: str = "https://api.loganalytics.io/v1", **kwargs: Any
     ) -> None:
         self._config = MonitorQueryClientConfiguration(**kwargs)
-        self._client = PipelineClient(base_url=endpoint, config=self._config, **kwargs)
+        self._client: PipelineClient = PipelineClient(base_url=endpoint, config=self._config, **kwargs)
 
         self._serialize = Serializer()
         self._deserialize = Deserializer()
         self._serialize.client_side_validation = False
         self.query = QueryOperations(self._client, self._config, self._serialize, self._deserialize)
         self.metadata = MetadataOperations(self._client, self._config, self._serialize, self._deserialize)
 
@@ -65,9 +65,9 @@
     def close(self) -> None:
         self._client.close()
 
     def __enter__(self) -> "MonitorQueryClient":
         self._client.__enter__()
         return self
 
-    def __exit__(self, *exc_details) -> None:
+    def __exit__(self, *exc_details: Any) -> None:
         self._client.__exit__(*exc_details)
```

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/_serialization.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/_serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 except ImportError:
     from urllib.parse import quote
 import xml.etree.ElementTree as ET
 
 import isodate  # type: ignore
 
 from azure.core.exceptions import DeserializationError, SerializationError, raise_with_traceback
+from azure.core.serialization import NULL as AzureCoreNull
 
 _BOM = codecs.BOM_UTF8.decode(encoding="utf-8")
 
 ModelType = TypeVar("ModelType", bound="Model")
 JSON = MutableMapping[str, Any]
 
 
@@ -624,15 +625,15 @@
                         xml_desc = attr_desc.get("xml", {})
                         xml_name = xml_desc.get("name", attr_desc["key"])
                         xml_prefix = xml_desc.get("prefix", None)
                         xml_ns = xml_desc.get("ns", None)
                         if xml_desc.get("attr", False):
                             if xml_ns:
                                 ET.register_namespace(xml_prefix, xml_ns)
-                                xml_name = "{}{}".format(xml_ns, xml_name)
+                                xml_name = "{{{}}}{}".format(xml_ns, xml_name)
                             serialized.set(xml_name, new_attr)  # type: ignore
                             continue
                         if xml_desc.get("text", False):
                             serialized.text = new_attr  # type: ignore
                             continue
                         if isinstance(new_attr, list):
                             serialized.extend(new_attr)  # type: ignore
@@ -798,14 +799,16 @@
         :raises: ValueError if data is None
         :raises: SerializationError if serialization fails.
         """
         if data is None:
             raise ValueError("No value for given attribute")
 
         try:
+            if data is AzureCoreNull:
+                return None
             if data_type in self.basic_types.values():
                 return self.serialize_basic(data, data_type, **kwargs)
 
             elif data_type in self.serialize_type:
                 return self.serialize_type[data_type](data, **kwargs)
 
             # If dependencies is empty, try with current data class
@@ -1264,15 +1267,15 @@
     :rtype: tuple
     :returns: A tuple XML name + namespace dict
     """
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
     xml_name = internal_type_xml_map.get("name", internal_type.__name__)
     xml_ns = internal_type_xml_map.get("ns", None)
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
     return xml_name
 
 
 def xml_key_extractor(attr, attr_desc, data):
     if isinstance(data, dict):
         return None
 
@@ -1288,15 +1291,15 @@
     is_wrapped = xml_desc.get("wrapped", False)
     internal_type = attr_desc.get("internalType", None)
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
 
     # Integrate namespace if necessary
     xml_ns = xml_desc.get("ns", internal_type_xml_map.get("ns", None))
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
 
     # If it's an attribute, that's simple
     if xml_desc.get("attr", False):
         return data.get(xml_name)
 
     # If it's x-ms-text, that's simple too
     if xml_desc.get("text", False):
```

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/_vendor.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/_configuration.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Note that all parameters used to create this instance are saved as instance
     attributes.
     """
 
     def __init__(self, **kwargs: Any) -> None:
         super(MonitorQueryClientConfiguration, self).__init__(**kwargs)
 
-        kwargs.setdefault("sdk_moniker", "monitorqueryclient/{}".format(VERSION))
+        kwargs.setdefault("sdk_moniker", "monitor-query/{}".format(VERSION))
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
```

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/__init__.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/_patch.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/operations/_operations.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/operations/_operations.py`

 * *Files 26% similar despite different names*

```diff
@@ -86,14 +86,67 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
+def build_query_resource_get_request(
+    resource_id: str, *, query: str, timespan: Optional[datetime.timedelta] = None, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/{resourceId}/query"
+    path_format_arguments = {
+        "resourceId": _SERIALIZER.url("resource_id", resource_id, "str", skip_quote=True),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["query"] = _SERIALIZER.query("query", query, "str")
+    if timespan is not None:
+        _params["timespan"] = _SERIALIZER.query("timespan", timespan, "duration")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_query_resource_execute_request(
+    resource_id: str, *, prefer: Optional[str] = None, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/{resourceId}/query"
+    path_format_arguments = {
+        "resourceId": _SERIALIZER.url("resource_id", resource_id, "str", skip_quote=True),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if prefer is not None:
+        _headers["Prefer"] = _SERIALIZER.header("prefer", prefer, "str")
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
 def build_query_batch_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
@@ -103,14 +156,67 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
+def build_query_resource_get_xms_request(
+    resource_id: str, *, query: str, timespan: Optional[datetime.timedelta] = None, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/{resourceId}/query"
+    path_format_arguments = {
+        "resourceId": _SERIALIZER.url("resource_id", resource_id, "str", skip_quote=True),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["query"] = _SERIALIZER.query("query", query, "str")
+    if timespan is not None:
+        _params["timespan"] = _SERIALIZER.query("timespan", timespan, "duration")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_query_resource_execute_xms_request(
+    resource_id: str, *, prefer: Optional[str] = None, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/{resourceId}/query"
+    path_format_arguments = {
+        "resourceId": _SERIALIZER.url("resource_id", resource_id, "str", skip_quote=True),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if prefer is not None:
+        _headers["Prefer"] = _SERIALIZER.header("prefer", prefer, "str")
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
 def build_metadata_get_request(workspace_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/workspaces/{workspaceId}/metadata"
@@ -253,16 +359,17 @@
             query=query,
             timespan=timespan,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
@@ -466,29 +573,41 @@
         an Analytics query.
 
         :param workspace_id: ID of the workspace. This is Workspace ID from the Properties blade in the
          Azure portal. Required.
         :type workspace_id: str
         :param body: The Analytics query. Learn more about the `Analytics query syntax
          <https://azure.microsoft.com/documentation/articles/app-insights-analytics-reference/>`_. Is
-         either a model type or a IO type. Required.
+         either a JSON type or a IO type. Required.
         :type body: JSON or IO
         :keyword prefer: Optional. The prefer header to set server timeout, query statistics and
          visualization information. Default value is None.
         :paramtype prefer: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "query": "str",  # The query to execute. Required.
+                    "timespan": "str",  # Optional. Optional. The timespan over which to query
+                      data. This is an ISO8601 time period value.  This timespan is applied in addition
+                      to any that are specified in the query expression.
+                    "workspaces": [
+                        "str"  # Optional. A list of workspaces that are included in the
+                          query.
+                    ]
+                }
+
                 # response body for status code(s): 200
                 response == {
                     "tables": [
                         {
                             "columns": [
                                 {
                                     "name": "str",  # The name of this column.
@@ -561,16 +680,454 @@
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})
+
+        return cast(JSON, deserialized)
+
+    @distributed_trace
+    def resource_get(
+        self, resource_id: str, *, query: str, timespan: Optional[datetime.timedelta] = None, **kwargs: Any
+    ) -> JSON:
+        """Execute an Analytics query using resource URI.
+
+        Executes an Analytics query for data in the context of a resource. `Here
+        <https://docs.microsoft.com/azure/azure-monitor/logs/api/azure-resource-queries>`_ is an
+        example for using POST with an Analytics query.
+
+        :param resource_id: The identifier of the resource. Required.
+        :type resource_id: str
+        :keyword query: The Analytics query. Learn more about the `Analytics query syntax
+         <https://azure.microsoft.com/documentation/articles/app-insights-analytics-reference/>`_.
+         Required.
+        :paramtype query: str
+        :keyword timespan: Optional. The timespan over which to query data. This is an ISO8601 time
+         period value.  This timespan is applied in addition to any that are specified in the query
+         expression. Default value is None.
+        :paramtype timespan: ~datetime.timedelta
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "tables": [
+                        {
+                            "columns": [
+                                {
+                                    "name": "str",  # The name of this column.
+                                      Required.
+                                    "type": "str"  # The data type of this
+                                      column. Required. Known values are: "bool", "datetime",
+                                      "dynamic", "int", "long", "real", "string", "guid", "decimal",
+                                      and "timespan".
+                                }
+                            ],
+                            "name": "str",  # The name of the table. Required.
+                            "rows": [
+                                [
+                                    {}  # The resulting rows from this query.
+                                      Required.
+                                ]
+                            ]
+                        }
+                    ],
+                    "error": {
+                        "code": "str",  # A machine readable error code. Required.
+                        "message": "str",  # A human readable error message. Required.
+                        "details": [
+                            {
+                                "code": "str",  # The error's code. Required.
+                                "message": "str",  # A human readable error message.
+                                  Required.
+                                "resources": [
+                                    "str"  # Optional. Indicates resources which
+                                      were responsible for the error.
+                                ],
+                                "target": "str",  # Optional. Indicates which
+                                  property in the request is responsible for the error.
+                                "value": "str"  # Optional. Indicates which value in
+                                  'target' is responsible for the error.
+                            }
+                        ],
+                        "innererror": ...
+                    },
+                    "render": {},  # Optional. Visualization data in JSON format.
+                    "statistics": {}  # Optional. Statistics represented in JSON format.
+                }
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        request = build_query_resource_get_request(
+            resource_id=resource_id,
+            query=query,
+            timespan=timespan,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})
+
+        return cast(JSON, deserialized)
+
+    @overload
+    def resource_execute(
+        self,
+        resource_id: str,
+        body: JSON,
+        *,
+        prefer: Optional[str] = None,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> JSON:
+        """Execute an Analytics query using resource ID.
+
+        Executes an Analytics query for data in the context of a resource. `Here
+        <https://docs.microsoft.com/azure/azure-monitor/logs/api/azure-resource-queries>`_ is an
+        example for using POST with an Analytics query.
+
+        :param resource_id: The identifier of the resource. Required.
+        :type resource_id: str
+        :param body: The Analytics query. Learn more about the `Analytics query syntax
+         <https://azure.microsoft.com/documentation/articles/app-insights-analytics-reference/>`_.
+         Required.
+        :type body: JSON
+        :keyword prefer: Optional. The prefer header to set server timeout, query statistics and
+         visualization information. Default value is None.
+        :paramtype prefer: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "query": "str",  # The query to execute. Required.
+                    "timespan": "str",  # Optional. Optional. The timespan over which to query
+                      data. This is an ISO8601 time period value.  This timespan is applied in addition
+                      to any that are specified in the query expression.
+                    "workspaces": [
+                        "str"  # Optional. A list of workspaces that are included in the
+                          query.
+                    ]
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "tables": [
+                        {
+                            "columns": [
+                                {
+                                    "name": "str",  # The name of this column.
+                                      Required.
+                                    "type": "str"  # The data type of this
+                                      column. Required. Known values are: "bool", "datetime",
+                                      "dynamic", "int", "long", "real", "string", "guid", "decimal",
+                                      and "timespan".
+                                }
+                            ],
+                            "name": "str",  # The name of the table. Required.
+                            "rows": [
+                                [
+                                    {}  # The resulting rows from this query.
+                                      Required.
+                                ]
+                            ]
+                        }
+                    ],
+                    "error": {
+                        "code": "str",  # A machine readable error code. Required.
+                        "message": "str",  # A human readable error message. Required.
+                        "details": [
+                            {
+                                "code": "str",  # The error's code. Required.
+                                "message": "str",  # A human readable error message.
+                                  Required.
+                                "resources": [
+                                    "str"  # Optional. Indicates resources which
+                                      were responsible for the error.
+                                ],
+                                "target": "str",  # Optional. Indicates which
+                                  property in the request is responsible for the error.
+                                "value": "str"  # Optional. Indicates which value in
+                                  'target' is responsible for the error.
+                            }
+                        ],
+                        "innererror": ...
+                    },
+                    "render": {},  # Optional. Visualization data in JSON format.
+                    "statistics": {}  # Optional. Statistics represented in JSON format.
+                }
+        """
+
+    @overload
+    def resource_execute(
+        self,
+        resource_id: str,
+        body: IO,
+        *,
+        prefer: Optional[str] = None,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> JSON:
+        """Execute an Analytics query using resource ID.
+
+        Executes an Analytics query for data in the context of a resource. `Here
+        <https://docs.microsoft.com/azure/azure-monitor/logs/api/azure-resource-queries>`_ is an
+        example for using POST with an Analytics query.
+
+        :param resource_id: The identifier of the resource. Required.
+        :type resource_id: str
+        :param body: The Analytics query. Learn more about the `Analytics query syntax
+         <https://azure.microsoft.com/documentation/articles/app-insights-analytics-reference/>`_.
+         Required.
+        :type body: IO
+        :keyword prefer: Optional. The prefer header to set server timeout, query statistics and
+         visualization information. Default value is None.
+        :paramtype prefer: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "tables": [
+                        {
+                            "columns": [
+                                {
+                                    "name": "str",  # The name of this column.
+                                      Required.
+                                    "type": "str"  # The data type of this
+                                      column. Required. Known values are: "bool", "datetime",
+                                      "dynamic", "int", "long", "real", "string", "guid", "decimal",
+                                      and "timespan".
+                                }
+                            ],
+                            "name": "str",  # The name of the table. Required.
+                            "rows": [
+                                [
+                                    {}  # The resulting rows from this query.
+                                      Required.
+                                ]
+                            ]
+                        }
+                    ],
+                    "error": {
+                        "code": "str",  # A machine readable error code. Required.
+                        "message": "str",  # A human readable error message. Required.
+                        "details": [
+                            {
+                                "code": "str",  # The error's code. Required.
+                                "message": "str",  # A human readable error message.
+                                  Required.
+                                "resources": [
+                                    "str"  # Optional. Indicates resources which
+                                      were responsible for the error.
+                                ],
+                                "target": "str",  # Optional. Indicates which
+                                  property in the request is responsible for the error.
+                                "value": "str"  # Optional. Indicates which value in
+                                  'target' is responsible for the error.
+                            }
+                        ],
+                        "innererror": ...
+                    },
+                    "render": {},  # Optional. Visualization data in JSON format.
+                    "statistics": {}  # Optional. Statistics represented in JSON format.
+                }
+        """
+
+    @distributed_trace
+    def resource_execute(
+        self, resource_id: str, body: Union[JSON, IO], *, prefer: Optional[str] = None, **kwargs: Any
+    ) -> JSON:
+        """Execute an Analytics query using resource ID.
+
+        Executes an Analytics query for data in the context of a resource. `Here
+        <https://docs.microsoft.com/azure/azure-monitor/logs/api/azure-resource-queries>`_ is an
+        example for using POST with an Analytics query.
+
+        :param resource_id: The identifier of the resource. Required.
+        :type resource_id: str
+        :param body: The Analytics query. Learn more about the `Analytics query syntax
+         <https://azure.microsoft.com/documentation/articles/app-insights-analytics-reference/>`_. Is
+         either a JSON type or a IO type. Required.
+        :type body: JSON or IO
+        :keyword prefer: Optional. The prefer header to set server timeout, query statistics and
+         visualization information. Default value is None.
+        :paramtype prefer: str
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "query": "str",  # The query to execute. Required.
+                    "timespan": "str",  # Optional. Optional. The timespan over which to query
+                      data. This is an ISO8601 time period value.  This timespan is applied in addition
+                      to any that are specified in the query expression.
+                    "workspaces": [
+                        "str"  # Optional. A list of workspaces that are included in the
+                          query.
+                    ]
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "tables": [
+                        {
+                            "columns": [
+                                {
+                                    "name": "str",  # The name of this column.
+                                      Required.
+                                    "type": "str"  # The data type of this
+                                      column. Required. Known values are: "bool", "datetime",
+                                      "dynamic", "int", "long", "real", "string", "guid", "decimal",
+                                      and "timespan".
+                                }
+                            ],
+                            "name": "str",  # The name of the table. Required.
+                            "rows": [
+                                [
+                                    {}  # The resulting rows from this query.
+                                      Required.
+                                ]
+                            ]
+                        }
+                    ],
+                    "error": {
+                        "code": "str",  # A machine readable error code. Required.
+                        "message": "str",  # A human readable error message. Required.
+                        "details": [
+                            {
+                                "code": "str",  # The error's code. Required.
+                                "message": "str",  # A human readable error message.
+                                  Required.
+                                "resources": [
+                                    "str"  # Optional. Indicates resources which
+                                      were responsible for the error.
+                                ],
+                                "target": "str",  # Optional. Indicates which
+                                  property in the request is responsible for the error.
+                                "value": "str"  # Optional. Indicates which value in
+                                  'target' is responsible for the error.
+                            }
+                        ],
+                        "innererror": ...
+                    },
+                    "render": {},  # Optional. Visualization data in JSON format.
+                    "statistics": {}  # Optional. Statistics represented in JSON format.
+                }
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IO, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        request = build_query_resource_execute_request(
+            resource_id=resource_id,
+            prefer=prefer,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
@@ -623,16 +1180,18 @@
                             "id": "str",  # The error details. Required.
                             "workspace": "str",  # Workspace Id to be included in the
                               query. Required.
                             "headers": {
                                 "str": "str"  # Optional. Dictionary of
                                   :code:`<string>`.
                             },
-                            "method": "str",  # Optional. "POST"
-                            "path": "str"  # Optional. "/query"
+                            "method": "POST",  # Optional. Default value is "POST". An
+                              single request in a batch. Required.
+                            "path": "/query"  # Optional. Default value is "/query". An
+                              single request in a batch. Required.
                         }
                     ]
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "responses": [
@@ -799,26 +1358,56 @@
     def batch(self, body: Union[JSON, IO], **kwargs: Any) -> JSON:
         """Execute a batch of Analytics queries.
 
         Executes a batch of Analytics queries for data. `Here
         <https://dev.loganalytics.io/documentation/Using-the-API>`_ is an example for using POST with
         an Analytics query.
 
-        :param body: The batch request body. Is either a model type or a IO type. Required.
+        :param body: The batch request body. Is either a JSON type or a IO type. Required.
         :type body: JSON or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "requests": [
+                        {
+                            "body": {
+                                "query": "str",  # The query to execute. Required.
+                                "timespan": "str",  # Optional. Optional. The
+                                  timespan over which to query data. This is an ISO8601 time period
+                                  value.  This timespan is applied in addition to any that are
+                                  specified in the query expression.
+                                "workspaces": [
+                                    "str"  # Optional. A list of workspaces that
+                                      are included in the query.
+                                ]
+                            },
+                            "id": "str",  # The error details. Required.
+                            "workspace": "str",  # Workspace Id to be included in the
+                              query. Required.
+                            "headers": {
+                                "str": "str"  # Optional. Dictionary of
+                                  :code:`<string>`.
+                            },
+                            "method": "POST",  # Optional. Default value is "POST". An
+                              single request in a batch. Required.
+                            "path": "/query"  # Optional. Default value is "/query". An
+                              single request in a batch. Required.
+                        }
+                    ]
+                }
+
                 # response body for status code(s): 200
                 response == {
                     "responses": [
                         {
                             "body": {
                                 "error": {
                                     "code": "str",  # A machine readable error
@@ -912,16 +1501,454 @@
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})
+
+        return cast(JSON, deserialized)
+
+    @distributed_trace
+    def resource_get_xms(
+        self, resource_id: str, *, query: str, timespan: Optional[datetime.timedelta] = None, **kwargs: Any
+    ) -> JSON:
+        """Execute an Analytics query using resource URI.
+
+        Executes an Analytics query for data in the context of a resource. `Here
+        <https://docs.microsoft.com/azure/azure-monitor/logs/api/azure-resource-queries>`_ is an
+        example for using POST with an Analytics query.
+
+        :param resource_id: The identifier of the resource. Required.
+        :type resource_id: str
+        :keyword query: The Analytics query. Learn more about the `Analytics query syntax
+         <https://azure.microsoft.com/documentation/articles/app-insights-analytics-reference/>`_.
+         Required.
+        :paramtype query: str
+        :keyword timespan: Optional. The timespan over which to query data. This is an ISO8601 time
+         period value.  This timespan is applied in addition to any that are specified in the query
+         expression. Default value is None.
+        :paramtype timespan: ~datetime.timedelta
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "tables": [
+                        {
+                            "columns": [
+                                {
+                                    "name": "str",  # The name of this column.
+                                      Required.
+                                    "type": "str"  # The data type of this
+                                      column. Required. Known values are: "bool", "datetime",
+                                      "dynamic", "int", "long", "real", "string", "guid", "decimal",
+                                      and "timespan".
+                                }
+                            ],
+                            "name": "str",  # The name of the table. Required.
+                            "rows": [
+                                [
+                                    {}  # The resulting rows from this query.
+                                      Required.
+                                ]
+                            ]
+                        }
+                    ],
+                    "error": {
+                        "code": "str",  # A machine readable error code. Required.
+                        "message": "str",  # A human readable error message. Required.
+                        "details": [
+                            {
+                                "code": "str",  # The error's code. Required.
+                                "message": "str",  # A human readable error message.
+                                  Required.
+                                "resources": [
+                                    "str"  # Optional. Indicates resources which
+                                      were responsible for the error.
+                                ],
+                                "target": "str",  # Optional. Indicates which
+                                  property in the request is responsible for the error.
+                                "value": "str"  # Optional. Indicates which value in
+                                  'target' is responsible for the error.
+                            }
+                        ],
+                        "innererror": ...
+                    },
+                    "render": {},  # Optional. Visualization data in JSON format.
+                    "statistics": {}  # Optional. Statistics represented in JSON format.
+                }
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        request = build_query_resource_get_xms_request(
+            resource_id=resource_id,
+            query=query,
+            timespan=timespan,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})
+
+        return cast(JSON, deserialized)
+
+    @overload
+    def resource_execute_xms(
+        self,
+        resource_id: str,
+        body: JSON,
+        *,
+        prefer: Optional[str] = None,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> JSON:
+        """Execute an Analytics query using resource ID.
+
+        Executes an Analytics query for data in the context of a resource. `Here
+        <https://docs.microsoft.com/azure/azure-monitor/logs/api/azure-resource-queries>`_ is an
+        example for using POST with an Analytics query.
+
+        :param resource_id: The identifier of the resource. Required.
+        :type resource_id: str
+        :param body: The Analytics query. Learn more about the `Analytics query syntax
+         <https://azure.microsoft.com/documentation/articles/app-insights-analytics-reference/>`_.
+         Required.
+        :type body: JSON
+        :keyword prefer: Optional. The prefer header to set server timeout, query statistics and
+         visualization information. Default value is None.
+        :paramtype prefer: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "query": "str",  # The query to execute. Required.
+                    "timespan": "str",  # Optional. Optional. The timespan over which to query
+                      data. This is an ISO8601 time period value.  This timespan is applied in addition
+                      to any that are specified in the query expression.
+                    "workspaces": [
+                        "str"  # Optional. A list of workspaces that are included in the
+                          query.
+                    ]
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "tables": [
+                        {
+                            "columns": [
+                                {
+                                    "name": "str",  # The name of this column.
+                                      Required.
+                                    "type": "str"  # The data type of this
+                                      column. Required. Known values are: "bool", "datetime",
+                                      "dynamic", "int", "long", "real", "string", "guid", "decimal",
+                                      and "timespan".
+                                }
+                            ],
+                            "name": "str",  # The name of the table. Required.
+                            "rows": [
+                                [
+                                    {}  # The resulting rows from this query.
+                                      Required.
+                                ]
+                            ]
+                        }
+                    ],
+                    "error": {
+                        "code": "str",  # A machine readable error code. Required.
+                        "message": "str",  # A human readable error message. Required.
+                        "details": [
+                            {
+                                "code": "str",  # The error's code. Required.
+                                "message": "str",  # A human readable error message.
+                                  Required.
+                                "resources": [
+                                    "str"  # Optional. Indicates resources which
+                                      were responsible for the error.
+                                ],
+                                "target": "str",  # Optional. Indicates which
+                                  property in the request is responsible for the error.
+                                "value": "str"  # Optional. Indicates which value in
+                                  'target' is responsible for the error.
+                            }
+                        ],
+                        "innererror": ...
+                    },
+                    "render": {},  # Optional. Visualization data in JSON format.
+                    "statistics": {}  # Optional. Statistics represented in JSON format.
+                }
+        """
+
+    @overload
+    def resource_execute_xms(
+        self,
+        resource_id: str,
+        body: IO,
+        *,
+        prefer: Optional[str] = None,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> JSON:
+        """Execute an Analytics query using resource ID.
+
+        Executes an Analytics query for data in the context of a resource. `Here
+        <https://docs.microsoft.com/azure/azure-monitor/logs/api/azure-resource-queries>`_ is an
+        example for using POST with an Analytics query.
+
+        :param resource_id: The identifier of the resource. Required.
+        :type resource_id: str
+        :param body: The Analytics query. Learn more about the `Analytics query syntax
+         <https://azure.microsoft.com/documentation/articles/app-insights-analytics-reference/>`_.
+         Required.
+        :type body: IO
+        :keyword prefer: Optional. The prefer header to set server timeout, query statistics and
+         visualization information. Default value is None.
+        :paramtype prefer: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "tables": [
+                        {
+                            "columns": [
+                                {
+                                    "name": "str",  # The name of this column.
+                                      Required.
+                                    "type": "str"  # The data type of this
+                                      column. Required. Known values are: "bool", "datetime",
+                                      "dynamic", "int", "long", "real", "string", "guid", "decimal",
+                                      and "timespan".
+                                }
+                            ],
+                            "name": "str",  # The name of the table. Required.
+                            "rows": [
+                                [
+                                    {}  # The resulting rows from this query.
+                                      Required.
+                                ]
+                            ]
+                        }
+                    ],
+                    "error": {
+                        "code": "str",  # A machine readable error code. Required.
+                        "message": "str",  # A human readable error message. Required.
+                        "details": [
+                            {
+                                "code": "str",  # The error's code. Required.
+                                "message": "str",  # A human readable error message.
+                                  Required.
+                                "resources": [
+                                    "str"  # Optional. Indicates resources which
+                                      were responsible for the error.
+                                ],
+                                "target": "str",  # Optional. Indicates which
+                                  property in the request is responsible for the error.
+                                "value": "str"  # Optional. Indicates which value in
+                                  'target' is responsible for the error.
+                            }
+                        ],
+                        "innererror": ...
+                    },
+                    "render": {},  # Optional. Visualization data in JSON format.
+                    "statistics": {}  # Optional. Statistics represented in JSON format.
+                }
+        """
+
+    @distributed_trace
+    def resource_execute_xms(
+        self, resource_id: str, body: Union[JSON, IO], *, prefer: Optional[str] = None, **kwargs: Any
+    ) -> JSON:
+        """Execute an Analytics query using resource ID.
+
+        Executes an Analytics query for data in the context of a resource. `Here
+        <https://docs.microsoft.com/azure/azure-monitor/logs/api/azure-resource-queries>`_ is an
+        example for using POST with an Analytics query.
+
+        :param resource_id: The identifier of the resource. Required.
+        :type resource_id: str
+        :param body: The Analytics query. Learn more about the `Analytics query syntax
+         <https://azure.microsoft.com/documentation/articles/app-insights-analytics-reference/>`_. Is
+         either a JSON type or a IO type. Required.
+        :type body: JSON or IO
+        :keyword prefer: Optional. The prefer header to set server timeout, query statistics and
+         visualization information. Default value is None.
+        :paramtype prefer: str
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "query": "str",  # The query to execute. Required.
+                    "timespan": "str",  # Optional. Optional. The timespan over which to query
+                      data. This is an ISO8601 time period value.  This timespan is applied in addition
+                      to any that are specified in the query expression.
+                    "workspaces": [
+                        "str"  # Optional. A list of workspaces that are included in the
+                          query.
+                    ]
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "tables": [
+                        {
+                            "columns": [
+                                {
+                                    "name": "str",  # The name of this column.
+                                      Required.
+                                    "type": "str"  # The data type of this
+                                      column. Required. Known values are: "bool", "datetime",
+                                      "dynamic", "int", "long", "real", "string", "guid", "decimal",
+                                      and "timespan".
+                                }
+                            ],
+                            "name": "str",  # The name of the table. Required.
+                            "rows": [
+                                [
+                                    {}  # The resulting rows from this query.
+                                      Required.
+                                ]
+                            ]
+                        }
+                    ],
+                    "error": {
+                        "code": "str",  # A machine readable error code. Required.
+                        "message": "str",  # A human readable error message. Required.
+                        "details": [
+                            {
+                                "code": "str",  # The error's code. Required.
+                                "message": "str",  # A human readable error message.
+                                  Required.
+                                "resources": [
+                                    "str"  # Optional. Indicates resources which
+                                      were responsible for the error.
+                                ],
+                                "target": "str",  # Optional. Indicates which
+                                  property in the request is responsible for the error.
+                                "value": "str"  # Optional. Indicates which value in
+                                  'target' is responsible for the error.
+                            }
+                        ],
+                        "innererror": ...
+                    },
+                    "render": {},  # Optional. Visualization data in JSON format.
+                    "statistics": {}  # Optional. Statistics represented in JSON format.
+                }
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IO, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        request = build_query_resource_execute_xms_request(
+            resource_id=resource_id,
+            prefer=prefer,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
@@ -1328,16 +2355,17 @@
         request = build_metadata_get_request(
             workspace_id=workspace_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
@@ -1726,16 +2754,17 @@
         request = build_metadata_post_request(
             workspace_id=workspace_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
```

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/operations/__init__.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/operations/_patch.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/_client.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     :paramtype endpoint: str
     """
 
     def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
         self, *, endpoint: str = "https://api.loganalytics.io/v1", **kwargs: Any
     ) -> None:
         self._config = MonitorQueryClientConfiguration(**kwargs)
-        self._client = AsyncPipelineClient(base_url=endpoint, config=self._config, **kwargs)
+        self._client: AsyncPipelineClient = AsyncPipelineClient(base_url=endpoint, config=self._config, **kwargs)
 
         self._serialize = Serializer()
         self._deserialize = Deserializer()
         self._serialize.client_side_validation = False
         self.query = QueryOperations(self._client, self._config, self._serialize, self._deserialize)
         self.metadata = MetadataOperations(self._client, self._config, self._serialize, self._deserialize)
 
@@ -65,9 +65,9 @@
     async def close(self) -> None:
         await self._client.close()
 
     async def __aenter__(self) -> "MonitorQueryClient":
         await self._client.__aenter__()
         return self
 
-    async def __aexit__(self, *exc_details) -> None:
+    async def __aexit__(self, *exc_details: Any) -> None:
         await self._client.__aexit__(*exc_details)
```

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/_configuration.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Note that all parameters used to create this instance are saved as instance
     attributes.
     """
 
     def __init__(self, **kwargs: Any) -> None:
         super(MonitorQueryClientConfiguration, self).__init__(**kwargs)
 
-        kwargs.setdefault("sdk_moniker", "monitorqueryclient/{}".format(VERSION))
+        kwargs.setdefault("sdk_moniker", "monitor-query/{}".format(VERSION))
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
```

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/__init__.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/_patch.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/operations/_operations.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/operations/_operations.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 
 from ...operations._operations import (
     build_metadata_get_request,
     build_metadata_post_request,
     build_query_batch_request,
     build_query_execute_request,
     build_query_get_request,
+    build_query_resource_execute_request,
+    build_query_resource_execute_xms_request,
+    build_query_resource_get_request,
+    build_query_resource_get_xms_request,
 )
 
 if sys.version_info >= (3, 9):
     from collections.abc import MutableMapping
 else:
     from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 JSON = MutableMapping[str, Any]  # pylint: disable=unsubscriptable-object
@@ -149,16 +153,17 @@
             query=query,
             timespan=timespan,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
@@ -364,29 +369,41 @@
         an Analytics query.
 
         :param workspace_id: ID of the workspace. This is Workspace ID from the Properties blade in the
          Azure portal. Required.
         :type workspace_id: str
         :param body: The Analytics query. Learn more about the `Analytics query syntax
          <https://azure.microsoft.com/documentation/articles/app-insights-analytics-reference/>`_. Is
-         either a model type or a IO type. Required.
+         either a JSON type or a IO type. Required.
         :type body: JSON or IO
         :keyword prefer: Optional. The prefer header to set server timeout, query statistics and
          visualization information. Default value is None.
         :paramtype prefer: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "query": "str",  # The query to execute. Required.
+                    "timespan": "str",  # Optional. Optional. The timespan over which to query
+                      data. This is an ISO8601 time period value.  This timespan is applied in addition
+                      to any that are specified in the query expression.
+                    "workspaces": [
+                        "str"  # Optional. A list of workspaces that are included in the
+                          query.
+                    ]
+                }
+
                 # response body for status code(s): 200
                 response == {
                     "tables": [
                         {
                             "columns": [
                                 {
                                     "name": "str",  # The name of this column.
@@ -459,16 +476,454 @@
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})
+
+        return cast(JSON, deserialized)
+
+    @distributed_trace_async
+    async def resource_get(
+        self, resource_id: str, *, query: str, timespan: Optional[datetime.timedelta] = None, **kwargs: Any
+    ) -> JSON:
+        """Execute an Analytics query using resource URI.
+
+        Executes an Analytics query for data in the context of a resource. `Here
+        <https://docs.microsoft.com/azure/azure-monitor/logs/api/azure-resource-queries>`_ is an
+        example for using POST with an Analytics query.
+
+        :param resource_id: The identifier of the resource. Required.
+        :type resource_id: str
+        :keyword query: The Analytics query. Learn more about the `Analytics query syntax
+         <https://azure.microsoft.com/documentation/articles/app-insights-analytics-reference/>`_.
+         Required.
+        :paramtype query: str
+        :keyword timespan: Optional. The timespan over which to query data. This is an ISO8601 time
+         period value.  This timespan is applied in addition to any that are specified in the query
+         expression. Default value is None.
+        :paramtype timespan: ~datetime.timedelta
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "tables": [
+                        {
+                            "columns": [
+                                {
+                                    "name": "str",  # The name of this column.
+                                      Required.
+                                    "type": "str"  # The data type of this
+                                      column. Required. Known values are: "bool", "datetime",
+                                      "dynamic", "int", "long", "real", "string", "guid", "decimal",
+                                      and "timespan".
+                                }
+                            ],
+                            "name": "str",  # The name of the table. Required.
+                            "rows": [
+                                [
+                                    {}  # The resulting rows from this query.
+                                      Required.
+                                ]
+                            ]
+                        }
+                    ],
+                    "error": {
+                        "code": "str",  # A machine readable error code. Required.
+                        "message": "str",  # A human readable error message. Required.
+                        "details": [
+                            {
+                                "code": "str",  # The error's code. Required.
+                                "message": "str",  # A human readable error message.
+                                  Required.
+                                "resources": [
+                                    "str"  # Optional. Indicates resources which
+                                      were responsible for the error.
+                                ],
+                                "target": "str",  # Optional. Indicates which
+                                  property in the request is responsible for the error.
+                                "value": "str"  # Optional. Indicates which value in
+                                  'target' is responsible for the error.
+                            }
+                        ],
+                        "innererror": ...
+                    },
+                    "render": {},  # Optional. Visualization data in JSON format.
+                    "statistics": {}  # Optional. Statistics represented in JSON format.
+                }
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        request = build_query_resource_get_request(
+            resource_id=resource_id,
+            query=query,
+            timespan=timespan,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})
+
+        return cast(JSON, deserialized)
+
+    @overload
+    async def resource_execute(
+        self,
+        resource_id: str,
+        body: JSON,
+        *,
+        prefer: Optional[str] = None,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> JSON:
+        """Execute an Analytics query using resource ID.
+
+        Executes an Analytics query for data in the context of a resource. `Here
+        <https://docs.microsoft.com/azure/azure-monitor/logs/api/azure-resource-queries>`_ is an
+        example for using POST with an Analytics query.
+
+        :param resource_id: The identifier of the resource. Required.
+        :type resource_id: str
+        :param body: The Analytics query. Learn more about the `Analytics query syntax
+         <https://azure.microsoft.com/documentation/articles/app-insights-analytics-reference/>`_.
+         Required.
+        :type body: JSON
+        :keyword prefer: Optional. The prefer header to set server timeout, query statistics and
+         visualization information. Default value is None.
+        :paramtype prefer: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "query": "str",  # The query to execute. Required.
+                    "timespan": "str",  # Optional. Optional. The timespan over which to query
+                      data. This is an ISO8601 time period value.  This timespan is applied in addition
+                      to any that are specified in the query expression.
+                    "workspaces": [
+                        "str"  # Optional. A list of workspaces that are included in the
+                          query.
+                    ]
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "tables": [
+                        {
+                            "columns": [
+                                {
+                                    "name": "str",  # The name of this column.
+                                      Required.
+                                    "type": "str"  # The data type of this
+                                      column. Required. Known values are: "bool", "datetime",
+                                      "dynamic", "int", "long", "real", "string", "guid", "decimal",
+                                      and "timespan".
+                                }
+                            ],
+                            "name": "str",  # The name of the table. Required.
+                            "rows": [
+                                [
+                                    {}  # The resulting rows from this query.
+                                      Required.
+                                ]
+                            ]
+                        }
+                    ],
+                    "error": {
+                        "code": "str",  # A machine readable error code. Required.
+                        "message": "str",  # A human readable error message. Required.
+                        "details": [
+                            {
+                                "code": "str",  # The error's code. Required.
+                                "message": "str",  # A human readable error message.
+                                  Required.
+                                "resources": [
+                                    "str"  # Optional. Indicates resources which
+                                      were responsible for the error.
+                                ],
+                                "target": "str",  # Optional. Indicates which
+                                  property in the request is responsible for the error.
+                                "value": "str"  # Optional. Indicates which value in
+                                  'target' is responsible for the error.
+                            }
+                        ],
+                        "innererror": ...
+                    },
+                    "render": {},  # Optional. Visualization data in JSON format.
+                    "statistics": {}  # Optional. Statistics represented in JSON format.
+                }
+        """
+
+    @overload
+    async def resource_execute(
+        self,
+        resource_id: str,
+        body: IO,
+        *,
+        prefer: Optional[str] = None,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> JSON:
+        """Execute an Analytics query using resource ID.
+
+        Executes an Analytics query for data in the context of a resource. `Here
+        <https://docs.microsoft.com/azure/azure-monitor/logs/api/azure-resource-queries>`_ is an
+        example for using POST with an Analytics query.
+
+        :param resource_id: The identifier of the resource. Required.
+        :type resource_id: str
+        :param body: The Analytics query. Learn more about the `Analytics query syntax
+         <https://azure.microsoft.com/documentation/articles/app-insights-analytics-reference/>`_.
+         Required.
+        :type body: IO
+        :keyword prefer: Optional. The prefer header to set server timeout, query statistics and
+         visualization information. Default value is None.
+        :paramtype prefer: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "tables": [
+                        {
+                            "columns": [
+                                {
+                                    "name": "str",  # The name of this column.
+                                      Required.
+                                    "type": "str"  # The data type of this
+                                      column. Required. Known values are: "bool", "datetime",
+                                      "dynamic", "int", "long", "real", "string", "guid", "decimal",
+                                      and "timespan".
+                                }
+                            ],
+                            "name": "str",  # The name of the table. Required.
+                            "rows": [
+                                [
+                                    {}  # The resulting rows from this query.
+                                      Required.
+                                ]
+                            ]
+                        }
+                    ],
+                    "error": {
+                        "code": "str",  # A machine readable error code. Required.
+                        "message": "str",  # A human readable error message. Required.
+                        "details": [
+                            {
+                                "code": "str",  # The error's code. Required.
+                                "message": "str",  # A human readable error message.
+                                  Required.
+                                "resources": [
+                                    "str"  # Optional. Indicates resources which
+                                      were responsible for the error.
+                                ],
+                                "target": "str",  # Optional. Indicates which
+                                  property in the request is responsible for the error.
+                                "value": "str"  # Optional. Indicates which value in
+                                  'target' is responsible for the error.
+                            }
+                        ],
+                        "innererror": ...
+                    },
+                    "render": {},  # Optional. Visualization data in JSON format.
+                    "statistics": {}  # Optional. Statistics represented in JSON format.
+                }
+        """
+
+    @distributed_trace_async
+    async def resource_execute(
+        self, resource_id: str, body: Union[JSON, IO], *, prefer: Optional[str] = None, **kwargs: Any
+    ) -> JSON:
+        """Execute an Analytics query using resource ID.
+
+        Executes an Analytics query for data in the context of a resource. `Here
+        <https://docs.microsoft.com/azure/azure-monitor/logs/api/azure-resource-queries>`_ is an
+        example for using POST with an Analytics query.
+
+        :param resource_id: The identifier of the resource. Required.
+        :type resource_id: str
+        :param body: The Analytics query. Learn more about the `Analytics query syntax
+         <https://azure.microsoft.com/documentation/articles/app-insights-analytics-reference/>`_. Is
+         either a JSON type or a IO type. Required.
+        :type body: JSON or IO
+        :keyword prefer: Optional. The prefer header to set server timeout, query statistics and
+         visualization information. Default value is None.
+        :paramtype prefer: str
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "query": "str",  # The query to execute. Required.
+                    "timespan": "str",  # Optional. Optional. The timespan over which to query
+                      data. This is an ISO8601 time period value.  This timespan is applied in addition
+                      to any that are specified in the query expression.
+                    "workspaces": [
+                        "str"  # Optional. A list of workspaces that are included in the
+                          query.
+                    ]
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "tables": [
+                        {
+                            "columns": [
+                                {
+                                    "name": "str",  # The name of this column.
+                                      Required.
+                                    "type": "str"  # The data type of this
+                                      column. Required. Known values are: "bool", "datetime",
+                                      "dynamic", "int", "long", "real", "string", "guid", "decimal",
+                                      and "timespan".
+                                }
+                            ],
+                            "name": "str",  # The name of the table. Required.
+                            "rows": [
+                                [
+                                    {}  # The resulting rows from this query.
+                                      Required.
+                                ]
+                            ]
+                        }
+                    ],
+                    "error": {
+                        "code": "str",  # A machine readable error code. Required.
+                        "message": "str",  # A human readable error message. Required.
+                        "details": [
+                            {
+                                "code": "str",  # The error's code. Required.
+                                "message": "str",  # A human readable error message.
+                                  Required.
+                                "resources": [
+                                    "str"  # Optional. Indicates resources which
+                                      were responsible for the error.
+                                ],
+                                "target": "str",  # Optional. Indicates which
+                                  property in the request is responsible for the error.
+                                "value": "str"  # Optional. Indicates which value in
+                                  'target' is responsible for the error.
+                            }
+                        ],
+                        "innererror": ...
+                    },
+                    "render": {},  # Optional. Visualization data in JSON format.
+                    "statistics": {}  # Optional. Statistics represented in JSON format.
+                }
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IO, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        request = build_query_resource_execute_request(
+            resource_id=resource_id,
+            prefer=prefer,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
@@ -521,16 +976,18 @@
                             "id": "str",  # The error details. Required.
                             "workspace": "str",  # Workspace Id to be included in the
                               query. Required.
                             "headers": {
                                 "str": "str"  # Optional. Dictionary of
                                   :code:`<string>`.
                             },
-                            "method": "str",  # Optional. "POST"
-                            "path": "str"  # Optional. "/query"
+                            "method": "POST",  # Optional. Default value is "POST". An
+                              single request in a batch. Required.
+                            "path": "/query"  # Optional. Default value is "/query". An
+                              single request in a batch. Required.
                         }
                     ]
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "responses": [
@@ -697,26 +1154,56 @@
     async def batch(self, body: Union[JSON, IO], **kwargs: Any) -> JSON:
         """Execute a batch of Analytics queries.
 
         Executes a batch of Analytics queries for data. `Here
         <https://dev.loganalytics.io/documentation/Using-the-API>`_ is an example for using POST with
         an Analytics query.
 
-        :param body: The batch request body. Is either a model type or a IO type. Required.
+        :param body: The batch request body. Is either a JSON type or a IO type. Required.
         :type body: JSON or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "requests": [
+                        {
+                            "body": {
+                                "query": "str",  # The query to execute. Required.
+                                "timespan": "str",  # Optional. Optional. The
+                                  timespan over which to query data. This is an ISO8601 time period
+                                  value.  This timespan is applied in addition to any that are
+                                  specified in the query expression.
+                                "workspaces": [
+                                    "str"  # Optional. A list of workspaces that
+                                      are included in the query.
+                                ]
+                            },
+                            "id": "str",  # The error details. Required.
+                            "workspace": "str",  # Workspace Id to be included in the
+                              query. Required.
+                            "headers": {
+                                "str": "str"  # Optional. Dictionary of
+                                  :code:`<string>`.
+                            },
+                            "method": "POST",  # Optional. Default value is "POST". An
+                              single request in a batch. Required.
+                            "path": "/query"  # Optional. Default value is "/query". An
+                              single request in a batch. Required.
+                        }
+                    ]
+                }
+
                 # response body for status code(s): 200
                 response == {
                     "responses": [
                         {
                             "body": {
                                 "error": {
                                     "code": "str",  # A machine readable error
@@ -810,16 +1297,454 @@
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})
+
+        return cast(JSON, deserialized)
+
+    @distributed_trace_async
+    async def resource_get_xms(
+        self, resource_id: str, *, query: str, timespan: Optional[datetime.timedelta] = None, **kwargs: Any
+    ) -> JSON:
+        """Execute an Analytics query using resource URI.
+
+        Executes an Analytics query for data in the context of a resource. `Here
+        <https://docs.microsoft.com/azure/azure-monitor/logs/api/azure-resource-queries>`_ is an
+        example for using POST with an Analytics query.
+
+        :param resource_id: The identifier of the resource. Required.
+        :type resource_id: str
+        :keyword query: The Analytics query. Learn more about the `Analytics query syntax
+         <https://azure.microsoft.com/documentation/articles/app-insights-analytics-reference/>`_.
+         Required.
+        :paramtype query: str
+        :keyword timespan: Optional. The timespan over which to query data. This is an ISO8601 time
+         period value.  This timespan is applied in addition to any that are specified in the query
+         expression. Default value is None.
+        :paramtype timespan: ~datetime.timedelta
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "tables": [
+                        {
+                            "columns": [
+                                {
+                                    "name": "str",  # The name of this column.
+                                      Required.
+                                    "type": "str"  # The data type of this
+                                      column. Required. Known values are: "bool", "datetime",
+                                      "dynamic", "int", "long", "real", "string", "guid", "decimal",
+                                      and "timespan".
+                                }
+                            ],
+                            "name": "str",  # The name of the table. Required.
+                            "rows": [
+                                [
+                                    {}  # The resulting rows from this query.
+                                      Required.
+                                ]
+                            ]
+                        }
+                    ],
+                    "error": {
+                        "code": "str",  # A machine readable error code. Required.
+                        "message": "str",  # A human readable error message. Required.
+                        "details": [
+                            {
+                                "code": "str",  # The error's code. Required.
+                                "message": "str",  # A human readable error message.
+                                  Required.
+                                "resources": [
+                                    "str"  # Optional. Indicates resources which
+                                      were responsible for the error.
+                                ],
+                                "target": "str",  # Optional. Indicates which
+                                  property in the request is responsible for the error.
+                                "value": "str"  # Optional. Indicates which value in
+                                  'target' is responsible for the error.
+                            }
+                        ],
+                        "innererror": ...
+                    },
+                    "render": {},  # Optional. Visualization data in JSON format.
+                    "statistics": {}  # Optional. Statistics represented in JSON format.
+                }
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        request = build_query_resource_get_xms_request(
+            resource_id=resource_id,
+            query=query,
+            timespan=timespan,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})
+
+        return cast(JSON, deserialized)
+
+    @overload
+    async def resource_execute_xms(
+        self,
+        resource_id: str,
+        body: JSON,
+        *,
+        prefer: Optional[str] = None,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> JSON:
+        """Execute an Analytics query using resource ID.
+
+        Executes an Analytics query for data in the context of a resource. `Here
+        <https://docs.microsoft.com/azure/azure-monitor/logs/api/azure-resource-queries>`_ is an
+        example for using POST with an Analytics query.
+
+        :param resource_id: The identifier of the resource. Required.
+        :type resource_id: str
+        :param body: The Analytics query. Learn more about the `Analytics query syntax
+         <https://azure.microsoft.com/documentation/articles/app-insights-analytics-reference/>`_.
+         Required.
+        :type body: JSON
+        :keyword prefer: Optional. The prefer header to set server timeout, query statistics and
+         visualization information. Default value is None.
+        :paramtype prefer: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "query": "str",  # The query to execute. Required.
+                    "timespan": "str",  # Optional. Optional. The timespan over which to query
+                      data. This is an ISO8601 time period value.  This timespan is applied in addition
+                      to any that are specified in the query expression.
+                    "workspaces": [
+                        "str"  # Optional. A list of workspaces that are included in the
+                          query.
+                    ]
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "tables": [
+                        {
+                            "columns": [
+                                {
+                                    "name": "str",  # The name of this column.
+                                      Required.
+                                    "type": "str"  # The data type of this
+                                      column. Required. Known values are: "bool", "datetime",
+                                      "dynamic", "int", "long", "real", "string", "guid", "decimal",
+                                      and "timespan".
+                                }
+                            ],
+                            "name": "str",  # The name of the table. Required.
+                            "rows": [
+                                [
+                                    {}  # The resulting rows from this query.
+                                      Required.
+                                ]
+                            ]
+                        }
+                    ],
+                    "error": {
+                        "code": "str",  # A machine readable error code. Required.
+                        "message": "str",  # A human readable error message. Required.
+                        "details": [
+                            {
+                                "code": "str",  # The error's code. Required.
+                                "message": "str",  # A human readable error message.
+                                  Required.
+                                "resources": [
+                                    "str"  # Optional. Indicates resources which
+                                      were responsible for the error.
+                                ],
+                                "target": "str",  # Optional. Indicates which
+                                  property in the request is responsible for the error.
+                                "value": "str"  # Optional. Indicates which value in
+                                  'target' is responsible for the error.
+                            }
+                        ],
+                        "innererror": ...
+                    },
+                    "render": {},  # Optional. Visualization data in JSON format.
+                    "statistics": {}  # Optional. Statistics represented in JSON format.
+                }
+        """
+
+    @overload
+    async def resource_execute_xms(
+        self,
+        resource_id: str,
+        body: IO,
+        *,
+        prefer: Optional[str] = None,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> JSON:
+        """Execute an Analytics query using resource ID.
+
+        Executes an Analytics query for data in the context of a resource. `Here
+        <https://docs.microsoft.com/azure/azure-monitor/logs/api/azure-resource-queries>`_ is an
+        example for using POST with an Analytics query.
+
+        :param resource_id: The identifier of the resource. Required.
+        :type resource_id: str
+        :param body: The Analytics query. Learn more about the `Analytics query syntax
+         <https://azure.microsoft.com/documentation/articles/app-insights-analytics-reference/>`_.
+         Required.
+        :type body: IO
+        :keyword prefer: Optional. The prefer header to set server timeout, query statistics and
+         visualization information. Default value is None.
+        :paramtype prefer: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "tables": [
+                        {
+                            "columns": [
+                                {
+                                    "name": "str",  # The name of this column.
+                                      Required.
+                                    "type": "str"  # The data type of this
+                                      column. Required. Known values are: "bool", "datetime",
+                                      "dynamic", "int", "long", "real", "string", "guid", "decimal",
+                                      and "timespan".
+                                }
+                            ],
+                            "name": "str",  # The name of the table. Required.
+                            "rows": [
+                                [
+                                    {}  # The resulting rows from this query.
+                                      Required.
+                                ]
+                            ]
+                        }
+                    ],
+                    "error": {
+                        "code": "str",  # A machine readable error code. Required.
+                        "message": "str",  # A human readable error message. Required.
+                        "details": [
+                            {
+                                "code": "str",  # The error's code. Required.
+                                "message": "str",  # A human readable error message.
+                                  Required.
+                                "resources": [
+                                    "str"  # Optional. Indicates resources which
+                                      were responsible for the error.
+                                ],
+                                "target": "str",  # Optional. Indicates which
+                                  property in the request is responsible for the error.
+                                "value": "str"  # Optional. Indicates which value in
+                                  'target' is responsible for the error.
+                            }
+                        ],
+                        "innererror": ...
+                    },
+                    "render": {},  # Optional. Visualization data in JSON format.
+                    "statistics": {}  # Optional. Statistics represented in JSON format.
+                }
+        """
+
+    @distributed_trace_async
+    async def resource_execute_xms(
+        self, resource_id: str, body: Union[JSON, IO], *, prefer: Optional[str] = None, **kwargs: Any
+    ) -> JSON:
+        """Execute an Analytics query using resource ID.
+
+        Executes an Analytics query for data in the context of a resource. `Here
+        <https://docs.microsoft.com/azure/azure-monitor/logs/api/azure-resource-queries>`_ is an
+        example for using POST with an Analytics query.
+
+        :param resource_id: The identifier of the resource. Required.
+        :type resource_id: str
+        :param body: The Analytics query. Learn more about the `Analytics query syntax
+         <https://azure.microsoft.com/documentation/articles/app-insights-analytics-reference/>`_. Is
+         either a JSON type or a IO type. Required.
+        :type body: JSON or IO
+        :keyword prefer: Optional. The prefer header to set server timeout, query statistics and
+         visualization information. Default value is None.
+        :paramtype prefer: str
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "query": "str",  # The query to execute. Required.
+                    "timespan": "str",  # Optional. Optional. The timespan over which to query
+                      data. This is an ISO8601 time period value.  This timespan is applied in addition
+                      to any that are specified in the query expression.
+                    "workspaces": [
+                        "str"  # Optional. A list of workspaces that are included in the
+                          query.
+                    ]
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "tables": [
+                        {
+                            "columns": [
+                                {
+                                    "name": "str",  # The name of this column.
+                                      Required.
+                                    "type": "str"  # The data type of this
+                                      column. Required. Known values are: "bool", "datetime",
+                                      "dynamic", "int", "long", "real", "string", "guid", "decimal",
+                                      and "timespan".
+                                }
+                            ],
+                            "name": "str",  # The name of the table. Required.
+                            "rows": [
+                                [
+                                    {}  # The resulting rows from this query.
+                                      Required.
+                                ]
+                            ]
+                        }
+                    ],
+                    "error": {
+                        "code": "str",  # A machine readable error code. Required.
+                        "message": "str",  # A human readable error message. Required.
+                        "details": [
+                            {
+                                "code": "str",  # The error's code. Required.
+                                "message": "str",  # A human readable error message.
+                                  Required.
+                                "resources": [
+                                    "str"  # Optional. Indicates resources which
+                                      were responsible for the error.
+                                ],
+                                "target": "str",  # Optional. Indicates which
+                                  property in the request is responsible for the error.
+                                "value": "str"  # Optional. Indicates which value in
+                                  'target' is responsible for the error.
+                            }
+                        ],
+                        "innererror": ...
+                    },
+                    "render": {},  # Optional. Visualization data in JSON format.
+                    "statistics": {}  # Optional. Statistics represented in JSON format.
+                }
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IO, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        request = build_query_resource_execute_xms_request(
+            resource_id=resource_id,
+            prefer=prefer,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
@@ -1226,16 +2151,17 @@
         request = build_metadata_get_request(
             workspace_id=workspace_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
@@ -1624,16 +2550,17 @@
         request = build_metadata_post_request(
             workspace_id=workspace_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
```

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/operations/__init__.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/aio/operations/_patch.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/_client.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     :paramtype endpoint: str
     """
 
     def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
         self, *, endpoint: str = "https://management.azure.com", **kwargs: Any
     ) -> None:
         self._config = MonitorMetricsClientConfiguration(**kwargs)
-        self._client = PipelineClient(base_url=endpoint, config=self._config, **kwargs)
+        self._client: PipelineClient = PipelineClient(base_url=endpoint, config=self._config, **kwargs)
 
         self._serialize = Serializer()
         self._deserialize = Deserializer()
         self._serialize.client_side_validation = False
         self.metric_definitions = MetricDefinitionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
@@ -72,9 +72,9 @@
     def close(self) -> None:
         self._client.close()
 
     def __enter__(self) -> "MonitorMetricsClient":
         self._client.__enter__()
         return self
 
-    def __exit__(self, *exc_details) -> None:
+    def __exit__(self, *exc_details: Any) -> None:
         self._client.__exit__(*exc_details)
```

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/_serialization.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/_serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 except ImportError:
     from urllib.parse import quote
 import xml.etree.ElementTree as ET
 
 import isodate  # type: ignore
 
 from azure.core.exceptions import DeserializationError, SerializationError, raise_with_traceback
+from azure.core.serialization import NULL as AzureCoreNull
 
 _BOM = codecs.BOM_UTF8.decode(encoding="utf-8")
 
 ModelType = TypeVar("ModelType", bound="Model")
 JSON = MutableMapping[str, Any]
 
 
@@ -624,15 +625,15 @@
                         xml_desc = attr_desc.get("xml", {})
                         xml_name = xml_desc.get("name", attr_desc["key"])
                         xml_prefix = xml_desc.get("prefix", None)
                         xml_ns = xml_desc.get("ns", None)
                         if xml_desc.get("attr", False):
                             if xml_ns:
                                 ET.register_namespace(xml_prefix, xml_ns)
-                                xml_name = "{}{}".format(xml_ns, xml_name)
+                                xml_name = "{{{}}}{}".format(xml_ns, xml_name)
                             serialized.set(xml_name, new_attr)  # type: ignore
                             continue
                         if xml_desc.get("text", False):
                             serialized.text = new_attr  # type: ignore
                             continue
                         if isinstance(new_attr, list):
                             serialized.extend(new_attr)  # type: ignore
@@ -798,14 +799,16 @@
         :raises: ValueError if data is None
         :raises: SerializationError if serialization fails.
         """
         if data is None:
             raise ValueError("No value for given attribute")
 
         try:
+            if data is AzureCoreNull:
+                return None
             if data_type in self.basic_types.values():
                 return self.serialize_basic(data, data_type, **kwargs)
 
             elif data_type in self.serialize_type:
                 return self.serialize_type[data_type](data, **kwargs)
 
             # If dependencies is empty, try with current data class
@@ -1264,15 +1267,15 @@
     :rtype: tuple
     :returns: A tuple XML name + namespace dict
     """
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
     xml_name = internal_type_xml_map.get("name", internal_type.__name__)
     xml_ns = internal_type_xml_map.get("ns", None)
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
     return xml_name
 
 
 def xml_key_extractor(attr, attr_desc, data):
     if isinstance(data, dict):
         return None
 
@@ -1288,15 +1291,15 @@
     is_wrapped = xml_desc.get("wrapped", False)
     internal_type = attr_desc.get("internalType", None)
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
 
     # Integrate namespace if necessary
     xml_ns = xml_desc.get("ns", internal_type_xml_map.get("ns", None))
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
 
     # If it's an attribute, that's simple
     if xml_desc.get("attr", False):
         return data.get(xml_name)
 
     # If it's x-ms-text, that's simple too
     if xml_desc.get("text", False):
```

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/_vendor.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/_configuration.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,20 @@
     Note that all parameters used to create this instance are saved as instance
     attributes.
     """
 
     def __init__(self, **kwargs: Any) -> None:
         super(MonitorMetricsClientConfiguration, self).__init__(**kwargs)
 
-        kwargs.setdefault("sdk_moniker", "monitormetricsclient/{}".format(VERSION))
+        kwargs.setdefault("sdk_moniker", "monitor-query/{}".format(VERSION))
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or policies.HttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
```

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/__init__.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/_patch.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/operations/_operations.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/operations/_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,33 +28,29 @@
 from .._serialization import Serializer
 from .._vendor import _format_url_section
 
 if sys.version_info >= (3, 9):
     from collections.abc import MutableMapping
 else:
     from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 JSON = MutableMapping[str, Any]  # pylint: disable=unsubscriptable-object
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_metric_definitions_list_request(
     resource_uri: str, *, metricnamespace: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2018-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-01-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/{resourceUri}/providers/Microsoft.Insights/metricDefinitions"
     path_format_arguments = {
         "resourceUri": _SERIALIZER.url("resource_uri", resource_uri, "str", skip_quote=True),
     }
@@ -85,15 +81,15 @@
     result_type: Optional[str] = None,
     metricnamespace: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2018-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-01-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/{resourceUri}/providers/Microsoft.Insights/metrics"
     path_format_arguments = {
         "resourceUri": _SERIALIZER.url("resource_uri", resource_uri, "str", skip_quote=True),
     }
@@ -129,17 +125,15 @@
 
 def build_metric_namespaces_list_request(
     resource_uri: str, *, start_time: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2017-12-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2017-12-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2017-12-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/{resourceUri}/providers/microsoft.insights/metricNamespaces"
     path_format_arguments = {
         "resourceUri": _SERIALIZER.url("resource_uri", resource_uri, "str", skip_quote=True),
     }
@@ -236,15 +230,15 @@
                       "MilliSeconds", "ByteSeconds", "Unspecified", "Cores", "MilliCores", "NanoCores",
                       and "BitsPerSecond".
                 }
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-01-01"))
         cls: ClsType[JSON] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -275,16 +269,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response)
 
@@ -458,15 +453,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-01-01"))
         cls: ClsType[JSON] = kwargs.pop("cls", None)
 
         request = build_metrics_list_request(
             resource_uri=resource_uri,
             timespan=timespan,
             interval=interval,
             metricnames=metricnames,
@@ -478,16 +473,17 @@
             metricnamespace=metricnamespace,
             api_version=api_version,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
@@ -547,17 +543,15 @@
                     },
                     "type": "str"  # Optional. The type of the namespace.
                 }
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2017-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", "2017-12-01-preview")
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2017-12-01-preview"))
         cls: ClsType[JSON] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -588,16 +582,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response)
```

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/operations/__init__.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/operations/_patch.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/_client.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     :paramtype endpoint: str
     """
 
     def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
         self, *, endpoint: str = "https://management.azure.com", **kwargs: Any
     ) -> None:
         self._config = MonitorMetricsClientConfiguration(**kwargs)
-        self._client = AsyncPipelineClient(base_url=endpoint, config=self._config, **kwargs)
+        self._client: AsyncPipelineClient = AsyncPipelineClient(base_url=endpoint, config=self._config, **kwargs)
 
         self._serialize = Serializer()
         self._deserialize = Deserializer()
         self._serialize.client_side_validation = False
         self.metric_definitions = MetricDefinitionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
@@ -72,9 +72,9 @@
     async def close(self) -> None:
         await self._client.close()
 
     async def __aenter__(self) -> "MonitorMetricsClient":
         await self._client.__aenter__()
         return self
 
-    async def __aexit__(self, *exc_details) -> None:
+    async def __aexit__(self, *exc_details: Any) -> None:
         await self._client.__aexit__(*exc_details)
```

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/_configuration.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/_configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,20 +20,20 @@
     Note that all parameters used to create this instance are saved as instance
     attributes.
     """
 
     def __init__(self, **kwargs: Any) -> None:
         super(MonitorMetricsClientConfiguration, self).__init__(**kwargs)
 
-        kwargs.setdefault("sdk_moniker", "monitormetricsclient/{}".format(VERSION))
+        kwargs.setdefault("sdk_moniker", "monitor-query/{}".format(VERSION))
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or policies.HttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
```

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/__init__.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/_patch.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/operations/_operations.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/operations/_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,18 +32,14 @@
     build_metrics_list_request,
 )
 
 if sys.version_info >= (3, 9):
     from collections.abc import MutableMapping
 else:
     from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 JSON = MutableMapping[str, Any]  # pylint: disable=unsubscriptable-object
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class MetricDefinitionsOperations:
     """
@@ -124,15 +120,15 @@
                       "MilliSeconds", "ByteSeconds", "Unspecified", "Cores", "MilliCores", "NanoCores",
                       and "BitsPerSecond".
                 }
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-01-01"))
         cls: ClsType[JSON] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -163,16 +159,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response)
 
@@ -346,15 +343,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2018-01-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-01-01"))
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-01-01"))
         cls: ClsType[JSON] = kwargs.pop("cls", None)
 
         request = build_metrics_list_request(
             resource_uri=resource_uri,
             timespan=timespan,
             interval=interval,
             metricnames=metricnames,
@@ -366,16 +363,17 @@
             metricnamespace=metricnamespace,
             api_version=api_version,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
@@ -435,17 +433,15 @@
                     },
                     "type": "str"  # Optional. The type of the namespace.
                 }
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2017-12-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", "2017-12-01-preview")
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2017-12-01-preview"))
         cls: ClsType[JSON] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -476,16 +472,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response)
```

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/operations/__init__.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/metrics/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/_generated/metrics/aio/operations/_patch.py` & `azure-monitor-query-1.2.0/azure/monitor/query/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/aio/_logs_query_client_async.py` & `azure-monitor-query-1.2.0/azure/monitor/query/aio/_logs_query_client_async.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 from datetime import datetime, timedelta
 from typing import Any, cast, Tuple, Union, Sequence, Dict, List, Optional
+from urllib.parse import urlparse
 
 from azure.core.credentials_async import AsyncTokenCredential
 from azure.core.exceptions import HttpResponseError
 from azure.core.tracing.decorator_async import distributed_trace_async
 
 from .._generated.aio._client import MonitorQueryClient
 from .._helpers import construct_iso8601, order_results, process_error, process_prefer
 from .._models import LogsQueryResult, LogsBatchQuery, LogsQueryPartialResult
 from ._helpers_async import get_authentication_policy
 from .._exceptions import LogsQueryError
 
 
-class LogsQueryClient(object): # pylint: disable=client-accepts-api-version-keyword
+class LogsQueryClient(object):  # pylint: disable=client-accepts-api-version-keyword
     """LogsQueryClient. Use this client to collect and organize log and performance data from
     monitored resources. Data from different sources such as platform logs from Azure services,
     log and performance data from virtual machines agents, and usage and performance data from
     apps can be consolidated into a single Azure Log Analytics workspace.
 
     The various data types can be analyzed together using the
     [Kusto Query Language](https://docs.microsoft.com/azure/data-explorer/kusto/query/)
@@ -30,37 +31,38 @@
     :param credential: The credential to authenticate the client
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :keyword endpoint: The endpoint to connect to. Defaults to 'https://api.loganalytics.io/v1'.
     :paramtype endpoint: Optional[str]
     """
 
     def __init__(self, credential: AsyncTokenCredential, **kwargs: Any) -> None:
-        endpoint = kwargs.pop("endpoint", "https://api.loganalytics.io")
+        endpoint = kwargs.pop("endpoint", "https://api.loganalytics.io/v1")
         if not endpoint.startswith("https://") and not endpoint.startswith("http://"):
             endpoint = "https://" + endpoint
+        parsed_endpoint = urlparse(endpoint)
+        # Assume audience is the base URL of the endpoint, unless a value is explicitly passed in.
+        audience = kwargs.pop("audience", f"{parsed_endpoint.scheme}://{parsed_endpoint.netloc}")
         self._endpoint = endpoint
         auth_policy = kwargs.pop("authentication_policy", None)
         self._client = MonitorQueryClient(
             credential=credential,
-            authentication_policy=auth_policy or get_authentication_policy(credential, endpoint),
-            endpoint=self._endpoint.rstrip('/') + "/v1",
-            **kwargs
+            authentication_policy=auth_policy or get_authentication_policy(credential, audience),
+            endpoint=self._endpoint,
+            **kwargs,
         )
         self._query_op = self._client.query
 
     @distributed_trace_async
     async def query_workspace(
         self,
         workspace_id: str,
         query: str,
         *,
-        timespan: Optional[Union[
-            timedelta, Tuple[datetime, timedelta], Tuple[datetime, datetime]
-        ]],
-        **kwargs: Any
+        timespan: Optional[Union[timedelta, Tuple[datetime, timedelta], Tuple[datetime, datetime]]],
+        **kwargs: Any,
     ) -> Union[LogsQueryResult, LogsQueryPartialResult]:
         """Execute an Analytics query.
 
         Executes an Analytics query for data.
 
         :param workspace_id: ID of the workspace. This is Workspace ID from the Properties blade in the
          Azure portal.
@@ -74,53 +76,43 @@
         :paramtype timespan: ~datetime.timedelta or tuple[~datetime.datetime, ~datetime.timedelta]
          or tuple[~datetime.datetime, ~datetime.datetime] or None
         :keyword int server_timeout: the server timeout in seconds. The default timeout is 3 minutes,
          and the maximum timeout is 10 minutes.
         :keyword bool include_statistics: To get information about query statistics.
         :keyword bool include_visualization: In the query language, it is possible to specify different
          visualization options. By default, the API does not return information regarding the type of
-         visualization to show. If your client requires this information, specify the preference
+         visualization to show. If your client requires this information, specify the preference.
         :keyword additional_workspaces: A list of workspaces that are included in the query.
-         These can be qualified workspace names, workspace Ids, or Azure resource Ids.
+         These can be qualified workspace names, workspace IDs, or Azure resource IDs.
         :paramtype additional_workspaces: Optional[List[str]]
         :return: LogsQueryResult if there is a success or LogsQueryPartialResult when there is a partial success.
         :rtype: ~azure.monitor.query.LogsQueryResult or ~azure.monitor.query.LogsQueryPartialResult
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         timespan_iso = construct_iso8601(timespan)
         include_statistics = kwargs.pop("include_statistics", False)
         include_visualization = kwargs.pop("include_visualization", False)
         server_timeout = kwargs.pop("server_timeout", None)
         additional_workspaces = kwargs.pop("additional_workspaces", None)
 
-        prefer = process_prefer(
-            server_timeout, include_statistics, include_visualization
-        )
+        prefer = process_prefer(server_timeout, include_statistics, include_visualization)
 
-        body = {
-            "query": query,
-            "timespan": timespan_iso,
-            "workspaces": additional_workspaces
-        }
+        body = {"query": query, "timespan": timespan_iso, "workspaces": additional_workspaces}
 
         try:
-            generated_response = (
-                await self._query_op.execute(  # pylint: disable=protected-access
-                    workspace_id=workspace_id, body=body, prefer=prefer, **kwargs
-                )
+            generated_response = await self._query_op.execute(  # pylint: disable=protected-access
+                workspace_id=workspace_id, body=body, prefer=prefer, **kwargs
             )
         except HttpResponseError as err:
             process_error(err, LogsQueryError)
         response: Union[LogsQueryResult, LogsQueryPartialResult]
         if not generated_response.get("error"):
-            response = LogsQueryResult._from_generated( # pylint: disable=protected-access
-                generated_response
-            )
+            response = LogsQueryResult._from_generated(generated_response)  # pylint: disable=protected-access
         else:
-            response = LogsQueryPartialResult._from_generated( # pylint: disable=protected-access
+            response = LogsQueryPartialResult._from_generated(  # pylint: disable=protected-access
                 generated_response, LogsQueryError
             )
         return response
 
     @distributed_trace_async
     async def query_batch(
         self, queries: Union[Sequence[Dict], Sequence[LogsBatchQuery]], **kwargs: Any
@@ -140,30 +132,104 @@
          or ~azure.monitor.query.LogsQueryError]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         try:
             queries = [LogsBatchQuery(**cast(Dict, q)) for q in queries]
         except (KeyError, TypeError):
             pass
-        queries = [
-            cast(LogsBatchQuery, q)._to_generated() for q in queries # pylint: disable=protected-access
-        ]
+        queries = [cast(LogsBatchQuery, q)._to_generated() for q in queries]  # pylint: disable=protected-access
         request_order = [req["id"] for req in queries]
         batch = {"requests": queries}
         generated = await self._query_op.batch(batch, **kwargs)
         mapping = {item["id"]: item for item in generated["responses"]}
         return order_results(
             request_order,
             mapping,
             obj=LogsQueryResult,
             err=LogsQueryError,
             partial_err=LogsQueryPartialResult,
             raise_with=LogsQueryError,
         )
 
+    @distributed_trace_async
+    async def query_resource(
+        self,
+        resource_id: str,
+        query: str,
+        *,
+        timespan: Optional[Union[timedelta, Tuple[datetime, timedelta], Tuple[datetime, datetime]]],
+        **kwargs: Any,
+    ) -> Union[LogsQueryResult, LogsQueryPartialResult]:
+        """Execute a Kusto query on a resource.
+
+        Returns all the Azure Monitor logs matching the given Kusto query for an Azure resource.
+
+        :param resource_id: The identifier of the resource. The expected format is
+         '/subscriptions/<sid>/resourceGroups/<rg>/providers/<providerName>/<resourceType>/<resourceName>'.
+        :type resource_id: str
+        :param query: The Kusto query. Learn more about the `Kusto query syntax
+         <https://docs.microsoft.com/azure/data-explorer/kusto/query/>`_.
+        :type query: str
+        :keyword timespan: Required. The timespan for which to query the data. This can be a timedelta,
+         a timedelta and a start datetime, or a start datetime/end datetime. Set to None to not constrain
+         the query to a timespan.
+        :paramtype timespan: ~datetime.timedelta or tuple[~datetime.datetime, ~datetime.timedelta]
+         or tuple[~datetime.datetime, ~datetime.datetime] or None
+        :keyword int server_timeout: the server timeout in seconds. The default timeout is 3 minutes,
+         and the maximum timeout is 10 minutes.
+        :keyword bool include_statistics: To get information about query statistics.
+        :keyword bool include_visualization: In the query language, it is possible to specify different
+         visualization options. By default, the API does not return information regarding the type of
+         visualization to show. If your client requires this information, specify the preference.
+        :keyword additional_workspaces: A list of workspaces that are included in the query.
+         These can be qualified workspace names, workspace IDs, or Azure resource IDs.
+        :paramtype additional_workspaces: Optional[List[str]]
+        :return: LogsQueryResult if there is a success or LogsQueryPartialResult when there is a partial success.
+        :rtype: Union[~azure.monitor.query.LogsQueryResult, ~azure.monitor.query.LogsQueryPartialResult]
+        :raises: ~azure.core.exceptions.HttpResponseError
+
+        .. admonition:: Example:
+
+        .. literalinclude:: ../samples/async_samples/sample_resource_logs_query_async.py
+            :start-after: [START resource_logs_query_async]
+            :end-before: [END resource_logs_query_async]
+            :language: python
+            :dedent: 0
+            :caption: Get a response for a single query on a resource's logs.
+        """
+        timespan_iso = construct_iso8601(timespan)
+        include_statistics = kwargs.pop("include_statistics", False)
+        include_visualization = kwargs.pop("include_visualization", False)
+        server_timeout = kwargs.pop("server_timeout", None)
+        additional_workspaces = kwargs.pop("additional_workspaces", None)
+
+        prefer = process_prefer(server_timeout, include_statistics, include_visualization)
+
+        body = {
+            "query": query,
+            "timespan": timespan_iso,
+            "additional_workspaces": additional_workspaces,
+        }
+
+        try:
+            generated_response = await self._query_op.resource_execute(  # pylint: disable=protected-access
+                resource_id=resource_id, body=body, prefer=prefer, **kwargs
+            )
+        except HttpResponseError as err:
+            process_error(err, LogsQueryError)
+
+        response: Union[LogsQueryResult, LogsQueryPartialResult]
+        if not generated_response.get("error"):
+            response = LogsQueryResult._from_generated(generated_response)  # pylint: disable=protected-access
+        else:
+            response = LogsQueryPartialResult._from_generated(  # pylint: disable=protected-access
+                generated_response, LogsQueryError
+            )
+        return response
+
     async def __aenter__(self) -> "LogsQueryClient":
         await self._client.__aenter__()
         return self
 
     async def __aexit__(self, *args: Any) -> None:
         await self._client.__aexit__(*args)
```

## Comparing `azure-monitor-query-1.1.1/azure/monitor/query/aio/_metrics_query_client_async.py` & `azure-monitor-query-1.2.0/azure/monitor/query/aio/_metrics_query_client_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,48 +12,46 @@
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.tracing.decorator_async import distributed_trace_async
 
 from .._generated._serialization import Serializer
 from .._generated.metrics.aio._client import MonitorMetricsClient
 
 from .._models import MetricsQueryResult, MetricDefinition, MetricNamespace
-from ._helpers_async import get_metrics_authentication_policy
+from ._helpers_async import get_authentication_policy
 from .._helpers import construct_iso8601
 
 
-class MetricsQueryClient(object): # pylint: disable=client-accepts-api-version-keyword
+class MetricsQueryClient(object):  # pylint: disable=client-accepts-api-version-keyword
     """MetricsQueryClient
 
     :param credential: The credential to authenticate the client
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :keyword endpoint: The endpoint to connect to. Defaults to 'https://management.azure.com'.
     :paramtype endpoint: Optional[str]
     """
 
     def __init__(self, credential: AsyncTokenCredential, **kwargs: Any) -> None:
-        audience = kwargs.pop("audience", None)
         endpoint = kwargs.pop("endpoint", "https://management.azure.com")
+        audience = kwargs.pop("audience", endpoint)
         if not endpoint.startswith("https://") and not endpoint.startswith("http://"):
             endpoint = "https://" + endpoint
         self._endpoint = endpoint
         auth_policy = kwargs.pop("authentication_policy", None)
         self._client = MonitorMetricsClient(
             credential=credential,
             endpoint=self._endpoint,
-            authentication_policy=auth_policy or get_metrics_authentication_policy(credential, audience),
+            authentication_policy=auth_policy or get_authentication_policy(credential, audience),
             **kwargs
         )
         self._metrics_op = self._client.metrics
         self._namespace_op = self._client.metric_namespaces
         self._definitions_op = self._client.metric_definitions
 
     @distributed_trace_async
-    async def query_resource(
-        self, resource_uri: str, metric_names: List[str], **kwargs: Any
-    ) -> MetricsQueryResult:
+    async def query_resource(self, resource_uri: str, metric_names: List[str], **kwargs: Any) -> MetricsQueryResult:
         """Lists the metric values for a resource.
 
         **Note**: Although the start_time, end_time, duration are optional parameters, it is highly
         recommended to specify the timespan. If not, the entire dataset is queried.
 
         :param resource_uri: The identifier of the resource.
         :type resource_uri: str
@@ -103,25 +101,19 @@
         kwargs.setdefault("top", kwargs.pop("max_results", None))
         kwargs.setdefault("interval", kwargs.pop("granularity", None))
         kwargs.setdefault("orderby", kwargs.pop("order_by", None))
         kwargs.setdefault("metricnamespace", kwargs.pop("metric_namespace", None))
         aggregations = kwargs.pop("aggregations", None)
         if aggregations:
             kwargs.setdefault("aggregation", ",".join(aggregations))
-        generated = await self._metrics_op.list(
-            resource_uri, connection_verify=False, **kwargs
-        )
-        return MetricsQueryResult._from_generated( # pylint: disable=protected-access
-            generated
-        )
+        generated = await self._metrics_op.list(resource_uri, connection_verify=False, **kwargs)
+        return MetricsQueryResult._from_generated(generated)  # pylint: disable=protected-access
 
     @distributed_trace
-    def list_metric_namespaces(
-        self, resource_uri: str, **kwargs: Any
-    ) -> AsyncItemPaged[MetricNamespace]:
+    def list_metric_namespaces(self, resource_uri: str, **kwargs: Any) -> AsyncItemPaged[MetricNamespace]:
         """Lists the metric namespaces for the resource.
 
         :param resource_uri: The identifier of the resource.
         :type resource_uri: str
         :keyword start_time: The start time from which to query for metric
          namespaces. This should be provided as a datetime object.
         :paramtype start_time: Optional[~datetime.datetime]
@@ -133,27 +125,22 @@
         if start_time:
             start_time = Serializer.serialize_iso(start_time)
         res = self._namespace_op.list(
             resource_uri,
             start_time=start_time,
             cls=kwargs.pop(
                 "cls",
-                lambda objs: [
-                    MetricNamespace._from_generated(x) # pylint: disable=protected-access
-                    for x in objs
-                ],
+                lambda objs: [MetricNamespace._from_generated(x) for x in objs],  # pylint: disable=protected-access
             ),
             **kwargs
         )
         return cast(AsyncItemPaged[MetricNamespace], res)
 
     @distributed_trace
-    def list_metric_definitions(
-        self, resource_uri: str, **kwargs: Any
-    ) -> AsyncItemPaged[MetricDefinition]:
+    def list_metric_definitions(self, resource_uri: str, **kwargs: Any) -> AsyncItemPaged[MetricDefinition]:
         """Lists the metric definitions for the resource.
 
         :param resource_uri: The identifier of the resource.
         :type resource_uri: str
         :keyword namespace: Metric namespace to query metric definitions for.
         :paramtype namespace: Optional[str]
         :return: An iterator like instance of either MetricDefinition or the result of cls(response)
@@ -162,18 +149,15 @@
         """
         metric_namespace = kwargs.pop("namespace", None)
         res = self._definitions_op.list(
             resource_uri,
             metricnamespace=metric_namespace,
             cls=kwargs.pop(
                 "cls",
-                lambda objs: [
-                    MetricDefinition._from_generated(x) # pylint: disable=protected-access
-                    for x in objs
-                ],
+                lambda objs: [MetricDefinition._from_generated(x) for x in objs],  # pylint: disable=protected-access
             ),
             **kwargs
         )
         return cast(AsyncItemPaged[MetricDefinition], res)
 
     async def __aenter__(self) -> "MetricsQueryClient":
         await self._client.__aenter__()
```

## Comparing `azure-monitor-query-1.1.1/azure_monitor_query.egg-info/PKG-INFO` & `azure-monitor-query-1.2.0/azure_monitor_query.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-monitor-query
-Version: 1.1.1
+Version: 1.2.0
 Summary: Microsoft Azure Monitor Query Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -26,14 +26,15 @@
 - [Logs](https://learn.microsoft.com/azure/azure-monitor/logs/data-platform-logs) - Collects and organizes log and performance data from monitored resources. Data from different sources such as platform logs from Azure services, log and performance data from virtual machines agents, and usage and performance data from apps can be consolidated into a single [Azure Log Analytics workspace](https://learn.microsoft.com/azure/azure-monitor/logs/data-platform-logs#log-analytics-and-workspaces). The various data types can be analyzed together using the [Kusto Query Language][kusto_query_language].
 - [Metrics](https://learn.microsoft.com/azure/azure-monitor/essentials/data-platform-metrics) - Collects numeric data from monitored resources into a time series database. Metrics are numerical values that are collected at regular intervals and describe some aspect of a system at a particular time. Metrics are lightweight and capable of supporting near real-time scenarios, making them useful for alerting and fast detection of issues.
 
 **Resources:**
 
 - [Source code][source]
 - [Package (PyPI)][package]
+- [Package (Conda)](https://anaconda.org/microsoft/azure-monitor-query/)
 - [API reference documentation][python-query-ref-docs]
 - [Service documentation][azure_monitor_overview]
 - [Samples][samples]
 - [Change log][changelog]
 
 ## Getting started
 
@@ -79,14 +80,25 @@
 from azure.monitor.query.aio import LogsQueryClient, MetricsQueryClient
 
 credential = DefaultAzureCredential()
 async_logs_client = LogsQueryClient(credential)
 async_metrics_client = MetricsQueryClient(credential)
 ```
 
+#### Configure clients for non-public Azure clouds
+
+By default, `LogsQueryClient` and `MetricsQueryClient` are configured to connect to the public Azure cloud. These can be configured to connect to non-public Azure clouds by passing in the correct `endpoint` argument: For example:
+
+```python
+logs_client = LogsQueryClient(credential, endpoint="https://api.loganalytics.azure.cn/v1")
+metrics_client = MetricsQueryClient(credential, endpoint="https://management.chinacloudapi.cn")
+```
+
+**Note**: Currently, `MetricsQueryClient` uses the Azure Resource Manager (ARM) endpoint for querying metrics, so you will need the corresponding management endpoint for your cloud when using this client. This is subject to change in the future.
+
 ### Execute the query
 
 For examples of Logs and Metrics queries, see the [Examples](#examples) section.
 
 ## Key concepts
 
 ### Logs query rate limits and throttling
@@ -108,26 +120,27 @@
 
 ## Examples
 
 - [Logs query](#logs-query)
   - [Specify timespan](#specify-timespan)
   - [Handle logs query response](#handle-logs-query-response)
 - [Batch logs query](#batch-logs-query)
+- [Resource logs query](#resource-logs-query)
 - [Advanced logs query scenarios](#advanced-logs-query-scenarios)
   - [Set logs query timeout](#set-logs-query-timeout)
   - [Query multiple workspaces](#query-multiple-workspaces)
   - [Include statistics](#include-statistics)
   - [Include visualization](#include-visualization)
 - [Metrics query](#metrics-query)
   - [Handle metrics query response](#handle-metrics-query-response)
   - [Example of handling response](#example-of-handling-response)
 
 ### Logs query
 
-This example shows getting a logs query. To handle the response and view it in a tabular form, the [pandas](https://pypi.org/project/pandas/) library is used. See the [samples][samples] if you choose not to use pandas.
+This example shows how to query a Log Analytics workspace. To handle the response and view it in a tabular form, the [pandas](https://pypi.org/project/pandas/) library is used. See the [samples][samples] if you choose not to use pandas.
 
 #### Specify timespan
 
 The `timespan` parameter specifies the time duration for which to query the data. This value can be one of the following:
 
 - a `timedelta`
 - a `timedelta` and a start datetime
@@ -164,44 +177,44 @@
     elif response.status == LogsQueryStatus.SUCCESS:
         data = response.tables
     for table in data:
         df = pd.DataFrame(data=table.rows, columns=table.columns)
         print(df)
 except HttpResponseError as err:
     print("something fatal happened")
-    print (err)
+    print(err)
 ```
 
 #### Handle logs query response
 
 The `query_workspace` API returns either a `LogsQueryResult` or a `LogsQueryPartialResult` object. The `batch_query` API returns a list that may contain `LogsQueryResult`, `LogsQueryPartialResult`, and `LogsQueryError` objects. Here's a hierarchy of the response:
 
 ```
 LogsQueryResult
 |---statistics
 |---visualization
 |---tables (list of `LogsTable` objects)
     |---name
     |---rows
     |---columns
-    |---column_types
+    |---columns_types
 
 LogsQueryPartialResult
 |---statistics
 |---visualization
 |---partial_error (a `LogsQueryError` object)
     |---code
     |---message
     |---details
     |---status
 |---partial_data (list of `LogsTable` objects)
     |---name
     |---rows
     |---columns
-    |---column_types
+    |---columns_types
 ```
 
 The `LogsQueryResult` directly iterates over the table as a convenience. For example, to handle a logs query response with tables and display it using pandas:
 
 ```python
 response = client.query(...)
 for table in response:
@@ -235,26 +248,26 @@
 
 credential = DefaultAzureCredential()
 client = LogsQueryClient(credential)
 requests = [
     LogsBatchQuery(
         query="AzureActivity | summarize count()",
         timespan=timedelta(hours=1),
-        workspace_id= os.environ['LOG_WORKSPACE_ID']
+        workspace_id=os.environ['LOG_WORKSPACE_ID']
     ),
     LogsBatchQuery(
         query= """bad query""",
         timespan=timedelta(days=1),
-        workspace_id= os.environ['LOG_WORKSPACE_ID']
+        workspace_id=os.environ['LOG_WORKSPACE_ID']
     ),
     LogsBatchQuery(
         query= """let Weight = 92233720368547758;
         range x from 1 to 3 step 1
         | summarize percentilesw(x, Weight * 100, 50)""",
-        workspace_id= os.environ['LOG_WORKSPACE_ID'],
+        workspace_id=os.environ['LOG_WORKSPACE_ID'],
         timespan=(datetime(2021, 6, 2, tzinfo=timezone.utc), datetime(2021, 6, 5, tzinfo=timezone.utc)), # (start, end)
         include_statistics=True
     ),
 ]
 results = client.query_batch(requests)
 
 for res in results:
@@ -271,14 +284,47 @@
         ## this will be a LogsQueryResult
         table = res.tables[0]
         df = pd.DataFrame(table.rows, columns=table.columns)
         print(df)
 
 ```
 
+### Resource logs query
+
+The following example demonstrates how to query logs directly from an Azure resource without the use of a Log Analytics workspace. Here, the `query_resource` method is used instead of `query_workspace`, and instead of a workspace ID, an Azure resource identifier is passed in (e.g. `/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}/providers/{resource-provider}/{resource-type}/{resource-name}`).
+
+```python
+import os
+import pandas as pd
+from datetime import timedelta
+from azure.monitor.query import LogsQueryClient, LogsQueryStatus
+from azure.core.exceptions import HttpResponseError
+from azure.identity import DefaultAzureCredential
+
+credential  = DefaultAzureCredential()
+client = LogsQueryClient(credential)
+
+query = """AzureActivity | take 5"""
+
+try:
+    response = client.query_resource(os.environ['LOGS_RESOURCE_ID'], query, timespan=timedelta(days=1))
+    if response.status == LogsQueryStatus.PARTIAL:
+        error = response.partial_error
+        data = response.partial_data
+        print(error)
+    elif response.status == LogsQueryStatus.SUCCESS:
+        data = response.tables
+    for table in data:
+        df = pd.DataFrame(data=table.rows, columns=table.columns)
+        print(df)
+except HttpResponseError as err:
+    print("something fatal happened")
+    print(err)
+```
+
 ### Advanced logs query scenarios
 
 #### Set logs query timeout
 
 The following example shows setting a server timeout in seconds. A gateway timeout is raised if the query takes more time than the mentioned timeout. The default is 180 seconds and can be set up to 10 minutes (600 seconds).
 
 ```python
@@ -492,27 +538,15 @@
                         metric_value.time_stamp
                     )
                 )
 ```
 
 ## Troubleshooting
 
-Enable the `azure.monitor.query` logger to collect traces from the library.
-
-### General
-
-Monitor Query client library will raise exceptions defined in [Azure Core][azure_core_exceptions].
-
-### Logging
-
-This library uses the standard [logging][python_logging] library for logging. Basic information about HTTP sessions, such as URLs and headers, is logged at the `INFO` level.
-
-### Optional configuration
-
-Optional keyword arguments can be passed in at the client and per-operation level. The `azure-core` [reference documentation][azure_core_ref_docs] describes available configurations for retries, logging, transport protocols, and more.
+See our [troubleshooting guide][troubleshooting_guide] for details on how to diagnose various failure scenarios.
 
 ## Next steps
 
 To learn more about Azure Monitor, see the [Azure Monitor service documentation][azure_monitor_overview].
 
 ### Samples
 
@@ -552,23 +586,38 @@
 [kusto_query_language]: https://learn.microsoft.com/azure/data-explorer/kusto/query/
 [package]: https://aka.ms/azsdk-python-monitor-query-pypi
 [pip]: https://pypi.org/project/pip/
 [python_logging]: https://docs.python.org/3/library/logging.html
 [python-query-ref-docs]: https://aka.ms/azsdk/python/monitor-query/docs
 [samples]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-query/samples
 [source]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-query/
+[troubleshooting_guide]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-query/TROUBLESHOOTING.md
 
 [cla]: https://cla.microsoft.com
 [code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
 [coc_faq]: https://opensource.microsoft.com/codeofconduct/faq/
 [coc_contact]: mailto:opencode@microsoft.com
 
 
 # Release History
 
+## 1.2.0 (2023-05-09)
+
+### Features Added
+
+- Add the `query_resource` method to `LogsQueryClient` to allow users to query Azure resources directly without the context of a workspace. ([#29365](https://github.com/Azure/azure-sdk-for-python/pull/29365))
+
+### Bugs Fixed
+
+- Fixed an inconsistent keyword argument name in the `LogsTable` constructor, changing `column_types` to `columns_types`. Note that this is a class that is typically only instantiated internally, and not by users. ([#29076](https://github.com/Azure/azure-sdk-for-python/pull/29076))
+
+### Other Changes
+
+- Improved client configuration logic for non-public Azure clouds where credential scope will be determined based on the configured endpoint. ([#29602](https://github.com/Azure/azure-sdk-for-python/pull/29602))
+
 ## 1.1.1 (2023-02-13)
 
 ### Bugs Fixed
 
 - Fixed a bug where the incorrect key `time_stamp` (should be `timeStamp`) was used in the creation of `MetricValue` objects (thanks @jamespic).  ([#28777](https://github.com/Azure/azure-sdk-for-python/pull/28777))
 
 ## 1.1.0 (2023-02-07)
```

## Comparing `azure-monitor-query-1.1.1/azure_monitor_query.egg-info/SOURCES.txt` & `azure-monitor-query-1.2.0/azure_monitor_query.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 TROUBLESHOOTING.md
 migration_guide.md
 migration_guide_app_insights.md
+pyproject.toml
 setup.py
 azure/__init__.py
 azure/monitor/__init__.py
 azure/monitor/query/__init__.py
 azure/monitor/query/_enums.py
 azure/monitor/query/_exceptions.py
 azure/monitor/query/_helpers.py
@@ -58,25 +59,30 @@
 azure_monitor_query.egg-info/dependency_links.txt
 azure_monitor_query.egg-info/not-zip-safe
 azure_monitor_query.egg-info/requires.txt
 azure_monitor_query.egg-info/top_level.txt
 samples/sample_batch_query.py
 samples/sample_log_query_multiple_workspaces.py
 samples/sample_logs_query_key_value_form.py
+samples/sample_logs_query_visualization.py
 samples/sample_logs_single_query.py
 samples/sample_logs_single_query_partial_result.py
 samples/sample_metric_definitions.py
 samples/sample_metric_namespaces.py
 samples/sample_metrics_query.py
+samples/sample_resource_logs_query.py
 samples/sample_server_timeout.py
 samples/sample_single_log_query_without_pandas.py
 samples/async_samples/sample_log_query_async.py
+samples/async_samples/sample_logs_query_visualization_async.py
 samples/async_samples/sample_metric_definitions_async.py
 samples/async_samples/sample_metric_namespaces_async.py
 samples/async_samples/sample_metrics_query_async.py
+samples/async_samples/sample_resource_logs_query_async.py
+tests/base_testcase.py
 tests/conftest.py
 tests/test_exceptions.py
 tests/test_exceptions_async.py
 tests/test_logs_client.py
 tests/test_logs_client_async.py
 tests/test_logs_response.py
 tests/test_logs_timespans.py
```

## Comparing `azure-monitor-query-1.1.1/tests/test_logs_timespans.py` & `azure-monitor-query-1.2.0/tests/test_logs_timespans.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,60 +7,61 @@
 import json
 
 from msrest.serialization import UTC
 import pytest
 
 from azure.monitor.query import LogsQueryClient
 from azure.monitor.query._helpers import construct_iso8601
-from devtools_testutils import AzureRecordedTestCase
 
+from base_testcase import AzureMonitorQueryLogsTestCase
 
-class TestLogsTimespans(AzureRecordedTestCase):
+
+class TestLogsTimespans(AzureMonitorQueryLogsTestCase):
 
     def test_query_no_duration(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(LogsQueryClient, self.get_credential(LogsQueryClient))
+        client = self.get_client(LogsQueryClient, self.get_credential(LogsQueryClient))
         query = """AppRequests |
         where TimeGenerated > ago(12h) |
         summarize avgRequestDuration=avg(DurationMs) by bin(TimeGenerated, 10m), _ResourceId"""
 
         def callback(request):
             dic = json.loads(request.http_request.body)
             assert dic.get('timespan') is None
         # returns LogsQueryResult
         client.query_workspace(monitor_info['workspace_id'], query, timespan=None)
 
     def test_query_start_and_end_time(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(LogsQueryClient, self.get_credential(LogsQueryClient))
+        client = self.get_client(LogsQueryClient, self.get_credential(LogsQueryClient))
         query = "AppRequests | take 5"
 
         end_time = datetime(2022, 11, 8)
         start_time = end_time - timedelta(days=3)
 
         def callback(request):
             dic = json.loads(request.http_request.body)
             assert dic.get('timespan') is not None
 
         client.query_workspace(monitor_info['workspace_id'], query, timespan=(start_time, end_time), raw_request_hook=callback)
 
     def test_query_duration_and_start_time(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(LogsQueryClient, self.get_credential(LogsQueryClient))
+        client = self.get_client(LogsQueryClient, self.get_credential(LogsQueryClient))
         query = "AppRequests | take 5"
 
         end_time = datetime(2022, 11, 8)
         start_time = end_time - timedelta(days=3)
         duration = timedelta(days=3)
 
         def callback(request):
             dic = json.loads(request.http_request.body)
             assert '/PT259200.0S' in dic.get('timespan')
 
         client.query_workspace(monitor_info['workspace_id'], query, timespan=(start_time,duration), raw_request_hook=callback)
 
     def test_query_duration_only(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(LogsQueryClient, self.get_credential(LogsQueryClient))
+        client = self.get_client(LogsQueryClient, self.get_credential(LogsQueryClient))
         query = "AppRequests | take 5"
 
         duration = timedelta(days=3)
 
         def callback(request):
             dic = json.loads(request.http_request.body)
             assert 'PT259200.0S' in dic.get('timespan')
```

## Comparing `azure-monitor-query-1.1.1/tests/test_exceptions_async.py` & `azure-monitor-query-1.2.0/tests/test_exceptions_async.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,49 +7,72 @@
 
 import pytest
 
 from azure.identity.aio import ClientSecretCredential
 from azure.core.exceptions import HttpResponseError
 from azure.monitor.query import LogsBatchQuery, LogsQueryError,LogsQueryResult, LogsQueryPartialResult
 from azure.monitor.query.aio import LogsQueryClient
-from devtools_testutils import AzureRecordedTestCase
 
+from base_testcase import AzureMonitorQueryLogsTestCase
 
-class TestQueryExceptionsAsync(AzureRecordedTestCase):
+
+class TestQueryExceptionsAsync(AzureMonitorQueryLogsTestCase):
 
     @pytest.mark.asyncio
     async def test_logs_single_query_fatal_exception(self, recorded_test):
-        client = self.create_client_from_credential(
+        client = self.get_client(
             LogsQueryClient, self.get_credential(LogsQueryClient, is_async=True))
         async with client:
             with pytest.raises(HttpResponseError):
                 await client.query_workspace('bad_workspace_id', 'AppRequests', timespan=None)
 
     @pytest.mark.asyncio
     async def test_logs_single_query_partial_exception_not_allowed(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(
+        client = self.get_client(
             LogsQueryClient, self.get_credential(LogsQueryClient, is_async=True))
         async with client:
             query = """let Weight = 92233720368547758;
             range x from 1 to 3 step 1
             | summarize percentilesw(x, Weight * 100, 50)"""
             response = await client.query_workspace(monitor_info['workspace_id'], query, timespan=timedelta(days=1))
             assert response.__class__ == LogsQueryPartialResult
             assert response.partial_error is not None
             assert response.partial_error.code == 'PartialError'
             assert response.partial_error.__class__ == LogsQueryError
 
     @pytest.mark.asyncio
+    async def test_logs_resource_query_fatal_exception(self, recorded_test):
+        client = self.get_client(
+            LogsQueryClient, self.get_credential(LogsQueryClient, is_async=True))
+        async with client:
+            with pytest.raises(HttpResponseError):
+                await client.query_resource('/bad/resource/id', 'AzureActivity', timespan=None)
+
+    @pytest.mark.asyncio
+    async def test_logs_resource_query_partial_exception(self, recorded_test, monitor_info):
+        client = self.get_client(
+            LogsQueryClient, self.get_credential(LogsQueryClient, is_async=True))
+        async with client:
+            query = """let Weight = 92233720368547758;
+            range x from 1 to 3 step 1
+            | summarize percentilesw(x, Weight * 100, 50)"""
+            response = await client.query_resource(monitor_info['metrics_resource_id'], query, timespan=timedelta(days=1))
+            assert response.__class__ == LogsQueryPartialResult
+            assert response.partial_error is not None
+            assert response.partial_error.code == 'PartialError'
+            assert response.partial_error.__class__ == LogsQueryError
+
+    @pytest.mark.asyncio
     async def test_logs_batch_query_fatal_exception(self, recorded_test, monitor_info):
         credential  = ClientSecretCredential(
             client_id = monitor_info['client_id'],
             client_secret = 'bad_secret',
             tenant_id = monitor_info['tenant_id']
         )
-        client = LogsQueryClient(credential)
+        client = self.get_client(LogsQueryClient, credential)
         async with client:
             requests = [
                 LogsBatchQuery(
                     query="AzureActivity | summarize count()",
                     timespan=timedelta(hours=1),
                     workspace_id=monitor_info['workspace_id']
                 ),
@@ -69,15 +92,15 @@
             ]
             with pytest.raises(HttpResponseError):
                 await client.query_batch(requests)
 
     @pytest.mark.live_test_only("Issues recording dynamic 'id' values in requests/responses")
     @pytest.mark.asyncio
     async def test_logs_batch_query_partial_exception_not_allowed(self, monitor_info):
-        client = self.create_client_from_credential(
+        client = self.get_client(
             LogsQueryClient, self.get_credential(LogsQueryClient, is_async=True))
         async with client:
             requests = [
                 LogsBatchQuery(
                     query="AzureActivity | summarize count()",
                     timespan=timedelta(hours=1),
                     workspace_id=monitor_info['workspace_id']
```

## Comparing `azure-monitor-query-1.1.1/tests/test_metrics_client.py` & `azure-monitor-query-1.2.0/tests/test_metrics_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,62 +3,68 @@
 # Licensed under the MIT License. See LICENSE.txt in the project root for
 # license information.
 # -------------------------------------------------------------------------
 from datetime import timedelta
 from unittest import mock
 
 from azure.monitor.query import MetricsQueryClient, MetricAggregationType, Metric
-from devtools_testutils import AzureRecordedTestCase
 
+from base_testcase import AzureMonitorQueryMetricsTestCase
 
-METRIC_NAME = "Event"
 
+METRIC_NAME = "requests/count"
+METRIC_RESOURCE_PROVIDER = "Microsoft.Insights/components"
 
-class TestMetricsClient(AzureRecordedTestCase):
+
+class TestMetricsClient(AzureMonitorQueryMetricsTestCase):
 
     def test_metrics_auth(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(MetricsQueryClient, self.get_credential(MetricsQueryClient))
+        client = self.get_client(MetricsQueryClient, self.get_credential(MetricsQueryClient))
         response = client.query_resource(
             monitor_info['metrics_resource_id'],
             metric_names=[METRIC_NAME],
             timespan=timedelta(days=1),
             aggregations=[MetricAggregationType.COUNT]
             )
         assert response
         assert response.metrics
 
     def test_metrics_granularity(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(MetricsQueryClient, self.get_credential(MetricsQueryClient))
+        client = self.get_client(MetricsQueryClient, self.get_credential(MetricsQueryClient))
         response = client.query_resource(
             monitor_info['metrics_resource_id'],
             metric_names=[METRIC_NAME],
             timespan=timedelta(days=1),
             granularity=timedelta(minutes=5),
             aggregations=[MetricAggregationType.COUNT]
             )
         assert response
         assert response.granularity == timedelta(minutes=5)
+        metric = response.metrics[METRIC_NAME]
+        assert metric.timeseries
+        for t in metric.timeseries:
+            assert t.metadata_values is not None
 
     def test_metrics_filter(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(MetricsQueryClient, self.get_credential(MetricsQueryClient))
+        client = self.get_client(MetricsQueryClient, self.get_credential(MetricsQueryClient))
         response = client.query_resource(
             monitor_info['metrics_resource_id'],
             metric_names=[METRIC_NAME],
             timespan=timedelta(days=1),
             granularity=timedelta(minutes=5),
-            filter="Source eq '*'",
+            filter="request/success eq '0'",
             aggregations=[MetricAggregationType.COUNT]
             )
         assert response
         metric = response.metrics[METRIC_NAME]
         for t in metric.timeseries:
             assert t.metadata_values is not None
 
     def test_metrics_list(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(MetricsQueryClient, self.get_credential(MetricsQueryClient))
+        client = self.get_client(MetricsQueryClient, self.get_credential(MetricsQueryClient))
         response = client.query_resource(
             monitor_info['metrics_resource_id'],
             metric_names=[METRIC_NAME],
             timespan=timedelta(days=1),
             granularity=timedelta(minutes=5),
             aggregations=[MetricAggregationType.COUNT]
             )
@@ -70,37 +76,45 @@
         assert metrics[METRIC_NAME] == metrics[0]
 
     def test_metrics_list_with_commas(self):
         """Commas in metric names should be encoded as %2."""
 
         with mock.patch("azure.monitor.query._generated.metrics.operations.MetricsOperations.list") as mock_list:
             mock_list.return_value = {"foo": "bar"}
-            client = self.create_client_from_credential(MetricsQueryClient, self.get_credential(MetricsQueryClient))
+            client = self.get_client(MetricsQueryClient, self.get_credential(MetricsQueryClient))
             client.query_resource(
                 "resource",
                 metric_names=["metric1,metric2", "foo,test,test"],
                 timespan=timedelta(days=1),
                 granularity=timedelta(minutes=5),
                 aggregations=[MetricAggregationType.COUNT]
             )
 
         assert "metricnames" in mock_list.call_args[1]
         assert mock_list.call_args[1]['metricnames'] == "metric1%2metric2,foo%2test%2test"
 
 
     def test_metrics_namespaces(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(MetricsQueryClient, self.get_credential(MetricsQueryClient))
+        client = self.get_client(MetricsQueryClient, self.get_credential(MetricsQueryClient))
 
         response = client.list_metric_namespaces(monitor_info['metrics_resource_id'])
 
         assert response is not None
         for item in response:
             assert item
 
     def test_metrics_definitions(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(MetricsQueryClient, self.get_credential(MetricsQueryClient))
+        client = self.get_client(MetricsQueryClient, self.get_credential(MetricsQueryClient))
         response = client.list_metric_definitions(
-            monitor_info['metrics_resource_id'], namespace='Microsoft.OperationalInsights/workspaces')
+            monitor_info['metrics_resource_id'], namespace=METRIC_RESOURCE_PROVIDER)
 
         assert response is not None
         for item in response:
             assert item
+
+    def test_client_different_endpoint(self):
+        credential = self.get_credential(MetricsQueryClient)
+        endpoint = "https://management.chinacloudapi.cn"
+        client = MetricsQueryClient(credential, endpoint=endpoint)
+
+        assert client._endpoint == endpoint
+        assert f"{endpoint}/.default" in client._client._config.authentication_policy._scopes
```

## Comparing `azure-monitor-query-1.1.1/tests/conftest.py` & `azure-monitor-query-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/tests/test_exceptions.py` & `azure-monitor-query-1.2.0/tests/test_exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,63 @@
 from datetime import timedelta, datetime
 
 import pytest
 
 from azure.identity import ClientSecretCredential
 from azure.core.exceptions import HttpResponseError
 from azure.monitor.query import LogsQueryClient, LogsBatchQuery, LogsQueryError, LogsQueryResult, LogsQueryPartialResult
-from devtools_testutils import AzureRecordedTestCase
 
+from base_testcase import AzureMonitorQueryLogsTestCase
 
-class TestQueryExceptions(AzureRecordedTestCase):
+
+class TestQueryExceptions(AzureMonitorQueryLogsTestCase):
 
     def test_logs_single_query_fatal_exception(self, recorded_test):
-        client = self.create_client_from_credential(LogsQueryClient, self.get_credential(LogsQueryClient))
+        client = self.get_client(LogsQueryClient, self.get_credential(LogsQueryClient))
         with pytest.raises(HttpResponseError):
             client.query_workspace('bad_workspace_id', 'AppRequests', timespan=None)
 
     def test_logs_single_query_partial_exception(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(LogsQueryClient, self.get_credential(LogsQueryClient))
+        client = self.get_client(LogsQueryClient, self.get_credential(LogsQueryClient))
         query = """let Weight = 92233720368547758;
         range x from 1 to 3 step 1
         | summarize percentilesw(x, Weight * 100, 50)"""
         response = client.query_workspace(monitor_info['workspace_id'], query, timespan=timedelta(days=1))
         assert response.__class__ == LogsQueryPartialResult
         assert response.partial_error is not None
         assert response.partial_data is not None
         assert response.partial_error.details is not None
         assert response.partial_error.code == 'PartialError'
         assert response.partial_error.__class__ == LogsQueryError
 
+    def test_logs_resource_query_fatal_exception(self, recorded_test):
+        client = self.get_client(LogsQueryClient, self.get_credential(LogsQueryClient))
+        with pytest.raises(HttpResponseError):
+            client.query_resource('/bad/resource/id', 'AzureActivity', timespan=None)
+
+    def test_logs_resource_query_partial_exception(self, recorded_test, monitor_info):
+        client = self.get_client(LogsQueryClient, self.get_credential(LogsQueryClient))
+        query = """let Weight = 92233720368547758;
+        range x from 1 to 3 step 1
+        | summarize percentilesw(x, Weight * 100, 50)"""
+        response = client.query_resource(monitor_info['metrics_resource_id'], query, timespan=timedelta(days=1))
+        assert response.__class__ == LogsQueryPartialResult
+        assert response.partial_error is not None
+        assert response.partial_data is not None
+        assert response.partial_error.details is not None
+        assert response.partial_error.code == 'PartialError'
+        assert response.partial_error.__class__ == LogsQueryError
+
     def test_logs_batch_query_fatal_exception(self, recorded_test, monitor_info):
         credential  = ClientSecretCredential(
             client_id = monitor_info['client_id'],
             client_secret = 'bad_secret',
             tenant_id = monitor_info['tenant_id']
         )
-        client = LogsQueryClient(credential)
+        client = self.get_client(LogsQueryClient, credential)
         requests = [
             LogsBatchQuery(
                 query="AzureActivity | summarize count()",
                 timespan=timedelta(hours=1),
                 workspace_id=monitor_info['workspace_id']
             ),
             LogsBatchQuery(
@@ -61,15 +80,15 @@
             ),
         ]
         with pytest.raises(HttpResponseError):
             responses = client.query_batch(requests)
 
     @pytest.mark.live_test_only("Issues recording dynamic 'id' values in requests/responses")
     def test_logs_batch_query_partial_exception(self, monitor_info):
-        client = self.create_client_from_credential(LogsQueryClient, self.get_credential(LogsQueryClient))
+        client = self.get_client(LogsQueryClient, self.get_credential(LogsQueryClient))
         requests = [
             LogsBatchQuery(
                 query="AzureActivity | summarize count()",
                 timespan=timedelta(hours=1),
                 workspace_id=monitor_info['workspace_id']
             ),
             LogsBatchQuery(
@@ -90,15 +109,15 @@
         r1, r2, r3 = responses[0], responses[1], responses[2]
         assert r1.__class__ == LogsQueryResult
         assert r2.__class__ == LogsQueryResult
         assert r3.__class__ == LogsQueryPartialResult
 
     @pytest.mark.live_test_only("Issues recording dynamic 'id' values in requests/responses")
     def test_logs_batch_query_non_fatal_exception(self, monitor_info):
-        client = self.create_client_from_credential(LogsQueryClient, self.get_credential(LogsQueryClient))
+        client = self.get_client(LogsQueryClient, self.get_credential(LogsQueryClient))
         requests = [
             LogsBatchQuery(
                 query="AzureActivity | summarize count()",
                 timespan=timedelta(hours=1),
                 workspace_id=monitor_info['workspace_id']
             ),
             LogsBatchQuery(
```

## Comparing `azure-monitor-query-1.1.1/tests/test_logs_response.py` & `azure-monitor-query-1.2.0/tests/test_logs_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See LICENSE.txt in the project root for
 # license information.
 # -------------------------------------------------------------------------
 from datetime import datetime, timezone
 
 from azure.monitor.query import LogsQueryClient
-from devtools_testutils import AzureRecordedTestCase
 
+from base_testcase import AzureMonitorQueryLogsTestCase
 
-class TestLogsResponse(AzureRecordedTestCase):
+
+class TestLogsResponse(AzureMonitorQueryLogsTestCase):
 
     def test_query_response_data(self, recorded_test, monitor_info):
         # Sample log entry that is populated in table before test.
         # {
         #    "Time": "2022-11-07T01:03:07.584426Z",
         #    "Computer": "Computer1",
         #    "AdditionalContext": '{"testContextKey": 1, "CounterName": "AppMetric1"}}'
         # }
 
-        client = self.create_client_from_credential(LogsQueryClient, self.get_credential(LogsQueryClient))
+        client = self.get_client(LogsQueryClient, self.get_credential(LogsQueryClient))
         query = (
             f"{monitor_info['table_name']} | project TimeGenerated, Type, ExtendedColumn, AdditionalContext"
             f"| order by TimeGenerated desc | take 5")
 
         # returns LogsQueryResult
         result = client.query_workspace(monitor_info['workspace_id'], query, timespan=None)
         assert isinstance(result.tables[0].rows[0][0], datetime)
@@ -35,15 +36,15 @@
         # Check if DCR transformation correctly populated the ExtendedColumn field.
         assert "AppMetric" in result.tables[0].rows[0][2]
 
         assert isinstance(result.tables[0].rows[0][3], str)
         assert "testContextKey" in result.tables[0].rows[0][3]
 
     def test_query_response_types(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(LogsQueryClient, self.get_credential(LogsQueryClient))
+        client = self.get_client(LogsQueryClient, self.get_credential(LogsQueryClient))
         query = """print "hello", true, make_datetime("2000-01-02 03:04:05Z"), toint(100), long(101), 102.1
             | project
                 stringcolumn=print_0,
                 boolcolumn=print_1,
                 datecolumn=print_2,
                 intcolumn=print_3,
                 longcolumn=print_4,
```

## Comparing `azure-monitor-query-1.1.1/tests/test_metrics_client_async.py` & `azure-monitor-query-1.2.0/tests/test_metrics_client_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,71 +7,78 @@
 import sys
 from unittest import mock
 
 import pytest
 
 from azure.monitor.query import MetricAggregationType, Metric
 from azure.monitor.query.aio import MetricsQueryClient
-from devtools_testutils import AzureRecordedTestCase
 
+from base_testcase import AzureMonitorQueryMetricsTestCase
 
-METRIC_NAME = "Event"
 
-class TestMetricsClientAsync(AzureRecordedTestCase):
+METRIC_NAME = "requests/count"
+METRIC_RESOURCE_PROVIDER = "Microsoft.Insights/components"
+
+
+class TestMetricsClientAsync(AzureMonitorQueryMetricsTestCase):
 
     @pytest.mark.asyncio
     async def test_metrics_auth(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(
+        client = self.get_client(
             MetricsQueryClient, self.get_credential(MetricsQueryClient, is_async=True))
         async with client:
             response = await client.query_resource(
                 monitor_info['metrics_resource_id'],
                 metric_names=[METRIC_NAME],
                 timespan=timedelta(days=1),
                 aggregations=[MetricAggregationType.COUNT]
                 )
             assert response
             assert response.metrics
 
     @pytest.mark.asyncio
     async def test_metrics_granularity(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(
+        client = self.get_client(
             MetricsQueryClient, self.get_credential(MetricsQueryClient, is_async=True))
         async with client:
             response = await client.query_resource(
                 monitor_info['metrics_resource_id'],
                 metric_names=[METRIC_NAME],
                 timespan=timedelta(days=1),
                 granularity=timedelta(minutes=5),
                 aggregations=[MetricAggregationType.COUNT]
                 )
             assert response
             assert response.granularity == timedelta(minutes=5)
+            metric = response.metrics[METRIC_NAME]
+            assert metric.timeseries
+            for t in metric.timeseries:
+                assert t.metadata_values is not None
 
     @pytest.mark.asyncio
     async def test_metrics_filter(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(
+        client = self.get_client(
             MetricsQueryClient, self.get_credential(MetricsQueryClient, is_async=True))
         async with client:
             response = await client.query_resource(
                 monitor_info['metrics_resource_id'],
                 metric_names=[METRIC_NAME],
                 timespan=timedelta(days=1),
                 granularity=timedelta(minutes=5),
-                filter="Source eq '*'",
+                filter="request/success eq '0'",
                 aggregations=[MetricAggregationType.COUNT]
                 )
             assert response
             metric = response.metrics[METRIC_NAME]
             for t in metric.timeseries:
                 assert t.metadata_values is not None
 
     @pytest.mark.asyncio
     async def test_metrics_list(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(
+        client = self.get_client(
             MetricsQueryClient, self.get_credential(MetricsQueryClient, is_async=True))
         async with client:
             response = await client.query_resource(
                 monitor_info['metrics_resource_id'],
                 metric_names=[METRIC_NAME],
                 timespan=timedelta(days=1),
                 granularity=timedelta(minutes=5),
@@ -87,15 +94,15 @@
     @pytest.mark.asyncio
     @pytest.mark.skipif(sys.version_info < (3, 8), reason="async mocks work differently in Python <= 3.7")
     async def test_metrics_list_with_commas(self):
         """Commas in metric names should be encoded as %2."""
 
         with mock.patch("azure.monitor.query._generated.metrics.aio.operations.MetricsOperations.list") as mock_list:
             mock_list.return_value = {"foo": "bar"}
-            client = self.create_client_from_credential(
+            client = self.get_client(
                 MetricsQueryClient, self.get_credential(MetricsQueryClient, is_async=True))
             async with client:
                 await client.query_resource(
                     "resource",
                     metric_names=["metric1,metric2", "foo,test,test"],
                     timespan=timedelta(days=1),
                     granularity=timedelta(minutes=5),
@@ -103,29 +110,38 @@
                 )
 
         assert "metricnames" in mock_list.call_args[1]
         assert mock_list.call_args[1]['metricnames'] == "metric1%2metric2,foo%2test%2test"
 
     @pytest.mark.asyncio
     async def test_metrics_namespaces(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(
+        client = self.get_client(
             MetricsQueryClient, self.get_credential(MetricsQueryClient, is_async=True))
 
         async with client:
             response = client.list_metric_namespaces(monitor_info['metrics_resource_id'])
 
             assert response is not None
             async for item in response:
                 assert item
 
     @pytest.mark.asyncio
     async def test_metrics_definitions(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(
+        client = self.get_client(
             MetricsQueryClient, self.get_credential(MetricsQueryClient, is_async=True))
 
         async with client:
             response = client.list_metric_definitions(
-                monitor_info['metrics_resource_id'], namespace='Microsoft.OperationalInsights/workspaces')
+                monitor_info['metrics_resource_id'], namespace=METRIC_RESOURCE_PROVIDER)
 
             assert response is not None
             async for item in response:
                 assert item
+
+    @pytest.mark.asyncio
+    async def test_client_different_endpoint(self):
+        credential = self.get_credential(MetricsQueryClient)
+        endpoint = "https://management.chinacloudapi.cn"
+        client = MetricsQueryClient(credential, endpoint=endpoint)
+
+        assert client._endpoint == endpoint
+        assert f"{endpoint}/.default" in client._client._config.authentication_policy._scopes
```

## Comparing `azure-monitor-query-1.1.1/tests/test_logs_client_async.py` & `azure-monitor-query-1.2.0/tests/test_logs_client_async.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,50 +6,51 @@
 from datetime import timedelta
 
 import pytest
 
 from azure.core.exceptions import HttpResponseError
 from azure.monitor.query import LogsBatchQuery, LogsQueryError, LogsTable, LogsQueryResult, LogsTableRow
 from azure.monitor.query.aio import LogsQueryClient
-from devtools_testutils import AzureRecordedTestCase
 
+from base_testcase import AzureMonitorQueryLogsTestCase
 
-class TestLogsClientAsync(AzureRecordedTestCase):
+
+class TestLogsClientAsync(AzureMonitorQueryLogsTestCase):
 
     @pytest.mark.asyncio
     async def test_logs_auth(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(
+        client = self.get_client(
             LogsQueryClient, self.get_credential(LogsQueryClient, is_async=True))
         async with client:
             query = """AppRequests |
             where TimeGenerated > ago(12h) |
             summarize avgRequestDuration=avg(DurationMs) by bin(TimeGenerated, 10m), _ResourceId"""
 
             # returns LogsQueryResult
             response = await client.query_workspace(monitor_info['workspace_id'], query, timespan=None)
 
             assert response is not None
             assert response.tables is not None
 
     @pytest.mark.asyncio
     async def test_logs_auth_no_timespan(self, monitor_info):
-        client = self.create_client_from_credential(
+        client = self.get_client(
             LogsQueryClient, self.get_credential(LogsQueryClient, is_async=True))
         async with client:
             query = """AppRequests |
             where TimeGenerated > ago(12h) |
             summarize avgRequestDuration=avg(DurationMs) by bin(TimeGenerated, 10m), _ResourceId"""
 
             # returns LogsQueryResult
             with pytest.raises(TypeError):
                 await client.query_workspace(monitor_info['workspace_id'], query)
 
     @pytest.mark.asyncio
     async def test_logs_server_timeout(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(
+        client = self.get_client(
             LogsQueryClient, self.get_credential(LogsQueryClient, is_async=True))
 
         with pytest.raises(HttpResponseError) as e:
             async with client:
                 await client.query_workspace(
                     monitor_info['workspace_id'],
                     "range x from 1 to 1000000000000000 step 1 | count",
@@ -66,15 +67,15 @@
                 workspace_id=monitor_info['workspace_id'],
                 query="AzureActivity | summarize count()",
             )
 
     @pytest.mark.live_test_only("Issues recording dynamic 'id' values in requests/responses")
     @pytest.mark.asyncio
     async def test_logs_query_batch_default(self, monitor_info):
-        client = self.create_client_from_credential(
+        client = self.get_client(
             LogsQueryClient, self.get_credential(LogsQueryClient, is_async=True))
         async with client:
             requests = [
                 LogsBatchQuery(
                     monitor_info['workspace_id'],
                     query="AzureActivity | summarize count()",
                     timespan=timedelta(hours=1)
@@ -101,15 +102,15 @@
             assert r1.tables[0].columns[1] == '_ResourceId'
             assert r1.tables[0].columns[2] == 'avgRequestDuration'
             r2 = response[2]
             assert r2.__class__ == LogsQueryError
 
     @pytest.mark.asyncio
     async def test_logs_single_query_additional_workspaces_async(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(
+        client = self.get_client(
             LogsQueryClient, self.get_credential(LogsQueryClient, is_async=True))
         async with client:
             query = (
                 f"{monitor_info['table_name']} | where TimeGenerated > ago(100d)"
                 "| project TenantId | summarize count() by TenantId"
             )
 
@@ -124,15 +125,15 @@
             assert response
             assert len(response.tables[0].rows) == 2
 
     @pytest.mark.skip("Flaky deserialization issues with msrest. Re-enable after removing msrest dependency.")
     @pytest.mark.live_test_only("Issues recording dynamic 'id' values in requests/responses")
     @pytest.mark.asyncio
     async def test_logs_query_batch_additional_workspaces(self, monitor_info):
-        client = self.create_client_from_credential(
+        client = self.get_client(
             LogsQueryClient, self.get_credential(LogsQueryClient, is_async=True))
         async with client:
             query = (
                 f"{monitor_info['table_name']} | where TimeGenerated > ago(100d)"
                 "| project TenantId | summarize count() by TenantId"
             )
             requests = [
@@ -159,41 +160,41 @@
 
             assert len(response) == 3
             for resp in response:
                 assert len(resp.tables[0].rows) == 2
 
     @pytest.mark.asyncio
     async def test_logs_single_query_with_visualization(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(
+        client = self.get_client(
             LogsQueryClient, self.get_credential(LogsQueryClient, is_async=True))
         async with client:
             query = """AppRequests | take 10"""
 
             # returns LogsQueryResult
             response = await client.query_workspace(
                 monitor_info['workspace_id'], query, timespan=None, include_visualization=True)
 
             assert response.visualization is not None
 
     @pytest.mark.asyncio
     async def test_logs_single_query_with_visualization_and_stats(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(
+        client = self.get_client(
             LogsQueryClient, self.get_credential(LogsQueryClient, is_async=True))
         async with client:
             query = """AppRequests | take 10"""
             # returns LogsQueryResult
             response = await client.query_workspace(
                 monitor_info['workspace_id'], query, timespan=None, include_visualization=True, include_statistics=True)
 
             assert response.visualization is not None
             assert response.statistics is not None
 
     @pytest.mark.asyncio
     async def test_logs_query_result_iterate_over_tables(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(
+        client = self.get_client(
             LogsQueryClient, self.get_credential(LogsQueryClient, is_async=True))
         async with client:
             query = "AppRequests | take 10; AppRequests | take 5"
             response = await client.query_workspace(
                 monitor_info['workspace_id'],
                 query,
                 timespan=None,
@@ -208,15 +209,15 @@
             assert response.statistics is not None
             assert response.visualization is not None
             assert len(response.tables) == 2
             assert response.__class__ == LogsQueryResult
 
     @pytest.mark.asyncio
     async def test_logs_query_result_row_type(self, recorded_test, monitor_info):
-        client = self.create_client_from_credential(
+        client = self.get_client(
             LogsQueryClient, self.get_credential(LogsQueryClient, is_async=True))
         async with client:
             query = "AppRequests | take 5"
             response = await client.query_workspace(
                 monitor_info['workspace_id'],
                 query,
                 timespan=None,
@@ -224,7 +225,47 @@
 
             ## should iterate over tables
             for table in response:
                 assert table.__class__ == LogsTable
 
                 for row in table.rows:
                     assert row.__class__ == LogsTableRow
+
+    @pytest.mark.asyncio
+    async def test_logs_resource_query(self, recorded_test, monitor_info):
+        client = self.get_client(
+            LogsQueryClient, self.get_credential(LogsQueryClient, is_async=True))
+        async with client:
+            query = "requests | summarize count()"
+
+            response = await client.query_resource(monitor_info['metrics_resource_id'], query, timespan=None)
+
+            assert response is not None
+            assert response.tables is not None
+            assert len(response.tables[0].rows) == 1
+
+    @pytest.mark.asyncio
+    async def test_logs_resource_query_additional_options(self, recorded_test, monitor_info):
+        client = self.get_client(
+            LogsQueryClient, self.get_credential(LogsQueryClient, is_async=True))
+        async with client:
+            query = "requests | summarize count()"
+
+            response = await client.query_resource(
+                monitor_info['metrics_resource_id'],
+                query,
+                timespan=None,
+                include_statistics=True,
+                include_visualization=True
+            )
+
+            assert response.visualization is not None
+            assert response.statistics is not None
+
+    @pytest.mark.asyncio
+    async def test_client_different_endpoint(self):
+        credential = self.get_credential(LogsQueryClient, is_async=True)
+        endpoint = "https://api.loganalytics.azure.cn/v1"
+        client = LogsQueryClient(credential, endpoint=endpoint)
+
+        assert client._endpoint == endpoint
+        assert "https://api.loganalytics.azure.cn/.default" in client._client._config.authentication_policy._scopes
```

## Comparing `azure-monitor-query-1.1.1/tests/perfstress_tests/single_query.py` & `azure-monitor-query-1.2.0/tests/perfstress_tests/single_query.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/tests/perfstress_tests/batch_query.py` & `azure-monitor-query-1.2.0/tests/perfstress_tests/batch_query.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-query-1.1.1/tests/perfstress_tests/metric_query.py` & `azure-monitor-query-1.2.0/tests/perfstress_tests/metric_query.py`

 * *Files identical despite different names*

