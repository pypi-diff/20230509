# Comparing `tmp/strongmind-platform-sdk-2.7.0.tar.gz` & `tmp/strongmind-platform-sdk-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strongmind-platform-sdk-2.7.0.tar", last modified: Thu Apr 13 23:24:40 2023, max compression
+gzip compressed data, was "strongmind-platform-sdk-2.8.1.tar", last modified: Mon May  8 22:49:03 2023, max compression
```

## Comparing `strongmind-platform-sdk-2.7.0.tar` & `strongmind-platform-sdk-2.8.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:24:40.432107 strongmind-platform-sdk-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-13 23:24:40.432107 strongmind-platform-sdk-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:24:40.424107 strongmind-platform-sdk-2.7.0/platform_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:24:40.424107 strongmind-platform-sdk-2.7.0/platform_sdk/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/clients/events_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/clients/identity_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/clients/mapper_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/clients/ods_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/clients/oneroster_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/clients/oneroster_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/clients/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/clients/user_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:24:40.424107 strongmind-platform-sdk-2.7.0/platform_sdk/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/helpers/exception_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/helpers/link_header.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:24:40.424107 strongmind-platform-sdk-2.7.0/platform_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/models/cloud_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/models/link_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/models/partner.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:24:40.424107 strongmind-platform-sdk-2.7.0/platform_sdk/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/shared/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/shared/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/platform_sdk/shared/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 23:24:40.432107 strongmind-platform-sdk-2.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:24:40.428107 strongmind-platform-sdk-2.7.0/strongmind_platform_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-13 23:24:40.000000 strongmind-platform-sdk-2.7.0/strongmind_platform_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-13 23:24:40.000000 strongmind-platform-sdk-2.7.0/strongmind_platform_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 23:24:40.000000 strongmind-platform-sdk-2.7.0/strongmind_platform_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 23:24:40.000000 strongmind-platform-sdk-2.7.0/strongmind_platform_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 23:24:40.000000 strongmind-platform-sdk-2.7.0/strongmind_platform_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:24:40.428107 strongmind-platform-sdk-2.7.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:24:40.432107 strongmind-platform-sdk-2.7.0/test/factories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/factories/event_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/factories/oneroster_academic_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/factories/oneroster_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/factories/oneroster_course.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/factories/oneroster_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/factories/oneroster_guidref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/factories/oneroster_lineitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/factories/oneroster_org_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/factories/oneroster_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/factories/oneroster_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/factories/oneroster_user_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/factories/partner.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/factories/response_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/factories/standalone_partner.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/factories/user_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/test_events_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/test_exception_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    33101 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/test_identity_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/test_link_header.py
--rw-r--r--   0 runner    (1001) docker     (123)    13441 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/test_ods_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/test_oneroster_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/test_oneroster_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/test_slack_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-13 23:23:33.000000 strongmind-platform-sdk-2.7.0/test/test_user_creation_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:03.257419 strongmind-platform-sdk-2.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-08 22:49:03.257419 strongmind-platform-sdk-2.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:03.245419 strongmind-platform-sdk-2.8.1/platform_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:03.249419 strongmind-platform-sdk-2.8.1/platform_sdk/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/clients/events_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/clients/identity_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/clients/mapper_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/clients/ods_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/clients/oneroster_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/clients/oneroster_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/clients/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/clients/user_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:03.249419 strongmind-platform-sdk-2.8.1/platform_sdk/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/helpers/exception_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/helpers/link_header.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:03.249419 strongmind-platform-sdk-2.8.1/platform_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/models/cloud_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/models/link_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/models/partner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:03.249419 strongmind-platform-sdk-2.8.1/platform_sdk/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/shared/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/shared/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/platform_sdk/shared/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 22:49:03.257419 strongmind-platform-sdk-2.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:03.249419 strongmind-platform-sdk-2.8.1/strongmind_platform_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-08 22:49:03.000000 strongmind-platform-sdk-2.8.1/strongmind_platform_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-08 22:49:03.000000 strongmind-platform-sdk-2.8.1/strongmind_platform_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 22:49:03.000000 strongmind-platform-sdk-2.8.1/strongmind_platform_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-08 22:49:03.000000 strongmind-platform-sdk-2.8.1/strongmind_platform_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 22:49:03.000000 strongmind-platform-sdk-2.8.1/strongmind_platform_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:03.253419 strongmind-platform-sdk-2.8.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:49:03.257419 strongmind-platform-sdk-2.8.1/test/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/factories/event_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/factories/oneroster_academic_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/factories/oneroster_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/factories/oneroster_course.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/factories/oneroster_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/factories/oneroster_guidref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/factories/oneroster_lineitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/factories/oneroster_org_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/factories/oneroster_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/factories/oneroster_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/factories/oneroster_user_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/factories/partner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/factories/response_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/factories/standalone_partner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/factories/user_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/test_events_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/test_exception_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36341 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/test_identity_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/test_link_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13441 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/test_ods_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/test_oneroster_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/test_oneroster_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/test_slack_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-08 22:47:22.000000 strongmind-platform-sdk-2.8.1/test/test_user_creation_client.py
```

### Comparing `strongmind-platform-sdk-2.7.0/PKG-INFO` & `strongmind-platform-sdk-2.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strongmind-platform-sdk
-Version: 2.7.0
+Version: 2.8.1
 Summary: Common utilities, models, and clients used with StrongMind Platform APIs
 Home-page: https://github.com/StrongMind/platform-python-sdk
 Author: Team Platform
 Author-email: platform@strongmind.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `strongmind-platform-sdk-2.7.0/README.md` & `strongmind-platform-sdk-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/platform_sdk/clients/events_client.py` & `strongmind-platform-sdk-2.8.1/platform_sdk/clients/events_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/platform_sdk/clients/identity_client.py` & `strongmind-platform-sdk-2.8.1/platform_sdk/clients/identity_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     def get_token(self):
         if self._token_expired():
             basic_auth = HTTPBasicAuth(username=self.client_id,
                                        password=self.client_secret)
             response = requests.post(f"{self.baseurl}/connect/token", auth=basic_auth,
                                      data={'grant_type': 'client_credentials'})
             raise_for_status_with_dependency_name(response, IDENTITY_SERVER)
+            raise_identity_client_error_if_identity_error_page(response)
+
             self.token = response.json()
             self.token['timestamp'] = datetime.datetime.utcnow()
 
         return self.token['access_token']
 
     def _token_expired(self):
         if not self.token:
@@ -63,14 +65,17 @@
     def _get(self, url, raise_404: bool = True):
         headers = self._headers()
         response = requests.get(url, headers=headers)
         try:
             raise_for_status_with_dependency_name(response, IDENTITY_SERVER)
         except requests.HTTPError as http_error:
             handle_http_error(http_error, raise_404)
+
+        raise_identity_client_error_if_identity_error_page(response)
+
         return response.json()
 
     def get_by_username(self, username):
         url = f"{self.baseurl}/api/accounts?username={username}"
         return self._get(url)
 
     def get_by_id(self, identity_id):
@@ -95,14 +100,16 @@
                        send_email: bool = False,
                        include_username: bool = False,
                        return_url: str = ""):
         headers = self._headers()
         url = f"{self.baseurl}/api/accounts/{identity_id}/PasswordReset?sendEmail={send_email}&includeUsername={include_username}&returnUrl={return_url}"
         response = requests.post(url, headers=headers)
         raise_for_status_with_dependency_name(response, IDENTITY_SERVER)
+        raise_identity_client_error_if_identity_error_page(response)
+
         if len(response.text) > 0:
             return response.json()
 
     def update_account(self, identity_id, username=None, email=None, is_active=None):
         headers = self._headers()
         url = f"{self.baseurl}/api/accounts/{identity_id}"
         data = {}
@@ -110,26 +117,26 @@
             data["username"] = username
         if email is not None:
             data["email"] = email
         if is_active is not None:
             data["isActive"] = is_active
         response = requests.patch(url, headers=headers, json=data)
         raise_for_status_with_dependency_name(response, IDENTITY_SERVER)
-
-        if response.text and 'Error - Identity' in response.text:
-            raise IdentityClientError(response.text)
+        raise_identity_client_error_if_identity_error_page(response)
 
         if response.text:
             return response.json()
 
     def send_reminder_email(self, identity_id):
         headers = self._headers()
         url = f"{self.baseurl}/api/accounts/SendReminderEmail"
         response = requests.post(url, json=identity_id, headers=headers)
         raise_for_status_with_dependency_name(response, IDENTITY_SERVER)
+        raise_identity_client_error_if_identity_error_page(response)
+
         if len(response.text) > 0:
             return response.json()
 
     def jwks_config(self):
         jwsk_url = f"{self.baseurl}/.well-known/openid-configuration/jwks"
         return self._get(jwsk_url)
 
@@ -140,7 +147,12 @@
 
 
 def handle_http_error(http_error, raise_404):
     if http_error.response.status_code == 404 and raise_404:
         raise IdentityNotFoundError(http_error)
     elif http_error.response.status_code != 404:
         raise http_error
+
+
+def raise_identity_client_error_if_identity_error_page(response):
+    if response.text and 'Error - Identity' in response.text:
+        raise IdentityClientError(response.text)
```

### Comparing `strongmind-platform-sdk-2.7.0/platform_sdk/clients/mapper_client.py` & `strongmind-platform-sdk-2.8.1/platform_sdk/clients/mapper_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/platform_sdk/clients/ods_client.py` & `strongmind-platform-sdk-2.8.1/platform_sdk/clients/ods_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/platform_sdk/clients/oneroster_authentication.py` & `strongmind-platform-sdk-2.8.1/platform_sdk/clients/oneroster_authentication.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/platform_sdk/clients/oneroster_client.py` & `strongmind-platform-sdk-2.8.1/platform_sdk/clients/oneroster_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/platform_sdk/clients/slack.py` & `strongmind-platform-sdk-2.8.1/platform_sdk/clients/slack.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/platform_sdk/clients/user_creation.py` & `strongmind-platform-sdk-2.8.1/platform_sdk/clients/user_creation.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/platform_sdk/helpers/exception_logger.py` & `strongmind-platform-sdk-2.8.1/platform_sdk/helpers/exception_logger.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/platform_sdk/helpers/link_header.py` & `strongmind-platform-sdk-2.8.1/platform_sdk/helpers/link_header.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/platform_sdk/models/user.py` & `strongmind-platform-sdk-2.8.1/platform_sdk/models/user.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/platform_sdk/shared/exceptions.py` & `strongmind-platform-sdk-2.8.1/platform_sdk/shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/setup.py` & `strongmind-platform-sdk-2.8.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='strongmind-platform-sdk',
-    version='2.7.0',
+    version='2.8.1',
     packages=find_packages(),
     url='https://github.com/StrongMind/platform-python-sdk',
     license='',
     author='Team Platform',
     author_email='platform@strongmind.com',
     description='Common utilities, models, and clients used with StrongMind Platform APIs',
     long_description=long_description,
```

### Comparing `strongmind-platform-sdk-2.7.0/strongmind_platform_sdk.egg-info/PKG-INFO` & `strongmind-platform-sdk-2.8.1/strongmind_platform_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strongmind-platform-sdk
-Version: 2.7.0
+Version: 2.8.1
 Summary: Common utilities, models, and clients used with StrongMind Platform APIs
 Home-page: https://github.com/StrongMind/platform-python-sdk
 Author: Team Platform
 Author-email: platform@strongmind.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `strongmind-platform-sdk-2.7.0/strongmind_platform_sdk.egg-info/SOURCES.txt` & `strongmind-platform-sdk-2.8.1/strongmind_platform_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/factories/event_factories.py` & `strongmind-platform-sdk-2.8.1/test/factories/event_factories.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/factories/oneroster_academic_session.py` & `strongmind-platform-sdk-2.8.1/test/factories/oneroster_academic_session.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/factories/oneroster_class.py` & `strongmind-platform-sdk-2.8.1/test/factories/oneroster_class.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/factories/oneroster_course.py` & `strongmind-platform-sdk-2.8.1/test/factories/oneroster_course.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/factories/oneroster_enrollment.py` & `strongmind-platform-sdk-2.8.1/test/factories/oneroster_enrollment.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/factories/oneroster_guidref.py` & `strongmind-platform-sdk-2.8.1/test/factories/oneroster_guidref.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/factories/oneroster_lineitem.py` & `strongmind-platform-sdk-2.8.1/test/factories/oneroster_lineitem.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/factories/oneroster_org_factory.py` & `strongmind-platform-sdk-2.8.1/test/factories/oneroster_org_factory.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/factories/oneroster_result.py` & `strongmind-platform-sdk-2.8.1/test/factories/oneroster_result.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/factories/oneroster_user.py` & `strongmind-platform-sdk-2.8.1/test/factories/oneroster_user.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/factories/partner.py` & `strongmind-platform-sdk-2.8.1/test/factories/partner.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/factories/response_factory.py` & `strongmind-platform-sdk-2.8.1/test/factories/response_factory.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/factories/standalone_partner.py` & `strongmind-platform-sdk-2.8.1/test/factories/standalone_partner.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/factories/user_factories.py` & `strongmind-platform-sdk-2.8.1/test/factories/user_factories.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/test_events_client.py` & `strongmind-platform-sdk-2.8.1/test/test_events_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/test_exception_logger.py` & `strongmind-platform-sdk-2.8.1/test/test_exception_logger.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/test_identity_client.py` & `strongmind-platform-sdk-2.8.1/test/test_identity_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,32 +53,82 @@
         mock_response = mock({'text': response_text})
         when(self.id_server_client)._headers().thenReturn(headers)
         when(requests).patch(url, headers=headers, json=data).thenReturn(mock_response)
         with self.assertRaises(IdentityClientError) as assert_error:
             self.id_server_client.update_account(identity_id, username=data['username'])
         expect(str(assert_error.exception)).to(equal(response_text))
 
+    def test_send_reminder_email_raises_identity_client_error_on_page_error(self):
+        identity_id = fake.uuid4()
+        url = f"https://{self.identity_server_domain}/api/accounts/SendReminderEmail"
+        headers = {'header': 'token'}
+        response_text = '<html><head><title>Error - Identity</title>'
+        mock_response = mock({'text': response_text})
+        when(self.id_server_client)._headers().thenReturn(headers)
+        when(requests).post(url, json=identity_id, headers=headers).thenReturn(mock_response)
+        with self.assertRaises(IdentityClientError) as assert_error:
+            self.id_server_client.send_reminder_email(identity_id)
+        expect(str(assert_error.exception)).to(equal(response_text))
+
+    def test_password_reset_raises_identity_client_error_on_page_error(self):
+        identity_id = fake.uuid4()
+        url = f"https://{self.identity_server_domain}/api/accounts/{identity_id}" \
+              f"/PasswordReset?sendEmail=False&includeUsername=False&returnUrl="
+        headers = {'header': 'token'}
+        response_text = '<html><head><title>Error - Identity</title>'
+        mock_response = mock({'text': response_text})
+        when(self.id_server_client)._headers().thenReturn(headers)
+        when(requests).post(url, headers=headers).thenReturn(mock_response)
+        with self.assertRaises(IdentityClientError) as assert_error:
+            self.id_server_client.password_reset(identity_id)
+        expect(str(assert_error.exception)).to(equal(response_text))
+
+    def test_get_token_raises_identity_client_error_on_page_error(self):
+        response_text = '<html><head><title>Error - Identity</title>'
+        mock_response = mock({'text': response_text})
+        basic_auth = HTTPBasicAuth(username=self.id_server_client.client_id,
+                                   password=self.id_server_client.client_secret)
+        when(requests).post(
+            f"{self.id_server_client.baseurl}/connect/token", auth=basic_auth, data={'grant_type': 'client_credentials'}
+        ).thenReturn(mock_response)
+        with self.assertRaises(IdentityClientError) as assert_error:
+            self.id_server_client.get_token()
+        expect(str(assert_error.exception)).to(equal(response_text))
+
+    def test_get_raises_identity_client_error_on_page_error(self):
+        url = f"https://{self.identity_server_domain}/api/accounts/{fake.uuid4()}"
+        headers = {'header': 'token'}
+        response_text = '<html><head><title>Error - Identity</title>'
+        mock_response = mock({'text': response_text})
+        when(self.id_server_client)._headers().thenReturn(headers)
+        when(requests).get(url, headers=headers).thenReturn(mock_response)
+        with self.assertRaises(IdentityClientError) as assert_error:
+            self.id_server_client._get(url)
+        expect(str(assert_error.exception)).to(equal(response_text))
+
     @freeze_time("2020-07-31")
     def test_identity_client_issues_new_token_when_none_exists(self):
         """When there is no token, we should get a new one so that we can have access"""
         expected_token = fake.word()
         response = mock({'status_code': 200, 'json': lambda: {"access_token": expected_token, "expires_in": 3600}})
+        response.text = fake.word()
         self.mock_token_retrieval(response)
         token = self.id_server_client.get_token()
         expect(token).to(equal(expected_token))
         verifyStubbedInvocationsAreUsed()
 
     @freeze_time("2020-07-31")
     def test_identity_client_issues_new_token_when_token_expired(self):
         """When the token is expired, we should get a new one so that we can have access"""
         stale_token = fake.word()
         expected_token = fake.word()
         self.id_server_client.token = {"access_token": stale_token, "expires_in": 3600,
                                        "timestamp": datetime.utcnow() - timedelta(days=1)}
         response = mock({'status_code': 200, 'json': lambda: {"access_token": expected_token, "expires_in": 3600}})
+        response.text = fake.word()
         self.mock_token_retrieval(response)
         token = self.id_server_client.get_token()
         expect(token).to(equal(expected_token))
         verifyStubbedInvocationsAreUsed()
 
     @freeze_time("2020-07-31")
     def test_identity_client_issues_new_token_when_token_is_about_to_expire(self):
@@ -88,14 +138,15 @@
         So that tokens do not expire while we are using them
         """
         stale_token = fake.word()
         expected_token = fake.word()
         self.id_server_client.token = {"access_token": stale_token, "expires_in": 3600,
                                        "timestamp": datetime.utcnow() - timedelta(minutes=59, seconds=45)}
         response = mock({'status_code': 200, 'json': lambda: {"access_token": expected_token, "expires_in": 3600}})
+        response.text = fake.word()
         self.mock_token_retrieval(response)
         token = self.id_server_client.get_token()
         expect(token).to(equal(expected_token))
         verifyStubbedInvocationsAreUsed()
 
     @freeze_time("2020-07-31")
     def test_identity_client_issues_same_token_when_one_exists(self):
@@ -118,14 +169,15 @@
         # Arrange
         self.id_server_client.token = {"access_token": "blah", "expires_in": 3600,
                                        "timestamp": datetime.utcnow() - timedelta(minutes=1)}
         username = fake.name()
         response = mock({
             'status_code': 200
         }, spec=requests.Response)
+        response.text = fake.word()
         when(response).raise_for_status().thenReturn()
         when(response).json().thenReturn({"username": username})
 
         when(requests).get(
             f"https://{self.identity_server_domain}/api/accounts?username={username}",
             headers={"Authorization": "Bearer blah", "Accept": "application/json"}).thenReturn(response)
 
@@ -144,14 +196,15 @@
                                        "timestamp": datetime.utcnow() - timedelta(minutes=1)}
         id = fake.uuid4()
         provider = fake.domain_word()
         account_external_id = fake.uuid4()
         response = mock({
             'status_code': 200
         }, spec=requests.Response)
+        response.text = fake.word()
         when(response).raise_for_status().thenReturn()
         when(response).json().thenReturn({"id": id})
 
         when(requests).get(
             f"https://{self.identity_server_domain}/api/externalaccounts/{provider}/{account_external_id}",
             headers={"Authorization": "Bearer blah", "Accept": "application/json"}).thenReturn(response)
 
@@ -189,14 +242,15 @@
         # Arrange
         self.id_server_client.token = {"access_token": "blah", "expires_in": 3600,
                                        "timestamp": datetime.utcnow() - timedelta(minutes=1)}
         identity_id = fake.uuid4()
         response = mock({
             'status_code': 200
         }, spec=requests.Response)
+        response.text = fake.word()
         when(response).raise_for_status().thenReturn()
         when(response).json().thenReturn({"id": identity_id})
 
         when(requests).get(
             f"https://{self.identity_server_domain}/api/accounts/{identity_id}",
             headers={"Authorization": "Bearer blah", "Accept": "application/json"}).thenReturn(response)
 
@@ -235,14 +289,15 @@
         self.id_server_client.token = {"access_token": "blah", "expires_in": 3600,
                                        "timestamp": datetime.utcnow() - timedelta(minutes=1)}
         identity_id_1 = fake.uuid4()
         identity_id_2 = fake.uuid4()
         response = mock({
             'status_code': 200
         }, spec=requests.Response)
+        response.text = fake.word()
         when(response).raise_for_status().thenReturn()
         when(response).json().thenReturn(
             {
                 "results": [
                     {
                         "id": identity_id_1
                     },
@@ -277,14 +332,15 @@
         """
         # Arrange
         self.id_server_client.token = {"access_token": "blah", "expires_in": 3600,
                                        "timestamp": datetime.utcnow() - timedelta(minutes=1)}
         response = mock({
             'status_code': 404
         }, spec=requests.Response)
+        response.text = fake.word()
         when(response).raise_for_status().thenRaise(requests.HTTPError(response=response))
         when(response).json().thenReturn({"results": []})
 
         search_param = fake.email()
 
         when(requests).get(
             f"https://{self.identity_server_domain}/api/accounts/search"
@@ -482,14 +538,15 @@
         self.id_server_client.token = {"access_token": "blah", "expires_in": 3600,
                                        "timestamp": datetime.utcnow() - timedelta(minutes=1)}
         source_system_id = fake.uuid4()
         identity_id = fake.uuid4()
         response = mock({
             'status_code': 200
         }, spec=requests.Response)
+        response.text = fake.word()
         when(response).raise_for_status().thenReturn()
         when(response).json().thenReturn({"id": identity_id, "sourceSystemId": source_system_id})
 
         when(requests).get(
             f"https://{self.identity_server_domain}/api/accounts/sourceSystemId/{source_system_id}",
             headers={"Authorization": "Bearer blah", "Accept": "application/json"}).thenReturn(response)
 
@@ -670,14 +727,15 @@
     def test_jwks_config(self):
         # Arrange
         self.id_server_client.token = {"access_token": "blah", "expires_in": 3600,
                                        "timestamp": datetime.utcnow() - timedelta(minutes=1)}
         response = mock({
             'status_code': 200
         }, spec=requests.Response)
+        response.text = fake.word()
         when(response).raise_for_status().thenReturn()
         when(response).json().thenReturn(self.jwks_config)
 
         when(requests).get(
             f"https://{self.identity_server_domain}/.well-known/openid-configuration/jwks",
             headers={"Authorization": "Bearer blah", "Accept": "application/json"}).thenReturn(response)
```

### Comparing `strongmind-platform-sdk-2.7.0/test/test_link_header.py` & `strongmind-platform-sdk-2.8.1/test/test_link_header.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/test_ods_client.py` & `strongmind-platform-sdk-2.8.1/test/test_ods_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/test_oneroster_authentication.py` & `strongmind-platform-sdk-2.8.1/test/test_oneroster_authentication.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/test_oneroster_client.py` & `strongmind-platform-sdk-2.8.1/test/test_oneroster_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/test_slack_client.py` & `strongmind-platform-sdk-2.8.1/test/test_slack_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.7.0/test/test_user_creation_client.py` & `strongmind-platform-sdk-2.8.1/test/test_user_creation_client.py`

 * *Files identical despite different names*

