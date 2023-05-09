# Comparing `tmp/aliyun-log-cli-0.2.5.tar.gz` & `tmp/aliyun-log-cli-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliyun-log-cli-0.2.5.tar", last modified: Mon Apr 10 03:14:56 2023, max compression
+gzip compressed data, was "aliyun-log-cli-0.2.6.tar", last modified: Tue May  9 04:00:40 2023, max compression
```

## Comparing `aliyun-log-cli-0.2.5.tar` & `aliyun-log-cli-0.2.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-04-10 03:14:56.593860 aliyun-log-cli-0.2.5/
--rw-r--r--   0 zhhfan     (502) staff       (20)     1070 2023-03-28 06:36:10.000000 aliyun-log-cli-0.2.5/LICENSE
--rw-r--r--   0 zhhfan     (502) staff       (20)      825 2023-04-10 03:14:56.593428 aliyun-log-cli-0.2.5/PKG-INFO
--rw-r--r--   0 zhhfan     (502) staff       (20)    19823 2023-03-28 06:36:10.000000 aliyun-log-cli-0.2.5/README.md
-drwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-04-10 03:14:56.587760 aliyun-log-cli-0.2.5/aliyun_log_cli.egg-info/
--rw-r--r--   0 zhhfan     (502) staff       (20)      825 2023-04-10 03:14:56.000000 aliyun-log-cli-0.2.5/aliyun_log_cli.egg-info/PKG-INFO
--rw-r--r--   0 zhhfan     (502) staff       (20)      423 2023-04-10 03:14:56.000000 aliyun-log-cli-0.2.5/aliyun_log_cli.egg-info/SOURCES.txt
--rw-r--r--   0 zhhfan     (502) staff       (20)        1 2023-04-10 03:14:56.000000 aliyun-log-cli-0.2.5/aliyun_log_cli.egg-info/dependency_links.txt
--rw-r--r--   0 zhhfan     (502) staff       (20)       52 2023-04-10 03:14:56.000000 aliyun-log-cli-0.2.5/aliyun_log_cli.egg-info/entry_points.txt
--rw-r--r--   0 zhhfan     (502) staff       (20)      100 2023-04-10 03:14:56.000000 aliyun-log-cli-0.2.5/aliyun_log_cli.egg-info/requires.txt
--rw-r--r--   0 zhhfan     (502) staff       (20)       13 2023-04-10 03:14:56.000000 aliyun-log-cli-0.2.5/aliyun_log_cli.egg-info/top_level.txt
-drwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-04-10 03:14:56.592880 aliyun-log-cli-0.2.5/aliyunlogcli/
--rw-r--r--   0 zhhfan     (502) staff       (20)       33 2023-03-28 06:36:10.000000 aliyun-log-cli-0.2.5/aliyunlogcli/__init__.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)      266 2023-03-28 06:36:10.000000 aliyun-log-cli-0.2.5/aliyunlogcli/cli.py
--rw-r--r--   0 zhhfan     (502) staff       (20)    11518 2023-04-10 03:12:40.000000 aliyun-log-cli-0.2.5/aliyunlogcli/cli_core.py
--rw-r--r--   0 zhhfan     (502) staff       (20)    20923 2023-04-10 03:12:40.000000 aliyun-log-cli-0.2.5/aliyunlogcli/config.py
--rw-r--r--   0 zhhfan     (502) staff       (20)      152 2023-03-28 06:36:10.000000 aliyun-log-cli-0.2.5/aliyunlogcli/exceptions.py
--rw-r--r--   0 zhhfan     (502) staff       (20)    13462 2023-04-10 03:12:40.000000 aliyun-log-cli-0.2.5/aliyunlogcli/parser.py
--rw-r--r--   0 zhhfan     (502) staff       (20)      147 2023-04-10 03:14:34.000000 aliyun-log-cli-0.2.5/aliyunlogcli/version.py
--rw-r--r--   0 zhhfan     (502) staff       (20)       38 2023-04-10 03:14:56.593966 aliyun-log-cli-0.2.5/setup.cfg
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     1719 2023-03-28 06:36:10.000000 aliyun-log-cli-0.2.5/setup.py
+drwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-05-09 04:00:40.790772 aliyun-log-cli-0.2.6/
+-rw-r--r--   0 zhhfan     (502) staff       (20)     1070 2023-03-28 06:36:10.000000 aliyun-log-cli-0.2.6/LICENSE
+-rw-r--r--   0 zhhfan     (502) staff       (20)      825 2023-05-09 04:00:40.790349 aliyun-log-cli-0.2.6/PKG-INFO
+-rw-r--r--   0 zhhfan     (502) staff       (20)    19823 2023-03-28 06:36:10.000000 aliyun-log-cli-0.2.6/README.md
+drwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-05-09 04:00:40.784577 aliyun-log-cli-0.2.6/aliyun_log_cli.egg-info/
+-rw-r--r--   0 zhhfan     (502) staff       (20)      825 2023-05-09 04:00:40.000000 aliyun-log-cli-0.2.6/aliyun_log_cli.egg-info/PKG-INFO
+-rw-r--r--   0 zhhfan     (502) staff       (20)      423 2023-05-09 04:00:40.000000 aliyun-log-cli-0.2.6/aliyun_log_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 zhhfan     (502) staff       (20)        1 2023-05-09 04:00:40.000000 aliyun-log-cli-0.2.6/aliyun_log_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 zhhfan     (502) staff       (20)       52 2023-05-09 04:00:40.000000 aliyun-log-cli-0.2.6/aliyun_log_cli.egg-info/entry_points.txt
+-rw-r--r--   0 zhhfan     (502) staff       (20)      100 2023-05-09 04:00:40.000000 aliyun-log-cli-0.2.6/aliyun_log_cli.egg-info/requires.txt
+-rw-r--r--   0 zhhfan     (502) staff       (20)       13 2023-05-09 04:00:40.000000 aliyun-log-cli-0.2.6/aliyun_log_cli.egg-info/top_level.txt
+drwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-05-09 04:00:40.789708 aliyun-log-cli-0.2.6/aliyunlogcli/
+-rw-r--r--   0 zhhfan     (502) staff       (20)       33 2023-03-28 06:36:10.000000 aliyun-log-cli-0.2.6/aliyunlogcli/__init__.py
+-rwxr-xr-x   0 zhhfan     (502) staff       (20)      266 2023-03-28 06:36:10.000000 aliyun-log-cli-0.2.6/aliyunlogcli/cli.py
+-rw-r--r--   0 zhhfan     (502) staff       (20)    11518 2023-04-10 03:12:40.000000 aliyun-log-cli-0.2.6/aliyunlogcli/cli_core.py
+-rw-r--r--   0 zhhfan     (502) staff       (20)    20979 2023-05-09 03:59:33.000000 aliyun-log-cli-0.2.6/aliyunlogcli/config.py
+-rw-r--r--   0 zhhfan     (502) staff       (20)      152 2023-03-28 06:36:10.000000 aliyun-log-cli-0.2.6/aliyunlogcli/exceptions.py
+-rw-r--r--   0 zhhfan     (502) staff       (20)    13462 2023-04-10 03:12:40.000000 aliyun-log-cli-0.2.6/aliyunlogcli/parser.py
+-rw-r--r--   0 zhhfan     (502) staff       (20)      147 2023-05-09 03:59:33.000000 aliyun-log-cli-0.2.6/aliyunlogcli/version.py
+-rw-r--r--   0 zhhfan     (502) staff       (20)       38 2023-05-09 04:00:40.790895 aliyun-log-cli-0.2.6/setup.cfg
+-rwxr-xr-x   0 zhhfan     (502) staff       (20)     1719 2023-03-28 06:36:10.000000 aliyun-log-cli-0.2.6/setup.py
```

### Comparing `aliyun-log-cli-0.2.5/LICENSE` & `aliyun-log-cli-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-log-cli-0.2.5/PKG-INFO` & `aliyun-log-cli-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aliyun-log-cli
-Version: 0.2.5
+Version: 0.2.6
 Summary: Aliyun log service CLI
 Home-page: https://github.com/aliyun/aliyun-log-cli
 Author: Aliyun
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.6
```

### Comparing `aliyun-log-cli-0.2.5/README.md` & `aliyun-log-cli-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `aliyun-log-cli-0.2.5/aliyun_log_cli.egg-info/PKG-INFO` & `aliyun-log-cli-0.2.6/aliyun_log_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aliyun-log-cli
-Version: 0.2.5
+Version: 0.2.6
 Summary: Aliyun log service CLI
 Home-page: https://github.com/aliyun/aliyun-log-cli
 Author: Aliyun
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.6
```

### Comparing `aliyun-log-cli-0.2.5/aliyunlogcli/cli_core.py` & `aliyun-log-cli-0.2.6/aliyunlogcli/cli_core.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-cli-0.2.5/aliyunlogcli/config.py` & `aliyun-log-cli-0.2.6/aliyunlogcli/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,32 +78,29 @@
 SUPPORT_LIST = {
     "Project": [
         "copy_project",
         "create_project",
         "delete_project",
         "get_project",
         "list_project",
-        "tag_project",
-        "untag_project",
     ],
     "Logstore": [
         "copy_logstore",
         "create_logstore",
         "delete_logstore",
-        "execute_logstore_sql",
         "get_logstore",
         "list_logstore",
         "update_logstore",
     ],
     "Index": [
         "create_index",
         "delete_index",
         "get_index_config",
-        "list_topics",
         "update_index",
+        "list_topics"
     ],
     "Logtail Config": [
         "create_logtail_config",
         "delete_logtail_config",
         "get_logtail_config",
         "list_logtail_config",
         "update_logtail_config",
@@ -116,32 +113,40 @@
         "get_machine_group",
         "get_machine_group_applied_configs",
         "list_machine_group",
         "list_machines",
         "remove_config_to_machine_group",
         "update_machine_group",
     ],
-    "Shard": ["arrange_shard", "list_shards", "merge_shard", "split_shard"],
+    "Shard": [
+        "arrange_shard",
+        "list_shards",
+        "merge_shard",
+        "split_shard",
+    ],
     "Cursor": [
         "get_begin_cursor",
         "get_cursor",
         "get_cursor_time",
         "get_end_cursor",
         "get_previous_cursor_time",
     ],
     "Logs": [
+        "copy_data",
         "get_context_logs",
         "get_histograms",
         "get_log",
-        "get_log_all",
         "get_logs",
+        "get_log_all",
         "get_project_logs",
         "pull_log",
-        "pull_log_dump",
         "pull_logs",
+        "pull_log_dump",
+        "execute_logstore_sql",
+        "execute_project_sql",
     ],
     "Consumer Group": [
         "create_consumer_group",
         "delete_consumer_group",
         "get_check_point",
         "get_check_point_fixed",
         "list_consumer_group",
@@ -167,35 +172,35 @@
         "delete_alert",
         "disable_alert",
         "enable_alert",
         "get_alert",
         "list_alert",
         "update_alert",
     ],
+    "Metric Store": [
+            "create_metric_store",
+            "get_metric_store",
+            "delete_metric_store",
+            "create_substore",
+            "get_substore",
+            "list_substore",
+            "update_substore",
+            "get_substore_ttl",
+            "update_substore_ttl",
+            "delete_substore",
+        ],
     "External Store": [
         "create_external_store",
         "delete_external_store",
         "get_external_store",
         "list_external_store",
         "update_external_store",
     ],
     "Others": [
-        "create_metric_store",
-        "create_substore",
-        "delete_metric_store",
-        "delete_substore",
         "es_migration",
-        "execute_project_sql",
-        "get_metric_store",
-        "get_project_tags",
-        "get_substore",
-        "get_substore_ttl",
-        "list_substore",
-        "update_substore",
-        "update_substore_ttl",
     ]
 }
 
 
 def _get_section_option(config, section_name, option_name, default=None):
     if six.PY3:
         return config.get(section_name, option_name, fallback=default)
```

### Comparing `aliyun-log-cli-0.2.5/aliyunlogcli/parser.py` & `aliyun-log-cli-0.2.6/aliyunlogcli/parser.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-cli-0.2.5/setup.py` & `aliyun-log-cli-0.2.6/setup.py`

 * *Files identical despite different names*

