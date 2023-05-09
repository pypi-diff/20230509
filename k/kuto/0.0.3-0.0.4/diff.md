# Comparing `tmp/kuto-0.0.3.tar.gz` & `tmp/kuto-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuto-0.0.3.tar", last modified: Tue May  9 02:53:05 2023, max compression
+gzip compressed data, was "kuto-0.0.4.tar", last modified: Tue May  9 03:03:01 2023, max compression
```

## Comparing `kuto-0.0.3.tar` & `kuto-0.0.4.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 02:53:05.570028 kuto-0.0.3/
--rw-r--r--   0 UI         (502) staff       (20)      484 2023-05-09 02:53:05.569812 kuto-0.0.3/PKG-INFO
--rw-r--r--   0 UI         (502) staff       (20)    17940 2023-04-25 02:58:48.000000 kuto-0.0.3/README.md
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 02:53:05.545770 kuto-0.0.3/demo/
--rw-r--r--   0 UI         (502) staff       (20)        0 2022-10-17 07:22:13.000000 kuto-0.0.3/demo/__init__.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 02:53:05.546715 kuto-0.0.3/demo/page/
--rw-r--r--   0 UI         (502) staff       (20)        0 2023-03-07 03:31:21.000000 kuto-0.0.3/demo/page/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)      394 2023-04-25 02:58:48.000000 kuto-0.0.3/demo/page/adr_page.py
--rw-r--r--   0 UI         (502) staff       (20)      394 2023-04-25 02:58:48.000000 kuto-0.0.3/demo/page/web_page.py
--rw-r--r--   0 UI         (502) staff       (20)     1161 2023-04-25 02:58:48.000000 kuto-0.0.3/demo/run.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 02:53:05.549708 kuto-0.0.3/demo/tests/
--rw-r--r--   0 UI         (502) staff       (20)        0 2023-03-07 03:29:41.000000 kuto-0.0.3/demo/tests/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)      476 2023-05-09 02:31:22.000000 kuto-0.0.3/demo/tests/test_android.py
--rw-r--r--   0 UI         (502) staff       (20)      423 2023-05-09 01:53:13.000000 kuto-0.0.3/demo/tests/test_api.py
--rw-r--r--   0 UI         (502) staff       (20)      873 2023-05-09 01:48:40.000000 kuto-0.0.3/demo/tests/test_image.py
--rw-r--r--   0 UI         (502) staff       (20)      435 2023-05-09 02:33:26.000000 kuto-0.0.3/demo/tests/test_ios.py
--rw-r--r--   0 UI         (502) staff       (20)      894 2023-05-09 01:48:40.000000 kuto-0.0.3/demo/tests/test_ocr.py
--rw-r--r--   0 UI         (502) staff       (20)      843 2023-05-09 01:48:40.000000 kuto-0.0.3/demo/tests/test_parameter.py
--rw-r--r--   0 UI         (502) staff       (20)      746 2023-05-09 02:26:20.000000 kuto-0.0.3/demo/tests/test_web.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 02:53:05.551831 kuto-0.0.3/kuto/
--rw-r--r--   0 UI         (502) staff       (20)      584 2023-05-09 02:52:06.000000 kuto-0.0.3/kuto/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)    10651 2023-05-09 02:17:01.000000 kuto-0.0.3/kuto/case.py
--rw-r--r--   0 UI         (502) staff       (20)     2057 2023-04-25 02:58:48.000000 kuto-0.0.3/kuto/cli.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 02:53:05.554292 kuto-0.0.3/kuto/core/
--rw-r--r--   0 UI         (502) staff       (20)        0 2023-02-03 12:13:24.000000 kuto-0.0.3/kuto/core/__init__.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 02:53:05.555651 kuto-0.0.3/kuto/core/android/
--rw-r--r--   0 UI         (502) staff       (20)        1 2022-09-21 12:42:07.000000 kuto-0.0.3/kuto/core/android/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)      901 2023-04-25 02:58:48.000000 kuto-0.0.3/kuto/core/android/common.py
--rw-r--r--   0 UI         (502) staff       (20)     9622 2023-05-09 02:26:49.000000 kuto-0.0.3/kuto/core/android/driver.py
--rw-r--r--   0 UI         (502) staff       (20)     6964 2023-05-08 12:55:06.000000 kuto-0.0.3/kuto/core/android/element.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 02:53:05.556285 kuto-0.0.3/kuto/core/api/
--rw-r--r--   0 UI         (502) staff       (20)        0 2022-10-17 03:04:55.000000 kuto-0.0.3/kuto/core/api/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)    24514 2023-04-25 02:58:48.000000 kuto-0.0.3/kuto/core/api/request.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 02:53:05.557222 kuto-0.0.3/kuto/core/h5/
--rw-r--r--   0 UI         (502) staff       (20)        1 2022-09-21 13:04:56.000000 kuto-0.0.3/kuto/core/h5/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     7220 2023-05-09 02:28:20.000000 kuto-0.0.3/kuto/core/h5/driver.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 02:53:05.558425 kuto-0.0.3/kuto/core/image/
--rw-r--r--   0 UI         (502) staff       (20)        0 2022-12-11 09:49:05.000000 kuto-0.0.3/kuto/core/image/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     2855 2023-05-08 12:35:04.000000 kuto-0.0.3/kuto/core/image/element.py
--rw-r--r--   0 UI         (502) staff       (20)     2414 2023-05-08 12:29:45.000000 kuto-0.0.3/kuto/core/image/image_discern.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 02:53:05.559670 kuto-0.0.3/kuto/core/ios/
--rw-r--r--   0 UI         (502) staff       (20)        2 2022-09-21 12:53:47.000000 kuto-0.0.3/kuto/core/ios/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     2155 2023-04-25 02:58:48.000000 kuto-0.0.3/kuto/core/ios/common.py
--rw-r--r--   0 UI         (502) staff       (20)     7599 2023-05-09 02:28:44.000000 kuto-0.0.3/kuto/core/ios/driver.py
--rw-r--r--   0 UI         (502) staff       (20)     7953 2023-05-08 12:55:23.000000 kuto-0.0.3/kuto/core/ios/element.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 02:53:05.560646 kuto-0.0.3/kuto/core/ocr/
--rw-r--r--   0 UI         (502) staff       (20)        0 2022-12-11 09:48:37.000000 kuto-0.0.3/kuto/core/ocr/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     2296 2023-05-08 12:33:55.000000 kuto-0.0.3/kuto/core/ocr/element.py
--rw-r--r--   0 UI         (502) staff       (20)     2839 2023-05-08 12:29:45.000000 kuto-0.0.3/kuto/core/ocr/ocr_discern.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 02:53:05.561284 kuto-0.0.3/kuto/core/sonic/
--rw-r--r--   0 UI         (502) staff       (20)        0 2023-03-20 03:43:29.000000 kuto-0.0.3/kuto/core/sonic/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     4111 2023-04-25 02:58:48.000000 kuto-0.0.3/kuto/core/sonic/sib_util.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 02:53:05.562358 kuto-0.0.3/kuto/core/web/
--rw-r--r--   0 UI         (502) staff       (20)        1 2022-09-21 13:04:56.000000 kuto-0.0.3/kuto/core/web/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)    13075 2023-05-09 02:26:58.000000 kuto-0.0.3/kuto/core/web/driver.py
--rw-r--r--   0 UI         (502) staff       (20)     9474 2023-05-08 12:54:24.000000 kuto-0.0.3/kuto/core/web/element.py
--rw-r--r--   0 UI         (502) staff       (20)     2065 2023-04-23 03:42:32.000000 kuto-0.0.3/kuto/general.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 02:53:05.563209 kuto-0.0.3/kuto/mock/
--rw-r--r--   0 UI         (502) staff       (20)    10642 2023-04-01 03:18:36.000000 kuto-0.0.3/kuto/mock/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)    18623 2022-09-29 09:22:30.000000 kuto-0.0.3/kuto/mock/data.py
--rw-r--r--   0 UI         (502) staff       (20)     3261 2023-04-25 02:58:48.000000 kuto-0.0.3/kuto/page.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 02:53:05.564632 kuto-0.0.3/kuto/running/
--rw-r--r--   0 UI         (502) staff       (20)        0 2022-05-05 11:41:00.000000 kuto-0.0.3/kuto/running/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)      191 2023-05-09 02:33:50.000000 kuto-0.0.3/kuto/running/conf.yml
--rw-r--r--   0 UI         (502) staff       (20)       72 2022-12-07 07:03:15.000000 kuto-0.0.3/kuto/running/config.py
--rw-r--r--   0 UI         (502) staff       (20)     3946 2023-05-09 01:57:33.000000 kuto-0.0.3/kuto/running/runner.py
--rw-r--r--   0 UI         (502) staff       (20)     5078 2023-05-08 12:29:45.000000 kuto-0.0.3/kuto/scaffold.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 02:53:05.569441 kuto-0.0.3/kuto/utils/
--rw-r--r--   0 UI         (502) staff       (20)        0 2022-05-05 11:41:00.000000 kuto-0.0.3/kuto/utils/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     5785 2023-05-08 12:29:45.000000 kuto-0.0.3/kuto/utils/allure_data.py
--rw-r--r--   0 UI         (502) staff       (20)      348 2023-05-09 02:23:26.000000 kuto-0.0.3/kuto/utils/allure_util.py
--rw-r--r--   0 UI         (502) staff       (20)     2304 2023-03-20 05:44:26.000000 kuto-0.0.3/kuto/utils/config.py
--rw-r--r--   0 UI         (502) staff       (20)     3312 2023-05-08 12:36:35.000000 kuto-0.0.3/kuto/utils/decorate.py
--rw-r--r--   0 UI         (502) staff       (20)     3276 2023-05-08 12:29:45.000000 kuto-0.0.3/kuto/utils/dingtalk.py
--rw-r--r--   0 UI         (502) staff       (20)      780 2022-10-26 06:34:19.000000 kuto-0.0.3/kuto/utils/encrypt.py
--rw-r--r--   0 UI         (502) staff       (20)     4438 2023-04-03 00:59:14.000000 kuto-0.0.3/kuto/utils/excel.py
--rw-r--r--   0 UI         (502) staff       (20)     1795 2023-03-20 09:31:36.000000 kuto-0.0.3/kuto/utils/exceptions.py
--rw-r--r--   0 UI         (502) staff       (20)      450 2023-03-27 10:02:36.000000 kuto-0.0.3/kuto/utils/log.py
--rw-r--r--   0 UI         (502) staff       (20)     3891 2023-05-08 12:29:45.000000 kuto-0.0.3/kuto/utils/mail.py
--rw-r--r--   0 UI         (502) staff       (20)     2009 2022-10-17 03:26:18.000000 kuto-0.0.3/kuto/utils/mongo_util.py
--rw-r--r--   0 UI         (502) staff       (20)     2149 2022-10-17 03:26:26.000000 kuto-0.0.3/kuto/utils/mysql_util.py
--rw-r--r--   0 UI         (502) staff       (20)     1719 2023-04-25 02:58:48.000000 kuto-0.0.3/kuto/utils/read_file.py
--rw-r--r--   0 UI         (502) staff       (20)      632 2023-04-25 02:58:48.000000 kuto-0.0.3/kuto/utils/schema_util.py
--rw-r--r--   0 UI         (502) staff       (20)     2177 2022-05-05 11:41:00.000000 kuto-0.0.3/kuto/utils/swagger_util.py
--rw-r--r--   0 UI         (502) staff       (20)     1662 2022-05-05 11:41:00.000000 kuto-0.0.3/kuto/utils/webdriver_manager_extend.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 02:53:05.553940 kuto-0.0.3/kuto.egg-info/
--rw-r--r--   0 UI         (502) staff       (20)      484 2023-05-09 02:53:05.000000 kuto-0.0.3/kuto.egg-info/PKG-INFO
--rw-r--r--   0 UI         (502) staff       (20)     1746 2023-05-09 02:53:05.000000 kuto-0.0.3/kuto.egg-info/SOURCES.txt
--rw-r--r--   0 UI         (502) staff       (20)        1 2023-05-09 02:53:05.000000 kuto-0.0.3/kuto.egg-info/dependency_links.txt
--rw-r--r--   0 UI         (502) staff       (20)       39 2023-05-09 02:53:05.000000 kuto-0.0.3/kuto.egg-info/entry_points.txt
--rw-r--r--   0 UI         (502) staff       (20)      835 2023-05-09 02:53:05.000000 kuto-0.0.3/kuto.egg-info/requires.txt
--rw-r--r--   0 UI         (502) staff       (20)       10 2023-05-09 02:53:05.000000 kuto-0.0.3/kuto.egg-info/top_level.txt
--rw-r--r--   0 UI         (502) staff       (20)       38 2023-05-09 02:53:05.570098 kuto-0.0.3/setup.cfg
--rw-r--r--   0 UI         (502) staff       (20)     2216 2023-05-09 02:52:49.000000 kuto-0.0.3/setup.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 03:03:01.910993 kuto-0.0.4/
+-rw-r--r--   0 UI         (502) staff       (20)      397 2023-05-09 03:03:01.910774 kuto-0.0.4/PKG-INFO
+-rw-r--r--   0 UI         (502) staff       (20)    17940 2023-04-25 02:58:48.000000 kuto-0.0.4/README.md
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 03:03:01.887352 kuto-0.0.4/demo/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2022-10-17 07:22:13.000000 kuto-0.0.4/demo/__init__.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 03:03:01.888457 kuto-0.0.4/demo/page/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2023-03-07 03:31:21.000000 kuto-0.0.4/demo/page/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)      394 2023-04-25 02:58:48.000000 kuto-0.0.4/demo/page/adr_page.py
+-rw-r--r--   0 UI         (502) staff       (20)      394 2023-04-25 02:58:48.000000 kuto-0.0.4/demo/page/web_page.py
+-rw-r--r--   0 UI         (502) staff       (20)     1161 2023-04-25 02:58:48.000000 kuto-0.0.4/demo/run.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 03:03:01.891453 kuto-0.0.4/demo/tests/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2023-03-07 03:29:41.000000 kuto-0.0.4/demo/tests/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)      476 2023-05-09 02:31:22.000000 kuto-0.0.4/demo/tests/test_android.py
+-rw-r--r--   0 UI         (502) staff       (20)      423 2023-05-09 01:53:13.000000 kuto-0.0.4/demo/tests/test_api.py
+-rw-r--r--   0 UI         (502) staff       (20)      873 2023-05-09 01:48:40.000000 kuto-0.0.4/demo/tests/test_image.py
+-rw-r--r--   0 UI         (502) staff       (20)      435 2023-05-09 02:33:26.000000 kuto-0.0.4/demo/tests/test_ios.py
+-rw-r--r--   0 UI         (502) staff       (20)      894 2023-05-09 01:48:40.000000 kuto-0.0.4/demo/tests/test_ocr.py
+-rw-r--r--   0 UI         (502) staff       (20)      843 2023-05-09 01:48:40.000000 kuto-0.0.4/demo/tests/test_parameter.py
+-rw-r--r--   0 UI         (502) staff       (20)      746 2023-05-09 02:26:20.000000 kuto-0.0.4/demo/tests/test_web.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 03:03:01.893682 kuto-0.0.4/kuto/
+-rw-r--r--   0 UI         (502) staff       (20)      584 2023-05-09 03:02:40.000000 kuto-0.0.4/kuto/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)    10651 2023-05-09 02:17:01.000000 kuto-0.0.4/kuto/case.py
+-rw-r--r--   0 UI         (502) staff       (20)     2057 2023-04-25 02:58:48.000000 kuto-0.0.4/kuto/cli.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 03:03:01.895821 kuto-0.0.4/kuto/core/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2023-02-03 12:13:24.000000 kuto-0.0.4/kuto/core/__init__.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 03:03:01.897344 kuto-0.0.4/kuto/core/android/
+-rw-r--r--   0 UI         (502) staff       (20)        1 2022-09-21 12:42:07.000000 kuto-0.0.4/kuto/core/android/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)      901 2023-04-25 02:58:48.000000 kuto-0.0.4/kuto/core/android/common.py
+-rw-r--r--   0 UI         (502) staff       (20)     9622 2023-05-09 02:26:49.000000 kuto-0.0.4/kuto/core/android/driver.py
+-rw-r--r--   0 UI         (502) staff       (20)     6964 2023-05-08 12:55:06.000000 kuto-0.0.4/kuto/core/android/element.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 03:03:01.897946 kuto-0.0.4/kuto/core/api/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2022-10-17 03:04:55.000000 kuto-0.0.4/kuto/core/api/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)    24514 2023-04-25 02:58:48.000000 kuto-0.0.4/kuto/core/api/request.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 03:03:01.898530 kuto-0.0.4/kuto/core/h5/
+-rw-r--r--   0 UI         (502) staff       (20)        1 2022-09-21 13:04:56.000000 kuto-0.0.4/kuto/core/h5/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     7220 2023-05-09 02:28:20.000000 kuto-0.0.4/kuto/core/h5/driver.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 03:03:01.899459 kuto-0.0.4/kuto/core/image/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2022-12-11 09:49:05.000000 kuto-0.0.4/kuto/core/image/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     2855 2023-05-08 12:35:04.000000 kuto-0.0.4/kuto/core/image/element.py
+-rw-r--r--   0 UI         (502) staff       (20)     2414 2023-05-08 12:29:45.000000 kuto-0.0.4/kuto/core/image/image_discern.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 03:03:01.900662 kuto-0.0.4/kuto/core/ios/
+-rw-r--r--   0 UI         (502) staff       (20)        2 2022-09-21 12:53:47.000000 kuto-0.0.4/kuto/core/ios/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     2155 2023-04-25 02:58:48.000000 kuto-0.0.4/kuto/core/ios/common.py
+-rw-r--r--   0 UI         (502) staff       (20)     7599 2023-05-09 02:28:44.000000 kuto-0.0.4/kuto/core/ios/driver.py
+-rw-r--r--   0 UI         (502) staff       (20)     7953 2023-05-08 12:55:23.000000 kuto-0.0.4/kuto/core/ios/element.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 03:03:01.901657 kuto-0.0.4/kuto/core/ocr/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2022-12-11 09:48:37.000000 kuto-0.0.4/kuto/core/ocr/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     2296 2023-05-08 12:33:55.000000 kuto-0.0.4/kuto/core/ocr/element.py
+-rw-r--r--   0 UI         (502) staff       (20)     2839 2023-05-08 12:29:45.000000 kuto-0.0.4/kuto/core/ocr/ocr_discern.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 03:03:01.902150 kuto-0.0.4/kuto/core/sonic/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2023-03-20 03:43:29.000000 kuto-0.0.4/kuto/core/sonic/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     4111 2023-04-25 02:58:48.000000 kuto-0.0.4/kuto/core/sonic/sib_util.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 03:03:01.902953 kuto-0.0.4/kuto/core/web/
+-rw-r--r--   0 UI         (502) staff       (20)        1 2022-09-21 13:04:56.000000 kuto-0.0.4/kuto/core/web/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)    13075 2023-05-09 02:26:58.000000 kuto-0.0.4/kuto/core/web/driver.py
+-rw-r--r--   0 UI         (502) staff       (20)     9474 2023-05-08 12:54:24.000000 kuto-0.0.4/kuto/core/web/element.py
+-rw-r--r--   0 UI         (502) staff       (20)     2065 2023-04-23 03:42:32.000000 kuto-0.0.4/kuto/general.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 03:03:01.903545 kuto-0.0.4/kuto/mock/
+-rw-r--r--   0 UI         (502) staff       (20)    10642 2023-04-01 03:18:36.000000 kuto-0.0.4/kuto/mock/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)    18623 2022-09-29 09:22:30.000000 kuto-0.0.4/kuto/mock/data.py
+-rw-r--r--   0 UI         (502) staff       (20)     3261 2023-04-25 02:58:48.000000 kuto-0.0.4/kuto/page.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 03:03:01.905019 kuto-0.0.4/kuto/running/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2022-05-05 11:41:00.000000 kuto-0.0.4/kuto/running/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)      191 2023-05-09 02:33:50.000000 kuto-0.0.4/kuto/running/conf.yml
+-rw-r--r--   0 UI         (502) staff       (20)       72 2022-12-07 07:03:15.000000 kuto-0.0.4/kuto/running/config.py
+-rw-r--r--   0 UI         (502) staff       (20)     3946 2023-05-09 01:57:33.000000 kuto-0.0.4/kuto/running/runner.py
+-rw-r--r--   0 UI         (502) staff       (20)     5078 2023-05-08 12:29:45.000000 kuto-0.0.4/kuto/scaffold.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 03:03:01.910452 kuto-0.0.4/kuto/utils/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2022-05-05 11:41:00.000000 kuto-0.0.4/kuto/utils/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     5785 2023-05-08 12:29:45.000000 kuto-0.0.4/kuto/utils/allure_data.py
+-rw-r--r--   0 UI         (502) staff       (20)      348 2023-05-09 02:23:26.000000 kuto-0.0.4/kuto/utils/allure_util.py
+-rw-r--r--   0 UI         (502) staff       (20)     2304 2023-03-20 05:44:26.000000 kuto-0.0.4/kuto/utils/config.py
+-rw-r--r--   0 UI         (502) staff       (20)     3312 2023-05-08 12:36:35.000000 kuto-0.0.4/kuto/utils/decorate.py
+-rw-r--r--   0 UI         (502) staff       (20)     3276 2023-05-08 12:29:45.000000 kuto-0.0.4/kuto/utils/dingtalk.py
+-rw-r--r--   0 UI         (502) staff       (20)      780 2022-10-26 06:34:19.000000 kuto-0.0.4/kuto/utils/encrypt.py
+-rw-r--r--   0 UI         (502) staff       (20)     4438 2023-04-03 00:59:14.000000 kuto-0.0.4/kuto/utils/excel.py
+-rw-r--r--   0 UI         (502) staff       (20)     1795 2023-03-20 09:31:36.000000 kuto-0.0.4/kuto/utils/exceptions.py
+-rw-r--r--   0 UI         (502) staff       (20)      450 2023-03-27 10:02:36.000000 kuto-0.0.4/kuto/utils/log.py
+-rw-r--r--   0 UI         (502) staff       (20)     3891 2023-05-08 12:29:45.000000 kuto-0.0.4/kuto/utils/mail.py
+-rw-r--r--   0 UI         (502) staff       (20)     2009 2022-10-17 03:26:18.000000 kuto-0.0.4/kuto/utils/mongo_util.py
+-rw-r--r--   0 UI         (502) staff       (20)     2149 2022-10-17 03:26:26.000000 kuto-0.0.4/kuto/utils/mysql_util.py
+-rw-r--r--   0 UI         (502) staff       (20)     1719 2023-04-25 02:58:48.000000 kuto-0.0.4/kuto/utils/read_file.py
+-rw-r--r--   0 UI         (502) staff       (20)      632 2023-04-25 02:58:48.000000 kuto-0.0.4/kuto/utils/schema_util.py
+-rw-r--r--   0 UI         (502) staff       (20)     2177 2022-05-05 11:41:00.000000 kuto-0.0.4/kuto/utils/swagger_util.py
+-rw-r--r--   0 UI         (502) staff       (20)     1662 2022-05-05 11:41:00.000000 kuto-0.0.4/kuto/utils/webdriver_manager_extend.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 03:03:01.895437 kuto-0.0.4/kuto.egg-info/
+-rw-r--r--   0 UI         (502) staff       (20)      397 2023-05-09 03:03:01.000000 kuto-0.0.4/kuto.egg-info/PKG-INFO
+-rw-r--r--   0 UI         (502) staff       (20)     1746 2023-05-09 03:03:01.000000 kuto-0.0.4/kuto.egg-info/SOURCES.txt
+-rw-r--r--   0 UI         (502) staff       (20)        1 2023-05-09 03:03:01.000000 kuto-0.0.4/kuto.egg-info/dependency_links.txt
+-rw-r--r--   0 UI         (502) staff       (20)       39 2023-05-09 03:03:01.000000 kuto-0.0.4/kuto.egg-info/entry_points.txt
+-rw-r--r--   0 UI         (502) staff       (20)      563 2023-05-09 03:03:01.000000 kuto-0.0.4/kuto.egg-info/requires.txt
+-rw-r--r--   0 UI         (502) staff       (20)       10 2023-05-09 03:03:01.000000 kuto-0.0.4/kuto.egg-info/top_level.txt
+-rw-r--r--   0 UI         (502) staff       (20)       38 2023-05-09 03:03:01.911084 kuto-0.0.4/setup.cfg
+-rw-r--r--   0 UI         (502) staff       (20)     1754 2023-05-09 03:02:33.000000 kuto-0.0.4/setup.py
```

### Comparing `kuto-0.0.3/README.md` & `kuto-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/demo/run.py` & `kuto-0.0.4/demo/run.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/demo/tests/test_image.py` & `kuto-0.0.4/demo/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/demo/tests/test_ocr.py` & `kuto-0.0.4/demo/tests/test_ocr.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/demo/tests/test_parameter.py` & `kuto-0.0.4/demo/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/demo/tests/test_web.py` & `kuto-0.0.4/demo/tests/test_web.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/__init__.py` & `kuto-0.0.4/kuto/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 )
 from kuto.running.runner import main
 from kuto.utils.config import config
 from kuto.utils.decorate import *
 from kuto.utils.log import logger
 
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __description__ = "移动、web、接口自动化测试框架"
```

### Comparing `kuto-0.0.3/kuto/case.py` & `kuto-0.0.4/kuto/case.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/cli.py` & `kuto-0.0.4/kuto/cli.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/core/android/common.py` & `kuto-0.0.4/kuto/core/android/common.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/core/android/driver.py` & `kuto-0.0.4/kuto/core/android/driver.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/core/android/element.py` & `kuto-0.0.4/kuto/core/android/element.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/core/api/request.py` & `kuto-0.0.4/kuto/core/api/request.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/core/h5/driver.py` & `kuto-0.0.4/kuto/core/h5/driver.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/core/image/element.py` & `kuto-0.0.4/kuto/core/image/element.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/core/image/image_discern.py` & `kuto-0.0.4/kuto/core/image/image_discern.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/core/ios/common.py` & `kuto-0.0.4/kuto/core/ios/common.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/core/ios/driver.py` & `kuto-0.0.4/kuto/core/ios/driver.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/core/ios/element.py` & `kuto-0.0.4/kuto/core/ios/element.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/core/ocr/element.py` & `kuto-0.0.4/kuto/core/ocr/element.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/core/ocr/ocr_discern.py` & `kuto-0.0.4/kuto/core/ocr/ocr_discern.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/core/sonic/sib_util.py` & `kuto-0.0.4/kuto/core/sonic/sib_util.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/core/web/driver.py` & `kuto-0.0.4/kuto/core/web/driver.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/core/web/element.py` & `kuto-0.0.4/kuto/core/web/element.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/general.py` & `kuto-0.0.4/kuto/general.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/mock/__init__.py` & `kuto-0.0.4/kuto/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/mock/data.py` & `kuto-0.0.4/kuto/mock/data.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/page.py` & `kuto-0.0.4/kuto/page.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/running/runner.py` & `kuto-0.0.4/kuto/running/runner.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/scaffold.py` & `kuto-0.0.4/kuto/scaffold.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/utils/allure_data.py` & `kuto-0.0.4/kuto/utils/allure_data.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/utils/config.py` & `kuto-0.0.4/kuto/utils/config.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/utils/decorate.py` & `kuto-0.0.4/kuto/utils/decorate.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/utils/dingtalk.py` & `kuto-0.0.4/kuto/utils/dingtalk.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/utils/encrypt.py` & `kuto-0.0.4/kuto/utils/encrypt.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/utils/excel.py` & `kuto-0.0.4/kuto/utils/excel.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/utils/exceptions.py` & `kuto-0.0.4/kuto/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/utils/mail.py` & `kuto-0.0.4/kuto/utils/mail.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/utils/mongo_util.py` & `kuto-0.0.4/kuto/utils/mongo_util.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/utils/mysql_util.py` & `kuto-0.0.4/kuto/utils/mysql_util.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/utils/read_file.py` & `kuto-0.0.4/kuto/utils/read_file.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/utils/schema_util.py` & `kuto-0.0.4/kuto/utils/schema_util.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/utils/swagger_util.py` & `kuto-0.0.4/kuto/utils/swagger_util.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto/utils/webdriver_manager_extend.py` & `kuto-0.0.4/kuto/utils/webdriver_manager_extend.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto.egg-info/SOURCES.txt` & `kuto-0.0.4/kuto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kuto-0.0.3/kuto.egg-info/requires.txt` & `kuto-0.0.4/kuto.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -9,45 +9,25 @@
 pytest==6.2.5
 pytest-rerunfailures==10.2
 pytest-ordering==0.6
 pytest-xdist==2.5.0
 pytest-dependency==0.5.1
 allure-pytest==2.9.45
 PyYAML==6.0
-
-[db]
-PyMySQL==0.10.1
-pymongo==4.0.1
-
-[encrypt]
-pycryptodome==3.14.1
-
-[excel]
 pandas==1.3.4
 openpyxl==3.0.9
 XlsxWriter==3.0.2
-
-[ext]
-yagmail==0.15.293
-genson==1.2.2
 pycryptodome==3.14.1
+yagmail==0.15.293
+
+[db]
 PyMySQL==0.10.1
 pymongo==4.0.1
-pandas==1.3.4
-openpyxl==3.0.9
-XlsxWriter==3.0.2
-easyocr==1.6.2
-opencv-python==4.6.0.66
-opencv-contrib-python==4.6.0.66
-opencv-python-headless==3.4.18.65
 
 [genson]
 genson==1.2.2
 
 [image]
 easyocr==1.6.2
 opencv-python==4.6.0.66
 opencv-contrib-python==4.6.0.66
 opencv-python-headless==3.4.18.65
-
-[mail]
-yagmail==0.15.293
```

### Comparing `kuto-0.0.3/setup.py` & `kuto-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,38 +37,26 @@
         'webdriver-manager==3.5.2',
         'pytest==6.2.5',
         'pytest-rerunfailures==10.2',
         'pytest-ordering==0.6',
         'pytest-xdist==2.5.0',
         'pytest-dependency==0.5.1',
         'allure-pytest==2.9.45',
-        'PyYAML==6.0'
+        'PyYAML==6.0',
+        'pandas==1.3.4',
+        'openpyxl==3.0.9',
+        'XlsxWriter==3.0.2',
+        'pycryptodome==3.14.1',
+        'yagmail==0.15.293'
     ],
     extras_require={
-        "mail": ['yagmail==0.15.293'],
         "genson": ['genson==1.2.2'],
-        "encrypt": ['pycryptodome==3.14.1'],
         "db": ['PyMySQL==0.10.1', 'pymongo==4.0.1'],
-        "excel": ['pandas==1.3.4', 'openpyxl==3.0.9', 'XlsxWriter==3.0.2'],
         "image": ['easyocr==1.6.2', 'opencv-python==4.6.0.66', 'opencv-contrib-python==4.6.0.66',
-                  'opencv-python-headless==3.4.18.65'],
-        "ext": [
-            'yagmail==0.15.293',
-            'genson==1.2.2',
-            'pycryptodome==3.14.1',
-            'PyMySQL==0.10.1',
-            'pymongo==4.0.1',
-            'pandas==1.3.4',
-            'openpyxl==3.0.9',
-            'XlsxWriter==3.0.2',
-            'easyocr==1.6.2',
-            'opencv-python==4.6.0.66',
-            'opencv-contrib-python==4.6.0.66',
-            'opencv-python-headless==3.4.18.65'
-        ]
+                  'opencv-python-headless==3.4.18.65']
     },
     entry_points={
         'console_scripts': [
             'kuto = kuto.cli:main'
         ]
     },
 )
```

