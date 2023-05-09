# Comparing `tmp/linktest-2.0.3.tar.gz` & `tmp/linktest-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/linktest-2.0.3.tar", last modified: Wed Apr 26 06:31:52 2023, max compression
+gzip compressed data, was "linktest-2.0.4.tar", last modified: Tue May  9 05:27:52 2023, max compression
```

## Comparing `linktest-2.0.3.tar` & `linktest-2.0.4.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-04-26 06:31:52.000000 linktest-2.0.3/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      192 2023-04-26 06:31:52.000000 linktest-2.0.3/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-04-26 06:31:52.000000 linktest-2.0.3/lintest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1071 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10929 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      461 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3597 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/xml_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2629 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/auto_generate_test_suite.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10159 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31798 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2511 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10758 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1786 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7822 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      420 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3052 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    30653 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7062 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      176 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/lintest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3135 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   111768 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2130 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/auto_organize_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1481 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    17741 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16348 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-04-25 06:29:43.000000 linktest-2.0.3/lintest/testcase_order.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-04-26 06:31:51.000000 linktest-2.0.3/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2023-04-25 12:18:59.000000 linktest-2.0.3/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9712 2023-04-26 06:07:11.000000 linktest-2.0.3/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2023-04-26 05:36:37.000000 linktest-2.0.3/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2023-04-26 06:29:23.000000 linktest-2.0.3/linktest/xml_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10159 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31803 2023-04-26 06:28:34.000000 linktest-2.0.3/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2023-04-26 06:27:01.000000 linktest-2.0.3/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2023-04-25 07:00:45.000000 linktest-2.0.3/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2023-04-26 06:20:46.000000 linktest-2.0.3/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-04-26 05:35:06.000000 linktest-2.0.3/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7822 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      422 2023-04-26 06:29:54.000000 linktest-2.0.3/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2023-04-25 12:18:59.000000 linktest-2.0.3/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2023-04-26 05:52:13.000000 linktest-2.0.3/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7110 2023-04-26 06:23:55.000000 linktest-2.0.3/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2023-04-25 12:18:59.000000 linktest-2.0.3/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   100509 2023-04-26 03:25:21.000000 linktest-2.0.3/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2023-04-25 13:06:43.000000 linktest-2.0.3/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      916 2023-04-26 06:27:01.000000 linktest-2.0.3/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16834 2023-04-26 05:58:55.000000 linktest-2.0.3/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16356 2023-04-25 07:00:45.000000 linktest-2.0.3/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-04-25 06:57:24.000000 linktest-2.0.3/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      454 2023-04-26 06:31:40.000000 linktest-2.0.3/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2023-04-26 06:31:52.000000 linktest-2.0.3/setup.cfg
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-04-26 06:31:51.000000 linktest-2.0.3/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      192 2023-04-26 06:31:51.000000 linktest-2.0.3/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2190 2023-04-26 06:31:51.000000 linktest-2.0.3/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      116 2023-04-26 06:31:51.000000 linktest-2.0.3/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2023-04-26 06:31:51.000000 linktest-2.0.3/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2023-04-26 06:31:51.000000 linktest-2.0.3/linktest.egg-info/dependency_links.txt
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 05:27:52.514191 linktest-2.0.4/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      100 2023-05-09 05:27:52.512964 linktest-2.0.4/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 05:27:52.417780 linktest-2.0.4/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-05-09 05:21:50.000000 linktest-2.0.4/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2023-04-26 05:36:37.000000 linktest-2.0.4/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2023-04-25 07:00:45.000000 linktest-2.0.4/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2023-04-26 05:52:13.000000 linktest-2.0.4/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16834 2023-04-26 05:58:55.000000 linktest-2.0.4/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9712 2023-04-26 06:07:11.000000 linktest-2.0.4/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2023-04-26 06:20:46.000000 linktest-2.0.4/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7110 2023-04-26 06:23:55.000000 linktest-2.0.4/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2023-04-26 06:27:01.000000 linktest-2.0.4/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16356 2023-04-25 07:00:45.000000 linktest-2.0.4/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      916 2023-04-26 06:27:01.000000 linktest-2.0.4/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2023-04-25 12:18:59.000000 linktest-2.0.4/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31803 2023-04-26 06:28:34.000000 linktest-2.0.4/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2023-04-25 13:06:43.000000 linktest-2.0.4/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9672 2023-05-09 05:27:04.000000 linktest-2.0.4/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   100564 2023-05-09 05:25:01.000000 linktest-2.0.4/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2023-04-25 12:18:59.000000 linktest-2.0.4/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7822 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      527 2023-05-09 05:21:39.000000 linktest-2.0.4/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2023-04-25 12:18:59.000000 linktest-2.0.4/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2023-04-26 06:29:23.000000 linktest-2.0.4/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 05:27:52.425678 linktest-2.0.4/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      100 2023-05-09 05:27:52.000000 linktest-2.0.4/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2190 2023-05-09 05:27:52.000000 linktest-2.0.4/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2023-05-09 05:27:52.000000 linktest-2.0.4/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      116 2023-05-09 05:27:52.000000 linktest-2.0.4/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2023-05-09 05:27:52.000000 linktest-2.0.4/linktest.egg-info/top_level.txt
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 05:27:52.511074 linktest-2.0.4/lintest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      461 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10758 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2629 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/auto_generate_test_suite.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    30653 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    17741 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2130 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/auto_organize_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10929 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1786 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7062 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2511 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16348 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1481 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3135 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31798 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      176 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/lintest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10159 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   111768 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1071 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7822 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      420 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3052 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3597 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/xml_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2023-05-09 05:27:52.514344 linktest-2.0.4/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      454 2023-05-09 05:27:37.000000 linktest-2.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `linktest-2.0.3/lintest/run.py` & `linktest-2.0.4/lintest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/base_testcase.py` & `linktest-2.0.4/lintest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/timeout_thread.py` & `linktest-2.0.4/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/get_platform_info.py` & `linktest-2.0.4/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/xml_report.py` & `linktest-2.0.4/lintest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/auto_generate_test_suite.py` & `linktest-2.0.4/lintest/auto_generate_test_suite.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/logged_requests.py` & `linktest-2.0.4/lintest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/html_report.py` & `linktest-2.0.4/lintest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/ui_testcase.py` & `linktest-2.0.4/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/date_utilities.py` & `linktest-2.0.4/lintest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/scp_report_to_specified_path.py` & `linktest-2.0.4/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/appium_utils.py` & `linktest-2.0.4/lintest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/clean_data.py` & `linktest-2.0.4/lintest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/conver_xml_into_db.py` & `linktest-2.0.4/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/run_testcase_thread.py` & `linktest-2.0.4/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/selenium_helper.py` & `linktest-2.0.4/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/memory_usage.py` & `linktest-2.0.4/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/update_config.py` & `linktest-2.0.4/lintest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/auto_generate_testcase_list.py` & `linktest-2.0.4/lintest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/database_helper.py` & `linktest-2.0.4/lintest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/get_ios_devices_list.py` & `linktest-2.0.4/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/get_project_info.py` & `linktest-2.0.4/lintest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/get_adb_devices.py` & `linktest-2.0.4/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/main.py` & `linktest-2.0.4/lintest/main.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/auto_organize_testcase.py` & `linktest-2.0.4/lintest/auto_organize_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/framework_log.py` & `linktest-2.0.4/lintest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/auto_generate_testcase_list_from_csv.py` & `linktest-2.0.4/lintest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/lintest/doctor.py` & `linktest-2.0.4/lintest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/run.py` & `linktest-2.0.4/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/base_testcase.py` & `linktest-2.0.4/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/timeout_thread.py` & `linktest-2.0.4/lintest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/get_platform_info.py` & `linktest-2.0.4/lintest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/xml_report.py` & `linktest-2.0.4/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/logged_requests.py` & `linktest-2.0.4/linktest/logged_requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,69 +63,61 @@
             print("================================ cURL End ============================" + os.linesep)
         return res
 
     return wrapper
 
 
 class LoggedRequests:
-    def __init__(self, executing_case):
-        self.this = executing_case
+    def __init__(self, logger):
+        self.logger = logger
     """
     封装 requests module 的常用方法，自动log 每次 request 的参数 & response 内容
     @author: Wang Lin
     """
 
     @log_curl
     def get(self, url, params=None, **kwargs):
-        self = self.this
-
         # 增加此判断逻辑，解释参见 post 方法
         if hasattr(settings, "auto_log_request") and settings.auto_log_request is False:
-            # 直接调用 开源 requests
             return requests.get(url, params, **kwargs)
 
         self.logger.info(
             os.linesep + os.linesep + ">>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>> GET Start:")
         self.logger.info(os.linesep + "---------------- URL: " + url)
 
         if params is not None:
             self.logger.info(os.linesep + "-------------- params:")
             self.logger.info(os.linesep + self.pformat(params))
 
         if len(kwargs.keys()) > 0:
             self.logger.info(os.linesep + "-------------- kwargs:")
             self.logger.info(os.linesep + json_func.dumps(kwargs, indent=2))
 
-        # call requests.get()
         response = requests.get(url, params, **kwargs)
 
         self.logger.info(
             os.linesep + os.linesep + "<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<< GET Response:")
         self.logger.info(response)
 
-        # todo
         if response.status_code == 200:
             try:
                 # self.logger.info(self.pformat(response.json()))
                 self.logger.info(os.linesep + json_func.dumps(response.json(), ensure_ascii=False, indent=2))
             except BaseException:
                 return response
 
         self.logger.info(
             os.linesep + "========================= GET DONE =========================" + os.linesep + os.linesep)
 
         return response
 
     @log_curl
     def post(self, url, data=None, json=None, **kwargs):
-        self = self.this
-
         #  为了 不重复记录 log,则 增加如下判断， 如果 settings.auto_log_request = False, 则不需要框架自动记录log!
         if hasattr(settings, "auto_log_request") and settings.auto_log_request is False:
-            # 直接调用 开源 requests
             return requests.post(url, data, json, **kwargs)
 
         self.logger.info(
             os.linesep + os.linesep + ">>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>> POST Start:")
         self.logger.info(os.linesep + "------------ URL: " + url)
 
         if data is not None:
@@ -140,32 +132,28 @@
             try:
                 # 此处省去各种判断逻辑, 如果 json.loads()报错，则直接 记录原始data
                 # self.logger.info(os.linesep + self.pformat(json_func.loads(data)))
                 self.logger.info(os.linesep + json_func.dumps(json_func.loads(data), ensure_ascii=False, indent=2))
             except BaseException:
                 self.logger.info(os.linesep + self.pformat(data))
 
-            # self.logger.info(os.linesep + "------------ data end -------" + os.linesep)
-
         if json is not None:
             self.logger.info(os.linesep + os.linesep + "------------ json:")
             self.logger.info(os.linesep + json_func.dumps(json, ensure_ascii=False, indent=2))
 
         if len(kwargs.keys()) > 0:
             self.logger.info(os.linesep + os.linesep + "------------ kwargs:")
             self.logger.info(os.linesep + json_func.dumps(kwargs, ensure_ascii=False, indent=2))
 
-        # call requests.post()
         response = requests.post(url, data, json, **kwargs)
 
         self.logger.info(
             os.linesep + os.linesep + "<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<< POST Response:")
         self.logger.info(response)
 
-        # todo
         if response.status_code == 200:
             try:
                 # dumps()方法中的 indent参数 如果 不为空 则会自动format输出结果
                 self.logger.info(os.linesep + json_func.dumps(response.json(), ensure_ascii=False, indent=2))
             except BaseException:
                 self.logger.info(response.__dict__)
                 return response
@@ -173,16 +161,14 @@
         self.logger.info(
             os.linesep + "========================= POST DONE =========================" + os.linesep + os.linesep)
 
         return response
 
     @log_curl
     def put(self, url, data=None, **kwargs):
-        self = self.this
-
         # 增加此判断逻辑，解释参见 post 方法
         if hasattr(settings, "auto_log_request") and settings.auto_log_request is False:
             # 直接调用 开源 requests
             return requests.put(url, data, **kwargs)
 
         self.logger.info(
             os.linesep + ">>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>> PUT Start:")
@@ -195,58 +181,52 @@
             except BaseException:
                 self.logger.info(os.linesep + self.pformat(data))
 
         if len(kwargs.keys()) > 0:
             self.logger.info(os.linesep + "------------ kwargs:")
             self.logger.info(os.linesep + json_func.dumps(kwargs, ensure_ascii=False, indent=2))
 
-        # call requests.put()
         response = requests.put(url, data, **kwargs)
 
         self.logger.info(
             os.linesep + os.linesep + "<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<< PUT Response:")
         self.logger.info(response)
 
-        # todo
         if response.status_code == 200:
             try:
                 self.logger.info(os.linesep + json_func.dumps(response.json(), ensure_ascii=False, indent=2))
             except BaseException:
                 return response
 
         self.logger.info(
             os.linesep + "========================= PUT DONE =========================" + os.linesep + os.linesep)
 
         return response
 
     @log_curl
     def delete(self, url, **kwargs):
-        self = self.this
-        
         # 增加此判断逻辑，解释参见 post 方法
         if hasattr(settings, "auto_log_request") and settings.auto_log_request is False:
             # 直接调用 开源 requests
             return requests.delete(url, **kwargs)
 
         self.logger.info(
             os.linesep + ">>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>> DELETE Start:")
         self.logger.info(os.linesep + "--------------- URL: " + url)
 
         if len(kwargs.keys()) > 0:
             self.logger.info(os.linesep + "------------ kwargs:")
             self.logger.info(os.linesep + json_func.dumps(kwargs, ensure_ascii=False, indent=2))
 
-        # call requests.delete()
         response = requests.delete(url, **kwargs)
 
         self.logger.info(
             os.linesep + os.linesep + "<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<< DELETE Response:")
         self.logger.info(response)
 
-        # todo
         if response.status_code == 200:
             try:
                 self.logger.info(os.linesep + json_func.dumps(response.json(), ensure_ascii=False, indent=2))
             except BaseException:
                 return response
 
         self.logger.info(
```

### Comparing `linktest-2.0.3/linktest/html_report.py` & `linktest-2.0.4/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/ui_testcase.py` & `linktest-2.0.4/lintest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/date_utilities.py` & `linktest-2.0.4/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/scp_report_to_specified_path.py` & `linktest-2.0.4/lintest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/appium_utils.py` & `linktest-2.0.4/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/clean_data.py` & `linktest-2.0.4/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/conver_xml_into_db.py` & `linktest-2.0.4/lintest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/run_testcase_thread.py` & `linktest-2.0.4/lintest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/selenium_helper.py` & `linktest-2.0.4/lintest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/memory_usage.py` & `linktest-2.0.4/lintest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/update_config.py` & `linktest-2.0.4/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/auto_generate_testcase_list.py` & `linktest-2.0.4/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/database_helper.py` & `linktest-2.0.4/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/get_ios_devices_list.py` & `linktest-2.0.4/lintest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/get_project_info.py` & `linktest-2.0.4/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/get_adb_devices.py` & `linktest-2.0.4/lintest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/main.py` & `linktest-2.0.4/linktest/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 - Facilitates setting Authentication tokens for UI test cases.
 - Automatically installs the appropriate Chromedriver for UI test cases based on the Chrome version.
 - Allows saving execution logs into testdb, which can be integrated with linktest-dashboard to display execution log summaries, details, and histories.
 - Supports assigning multiple tags to a single test case for easy grouping.
 - Allows setting priorities for test cases, offering another way to group test cases.
 - Automatically store HTTP request and response data in the corresponding log file.
 - Easily and directly save specified data to the GlobalDataList between different test cases (useful for aggregation and summary functions).
+- integrate with test-engine-platform (easy to write the E2E testcases)
 
 To utilize the linktest framework, your project must have two configuration files (these will be auto-generated if not present):
 
 1. settings/__init__.py is used to configure the following items for linktest:
     - Environment (test environment: UAT, QA, PROD, etc.)
     - TESTCASE_TIMEOUT (if a test case's execution is not complete after Testcase_Timeout seconds, a TimeoutException will be thrown)
     - RERUN_FLAG (controls rerunning of failed test cases; default is False)
@@ -650,25 +651,26 @@
                 executing_testcase.full_tc_folder = testcase_full_folder
 
                 if executing_testcase.rerun_tag == 0:
                     logger, logfile_full_name = self.create_logger(testcase.__name__,
                                                                    executing_testcase.full_tc_folder,
                                                                    "test.log")
                     executing_testcase.logger = logger
-                    executing_testcase.requests = LoggedRequests(executing_testcase)
+                    executing_testcase.requests = LoggedRequests(logger)
 
                     executing_testcase.logfile_full_name = logfile_full_name
                     executing_testcase.log_file_path = logfile_full_name.replace(project_info.output_folder, ".")
 
                 else:
                     logger_rerun, logfile_full_name_rerun = self.create_logger(testcase.__name__,
                                                                                executing_testcase.full_tc_folder,
                                                                                "test.rerun.log")
                     executing_testcase.logger = logger_rerun
-                    executing_testcase.requests = LoggedRequests(executing_testcase)
+                    executing_testcase.requests = LoggedRequests(logger_rerun)
+
 
                     executing_testcase.logfile_full_name = logfile_full_name_rerun
                     executing_testcase.log_file_path = logfile_full_name_rerun.replace(project_info.output_folder, ".")
 
                 executing_testcase.logger.info(
                     "====================== TestCase: {TestCaseName} Execution Log ======================".format(
                         TestCaseName=testcase.__name__) + os.linesep)
```

### Comparing `linktest-2.0.3/linktest/framework_log.py` & `linktest-2.0.4/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.0.4/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest/doctor.py` & `linktest-2.0.4/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.3/linktest.egg-info/SOURCES.txt` & `linktest-2.0.4/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

