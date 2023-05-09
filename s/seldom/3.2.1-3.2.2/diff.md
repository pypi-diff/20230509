# Comparing `tmp/seldom-3.2.1.tar.gz` & `tmp/seldom-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\seldom-3.2.1.tar", last modified: Thu Apr 13 16:55:00 2023, max compression
+gzip compressed data, was "seldom-3.2.2.tar", last modified: Tue May  9 16:56:34 2023, max compression
```

## Comparing `seldom-3.2.1.tar` & `seldom-3.2.2.tar`

### file list

```diff
@@ -1,109 +1,112 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.427087 seldom-3.2.1/
--rw-rw-rw-   0        0        0    11565 2022-12-06 15:57:51.000000 seldom-3.2.1/LICENSE
--rw-rw-rw-   0        0        0       44 2022-12-06 15:57:51.000000 seldom-3.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1118 2023-04-13 16:55:00.426085 seldom-3.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     9605 2023-03-19 02:36:19.000000 seldom-3.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.269780 seldom-3.2.1/demo/
--rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.1/demo/__init__.py
--rw-rw-rw-   0        0        0     1164 2023-01-11 15:24:10.000000 seldom-3.2.1/demo/confrun.py
--rw-rw-rw-   0        0        0     1583 2022-12-06 15:57:51.000000 seldom-3.2.1/demo/run.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.272782 seldom-3.2.1/demo/test_dir/
--rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.1/demo/test_dir/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.275785 seldom-3.2.1/demo/test_dir/api_case/
--rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.1/demo/test_dir/api_case/__init__.py
--rw-rw-rw-   0        0        0     3713 2023-01-11 15:24:10.000000 seldom-3.2.1/demo/test_dir/api_case/test_http_demo.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.283790 seldom-3.2.1/demo/test_dir/app_case/
--rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.1/demo/test_dir/app_case/__init__.py
--rw-rw-rw-   0        0        0      994 2022-12-06 15:57:51.000000 seldom-3.2.1/demo/test_dir/app_case/test_first_demo.py
--rw-rw-rw-   0        0        0     1231 2023-03-19 02:35:00.000000 seldom-3.2.1/demo/test_dir/app_case/test_po_demo.py
--rw-rw-rw-   0        0        0      875 2023-03-14 15:43:32.000000 seldom-3.2.1/demo/test_dir/app_case/test_u2_demo.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.296793 seldom-3.2.1/demo/test_dir/web_case/
--rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.1/demo/test_dir/web_case/__init__.py
--rw-rw-rw-   0        0        0      579 2022-12-06 15:57:51.000000 seldom-3.2.1/demo/test_dir/web_case/test_data_demo.py
--rw-rw-rw-   0        0        0     4287 2023-01-11 15:24:10.000000 seldom-3.2.1/demo/test_dir/web_case/test_ddt_demo.py
--rw-rw-rw-   0        0        0      589 2023-01-11 15:24:10.000000 seldom-3.2.1/demo/test_dir/web_case/test_first_demo.py
--rw-rw-rw-   0        0        0      846 2022-12-06 15:57:51.000000 seldom-3.2.1/demo/test_dir/web_case/test_fixture_demo.py
--rw-rw-rw-   0        0        0      953 2023-01-11 15:24:10.000000 seldom-3.2.1/demo/test_dir/web_case/test_playwright_demo.py
--rw-rw-rw-   0        0        0     1194 2023-03-19 02:31:03.000000 seldom-3.2.1/demo/test_dir/web_case/test_po_demo.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.303852 seldom-3.2.1/proj/
--rw-rw-rw-   0        0        0        0 2022-12-08 16:29:03.000000 seldom-3.2.1/proj/__init__.py
--rw-rw-rw-   0        0        0      110 2022-12-12 15:41:44.000000 seldom-3.2.1/proj/confrun.py
--rw-rw-rw-   0        0        0     1031 2022-12-12 15:42:40.000000 seldom-3.2.1/proj/loader.py
--rw-rw-rw-   0        0        0      293 2022-12-12 15:41:28.000000 seldom-3.2.1/proj/run.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.318852 seldom-3.2.1/seldom/
--rw-rw-rw-   0        0        0     1305 2023-04-13 16:51:46.000000 seldom-3.2.1/seldom/__init__.py
--rw-rw-rw-   0        0        0     5373 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/appdriver.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.338853 seldom-3.2.1/seldom/appium_lab/
--rw-rw-rw-   0        0        0     1669 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/appium_lab/__init__.py
--rw-rw-rw-   0        0        0     3909 2023-03-13 16:12:23.000000 seldom-3.2.1/seldom/appium_lab/action.py
--rw-rw-rw-   0        0        0     7248 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/appium_lab/find.py
--rw-rw-rw-   0        0        0     2997 2023-03-13 16:12:23.000000 seldom-3.2.1/seldom/appium_lab/keyboard.py
--rw-rw-rw-   0        0        0     1721 2023-03-13 16:12:23.000000 seldom-3.2.1/seldom/appium_lab/switch.py
--rw-rw-rw-   0        0        0    11006 2023-03-13 16:12:38.000000 seldom-3.2.1/seldom/case.py
--rw-rw-rw-   0        0        0    13177 2022-12-16 17:09:13.000000 seldom-3.2.1/seldom/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.348853 seldom-3.2.1/seldom/db_operation/
--rw-rw-rw-   0        0        0       64 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/db_operation/__init__.py
--rw-rw-rw-   0        0        0     1698 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/db_operation/base_db.py
--rw-rw-rw-   0        0        0      715 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/db_operation/mongo_db.py
--rw-rw-rw-   0        0        0     3958 2023-04-13 16:34:19.000000 seldom-3.2.1/seldom/db_operation/mssql_db.py
--rw-rw-rw-   0        0        0     4265 2023-04-13 16:36:12.000000 seldom-3.2.1/seldom/db_operation/mysql_db.py
--rw-rw-rw-   0        0        0     3159 2023-04-13 16:31:28.000000 seldom-3.2.1/seldom/db_operation/sqlite_db.py
--rw-rw-rw-   0        0        0     5665 2023-03-14 15:43:32.000000 seldom-3.2.1/seldom/driver.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.352852 seldom-3.2.1/seldom/har2case/
--rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/har2case/__init__.py
--rw-rw-rw-   0        0        0     4014 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/har2case/core.py
--rw-rw-rw-   0        0        0     1171 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/har2case/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.358856 seldom-3.2.1/seldom/logging/
--rw-rw-rw-   0        0        0       48 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/logging/__init__.py
--rw-rw-rw-   0        0        0     1101 2023-01-02 07:33:41.000000 seldom-3.2.1/seldom/logging/exceptions.py
--rw-rw-rw-   0        0        0     1887 2023-03-16 00:03:22.000000 seldom-3.2.1/seldom/logging/log.py
--rw-rw-rw-   0        0        0    11842 2023-03-19 02:45:19.000000 seldom-3.2.1/seldom/request.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.371857 seldom-3.2.1/seldom/running/
--rw-rw-rw-   0        0        0     2477 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/running/DebugTestRunner.py
--rw-rw-rw-   0        0        0      803 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/running/__init__.py
--rw-rw-rw-   0        0        0      561 2023-03-14 15:43:32.000000 seldom-3.2.1/seldom/running/config.py
--rw-rw-rw-   0        0        0     1467 2022-12-07 17:25:01.000000 seldom-3.2.1/seldom/running/loader.py
--rw-rw-rw-   0        0        0     7450 2022-12-15 14:14:22.000000 seldom-3.2.1/seldom/running/loader_extend.py
--rw-rw-rw-   0        0        0     1006 2022-12-12 16:47:54.000000 seldom-3.2.1/seldom/running/loader_hook.py
--rw-rw-rw-   0        0        0    14706 2023-03-14 15:43:32.000000 seldom-3.2.1/seldom/running/runner.py
--rw-rw-rw-   0        0        0     2670 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/skip.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.381856 seldom-3.2.1/seldom/testdata/
--rw-rw-rw-   0        0        0       28 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/testdata/__init__.py
--rw-rw-rw-   0        0        0     4164 2023-03-13 16:12:23.000000 seldom-3.2.1/seldom/testdata/conversion.py
--rw-rw-rw-   0        0        0    10749 2023-04-03 16:11:58.000000 seldom-3.2.1/seldom/testdata/parameterization.py
--rw-rw-rw-   0        0        0    18847 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/testdata/random_data.py
--rw-rw-rw-   0        0        0    11986 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/testdata/random_func.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.407083 seldom-3.2.1/seldom/utils/
--rw-rw-rw-   0        0        0      232 2023-04-01 06:05:16.000000 seldom-3.2.1/seldom/utils/__init__.py
--rw-rw-rw-   0        0        0     5564 2023-04-01 06:05:16.000000 seldom-3.2.1/seldom/utils/cache.py
--rw-rw-rw-   0        0        0     1067 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/utils/curlify.py
--rw-rw-rw-   0        0        0     2395 2023-03-13 16:12:38.000000 seldom-3.2.1/seldom/utils/diff.py
--rw-rw-rw-   0        0        0     3280 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/utils/file_extend.py
--rw-rw-rw-   0        0        0      438 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/utils/genson.py
--rw-rw-rw-   0        0        0      243 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/utils/jmespath.py
--rw-rw-rw-   0        0        0    10473 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/utils/jsonpath.py
--rw-rw-rw-   0        0        0     3964 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/utils/klook.py
--rw-rw-rw-   0        0        0     1500 2023-03-13 16:12:23.000000 seldom-3.2.1/seldom/utils/send_extend.py
--rw-rw-rw-   0        0        0     1577 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/utils/thread_lab.py
--rw-rw-rw-   0        0        0     1543 2022-12-06 15:42:11.000000 seldom-3.2.1/seldom/utils/webdriver_manager_extend.py
--rw-rw-rw-   0        0        0    31413 2023-04-03 17:12:07.000000 seldom-3.2.1/seldom/webdriver.py
--rw-rw-rw-   0        0        0    10549 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/webdriver_chaining.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.330852 seldom-3.2.1/seldom.egg-info/
--rw-rw-rw-   0        0        0     1118 2023-04-13 16:54:59.000000 seldom-3.2.1/seldom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2390 2023-04-13 16:54:59.000000 seldom-3.2.1/seldom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 16:54:59.000000 seldom-3.2.1/seldom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-04-13 16:54:59.000000 seldom-3.2.1/seldom.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-15 14:29:25.000000 seldom-3.2.1/seldom.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      252 2023-04-13 16:54:59.000000 seldom-3.2.1/seldom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-13 16:54:59.000000 seldom-3.2.1/seldom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 16:55:00.428083 seldom-3.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1853 2023-03-13 16:12:23.000000 seldom-3.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.424083 seldom-3.2.1/test/
--rw-rw-rw-   0        0        0      594 2022-12-06 15:57:51.000000 seldom-3.2.1/test/test_cache.py
--rw-rw-rw-   0        0        0     8814 2023-04-13 16:38:59.000000 seldom-3.2.1/test/test_db_operation.py
--rw-rw-rw-   0        0        0      691 2022-12-06 15:57:51.000000 seldom-3.2.1/test/test_klook.py
--rw-rw-rw-   0        0        0     1062 2022-12-06 15:57:51.000000 seldom-3.2.1/test/test_log.py
--rw-rw-rw-   0        0        0      761 2023-04-01 06:05:16.000000 seldom-3.2.1/test/test_memory_cache.py
--rw-rw-rw-   0        0        0     2204 2022-12-06 15:57:51.000000 seldom-3.2.1/test/test_testdata.py
--rw-rw-rw-   0        0        0     1658 2022-12-06 15:57:51.000000 seldom-3.2.1/test/test_thread.py
--rw-rw-rw-   0        0        0      999 2022-12-06 15:57:51.000000 seldom-3.2.1/test/test_thread2.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:56:34.050982 seldom-3.2.2/
+-rw-rw-rw-   0        0        0    11565 2022-12-06 15:57:51.000000 seldom-3.2.2/LICENSE
+-rw-rw-rw-   0        0        0       44 2022-12-06 15:57:51.000000 seldom-3.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1041 2023-05-09 16:56:34.049980 seldom-3.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9716 2023-05-05 15:56:59.000000 seldom-3.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.936361 seldom-3.2.2/demo/
+-rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.2/demo/__init__.py
+-rw-rw-rw-   0        0        0     1164 2023-01-11 15:24:10.000000 seldom-3.2.2/demo/confrun.py
+-rw-rw-rw-   0        0        0     1583 2022-12-06 15:57:51.000000 seldom-3.2.2/demo/run.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.937359 seldom-3.2.2/demo/test_dir/
+-rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.2/demo/test_dir/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.939355 seldom-3.2.2/demo/test_dir/api_case/
+-rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.2/demo/test_dir/api_case/__init__.py
+-rw-rw-rw-   0        0        0     3713 2023-01-11 15:24:10.000000 seldom-3.2.2/demo/test_dir/api_case/test_http_demo.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.944366 seldom-3.2.2/demo/test_dir/app_case/
+-rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.2/demo/test_dir/app_case/__init__.py
+-rw-rw-rw-   0        0        0      994 2022-12-06 15:57:51.000000 seldom-3.2.2/demo/test_dir/app_case/test_first_demo.py
+-rw-rw-rw-   0        0        0     1231 2023-03-19 02:35:00.000000 seldom-3.2.2/demo/test_dir/app_case/test_po_demo.py
+-rw-rw-rw-   0        0        0      875 2023-03-14 15:43:32.000000 seldom-3.2.2/demo/test_dir/app_case/test_u2_demo.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.952991 seldom-3.2.2/demo/test_dir/web_case/
+-rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.2/demo/test_dir/web_case/__init__.py
+-rw-rw-rw-   0        0        0      579 2022-12-06 15:57:51.000000 seldom-3.2.2/demo/test_dir/web_case/test_data_demo.py
+-rw-rw-rw-   0        0        0     4287 2023-01-11 15:24:10.000000 seldom-3.2.2/demo/test_dir/web_case/test_ddt_demo.py
+-rw-rw-rw-   0        0        0      589 2023-01-11 15:24:10.000000 seldom-3.2.2/demo/test_dir/web_case/test_first_demo.py
+-rw-rw-rw-   0        0        0      846 2022-12-06 15:57:51.000000 seldom-3.2.2/demo/test_dir/web_case/test_fixture_demo.py
+-rw-rw-rw-   0        0        0      953 2023-01-11 15:24:10.000000 seldom-3.2.2/demo/test_dir/web_case/test_playwright_demo.py
+-rw-rw-rw-   0        0        0     1194 2023-03-19 02:31:03.000000 seldom-3.2.2/demo/test_dir/web_case/test_po_demo.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.958995 seldom-3.2.2/proj/
+-rw-rw-rw-   0        0        0        0 2022-12-08 16:29:03.000000 seldom-3.2.2/proj/__init__.py
+-rw-rw-rw-   0        0        0      110 2022-12-12 15:41:44.000000 seldom-3.2.2/proj/confrun.py
+-rw-rw-rw-   0        0        0     1031 2022-12-12 15:42:40.000000 seldom-3.2.2/proj/loader.py
+-rw-rw-rw-   0        0        0      293 2022-12-12 15:41:28.000000 seldom-3.2.2/proj/run.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.969980 seldom-3.2.2/seldom/
+-rw-rw-rw-   0        0        0     1305 2023-05-09 16:52:08.000000 seldom-3.2.2/seldom/__init__.py
+-rw-rw-rw-   0        0        0     5373 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/appdriver.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.984991 seldom-3.2.2/seldom/appium_lab/
+-rw-rw-rw-   0        0        0     1669 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/appium_lab/__init__.py
+-rw-rw-rw-   0        0        0     3909 2023-03-13 16:12:23.000000 seldom-3.2.2/seldom/appium_lab/action.py
+-rw-rw-rw-   0        0        0     7248 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/appium_lab/find.py
+-rw-rw-rw-   0        0        0     2997 2023-03-13 16:12:23.000000 seldom-3.2.2/seldom/appium_lab/keyboard.py
+-rw-rw-rw-   0        0        0     1721 2023-03-13 16:12:23.000000 seldom-3.2.2/seldom/appium_lab/switch.py
+-rw-rw-rw-   0        0        0    11006 2023-03-13 16:12:38.000000 seldom-3.2.2/seldom/case.py
+-rw-rw-rw-   0        0        0    13177 2022-12-16 17:09:13.000000 seldom-3.2.2/seldom/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.993015 seldom-3.2.2/seldom/db_operation/
+-rw-rw-rw-   0        0        0       64 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/db_operation/__init__.py
+-rw-rw-rw-   0        0        0     1698 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/db_operation/base_db.py
+-rw-rw-rw-   0        0        0      715 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/db_operation/mongo_db.py
+-rw-rw-rw-   0        0        0     4084 2023-05-04 15:57:05.000000 seldom-3.2.2/seldom/db_operation/mssql_db.py
+-rw-rw-rw-   0        0        0     4329 2023-05-04 15:55:58.000000 seldom-3.2.2/seldom/db_operation/mysql_db.py
+-rw-rw-rw-   0        0        0     3206 2023-05-04 15:54:53.000000 seldom-3.2.2/seldom/db_operation/sqlite_db.py
+-rw-rw-rw-   0        0        0     5665 2023-03-14 15:43:32.000000 seldom-3.2.2/seldom/driver.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.996015 seldom-3.2.2/seldom/har2case/
+-rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/har2case/__init__.py
+-rw-rw-rw-   0        0        0     4014 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/har2case/core.py
+-rw-rw-rw-   0        0        0     1171 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/har2case/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.999991 seldom-3.2.2/seldom/logging/
+-rw-rw-rw-   0        0        0       48 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/logging/__init__.py
+-rw-rw-rw-   0        0        0     1101 2023-01-02 07:33:41.000000 seldom-3.2.2/seldom/logging/exceptions.py
+-rw-rw-rw-   0        0        0     1887 2023-03-16 00:03:22.000000 seldom-3.2.2/seldom/logging/log.py
+-rw-rw-rw-   0        0        0    11842 2023-03-19 02:45:19.000000 seldom-3.2.2/seldom/request.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:56:34.010991 seldom-3.2.2/seldom/running/
+-rw-rw-rw-   0        0        0     2477 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/running/DebugTestRunner.py
+-rw-rw-rw-   0        0        0      803 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/running/__init__.py
+-rw-rw-rw-   0        0        0      561 2023-03-14 15:43:32.000000 seldom-3.2.2/seldom/running/config.py
+-rw-rw-rw-   0        0        0     1467 2022-12-07 17:25:01.000000 seldom-3.2.2/seldom/running/loader.py
+-rw-rw-rw-   0        0        0     7450 2022-12-15 14:14:22.000000 seldom-3.2.2/seldom/running/loader_extend.py
+-rw-rw-rw-   0        0        0     1006 2022-12-12 16:47:54.000000 seldom-3.2.2/seldom/running/loader_hook.py
+-rw-rw-rw-   0        0        0    14707 2023-05-09 15:45:14.000000 seldom-3.2.2/seldom/running/runner.py
+-rw-rw-rw-   0        0        0     3119 2023-05-09 15:45:14.000000 seldom-3.2.2/seldom/skip.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:56:34.016991 seldom-3.2.2/seldom/testdata/
+-rw-rw-rw-   0        0        0       28 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/testdata/__init__.py
+-rw-rw-rw-   0        0        0     4164 2023-03-13 16:12:23.000000 seldom-3.2.2/seldom/testdata/conversion.py
+-rw-rw-rw-   0        0        0    10749 2023-04-03 16:11:58.000000 seldom-3.2.2/seldom/testdata/parameterization.py
+-rw-rw-rw-   0        0        0    18847 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/testdata/random_data.py
+-rw-rw-rw-   0        0        0    11986 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/testdata/random_func.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:56:34.034003 seldom-3.2.2/seldom/utils/
+-rw-rw-rw-   0        0        0      263 2023-05-09 15:45:14.000000 seldom-3.2.2/seldom/utils/__init__.py
+-rw-rw-rw-   0        0        0     5564 2023-04-01 06:05:16.000000 seldom-3.2.2/seldom/utils/cache.py
+-rw-rw-rw-   0        0        0     1067 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/utils/curlify.py
+-rw-rw-rw-   0        0        0     2395 2023-03-13 16:12:38.000000 seldom-3.2.2/seldom/utils/diff.py
+-rw-rw-rw-   0        0        0     3280 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/utils/file_extend.py
+-rw-rw-rw-   0        0        0      438 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/utils/genson.py
+-rw-rw-rw-   0        0        0      243 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/utils/jmespath.py
+-rw-rw-rw-   0        0        0    10473 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/utils/jsonpath.py
+-rw-rw-rw-   0        0        0     3964 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/utils/klook.py
+-rw-rw-rw-   0        0        0     1500 2023-03-13 16:12:23.000000 seldom-3.2.2/seldom/utils/send_extend.py
+-rw-rw-rw-   0        0        0     1577 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/utils/thread_lab.py
+-rw-rw-rw-   0        0        0     1599 2023-05-09 15:45:14.000000 seldom-3.2.2/seldom/utils/tomorrow.py
+-rw-rw-rw-   0        0        0     1543 2022-12-06 15:42:11.000000 seldom-3.2.2/seldom/utils/webdriver_manager_extend.py
+-rw-rw-rw-   0        0        0    32336 2023-05-09 15:45:14.000000 seldom-3.2.2/seldom/webdriver.py
+-rw-rw-rw-   0        0        0    10549 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/webdriver_chaining.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.978991 seldom-3.2.2/seldom.egg-info/
+-rw-rw-rw-   0        0        0     1041 2023-05-09 16:56:33.000000 seldom-3.2.2/seldom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2465 2023-05-09 16:56:33.000000 seldom-3.2.2/seldom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 16:56:33.000000 seldom-3.2.2/seldom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-09 16:56:33.000000 seldom-3.2.2/seldom.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-09 16:56:22.000000 seldom-3.2.2/seldom.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      252 2023-05-09 16:56:33.000000 seldom-3.2.2/seldom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-09 16:56:33.000000 seldom-3.2.2/seldom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 16:56:34.050982 seldom-3.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1904 2023-05-05 16:01:28.000000 seldom-3.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:56:34.048991 seldom-3.2.2/test/
+-rw-rw-rw-   0        0        0      594 2022-12-06 15:57:51.000000 seldom-3.2.2/test/test_cache.py
+-rw-rw-rw-   0        0        0     8814 2023-04-13 16:38:59.000000 seldom-3.2.2/test/test_db_operation.py
+-rw-rw-rw-   0        0        0      691 2022-12-06 15:57:51.000000 seldom-3.2.2/test/test_klook.py
+-rw-rw-rw-   0        0        0     1062 2022-12-06 15:57:51.000000 seldom-3.2.2/test/test_log.py
+-rw-rw-rw-   0        0        0      761 2023-04-01 06:05:16.000000 seldom-3.2.2/test/test_memory_cache.py
+-rw-rw-rw-   0        0        0     2204 2022-12-06 15:57:51.000000 seldom-3.2.2/test/test_testdata.py
+-rw-rw-rw-   0        0        0     1601 2023-05-09 15:45:14.000000 seldom-3.2.2/test/test_thread.py
+-rw-rw-rw-   0        0        0      999 2022-12-06 15:57:51.000000 seldom-3.2.2/test/test_thread2.py
+-rw-rw-rw-   0        0        0      776 2023-05-09 16:33:27.000000 seldom-3.2.2/test/test_thread_case.py
+-rw-rw-rw-   0        0        0      520 2023-05-09 16:38:11.000000 seldom-3.2.2/test/test_thread_path.py
```

### Comparing `seldom-3.2.1/LICENSE` & `seldom-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/PKG-INFO` & `seldom-3.2.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: seldom
-Version: 3.2.1
+Version: 3.2.2
 Summary: Seldom automation testing framework based on unittest.
 Home-page: https://github.com/seldomQA/seldom/
 Author: bugmaster
 Author-email: fnngj@126.com
 License: BSD
-Description: seldom
-        ---------------
-        
-        WebUI/HTTP automation testing framework based on unittest.
-        
-        Installation
-        ------------
-        
-            $ pip install seldom
-        
-        
-        Documentation
-        ++++++++++++++++++
-        
-        https://github.com/SeldomQA/seldom
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Testing
+License-File: LICENSE
+
+seldom
+---------------
+
+WebUI/HTTP automation testing framework based on unittest.
+
+Installation
+------------
+
+    $ pip install seldom
+
+
+Documentation
+++++++++++++++++++
+
+https://github.com/SeldomQA/seldom
```

### Comparing `seldom-3.2.1/README.md` & `seldom-3.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -290,14 +290,18 @@
 
 * [HTMLTestRunner_cn](https://github.com/GoverSky/HTMLTestRunner_cn)
 
 * [parameterized](https://github.com/wolever/parameterized)
 
 * [utx](https://github.com/jianbing/utx)
 
+### Star History
+
+![Star History Chart](https://api.star-history.com/svg?repos=SeldomQA/seldom&type=Date)
+
 ### 交流
 
 QQ群：948994709
 
 
 ## 🔥 company
```

### Comparing `seldom-3.2.1/demo/confrun.py` & `seldom-3.2.2/demo/confrun.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/demo/run.py` & `seldom-3.2.2/demo/run.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/demo/test_dir/api_case/test_http_demo.py` & `seldom-3.2.2/demo/test_dir/api_case/test_http_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/demo/test_dir/app_case/test_first_demo.py` & `seldom-3.2.2/demo/test_dir/app_case/test_first_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/demo/test_dir/app_case/test_po_demo.py` & `seldom-3.2.2/demo/test_dir/app_case/test_po_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/demo/test_dir/app_case/test_u2_demo.py` & `seldom-3.2.2/demo/test_dir/app_case/test_u2_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/demo/test_dir/web_case/test_data_demo.py` & `seldom-3.2.2/demo/test_dir/web_case/test_data_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/demo/test_dir/web_case/test_ddt_demo.py` & `seldom-3.2.2/demo/test_dir/web_case/test_ddt_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/demo/test_dir/web_case/test_first_demo.py` & `seldom-3.2.2/demo/test_dir/web_case/test_first_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/demo/test_dir/web_case/test_fixture_demo.py` & `seldom-3.2.2/demo/test_dir/web_case/test_fixture_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/demo/test_dir/web_case/test_playwright_demo.py` & `seldom-3.2.2/demo/test_dir/web_case/test_playwright_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/demo/test_dir/web_case/test_po_demo.py` & `seldom-3.2.2/demo/test_dir/web_case/test_po_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/proj/loader.py` & `seldom-3.2.2/proj/loader.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/__init__.py` & `seldom-3.2.2/seldom/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,10 +27,10 @@
 from .skip import *
 from .driver import *
 from .testdata.parameterization import *
 
 
 __author__ = "bugmaster"
 
-__version__ = "3.2.1"
+__version__ = "3.2.2"
 
 __description__ = "WebUI/HTTP automation testing framework based on unittest."
```

### Comparing `seldom-3.2.1/seldom/appdriver.py` & `seldom-3.2.2/seldom/appdriver.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/appium_lab/__init__.py` & `seldom-3.2.2/seldom/appium_lab/__init__.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/appium_lab/action.py` & `seldom-3.2.2/seldom/appium_lab/action.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/appium_lab/find.py` & `seldom-3.2.2/seldom/appium_lab/find.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/appium_lab/keyboard.py` & `seldom-3.2.2/seldom/appium_lab/keyboard.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/appium_lab/switch.py` & `seldom-3.2.2/seldom/appium_lab/switch.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/case.py` & `seldom-3.2.2/seldom/case.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/cli.py` & `seldom-3.2.2/seldom/cli.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/db_operation/base_db.py` & `seldom-3.2.2/seldom/db_operation/base_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/db_operation/mongo_db.py` & `seldom-3.2.2/seldom/db_operation/mongo_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/db_operation/mssql_db.py` & `seldom-3.2.2/seldom/db_operation/mssql_db.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,27 @@
     raise ModuleNotFoundError("Please install the library. https://github.com/pymssql/pymssql")
 from seldom.db_operation.base_db import SQLBase
 
 
 class MSSQLDB(SQLBase):
     """SQL Server DB table API"""
 
-    def __init__(self, server: str, user: str, password: str, database: str):
+    def __init__(self, server: str, user: str, password: str, database: str, charset="utf8mb4"):
         """
         Connect to the SQL Server database
         :param server:
         :param user:
         :param password:
         :param database:
         """
         self.connection = pymssql.connect(server=server,
                                           user=user,
                                           password=password,
-                                          database=database)
+                                          database=database,
+                                          charset=charset)
 
         # self.cursor = self.connection.cursor(as_dict=True)
 
     def close(self) -> None:
         """
         Close the database connection
         """
@@ -117,15 +118,16 @@
         delete table data
         """
         sql = f"""delete from {table}"""
         if where is not None:
             sql += f""" where {self.dict_to_str_and(where)};"""
         self.execute_sql(sql)
 
-    def init_table(self, table_data: dict) -> None:
+    def init_table(self, table_data: dict, clear: bool = True) -> None:
         """
         init table data
         """
         for table, data_list in table_data.items():
-            self.delete_data(table)
+            if clear:
+                self.delete_data(table)
             for data in data_list:
                 self.insert_data(table, data)
```

### Comparing `seldom-3.2.1/seldom/db_operation/mysql_db.py` & `seldom-3.2.2/seldom/db_operation/mysql_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 import pymysql.cursors
 from seldom.db_operation.base_db import SQLBase
 
 
 class MySQLDB(SQLBase):
     """MySQL DB table API"""
 
-    def __init__(self, host: str, port: int, user: str, password: str, database: str):
+    def __init__(self, host: str, port: int, user: str, password: str, database: str, charset='utf8mb4'):
         """
         Connect to the MySQL database
         :param host:
         :param port:
         :param user:
         :param password:
         :param database:
         """
         self.connection = pymysql.connect(host=host,
                                           port=int(port),
                                           user=user,
                                           password=password,
                                           database=database,
-                                          charset='utf8mb4',
+                                          charset=charset,
                                           cursorclass=pymysql.cursors.DictCursor)
 
     def close(self) -> None:
         """
         Close the database connection
         """
         self.connection.close()
@@ -121,16 +121,17 @@
         delete table data
         """
         sql = f"""delete from {table}"""
         if where is not None:
             sql += f""" where {self.dict_to_str_and(where)};"""
         self.execute_sql(sql)
 
-    def init_table(self, table_data: dict) -> None:
+    def init_table(self, table_data: dict, clear: bool = True) -> None:
         """
         init table data
         """
         for table, data_list in table_data.items():
-            self.delete_data(table)
+            if clear:
+                self.delete_data(table)
             for data in data_list:
                 self.insert_data(table, data)
         self.close()
```

### Comparing `seldom-3.2.1/seldom/db_operation/sqlite_db.py` & `seldom-3.2.2/seldom/db_operation/sqlite_db.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,15 +99,16 @@
         delete table data
         """
         sql = f"""delete from {table}"""
         if where is not None:
             sql += f""" where {self.dict_to_str_and(where)};"""
         self.execute_sql(sql)
 
-    def init_table(self, table_data: dict) -> None:
+    def init_table(self, table_data: dict, clear: bool = True) -> None:
         """
         init table data
         """
         for table, data_list in table_data.items():
-            self.delete_data(table)
+            if clear:
+                self.delete_data(table)
             for data in data_list:
                 self.insert_data(table, data)
```

### Comparing `seldom-3.2.1/seldom/driver.py` & `seldom-3.2.2/seldom/driver.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/har2case/core.py` & `seldom-3.2.2/seldom/har2case/core.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/har2case/utils.py` & `seldom-3.2.2/seldom/har2case/utils.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/logging/exceptions.py` & `seldom-3.2.2/seldom/logging/exceptions.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/logging/log.py` & `seldom-3.2.2/seldom/logging/log.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/request.py` & `seldom-3.2.2/seldom/request.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/running/DebugTestRunner.py` & `seldom-3.2.2/seldom/running/DebugTestRunner.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/running/__init__.py` & `seldom-3.2.2/seldom/running/__init__.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/running/config.py` & `seldom-3.2.2/seldom/running/config.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/running/loader.py` & `seldom-3.2.2/seldom/running/loader.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/running/loader_extend.py` & `seldom-3.2.2/seldom/running/loader_extend.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/running/loader_hook.py` & `seldom-3.2.2/seldom/running/loader_hook.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/running/runner.py` & `seldom-3.2.2/seldom/running/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
         if self.browser is not None:
             if isinstance(self.browser, str):
                 BrowserConfig.NAME = self.browser
             elif isinstance(self.browser, dict):
                 BrowserConfig.NAME = self.browser.get("browser", None)
                 BrowserConfig.command_executor = self.browser.get("command_executor", "")
                 BrowserConfig.executable_path = self.browser.get("executable_path", "")
-                BrowserConfig.options = self.browser.get("option", None)
+                BrowserConfig.options = self.browser.get("options", None)
             else:
                 raise TypeError("browser type error, str or dict.")
             Seldom.driver = Browser(BrowserConfig.NAME)
 
     @staticmethod
     def close_browser() -> None:
         """
```

### Comparing `seldom-3.2.1/seldom/skip.py` & `seldom-3.2.2/seldom/skip.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 unittest decorator
 """
 import unittest
 import functools
 
 __all__ = [
-    "skip", "skip_if", "skip_unless", "expected_failure", "depend", "if_depend", "label"
+    "skip", "skip_if", "skip_unless", "expected_failure", "depend", "if_depend", "label", "rerun"
 ]
 
 
 def skip(reason=None):
     """
     Unconditionally skip a test.
     :param reason:
@@ -103,7 +103,27 @@
 
     def inner(cls):
         # append labels to class
         cls._labels = set(labels) | getattr(cls, '_labels', set())
         return cls
 
     return inner
+
+
+def rerun(times: int = 2):
+    """
+    Repeat a function multiple times.
+    Note: The change method cannot count the number of test cases.
+
+    :param times: Number of runs, default 2
+    return
+    """
+    def wrapper(func):
+
+        @functools.wraps(func)
+        def decorator(*args, **kwargs):
+            for i in range(times):
+                func(*args, **kwargs)
+
+        return decorator
+
+    return wrapper
```

### Comparing `seldom-3.2.1/seldom/testdata/conversion.py` & `seldom-3.2.2/seldom/testdata/conversion.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/testdata/parameterization.py` & `seldom-3.2.2/seldom/testdata/parameterization.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/testdata/random_data.py` & `seldom-3.2.2/seldom/testdata/random_data.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/testdata/random_func.py` & `seldom-3.2.2/seldom/testdata/random_func.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/utils/cache.py` & `seldom-3.2.2/seldom/utils/cache.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/utils/curlify.py` & `seldom-3.2.2/seldom/utils/curlify.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/utils/diff.py` & `seldom-3.2.2/seldom/utils/diff.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/utils/file_extend.py` & `seldom-3.2.2/seldom/utils/file_extend.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/utils/jsonpath.py` & `seldom-3.2.2/seldom/utils/jsonpath.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/utils/klook.py` & `seldom-3.2.2/seldom/utils/klook.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/utils/send_extend.py` & `seldom-3.2.2/seldom/utils/send_extend.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/utils/thread_lab.py` & `seldom-3.2.2/seldom/utils/thread_lab.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/utils/webdriver_manager_extend.py` & `seldom-3.2.2/seldom/utils/webdriver_manager_extend.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom/webdriver.py` & `seldom-3.2.2/seldom/webdriver.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,23 +300,26 @@
          Gets the width and height of the current window.
 
         :Usage:
             driver.get_windows()
         """
         return Seldom.driver.get_window_size()
 
-    def type(self, text: str, clear: bool = False, enter: bool = False, index: int = 0, **kwargs) -> None:
+    def type(self, text: str, clear: bool = False, enter: bool = False, click: bool = False, index: int = 0, **kwargs) -> None:
         """
         Operation input box.
 
         Usage:
             self.type(css="#el", text="selenium")
         """
         if clear is True:
             self.clear(index, **kwargs)
+        if click is True:
+            self.click(index, **kwargs)
+            self.sleep(0.5)
         web_elem = WebElement(**kwargs)
         elem = web_elem.get_elements(index)
         web_elem.show_element(elem)
         log.info(f"✅ {web_elem.info} -> input '{text}'.")
         elem.send_keys(text)
         if enter is True:
             elem.send_keys(Keys.ENTER)
@@ -729,51 +732,74 @@
 
         :Usage:
             self.switch_to_new_window('tab')
         """
         log.info("✅ switch to new window.")
         Seldom.driver.switch_to.new_window(type_hint=type_hint)
 
-    def screenshots(self, file_path: str = None) -> None:
+    @staticmethod
+    def save_screenshot(file_path: str = None, index: int = 0, **kwargs) -> None:
         """
         Saves a screenshots of the current window to a PNG image file.
 
         Usage:
-            self.screenshots()
-            self.screenshots('/Screenshots/foo.png')
+            self.save_screenshot()
+            self.save_screenshot('/Screenshots/foo.png')
+            self.save_screenshot(id_="bLogo", index=0)
         """
+
         if file_path is None:
             img_dir = os.path.join(os.getcwd(), "reports", "images")
             if os.path.exists(img_dir) is False:
                 os.mkdir(img_dir)
             file_path = os.path.join(img_dir, get_timestamp() + ".png")
+
+        if len(kwargs) == 0:
+            log.info(f"📷️  screenshot -> ({file_path}).")
+            Seldom.driver.save_screenshot(file_path)
+        else:
+            log.info(f"📷️  element screenshot -> ({file_path}).")
+            web_elem = WebElement(**kwargs)
+            elem = web_elem.get_elements(index)
+            elem.screenshot(file_path)
+
+    def screenshots(self) -> None:
+        """
+        Saves a screenshots of the current window to HTML report.
+
+        Usage:
+            self.screenshots()
+        """
         if Seldom.debug is True:
+            img_dir = os.path.join(os.getcwd(), "reports", "images")
+            if os.path.exists(img_dir) is False:
+                os.mkdir(img_dir)
+            file_path = os.path.join(img_dir, get_timestamp() + ".png")
             log.info(f"📷️  screenshot -> ({file_path}).")
             Seldom.driver.save_screenshot(file_path)
         else:
             log.info("📷️  screenshot -> HTML report.")
             self.images.append(Seldom.driver.get_screenshot_as_base64())
 
-    def element_screenshot(self, file_path: str = None, index: int = 0, **kwargs) -> None:
+    def element_screenshot(self, index: int = 0, **kwargs) -> None:
         """
-        Saves an element screenshot of the element to a PNG image file.
+        Saves an element screenshot of the element to HTML report.
 
         Usage:
             self.element_screenshot(css="#id")
-            self.element_screenshot(css="#id", file_path='/Screenshots/foo.png')
+            self.element_screenshot(css="#id", index=0)
         """
 
         web_elem = WebElement(**kwargs)
         elem = web_elem.get_elements(index)
-        if file_path is None:
+        if Seldom.debug is True:
             img_dir = os.path.join(os.getcwd(), "reports", "images")
             if os.path.exists(img_dir) is False:
                 os.mkdir(img_dir)
             file_path = os.path.join(img_dir, get_timestamp() + ".png")
-        if Seldom.debug is True:
             log.info(f"📷️ element screenshot -> ({file_path}).")
             elem.screenshot(file_path)
         else:
             log.info("📷️ element screenshot -> HTML Report.")
             self.images.append(elem.screenshot_as_base64)
 
     @staticmethod
```

### Comparing `seldom-3.2.1/seldom/webdriver_chaining.py` & `seldom-3.2.2/seldom/webdriver_chaining.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/seldom.egg-info/PKG-INFO` & `seldom-3.2.2/seldom.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: seldom
-Version: 3.2.1
+Version: 3.2.2
 Summary: Seldom automation testing framework based on unittest.
 Home-page: https://github.com/seldomQA/seldom/
 Author: bugmaster
 Author-email: fnngj@126.com
 License: BSD
-Description: seldom
-        ---------------
-        
-        WebUI/HTTP automation testing framework based on unittest.
-        
-        Installation
-        ------------
-        
-            $ pip install seldom
-        
-        
-        Documentation
-        ++++++++++++++++++
-        
-        https://github.com/SeldomQA/seldom
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Testing
+License-File: LICENSE
+
+seldom
+---------------
+
+WebUI/HTTP automation testing framework based on unittest.
+
+Installation
+------------
+
+    $ pip install seldom
+
+
+Documentation
+++++++++++++++++++
+
+https://github.com/SeldomQA/seldom
```

### Comparing `seldom-3.2.1/seldom.egg-info/SOURCES.txt` & `seldom-3.2.2/seldom.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -75,16 +75,19 @@
 seldom/utils/file_extend.py
 seldom/utils/genson.py
 seldom/utils/jmespath.py
 seldom/utils/jsonpath.py
 seldom/utils/klook.py
 seldom/utils/send_extend.py
 seldom/utils/thread_lab.py
+seldom/utils/tomorrow.py
 seldom/utils/webdriver_manager_extend.py
 test/test_cache.py
 test/test_db_operation.py
 test/test_klook.py
 test/test_log.py
 test/test_memory_cache.py
 test/test_testdata.py
 test/test_thread.py
-test/test_thread2.py
+test/test_thread2.py
+test/test_thread_case.py
+test/test_thread_path.py
```

### Comparing `seldom-3.2.1/setup.py` & `seldom-3.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     description='Seldom automation testing framework based on unittest.',
     long_description=open(join(abspath(dirname(__file__)), "description.rst"), encoding='utf8').read(),
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'Appium-Python-Client>=2.1.0',
-        'XTestRunner>=1.6.2',
+        'XTestRunner>=1.7.0',
         'parameterized==0.8.1',
         'loguru==0.6.0',
         'openpyxl>=3.0.3',
         'pyyaml>=5.1',
         'requests>=2.22.0',
         'jsonschema>=3.2.0',
         'jmespath>=0.10.0',
@@ -44,14 +44,15 @@
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         "Topic :: Software Development :: Testing",
     ],
     entry_points='''
         [console_scripts]
         seldom=seldom.cli:main
     '''
```

### Comparing `seldom-3.2.1/test/test_cache.py` & `seldom-3.2.2/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/test/test_db_operation.py` & `seldom-3.2.2/test/test_db_operation.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/test/test_klook.py` & `seldom-3.2.2/test/test_klook.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/test/test_log.py` & `seldom-3.2.2/test/test_log.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/test/test_memory_cache.py` & `seldom-3.2.2/test/test_memory_cache.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/test/test_testdata.py` & `seldom-3.2.2/test/test_testdata.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.1/test/test_thread.py` & `seldom-3.2.2/test/test_thread.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,14 +25,22 @@
 class MyTest(seldom.TestCase):
 
     @classmethod
     def start_class(cls):
         # 存放用例和结果
         cls.assertDict = {}
 
+    def end_class(self):
+        """
+        ** 所有用例运行完成，搜集结果并断言
+        """
+        all_result = ThreadWait.get_all_result()
+        for case, value in all_result.items():
+            self.assertEqual(self.assertDict[case], value)
+
     def test_case_success(self):
         self.sleep(1)
         # 调用slow_event
         slow_event("test_case_success", 2)
         self.assertDict['test_case_success'] = 3
 
     def test_case_fail(self):
@@ -48,20 +56,11 @@
     ])
     def test_ddt(self, _, name, sec, ret):
         self.sleep(1)
         # 调用slow_event
         slow_event(f"test_case3_{name}", sec)
         self.assertDict[f"test_case3_{name}"] = ret
 
-    def test_zz_result(self):
-        """
-        ** 必须最后一个执行
-        ** 等待前面的所有用例运行完成，搜集结果并断言
-        """
-        all_result = ThreadWait.get_all_result()
-        for case, value in all_result.items():
-            self.assertEqual(self.assertDict[case], value)
-
 
 if __name__ == '__main__':
     seldom.main(debug=False)
```

### Comparing `seldom-3.2.1/test/test_thread2.py` & `seldom-3.2.2/test/test_thread2.py`

 * *Files identical despite different names*

