# Comparing `tmp/linktest-2.0.6.tar.gz` & `tmp/linktest-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.0.6.tar", last modified: Tue May  9 07:10:47 2023, max compression
+gzip compressed data, was "linktest-2.0.7.tar", last modified: Tue May  9 07:28:53 2023, max compression
```

## Comparing `linktest-2.0.6.tar` & `linktest-2.0.7.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 07:10:47.792403 linktest-2.0.6/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      100 2023-05-09 07:10:47.791406 linktest-2.0.6/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 07:10:47.703683 linktest-2.0.6/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-05-09 07:09:42.000000 linktest-2.0.6/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2023-04-26 05:36:37.000000 linktest-2.0.6/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-04-25 06:57:24.000000 linktest-2.0.6/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2023-04-25 07:00:45.000000 linktest-2.0.6/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2023-04-26 05:52:13.000000 linktest-2.0.6/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16834 2023-04-26 05:58:55.000000 linktest-2.0.6/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9712 2023-04-26 06:07:11.000000 linktest-2.0.6/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2023-04-26 06:20:46.000000 linktest-2.0.6/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-04-25 06:57:24.000000 linktest-2.0.6/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7110 2023-04-26 06:23:55.000000 linktest-2.0.6/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2023-04-26 06:27:01.000000 linktest-2.0.6/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16356 2023-04-25 07:00:45.000000 linktest-2.0.6/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      916 2023-04-26 06:27:01.000000 linktest-2.0.6/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-04-25 06:57:24.000000 linktest-2.0.6/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-04-25 06:57:24.000000 linktest-2.0.6/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-04-25 06:57:24.000000 linktest-2.0.6/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2023-04-25 12:18:59.000000 linktest-2.0.6/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31803 2023-04-26 06:28:34.000000 linktest-2.0.6/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-04-25 06:57:24.000000 linktest-2.0.6/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2023-04-25 13:06:43.000000 linktest-2.0.6/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8706 2023-05-09 07:09:35.000000 linktest-2.0.6/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   100613 2023-05-09 06:02:21.000000 linktest-2.0.6/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-04-25 06:57:24.000000 linktest-2.0.6/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2023-04-25 12:18:59.000000 linktest-2.0.6/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-04-25 06:57:24.000000 linktest-2.0.6/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-04-25 06:57:24.000000 linktest-2.0.6/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7822 2023-04-25 06:57:24.000000 linktest-2.0.6/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-04-25 06:57:24.000000 linktest-2.0.6/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      527 2023-05-09 07:09:51.000000 linktest-2.0.6/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-04-25 06:57:24.000000 linktest-2.0.6/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-04-25 06:57:24.000000 linktest-2.0.6/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-04-25 06:57:24.000000 linktest-2.0.6/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-04-25 06:57:24.000000 linktest-2.0.6/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2023-04-25 12:18:59.000000 linktest-2.0.6/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-04-25 06:57:24.000000 linktest-2.0.6/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2023-04-26 06:29:23.000000 linktest-2.0.6/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 07:10:47.713175 linktest-2.0.6/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      100 2023-05-09 07:10:47.000000 linktest-2.0.6/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2190 2023-05-09 07:10:47.000000 linktest-2.0.6/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2023-05-09 07:10:47.000000 linktest-2.0.6/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      116 2023-05-09 07:10:47.000000 linktest-2.0.6/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2023-05-09 07:10:47.000000 linktest-2.0.6/linktest.egg-info/top_level.txt
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 07:10:47.789734 linktest-2.0.6/lintest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      461 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10758 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2629 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/auto_generate_test_suite.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    30653 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    17741 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2130 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/auto_organize_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10929 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1786 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7062 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2511 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16348 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1481 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3135 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31798 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      176 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/lintest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10159 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   111768 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1071 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7822 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      420 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3052 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3597 2023-04-25 06:29:43.000000 linktest-2.0.6/lintest/xml_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2023-05-09 07:10:47.792579 linktest-2.0.6/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      454 2023-05-09 07:10:42.000000 linktest-2.0.6/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 07:28:53.951580 linktest-2.0.7/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      100 2023-05-09 07:28:53.950883 linktest-2.0.7/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 07:28:53.858067 linktest-2.0.7/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-05-09 07:25:48.000000 linktest-2.0.7/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2023-04-26 05:36:37.000000 linktest-2.0.7/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-04-25 06:57:24.000000 linktest-2.0.7/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2023-04-25 07:00:45.000000 linktest-2.0.7/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2023-04-26 05:52:13.000000 linktest-2.0.7/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16834 2023-04-26 05:58:55.000000 linktest-2.0.7/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9712 2023-04-26 06:07:11.000000 linktest-2.0.7/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2023-04-26 06:20:46.000000 linktest-2.0.7/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-04-25 06:57:24.000000 linktest-2.0.7/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7110 2023-04-26 06:23:55.000000 linktest-2.0.7/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2023-04-26 06:27:01.000000 linktest-2.0.7/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16356 2023-04-25 07:00:45.000000 linktest-2.0.7/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      916 2023-04-26 06:27:01.000000 linktest-2.0.7/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-04-25 06:57:24.000000 linktest-2.0.7/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-04-25 06:57:24.000000 linktest-2.0.7/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-04-25 06:57:24.000000 linktest-2.0.7/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2023-04-25 12:18:59.000000 linktest-2.0.7/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31803 2023-04-26 06:28:34.000000 linktest-2.0.7/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-04-25 06:57:24.000000 linktest-2.0.7/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2023-04-25 13:06:43.000000 linktest-2.0.7/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8706 2023-05-09 07:09:35.000000 linktest-2.0.7/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   100661 2023-05-09 07:25:32.000000 linktest-2.0.7/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-04-25 06:57:24.000000 linktest-2.0.7/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2023-04-25 12:18:59.000000 linktest-2.0.7/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-04-25 06:57:24.000000 linktest-2.0.7/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-04-25 06:57:24.000000 linktest-2.0.7/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7822 2023-04-25 06:57:24.000000 linktest-2.0.7/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-04-25 06:57:24.000000 linktest-2.0.7/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      527 2023-05-09 07:25:58.000000 linktest-2.0.7/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-04-25 06:57:24.000000 linktest-2.0.7/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-04-25 06:57:24.000000 linktest-2.0.7/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-04-25 06:57:24.000000 linktest-2.0.7/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-04-25 06:57:24.000000 linktest-2.0.7/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2023-04-25 12:18:59.000000 linktest-2.0.7/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-04-25 06:57:24.000000 linktest-2.0.7/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2023-04-26 06:29:23.000000 linktest-2.0.7/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 07:28:53.867403 linktest-2.0.7/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      100 2023-05-09 07:28:53.000000 linktest-2.0.7/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2190 2023-05-09 07:28:53.000000 linktest-2.0.7/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2023-05-09 07:28:53.000000 linktest-2.0.7/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      116 2023-05-09 07:28:53.000000 linktest-2.0.7/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2023-05-09 07:28:53.000000 linktest-2.0.7/linktest.egg-info/top_level.txt
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 07:28:53.949118 linktest-2.0.7/lintest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      461 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10758 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2629 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/auto_generate_test_suite.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    30653 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    17741 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2130 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/auto_organize_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10929 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1786 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7062 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2511 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16348 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1481 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3135 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31798 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      176 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/lintest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10159 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   111768 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1071 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7822 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      420 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3052 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3597 2023-04-25 06:29:43.000000 linktest-2.0.7/lintest/xml_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2023-05-09 07:28:53.951719 linktest-2.0.7/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      454 2023-05-09 07:26:23.000000 linktest-2.0.7/setup.py
```

### Comparing `linktest-2.0.6/linktest/appium_utils.py` & `linktest-2.0.7/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/auto_generate_testcase_list.py` & `linktest-2.0.7/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.0.7/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/base_testcase.py` & `linktest-2.0.7/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/clean_data.py` & `linktest-2.0.7/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/conver_xml_into_db.py` & `linktest-2.0.7/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/database_helper.py` & `linktest-2.0.7/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/date_utilities.py` & `linktest-2.0.7/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/doctor.py` & `linktest-2.0.7/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/framework_log.py` & `linktest-2.0.7/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/get_adb_devices.py` & `linktest-2.0.7/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/get_ios_devices_list.py` & `linktest-2.0.7/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/get_platform_info.py` & `linktest-2.0.7/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/get_project_info.py` & `linktest-2.0.7/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/html_report.py` & `linktest-2.0.7/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/logged_requests.py` & `linktest-2.0.7/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/main.py` & `linktest-2.0.7/linktest/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1629,14 +1629,15 @@
                     if argument.__contains__("."):
                         print("Warning: there are '.' in tag {tag}, here replace '.' as '_' ".format(tag=argument))
                         tag_name = argument.replace(".", "_")
                     else:
                         tag_name = argument
 
                     tag_name = tag_name.lower()
+                    argument = argument.lower()
 
                     # first try to find the argument as a tag name
                     if isinstance(testcase_dict_for_tags[tag_name], list):
                         for testcase_for_tag in testcase_dict_for_tags[tag_name]:
                             testcase_list.append(testcase_for_tag)
 
                     elif issubclass(testcase_dict_for_tags[tag_name], base_testcase.BaseTestCase):
```

### Comparing `linktest-2.0.6/linktest/memory_usage.py` & `linktest-2.0.7/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/run.py` & `linktest-2.0.7/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/run_testcase_thread.py` & `linktest-2.0.7/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/scp_report_to_specified_path.py` & `linktest-2.0.7/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/selenium_helper.py` & `linktest-2.0.7/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/setup.py` & `linktest-2.0.7/linktest/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='linktest',
-    version='2.0.6',
+    version='2.0.7',
     author='Wang Lin',
     author_email='think_wl@163.com',
     packages=['linktest'],
     install_requires=[
         "psutil",
         "requests",
         "curlify",
```

### Comparing `linktest-2.0.6/linktest/timeout_thread.py` & `linktest-2.0.7/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/ui_testcase.py` & `linktest-2.0.7/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/update_config.py` & `linktest-2.0.7/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest/xml_report.py` & `linktest-2.0.7/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/linktest.egg-info/SOURCES.txt` & `linktest-2.0.7/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/appium_utils.py` & `linktest-2.0.7/lintest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/auto_generate_test_suite.py` & `linktest-2.0.7/lintest/auto_generate_test_suite.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/auto_generate_testcase_list.py` & `linktest-2.0.7/lintest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/auto_generate_testcase_list_from_csv.py` & `linktest-2.0.7/lintest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/auto_organize_testcase.py` & `linktest-2.0.7/lintest/auto_organize_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/base_testcase.py` & `linktest-2.0.7/lintest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/clean_data.py` & `linktest-2.0.7/lintest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/conver_xml_into_db.py` & `linktest-2.0.7/lintest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/database_helper.py` & `linktest-2.0.7/lintest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/date_utilities.py` & `linktest-2.0.7/lintest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/doctor.py` & `linktest-2.0.7/lintest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/framework_log.py` & `linktest-2.0.7/lintest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/get_adb_devices.py` & `linktest-2.0.7/lintest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/get_ios_devices_list.py` & `linktest-2.0.7/lintest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/get_platform_info.py` & `linktest-2.0.7/lintest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/get_project_info.py` & `linktest-2.0.7/lintest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/html_report.py` & `linktest-2.0.7/lintest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/logged_requests.py` & `linktest-2.0.7/lintest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/main.py` & `linktest-2.0.7/lintest/main.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/memory_usage.py` & `linktest-2.0.7/lintest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/run.py` & `linktest-2.0.7/lintest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/run_testcase_thread.py` & `linktest-2.0.7/lintest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/scp_report_to_specified_path.py` & `linktest-2.0.7/lintest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/selenium_helper.py` & `linktest-2.0.7/lintest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/timeout_thread.py` & `linktest-2.0.7/lintest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/ui_testcase.py` & `linktest-2.0.7/lintest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/update_config.py` & `linktest-2.0.7/lintest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.6/lintest/xml_report.py` & `linktest-2.0.7/lintest/xml_report.py`

 * *Files identical despite different names*

