# Comparing `tmp/linktest-2.0.4.tar.gz` & `tmp/linktest-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.0.4.tar", last modified: Tue May  9 05:27:52 2023, max compression
+gzip compressed data, was "linktest-2.0.5.tar", last modified: Tue May  9 06:08:52 2023, max compression
```

## Comparing `linktest-2.0.4.tar` & `linktest-2.0.5.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 05:27:52.514191 linktest-2.0.4/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      100 2023-05-09 05:27:52.512964 linktest-2.0.4/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 05:27:52.417780 linktest-2.0.4/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-05-09 05:21:50.000000 linktest-2.0.4/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2023-04-26 05:36:37.000000 linktest-2.0.4/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2023-04-25 07:00:45.000000 linktest-2.0.4/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2023-04-26 05:52:13.000000 linktest-2.0.4/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16834 2023-04-26 05:58:55.000000 linktest-2.0.4/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9712 2023-04-26 06:07:11.000000 linktest-2.0.4/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2023-04-26 06:20:46.000000 linktest-2.0.4/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7110 2023-04-26 06:23:55.000000 linktest-2.0.4/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2023-04-26 06:27:01.000000 linktest-2.0.4/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16356 2023-04-25 07:00:45.000000 linktest-2.0.4/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      916 2023-04-26 06:27:01.000000 linktest-2.0.4/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2023-04-25 12:18:59.000000 linktest-2.0.4/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31803 2023-04-26 06:28:34.000000 linktest-2.0.4/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2023-04-25 13:06:43.000000 linktest-2.0.4/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9672 2023-05-09 05:27:04.000000 linktest-2.0.4/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   100564 2023-05-09 05:25:01.000000 linktest-2.0.4/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2023-04-25 12:18:59.000000 linktest-2.0.4/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7822 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      527 2023-05-09 05:21:39.000000 linktest-2.0.4/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2023-04-25 12:18:59.000000 linktest-2.0.4/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-04-25 06:57:24.000000 linktest-2.0.4/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2023-04-26 06:29:23.000000 linktest-2.0.4/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 05:27:52.425678 linktest-2.0.4/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      100 2023-05-09 05:27:52.000000 linktest-2.0.4/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2190 2023-05-09 05:27:52.000000 linktest-2.0.4/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2023-05-09 05:27:52.000000 linktest-2.0.4/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      116 2023-05-09 05:27:52.000000 linktest-2.0.4/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2023-05-09 05:27:52.000000 linktest-2.0.4/linktest.egg-info/top_level.txt
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 05:27:52.511074 linktest-2.0.4/lintest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      461 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10758 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2629 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/auto_generate_test_suite.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    30653 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    17741 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2130 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/auto_organize_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10929 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1786 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7062 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2511 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16348 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1481 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3135 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31798 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      176 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/lintest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10159 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   111768 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1071 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7822 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      420 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3052 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3597 2023-04-25 06:29:43.000000 linktest-2.0.4/lintest/xml_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2023-05-09 05:27:52.514344 linktest-2.0.4/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      454 2023-05-09 05:27:37.000000 linktest-2.0.4/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 06:08:52.612394 linktest-2.0.5/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      100 2023-05-09 06:08:52.611794 linktest-2.0.5/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 06:08:52.537972 linktest-2.0.5/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-05-09 06:02:34.000000 linktest-2.0.5/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2023-04-26 05:36:37.000000 linktest-2.0.5/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-04-25 06:57:24.000000 linktest-2.0.5/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2023-04-25 07:00:45.000000 linktest-2.0.5/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2023-04-26 05:52:13.000000 linktest-2.0.5/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16834 2023-04-26 05:58:55.000000 linktest-2.0.5/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9712 2023-04-26 06:07:11.000000 linktest-2.0.5/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2023-04-26 06:20:46.000000 linktest-2.0.5/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-04-25 06:57:24.000000 linktest-2.0.5/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7110 2023-04-26 06:23:55.000000 linktest-2.0.5/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2023-04-26 06:27:01.000000 linktest-2.0.5/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16356 2023-04-25 07:00:45.000000 linktest-2.0.5/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      916 2023-04-26 06:27:01.000000 linktest-2.0.5/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-04-25 06:57:24.000000 linktest-2.0.5/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-04-25 06:57:24.000000 linktest-2.0.5/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-04-25 06:57:24.000000 linktest-2.0.5/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2023-04-25 12:18:59.000000 linktest-2.0.5/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31803 2023-04-26 06:28:34.000000 linktest-2.0.5/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-04-25 06:57:24.000000 linktest-2.0.5/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2023-04-25 13:06:43.000000 linktest-2.0.5/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9672 2023-05-09 05:27:04.000000 linktest-2.0.5/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   100613 2023-05-09 06:02:21.000000 linktest-2.0.5/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-04-25 06:57:24.000000 linktest-2.0.5/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2023-04-25 12:18:59.000000 linktest-2.0.5/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-04-25 06:57:24.000000 linktest-2.0.5/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-04-25 06:57:24.000000 linktest-2.0.5/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7822 2023-04-25 06:57:24.000000 linktest-2.0.5/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-04-25 06:57:24.000000 linktest-2.0.5/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      527 2023-05-09 06:02:43.000000 linktest-2.0.5/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-04-25 06:57:24.000000 linktest-2.0.5/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-04-25 06:57:24.000000 linktest-2.0.5/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-04-25 06:57:24.000000 linktest-2.0.5/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-04-25 06:57:24.000000 linktest-2.0.5/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2023-04-25 12:18:59.000000 linktest-2.0.5/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-04-25 06:57:24.000000 linktest-2.0.5/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2023-04-26 06:29:23.000000 linktest-2.0.5/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 06:08:52.545634 linktest-2.0.5/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      100 2023-05-09 06:08:52.000000 linktest-2.0.5/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2190 2023-05-09 06:08:52.000000 linktest-2.0.5/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2023-05-09 06:08:52.000000 linktest-2.0.5/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      116 2023-05-09 06:08:52.000000 linktest-2.0.5/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2023-05-09 06:08:52.000000 linktest-2.0.5/linktest.egg-info/top_level.txt
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-09 06:08:52.610260 linktest-2.0.5/lintest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      461 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10758 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2629 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/auto_generate_test_suite.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    30653 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    17741 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2130 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/auto_organize_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10929 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1786 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7062 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2511 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16348 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1481 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3135 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31798 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      176 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/lintest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10159 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   111768 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1071 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7822 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      420 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3052 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3597 2023-04-25 06:29:43.000000 linktest-2.0.5/lintest/xml_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2023-05-09 06:08:52.612574 linktest-2.0.5/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      454 2023-05-09 06:08:44.000000 linktest-2.0.5/setup.py
```

### Comparing `linktest-2.0.4/linktest/appium_utils.py` & `linktest-2.0.5/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/auto_generate_testcase_list.py` & `linktest-2.0.5/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.0.5/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/base_testcase.py` & `linktest-2.0.5/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/clean_data.py` & `linktest-2.0.5/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/conver_xml_into_db.py` & `linktest-2.0.5/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/database_helper.py` & `linktest-2.0.5/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/date_utilities.py` & `linktest-2.0.5/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/doctor.py` & `linktest-2.0.5/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/framework_log.py` & `linktest-2.0.5/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/get_adb_devices.py` & `linktest-2.0.5/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/get_ios_devices_list.py` & `linktest-2.0.5/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/get_platform_info.py` & `linktest-2.0.5/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/get_project_info.py` & `linktest-2.0.5/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/html_report.py` & `linktest-2.0.5/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/logged_requests.py` & `linktest-2.0.5/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/main.py` & `linktest-2.0.5/linktest/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1628,14 +1628,16 @@
                 try:
                     if argument.__contains__("."):
                         print("Warning: there are '.' in tag {tag}, here replace '.' as '_' ".format(tag=argument))
                         tag_name = argument.replace(".", "_")
                     else:
                         tag_name = argument
 
+                    tag_name = tag_name.lower()
+
                     # first try to find the argument as a tag name
                     if isinstance(testcase_dict_for_tags[tag_name], list):
                         for testcase_for_tag in testcase_dict_for_tags[tag_name]:
                             testcase_list.append(testcase_for_tag)
 
                     elif issubclass(testcase_dict_for_tags[tag_name], base_testcase.BaseTestCase):
                         testcase_list.append(testcase_dict_for_tags[tag_name])
```

### Comparing `linktest-2.0.4/linktest/memory_usage.py` & `linktest-2.0.5/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/run.py` & `linktest-2.0.5/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/run_testcase_thread.py` & `linktest-2.0.5/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/scp_report_to_specified_path.py` & `linktest-2.0.5/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/selenium_helper.py` & `linktest-2.0.5/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/setup.py` & `linktest-2.0.5/linktest/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='linktest',
-    version='2.0.4',
+    version='2.0.5',
     author='Wang Lin',
     author_email='think_wl@163.com',
     packages=['linktest'],
     install_requires=[
         "psutil",
         "requests",
         "curlify",
```

### Comparing `linktest-2.0.4/linktest/timeout_thread.py` & `linktest-2.0.5/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/ui_testcase.py` & `linktest-2.0.5/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/update_config.py` & `linktest-2.0.5/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest/xml_report.py` & `linktest-2.0.5/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/linktest.egg-info/SOURCES.txt` & `linktest-2.0.5/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/appium_utils.py` & `linktest-2.0.5/lintest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/auto_generate_test_suite.py` & `linktest-2.0.5/lintest/auto_generate_test_suite.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/auto_generate_testcase_list.py` & `linktest-2.0.5/lintest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/auto_generate_testcase_list_from_csv.py` & `linktest-2.0.5/lintest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/auto_organize_testcase.py` & `linktest-2.0.5/lintest/auto_organize_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/base_testcase.py` & `linktest-2.0.5/lintest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/clean_data.py` & `linktest-2.0.5/lintest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/conver_xml_into_db.py` & `linktest-2.0.5/lintest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/database_helper.py` & `linktest-2.0.5/lintest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/date_utilities.py` & `linktest-2.0.5/lintest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/doctor.py` & `linktest-2.0.5/lintest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/framework_log.py` & `linktest-2.0.5/lintest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/get_adb_devices.py` & `linktest-2.0.5/lintest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/get_ios_devices_list.py` & `linktest-2.0.5/lintest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/get_platform_info.py` & `linktest-2.0.5/lintest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/get_project_info.py` & `linktest-2.0.5/lintest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/html_report.py` & `linktest-2.0.5/lintest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/logged_requests.py` & `linktest-2.0.5/lintest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/main.py` & `linktest-2.0.5/lintest/main.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/memory_usage.py` & `linktest-2.0.5/lintest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/run.py` & `linktest-2.0.5/lintest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/run_testcase_thread.py` & `linktest-2.0.5/lintest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/scp_report_to_specified_path.py` & `linktest-2.0.5/lintest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/selenium_helper.py` & `linktest-2.0.5/lintest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/timeout_thread.py` & `linktest-2.0.5/lintest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/ui_testcase.py` & `linktest-2.0.5/lintest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/update_config.py` & `linktest-2.0.5/lintest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.4/lintest/xml_report.py` & `linktest-2.0.5/lintest/xml_report.py`

 * *Files identical despite different names*

