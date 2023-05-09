# Comparing `tmp/pyfirebird-0.0.27.tar.gz` & `tmp/pyfirebird-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfirebird-0.0.27.tar", last modified: Tue May  9 02:14:22 2023, max compression
+gzip compressed data, was "pyfirebird-0.0.28.tar", last modified: Tue May  9 02:43:39 2023, max compression
```

## Comparing `pyfirebird-0.0.27.tar` & `pyfirebird-0.0.28.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:14:22.949474 pyfirebird-0.0.27/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-05-09 02:14:22.949474 pyfirebird-0.0.27/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        8 2023-04-30 05:34:25.000000 pyfirebird-0.0.27/README.md
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-05-09 02:14:22.949474 pyfirebird-0.0.27/setup.cfg
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1301 2023-05-09 02:14:20.000000 pyfirebird-0.0.27/setup.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:14:22.945474 pyfirebird-0.0.27/src/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:14:22.945474 pyfirebird-0.0.27/src/firebird/
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)      169 2023-04-30 06:39:02.000000 pyfirebird-0.0.27/src/firebird/__init__.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)    10421 2023-05-09 01:41:45.000000 pyfirebird-0.0.27/src/firebird/base.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:14:22.949474 pyfirebird-0.0.27/src/firebird/cmd_tools/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 05:45:15.000000 pyfirebird-0.0.27/src/firebird/cmd_tools/__init__.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2903 2023-05-07 02:10:48.000000 pyfirebird-0.0.27/src/firebird/cmd_tools/executor.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     4964 2023-05-05 03:26:12.000000 pyfirebird-0.0.27/src/firebird/cmd_tools/executor_impl.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      649 2023-05-06 21:14:34.000000 pyfirebird-0.0.27/src/firebird/cmd_tools/fbconsole.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     3083 2023-05-09 02:04:29.000000 pyfirebird-0.0.27/src/firebird/cmd_tools/pipeline.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2595 2023-05-09 02:12:28.000000 pyfirebird-0.0.27/src/firebird/cmd_tools/pipeline_impl.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2972 2023-04-30 05:32:50.000000 pyfirebird-0.0.27/src/firebird/rabbitmq.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:14:22.949474 pyfirebird-0.0.27/src/firebird/utils/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-05-05 02:58:25.000000 pyfirebird-0.0.27/src/firebird/utils/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4359 2023-05-05 02:56:50.000000 pyfirebird-0.0.27/src/firebird/utils/checkpoint.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     6296 2023-05-09 02:11:15.000000 pyfirebird-0.0.27/src/firebird/zkdb.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:14:22.949474 pyfirebird-0.0.27/src/firebirdconsole/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-06 20:57:08.000000 pyfirebird-0.0.27/src/firebirdconsole/__init__.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:14:22.949474 pyfirebird-0.0.27/src/firebirdconsole/firebirdconsole/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-06 20:05:23.000000 pyfirebird-0.0.27/src/firebirdconsole/firebirdconsole/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-05-06 20:05:23.000000 pyfirebird-0.0.27/src/firebirdconsole/firebirdconsole/asgi.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3803 2023-05-07 02:13:47.000000 pyfirebird-0.0.27/src/firebirdconsole/firebirdconsole/settings.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      836 2023-05-06 20:43:13.000000 pyfirebird-0.0.27/src/firebirdconsole/firebirdconsole/urls.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-05-06 20:05:23.000000 pyfirebird-0.0.27/src/firebirdconsole/firebirdconsole/wsgi.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:14:22.949474 pyfirebird-0.0.27/src/firebirdconsole/ui/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-06 20:06:08.000000 pyfirebird-0.0.27/src/firebirdconsole/ui/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       63 2023-05-06 20:06:08.000000 pyfirebird-0.0.27/src/firebirdconsole/ui/admin.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-05-06 20:35:46.000000 pyfirebird-0.0.27/src/firebirdconsole/ui/apps.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:14:22.949474 pyfirebird-0.0.27/src/firebirdconsole/ui/migrations/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-06 20:06:08.000000 pyfirebird-0.0.27/src/firebirdconsole/ui/migrations/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       57 2023-05-06 20:06:08.000000 pyfirebird-0.0.27/src/firebirdconsole/ui/models.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:14:22.945474 pyfirebird-0.0.27/src/firebirdconsole/ui/static/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:14:22.949474 pyfirebird-0.0.27/src/firebirdconsole/ui/static/images/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)   126365 2023-05-04 00:03:29.000000 pyfirebird-0.0.27/src/firebirdconsole/ui/static/images/logo.jpeg
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:14:22.949474 pyfirebird-0.0.27/src/firebirdconsole/ui/static/js-bundle/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)   287253 2023-05-09 01:20:58.000000 pyfirebird-0.0.27/src/firebirdconsole/ui/static/js-bundle/home.js
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:14:22.949474 pyfirebird-0.0.27/src/firebirdconsole/ui/templates/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3817 2023-05-08 02:11:53.000000 pyfirebird-0.0.27/src/firebirdconsole/ui/templates/application.html
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      217 2023-05-06 20:12:44.000000 pyfirebird-0.0.27/src/firebirdconsole/ui/templates/index.html
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:14:22.949474 pyfirebird-0.0.27/src/firebirdconsole/ui/templatetags/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 00:25:05.000000 pyfirebird-0.0.27/src/firebirdconsole/ui/templatetags/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      639 2023-05-09 00:25:31.000000 pyfirebird-0.0.27/src/firebirdconsole/ui/templatetags/app_filters.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-05-06 20:06:08.000000 pyfirebird-0.0.27/src/firebirdconsole/ui/tests.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      212 2023-05-09 01:25:27.000000 pyfirebird-0.0.27/src/firebirdconsole/ui/urls.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      571 2023-05-08 02:38:33.000000 pyfirebird-0.0.27/src/firebirdconsole/ui/view_tools.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:14:22.949474 pyfirebird-0.0.27/src/firebirdconsole/ui/views/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       23 2023-05-09 00:56:45.000000 pyfirebird-0.0.27/src/firebirdconsole/ui/views/__init__.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:14:22.949474 pyfirebird-0.0.27/src/firebirdconsole/ui/views/apis/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       34 2023-05-09 01:11:40.000000 pyfirebird-0.0.27/src/firebirdconsole/ui/views/apis/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-05-09 02:13:29.000000 pyfirebird-0.0.27/src/firebirdconsole/ui/views/apis/main.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      288 2023-05-09 00:32:38.000000 pyfirebird-0.0.27/src/firebirdconsole/ui/views/home.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:14:22.949474 pyfirebird-0.0.27/src/pyfirebird.egg-info/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-05-09 02:14:22.000000 pyfirebird-0.0.27/src/pyfirebird.egg-info/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1616 2023-05-09 02:14:22.000000 pyfirebird-0.0.27/src/pyfirebird.egg-info/SOURCES.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-05-09 02:14:22.000000 pyfirebird-0.0.27/src/pyfirebird.egg-info/dependency_links.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-05-09 02:14:22.000000 pyfirebird-0.0.27/src/pyfirebird.egg-info/entry_points.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       70 2023-05-09 02:14:22.000000 pyfirebird-0.0.27/src/pyfirebird.egg-info/requires.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       25 2023-05-09 02:14:22.000000 pyfirebird-0.0.27/src/pyfirebird.egg-info/top_level.txt
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:43:39.040686 pyfirebird-0.0.28/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-05-09 02:43:39.040686 pyfirebird-0.0.28/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        8 2023-04-30 05:34:25.000000 pyfirebird-0.0.28/README.md
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-05-09 02:43:39.040686 pyfirebird-0.0.28/setup.cfg
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1301 2023-05-09 02:43:36.000000 pyfirebird-0.0.28/setup.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:43:39.036685 pyfirebird-0.0.28/src/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:43:39.036685 pyfirebird-0.0.28/src/firebird/
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)      169 2023-04-30 06:39:02.000000 pyfirebird-0.0.28/src/firebird/__init__.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)    10421 2023-05-09 01:41:45.000000 pyfirebird-0.0.28/src/firebird/base.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:43:39.036685 pyfirebird-0.0.28/src/firebird/cmd_tools/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 05:45:15.000000 pyfirebird-0.0.28/src/firebird/cmd_tools/__init__.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2903 2023-05-07 02:10:48.000000 pyfirebird-0.0.28/src/firebird/cmd_tools/executor.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     4964 2023-05-05 03:26:12.000000 pyfirebird-0.0.28/src/firebird/cmd_tools/executor_impl.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      649 2023-05-06 21:14:34.000000 pyfirebird-0.0.28/src/firebird/cmd_tools/fbconsole.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     3083 2023-05-09 02:04:29.000000 pyfirebird-0.0.28/src/firebird/cmd_tools/pipeline.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2603 2023-05-09 02:43:23.000000 pyfirebird-0.0.28/src/firebird/cmd_tools/pipeline_impl.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2972 2023-04-30 05:32:50.000000 pyfirebird-0.0.28/src/firebird/rabbitmq.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:43:39.036685 pyfirebird-0.0.28/src/firebird/utils/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-05-05 02:58:25.000000 pyfirebird-0.0.28/src/firebird/utils/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4359 2023-05-05 02:56:50.000000 pyfirebird-0.0.28/src/firebird/utils/checkpoint.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     6296 2023-05-09 02:11:15.000000 pyfirebird-0.0.28/src/firebird/zkdb.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:43:39.036685 pyfirebird-0.0.28/src/firebirdconsole/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-06 20:57:08.000000 pyfirebird-0.0.28/src/firebirdconsole/__init__.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:43:39.040686 pyfirebird-0.0.28/src/firebirdconsole/firebirdconsole/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-06 20:05:23.000000 pyfirebird-0.0.28/src/firebirdconsole/firebirdconsole/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-05-06 20:05:23.000000 pyfirebird-0.0.28/src/firebirdconsole/firebirdconsole/asgi.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3803 2023-05-07 02:13:47.000000 pyfirebird-0.0.28/src/firebirdconsole/firebirdconsole/settings.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      836 2023-05-06 20:43:13.000000 pyfirebird-0.0.28/src/firebirdconsole/firebirdconsole/urls.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-05-06 20:05:23.000000 pyfirebird-0.0.28/src/firebirdconsole/firebirdconsole/wsgi.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:43:39.040686 pyfirebird-0.0.28/src/firebirdconsole/ui/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-06 20:06:08.000000 pyfirebird-0.0.28/src/firebirdconsole/ui/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       63 2023-05-06 20:06:08.000000 pyfirebird-0.0.28/src/firebirdconsole/ui/admin.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-05-06 20:35:46.000000 pyfirebird-0.0.28/src/firebirdconsole/ui/apps.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:43:39.040686 pyfirebird-0.0.28/src/firebirdconsole/ui/migrations/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-06 20:06:08.000000 pyfirebird-0.0.28/src/firebirdconsole/ui/migrations/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       57 2023-05-06 20:06:08.000000 pyfirebird-0.0.28/src/firebirdconsole/ui/models.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:43:39.036685 pyfirebird-0.0.28/src/firebirdconsole/ui/static/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:43:39.040686 pyfirebird-0.0.28/src/firebirdconsole/ui/static/images/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)   126365 2023-05-04 00:03:29.000000 pyfirebird-0.0.28/src/firebirdconsole/ui/static/images/logo.jpeg
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:43:39.040686 pyfirebird-0.0.28/src/firebirdconsole/ui/static/js-bundle/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)   287253 2023-05-09 01:20:58.000000 pyfirebird-0.0.28/src/firebirdconsole/ui/static/js-bundle/home.js
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:43:39.040686 pyfirebird-0.0.28/src/firebirdconsole/ui/templates/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3817 2023-05-08 02:11:53.000000 pyfirebird-0.0.28/src/firebirdconsole/ui/templates/application.html
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      217 2023-05-06 20:12:44.000000 pyfirebird-0.0.28/src/firebirdconsole/ui/templates/index.html
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:43:39.040686 pyfirebird-0.0.28/src/firebirdconsole/ui/templatetags/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 00:25:05.000000 pyfirebird-0.0.28/src/firebirdconsole/ui/templatetags/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      639 2023-05-09 00:25:31.000000 pyfirebird-0.0.28/src/firebirdconsole/ui/templatetags/app_filters.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-05-06 20:06:08.000000 pyfirebird-0.0.28/src/firebirdconsole/ui/tests.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      212 2023-05-09 01:25:27.000000 pyfirebird-0.0.28/src/firebirdconsole/ui/urls.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      571 2023-05-08 02:38:33.000000 pyfirebird-0.0.28/src/firebirdconsole/ui/view_tools.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:43:39.040686 pyfirebird-0.0.28/src/firebirdconsole/ui/views/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       23 2023-05-09 00:56:45.000000 pyfirebird-0.0.28/src/firebirdconsole/ui/views/__init__.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:43:39.040686 pyfirebird-0.0.28/src/firebirdconsole/ui/views/apis/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       34 2023-05-09 01:11:40.000000 pyfirebird-0.0.28/src/firebirdconsole/ui/views/apis/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-05-09 02:13:29.000000 pyfirebird-0.0.28/src/firebirdconsole/ui/views/apis/main.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      288 2023-05-09 00:32:38.000000 pyfirebird-0.0.28/src/firebirdconsole/ui/views/home.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 02:43:39.040686 pyfirebird-0.0.28/src/pyfirebird.egg-info/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-05-09 02:43:39.000000 pyfirebird-0.0.28/src/pyfirebird.egg-info/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1616 2023-05-09 02:43:39.000000 pyfirebird-0.0.28/src/pyfirebird.egg-info/SOURCES.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-05-09 02:43:39.000000 pyfirebird-0.0.28/src/pyfirebird.egg-info/dependency_links.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-05-09 02:43:39.000000 pyfirebird-0.0.28/src/pyfirebird.egg-info/entry_points.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       70 2023-05-09 02:43:39.000000 pyfirebird-0.0.28/src/pyfirebird.egg-info/requires.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       25 2023-05-09 02:43:39.000000 pyfirebird-0.0.28/src/pyfirebird.egg-info/top_level.txt
```

### Comparing `pyfirebird-0.0.27/setup.py` & `pyfirebird-0.0.28/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), "r") as f:
     README = f.read()
 
 # This call to setup() does all the work
 setup(
     name="pyfirebird",
-    version="0.0.27",
+    version="0.0.28",
     description="Streaming Data Processing Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/stonezhong/firebird",
     author="Stone Zhong",
     author_email="stonezhong@hotmail.com",
     license="MIT",
```

### Comparing `pyfirebird-0.0.27/src/firebird/base.py` & `pyfirebird-0.0.28/src/firebird/base.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.27/src/firebird/cmd_tools/executor.py` & `pyfirebird-0.0.28/src/firebird/cmd_tools/executor.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.27/src/firebird/cmd_tools/executor_impl.py` & `pyfirebird-0.0.28/src/firebird/cmd_tools/executor_impl.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.27/src/firebird/cmd_tools/fbconsole.py` & `pyfirebird-0.0.28/src/firebird/cmd_tools/fbconsole.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.27/src/firebird/cmd_tools/pipeline.py` & `pyfirebird-0.0.28/src/firebird/cmd_tools/pipeline.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.27/src/firebird/cmd_tools/pipeline_impl.py` & `pyfirebird-0.0.28/src/firebird/cmd_tools/pipeline_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         db.unregister_pipeline(pipeline_id)
 
 def list_command(config):
     with zkdb(**config['zookeeper']) as db:
         pipelines = db.get_pipelines()
 
     for pipeline in pipelines:
-        print(f"{pipeline['id']}:")
+        print(f"{pipeline['info']['id']}:")
         print(f"    module: {pipeline['module']}")
         if len(pipeline["executors"]) == 0:
             print("    executors: None")
         else:
             print("    executors:")
             for executor_id, executor in pipeline["executors"].items():
                 executor_info = executor["info"]
```

### Comparing `pyfirebird-0.0.27/src/firebird/rabbitmq.py` & `pyfirebird-0.0.28/src/firebird/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.27/src/firebird/utils/checkpoint.py` & `pyfirebird-0.0.28/src/firebird/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.27/src/firebird/zkdb.py` & `pyfirebird-0.0.28/src/firebird/zkdb.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.27/src/firebirdconsole/firebirdconsole/settings.py` & `pyfirebird-0.0.28/src/firebirdconsole/firebirdconsole/settings.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.27/src/firebirdconsole/firebirdconsole/urls.py` & `pyfirebird-0.0.28/src/firebirdconsole/firebirdconsole/urls.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.27/src/firebirdconsole/ui/static/images/logo.jpeg` & `pyfirebird-0.0.28/src/firebirdconsole/ui/static/images/logo.jpeg`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.27/src/firebirdconsole/ui/static/js-bundle/home.js` & `pyfirebird-0.0.28/src/firebirdconsole/ui/static/js-bundle/home.js`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.27/src/firebirdconsole/ui/templates/application.html` & `pyfirebird-0.0.28/src/firebirdconsole/ui/templates/application.html`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.27/src/firebirdconsole/ui/templatetags/app_filters.py` & `pyfirebird-0.0.28/src/firebirdconsole/ui/templatetags/app_filters.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.27/src/firebirdconsole/ui/view_tools.py` & `pyfirebird-0.0.28/src/firebirdconsole/ui/view_tools.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.27/src/pyfirebird.egg-info/SOURCES.txt` & `pyfirebird-0.0.28/src/pyfirebird.egg-info/SOURCES.txt`

 * *Files identical despite different names*

