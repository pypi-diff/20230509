# Comparing `tmp/pyfirebird-0.0.37.tar.gz` & `tmp/pyfirebird-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfirebird-0.0.37.tar", last modified: Tue May  9 05:22:06 2023, max compression
+gzip compressed data, was "pyfirebird-0.0.38.tar", last modified: Tue May  9 05:29:45 2023, max compression
```

## Comparing `pyfirebird-0.0.37.tar` & `pyfirebird-0.0.38.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:22:06.471014 pyfirebird-0.0.37/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-05-09 05:22:06.471014 pyfirebird-0.0.37/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        8 2023-04-30 05:34:25.000000 pyfirebird-0.0.37/README.md
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-05-09 05:22:06.471014 pyfirebird-0.0.37/setup.cfg
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1301 2023-05-09 05:22:03.000000 pyfirebird-0.0.37/setup.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:22:06.467014 pyfirebird-0.0.37/src/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:22:06.467014 pyfirebird-0.0.37/src/firebird/
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)      169 2023-04-30 06:39:02.000000 pyfirebird-0.0.37/src/firebird/__init__.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)    10367 2023-05-09 05:21:17.000000 pyfirebird-0.0.37/src/firebird/base.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:22:06.467014 pyfirebird-0.0.37/src/firebird/cmd_tools/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 05:45:15.000000 pyfirebird-0.0.37/src/firebird/cmd_tools/__init__.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2903 2023-05-07 02:10:48.000000 pyfirebird-0.0.37/src/firebird/cmd_tools/executor.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     4964 2023-05-05 03:26:12.000000 pyfirebird-0.0.37/src/firebird/cmd_tools/executor_impl.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      649 2023-05-06 21:14:34.000000 pyfirebird-0.0.37/src/firebird/cmd_tools/fbconsole.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     3083 2023-05-09 02:04:29.000000 pyfirebird-0.0.37/src/firebird/cmd_tools/pipeline.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2603 2023-05-09 02:43:23.000000 pyfirebird-0.0.37/src/firebird/cmd_tools/pipeline_impl.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2972 2023-04-30 05:32:50.000000 pyfirebird-0.0.37/src/firebird/rabbitmq.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:22:06.467014 pyfirebird-0.0.37/src/firebird/utils/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-05-05 02:58:25.000000 pyfirebird-0.0.37/src/firebird/utils/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4359 2023-05-05 02:56:50.000000 pyfirebird-0.0.37/src/firebird/utils/checkpoint.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     6296 2023-05-09 02:11:15.000000 pyfirebird-0.0.37/src/firebird/zkdb.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:22:06.467014 pyfirebird-0.0.37/src/firebirdconsole/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-06 20:57:08.000000 pyfirebird-0.0.37/src/firebirdconsole/__init__.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:22:06.467014 pyfirebird-0.0.37/src/firebirdconsole/firebirdconsole/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-06 20:05:23.000000 pyfirebird-0.0.37/src/firebirdconsole/firebirdconsole/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-05-06 20:05:23.000000 pyfirebird-0.0.37/src/firebirdconsole/firebirdconsole/asgi.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3803 2023-05-07 02:13:47.000000 pyfirebird-0.0.37/src/firebirdconsole/firebirdconsole/settings.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      836 2023-05-06 20:43:13.000000 pyfirebird-0.0.37/src/firebirdconsole/firebirdconsole/urls.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-05-06 20:05:23.000000 pyfirebird-0.0.37/src/firebirdconsole/firebirdconsole/wsgi.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:22:06.467014 pyfirebird-0.0.37/src/firebirdconsole/ui/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-06 20:06:08.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       63 2023-05-06 20:06:08.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/admin.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-05-06 20:35:46.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/apps.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:22:06.467014 pyfirebird-0.0.37/src/firebirdconsole/ui/migrations/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-06 20:06:08.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/migrations/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       57 2023-05-06 20:06:08.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/models.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:22:06.467014 pyfirebird-0.0.37/src/firebirdconsole/ui/static/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:22:06.467014 pyfirebird-0.0.37/src/firebirdconsole/ui/static/images/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)   126365 2023-05-04 00:03:29.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/static/images/logo.jpeg
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:22:06.471014 pyfirebird-0.0.37/src/firebirdconsole/ui/static/js-bundle/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)  1548450 2023-05-09 03:56:06.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/static/js-bundle/home.js
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)   290225 2023-05-09 05:01:10.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/static/js-bundle/pipeline.js
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:22:06.471014 pyfirebird-0.0.37/src/firebirdconsole/ui/templates/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3817 2023-05-08 02:11:53.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/templates/application.html
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      217 2023-05-06 20:12:44.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/templates/index.html
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:22:06.471014 pyfirebird-0.0.37/src/firebirdconsole/ui/templatetags/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 00:25:05.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/templatetags/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      639 2023-05-09 00:25:31.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/templatetags/app_filters.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-05-06 20:06:08.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/tests.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      372 2023-05-09 03:57:30.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/urls.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      571 2023-05-08 02:38:33.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/view_tools.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:22:06.471014 pyfirebird-0.0.37/src/firebirdconsole/ui/views/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       54 2023-05-09 04:03:37.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/views/__init__.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:22:06.471014 pyfirebird-0.0.37/src/firebirdconsole/ui/views/apis/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       48 2023-05-09 04:06:17.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/views/apis/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1681 2023-05-09 05:21:55.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/views/apis/main.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      288 2023-05-09 00:32:38.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/views/home.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      387 2023-05-09 04:03:49.000000 pyfirebird-0.0.37/src/firebirdconsole/ui/views/pipeline.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:22:06.471014 pyfirebird-0.0.37/src/pyfirebird.egg-info/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-05-09 05:22:06.000000 pyfirebird-0.0.37/src/pyfirebird.egg-info/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1709 2023-05-09 05:22:06.000000 pyfirebird-0.0.37/src/pyfirebird.egg-info/SOURCES.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-05-09 05:22:06.000000 pyfirebird-0.0.37/src/pyfirebird.egg-info/dependency_links.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-05-09 05:22:06.000000 pyfirebird-0.0.37/src/pyfirebird.egg-info/entry_points.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       70 2023-05-09 05:22:06.000000 pyfirebird-0.0.37/src/pyfirebird.egg-info/requires.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       25 2023-05-09 05:22:06.000000 pyfirebird-0.0.37/src/pyfirebird.egg-info/top_level.txt
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:29:45.947692 pyfirebird-0.0.38/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-05-09 05:29:45.947692 pyfirebird-0.0.38/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        8 2023-04-30 05:34:25.000000 pyfirebird-0.0.38/README.md
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-05-09 05:29:45.947692 pyfirebird-0.0.38/setup.cfg
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1301 2023-05-09 05:29:42.000000 pyfirebird-0.0.38/setup.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:29:45.943692 pyfirebird-0.0.38/src/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:29:45.943692 pyfirebird-0.0.38/src/firebird/
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)      169 2023-04-30 06:39:02.000000 pyfirebird-0.0.38/src/firebird/__init__.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)    10313 2023-05-09 05:29:15.000000 pyfirebird-0.0.38/src/firebird/base.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:29:45.943692 pyfirebird-0.0.38/src/firebird/cmd_tools/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 05:45:15.000000 pyfirebird-0.0.38/src/firebird/cmd_tools/__init__.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2903 2023-05-07 02:10:48.000000 pyfirebird-0.0.38/src/firebird/cmd_tools/executor.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     4964 2023-05-05 03:26:12.000000 pyfirebird-0.0.38/src/firebird/cmd_tools/executor_impl.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      649 2023-05-06 21:14:34.000000 pyfirebird-0.0.38/src/firebird/cmd_tools/fbconsole.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     3083 2023-05-09 02:04:29.000000 pyfirebird-0.0.38/src/firebird/cmd_tools/pipeline.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2603 2023-05-09 02:43:23.000000 pyfirebird-0.0.38/src/firebird/cmd_tools/pipeline_impl.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2972 2023-04-30 05:32:50.000000 pyfirebird-0.0.38/src/firebird/rabbitmq.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:29:45.943692 pyfirebird-0.0.38/src/firebird/utils/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-05-05 02:58:25.000000 pyfirebird-0.0.38/src/firebird/utils/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4359 2023-05-05 02:56:50.000000 pyfirebird-0.0.38/src/firebird/utils/checkpoint.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     6296 2023-05-09 02:11:15.000000 pyfirebird-0.0.38/src/firebird/zkdb.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:29:45.943692 pyfirebird-0.0.38/src/firebirdconsole/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-06 20:57:08.000000 pyfirebird-0.0.38/src/firebirdconsole/__init__.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:29:45.943692 pyfirebird-0.0.38/src/firebirdconsole/firebirdconsole/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-06 20:05:23.000000 pyfirebird-0.0.38/src/firebirdconsole/firebirdconsole/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-05-06 20:05:23.000000 pyfirebird-0.0.38/src/firebirdconsole/firebirdconsole/asgi.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3803 2023-05-07 02:13:47.000000 pyfirebird-0.0.38/src/firebirdconsole/firebirdconsole/settings.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      836 2023-05-06 20:43:13.000000 pyfirebird-0.0.38/src/firebirdconsole/firebirdconsole/urls.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-05-06 20:05:23.000000 pyfirebird-0.0.38/src/firebirdconsole/firebirdconsole/wsgi.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:29:45.943692 pyfirebird-0.0.38/src/firebirdconsole/ui/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-06 20:06:08.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       63 2023-05-06 20:06:08.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/admin.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-05-06 20:35:46.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/apps.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:29:45.943692 pyfirebird-0.0.38/src/firebirdconsole/ui/migrations/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-06 20:06:08.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/migrations/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       57 2023-05-06 20:06:08.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/models.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:29:45.943692 pyfirebird-0.0.38/src/firebirdconsole/ui/static/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:29:45.943692 pyfirebird-0.0.38/src/firebirdconsole/ui/static/images/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)   126365 2023-05-04 00:03:29.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/static/images/logo.jpeg
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:29:45.943692 pyfirebird-0.0.38/src/firebirdconsole/ui/static/js-bundle/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)  1548450 2023-05-09 03:56:06.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/static/js-bundle/home.js
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)   290225 2023-05-09 05:01:10.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/static/js-bundle/pipeline.js
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:29:45.943692 pyfirebird-0.0.38/src/firebirdconsole/ui/templates/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3817 2023-05-08 02:11:53.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/templates/application.html
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      217 2023-05-06 20:12:44.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/templates/index.html
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:29:45.943692 pyfirebird-0.0.38/src/firebirdconsole/ui/templatetags/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 00:25:05.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/templatetags/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      639 2023-05-09 00:25:31.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/templatetags/app_filters.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-05-06 20:06:08.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/tests.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      372 2023-05-09 03:57:30.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/urls.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      571 2023-05-08 02:38:33.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/view_tools.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:29:45.943692 pyfirebird-0.0.38/src/firebirdconsole/ui/views/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       54 2023-05-09 04:03:37.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/views/__init__.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:29:45.943692 pyfirebird-0.0.38/src/firebirdconsole/ui/views/apis/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       48 2023-05-09 04:06:17.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/views/apis/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1681 2023-05-09 05:21:55.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/views/apis/main.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      288 2023-05-09 00:32:38.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/views/home.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      387 2023-05-09 04:03:49.000000 pyfirebird-0.0.38/src/firebirdconsole/ui/views/pipeline.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-09 05:29:45.947692 pyfirebird-0.0.38/src/pyfirebird.egg-info/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-05-09 05:29:45.000000 pyfirebird-0.0.38/src/pyfirebird.egg-info/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1709 2023-05-09 05:29:45.000000 pyfirebird-0.0.38/src/pyfirebird.egg-info/SOURCES.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-05-09 05:29:45.000000 pyfirebird-0.0.38/src/pyfirebird.egg-info/dependency_links.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-05-09 05:29:45.000000 pyfirebird-0.0.38/src/pyfirebird.egg-info/entry_points.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       70 2023-05-09 05:29:45.000000 pyfirebird-0.0.38/src/pyfirebird.egg-info/requires.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       25 2023-05-09 05:29:45.000000 pyfirebird-0.0.38/src/pyfirebird.egg-info/top_level.txt
```

### Comparing `pyfirebird-0.0.37/setup.py` & `pyfirebird-0.0.38/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), "r") as f:
     README = f.read()
 
 # This call to setup() does all the work
 setup(
     name="pyfirebird",
-    version="0.0.37",
+    version="0.0.38",
     description="Streaming Data Processing Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/stonezhong/firebird",
     author="Stone Zhong",
     author_email="stonezhong@hotmail.com",
     license="MIT",
```

### Comparing `pyfirebird-0.0.37/src/firebird/base.py` & `pyfirebird-0.0.38/src/firebird/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,18 +66,16 @@
         
         pipeline._add_node(self)
     
     def to_json(self):
         ret = {
             "id": self.id,
             "description": self.description,
-            "ports": {}
+            "ports": [port.to_json() for port in self._ports_dict.values()]
         }
-        for port_id, port in self._ports_dict.items():
-            ret["ports"][port_id] = port.to_json()
         return ret
     
     def __getitem__(self, port_id:str) -> Optional["Port"]:
         return self.get_port(port_id)
 
     @property
     def input_port_ids(self):
```

### Comparing `pyfirebird-0.0.37/src/firebird/cmd_tools/executor.py` & `pyfirebird-0.0.38/src/firebird/cmd_tools/executor.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.37/src/firebird/cmd_tools/executor_impl.py` & `pyfirebird-0.0.38/src/firebird/cmd_tools/executor_impl.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.37/src/firebird/cmd_tools/fbconsole.py` & `pyfirebird-0.0.38/src/firebird/cmd_tools/fbconsole.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.37/src/firebird/cmd_tools/pipeline.py` & `pyfirebird-0.0.38/src/firebird/cmd_tools/pipeline.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.37/src/firebird/cmd_tools/pipeline_impl.py` & `pyfirebird-0.0.38/src/firebird/cmd_tools/pipeline_impl.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.37/src/firebird/rabbitmq.py` & `pyfirebird-0.0.38/src/firebird/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.37/src/firebird/utils/checkpoint.py` & `pyfirebird-0.0.38/src/firebird/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.37/src/firebird/zkdb.py` & `pyfirebird-0.0.38/src/firebird/zkdb.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.37/src/firebirdconsole/firebirdconsole/settings.py` & `pyfirebird-0.0.38/src/firebirdconsole/firebirdconsole/settings.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.37/src/firebirdconsole/firebirdconsole/urls.py` & `pyfirebird-0.0.38/src/firebirdconsole/firebirdconsole/urls.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.37/src/firebirdconsole/ui/static/images/logo.jpeg` & `pyfirebird-0.0.38/src/firebirdconsole/ui/static/images/logo.jpeg`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.37/src/firebirdconsole/ui/static/js-bundle/home.js` & `pyfirebird-0.0.38/src/firebirdconsole/ui/static/js-bundle/home.js`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.37/src/firebirdconsole/ui/static/js-bundle/pipeline.js` & `pyfirebird-0.0.38/src/firebirdconsole/ui/static/js-bundle/pipeline.js`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.37/src/firebirdconsole/ui/templates/application.html` & `pyfirebird-0.0.38/src/firebirdconsole/ui/templates/application.html`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.37/src/firebirdconsole/ui/templatetags/app_filters.py` & `pyfirebird-0.0.38/src/firebirdconsole/ui/templatetags/app_filters.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.37/src/firebirdconsole/ui/view_tools.py` & `pyfirebird-0.0.38/src/firebirdconsole/ui/view_tools.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.37/src/firebirdconsole/ui/views/apis/main.py` & `pyfirebird-0.0.38/src/firebirdconsole/ui/views/apis/main.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.37/src/pyfirebird.egg-info/SOURCES.txt` & `pyfirebird-0.0.38/src/pyfirebird.egg-info/SOURCES.txt`

 * *Files identical despite different names*

