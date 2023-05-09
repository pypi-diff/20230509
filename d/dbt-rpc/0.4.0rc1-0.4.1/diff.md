# Comparing `tmp/dbt-rpc-0.4.0rc1.tar.gz` & `tmp/dbt-rpc-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-rpc-0.4.0rc1.tar", last modified: Thu Apr 13 00:25:36 2023, max compression
+gzip compressed data, was "dbt-rpc-0.4.1.tar", last modified: Tue May  9 19:01:17 2023, max compression
```

## Comparing `dbt-rpc-0.4.0rc1.tar` & `dbt-rpc-0.4.1.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-04-13 00:25:36.066645 dbt-rpc-0.4.0rc1/
--rw-r--r--   0 chenyuli   (502) staff       (20)    11344 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/LICENSE.md
--rw-r--r--   0 chenyuli   (502) staff       (20)      863 2023-04-13 00:25:36.066500 dbt-rpc-0.4.0rc1/PKG-INFO
--rw-r--r--   0 chenyuli   (502) staff       (20)     1864 2022-12-16 19:31:44.000000 dbt-rpc-0.4.0rc1/README.md
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-04-13 00:25:36.056728 dbt-rpc-0.4.0rc1/dbt_rpc/
--rw-r--r--   0 chenyuli   (502) staff       (20)        0 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/dbt_rpc/__init__.py
--rw-r--r--   0 chenyuli   (502) staff       (20)    17375 2023-02-28 18:49:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc/__main__.py
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-04-13 00:25:36.058142 dbt-rpc-0.4.0rc1/dbt_rpc/contracts/
--rw-r--r--   0 chenyuli   (502) staff       (20)    22857 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0rc1/dbt_rpc/contracts/rpc.py
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-04-13 00:25:36.058643 dbt-rpc-0.4.0rc1/dbt_rpc/parser/
--rw-r--r--   0 chenyuli   (502) staff       (20)     1966 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0rc1/dbt_rpc/parser/rpc.py
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-04-13 00:25:36.061640 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/
--rw-r--r--   0 chenyuli   (502) staff       (20)     1992 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/__init__.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     8439 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/builtins.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     2259 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/error.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     3927 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/gc.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     6024 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/logger.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     5133 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/method.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     4374 2023-04-13 00:25:34.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/node_runners.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     4870 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/response_manager.py
--rw-r--r--   0 chenyuli   (502) staff       (20)    19107 2023-04-13 00:25:34.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/task_handler.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     2696 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/task_handler_protocol.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     9512 2023-02-28 18:49:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/task_manager.py
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-04-13 00:25:36.063322 dbt-rpc-0.4.0rc1/dbt_rpc/task/
--rw-r--r--   0 chenyuli   (502) staff       (20)        0 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/dbt_rpc/task/__init__.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     1569 2023-02-28 18:49:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc/task/base.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     5059 2023-02-28 18:49:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc/task/cli.py
--rw-r--r--   0 chenyuli   (502) staff       (20)      976 2023-02-28 18:49:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc/task/deps.py
--rw-r--r--   0 chenyuli   (502) staff       (20)    10644 2023-02-28 18:49:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc/task/project_commands.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     6222 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0rc1/dbt_rpc/task/server.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     7375 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0rc1/dbt_rpc/task/sql_commands.py
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-04-13 00:25:36.058003 dbt-rpc-0.4.0rc1/dbt_rpc.egg-info/
--rw-r--r--   0 chenyuli   (502) staff       (20)      863 2023-04-13 00:25:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc.egg-info/PKG-INFO
--rw-r--r--   0 chenyuli   (502) staff       (20)     1089 2023-04-13 00:25:36.000000 dbt-rpc-0.4.0rc1/dbt_rpc.egg-info/SOURCES.txt
--rw-r--r--   0 chenyuli   (502) staff       (20)        1 2023-04-13 00:25:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc.egg-info/dependency_links.txt
--rw-r--r--   0 chenyuli   (502) staff       (20)       50 2023-04-13 00:25:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc.egg-info/entry_points.txt
--rw-r--r--   0 chenyuli   (502) staff       (20)        1 2022-07-20 22:27:25.000000 dbt-rpc-0.4.0rc1/dbt_rpc.egg-info/not-zip-safe
--rw-r--r--   0 chenyuli   (502) staff       (20)       36 2023-04-13 00:25:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc.egg-info/requires.txt
--rw-r--r--   0 chenyuli   (502) staff       (20)        8 2023-04-13 00:25:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc.egg-info/top_level.txt
--rw-r--r--   0 chenyuli   (502) staff       (20)       38 2023-04-13 00:25:36.066688 dbt-rpc-0.4.0rc1/setup.cfg
--rw-r--r--   0 chenyuli   (502) staff       (20)     1443 2023-04-13 00:25:34.000000 dbt-rpc-0.4.0rc1/setup.py
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-04-13 00:25:36.066285 dbt-rpc-0.4.0rc1/tests/
--rw-r--r--   0 chenyuli   (502) staff       (20)     5803 2023-02-14 23:05:02.000000 dbt-rpc-0.4.0rc1/tests/test_build.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     2763 2023-04-06 22:01:40.000000 dbt-rpc-0.4.0rc1/tests/test_compile.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     1284 2023-04-13 00:25:34.000000 dbt-rpc-0.4.0rc1/tests/test_compile_sql.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     1154 2022-07-23 23:11:05.000000 dbt-rpc-0.4.0rc1/tests/test_concurrency.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     5955 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/tests/test_deps.py
--rw-r--r--   0 chenyuli   (502) staff       (20)    12604 2022-12-30 20:30:27.000000 dbt-rpc-0.4.0rc1/tests/test_management.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     4500 2022-07-23 23:11:26.000000 dbt-rpc-0.4.0rc1/tests/test_run.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     3018 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/tests/test_run_operation.py
--rw-r--r--   0 chenyuli   (502) staff       (20)      562 2022-09-14 22:22:50.000000 dbt-rpc-0.4.0rc1/tests/test_run_sql.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     3517 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/tests/test_seed.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     4638 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/tests/test_snapshots.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     6387 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/tests/test_source_freshness.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     3242 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/tests/test_test.py
+drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-05-09 19:01:17.295311 dbt-rpc-0.4.1/
+-rw-r--r--   0 chenyuli   (502) staff       (20)    11344 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/LICENSE.md
+-rw-r--r--   0 chenyuli   (502) staff       (20)      860 2023-05-09 19:01:17.295141 dbt-rpc-0.4.1/PKG-INFO
+-rw-r--r--   0 chenyuli   (502) staff       (20)     1864 2023-05-09 18:24:11.000000 dbt-rpc-0.4.1/README.md
+drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-05-09 19:01:17.278730 dbt-rpc-0.4.1/dbt_rpc/
+-rw-r--r--   0 chenyuli   (502) staff       (20)        0 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/dbt_rpc/__init__.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)    17375 2023-05-09 18:24:31.000000 dbt-rpc-0.4.1/dbt_rpc/__main__.py
+drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-05-09 19:01:17.280374 dbt-rpc-0.4.1/dbt_rpc/contracts/
+-rw-r--r--   0 chenyuli   (502) staff       (20)    23370 2023-05-09 19:01:03.000000 dbt-rpc-0.4.1/dbt_rpc/contracts/rpc.py
+drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-05-09 19:01:17.280602 dbt-rpc-0.4.1/dbt_rpc/parser/
+-rw-r--r--   0 chenyuli   (502) staff       (20)     1966 2023-05-09 18:24:11.000000 dbt-rpc-0.4.1/dbt_rpc/parser/rpc.py
+drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-05-09 19:01:17.284076 dbt-rpc-0.4.1/dbt_rpc/rpc/
+-rw-r--r--   0 chenyuli   (502) staff       (20)     1992 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/__init__.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     8811 2023-05-09 19:01:03.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/builtins.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     2259 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/error.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     3926 2023-05-09 19:01:03.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/gc.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     6024 2023-05-09 18:24:11.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/logger.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     5133 2023-05-09 18:24:11.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/method.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     4374 2023-05-09 18:24:31.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/node_runners.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     4869 2023-05-09 19:01:03.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/response_manager.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)    19107 2023-05-09 18:24:31.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/task_handler.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     2694 2023-05-09 19:01:03.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/task_handler_protocol.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     9510 2023-05-09 19:01:03.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/task_manager.py
+drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-05-09 19:01:17.285959 dbt-rpc-0.4.1/dbt_rpc/task/
+-rw-r--r--   0 chenyuli   (502) staff       (20)        0 2023-05-01 23:43:40.000000 dbt-rpc-0.4.1/dbt_rpc/task/__init__.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     1569 2023-05-09 18:24:31.000000 dbt-rpc-0.4.1/dbt_rpc/task/base.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     5059 2023-05-09 18:24:31.000000 dbt-rpc-0.4.1/dbt_rpc/task/cli.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)      976 2023-05-09 18:24:31.000000 dbt-rpc-0.4.1/dbt_rpc/task/deps.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)    10644 2023-05-09 18:24:31.000000 dbt-rpc-0.4.1/dbt_rpc/task/project_commands.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     6222 2023-05-09 18:24:11.000000 dbt-rpc-0.4.1/dbt_rpc/task/server.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     7375 2023-05-09 18:24:11.000000 dbt-rpc-0.4.1/dbt_rpc/task/sql_commands.py
+drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-05-09 19:01:17.280179 dbt-rpc-0.4.1/dbt_rpc.egg-info/
+-rw-r--r--   0 chenyuli   (502) staff       (20)      860 2023-05-09 19:01:17.000000 dbt-rpc-0.4.1/dbt_rpc.egg-info/PKG-INFO
+-rw-r--r--   0 chenyuli   (502) staff       (20)     1129 2023-05-09 19:01:17.000000 dbt-rpc-0.4.1/dbt_rpc.egg-info/SOURCES.txt
+-rw-r--r--   0 chenyuli   (502) staff       (20)        1 2023-05-09 19:01:17.000000 dbt-rpc-0.4.1/dbt_rpc.egg-info/dependency_links.txt
+-rw-r--r--   0 chenyuli   (502) staff       (20)       50 2023-05-09 19:01:17.000000 dbt-rpc-0.4.1/dbt_rpc.egg-info/entry_points.txt
+-rw-r--r--   0 chenyuli   (502) staff       (20)        1 2022-07-20 22:27:25.000000 dbt-rpc-0.4.1/dbt_rpc.egg-info/not-zip-safe
+-rw-r--r--   0 chenyuli   (502) staff       (20)       34 2023-05-09 19:01:17.000000 dbt-rpc-0.4.1/dbt_rpc.egg-info/requires.txt
+-rw-r--r--   0 chenyuli   (502) staff       (20)        8 2023-05-09 19:01:17.000000 dbt-rpc-0.4.1/dbt_rpc.egg-info/top_level.txt
+-rw-r--r--   0 chenyuli   (502) staff       (20)       38 2023-05-09 19:01:17.295373 dbt-rpc-0.4.1/setup.cfg
+-rw-r--r--   0 chenyuli   (502) staff       (20)     1413 2023-05-09 19:01:03.000000 dbt-rpc-0.4.1/setup.py
+drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-05-09 19:01:17.294876 dbt-rpc-0.4.1/tests/
+-rw-r--r--   0 chenyuli   (502) staff       (20)     5803 2023-02-14 23:05:02.000000 dbt-rpc-0.4.1/tests/test_build.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     2763 2023-04-06 22:01:40.000000 dbt-rpc-0.4.1/tests/test_compile.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     1284 2023-05-09 18:24:31.000000 dbt-rpc-0.4.1/tests/test_compile_sql.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     1154 2022-07-23 23:11:05.000000 dbt-rpc-0.4.1/tests/test_concurrency.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     5955 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/tests/test_deps.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     1071 2023-05-09 16:38:54.000000 dbt-rpc-0.4.1/tests/test_list.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)    12604 2023-05-09 18:24:11.000000 dbt-rpc-0.4.1/tests/test_management.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)      502 2023-05-03 14:55:51.000000 dbt-rpc-0.4.1/tests/test_reload.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     4500 2022-07-23 23:11:26.000000 dbt-rpc-0.4.1/tests/test_run.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     3018 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/tests/test_run_operation.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)      562 2022-09-14 22:22:50.000000 dbt-rpc-0.4.1/tests/test_run_sql.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     3517 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/tests/test_seed.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     4638 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/tests/test_snapshots.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     6387 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/tests/test_source_freshness.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     3242 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/tests/test_test.py
```

### Comparing `dbt-rpc-0.4.0rc1/LICENSE.md` & `dbt-rpc-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/PKG-INFO` & `dbt-rpc-0.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-rpc
-Version: 0.4.0rc1
+Version: 0.4.1
 Summary:  A JSON RPC server that provides an interface to programmically interact with dbt projects. 
 Home-page: https://github.com/dbt-labs/dbt-rpc
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-rpc-0.4.0rc1/README.md` & `dbt-rpc-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/__main__.py` & `dbt-rpc-0.4.1/dbt_rpc/__main__.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/contracts/rpc.py` & `dbt-rpc-0.4.1/dbt_rpc/contracts/rpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from typing import Optional, Union, List, Any, Dict, Type, Sequence
 
 from dbt.dataclass_schema import dbtClassMixin, StrEnum
 
 from dbt.contracts.graph.nodes import ResultNode
 from dbt.contracts.graph.manifest import WritableManifest
 from dbt.contracts.results import (
-    RunResult, RunResultsArtifact, TimingInfo,
+    RunResult,
+    RunResultsArtifact,
+    TimingInfo,
     CatalogArtifact,
     CatalogResults,
     ExecutionResult,
     FreshnessExecutionResultArtifact,
     FreshnessResult,
     RunOperationResult,
     RunOperationResultsArtifact,
@@ -36,27 +38,27 @@
 class RPCParameters(dbtClassMixin):
     task_tags: TaskTags
     timeout: Optional[float]
 
     @classmethod
     def __pre_deserialize__(cls, data, omit_none=True):
         data = super().__pre_deserialize__(data)
-        if 'timeout' not in data:
-            data['timeout'] = None
-        if 'task_tags' not in data:
-            data['task_tags'] = None
+        if "timeout" not in data:
+            data["timeout"] = None
+        if "task_tags" not in data:
+            data["task_tags"] = None
         return data
 
 
 @dataclass
 class RPCExecParameters(RPCParameters):
     name: str
     sql: str
     macros: Optional[str] = None
-    language: Optional[str] = 'sql'
+    language: Optional[str] = "sql"
 
 
 @dataclass
 class RPCCompileParameters(RPCParameters):
     threads: Optional[int] = None
     models: Union[None, str, List[str]] = None
     select: Union[None, str, List[str]] = None
@@ -68,15 +70,15 @@
 @dataclass
 class RPCListParameters(RPCParameters):
     resource_types: Optional[List[str]] = None
     models: Union[None, str, List[str]] = None
     exclude: Union[None, str, List[str]] = None
     select: Union[None, str, List[str]] = None
     selector: Optional[str] = None
-    output: Optional[str] = 'json'
+    output: Optional[str] = "json"
     output_keys: Optional[List[str]] = None
 
 
 @dataclass
 class RPCRunParameters(RPCParameters):
     threads: Optional[int] = None
     models: Union[None, str, List[str]] = None
@@ -161,14 +163,19 @@
 
 @dataclass
 class StatusParameters(RPCParameters):
     pass
 
 
 @dataclass
+class ReloadParameters(RPCParameters):
+    pass
+
+
+@dataclass
 class GCSettings(dbtClassMixin):
     # start evicting the longest-ago-ended tasks here
     maxsize: int
     # start evicting all tasks before now - auto_reap_age when we have this
     # many tasks in the table
     reapsize: int
     # a positive timedelta indicating how far back we should go
@@ -182,14 +189,15 @@
     - task_ids: An optional list of task ID UUIDs to try to GC
     - before: If provided, should be a datetime string. All tasks that finished
         before that datetime will be GCed
     - settings: If provided, should be a GCSettings object in JSON form. It
         will be applied to the task manager before GC starts. By default the
         existing gc settings remain.
     """
+
     task_ids: Optional[List[TaskID]] = None
     before: Optional[datetime] = None
     settings: Optional[GCSettings] = None
 
 
 @dataclass
 class RPCRunOperationParameters(RPCParameters):
@@ -205,45 +213,46 @@
     selector: Optional[str] = None
 
 
 @dataclass
 class GetManifestParameters(RPCParameters):
     pass
 
+
 # Outputs
 
 
 @dataclass
 class RemoteResult(VersionedSchema):
     logs: List[LogMessage]
 
     def __post_serialize__(self, dct):
-        if 'node' in dct:
-            if 'raw_code' in dct['node']:
-                dct['node']['raw_sql'] = dct['node'].pop('raw_code')
-            if 'compiled_code' in dct['node']:
-                dct['node']['compiled_sql'] = dct['node'].pop('compiled_code')
+        if "node" in dct:
+            if "raw_code" in dct["node"]:
+                dct["node"]["raw_sql"] = dct["node"].pop("raw_code")
+            if "compiled_code" in dct["node"]:
+                dct["node"]["compiled_sql"] = dct["node"].pop("compiled_code")
         return dct
 
 
 @dataclass
-@schema_version('remote-list-results', 1)
+@schema_version("remote-list-results", 1)
 class RemoteListResults(RemoteResult):
     output: List[Any]
     generated_at: datetime = field(default_factory=datetime.utcnow)
 
 
 @dataclass
-@schema_version('remote-deps-result', 1)
+@schema_version("remote-deps-result", 1)
 class RemoteDepsResult(RemoteResult):
     generated_at: datetime = field(default_factory=datetime.utcnow)
 
 
 @dataclass
-@schema_version('remote-catalog-result', 1)
+@schema_version("remote-catalog-result", 1)
 class RemoteCatalogResults(CatalogResults, RemoteResult):
     generated_at: datetime = field(default_factory=datetime.utcnow)
 
     def write(self, path: str):
         artifact = CatalogArtifact.from_results(
             generated_at=self.generated_at,
             nodes=self.nodes,
@@ -259,37 +268,39 @@
     raw_sql: str
     compiled_sql: str
     node: ResultNode
     timing: List[TimingInfo]
 
 
 @dataclass
-@schema_version('remote-compile-result', 1)
+@schema_version("remote-compile-result", 1)
 class RemoteCompileResult(RemoteCompileResultMixin):
     generated_at: datetime = field(default_factory=datetime.utcnow)
 
     @property
     def error(self):
         return None
 
 
 @dataclass
-@schema_version('remote-execution-result', 1)
+@schema_version("remote-execution-result", 1)
 class RemoteExecutionResult(ExecutionResult, RemoteResult):
     results: Sequence[RunResult]
     args: Dict[str, Any] = field(default_factory=dict)
     generated_at: datetime = field(default_factory=datetime.utcnow)
 
     def __post_serialize__(self, dct):
-        for node_dct in dct['results']:
-            if 'node' in node_dct:
-                if 'raw_code' in node_dct['node']:
-                    node_dct['node']['raw_sql'] = node_dct['node'].pop('raw_code')
-                if 'compiled_code' in node_dct['node']:
-                    node_dct['node']['compiled_sql'] = node_dct['node'].pop('compiled_code')
+        for node_dct in dct["results"]:
+            if "node" in node_dct:
+                if "raw_code" in node_dct["node"]:
+                    node_dct["node"]["raw_sql"] = node_dct["node"].pop("raw_code")
+                if "compiled_code" in node_dct["node"]:
+                    node_dct["node"]["compiled_sql"] = node_dct["node"].pop(
+                        "compiled_code"
+                    )
         return dct
 
     def write(self, path: str):
         writable = RunResultsArtifact.from_execution_results(
             generated_at=self.generated_at,
             results=self.results,
             elapsed_time=self.elapsed_time,
@@ -298,15 +309,15 @@
         writable.write(path)
 
     @classmethod
     def from_local_result(
         cls,
         base: RunExecutionResult,
         logs: List[LogMessage],
-    ) -> 'RemoteExecutionResult':
+    ) -> "RemoteExecutionResult":
         return cls(
             generated_at=base.generated_at,
             results=base.results,
             elapsed_time=base.elapsed_time,
             args=base.args,
             logs=logs,
         )
@@ -315,24 +326,24 @@
 @dataclass
 class ResultTable(dbtClassMixin):
     column_names: List[str]
     rows: List[Any]
 
 
 @dataclass
-@schema_version('remote-run-operation-result', 1)
+@schema_version("remote-run-operation-result", 1)
 class RemoteRunOperationResult(RunOperationResult, RemoteResult):
     generated_at: datetime = field(default_factory=datetime.utcnow)
 
     @classmethod
     def from_local_result(
         cls,
         base: RunOperationResultsArtifact,
         logs: List[LogMessage],
-    ) -> 'RemoteRunOperationResult':
+    ) -> "RemoteRunOperationResult":
         return cls(
             generated_at=base.metadata.generated_at,
             results=base.results,
             elapsed_time=base.elapsed_time,
             success=base.success,
             logs=logs,
         )
@@ -343,37 +354,36 @@
             generated_at=self.generated_at,
             elapsed_time=self.elapsed_time,
         )
         writable.write(path)
 
 
 @dataclass
-@schema_version('remote-freshness-result', 1)
+@schema_version("remote-freshness-result", 1)
 class RemoteFreshnessResult(FreshnessResult, RemoteResult):
-
     @classmethod
     def from_local_result(
         cls,
         base: FreshnessResult,
         logs: List[LogMessage],
-    ) -> 'RemoteFreshnessResult':
+    ) -> "RemoteFreshnessResult":
         return cls(
             metadata=base.metadata,
             results=base.results,
             elapsed_time=base.elapsed_time,
             logs=logs,
         )
 
     def write(self, path: str):
         writable = FreshnessExecutionResultArtifact.from_result(base=self)
         writable.write(path)
 
 
 @dataclass
-@schema_version('remote-run-result', 1)
+@schema_version("remote-run-result", 1)
 class RemoteRunResult(RemoteCompileResultMixin):
     table: ResultTable
     generated_at: datetime = field(default_factory=datetime.utcnow)
 
 
 RPCResult = Union[
     RemoteCompileResult,
@@ -383,90 +393,86 @@
     RemoteDepsResult,
     RemoteRunOperationResult,
 ]
 
 
 # GC types
 
+
 class GCResultState(StrEnum):
-    Deleted = 'deleted'  # successful GC
-    Missing = 'missing'  # nothing to GC
-    Running = 'running'  # can't GC
+    Deleted = "deleted"  # successful GC
+    Missing = "missing"  # nothing to GC
+    Running = "running"  # can't GC
 
 
 @dataclass
-@schema_version('remote-gc-result', 1)
+@schema_version("remote-gc-result", 1)
 class GCResult(RemoteResult):
     logs: List[LogMessage] = field(default_factory=list)
     deleted: List[TaskID] = field(default_factory=list)
     missing: List[TaskID] = field(default_factory=list)
     running: List[TaskID] = field(default_factory=list)
 
     def add_result(self, task_id: TaskID, state: GCResultState):
         if state == GCResultState.Missing:
             self.missing.append(task_id)
         elif state == GCResultState.Running:
             self.running.append(task_id)
         elif state == GCResultState.Deleted:
             self.deleted.append(task_id)
         else:
-            raise DbtInternalError(
-                f'Got invalid state in add_result: {state}'
-            )
+            raise DbtInternalError(f"Got invalid state in add_result: {state}")
+
 
 # Task management types
 
 
 class TaskHandlerState(StrEnum):
-    NotStarted = 'not started'
-    Initializing = 'initializing'
-    Running = 'running'
-    Success = 'success'
-    Error = 'error'
-    Killed = 'killed'
-    Failed = 'failed'
+    NotStarted = "not started"
+    Initializing = "initializing"
+    Running = "running"
+    Success = "success"
+    Error = "error"
+    Killed = "killed"
+    Failed = "failed"
 
     def __lt__(self, other) -> bool:
         """A logical ordering for TaskHandlerState:
 
         NotStarted < Initializing < Running < (Success, Error, Killed, Failed)
         """
         if not isinstance(other, TaskHandlerState):
-            raise TypeError('cannot compare to non-TaskHandlerState')
+            raise TypeError("cannot compare to non-TaskHandlerState")
         order = (self.NotStarted, self.Initializing, self.Running)
         smaller = set()
         for value in order:
             smaller.add(value)
             if self == value:
                 return other not in smaller
 
         return False
 
     def __le__(self, other) -> bool:
         # so that ((Success <= Error) is True)
-        return ((self < other) or
-                (self == other) or
-                (self.finished and other.finished))
+        return (self < other) or (self == other) or (self.finished and other.finished)
 
     def __gt__(self, other) -> bool:
         if not isinstance(other, TaskHandlerState):
-            raise TypeError('cannot compare to non-TaskHandlerState')
+            raise TypeError("cannot compare to non-TaskHandlerState")
         order = (self.NotStarted, self.Initializing, self.Running)
         smaller = set()
         for value in order:
             smaller.add(value)
             if self == value:
                 return other in smaller
         return other in smaller
 
     def __ge__(self, other) -> bool:
         # so that ((Success <= Error) is True)
-        return ((self > other) or
-                (self == other) or
-                (self.finished and other.finished))
+        return (self > other) or (self == other) or (self.finished and other.finished)
 
     @property
     def finished(self) -> bool:
         return self in (self.Error, self.Success, self.Killed, self.Failed)
 
 
 @dataclass
@@ -477,15 +483,15 @@
     elapsed: Optional[float]
 
     # These ought to be defaults but superclass order doesn't
     # allow that to work
     @classmethod
     def __pre_deserialize__(cls, data):
         data = super().__pre_deserialize__(data)
-        for field_name in ('start', 'end', 'elapsed'):
+        for field_name in ("start", "end", "elapsed"):
             if field_name not in data:
                 data[field_name] = None
         return data
 
 
 @dataclass
 class TaskRow(TaskTiming):
@@ -494,35 +500,35 @@
     method: str
     request_id: Union[str, int]
     tags: TaskTags = None
     timeout: Optional[float] = None
 
 
 @dataclass
-@schema_version('remote-ps-result', 1)
+@schema_version("remote-ps-result", 1)
 class PSResult(RemoteResult):
     rows: List[TaskRow]
 
 
 class KillResultStatus(StrEnum):
-    Missing = 'missing'
-    NotStarted = 'not_started'
-    Killed = 'killed'
-    Finished = 'finished'
+    Missing = "missing"
+    NotStarted = "not_started"
+    Killed = "killed"
+    Finished = "finished"
 
 
 @dataclass
-@schema_version('remote-kill-result', 1)
+@schema_version("remote-kill-result", 1)
 class KillResult(RemoteResult):
     state: KillResultStatus = KillResultStatus.Missing
     logs: List[LogMessage] = field(default_factory=list)
 
 
 @dataclass
-@schema_version('remote-manifest-result', 1)
+@schema_version("remote-manifest-result", 1)
 class GetManifestResult(RemoteResult):
     manifest: Optional[WritableManifest] = None
 
 
 # this is kind of carefuly structured: BlocksManifestTasks is implied by
 # RequiresConfigReloadBefore and RequiresManifestReloadAfter
 class RemoteMethodFlags(enum.Flag):
@@ -545,176 +551,171 @@
     elapsed: Optional[float]
 
     # These ought to be defaults but superclass order doesn't
     # allow that to work
     @classmethod
     def __pre_deserialize__(cls, data):
         data = super().__pre_deserialize__(data)
-        for field_name in ('start', 'end', 'elapsed'):
+        for field_name in ("start", "end", "elapsed"):
             if field_name not in data:
                 data[field_name] = None
         return data
 
 
 @dataclass
-@schema_version('poll-remote-deps-result', 1)
+@schema_version("poll-remote-deps-result", 1)
 class PollRemoteEmptyCompleteResult(PollResult, RemoteResult):
     state: TaskHandlerState = field(
-        metadata=restrict_to(TaskHandlerState.Success,
-                             TaskHandlerState.Failed),
+        metadata=restrict_to(TaskHandlerState.Success, TaskHandlerState.Failed),
     )
     generated_at: datetime = field(default_factory=datetime.utcnow)
 
     @classmethod
     def from_result(
-        cls: Type['PollRemoteEmptyCompleteResult'],
+        cls: Type["PollRemoteEmptyCompleteResult"],
         base: RemoteDepsResult,
         tags: TaskTags,
         timing: TaskTiming,
         logs: List[LogMessage],
-    ) -> 'PollRemoteEmptyCompleteResult':
+    ) -> "PollRemoteEmptyCompleteResult":
         return cls(
             logs=logs,
             tags=tags,
             state=timing.state,
             start=timing.start,
             end=timing.end,
             elapsed=timing.elapsed,
-            generated_at=base.generated_at
+            generated_at=base.generated_at,
         )
 
 
 @dataclass
-@schema_version('poll-remote-killed-result', 1)
+@schema_version("poll-remote-killed-result", 1)
 class PollKilledResult(PollResult):
     state: TaskHandlerState = field(
         metadata=restrict_to(TaskHandlerState.Killed),
     )
 
 
 @dataclass
-@schema_version('poll-remote-execution-result', 1)
+@schema_version("poll-remote-execution-result", 1)
 class PollExecuteCompleteResult(
     RemoteExecutionResult,
     PollResult,
 ):
     state: TaskHandlerState = field(
-        metadata=restrict_to(TaskHandlerState.Success,
-                             TaskHandlerState.Failed),
+        metadata=restrict_to(TaskHandlerState.Success, TaskHandlerState.Failed),
     )
 
     @classmethod
     def from_result(
-        cls: Type['PollExecuteCompleteResult'],
+        cls: Type["PollExecuteCompleteResult"],
         base: RemoteExecutionResult,
         tags: TaskTags,
         timing: TaskTiming,
         logs: List[LogMessage],
-    ) -> 'PollExecuteCompleteResult':
+    ) -> "PollExecuteCompleteResult":
         return cls(
             results=base.results,
             elapsed_time=base.elapsed_time,
             logs=logs,
             tags=tags,
             state=timing.state,
             start=timing.start,
             end=timing.end,
             elapsed=timing.elapsed,
             generated_at=base.generated_at,
         )
 
 
 @dataclass
-@schema_version('poll-remote-compile-result', 1)
+@schema_version("poll-remote-compile-result", 1)
 class PollCompileCompleteResult(
     RemoteCompileResult,
     PollResult,
 ):
     state: TaskHandlerState = field(
-        metadata=restrict_to(TaskHandlerState.Success,
-                             TaskHandlerState.Failed),
+        metadata=restrict_to(TaskHandlerState.Success, TaskHandlerState.Failed),
     )
 
     @classmethod
     def from_result(
-        cls: Type['PollCompileCompleteResult'],
+        cls: Type["PollCompileCompleteResult"],
         base: RemoteCompileResult,
         tags: TaskTags,
         timing: TaskTiming,
         logs: List[LogMessage],
-    ) -> 'PollCompileCompleteResult':
+    ) -> "PollCompileCompleteResult":
         return cls(
             raw_sql=base.raw_sql,
             compiled_sql=base.compiled_sql,
             node=base.node,
             timing=base.timing,
             logs=logs,
             tags=tags,
             state=timing.state,
             start=timing.start,
             end=timing.end,
             elapsed=timing.elapsed,
-            generated_at=base.generated_at
+            generated_at=base.generated_at,
         )
 
 
 @dataclass
-@schema_version('poll-remote-run-result', 1)
+@schema_version("poll-remote-run-result", 1)
 class PollRunCompleteResult(
     RemoteRunResult,
     PollResult,
 ):
     state: TaskHandlerState = field(
-        metadata=restrict_to(TaskHandlerState.Success,
-                             TaskHandlerState.Failed),
+        metadata=restrict_to(TaskHandlerState.Success, TaskHandlerState.Failed),
     )
 
     @classmethod
     def from_result(
-        cls: Type['PollRunCompleteResult'],
+        cls: Type["PollRunCompleteResult"],
         base: RemoteRunResult,
         tags: TaskTags,
         timing: TaskTiming,
         logs: List[LogMessage],
-    ) -> 'PollRunCompleteResult':
+    ) -> "PollRunCompleteResult":
         return cls(
             raw_sql=base.raw_sql,
             compiled_sql=base.compiled_sql,
             node=base.node,
             timing=base.timing,
             logs=logs,
             table=base.table,
             tags=tags,
             state=timing.state,
             start=timing.start,
             end=timing.end,
             elapsed=timing.elapsed,
-            generated_at=base.generated_at
+            generated_at=base.generated_at,
         )
 
 
 @dataclass
-@schema_version('poll-remote-run-operation-result', 1)
+@schema_version("poll-remote-run-operation-result", 1)
 class PollRunOperationCompleteResult(
     RemoteRunOperationResult,
     PollResult,
 ):
     state: TaskHandlerState = field(
-        metadata=restrict_to(TaskHandlerState.Success,
-                             TaskHandlerState.Failed),
+        metadata=restrict_to(TaskHandlerState.Success, TaskHandlerState.Failed),
     )
 
     @classmethod
     def from_result(
-        cls: Type['PollRunOperationCompleteResult'],
+        cls: Type["PollRunOperationCompleteResult"],
         base: RemoteRunOperationResult,
         tags: TaskTags,
         timing: TaskTiming,
         logs: List[LogMessage],
-    ) -> 'PollRunOperationCompleteResult':
+    ) -> "PollRunOperationCompleteResult":
         return cls(
             success=base.success,
             results=base.results,
             generated_at=base.generated_at,
             elapsed_time=base.elapsed_time,
             logs=logs,
             tags=tags,
@@ -722,29 +723,28 @@
             start=timing.start,
             end=timing.end,
             elapsed=timing.elapsed,
         )
 
 
 @dataclass
-@schema_version('poll-remote-catalog-result', 1)
+@schema_version("poll-remote-catalog-result", 1)
 class PollCatalogCompleteResult(RemoteCatalogResults, PollResult):
     state: TaskHandlerState = field(
-        metadata=restrict_to(TaskHandlerState.Success,
-                             TaskHandlerState.Failed),
+        metadata=restrict_to(TaskHandlerState.Success, TaskHandlerState.Failed),
     )
 
     @classmethod
     def from_result(
-        cls: Type['PollCatalogCompleteResult'],
+        cls: Type["PollCatalogCompleteResult"],
         base: RemoteCatalogResults,
         tags: TaskTags,
         timing: TaskTiming,
         logs: List[LogMessage],
-    ) -> 'PollCatalogCompleteResult':
+    ) -> "PollCatalogCompleteResult":
         return cls(
             nodes=base.nodes,
             sources=base.sources,
             generated_at=base.generated_at,
             errors=base.errors,
             _compile_results=base._compile_results,
             logs=logs,
@@ -753,85 +753,111 @@
             start=timing.start,
             end=timing.end,
             elapsed=timing.elapsed,
         )
 
 
 @dataclass
-@schema_version('poll-remote-in-progress-result', 1)
+@schema_version("poll-remote-in-progress-result", 1)
 class PollInProgressResult(PollResult):
     pass
 
 
 @dataclass
-@schema_version('poll-remote-get-manifest-result', 1)
+@schema_version("poll-remote-get-manifest-result", 1)
 class PollGetManifestResult(GetManifestResult, PollResult):
     state: TaskHandlerState = field(
-        metadata=restrict_to(TaskHandlerState.Success,
-                             TaskHandlerState.Failed),
+        metadata=restrict_to(TaskHandlerState.Success, TaskHandlerState.Failed),
     )
 
     @classmethod
     def from_result(
-        cls: Type['PollGetManifestResult'],
+        cls: Type["PollGetManifestResult"],
         base: GetManifestResult,
         tags: TaskTags,
         timing: TaskTiming,
         logs: List[LogMessage],
-    ) -> 'PollGetManifestResult':
+    ) -> "PollGetManifestResult":
         return cls(
             manifest=base.manifest,
             logs=logs,
             tags=tags,
             state=timing.state,
             start=timing.start,
             end=timing.end,
             elapsed=timing.elapsed,
         )
 
 
 @dataclass
-@schema_version('poll-remote-freshness-result', 1)
-class PollFreshnessResult(RemoteFreshnessResult, PollResult):
+@schema_version('poll-remote-list-result', 1)
+class PollListResult(RemoteListResults, PollResult):
     state: TaskHandlerState = field(
         metadata=restrict_to(TaskHandlerState.Success,
                              TaskHandlerState.Failed),
     )
 
     @classmethod
     def from_result(
-        cls: Type['PollFreshnessResult'],
+        cls: Type['PollListResult'],
+        base: RemoteListResults,
+        tags: TaskTags,
+        timing: TaskTiming,
+        logs: List[LogMessage],
+    ) -> 'PollListResult':
+        return cls(
+            output=base.output,
+            logs=logs,
+            tags=tags,
+            state=timing.state,
+            start=timing.start,
+            end=timing.end,
+            elapsed=timing.elapsed,
+        )
+
+
+@dataclass
+@schema_version("poll-remote-freshness-result", 1)
+class PollFreshnessResult(RemoteFreshnessResult, PollResult):
+    state: TaskHandlerState = field(
+        metadata=restrict_to(TaskHandlerState.Success, TaskHandlerState.Failed),
+    )
+
+    @classmethod
+    def from_result(
+        cls: Type["PollFreshnessResult"],
         base: RemoteFreshnessResult,
         tags: TaskTags,
         timing: TaskTiming,
         logs: List[LogMessage],
-    ) -> 'PollFreshnessResult':
+    ) -> "PollFreshnessResult":
         return cls(
             logs=logs,
             tags=tags,
             state=timing.state,
             start=timing.start,
             end=timing.end,
             elapsed=timing.elapsed,
             metadata=base.metadata,
             results=base.results,
             elapsed_time=base.elapsed_time,
         )
 
+
 # Manifest parsing types
 
 
 class ManifestStatus(StrEnum):
-    Init = 'init'
-    Compiling = 'compiling'
-    Ready = 'ready'
-    Error = 'error'
+    Init = "init"
+    Compiling = "compiling"
+    Ready = "ready"
+    Error = "error"
 
 
 @dataclass
-@schema_version('remote-status-result', 1)
+@schema_version("remote-status-result", 1)
 class LastParse(RemoteResult):
     state: ManifestStatus = ManifestStatus.Init
     logs: List[LogMessage] = field(default_factory=list)
     error: Optional[Dict[str, Any]] = None
     timestamp: datetime = field(default_factory=datetime.utcnow)
     pid: int = field(default_factory=os.getpid)
```

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/parser/rpc.py` & `dbt-rpc-0.4.1/dbt_rpc/parser/rpc.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/__init__.py` & `dbt-rpc-0.4.1/dbt_rpc/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/builtins.py` & `dbt-rpc-0.4.1/dbt_rpc/rpc/builtins.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import os
 import signal
 from datetime import datetime
 from typing import Type, Union, Any, List, Dict
 
 import dbt.exceptions
 from dbt_rpc.contracts.rpc import (
+    PollListResult,
+    RemoteListResults,
     TaskTags,
     StatusParameters,
+    ReloadParameters,
     LastParse,
     GCParameters,
     GCResult,
     GetManifestResult,
     KillParameters,
     KillResult,
     KillResultStatus,
@@ -42,38 +45,38 @@
 from dbt.logger import LogMessage
 from dbt_rpc.rpc.error import dbt_error, RPCException
 from dbt_rpc.rpc.method import RemoteBuiltinMethod
 from dbt_rpc.rpc.task_handler import RequestTaskHandler
 
 
 class GC(RemoteBuiltinMethod[GCParameters, GCResult]):
-    METHOD_NAME = 'gc'
+    METHOD_NAME = "gc"
 
     def set_args(self, params: GCParameters):
         super().set_args(params)
 
     def handle_request(self) -> GCResult:
         if self.params is None:
-            raise dbt.exceptions.InternalException('GC: params not set')
+            raise dbt.exceptions.DbtInternalError("GC: params not set")
         return self.task_manager.gc_safe(
             task_ids=self.params.task_ids,
             before=self.params.before,
             settings=self.params.settings,
         )
 
 
 class Kill(RemoteBuiltinMethod[KillParameters, KillResult]):
-    METHOD_NAME = 'kill'
+    METHOD_NAME = "kill"
 
     def set_args(self, params: KillParameters):
         super().set_args(params)
 
     def handle_request(self) -> KillResult:
         if self.params is None:
-            raise dbt.exceptions.InternalException('Kill: params not set')
+            raise dbt.exceptions.DbtInternalError("Kill: params not set")
         result = KillResult()
         task: RequestTaskHandler
         try:
             task = self.task_manager.get_request(self.params.task_id)
         except dbt.exceptions.UnknownAsyncIDException:
             # nothing to do!
             return result
@@ -95,66 +98,67 @@
             result.state = KillResultStatus.Finished
             # the state must be "Completed"
 
         return result
 
 
 class Status(RemoteBuiltinMethod[StatusParameters, LastParse]):
-    METHOD_NAME = 'status'
+    METHOD_NAME = "status"
 
     def set_args(self, params: StatusParameters):
         super().set_args(params)
 
     def handle_request(self) -> LastParse:
         return self.task_manager.last_parse
 
 
 class PS(RemoteBuiltinMethod[PSParameters, PSResult]):
-    METHOD_NAME = 'ps'
+    METHOD_NAME = "ps"
 
     def set_args(self, params: PSParameters):
         super().set_args(params)
 
     def keep(self, row: TaskRow):
         if self.params is None:
-            raise dbt.exceptions.InternalException('PS: params not set')
+            raise dbt.exceptions.DbtInternalError("PS: params not set")
         if row.state.finished and self.params.completed:
             return True
         elif not row.state.finished and self.params.active:
             return True
         else:
             return False
 
     def handle_request(self) -> PSResult:
-        rows = [
-            row for row in self.task_manager.task_table() if self.keep(row)
-        ]
+        rows = [row for row in self.task_manager.task_table() if self.keep(row)]
         rows.sort(key=lambda r: (r.state, r.start, r.method))
         result = PSResult(rows=rows, logs=[])
         return result
 
 
 def poll_complete(
     timing: TaskTiming, result: Any, tags: TaskTags, logs: List[LogMessage]
 ) -> PollResult:
     if timing.state not in (TaskHandlerState.Success, TaskHandlerState.Failed):
-        raise dbt.exceptions.InternalException(
-            f'got invalid result state in poll_complete: {timing.state}'
+        raise dbt.exceptions.DbtInternalError(
+            f"got invalid result state in poll_complete: {timing.state}"
         )
 
-    cls: Type[Union[
-        PollExecuteCompleteResult,
-        PollRunCompleteResult,
-        PollCompileCompleteResult,
-        PollCatalogCompleteResult,
-        PollRemoteEmptyCompleteResult,
-        PollRunOperationCompleteResult,
-        PollGetManifestResult,
-        PollFreshnessResult,
-    ]]
+    cls: Type[
+        Union[
+            PollExecuteCompleteResult,
+            PollRunCompleteResult,
+            PollCompileCompleteResult,
+            PollCatalogCompleteResult,
+            PollRemoteEmptyCompleteResult,
+            PollRunOperationCompleteResult,
+            PollGetManifestResult,
+            PollFreshnessResult,
+            PollListResult,
+        ]
+    ]
 
     if isinstance(result, RemoteExecutionResult):
         cls = PollExecuteCompleteResult
     # order matters here, as RemoteRunResult subclasses RemoteCompileResult
     elif isinstance(result, RemoteRunResult):
         cls = PollRunCompleteResult
     elif isinstance(result, RemoteCompileResult):
@@ -165,34 +169,36 @@
         cls = PollRemoteEmptyCompleteResult
     elif isinstance(result, RemoteRunOperationResult):
         cls = PollRunOperationCompleteResult
     elif isinstance(result, GetManifestResult):
         cls = PollGetManifestResult
     elif isinstance(result, RemoteFreshnessResult):
         cls = PollFreshnessResult
+    elif isinstance(result, RemoteListResults):
+        cls = PollListResult
     else:
-        raise dbt.exceptions.InternalException(
-            'got invalid result in poll_complete: {}'.format(result)
+        raise dbt.exceptions.DbtInternalError(
+            "got invalid result in poll_complete: {}".format(result)
         )
     return cls.from_result(result, tags, timing, logs)
 
 
 def _dict_logs(logs: List[LogMessage]) -> List[Dict[str, Any]]:
     return [log.to_dict(omit_none=True) for log in logs]
 
 
 class Poll(RemoteBuiltinMethod[PollParameters, PollResult]):
-    METHOD_NAME = 'poll'
+    METHOD_NAME = "poll"
 
     def set_args(self, params: PollParameters):
         super().set_args(params)
 
     def handle_request(self) -> PollResult:
         if self.params is None:
-            raise dbt.exceptions.InternalException('Poll: params not set')
+            raise dbt.exceptions.DbtInternalError("Poll: params not set")
         task_id = self.params.request_token
         task: RequestTaskHandler = self.task_manager.get_request(task_id)
 
         task_logs: List[LogMessage] = []
         if self.params.logs:
             task_logs = task.logs[self.params.logs_start:]
 
@@ -211,48 +217,52 @@
                 start=timing.start,
                 end=timing.end,
                 elapsed=timing.elapsed,
             )
         elif state == TaskHandlerState.Error:
             err = task.error
             if err is None:
-                exc = dbt.exceptions.InternalException(
-                    f'At end of task {task_id}, error state but error is None'
+                exc = dbt.exceptions.DbtInternalError(
+                    f"At end of task {task_id}, error state but error is None"
                 )
                 raise RPCException.from_error(
                     dbt_error(exc, logs=_dict_logs(task_logs))
                 )
             # the exception has logs already attached from the child, don't
             # overwrite those
             raise err
         elif state in (TaskHandlerState.Success, TaskHandlerState.Failed):
-
             if task.result is None:
-                exc = dbt.exceptions.InternalException(
-                    f'At end of task {task_id}, state={state} but result is '
-                    'None'
+                exc = dbt.exceptions.DbtInternalError(
+                    f"At end of task {task_id}, state={state} but result is " "None"
                 )
                 raise RPCException.from_error(
                     dbt_error(exc, logs=_dict_logs(task_logs))
                 )
             return poll_complete(
-                timing=timing,
-                result=task.result,
-                tags=task.tags,
-                logs=task_logs
+                timing=timing, result=task.result, tags=task.tags, logs=task_logs
             )
         elif state == TaskHandlerState.Killed:
             return PollKilledResult(
                 tags=task.tags,
                 logs=task_logs,
                 state=timing.state,
                 start=timing.start,
                 end=timing.end,
                 elapsed=timing.elapsed,
             )
         else:
-            exc = dbt.exceptions.InternalException(
-                f'Got unknown value state={state} for task {task_id}'
-            )
-            raise RPCException.from_error(
-                dbt_error(exc, logs=_dict_logs(task_logs))
+            exc = dbt.exceptions.DbtInternalError(
+                f"Got unknown value state={state} for task {task_id}"
             )
+            raise RPCException.from_error(dbt_error(exc, logs=_dict_logs(task_logs)))
+
+
+class Reload(RemoteBuiltinMethod[ReloadParameters, None]):
+    METHOD_NAME = "reload"
+
+    def set_args(self, params: ReloadParameters):
+        super().set_args(params)
+
+    def handle_request(self) -> None:
+        os.kill(os.getpid(), signal.SIGHUP)
+        return os.getpid()
```

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/error.py` & `dbt-rpc-0.4.1/dbt_rpc/rpc/error.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/gc.py` & `dbt-rpc-0.4.1/dbt_rpc/rpc/gc.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         You must hold the lock, as this mutates `tasks`.
         """
         try:
             state = self._remove_task_if_finished(task_id)
         except KeyError:
             # someone was mutating tasks while we had the lock, that's
             # not right!
-            raise dbt.exceptions.InternalException(
+            raise dbt.exceptions.DbtInternalError(
                 'Got a KeyError for task uuid={} during gc'
                 .format(task_id)
             )
 
         return result.add_result(task_id=task_id, state=state)
 
     def collect_multiple_task_ids(
```

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/logger.py` & `dbt-rpc-0.4.1/dbt_rpc/rpc/logger.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/method.py` & `dbt-rpc-0.4.1/dbt_rpc/rpc/method.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/node_runners.py` & `dbt-rpc-0.4.1/dbt_rpc/rpc/node_runners.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/response_manager.py` & `dbt-rpc-0.4.1/dbt_rpc/rpc/response_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         elif isinstance(handler, RemoteMethod):
             # the handler must be a task. Wrap it in a task handler so it can
             # go async
             return RequestTaskHandler(
                 self.manager, handler, self.http_request, self.json_rpc_request
             )
         else:
-            raise dbt.exceptions.InternalException(
+            raise dbt.exceptions.DbtInternalError(
                 f'Got an invalid handler from get_handler. Expected None, '
                 f'callable, or RemoteMethod, got {handler}'
             )
 
 
 class ResponseManager(JSONRPCResponseManager):
     """Override the default response manager to handle request metadata and
```

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/task_handler.py` & `dbt-rpc-0.4.1/dbt_rpc/rpc/task_handler.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/task_handler_protocol.py` & `dbt-rpc-0.4.1/dbt_rpc/rpc/task_handler_protocol.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,22 +38,22 @@
 
     @property
     def tags(self) -> Optional[TaskTags]:
         pass
 
     def _assert_started(self) -> datetime:
         if self.started is None:
-            raise dbt.exceptions.InternalException(
+            raise dbt.exceptions.DbtInternalError(
                 'task handler started but start time is not set'
             )
         return self.started
 
     def _assert_ended(self) -> datetime:
         if self.ended is None:
-            raise dbt.exceptions.InternalException(
+            raise dbt.exceptions.DbtInternalError(
                 'task handler finished but end time is not set'
             )
         return self.ended
 
     def make_task_timing(
         self, now_time: datetime
     ) -> TaskTiming:
```

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/task_manager.py` & `dbt-rpc-0.4.1/dbt_rpc/rpc/task_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         state = self.last_parse.state
         if state == ManifestStatus.Compiling:
             return CurrentlyCompiling()
         elif state == ManifestStatus.Error:
             return ParseError(self.last_parse.error)
         else:
             if self.manifest is None:
-                raise dbt.exceptions.InternalException(
+                raise dbt.exceptions.DbtInternalError(
                     f'Manifest should not be None if the last parse state is '
                     f'{state}'
                 )
             return task(deepcopy(self.args), self.config, self.manifest)
 
     def rpc_task(
         self, method_name: str
@@ -175,15 +175,15 @@
             if issubclass(task, RemoteBuiltinMethod):
                 return task(self)
             elif issubclass(task, RemoteManifestMethod):
                 return self._get_manifest_callable(task)
             elif issubclass(task, RemoteMethod):
                 return task(deepcopy(self.args), self.config)
             else:
-                raise dbt.exceptions.InternalException(
+                raise dbt.exceptions.DbtInternalError(
                     f'Got a task with an invalid type! {task} with method '
                     f'name {method_name} has a type of {task.__class__}, '
                     f'should be a RemoteMethod'
                 )
 
     def ready(self) -> bool:
         with self._lock:
```

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/task/base.py` & `dbt-rpc-0.4.1/dbt_rpc/task/base.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/task/cli.py` & `dbt-rpc-0.4.1/dbt_rpc/task/cli.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/task/deps.py` & `dbt-rpc-0.4.1/dbt_rpc/task/deps.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/task/project_commands.py` & `dbt-rpc-0.4.1/dbt_rpc/task/project_commands.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/task/server.py` & `dbt-rpc-0.4.1/dbt_rpc/task/server.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc/task/sql_commands.py` & `dbt-rpc-0.4.1/dbt_rpc/task/sql_commands.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc.egg-info/PKG-INFO` & `dbt-rpc-0.4.1/dbt_rpc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-rpc
-Version: 0.4.0rc1
+Version: 0.4.1
 Summary:  A JSON RPC server that provides an interface to programmically interact with dbt projects. 
 Home-page: https://github.com/dbt-labs/dbt-rpc
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-rpc-0.4.0rc1/dbt_rpc.egg-info/SOURCES.txt` & `dbt-rpc-0.4.1/dbt_rpc.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,17 @@
 dbt_rpc/task/server.py
 dbt_rpc/task/sql_commands.py
 tests/test_build.py
 tests/test_compile.py
 tests/test_compile_sql.py
 tests/test_concurrency.py
 tests/test_deps.py
+tests/test_list.py
 tests/test_management.py
+tests/test_reload.py
 tests/test_run.py
 tests/test_run_operation.py
 tests/test_run_sql.py
 tests/test_seed.py
 tests/test_snapshots.py
 tests/test_source_freshness.py
 tests/test_test.py
```

### Comparing `dbt-rpc-0.4.0rc1/tests/test_build.py` & `dbt-rpc-0.4.1/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/tests/test_compile.py` & `dbt-rpc-0.4.1/tests/test_compile.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/tests/test_compile_sql.py` & `dbt-rpc-0.4.1/tests/test_compile_sql.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/tests/test_concurrency.py` & `dbt-rpc-0.4.1/tests/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/tests/test_deps.py` & `dbt-rpc-0.4.1/tests/test_deps.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/tests/test_management.py` & `dbt-rpc-0.4.1/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/tests/test_run.py` & `dbt-rpc-0.4.1/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/tests/test_run_operation.py` & `dbt-rpc-0.4.1/tests/test_run_operation.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/tests/test_run_sql.py` & `dbt-rpc-0.4.1/tests/test_run_sql.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/tests/test_seed.py` & `dbt-rpc-0.4.1/tests/test_seed.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/tests/test_snapshots.py` & `dbt-rpc-0.4.1/tests/test_snapshots.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/tests/test_source_freshness.py` & `dbt-rpc-0.4.1/tests/test_source_freshness.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0rc1/tests/test_test.py` & `dbt-rpc-0.4.1/tests/test_test.py`

 * *Files identical despite different names*

