# Comparing `tmp/spaceone-notification-1.11.0.tar.gz` & `tmp/spaceone-notification-1.12.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaceone-notification-1.11.0.tar", last modified: Tue May  9 01:04:19 2023, max compression
+gzip compressed data, was "spaceone-notification-1.12.dev3.tar", last modified: Tue May  9 02:42:48 2023, max compression
```

## Comparing `spaceone-notification-1.11.0.tar` & `spaceone-notification-1.12.dev3.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:19.095878 spaceone-notification-1.11.0/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-09 01:04:19.091878 spaceone-notification-1.11.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 01:04:19.095878 spaceone-notification-1.11.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:19.071877 spaceone-notification-1.11.0/spaceone/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:19.071877 spaceone-notification-1.11.0/spaceone/notification/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:19.071877 spaceone-notification-1.11.0/spaceone/notification/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/conf/global_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/conf/proto_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/conf/protocol_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:19.075877 spaceone-notification-1.11.0/spaceone/notification/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/connector/identity_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/connector/notification_plugin_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/connector/plugin_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/connector/repository_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/connector/secret_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:19.075877 spaceone-notification-1.11.0/spaceone/notification/error/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/error/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/error/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/error/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/error/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/error/quota.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:19.079877 spaceone-notification-1.11.0/spaceone/notification/info/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/info/common_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/info/notification_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/info/notification_usage_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/info/project_channel_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/info/protocol_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/info/quota_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/info/user_channel_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:19.079877 spaceone-notification-1.11.0/spaceone/notification/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:19.079877 spaceone-notification-1.11.0/spaceone/notification/interface/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/interface/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:19.083877 spaceone-notification-1.11.0/spaceone/notification/interface/grpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/interface/grpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/interface/grpc/v1/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/interface/grpc/v1/notification_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/interface/grpc/v1/project_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/interface/grpc/v1/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/interface/grpc/v1/quota.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/interface/grpc/v1/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:19.083877 spaceone-notification-1.11.0/spaceone/notification/interface/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/interface/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:19.083877 spaceone-notification-1.11.0/spaceone/notification/interface/task/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/interface/task/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/interface/task/v1/delete_old_notification_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:19.083877 spaceone-notification-1.11.0/spaceone/notification/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/lib/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/lib/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:19.087878 spaceone-notification-1.11.0/spaceone/notification/manager/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/manager/identity_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/manager/notification_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/manager/notification_usage_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/manager/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/manager/project_channel_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/manager/protocol_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/manager/quota_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/manager/repository_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/manager/secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/manager/user_channel_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:19.091878 spaceone-notification-1.11.0/spaceone/notification/model/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/model/notification_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/model/notification_usage_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/model/project_channel_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/model/protocol_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/model/quota_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/model/schedule_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/model/user_channel_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:19.091878 spaceone-notification-1.11.0/spaceone/notification/service/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22978 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/service/notification_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/service/notification_usage_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/service/project_channel_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/service/protocol_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/service/quota_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-05-09 01:04:02.000000 spaceone-notification-1.11.0/spaceone/notification/service/user_channel_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:04:19.091878 spaceone-notification-1.11.0/spaceone_notification.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-09 01:04:18.000000 spaceone-notification-1.11.0/spaceone_notification.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-09 01:04:19.000000 spaceone-notification-1.11.0/spaceone_notification.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 01:04:18.000000 spaceone-notification-1.11.0/spaceone_notification.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 01:04:18.000000 spaceone-notification-1.11.0/spaceone_notification.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-09 01:04:18.000000 spaceone-notification-1.11.0/spaceone_notification.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 01:04:18.000000 spaceone-notification-1.11.0/spaceone_notification.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:48.679275 spaceone-notification-1.12.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-09 02:42:48.679275 spaceone-notification-1.12.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 02:42:48.679275 spaceone-notification-1.12.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:48.671275 spaceone-notification-1.12.dev3/spaceone/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:48.671275 spaceone-notification-1.12.dev3/spaceone/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:48.671275 spaceone-notification-1.12.dev3/spaceone/notification/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/conf/global_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/conf/proto_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/conf/protocol_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:48.671275 spaceone-notification-1.12.dev3/spaceone/notification/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/connector/identity_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/connector/notification_plugin_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/connector/plugin_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/connector/repository_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/connector/secret_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:48.671275 spaceone-notification-1.12.dev3/spaceone/notification/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/error/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/error/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/error/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/error/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/error/quota.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:48.671275 spaceone-notification-1.12.dev3/spaceone/notification/info/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/info/common_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/info/notification_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/info/notification_usage_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/info/project_channel_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/info/protocol_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/info/quota_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/info/user_channel_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:48.671275 spaceone-notification-1.12.dev3/spaceone/notification/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:48.671275 spaceone-notification-1.12.dev3/spaceone/notification/interface/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/interface/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:48.675275 spaceone-notification-1.12.dev3/spaceone/notification/interface/grpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/interface/grpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/interface/grpc/v1/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/interface/grpc/v1/notification_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/interface/grpc/v1/project_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/interface/grpc/v1/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/interface/grpc/v1/quota.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/interface/grpc/v1/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:48.675275 spaceone-notification-1.12.dev3/spaceone/notification/interface/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/interface/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:48.675275 spaceone-notification-1.12.dev3/spaceone/notification/interface/task/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/interface/task/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/interface/task/v1/delete_old_notification_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:48.675275 spaceone-notification-1.12.dev3/spaceone/notification/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/lib/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/lib/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:48.675275 spaceone-notification-1.12.dev3/spaceone/notification/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/manager/identity_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/manager/notification_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/manager/notification_usage_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/manager/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/manager/project_channel_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/manager/protocol_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/manager/quota_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/manager/repository_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/manager/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/manager/user_channel_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:48.675275 spaceone-notification-1.12.dev3/spaceone/notification/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/model/notification_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/model/notification_usage_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/model/project_channel_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/model/protocol_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/model/quota_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/model/schedule_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/model/user_channel_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:48.675275 spaceone-notification-1.12.dev3/spaceone/notification/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22978 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/service/notification_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/service/notification_usage_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/service/project_channel_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/service/protocol_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/service/quota_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-05-09 02:42:38.000000 spaceone-notification-1.12.dev3/spaceone/notification/service/user_channel_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:42:48.679275 spaceone-notification-1.12.dev3/spaceone_notification.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-09 02:42:48.000000 spaceone-notification-1.12.dev3/spaceone_notification.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-09 02:42:48.000000 spaceone-notification-1.12.dev3/spaceone_notification.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 02:42:48.000000 spaceone-notification-1.12.dev3/spaceone_notification.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 02:42:48.000000 spaceone-notification-1.12.dev3/spaceone_notification.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-09 02:42:48.000000 spaceone-notification-1.12.dev3/spaceone_notification.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 02:42:48.000000 spaceone-notification-1.12.dev3/spaceone_notification.egg-info/top_level.txt
```

### Comparing `spaceone-notification-1.11.0/setup.py` & `spaceone-notification-1.12.dev3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,24 +9,20 @@
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
-
+import os
 from setuptools import setup, find_packages
 
-with open('VERSION', 'r') as f: 
-    VERSION = f.read().strip()
-    f.close()
-
 setup(
     name='spaceone-notification',
-    version=VERSION,
+    version=os.environ.get('PACKAGE_VERSION'),
     description='SpaceONE notification service',
     long_description='',
     url='https://www.spaceone.dev/',
     author='MEGAZONE SpaceONE Team',
     author_email='admin@spaceone.dev',
     license='Apache License 2.0',
     packages=find_packages(),
```

### Comparing `spaceone-notification-1.11.0/spaceone/notification/conf/global_conf.py` & `spaceone-notification-1.12.dev3/spaceone/notification/conf/global_conf.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/connector/identity_connector.py` & `spaceone-notification-1.12.dev3/spaceone/notification/connector/identity_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/connector/notification_plugin_connector.py` & `spaceone-notification-1.12.dev3/spaceone/notification/connector/notification_plugin_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/connector/plugin_connector.py` & `spaceone-notification-1.12.dev3/spaceone/notification/connector/plugin_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/connector/repository_connector.py` & `spaceone-notification-1.12.dev3/spaceone/notification/connector/repository_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/connector/secret_connector.py` & `spaceone-notification-1.12.dev3/spaceone/notification/connector/secret_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/error/channel.py` & `spaceone-notification-1.12.dev3/spaceone/notification/error/channel.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/error/plugin.py` & `spaceone-notification-1.12.dev3/spaceone/notification/error/plugin.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/error/protocol.py` & `spaceone-notification-1.12.dev3/spaceone/notification/error/protocol.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/info/notification_info.py` & `spaceone-notification-1.12.dev3/spaceone/notification/info/notification_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/info/notification_usage_info.py` & `spaceone-notification-1.12.dev3/spaceone/notification/info/notification_usage_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/info/project_channel_info.py` & `spaceone-notification-1.12.dev3/spaceone/notification/info/project_channel_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/info/protocol_info.py` & `spaceone-notification-1.12.dev3/spaceone/notification/info/protocol_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/info/quota_info.py` & `spaceone-notification-1.12.dev3/spaceone/notification/info/quota_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/info/user_channel_info.py` & `spaceone-notification-1.12.dev3/spaceone/notification/info/user_channel_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/interface/grpc/v1/notification.py` & `spaceone-notification-1.12.dev3/spaceone/notification/interface/grpc/v1/notification.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/interface/grpc/v1/notification_usage.py` & `spaceone-notification-1.12.dev3/spaceone/notification/interface/grpc/v1/notification_usage.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/interface/grpc/v1/project_channel.py` & `spaceone-notification-1.12.dev3/spaceone/notification/interface/grpc/v1/project_channel.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/interface/grpc/v1/protocol.py` & `spaceone-notification-1.12.dev3/spaceone/notification/interface/grpc/v1/protocol.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/interface/grpc/v1/quota.py` & `spaceone-notification-1.12.dev3/spaceone/notification/interface/grpc/v1/quota.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/interface/grpc/v1/user_channel.py` & `spaceone-notification-1.12.dev3/spaceone/notification/interface/grpc/v1/user_channel.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/interface/task/v1/delete_old_notification_scheduler.py` & `spaceone-notification-1.12.dev3/spaceone/notification/interface/task/v1/delete_old_notification_scheduler.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/lib/schedule.py` & `spaceone-notification-1.12.dev3/spaceone/notification/lib/schedule.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/manager/__init__.py` & `spaceone-notification-1.12.dev3/spaceone/notification/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/manager/identity_manager.py` & `spaceone-notification-1.12.dev3/spaceone/notification/manager/identity_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/manager/notification_manager.py` & `spaceone-notification-1.12.dev3/spaceone/notification/manager/notification_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/manager/notification_usage_manager.py` & `spaceone-notification-1.12.dev3/spaceone/notification/manager/notification_usage_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/manager/plugin_manager.py` & `spaceone-notification-1.12.dev3/spaceone/notification/manager/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/manager/project_channel_manager.py` & `spaceone-notification-1.12.dev3/spaceone/notification/manager/project_channel_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/manager/protocol_manager.py` & `spaceone-notification-1.12.dev3/spaceone/notification/manager/protocol_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/manager/quota_manager.py` & `spaceone-notification-1.12.dev3/spaceone/notification/manager/quota_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/manager/repository_manager.py` & `spaceone-notification-1.12.dev3/spaceone/notification/manager/repository_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/manager/secret_manager.py` & `spaceone-notification-1.12.dev3/spaceone/notification/manager/secret_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/manager/user_channel_manager.py` & `spaceone-notification-1.12.dev3/spaceone/notification/manager/user_channel_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/model/notification_model.py` & `spaceone-notification-1.12.dev3/spaceone/notification/model/notification_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/model/notification_usage_model.py` & `spaceone-notification-1.12.dev3/spaceone/notification/model/notification_usage_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/model/project_channel_model.py` & `spaceone-notification-1.12.dev3/spaceone/notification/model/project_channel_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/model/protocol_model.py` & `spaceone-notification-1.12.dev3/spaceone/notification/model/protocol_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/model/quota_model.py` & `spaceone-notification-1.12.dev3/spaceone/notification/model/quota_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/model/user_channel_model.py` & `spaceone-notification-1.12.dev3/spaceone/notification/model/user_channel_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/service/notification_service.py` & `spaceone-notification-1.12.dev3/spaceone/notification/service/notification_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/service/notification_usage_service.py` & `spaceone-notification-1.12.dev3/spaceone/notification/service/notification_usage_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/service/project_channel_service.py` & `spaceone-notification-1.12.dev3/spaceone/notification/service/project_channel_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/service/protocol_service.py` & `spaceone-notification-1.12.dev3/spaceone/notification/service/protocol_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/service/quota_service.py` & `spaceone-notification-1.12.dev3/spaceone/notification/service/quota_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone/notification/service/user_channel_service.py` & `spaceone-notification-1.12.dev3/spaceone/notification/service/user_channel_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-1.11.0/spaceone_notification.egg-info/SOURCES.txt` & `spaceone-notification-1.12.dev3/spaceone_notification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

