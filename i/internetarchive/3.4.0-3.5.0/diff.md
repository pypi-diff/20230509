# Comparing `tmp/internetarchive-3.4.0.tar.gz` & `tmp/internetarchive-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internetarchive-3.4.0.tar", last modified: Wed Apr  5 20:01:57 2023, max compression
+gzip compressed data, was "internetarchive-3.5.0.tar", last modified: Tue May  9 17:55:16 2023, max compression
```

## Comparing `internetarchive-3.4.0.tar` & `internetarchive-3.5.0.tar`

### file list

```diff
@@ -1,64 +1,67 @@
-drwxr-xr-x   0 jake       (501) staff       (20)        0 2023-04-05 20:01:57.553132 internetarchive-3.4.0/
--rw-r--r--   0 jake       (501) staff       (20)      427 2022-08-15 17:17:53.000000 internetarchive-3.4.0/AUTHORS.rst
--rw-r--r--   0 jake       (501) staff       (20)    32544 2023-04-05 19:47:30.000000 internetarchive-3.4.0/HISTORY.rst
--rw-r--r--   0 jake       (501) staff       (20)    34520 2021-12-09 01:11:21.000000 internetarchive-3.4.0/LICENSE
--rw-r--r--   0 jake       (501) staff       (20)       69 2021-12-09 01:11:21.000000 internetarchive-3.4.0/MANIFEST.in
--rw-r--r--   0 jake       (501) staff       (20)     2707 2023-04-05 20:01:57.553272 internetarchive-3.4.0/PKG-INFO
--rw-r--r--   0 jake       (501) staff       (20)     1766 2021-12-09 01:11:21.000000 internetarchive-3.4.0/README.rst
-drwxr-xr-x   0 jake       (501) staff       (20)        0 2023-04-05 20:01:57.545099 internetarchive-3.4.0/internetarchive/
--rw-r--r--   0 jake       (501) staff       (20)     2237 2022-06-15 19:17:01.000000 internetarchive-3.4.0/internetarchive/__init__.py
--rw-r--r--   0 jake       (501) staff       (20)       22 2023-04-05 19:47:45.000000 internetarchive-3.4.0/internetarchive/__version__.py
--rw-r--r--   0 jake       (501) staff       (20)    20049 2023-04-05 19:42:47.000000 internetarchive-3.4.0/internetarchive/api.py
--rw-r--r--   0 jake       (501) staff       (20)     2641 2022-05-09 19:53:33.000000 internetarchive-3.4.0/internetarchive/auth.py
--rw-r--r--   0 jake       (501) staff       (20)    11922 2022-05-25 17:26:41.000000 internetarchive-3.4.0/internetarchive/catalog.py
-drwxr-xr-x   0 jake       (501) staff       (20)        0 2023-04-05 20:01:57.548829 internetarchive-3.4.0/internetarchive/cli/
--rw-r--r--   0 jake       (501) staff       (20)     1297 2022-05-25 17:26:41.000000 internetarchive-3.4.0/internetarchive/cli/__init__.py
--rw-r--r--   0 jake       (501) staff       (20)     2528 2022-05-25 17:26:41.000000 internetarchive-3.4.0/internetarchive/cli/argparser.py
--rwxr-xr-x   0 jake       (501) staff       (20)     6068 2022-05-25 17:26:41.000000 internetarchive-3.4.0/internetarchive/cli/ia.py
--rw-r--r--   0 jake       (501) staff       (20)     4133 2022-05-25 17:26:41.000000 internetarchive-3.4.0/internetarchive/cli/ia_configure.py
--rw-r--r--   0 jake       (501) staff       (20)     6307 2022-05-25 17:26:41.000000 internetarchive-3.4.0/internetarchive/cli/ia_copy.py
--rw-r--r--   0 jake       (501) staff       (20)     5652 2022-05-25 17:26:41.000000 internetarchive-3.4.0/internetarchive/cli/ia_delete.py
--rw-r--r--   0 jake       (501) staff       (20)     9850 2023-04-05 19:41:25.000000 internetarchive-3.4.0/internetarchive/cli/ia_download.py
--rw-r--r--   0 jake       (501) staff       (20)     3002 2022-05-25 17:26:41.000000 internetarchive-3.4.0/internetarchive/cli/ia_list.py
--rw-r--r--   0 jake       (501) staff       (20)    12394 2023-01-19 17:53:42.000000 internetarchive-3.4.0/internetarchive/cli/ia_metadata.py
--rw-r--r--   0 jake       (501) staff       (20)     3225 2022-05-25 17:26:41.000000 internetarchive-3.4.0/internetarchive/cli/ia_move.py
--rw-r--r--   0 jake       (501) staff       (20)     3412 2023-04-03 23:01:06.000000 internetarchive-3.4.0/internetarchive/cli/ia_reviews.py
--rw-r--r--   0 jake       (501) staff       (20)     4859 2023-04-04 17:42:58.000000 internetarchive-3.4.0/internetarchive/cli/ia_search.py
--rw-r--r--   0 jake       (501) staff       (20)     6838 2023-04-04 17:42:58.000000 internetarchive-3.4.0/internetarchive/cli/ia_tasks.py
--rw-r--r--   0 jake       (501) staff       (20)    14348 2022-12-21 18:00:57.000000 internetarchive-3.4.0/internetarchive/cli/ia_upload.py
--rw-r--r--   0 jake       (501) staff       (20)     6715 2022-05-25 17:26:41.000000 internetarchive-3.4.0/internetarchive/config.py
--rw-r--r--   0 jake       (501) staff       (20)     1305 2022-05-06 00:42:03.000000 internetarchive-3.4.0/internetarchive/exceptions.py
--rw-r--r--   0 jake       (501) staff       (20)    15178 2023-04-05 18:57:45.000000 internetarchive-3.4.0/internetarchive/files.py
--rw-r--r--   0 jake       (501) staff       (20)    19287 2023-01-25 21:07:48.000000 internetarchive-3.4.0/internetarchive/iarequest.py
--rw-r--r--   0 jake       (501) staff       (20)    52830 2023-04-05 19:42:47.000000 internetarchive-3.4.0/internetarchive/item.py
--rw-r--r--   0 jake       (501) staff       (20)     9829 2023-01-30 18:34:54.000000 internetarchive-3.4.0/internetarchive/search.py
--rw-r--r--   0 jake       (501) staff       (20)    22967 2023-04-05 17:35:41.000000 internetarchive-3.4.0/internetarchive/session.py
--rw-r--r--   0 jake       (501) staff       (20)    13767 2022-09-21 16:38:56.000000 internetarchive-3.4.0/internetarchive/utils.py
-drwxr-xr-x   0 jake       (501) staff       (20)        0 2023-04-05 20:01:57.546215 internetarchive-3.4.0/internetarchive.egg-info/
--rw-r--r--   0 jake       (501) staff       (20)     2707 2023-04-05 20:01:57.000000 internetarchive-3.4.0/internetarchive.egg-info/PKG-INFO
--rw-r--r--   0 jake       (501) staff       (20)     1522 2023-04-05 20:01:57.000000 internetarchive-3.4.0/internetarchive.egg-info/SOURCES.txt
--rw-r--r--   0 jake       (501) staff       (20)        1 2023-04-05 20:01:57.000000 internetarchive-3.4.0/internetarchive.egg-info/dependency_links.txt
--rw-r--r--   0 jake       (501) staff       (20)       52 2023-04-05 20:01:57.000000 internetarchive-3.4.0/internetarchive.egg-info/entry_points.txt
--rw-r--r--   0 jake       (501) staff       (20)        1 2021-12-09 02:36:16.000000 internetarchive-3.4.0/internetarchive.egg-info/not-zip-safe
--rw-r--r--   0 jake       (501) staff       (20)      916 2023-04-05 20:01:57.000000 internetarchive-3.4.0/internetarchive.egg-info/requires.txt
--rw-r--r--   0 jake       (501) staff       (20)       16 2023-04-05 20:01:57.000000 internetarchive-3.4.0/internetarchive.egg-info/top_level.txt
--rw-r--r--   0 jake       (501) staff       (20)     2430 2023-04-05 20:01:57.553905 internetarchive-3.4.0/setup.cfg
--rw-r--r--   0 jake       (501) staff       (20)       38 2022-05-25 17:26:41.000000 internetarchive-3.4.0/setup.py
-drwxr-xr-x   0 jake       (501) staff       (20)        0 2023-04-05 20:01:57.551039 internetarchive-3.4.0/tests/
--rw-r--r--   0 jake       (501) staff       (20)        0 2021-12-09 01:11:21.000000 internetarchive-3.4.0/tests/__init__.py
-drwxr-xr-x   0 jake       (501) staff       (20)        0 2023-04-05 20:01:57.552790 internetarchive-3.4.0/tests/cli/
--rw-r--r--   0 jake       (501) staff       (20)     1047 2022-05-24 22:31:00.000000 internetarchive-3.4.0/tests/cli/test_argparser.py
--rw-r--r--   0 jake       (501) staff       (20)      541 2021-12-09 01:11:21.000000 internetarchive-3.4.0/tests/cli/test_ia.py
--rw-r--r--   0 jake       (501) staff       (20)     3972 2022-12-05 19:47:24.000000 internetarchive-3.4.0/tests/cli/test_ia_download.py
--rw-r--r--   0 jake       (501) staff       (20)     2759 2022-02-03 22:48:23.000000 internetarchive-3.4.0/tests/cli/test_ia_list.py
--rw-r--r--   0 jake       (501) staff       (20)     1563 2022-03-07 19:43:12.000000 internetarchive-3.4.0/tests/cli/test_ia_metadata.py
--rw-r--r--   0 jake       (501) staff       (20)     1490 2023-01-30 18:36:38.000000 internetarchive-3.4.0/tests/cli/test_ia_search.py
--rw-r--r--   0 jake       (501) staff       (20)    14563 2022-12-07 21:41:22.000000 internetarchive-3.4.0/tests/cli/test_ia_upload.py
--rw-r--r--   0 jake       (501) staff       (20)     3649 2023-04-04 17:42:58.000000 internetarchive-3.4.0/tests/conftest.py
--rw-r--r--   0 jake       (501) staff       (20)    14392 2022-12-07 20:32:10.000000 internetarchive-3.4.0/tests/test_api.py
--rw-r--r--   0 jake       (501) staff       (20)      418 2021-12-09 01:11:21.000000 internetarchive-3.4.0/tests/test_bad_data.py
--rw-r--r--   0 jake       (501) staff       (20)    14898 2022-04-26 18:19:02.000000 internetarchive-3.4.0/tests/test_config.py
--rw-r--r--   0 jake       (501) staff       (20)      243 2022-02-03 22:48:23.000000 internetarchive-3.4.0/tests/test_exceptions.py
--rw-r--r--   0 jake       (501) staff       (20)    26906 2022-08-15 17:17:53.000000 internetarchive-3.4.0/tests/test_item.py
--rw-r--r--   0 jake       (501) staff       (20)     4477 2022-05-06 00:42:03.000000 internetarchive-3.4.0/tests/test_session.py
--rw-r--r--   0 jake       (501) staff       (20)     3493 2022-05-06 00:42:03.000000 internetarchive-3.4.0/tests/test_utils.py
+drwxr-xr-x   0 jake       (501) staff       (20)        0 2023-05-09 17:55:16.758367 internetarchive-3.5.0/
+-rw-r--r--   0 jake       (501) staff       (20)      427 2022-08-15 17:17:53.000000 internetarchive-3.5.0/AUTHORS.rst
+-rw-r--r--   0 jake       (501) staff       (20)    32797 2023-05-09 17:53:50.000000 internetarchive-3.5.0/HISTORY.rst
+-rw-r--r--   0 jake       (501) staff       (20)    34520 2021-12-09 01:11:21.000000 internetarchive-3.5.0/LICENSE
+-rw-r--r--   0 jake       (501) staff       (20)       69 2021-12-09 01:11:21.000000 internetarchive-3.5.0/MANIFEST.in
+-rw-r--r--   0 jake       (501) staff       (20)     2687 2023-05-09 17:55:16.758437 internetarchive-3.5.0/PKG-INFO
+-rw-r--r--   0 jake       (501) staff       (20)     1766 2021-12-09 01:11:21.000000 internetarchive-3.5.0/README.rst
+drwxr-xr-x   0 jake       (501) staff       (20)        0 2023-05-09 17:55:16.751653 internetarchive-3.5.0/internetarchive/
+-rw-r--r--   0 jake       (501) staff       (20)     2237 2022-06-15 19:17:01.000000 internetarchive-3.5.0/internetarchive/__init__.py
+-rw-r--r--   0 jake       (501) staff       (20)       22 2023-05-09 17:53:21.000000 internetarchive-3.5.0/internetarchive/__version__.py
+-rw-r--r--   0 jake       (501) staff       (20)    20034 2023-05-01 17:00:08.000000 internetarchive-3.5.0/internetarchive/api.py
+-rw-r--r--   0 jake       (501) staff       (20)     2641 2022-05-09 19:53:33.000000 internetarchive-3.5.0/internetarchive/auth.py
+-rw-r--r--   0 jake       (501) staff       (20)    11922 2022-05-25 17:26:41.000000 internetarchive-3.5.0/internetarchive/catalog.py
+drwxr-xr-x   0 jake       (501) staff       (20)        0 2023-05-09 17:55:16.756549 internetarchive-3.5.0/internetarchive/cli/
+-rw-r--r--   0 jake       (501) staff       (20)     1297 2022-05-25 17:26:41.000000 internetarchive-3.5.0/internetarchive/cli/__init__.py
+-rw-r--r--   0 jake       (501) staff       (20)     2528 2022-05-25 17:26:41.000000 internetarchive-3.5.0/internetarchive/cli/argparser.py
+-rwxr-xr-x   0 jake       (501) staff       (20)     6068 2023-05-09 17:01:11.000000 internetarchive-3.5.0/internetarchive/cli/ia.py
+-rw-r--r--   0 jake       (501) staff       (20)     4133 2022-05-25 17:26:41.000000 internetarchive-3.5.0/internetarchive/cli/ia_configure.py
+-rw-r--r--   0 jake       (501) staff       (20)     6307 2022-05-25 17:26:41.000000 internetarchive-3.5.0/internetarchive/cli/ia_copy.py
+-rw-r--r--   0 jake       (501) staff       (20)     5652 2022-05-25 17:26:41.000000 internetarchive-3.5.0/internetarchive/cli/ia_delete.py
+-rw-r--r--   0 jake       (501) staff       (20)     9850 2023-04-05 19:41:25.000000 internetarchive-3.5.0/internetarchive/cli/ia_download.py
+-rw-r--r--   0 jake       (501) staff       (20)     3002 2022-05-25 17:26:41.000000 internetarchive-3.5.0/internetarchive/cli/ia_list.py
+-rw-r--r--   0 jake       (501) staff       (20)    12729 2023-05-01 17:25:57.000000 internetarchive-3.5.0/internetarchive/cli/ia_metadata.py
+-rw-r--r--   0 jake       (501) staff       (20)     3225 2022-05-25 17:26:41.000000 internetarchive-3.5.0/internetarchive/cli/ia_move.py
+-rw-r--r--   0 jake       (501) staff       (20)     3412 2023-04-03 23:01:06.000000 internetarchive-3.5.0/internetarchive/cli/ia_reviews.py
+-rw-r--r--   0 jake       (501) staff       (20)     4859 2023-04-04 17:42:58.000000 internetarchive-3.5.0/internetarchive/cli/ia_search.py
+-rw-r--r--   0 jake       (501) staff       (20)     6838 2023-04-04 17:42:58.000000 internetarchive-3.5.0/internetarchive/cli/ia_tasks.py
+-rw-r--r--   0 jake       (501) staff       (20)    14348 2023-05-01 16:59:46.000000 internetarchive-3.5.0/internetarchive/cli/ia_upload.py
+-rw-r--r--   0 jake       (501) staff       (20)        0 2022-05-25 17:26:41.000000 internetarchive-3.5.0/internetarchive/cli/py.typed
+-rw-r--r--   0 jake       (501) staff       (20)     6727 2023-05-01 17:00:08.000000 internetarchive-3.5.0/internetarchive/config.py
+-rw-r--r--   0 jake       (501) staff       (20)     1305 2022-05-06 00:42:03.000000 internetarchive-3.5.0/internetarchive/exceptions.py
+-rw-r--r--   0 jake       (501) staff       (20)    15178 2023-05-01 16:59:32.000000 internetarchive-3.5.0/internetarchive/files.py
+-rw-r--r--   0 jake       (501) staff       (20)    19447 2023-05-09 16:33:04.000000 internetarchive-3.5.0/internetarchive/iarequest.py
+-rw-r--r--   0 jake       (501) staff       (20)    53054 2023-05-01 17:29:00.000000 internetarchive-3.5.0/internetarchive/item.py
+-rw-r--r--   0 jake       (501) staff       (20)        0 2022-05-25 17:26:41.000000 internetarchive-3.5.0/internetarchive/py.typed
+-rw-r--r--   0 jake       (501) staff       (20)     9829 2023-01-30 18:34:54.000000 internetarchive-3.5.0/internetarchive/search.py
+-rw-r--r--   0 jake       (501) staff       (20)    22967 2023-04-05 17:35:41.000000 internetarchive-3.5.0/internetarchive/session.py
+-rw-r--r--   0 jake       (501) staff       (20)    13767 2022-09-21 16:38:56.000000 internetarchive-3.5.0/internetarchive/utils.py
+drwxr-xr-x   0 jake       (501) staff       (20)        0 2023-05-09 17:55:16.752595 internetarchive-3.5.0/internetarchive.egg-info/
+-rw-r--r--   0 jake       (501) staff       (20)     2687 2023-05-09 17:55:16.000000 internetarchive-3.5.0/internetarchive.egg-info/PKG-INFO
+-rw-r--r--   0 jake       (501) staff       (20)     1591 2023-05-09 17:55:16.000000 internetarchive-3.5.0/internetarchive.egg-info/SOURCES.txt
+-rw-r--r--   0 jake       (501) staff       (20)        1 2023-05-09 17:55:16.000000 internetarchive-3.5.0/internetarchive.egg-info/dependency_links.txt
+-rw-r--r--   0 jake       (501) staff       (20)       51 2023-05-09 17:55:16.000000 internetarchive-3.5.0/internetarchive.egg-info/entry_points.txt
+-rw-r--r--   0 jake       (501) staff       (20)        1 2021-12-09 02:36:16.000000 internetarchive-3.5.0/internetarchive.egg-info/not-zip-safe
+-rw-r--r--   0 jake       (501) staff       (20)      784 2023-05-09 17:55:16.000000 internetarchive-3.5.0/internetarchive.egg-info/requires.txt
+-rw-r--r--   0 jake       (501) staff       (20)       16 2023-05-09 17:55:16.000000 internetarchive-3.5.0/internetarchive.egg-info/top_level.txt
+-rw-r--r--   0 jake       (501) staff       (20)     1962 2023-05-01 17:00:08.000000 internetarchive-3.5.0/pyproject.toml
+-rw-r--r--   0 jake       (501) staff       (20)     2001 2023-05-09 17:55:16.758823 internetarchive-3.5.0/setup.cfg
+-rw-r--r--   0 jake       (501) staff       (20)       38 2022-05-25 17:26:41.000000 internetarchive-3.5.0/setup.py
+drwxr-xr-x   0 jake       (501) staff       (20)        0 2023-05-09 17:55:16.757506 internetarchive-3.5.0/tests/
+-rw-r--r--   0 jake       (501) staff       (20)        0 2021-12-09 01:11:21.000000 internetarchive-3.5.0/tests/__init__.py
+drwxr-xr-x   0 jake       (501) staff       (20)        0 2023-05-09 17:55:16.758279 internetarchive-3.5.0/tests/cli/
+-rw-r--r--   0 jake       (501) staff       (20)     1047 2022-05-24 22:31:00.000000 internetarchive-3.5.0/tests/cli/test_argparser.py
+-rw-r--r--   0 jake       (501) staff       (20)      541 2021-12-09 01:11:21.000000 internetarchive-3.5.0/tests/cli/test_ia.py
+-rw-r--r--   0 jake       (501) staff       (20)     3972 2022-12-05 19:47:24.000000 internetarchive-3.5.0/tests/cli/test_ia_download.py
+-rw-r--r--   0 jake       (501) staff       (20)     2759 2022-02-03 22:48:23.000000 internetarchive-3.5.0/tests/cli/test_ia_list.py
+-rw-r--r--   0 jake       (501) staff       (20)     1563 2022-03-07 19:43:12.000000 internetarchive-3.5.0/tests/cli/test_ia_metadata.py
+-rw-r--r--   0 jake       (501) staff       (20)     1490 2023-01-30 18:36:38.000000 internetarchive-3.5.0/tests/cli/test_ia_search.py
+-rw-r--r--   0 jake       (501) staff       (20)    14563 2022-12-07 21:41:22.000000 internetarchive-3.5.0/tests/cli/test_ia_upload.py
+-rw-r--r--   0 jake       (501) staff       (20)     3661 2023-05-01 17:00:08.000000 internetarchive-3.5.0/tests/conftest.py
+-rw-r--r--   0 jake       (501) staff       (20)    14392 2022-12-07 20:32:10.000000 internetarchive-3.5.0/tests/test_api.py
+-rw-r--r--   0 jake       (501) staff       (20)      418 2021-12-09 01:11:21.000000 internetarchive-3.5.0/tests/test_bad_data.py
+-rw-r--r--   0 jake       (501) staff       (20)    14898 2022-04-26 18:19:02.000000 internetarchive-3.5.0/tests/test_config.py
+-rw-r--r--   0 jake       (501) staff       (20)      243 2022-02-03 22:48:23.000000 internetarchive-3.5.0/tests/test_exceptions.py
+-rw-r--r--   0 jake       (501) staff       (20)    27172 2023-05-09 17:44:04.000000 internetarchive-3.5.0/tests/test_item.py
+-rw-r--r--   0 jake       (501) staff       (20)     4477 2022-05-06 00:42:03.000000 internetarchive-3.5.0/tests/test_session.py
+-rw-r--r--   0 jake       (501) staff       (20)     3493 2022-05-06 00:42:03.000000 internetarchive-3.5.0/tests/test_utils.py
```

### Comparing `internetarchive-3.4.0/HISTORY.rst` & `internetarchive-3.5.0/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 .. :changelog:
 
 Release History
 ---------------
 
+3.5.0 (2023-05-09)
+++++++++++++++++++
+
+**Bugfixes**
+
+- Fixed bug in ``ia metadata --insert`` where duplicate values were being added in
+  some cases
+
+**Features and Improvements**
+
+- Added timeout option for metadata writes. Set default to 60 seconds.
+
 3.4.0 (2023-04-05)
 ++++++++++++++++++
 
 **Features and Improvements**
 
 - Added parameters for filtering files based on their source value in files.xml.
 - Added support for downloading multiple files to stdout.
```

### Comparing `internetarchive-3.4.0/LICENSE` & `internetarchive-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/PKG-INFO` & `internetarchive-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: internetarchive
-Version: 3.4.0
+Version: 3.5.0
 Summary: A Python interface to archive.org.
 Home-page: https://github.com/jjjake/internetarchive
 Author: Jacob M. Johnson
 Author-email: jake@archive.org
 License: AGPL-3.0
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -74,9 +73,7 @@
 Documentation is available at `https://archive.org/services/docs/api/internetarchive <https://archive.org/services/docs/api/internetarchive>`_.
 
 
 Contributing
 ------------
 
 All contributions are welcome and appreciated. Please see `https://archive.org/services/docs/api/internetarchive/contributing.html <https://archive.org/services/docs/api/internetarchive/contributing.html>`_ for more details.
-
-
```

### Comparing `internetarchive-3.4.0/README.rst` & `internetarchive-3.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/__init__.py` & `internetarchive-3.5.0/internetarchive/__init__.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/api.py` & `internetarchive-3.5.0/internetarchive/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,16 @@
 
 from getpass import getpass
 from typing import Iterable, Mapping, MutableMapping
 
 import requests
 from urllib3 import Retry
 
-from internetarchive import auth, catalog
+from internetarchive import auth, catalog, files, item, search, session
 from internetarchive import config as config_module
-from internetarchive import files, item, search, session
 from internetarchive.exceptions import AuthenticationError
 
 
 def get_session(
     config: Mapping | None = None,
     config_file: str | None = None,
     debug: bool = False,
@@ -576,14 +575,14 @@
 
     :param secret_key: IA-S3 secret_key to use when making the given request.
 
     :returns: Archive.org use info.
     """
     u = "https://s3.us.archive.org"
     p = {"check_auth": 1}
-    r = requests.get(u, params=p, auth=auth.S3Auth(access_key, secret_key))
+    r = requests.get(u, params=p, auth=auth.S3Auth(access_key, secret_key), timeout=10)
     r.raise_for_status()
     j = r.json()
     if j.get("error"):
         raise AuthenticationError(j.get("error"))
     else:
         return j
```

### Comparing `internetarchive-3.4.0/internetarchive/auth.py` & `internetarchive-3.5.0/internetarchive/auth.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/catalog.py` & `internetarchive-3.5.0/internetarchive/catalog.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/cli/__init__.py` & `internetarchive-3.5.0/internetarchive/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/cli/argparser.py` & `internetarchive-3.5.0/internetarchive/cli/argparser.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/cli/ia.py` & `internetarchive-3.5.0/internetarchive/cli/ia.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/cli/ia_configure.py` & `internetarchive-3.5.0/internetarchive/cli/ia_configure.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/cli/ia_copy.py` & `internetarchive-3.5.0/internetarchive/cli/ia_copy.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/cli/ia_delete.py` & `internetarchive-3.5.0/internetarchive/cli/ia_delete.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/cli/ia_download.py` & `internetarchive-3.5.0/internetarchive/cli/ia_download.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/cli/ia_list.py` & `internetarchive-3.5.0/internetarchive/cli/ia_list.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/cli/ia_metadata.py` & `internetarchive-3.5.0/internetarchive/cli/ia_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,23 +18,25 @@
 
 """Retrieve and modify Archive.org metadata.
 
 usage:
     ia metadata <identifier>... [--exists | --formats] [--header=<key:value>...]
     ia metadata <identifier>... --modify=<key:value>... [--target=<target>]
                                 [--priority=<priority>] [--header=<key:value>...]
+                                [--timeout=<value>]
     ia metadata <identifier>... --remove=<key:value>... [--priority=<priority>]
-                                [--header=<key:value>...]
+                                [--header=<key:value>...] [--timeout=<value>]
     ia metadata <identifier>... [--append=<key:value>... | --append-list=<key:value>...]
                                 [--priority=<priority>] [--target=<target>]
-                                [--header=<key:value>...]
+                                [--header=<key:value>...] [--timeout=<value>]
     ia metadata <identifier>... --insert=<key:value>... [--priority=<priority>]
                                 [--target=<target>] [--header=<key:value>...]
+                                [--timeout=<value>]
     ia metadata --spreadsheet=<metadata.csv> [--priority=<priority>]
-                [--modify=<key:value>...] [--header=<key:value>...]
+                [--modify=<key:value>...] [--header=<key:value>...] [--timeout=<value>]
     ia metadata --help
 
 options:
     -h, --help
     -m, --modify=<key:value>            Modify the metadata of an item.
     -H, --header=<key:value>...         S3 HTTP headers to send with your request.
     -t, --target=<target>               The metadata target to modify.
@@ -46,14 +48,15 @@
                                         input.
     -e, --exists                        Check if an item exists
     -F, --formats                       Return the file-formats the given item contains.
     -p, --priority=<priority>           Set the task priority.
     -r, --remove=<key:value>...         Remove <key:value> from a metadata element.
                                         Works on both single and multi-field metadata
                                         elements.
+    --timeout=<value>                   Set a timeout for metadata writes.
 """
 from __future__ import annotations
 
 import csv
 import os
 import sys
 from collections import defaultdict
@@ -77,15 +80,16 @@
 def modify_metadata(item: item.Item, metadata: Mapping, args: Mapping) -> Response:
     append = bool(args['--append'])
     append_list = bool(args['--append-list'])
     insert = bool(args['--insert'])
     try:
         r = item.modify_metadata(metadata, target=args['--target'], append=append,
                                  priority=args['--priority'], append_list=append_list,
-                                 headers=args['--header'], insert=insert)
+                                 headers=args['--header'], insert=insert,
+                                 timeout=args['--timeout'])
         assert isinstance(r, Response)  # mypy: modify_metadata() -> Request | Response
     except ItemLocateError as exc:
         print(f'{item.identifier} - error: {exc}', file=sys.stderr)
         sys.exit(1)
     if not r.json()['success']:
         error_msg = r.json()['error']
         etype = 'warning' if 'no changes' in r.text else 'error'
@@ -180,14 +184,15 @@
         '--append-list': list,
         '--insert': list,
         '--remove': list,
         '--spreadsheet': Or(None, And(lambda f: os.path.exists(f),
                             error='<file> should be a readable file or directory.')),
         '--target': Or(None, str),
         '--priority': Or(None, Use(int, error='<priority> should be an integer.')),
+        '--timeout': Or(None, str),
     })
     try:
         args = s.validate(args)
     except SchemaError as exc:
         print(f'{exc}\n{printable_usage(__doc__)}', file=sys.stderr)
         sys.exit(1)
```

### Comparing `internetarchive-3.4.0/internetarchive/cli/ia_move.py` & `internetarchive-3.5.0/internetarchive/cli/ia_move.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/cli/ia_reviews.py` & `internetarchive-3.5.0/internetarchive/cli/ia_reviews.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/cli/ia_search.py` & `internetarchive-3.5.0/internetarchive/cli/ia_search.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/cli/ia_tasks.py` & `internetarchive-3.5.0/internetarchive/cli/ia_tasks.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/cli/ia_upload.py` & `internetarchive-3.5.0/internetarchive/cli/ia_upload.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/config.py` & `internetarchive-3.5.0/internetarchive/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from internetarchive.utils import deep_update
 
 
 def get_auth_config(email: str, password: str, host: str = 'archive.org') -> dict:
     u = f'https://{host}/services/xauthn/'
     p = {'op': 'login'}
     d = {'email': email, 'password': password}
-    r = requests.post(u, params=p, data=d)
+    r = requests.post(u, params=p, data=d, timeout=10)
     j = r.json()
     if not j.get('success'):
         try:
             msg = j['values']['reason']
         except KeyError:
             msg = j['error']
         if msg == 'account_not_found':
```

### Comparing `internetarchive-3.4.0/internetarchive/exceptions.py` & `internetarchive-3.5.0/internetarchive/exceptions.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/files.py` & `internetarchive-3.5.0/internetarchive/files.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/iarequest.py` & `internetarchive-3.5.0/internetarchive/iarequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         self.prepare_hooks(hooks)
 
     def prepare_body(self, metadata, source_metadata, target, priority, append,
                      append_list, insert):
         priority = priority or -5
 
         if not source_metadata:
-            r = requests.get(self.url)
+            r = requests.get(self.url, timeout=10)
             source_metadata = r.json()
 
         # Write to many targets
         if (isinstance(metadata, list)
                 or any('/' in k for k in metadata)
                 or all(isinstance(k, dict) for k in metadata.values())):
             changes = []
@@ -450,15 +450,19 @@
             # If no index is provided, e.g. `collection[i]`, assume 0
             if not index:
                 index = 0
             _key = rm_index(key)
             if not isinstance(source_metadata[_key], list):
                 source_metadata[_key] = [source_metadata[_key]]
             source_metadata[_key].insert(index, metadata[key])
-            prepared_metadata[_key] = source_metadata[_key]
+            insert_md = []
+            for _v in source_metadata[_key]:
+                if _v not in insert_md and _v:
+                    insert_md.append(_v)
+            prepared_metadata[_key] = insert_md
         else:
             prepared_metadata[key] = metadata[key]
 
     # Remove values from metadata if value is REMOVE_TAG.
     _done = []
     for key in indexed_keys:
         # Filter None values from items with arrays as values
```

### Comparing `internetarchive-3.4.0/internetarchive/item.py` & `internetarchive-3.5.0/internetarchive/item.py`

 * *Files 0% similar despite different names*

```diff
@@ -773,15 +773,16 @@
                         append_list: bool = False,
                         insert: bool = False,
                         priority: int = 0,
                         access_key: str | None = None,
                         secret_key: str | None = None,
                         debug: bool = False,
                         headers: Mapping | None = None,
-                        request_kwargs: Mapping | None = None) -> Request | Response:
+                        request_kwargs: Mapping | None = None,
+                        timeout: int | float | None = None) -> Request | Response:
         """Modify the metadata of an existing item on Archive.org.
 
         Note: The Metadata Write API does not yet comply with the
         latest Json-Patch standard. It currently complies with `version 02
         <https://tools.ietf.org/html/draft-ietf-appsawg-json-patch-02>`__.
 
         :param metadata: Metadata used to update the item.
@@ -807,14 +808,18 @@
         """
         append = bool(append)
         access_key = access_key or self.session.access_key
         secret_key = secret_key or self.session.secret_key
         debug = bool(debug)
         headers = headers or {}
         request_kwargs = request_kwargs or {}
+        if timeout:
+            request_kwargs["timeout"] = float(timeout)  # type: ignore
+        else:
+            request_kwargs["timeout"] = 60  # type: ignore
 
         _headers = self.session.headers.copy()
         _headers.update(headers)
 
         url = f'{self.session.protocol}//{self.session.host}/metadata/{self.identifier}'
         # TODO: currently files and metadata targets do not support dict's,
         # but they might someday?? refactor this check.
```

### Comparing `internetarchive-3.4.0/internetarchive/search.py` & `internetarchive-3.5.0/internetarchive/search.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/session.py` & `internetarchive-3.5.0/internetarchive/session.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive/utils.py` & `internetarchive-3.5.0/internetarchive/utils.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/internetarchive.egg-info/PKG-INFO` & `internetarchive-3.5.0/internetarchive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: internetarchive
-Version: 3.4.0
+Version: 3.5.0
 Summary: A Python interface to archive.org.
 Home-page: https://github.com/jjjake/internetarchive
 Author: Jacob M. Johnson
 Author-email: jake@archive.org
 License: AGPL-3.0
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -74,9 +73,7 @@
 Documentation is available at `https://archive.org/services/docs/api/internetarchive <https://archive.org/services/docs/api/internetarchive>`_.
 
 
 Contributing
 ------------
 
 All contributions are welcome and appreciated. Please see `https://archive.org/services/docs/api/internetarchive/contributing.html <https://archive.org/services/docs/api/internetarchive/contributing.html>`_ for more details.
-
-
```

### Comparing `internetarchive-3.4.0/internetarchive.egg-info/SOURCES.txt` & `internetarchive-3.5.0/internetarchive.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 AUTHORS.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 internetarchive/__init__.py
 internetarchive/__version__.py
 internetarchive/api.py
 internetarchive/auth.py
 internetarchive/catalog.py
 internetarchive/config.py
 internetarchive/exceptions.py
 internetarchive/files.py
 internetarchive/iarequest.py
 internetarchive/item.py
+internetarchive/py.typed
 internetarchive/search.py
 internetarchive/session.py
 internetarchive/utils.py
 internetarchive.egg-info/PKG-INFO
 internetarchive.egg-info/SOURCES.txt
 internetarchive.egg-info/dependency_links.txt
 internetarchive.egg-info/entry_points.txt
@@ -35,14 +37,15 @@
 internetarchive/cli/ia_list.py
 internetarchive/cli/ia_metadata.py
 internetarchive/cli/ia_move.py
 internetarchive/cli/ia_reviews.py
 internetarchive/cli/ia_search.py
 internetarchive/cli/ia_tasks.py
 internetarchive/cli/ia_upload.py
+internetarchive/cli/py.typed
 tests/__init__.py
 tests/conftest.py
 tests/test_api.py
 tests/test_bad_data.py
 tests/test_config.py
 tests/test_exceptions.py
 tests/test_item.py
```

### Comparing `internetarchive-3.4.0/setup.cfg` & `internetarchive-3.5.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -42,33 +42,28 @@
 [options.extras_require]
 all = 
 	%(dev)s
 	%(test)s
 	%(types)s
 dev = 
 	black
-	flake8
-	flake8-2020
-	flake8-bugbear
-	flake8-comprehensions
 	mypy
 	pre-commit
 	pytest
-	pyupgrade
 	safety
 	setuptools
 docs = 
 	alabaster==0.7.12
 	docutils<0.18
 	sphinx==4.5.0
 	sphinx-autodoc-typehints==1.18.1
 test = 
-	flake8==6.0.0
 	pytest==7.1.2
 	responses==0.20.0
+	ruff==0.0.261
 types = 
 	tqdm-stubs>=0.2.0
 	types-colorama
 	types-docopt>=0.6.10,<0.7.0
 	types-jsonpatch>=0.1.0a0
 	types-pygments
 	types-requests>=2.25.0,<3.0.0
@@ -78,42 +73,24 @@
 
 [options.package_data]
 * = py.typed
 
 [codespell]
 ignore-words-list = alers
 
-[flake8]
-ignore = E128,E722,F401,F841,W503,W605
-exclude = .git,__pycache__,docs/source/conf.py,old,build,dist,.tox
-max-complexity = 43
-max-line-length = 102
-per-file-ignores = 
-	./tests/conftest.py: F811
-	./tests/cli/test_ia_list.py: E741
-	./tests/test_api.py: E712
-show-source = true
-statistics = true
-
 [mypy]
 exclude = ^\.git/|^__pycache__/|^docs/source/conf.py$|^old/|^build/|^dist/|\.tox
 python_version = 3.9
 install_types = True
 pretty = True
 scripts_are_modules = True
 show_error_codes = True
 show_error_context = True
 
-[isort]
-profile = black
-
 [tool:black]
 line-length = 102
 skip-string-normalization = true
 
-[bdist_wheel]
-universal = 1
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `internetarchive-3.4.0/tests/cli/test_argparser.py` & `internetarchive-3.5.0/tests/cli/test_argparser.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/tests/cli/test_ia.py` & `internetarchive-3.5.0/tests/cli/test_ia.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/tests/cli/test_ia_download.py` & `internetarchive-3.5.0/tests/cli/test_ia_download.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/tests/cli/test_ia_list.py` & `internetarchive-3.5.0/tests/cli/test_ia_list.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/tests/cli/test_ia_metadata.py` & `internetarchive-3.5.0/tests/cli/test_ia_metadata.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/tests/cli/test_ia_search.py` & `internetarchive-3.5.0/tests/cli/test_ia_search.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/tests/cli/test_ia_upload.py` & `internetarchive-3.5.0/tests/cli/test_ia_upload.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/tests/conftest.py` & `internetarchive-3.5.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,42 +97,42 @@
 
     def mock_all_downloads(self, num_calls=1, body='test content', protocol='https?'):
         url = re.compile(f'{protocol}://archive.org/download/.*')
         for _ in range(6):
             self.add(responses.GET, url, body=body)
 
 
-@pytest.fixture
+@pytest.fixture()
 def tmpdir_ch(tmpdir):
     tmpdir.chdir()
     return tmpdir
 
 
-@pytest.fixture
+@pytest.fixture()
 def nasa_mocker():
     with IaRequestsMock() as mocker:
         mocker.add_metadata_mock('nasa')
         yield mocker
 
 
-@pytest.fixture
+@pytest.fixture()
 def nasa_item():
     session = get_session()
     with IaRequestsMock() as mocker:
         mocker.add_metadata_mock('nasa')
         yield session.get_item('nasa')
 
 
-@pytest.fixture
+@pytest.fixture()
 def session():
     return get_session(config={'s3': {'access': 'access', 'secret': 'secret'}})
 
 
-@pytest.fixture
+@pytest.fixture()
 def nasa_metadata():
     return json.loads(load_test_data_file('metadata/nasa.json'))
 
 
 # TODO: Why is this function defined twice in this file?  See issue #505
-@pytest.fixture  # type: ignore
+@pytest.fixture()  # type: ignore
 def nasa_item(nasa_mocker):
     return get_item('nasa')
```

### Comparing `internetarchive-3.4.0/tests/test_api.py` & `internetarchive-3.5.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/tests/test_config.py` & `internetarchive-3.5.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/tests/test_item.py` & `internetarchive-3.5.0/tests/test_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import os
 import re
 import types
 from copy import deepcopy
 
 import pytest
 import responses
@@ -210,22 +211,23 @@
         nasa_item = get_item('nasa')
         nasa_item.download(files='nasa_meta.xml')
         nasa_item.download(files='nasa_meta.xml', checksum=True)
 
         assert load_file('nasa/nasa_meta.xml') == 'overwrite based on md5'
 
         # test no overwrite based on checksum.
-        rsps.reset()
-        rsps.add(responses.GET, DOWNLOAD_URL_RE,
-                 body=load_test_data_file('nasa_meta.xml'))
-        nasa_item.download(files='nasa_meta.xml', checksum=True)
-        nasa_item.download(files='nasa_meta.xml', checksum=True)
+        with caplog.at_level(logging.DEBUG):
+            rsps.reset()
+            rsps.add(responses.GET, DOWNLOAD_URL_RE,
+                     body=load_test_data_file('nasa_meta.xml'))
+            nasa_item.download(files='nasa_meta.xml', checksum=True, verbose=True)
+            nasa_item.download(files='nasa_meta.xml', checksum=True, verbose=True)
 
-        assert 'skipping nasa' in caplog.text
-        assert 'nasa_meta.xml, file already exists based on checksum.' in caplog.text
+            assert 'skipping nasa' in caplog.text
+            assert 'nasa_meta.xml, file already exists based on checksum.' in caplog.text
 
 
 def test_download_destdir(tmpdir, nasa_item):
     tmpdir.chdir()
     with IaRequestsMock() as rsps:
         rsps.add(responses.GET, DOWNLOAD_URL_RE, body='new destdir')
         dest = os.path.join(str(tmpdir), 'new destdir')
@@ -274,18 +276,17 @@
 
 
 def test_download_verbose(tmpdir, capsys, nasa_item):
     tmpdir.chdir()
     with IaRequestsMock(assert_all_requests_are_fired=False) as rsps:
         rsps.add(responses.GET, DOWNLOAD_URL_RE,
                  body='no dest dir',
-                 adding_headers={'content-length': '100'})
+                 adding_headers={'content-length': '11'})
         nasa_item.download(files='nasa_meta.xml', verbose=True)
         out, err = capsys.readouterr()
-        print(repr(err))
         assert 'downloading nasa_meta.xml' in err
 
 
 def test_download_dark_item(tmpdir, capsys, nasa_metadata, session):
     tmpdir.chdir()
     with IaRequestsMock(assert_all_requests_are_fired=False) as rsps:
         nasa_metadata['metadata']['identifier'] = 'dark-item'
@@ -402,15 +403,18 @@
             '<Error><Code>SlowDown</Code><Message>Please reduce your request rate.'
             '</Message><Resource>simulated error caused by x-(amz|archive)-simulate-error'
             ', try x-archive-simulate-error:help</Resource><RequestId>d36ec445-8d4a-4a64-'
             'a110-f67af6ee2c2a</RequestId></Error>')
     with IaRequestsMock(assert_all_requests_are_fired=False) as rsps:
         _expected_headers = deepcopy(EXPECTED_S3_HEADERS)
         rsps.add(responses.GET, S3_URL_RE,
-                 body='{"over_limit": "1"}')
+                 body='{"over_limit": "1"}',
+                 adding_headers={'content-length': '19'}
+                 )
+        _expected_headers['content-length'] = '296'
         rsps.add(responses.PUT, S3_URL_RE,
                  body=body,
                  adding_headers=_expected_headers,
                  status=503)
         try:
             nasa_item.upload(NASA_METADATA_PATH,
                              access_key='a',
@@ -492,14 +496,15 @@
             '<Error><Code>BadDigest</Code><Message>The Content-MD5 you specified did not '
             'match what we received.</Message><Resource>content-md5 submitted with PUT: '
             'foo != received data md5: 70871f9fce8dd23853d6e42417356b05also not equal to '
             'base64 version: cIcfn86N0jhT1uQkFzVrBQ==</Resource><RequestId>ec03fe7c-e123-'
             '4133-a207-3141d4d74096</RequestId></Error>')
 
     _expected_headers = deepcopy(EXPECTED_S3_HEADERS)
+    _expected_headers['content-length'] = '383'
     del _expected_headers['x-archive-meta00-scanner']
     tmpdir.chdir()
     test_file = os.path.join(str(tmpdir), 'test.txt')
     with open(test_file, 'w') as fh:
         fh.write('test delete')
 
     with IaRequestsMock(assert_all_requests_are_fired=False) as rsps:
```

### Comparing `internetarchive-3.4.0/tests/test_session.py` & `internetarchive-3.5.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `internetarchive-3.4.0/tests/test_utils.py` & `internetarchive-3.5.0/tests/test_utils.py`

 * *Files identical despite different names*

