# Comparing `tmp/th2_data_services-2.0.0.dev4892029505.tar.gz` & `tmp/th2_data_services-2.0.0.dev4925844112.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services-2.0.0.dev4892029505.tar", last modified: Fri May  5 09:41:52 2023, max compression
+gzip compressed data, was "dist/th2_data_services-2.0.0.dev4925844112.tar", last modified: Tue May  9 12:51:14 2023, max compression
```

## Comparing `th2_data_services-2.0.0.dev4892029505.tar` & `th2_data_services-2.0.0.dev4925844112.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 09:41:52.000000 th2_data_services-2.0.0.dev4892029505/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)   614698 2023-05-05 09:41:52.000000 th2_data_services-2.0.0.dev4892029505/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)   510907 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-05 09:41:29.000000 th2_data_services-2.0.0.dev4892029505/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-05 09:41:52.000000 th2_data_services-2.0.0.dev4892029505/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 09:41:52.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 09:41:52.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/config/
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/config/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    29341 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 09:41:52.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      806 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/event_tree/etc_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/event_tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/event_tree/event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/event_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/event_tree/parent_event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 09:41:52.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      706 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 09:41:52.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2705 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/utils/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 09:41:52.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     3360 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/_json.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     8635 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/aggregation_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    15216 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/az_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/categorizers.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/category.py
--rw-r--r--   0 runner    (1001) docker     (122)     3296 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)      908 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/decode_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 09:41:52.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/event_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/event_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/event_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/event_utils/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/event_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/event_utils/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     6805 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/event_utils/totals.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 09:41:52.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/message_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/message_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/message_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    14456 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/message_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    15739 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     8331 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/perfect_table.py
--rw-r--r--   0 runner    (1001) docker     (122)    33801 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/script_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/sse_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5285 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     6717 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/total_category_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 09:41:52.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/viewer_structs/
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/viewer_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-05-05 09:39:25.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/viewer_structs/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 09:41:52.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)   614698 2023-05-05 09:41:52.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2306 2023-05-05 09:41:52.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 09:41:52.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-05-05 09:41:52.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-05 09:41:52.000000 th2_data_services-2.0.0.dev4892029505/th2_data_services.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:51:14.000000 th2_data_services-2.0.0.dev4925844112/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)   614698 2023-05-09 12:51:14.000000 th2_data_services-2.0.0.dev4925844112/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)   510907 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-09 12:50:44.000000 th2_data_services-2.0.0.dev4925844112/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 12:51:14.000000 th2_data_services-2.0.0.dev4925844112/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:51:14.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:51:14.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29341 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:51:14.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/event_tree/etc_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/event_tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/event_tree/event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/event_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/event_tree/parent_event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:51:14.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:51:14.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2705 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/utils/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:51:14.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     3360 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16102 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/aggregation_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15216 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/az_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/categorizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/category.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3296 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      908 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/decode_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:51:14.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/event_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/event_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/event_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/event_utils/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/event_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/event_utils/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6805 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/event_utils/totals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:51:14.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/message_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/message_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/message_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14456 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/message_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15739 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10292 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/perfect_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33801 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/script_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/sse_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5285 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6399 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/total_category_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:51:14.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/viewer_structs/
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/viewer_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-05-09 12:49:15.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/viewer_structs/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:51:14.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)   614698 2023-05-09 12:51:13.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2306 2023-05-09 12:51:14.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 12:51:13.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-05-09 12:51:13.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-09 12:51:13.000000 th2_data_services-2.0.0.dev4925844112/th2_data_services.egg-info/top_level.txt
```

### Comparing `th2_data_services-2.0.0.dev4892029505/PKG-INFO` & `th2_data_services-2.0.0.dev4925844112/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 325f  : 2.1.Name: th2_
 00000020: 6461 7461 5f73 6572 7669 6365 730a 5665  data_services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3438 3932 3032 3935 3035 0a53 756d 6d61  4892029505.Summa
+00000040: 3439 3235 3834 3431 3132 0a53 756d 6d61  4925844112.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev4892029505/README.md` & `th2_data_services-2.0.0.dev4925844112/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/setup.py` & `th2_data_services-2.0.0.dev4925844112/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/config/__init__.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/config/config.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/config/config.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/data.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/data.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/event_tree/__init__.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/event_tree/etc_driver.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/event_tree/etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/event_tree/event_tree.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/event_tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/event_tree/event_tree_collection.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/event_tree/event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/event_tree/exceptions.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/event_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/event_tree/parent_event_tree_collection.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/event_tree/parent_event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/exceptions.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/__init__.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/adapter.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/command.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/data_source.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/source_api.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/struct.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/stub_builder.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/utils/__init__.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/utils/converter.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/utils/converter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/interfaces/utils/resolver.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/interfaces/utils/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/_json.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/_json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/_types.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/_types.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/az_tree.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/az_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/categorizers.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/categorizers.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/category.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/category.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/converters.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/converters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/decode_error_handler.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/decode_error_handler.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/display.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/event_utils/__init__.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/event_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/event_utils/display.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/event_utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/event_utils/event_utils.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/event_utils/event_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/event_utils/frequencies.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/event_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/event_utils/select.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/event_utils/select.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/event_utils/totals.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/event_utils/totals.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/experimental.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/experimental.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/message_utils/__init__.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/message_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/message_utils/frequencies.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/message_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/message_utils/message_utils.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/message_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/misc_utils.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/perfect_table.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/perfect_table.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 
 
 def namedtuple_with_slice(name, args):  # noqa
     args_dict = {arg: pars_arg(arg) for arg in args}
     new_args = [pars_arg(arg) for arg in args]
     cls = namedtuple(name, new_args)  # TODO - we can have the same values!!!
 
+    # TODO - I think we don't need getitem for strings. (strings column names.
+    #  We would not do `row.abc` but we often have abc like 'a b 123 c' so it's not a problem.
+    #  It means we don't need named tuples more
+    #   We need to get only via item NOT ATTRIBUTE
     def getitem(self, index):
         # `type(self)` can result in issues in case of multiple inheritance.
         # But shouldn't be an issue here.
         if isinstance(index, int):
             value = super(type(self), self).__getitem__(index)  # Superclass for namedtuple is sequence
         elif isinstance(index, slice):
             value = super(type(self), self).__getitem__(index)
@@ -49,25 +53,78 @@
             # raise Exception('I dont can stings now')
         return value
 
     cls.__getitem__ = getitem
     return cls
 
 
+class RowBase(tuple):
+    _column_idx = {}  # {COL_NAME: index}
+
+    def __new__(cls, *args: list):
+        if not cls._column_idx:
+            raise Exception("Row class is not initialized.")
+
+        return super().__new__(cls, args)
+
+    def __init__(self, *args: list):  # noqa
+        if len(self._column_idx) != len(args):
+            raise Exception(
+                f"The number of provided values '{len(args)}' != the number of columns '{len(self._column_idx)}'"
+            )
+        super().__init__()
+
+    @property
+    def keys(self):
+        return self._column_idx.keys()
+
+    def _get_idx(self, col_name) -> int:
+        try:
+            return self._column_idx[col_name]
+        except KeyError:
+            raise Exception(f"Row class doesn't have '{col_name}' column")
+
+    def __getitem__(self, index):
+        # `type(self)` can result in issues in case of multiple inheritance.
+        # But shouldn't be an issue here.
+        if isinstance(index, int):
+            value = super().__getitem__(index)
+            # elif isinstance(index, slice):
+        #     new_column_idx =
+        #     value = self.__getitem__(index)
+        #     cls = namedtuple(name, new_args[index])
+        #     cls.__getitem__ = getitem
+        #     value = cls(*value)
+        elif isinstance(index, str):
+            value = self[self._get_idx(index)]
+        else:
+            raise Exception("Some unexpected situation")
+
+        return value
+
+
+def row_cls_init(name, args):
+    """Init RowBase."""
+    cls = type(name, (RowBase,), {})
+    cls._column_idx = {k: idx for idx, k in enumerate(args)}
+    return cls
+
+
 # TODO - this table should be placed to another repo in the future.
 class PerfectTable:
     def __init__(self, header: List[str]):  # noqa
         self._headers = tuple(header)
-        self.row_class = self._create_row_class(self._headers)
+        self.row_class: RowBase = self._create_row_class(self._headers)
         self._rows = []
         self._columns = defaultdict(tuple)
         # self._add_headers_as_attr()
 
-    def _create_row_class(self, headers):
-        return namedtuple_with_slice("Row", headers)
+    def _create_row_class(self, headers) -> RowBase:
+        # return namedtuple_with_slice("Row", headers)
+        return row_cls_init("Row", headers)
 
     def __contains__(self, item):
         return item in self._headers
 
     def __iter__(self):
         return iter(self._rows)
```

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/script_report_utils.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/script_report_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/sse_client.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/time.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/time.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/total_category_calculator.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/total_category_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,15 @@
 
 
 # First you need to pull out all the metrics, and only then connect
 
 
 class TotalCategoryCalculator:
     def __init__(self, categories: List[Category], combinations: Union[List[Sequence[str]], List[Sequence[Category]]]):
-        """
-        Calculates, aggregates to tables and prints categories combinations.
+        """Calculates, aggregates to tables and prints categories combinations.
 
         This class allows you to calculate any metrics and their combinations in stream-like way.
 
         It does not accumulate all data in memory.
         Keeps calculated metrics only.
 
         categories: [Category('a'), Category(b)]
@@ -143,41 +142,30 @@
 
         # concat them  == values
 
         for v in self.combinations:  # v = ['session', 'direction']
             val_for_counter = tuple([metric_values[metric] for metric in v])
             self._counters[v].update([val_for_counter])
 
-    def get_table(self, combination: CategoryCombination, add_total=False) -> TotalCategoryTable:
+    def get_table(self, combination: CategoryCombination) -> TotalCategoryTable:
         """Returns a PrettyTable class for certain combination.
 
         Args:
             combination: Union[Tuple[str], List[str]]
             add_total: If True, adds total value in the last line.
 
         """
         combination = self._prepare_combination(combination)
 
         t = PrettyTable()
         t.field_names = [*combination, self.counter_field_name]
         c = self._get_counter(combination)
 
-        if add_total:
-            total_val = 0
-
-            for key, cnt in c.items():
-                t.add_row([*key, cnt])
-                total_val += cnt
-
-            # Add total row.
-            t.add_row([*["" for _ in combination], total_val])
-
-        else:
-            for key, cnt in c.items():
-                t.add_row([*key, cnt])
+        for key, cnt in c.items():
+            t.add_row([*key, cnt])
 
         return TotalCategoryTable(header=t.field_names, rows=t.rows).sort_by([self.counter_field_name], ascending=False)
 
     def show(self):
         """Prints all tables.
 
         Sorted by cnt.
@@ -215,9 +203,9 @@
     for m in messages:
         sc.append(m)
 
     sc.show()
 
     print(time.time() - t1)
 
-    print(sc.get_table(["direction", "messageType", session_m], add_total=True))
+    print(sc.get_table(["direction", "messageType", session_m]))
     print(time.time() - t1)
```

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/viewer_structs/__init__.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/viewer_structs/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services/utils/viewer_structs/verification.py` & `th2_data_services-2.0.0.dev4925844112/th2_data_services/utils/viewer_structs/verification.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services.egg-info/PKG-INFO` & `th2_data_services-2.0.0.dev4925844112/th2_data_services.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 322d  : 2.1.Name: th2-
 00000020: 6461 7461 2d73 6572 7669 6365 730a 5665  data-services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3438 3932 3032 3935 3035 0a53 756d 6d61  4892029505.Summa
+00000040: 3439 3235 3834 3431 3132 0a53 756d 6d61  4925844112.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services.egg-info/SOURCES.txt` & `th2_data_services-2.0.0.dev4925844112/th2_data_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4892029505/th2_data_services.egg-info/requires.txt` & `th2_data_services-2.0.0.dev4925844112/th2_data_services.egg-info/requires.txt`

 * *Files identical despite different names*

