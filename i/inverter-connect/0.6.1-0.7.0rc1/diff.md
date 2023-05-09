# Comparing `tmp/inverter-connect-0.6.1.tar.gz` & `tmp/inverter-connect-0.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inverter-connect-0.6.1.tar", last modified: Sun May  7 10:42:43 2023, max compression
+gzip compressed data, was "inverter-connect-0.7.0rc1.tar", last modified: Tue May  9 16:28:33 2023, max compression
```

## Comparing `inverter-connect-0.6.1.tar` & `inverter-connect-0.7.0rc1.tar`

### file list

```diff
@@ -1,76 +1,67 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.6.1/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.6.1/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-05-03 17:50:50.000000 inverter-connect-0.6.1/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.6.1/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)    16300 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)    15886 2023-05-06 10:27:49.000000 inverter-connect-0.6.1/README.md
--rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:23:42.000000 inverter-connect-0.6.1/cli.py
--rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:24:01.000000 inverter-connect-0.6.1/dev-cli.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.6.1/inverter/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.6.1/inverter/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.6.1/inverter/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.6.1/inverter/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)      148 2023-05-07 09:25:42.000000 inverter-connect-0.6.1/inverter/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.6.1/inverter/__main__.py
--rw-rw-r--   0 jens      (1000) users      (100)     4852 2023-05-07 09:15:43.000000 inverter-connect-0.6.1/inverter/api.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/cli/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.6.1/inverter/cli/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)    13874 2023-05-07 09:17:33.000000 inverter-connect-0.6.1/inverter/cli/cli_app.py
--rw-rw-r--   0 jens      (1000) users      (100)     7864 2023-05-03 17:42:33.000000 inverter-connect-0.6.1/inverter/cli/dev.py
--rw-rw-r--   0 jens      (1000) users      (100)    10423 2023-05-07 09:11:34.000000 inverter-connect-0.6.1/inverter/connection.py
--rw-rw-r--   0 jens      (1000) users      (100)      312 2023-05-06 10:27:41.000000 inverter-connect-0.6.1/inverter/constants.py
--rw-rw-r--   0 jens      (1000) users      (100)     1768 2023-05-06 10:26:14.000000 inverter-connect-0.6.1/inverter/daily_reset.py
--rw-rw-r--   0 jens      (1000) users      (100)     3700 2023-05-07 09:03:56.000000 inverter-connect-0.6.1/inverter/data_types.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/definitions/
--rw-rw-r--   0 jens      (1000) users      (100)     2918 2023-04-23 17:07:32.000000 inverter-connect-0.6.1/inverter/definitions/deye_2mppt.yaml
--rw-rw-r--   0 jens      (1000) users      (100)      213 2023-05-06 09:30:48.000000 inverter-connect-0.6.1/inverter/definitions/deye_2mppt_validations.yaml
--rw-rw-r--   0 jens      (1000) users      (100)     2260 2023-05-06 10:26:15.000000 inverter-connect-0.6.1/inverter/definitions.py
--rw-rw-r--   0 jens      (1000) users      (100)      538 2023-05-06 10:11:26.000000 inverter-connect-0.6.1/inverter/exceptions.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/mqtt4homeassistant/
--rw-rw-r--   0 jens      (1000) users      (100)       22 2023-04-24 06:39:33.000000 inverter-connect-0.6.1/inverter/mqtt4homeassistant/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1892 2023-04-27 06:35:47.000000 inverter-connect-0.6.1/inverter/mqtt4homeassistant/converter.py
--rw-rw-r--   0 jens      (1000) users      (100)     1209 2023-04-24 07:07:57.000000 inverter-connect-0.6.1/inverter/mqtt4homeassistant/data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)     3803 2023-04-24 07:36:06.000000 inverter-connect-0.6.1/inverter/mqtt4homeassistant/mqtt.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/mqtt4homeassistant/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.6.1/inverter/mqtt4homeassistant/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2136 2023-04-27 06:35:47.000000 inverter-connect-0.6.1/inverter/mqtt4homeassistant/tests/test_converter.py
--rw-rw-r--   0 jens      (1000) users      (100)      245 2023-04-24 06:13:14.000000 inverter-connect-0.6.1/inverter/mqtt4homeassistant/tests/test_doctests.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/mqtt4homeassistant/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.6.1/inverter/mqtt4homeassistant/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      315 2023-04-23 16:57:27.000000 inverter-connect-0.6.1/inverter/mqtt4homeassistant/utilities/string_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     3138 2023-05-07 09:16:41.000000 inverter-connect-0.6.1/inverter/publish_loop.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/tests/
--rw-rw-r--   0 jens      (1000) users      (100)      269 2023-04-23 16:25:11.000000 inverter-connect-0.6.1/inverter/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3293 2023-05-06 10:24:09.000000 inverter-connect-0.6.1/inverter/tests/test_api.py
--rw-rw-r--   0 jens      (1000) users      (100)     1230 2023-05-07 09:25:28.000000 inverter-connect-0.6.1/inverter/tests/test_cli.py
--rw-rw-r--   0 jens      (1000) users      (100)      826 2023-05-06 10:26:14.000000 inverter-connect-0.6.1/inverter/tests/test_connect.py
--rw-rw-r--   0 jens      (1000) users      (100)     5880 2023-05-06 10:42:16.000000 inverter-connect-0.6.1/inverter/tests/test_daily_reset.py
--rw-rw-r--   0 jens      (1000) users      (100)     1589 2023-05-06 10:41:55.000000 inverter-connect-0.6.1/inverter/tests/test_definitions.py
--rw-rw-r--   0 jens      (1000) users      (100)      211 2023-04-17 13:29:40.000000 inverter-connect-0.6.1/inverter/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     2641 2023-05-03 17:38:17.000000 inverter-connect-0.6.1/inverter/tests/test_project_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     3422 2023-05-05 19:51:25.000000 inverter-connect-0.6.1/inverter/tests/test_readme.py
--rw-rw-r--   0 jens      (1000) users      (100)     2114 2023-05-06 11:19:29.000000 inverter-connect-0.6.1/inverter/tests/test_validators.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.6.1/inverter/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2179 2023-05-06 10:25:25.000000 inverter-connect-0.6.1/inverter/utilities/cli.py
--rw-rw-r--   0 jens      (1000) users      (100)      925 2023-04-24 15:15:46.000000 inverter-connect-0.6.1/inverter/utilities/credentials.py
--rw-rw-r--   0 jens      (1000) users      (100)      175 2023-04-24 15:15:46.000000 inverter-connect-0.6.1/inverter/utilities/log_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-24 08:58:03.000000 inverter-connect-0.6.1/inverter/utilities/modbus_converter.py
--rw-rw-r--   0 jens      (1000) users      (100)     1562 2023-05-06 10:34:37.000000 inverter-connect-0.6.1/inverter/validators.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter_connect.egg-info/
--rw-rw-r--   0 jens      (1000) users      (100)    16300 2023-05-07 10:42:43.000000 inverter-connect-0.6.1/inverter_connect.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     1771 2023-05-07 10:42:43.000000 inverter-connect-0.6.1/inverter_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-07 10:42:43.000000 inverter-connect-0.6.1/inverter_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)       93 2023-05-07 10:42:43.000000 inverter-connect-0.6.1/inverter_connect.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      277 2023-05-07 10:42:43.000000 inverter-connect-0.6.1/inverter_connect.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)        9 2023-05-07 10:42:43.000000 inverter-connect-0.6.1/inverter_connect.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) users      (100)     4882 2023-05-06 09:28:26.000000 inverter-connect-0.6.1/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    53370 2023-05-06 09:28:51.000000 inverter-connect-0.6.1/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)     7830 2023-05-06 09:28:32.000000 inverter-connect-0.6.1/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.7.0rc1/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.7.0rc1/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1570 2023-05-09 16:20:44.000000 inverter-connect-0.7.0rc1/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.7.0rc1/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)    17208 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)    16791 2023-05-09 16:26:48.000000 inverter-connect-0.7.0rc1/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:23:42.000000 inverter-connect-0.7.0rc1/cli.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:24:01.000000 inverter-connect-0.7.0rc1/dev-cli.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/inverter/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.7.0rc1/inverter/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.7.0rc1/inverter/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/inverter/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/inverter/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.7.0rc1/inverter/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.7.0rc1/inverter/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)      151 2023-05-08 20:06:40.000000 inverter-connect-0.7.0rc1/inverter/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.7.0rc1/inverter/__main__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4860 2023-05-08 19:17:03.000000 inverter-connect-0.7.0rc1/inverter/api.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/inverter/cli/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.7.0rc1/inverter/cli/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)    14946 2023-05-09 06:54:43.000000 inverter-connect-0.7.0rc1/inverter/cli/cli_app.py
+-rw-rw-r--   0 jens      (1000) users      (100)     8894 2023-05-09 16:16:52.000000 inverter-connect-0.7.0rc1/inverter/cli/dev.py
+-rw-rw-r--   0 jens      (1000) users      (100)    10495 2023-05-08 19:17:03.000000 inverter-connect-0.7.0rc1/inverter/connection.py
+-rw-rw-r--   0 jens      (1000) users      (100)      361 2023-05-08 16:20:47.000000 inverter-connect-0.7.0rc1/inverter/constants.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1768 2023-05-06 10:26:14.000000 inverter-connect-0.7.0rc1/inverter/daily_reset.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3795 2023-05-09 06:54:47.000000 inverter-connect-0.7.0rc1/inverter/data_types.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/inverter/definitions/
+-rw-rw-r--   0 jens      (1000) users      (100)     2918 2023-04-23 17:07:32.000000 inverter-connect-0.7.0rc1/inverter/definitions/deye_2mppt.yaml
+-rw-rw-r--   0 jens      (1000) users      (100)      213 2023-05-06 09:30:48.000000 inverter-connect-0.7.0rc1/inverter/definitions/deye_2mppt_validations.yaml
+-rw-rw-r--   0 jens      (1000) users      (100)     2260 2023-05-06 10:26:15.000000 inverter-connect-0.7.0rc1/inverter/definitions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      538 2023-05-06 10:11:26.000000 inverter-connect-0.7.0rc1/inverter/exceptions.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3350 2023-05-09 07:31:07.000000 inverter-connect-0.7.0rc1/inverter/publish_loop.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/inverter/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)      256 2023-05-08 19:20:13.000000 inverter-connect-0.7.0rc1/inverter/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      548 2023-05-08 19:29:24.000000 inverter-connect-0.7.0rc1/inverter/tests/fixtures.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3293 2023-05-06 10:24:09.000000 inverter-connect-0.7.0rc1/inverter/tests/test_api.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1412 2023-05-09 07:33:09.000000 inverter-connect-0.7.0rc1/inverter/tests/test_cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)      826 2023-05-06 10:26:14.000000 inverter-connect-0.7.0rc1/inverter/tests/test_connect.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5888 2023-05-08 19:33:47.000000 inverter-connect-0.7.0rc1/inverter/tests/test_daily_reset.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1563 2023-05-08 19:29:30.000000 inverter-connect-0.7.0rc1/inverter/tests/test_definitions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      211 2023-04-17 13:29:40.000000 inverter-connect-0.7.0rc1/inverter/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2641 2023-05-03 17:38:17.000000 inverter-connect-0.7.0rc1/inverter/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5436 2023-05-09 06:29:28.000000 inverter-connect-0.7.0rc1/inverter/tests/test_readme.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1975 2023-05-08 17:44:09.000000 inverter-connect-0.7.0rc1/inverter/tests/test_user_settings.py
+-rw-rw-r--   0 jens      (1000) users      (100)      537 2023-05-09 07:37:24.000000 inverter-connect-0.7.0rc1/inverter/tests/test_user_settings_migrate_old_settings_1.snapshot.toml
+-rw-rw-r--   0 jens      (1000) users      (100)     2114 2023-05-08 19:34:46.000000 inverter-connect-0.7.0rc1/inverter/tests/test_validators.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2682 2023-05-09 07:37:21.000000 inverter-connect-0.7.0rc1/inverter/user_settings.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/inverter/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.7.0rc1/inverter/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3242 2023-05-09 07:31:16.000000 inverter-connect-0.7.0rc1/inverter/utilities/cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-24 08:58:03.000000 inverter-connect-0.7.0rc1/inverter/utilities/modbus_converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1562 2023-05-06 10:34:37.000000 inverter-connect-0.7.0rc1/inverter/validators.py
+-rw-rw-r--   0 jens      (1000) users      (100)      732 2023-05-08 19:17:53.000000 inverter-connect-0.7.0rc1/inverter/verbosity.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/inverter_connect.egg-info/
+-rw-rw-r--   0 jens      (1000) users      (100)    17208 2023-05-09 16:28:33.000000 inverter-connect-0.7.0rc1/inverter_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     1474 2023-05-09 16:28:33.000000 inverter-connect-0.7.0rc1/inverter_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-09 16:28:33.000000 inverter-connect-0.7.0rc1/inverter_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       93 2023-05-09 16:28:33.000000 inverter-connect-0.7.0rc1/inverter_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      289 2023-05-09 16:28:33.000000 inverter-connect-0.7.0rc1/inverter_connect.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        9 2023-05-09 16:28:33.000000 inverter-connect-0.7.0rc1/inverter_connect.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     4940 2023-05-08 16:12:10.000000 inverter-connect-0.7.0rc1/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    53766 2023-05-08 16:13:00.000000 inverter-connect-0.7.0rc1/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     8423 2023-05-08 16:12:42.000000 inverter-connect-0.7.0rc1/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/setup.cfg
```

### Comparing `inverter-connect-0.6.1/.github/workflows/tests.yml` & `inverter-connect-0.7.0rc1/.github/workflows/tests.yml`

 * *Files 4% similar despite different names*

```diff
@@ -36,18 +36,21 @@
         cache: 'pip' # caching pip dependencies
         cache-dependency-path: '**/requirements.dev.txt'
 
     - name: 'Bootstrap'
       # The first CLI call will create the .venv
       run: |
         ./dev-cli.py version
+        ./dev-cli.py create-default-settings
+        ./cli.py version
 
     - name: 'CLI help'
       run: |
         ./dev-cli.py --help
+        ./cli.py --help
 
     - name: 'Safety'
       run: |
         ./dev-cli.py safety
 
     - name: 'Run tests with Python v${{ matrix.python-version }}'
       run: |
```

### Comparing `inverter-connect-0.6.1/PKG-INFO` & `inverter-connect-0.7.0rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inverter-connect
-Version: 0.6.1
+Version: 0.7.0rc1
 Summary: Get information from Deye Microinverter
 Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/inverter-connect
 Project-URL: Source, https://github.com/jedie/inverter-connect
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
@@ -21,14 +21,21 @@
 Get information from Deye Microinverter
 
 The whole thing is just a learning exercise for now. We will see.
 
 
 # quickstart
 
+## overview
+
+* clone the sources
+* Bootstrap and create default user settings by just call `./cli.py edit-settings`
+* Change the settings for your needs
+* ...use the commands... ;)
+
 Currently just clone the project and just start the cli (that will create a virtualenv and installs every dependencies)
 
 Note: Please enable https://www.piwheels.org/ if you are on a Raspberry Pi !
 
 e.g.:
 ```bash
 ~$ git clone https://github.com/jedie/inverter-connect.git
@@ -43,20 +50,20 @@
 Usage: ./cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
 │ debug-settings           Display (anonymized) MQTT server username and password                  │
+│ edit-settings            Edit the settings file. On first call: Create the default one.          │
 │ print-at-commands        Print one or more AT command values from Inverter.                      │
 │ print-values             Print all known register values from Inverter, e.g.:                    │
 │ publish-loop             Publish current data via MQTT for Home Assistant (endless loop)         │
 │ read-register            Read register(s) from the inverter                                      │
 │ set-time                 Set current date time in the inverter device.                           │
-│ store-settings           Store MQTT server settings.                                             │
 │ test-mqtt-connection     Test connection to MQTT Server                                          │
 │ version                  Print version and exit                                                  │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
@@ -65,61 +72,63 @@
 
 ## publish-loop
 
 Help from `./cli.py print-values --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated publish-loop help start ✂✂✂)
 ```
-Usage: ./cli.py publish-loop [OPTIONS] IP
+Usage: ./cli.py publish-loop [OPTIONS]
 
  Publish current data via MQTT for Home Assistant (endless loop)
  The "Daily Production" count will be cleared in the night, by set the current date time via
  AT-command.
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ *  --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                │
-│                                                              [default: 48899; 1000<=x<=65535]    │
-│                                                              [required]                          │
-│ *  --inverter                TEXT                            Prefix of yaml config files in      │
-│                                                              inverter/definitions/               │
-│                                                              [default: deye_2mppt]               │
-│                                                              [required]                          │
-│    --log/--no-log                                            [default: log]                      │
-│    --verbose/--no-verbose                                    [default: verbose]                  │
-│    --debug/--no-debug                                        [default: no-debug]                 │
-│    --help                                                    Show this message and exit.         │
+│ *  --ip             TEXT                     IP address of your inverter [required]              │
+│ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
+│                                              [required]                                          │
+│ *  --inverter       TEXT                     Prefix of yaml config files in                      │
+│                                              inverter/definitions/                               │
+│                                              [default: deye_2mppt]                               │
+│                                              [required]                                          │
+│    --verbosity  -v  INTEGER RANGE [0<=x<=3]  Verbosity level; Accepts integer value e.g.:        │
+│                                              "--verbose 2" or can be count e.g.: "-vv"           │
+│                                              [default: 1; 0<=x<=3]                               │
+│    --help                                    Show this message and exit.                         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated publish-loop help end ✂✂✂)
 
 
 ----
 
 
 ## print-values
 
 Help from `./cli.py print-values --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated print-values help start ✂✂✂)
 ```
-Usage: ./cli.py print-values [OPTIONS] IP
+Usage: ./cli.py print-values [OPTIONS]
 
  Print all known register values from Inverter, e.g.:
  .../inverter-connect$ ./cli.py print-values 192.168.123.456
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│    --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                │
-│                                                              [default: 48899; 1000<=x<=65535]    │
-│ *  --inverter                TEXT                            Prefix of yaml config files in      │
-│                                                              inverter/definitions/               │
-│                                                              [default: deye_2mppt]               │
-│                                                              [required]                          │
-│    --verbose/--no-verbose                                    [default: verbose]                  │
-│    --debug/--no-debug                                        [default: no-debug]                 │
-│    --help                                                    Show this message and exit.         │
+│ *  --ip             TEXT                     IP address of your inverter [required]              │
+│ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
+│                                              [required]                                          │
+│ *  --inverter       TEXT                     Prefix of yaml config files in                      │
+│                                              inverter/definitions/                               │
+│                                              [default: deye_2mppt]                               │
+│                                              [required]                                          │
+│    --verbosity  -v  INTEGER RANGE [0<=x<=3]  Verbosity level; Accepts integer value e.g.:        │
+│                                              "--verbose 2" or can be count e.g.: "-vv"           │
+│                                              [default: 1; 0<=x<=3]                               │
+│    --help                                    Show this message and exit.                         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated print-values help end ✂✂✂)
 
 Example output of `print-values` call:
 
 ![print-values](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-55.png "2023-04-28_08-55.png")
@@ -129,15 +138,15 @@
 
 ## print-at-commands
 
 Help from `./cli.py print-at-commands --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated print-at-commands help start ✂✂✂)
 ```
-Usage: ./cli.py print-at-commands [OPTIONS] IP [COMMANDS]...
+Usage: ./cli.py print-at-commands [OPTIONS] [COMMANDS]...
 
  Print one or more AT command values from Inverter.
  Use all known AT commands, if no one is given, e.g.:
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456
  Or specify one or more AT-commands, e.g.:
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 WEBVER .../inverter-connect$
  ./cli.py print-at-commands 192.168.123.456 WEBVER WEBU
@@ -145,19 +154,21 @@
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPSER=192.168.1.1 NTPEN=on
  NTPSER NTPEN
  wait a while and request the current date time:
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPTM
  (Note: The prefix "AT+" will be added to every command)
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                   │
-│                                                           [default: 48899; 1000<=x<=65535]       │
-│ --verbose/--no-verbose                                    [default: verbose]                     │
-│ --debug/--no-debug                                        [default: no-debug]                    │
-│ --help                                                    Show this message and exit.            │
+│ *  --ip             TEXT                     IP address of your inverter [required]              │
+│ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
+│                                              [required]                                          │
+│    --verbosity  -v  INTEGER RANGE [0<=x<=3]  Verbosity level; Accepts integer value e.g.:        │
+│                                              "--verbose 2" or can be count e.g.: "-vv"           │
+│                                              [default: 1; 0<=x<=3]                               │
+│    --help                                    Show this message and exit.                         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated print-at-commands help end ✂✂✂)
 
 Example output of `print-at-commands` call:
 
 ![print-at-commands](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-57.png "2023-04-28_08-57.png")
@@ -167,29 +178,31 @@
 
 ## read-register
 
 Help from `./cli.py read-register --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated read-register help start ✂✂✂)
 ```
-Usage: ./cli.py read-register [OPTIONS] IP REGISTER LENGTH
+Usage: ./cli.py read-register [OPTIONS] REGISTER LENGTH
 
  Read register(s) from the inverter
  e.g.: read 3 registers starting from 0x16:
  .../inverter-connect$ ./cli.py read-register 192.168.123.456 0x16 3
  e.g.: read the first 32 registers:
  .../inverter-connect$ ./cli.py read-register 192.168.123.456 0 32
  The start address can be pass as decimal number or as hex string, e.g.: 0x123
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                   │
-│                                                           [default: 48899; 1000<=x<=65535]       │
-│ --verbose/--no-verbose                                    [default: verbose]                     │
-│ --debug/--no-debug                                        [default: no-debug]                    │
-│ --help                                                    Show this message and exit.            │
+│ *  --ip             TEXT                     IP address of your inverter [required]              │
+│ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
+│                                              [required]                                          │
+│    --verbosity  -v  INTEGER RANGE [0<=x<=3]  Verbosity level; Accepts integer value e.g.:        │
+│                                              "--verbose 2" or can be count e.g.: "-vv"           │
+│                                              [default: 1; 0<=x<=3]                               │
+│    --help                                    Show this message and exit.                         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated read-register help end ✂✂✂)
 
 Example output of `read-register` call:
 
 ![read-register](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-53.png "2023-04-28_08-53.png")
@@ -212,14 +225,15 @@
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
 │ check-code-style            Check code style by calling darker + flake8                          │
 │ coverage                    Run and show coverage.                                               │
+│ create-default-settings     Create a default user settings file. (Used by CI pipeline ;)         │
 │ fix-code-style              Fix code style of all inverter source code files via darker          │
 │ install                     Run pip-sync and install 'inverter' via pip as editable.             │
 │ mypy                        Run Mypy (configured in pyproject.toml)                              │
 │ publish                     Build and upload this project to PyPi                                │
 │ safety                      Run safety check against current requirements files                  │
 │ test                        Run unittests                                                        │
 │ tox                         Run tox                                                              │
```

### Comparing `inverter-connect-0.6.1/README.md` & `inverter-connect-0.7.0rc1/inverter_connect.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: inverter-connect
+Version: 0.7.0rc1
+Summary: Get information from Deye Microinverter
+Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
+License: GPL-3.0-or-later
+Project-URL: Documentation, https://github.com/jedie/inverter-connect
+Project-URL: Source, https://github.com/jedie/inverter-connect
+Requires-Python: <4,>=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
 # inverter
 
 [![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/inverter-connect/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/inverter-connect)
 [![inverter-connect @ PyPi](https://img.shields.io/pypi/v/inverter-connect?label=inverter-connect%20%40%20PyPi)](https://pypi.org/project/inverter-connect/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/pyproject.toml)
 [![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/LICENSE)
@@ -9,14 +21,21 @@
 Get information from Deye Microinverter
 
 The whole thing is just a learning exercise for now. We will see.
 
 
 # quickstart
 
+## overview
+
+* clone the sources
+* Bootstrap and create default user settings by just call `./cli.py edit-settings`
+* Change the settings for your needs
+* ...use the commands... ;)
+
 Currently just clone the project and just start the cli (that will create a virtualenv and installs every dependencies)
 
 Note: Please enable https://www.piwheels.org/ if you are on a Raspberry Pi !
 
 e.g.:
 ```bash
 ~$ git clone https://github.com/jedie/inverter-connect.git
@@ -31,20 +50,20 @@
 Usage: ./cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
 │ debug-settings           Display (anonymized) MQTT server username and password                  │
+│ edit-settings            Edit the settings file. On first call: Create the default one.          │
 │ print-at-commands        Print one or more AT command values from Inverter.                      │
 │ print-values             Print all known register values from Inverter, e.g.:                    │
 │ publish-loop             Publish current data via MQTT for Home Assistant (endless loop)         │
 │ read-register            Read register(s) from the inverter                                      │
 │ set-time                 Set current date time in the inverter device.                           │
-│ store-settings           Store MQTT server settings.                                             │
 │ test-mqtt-connection     Test connection to MQTT Server                                          │
 │ version                  Print version and exit                                                  │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
@@ -53,61 +72,63 @@
 
 ## publish-loop
 
 Help from `./cli.py print-values --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated publish-loop help start ✂✂✂)
 ```
-Usage: ./cli.py publish-loop [OPTIONS] IP
+Usage: ./cli.py publish-loop [OPTIONS]
 
  Publish current data via MQTT for Home Assistant (endless loop)
  The "Daily Production" count will be cleared in the night, by set the current date time via
  AT-command.
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ *  --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                │
-│                                                              [default: 48899; 1000<=x<=65535]    │
-│                                                              [required]                          │
-│ *  --inverter                TEXT                            Prefix of yaml config files in      │
-│                                                              inverter/definitions/               │
-│                                                              [default: deye_2mppt]               │
-│                                                              [required]                          │
-│    --log/--no-log                                            [default: log]                      │
-│    --verbose/--no-verbose                                    [default: verbose]                  │
-│    --debug/--no-debug                                        [default: no-debug]                 │
-│    --help                                                    Show this message and exit.         │
+│ *  --ip             TEXT                     IP address of your inverter [required]              │
+│ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
+│                                              [required]                                          │
+│ *  --inverter       TEXT                     Prefix of yaml config files in                      │
+│                                              inverter/definitions/                               │
+│                                              [default: deye_2mppt]                               │
+│                                              [required]                                          │
+│    --verbosity  -v  INTEGER RANGE [0<=x<=3]  Verbosity level; Accepts integer value e.g.:        │
+│                                              "--verbose 2" or can be count e.g.: "-vv"           │
+│                                              [default: 1; 0<=x<=3]                               │
+│    --help                                    Show this message and exit.                         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated publish-loop help end ✂✂✂)
 
 
 ----
 
 
 ## print-values
 
 Help from `./cli.py print-values --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated print-values help start ✂✂✂)
 ```
-Usage: ./cli.py print-values [OPTIONS] IP
+Usage: ./cli.py print-values [OPTIONS]
 
  Print all known register values from Inverter, e.g.:
  .../inverter-connect$ ./cli.py print-values 192.168.123.456
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│    --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                │
-│                                                              [default: 48899; 1000<=x<=65535]    │
-│ *  --inverter                TEXT                            Prefix of yaml config files in      │
-│                                                              inverter/definitions/               │
-│                                                              [default: deye_2mppt]               │
-│                                                              [required]                          │
-│    --verbose/--no-verbose                                    [default: verbose]                  │
-│    --debug/--no-debug                                        [default: no-debug]                 │
-│    --help                                                    Show this message and exit.         │
+│ *  --ip             TEXT                     IP address of your inverter [required]              │
+│ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
+│                                              [required]                                          │
+│ *  --inverter       TEXT                     Prefix of yaml config files in                      │
+│                                              inverter/definitions/                               │
+│                                              [default: deye_2mppt]                               │
+│                                              [required]                                          │
+│    --verbosity  -v  INTEGER RANGE [0<=x<=3]  Verbosity level; Accepts integer value e.g.:        │
+│                                              "--verbose 2" or can be count e.g.: "-vv"           │
+│                                              [default: 1; 0<=x<=3]                               │
+│    --help                                    Show this message and exit.                         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated print-values help end ✂✂✂)
 
 Example output of `print-values` call:
 
 ![print-values](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-55.png "2023-04-28_08-55.png")
@@ -117,15 +138,15 @@
 
 ## print-at-commands
 
 Help from `./cli.py print-at-commands --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated print-at-commands help start ✂✂✂)
 ```
-Usage: ./cli.py print-at-commands [OPTIONS] IP [COMMANDS]...
+Usage: ./cli.py print-at-commands [OPTIONS] [COMMANDS]...
 
  Print one or more AT command values from Inverter.
  Use all known AT commands, if no one is given, e.g.:
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456
  Or specify one or more AT-commands, e.g.:
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 WEBVER .../inverter-connect$
  ./cli.py print-at-commands 192.168.123.456 WEBVER WEBU
@@ -133,19 +154,21 @@
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPSER=192.168.1.1 NTPEN=on
  NTPSER NTPEN
  wait a while and request the current date time:
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPTM
  (Note: The prefix "AT+" will be added to every command)
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                   │
-│                                                           [default: 48899; 1000<=x<=65535]       │
-│ --verbose/--no-verbose                                    [default: verbose]                     │
-│ --debug/--no-debug                                        [default: no-debug]                    │
-│ --help                                                    Show this message and exit.            │
+│ *  --ip             TEXT                     IP address of your inverter [required]              │
+│ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
+│                                              [required]                                          │
+│    --verbosity  -v  INTEGER RANGE [0<=x<=3]  Verbosity level; Accepts integer value e.g.:        │
+│                                              "--verbose 2" or can be count e.g.: "-vv"           │
+│                                              [default: 1; 0<=x<=3]                               │
+│    --help                                    Show this message and exit.                         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated print-at-commands help end ✂✂✂)
 
 Example output of `print-at-commands` call:
 
 ![print-at-commands](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-57.png "2023-04-28_08-57.png")
@@ -155,29 +178,31 @@
 
 ## read-register
 
 Help from `./cli.py read-register --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated read-register help start ✂✂✂)
 ```
-Usage: ./cli.py read-register [OPTIONS] IP REGISTER LENGTH
+Usage: ./cli.py read-register [OPTIONS] REGISTER LENGTH
 
  Read register(s) from the inverter
  e.g.: read 3 registers starting from 0x16:
  .../inverter-connect$ ./cli.py read-register 192.168.123.456 0x16 3
  e.g.: read the first 32 registers:
  .../inverter-connect$ ./cli.py read-register 192.168.123.456 0 32
  The start address can be pass as decimal number or as hex string, e.g.: 0x123
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                   │
-│                                                           [default: 48899; 1000<=x<=65535]       │
-│ --verbose/--no-verbose                                    [default: verbose]                     │
-│ --debug/--no-debug                                        [default: no-debug]                    │
-│ --help                                                    Show this message and exit.            │
+│ *  --ip             TEXT                     IP address of your inverter [required]              │
+│ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
+│                                              [required]                                          │
+│    --verbosity  -v  INTEGER RANGE [0<=x<=3]  Verbosity level; Accepts integer value e.g.:        │
+│                                              "--verbose 2" or can be count e.g.: "-vv"           │
+│                                              [default: 1; 0<=x<=3]                               │
+│    --help                                    Show this message and exit.                         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated read-register help end ✂✂✂)
 
 Example output of `read-register` call:
 
 ![read-register](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-53.png "2023-04-28_08-53.png")
@@ -200,14 +225,15 @@
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
 │ check-code-style            Check code style by calling darker + flake8                          │
 │ coverage                    Run and show coverage.                                               │
+│ create-default-settings     Create a default user settings file. (Used by CI pipeline ;)         │
 │ fix-code-style              Fix code style of all inverter source code files via darker          │
 │ install                     Run pip-sync and install 'inverter' via pip as editable.             │
 │ mypy                        Run Mypy (configured in pyproject.toml)                              │
 │ publish                     Build and upload this project to PyPi                                │
 │ safety                      Run safety check against current requirements files                  │
 │ test                        Run unittests                                                        │
 │ tox                         Run tox                                                              │
```

### Comparing `inverter-connect-0.6.1/cli.py` & `inverter-connect-0.7.0rc1/cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.1/dev-cli.py` & `inverter-connect-0.7.0rc1/dev-cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.1/inverter/.github/workflows/tests.yml` & `inverter-connect-0.7.0rc1/inverter/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.1/inverter/api.py` & `inverter-connect-0.7.0rc1/inverter/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                 name=name,
                 value=result.parsed_value,
                 device_class=parameter.device_class,
                 state_class=parameter.state_class,
                 unit=parameter.unit,
                 result=result,
             )
-            if self.config.debug:
+            if self.config.verbosity > 1:
                 pprint(value, indent_guides=False)
 
             try:
                 self.value_validator(inverter_value=value)
             except ValidationError as err:
                 logger.info(f'Validation error: {err}')
                 raise
```

### Comparing `inverter-connect-0.6.1/inverter/cli/cli_app.py` & `inverter-connect-0.7.0rc1/inverter/cli/cli_app.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     CLI for usage
 """
-import getpass
+
 import logging
 import sys
 import time
 from pathlib import Path
 
 import rich_click as click
 from bx_py_utils.path import assert_is_file
+from ha_services.mqtt4homeassistant.mqtt import get_connected_client
+from ha_services.toml_settings.api import debug_print_user_settings, edit_user_settings, get_user_settings
+from ha_services.toml_settings.exceptions import UserSettingsNotFound
 from rich import print  # noqa
-from rich.pretty import pprint
 from rich_click import RichGroup
 
 import inverter
 from inverter import constants
 from inverter.api import Inverter, set_current_time
 from inverter.connection import InverterSock
-from inverter.constants import ERROR_STR_NO_DATA
-from inverter.data_types import Config, Parameter, ValueType
+from inverter.constants import ERROR_STR_NO_DATA, USER_SETTINGS_PATH
+from inverter.data_types import Parameter, ValueType
 from inverter.exceptions import ReadInverterError
-from inverter.mqtt4homeassistant.data_classes import MqttSettings
-from inverter.mqtt4homeassistant.mqtt import get_connected_client
 from inverter.publish_loop import publish_forever
+from inverter.user_settings import UserSettings, make_config, migrate_old_settings
 from inverter.utilities.cli import convert_address_option, print_register
-from inverter.utilities.credentials import get_mqtt_settings, store_mqtt_settings
-from inverter.utilities.log_setup import basic_log_setup
+from inverter.verbosity import OPTION_KWARGS_VERBOSE, setup_logging
 
 
 logger = logging.getLogger(__name__)
 
 
 PACKAGE_ROOT = Path(inverter.__file__).parent.parent
 assert_is_file(PACKAGE_ROOT / 'pyproject.toml')
@@ -49,22 +49,14 @@
         path_type=Path,
     )
 )
 ARGUMENT_EXISTING_FILE = dict(
     type=click.Path(exists=True, file_okay=True, dir_okay=False, readable=True, path_type=Path)
 )
 
-INVERTER_NAME = dict(
-    required=True,
-    type=str,
-    default='deye_2mppt',
-    help='Prefix of yaml config files in inverter/definitions/',
-    show_default=True,
-)
-
 
 class ClickGroup(RichGroup):  # FIXME: How to set the "info_name" easier?
     def make_context(self, info_name, *args, **kwargs):
         info_name = './cli.py'
         return super().make_context(info_name, *args, **kwargs)
 
 
@@ -72,41 +64,123 @@
     cls=ClickGroup,
     epilog=constants.CLI_EPILOG,
 )
 def cli():
     pass
 
 
+######################################################################################################
+
+
 @click.command()
 def version():
     """Print version and exit"""
     # Pseudo command, because the version always printed on every CLI call ;)
     sys.exit(0)
 
 
 cli.add_command(version)
 
 
-@click.command()
-@click.argument('ip')
-@click.option(
-    '--port', type=click.IntRange(1000, 65535), default=48899, help='Port of the inverter', show_default=True
+######################################################################################################
+# User settings
+
+
+migrate_old_settings()  # TODO: Remove in the Future
+
+try:
+    user_settings: UserSettings = get_user_settings(user_settings=UserSettings(), settings_path=USER_SETTINGS_PATH)
+except UserSettingsNotFound:
+    print(f'[red]No settings file found: [yellow]{USER_SETTINGS_PATH}')
+    input('Press any key, to create it')
+    edit_user_settings(user_settings=UserSettings(), settings_path=USER_SETTINGS_PATH)
+    sys.exit(1)
+
+
+option_kwargs_ip = dict(
+    required=True,
+    type=str,
+    help='IP address of your inverter',
+    default=user_settings.inverter.ip or None,  # Don't accept empty string as IP: We need a address ;)
+    show_default=True,
+)
+option_kwargs_port = dict(
+    required=True,
+    type=int,
+    default=user_settings.inverter.port,
+    help='Port of inverter services',
+    show_default=True,
+)
+option_kwargs_inverter_name = dict(
+    required=True,
+    type=str,
+    default=user_settings.inverter.name,
+    help='Prefix of yaml config files in inverter/definitions/',
+    show_default=True,
 )
-@click.option('--inverter', **INVERTER_NAME)
-@click.option('--verbose/--no-verbose', **OPTION_ARGS_DEFAULT_TRUE)
-@click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_FALSE)
-def print_values(ip, port, inverter, verbose, debug):
+
+
+@click.command()
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def edit_settings(verbosity: int):
+    """
+    Edit the settings file. On first call: Create the default one.
+    """
+    setup_logging(verbosity=verbosity)
+    edit_user_settings(user_settings=UserSettings(), settings_path=USER_SETTINGS_PATH)
+
+
+cli.add_command(edit_settings)
+
+
+@click.command()
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def debug_settings(verbosity: int):
+    """
+    Display (anonymized) MQTT server username and password
+    """
+    setup_logging(verbosity=verbosity)
+    try:
+        debug_print_user_settings(user_settings=UserSettings(), settings_path=USER_SETTINGS_PATH)
+    except UserSettingsNotFound as err:
+        print(f'[yellow]No settings created yet[/yellow]: {err} [green](Hint: call "edit-settings" first!)')
+
+
+cli.add_command(debug_settings)
+
+
+######################################################################################################
+
+
+@click.command()
+@click.option('--ip', **option_kwargs_ip)
+@click.option('--port', **option_kwargs_port)
+@click.option('--inverter', **option_kwargs_inverter_name)
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def print_values(ip, port, inverter, verbosity: int):
     """
     Print all known register values from Inverter, e.g.:
 
     .../inverter-connect$ ./cli.py print-values 192.168.123.456
     """
-    basic_log_setup(debug=debug)
-
-    config = Config(inverter_name=inverter, host=ip, port=port, verbose=verbose, debug=debug)
+    if user_settings is None:
+        print('[yellow]No settings created yet! [green]Call "edit-settings" first!')
+        return
+
+    setup_logging(verbosity=verbosity)
+
+    print()
+
+    config = make_config(
+        user_settings=user_settings,
+        verbosity=verbosity,
+        ip=ip,
+        port=port,
+        inverter=inverter,
+    )
 
     with Inverter(config=config) as inverter:
         try:
             inverter.connect()
         except ReadInverterError as err:
             print(f'[red]{err}')
             sys.exit(1)
@@ -126,30 +200,27 @@
                 print(
                     f'(Register: [cyan]{parameter.start_register:04X}[/cyan], length:'
                     f' [blue]{parameter.length}[/blue])'
                 )
             elif value.type == ValueType.COMPUTED:
                 print('(Computed)')
 
-            if debug:
+            if verbosity:
                 print()
 
 
 cli.add_command(print_values)
 
 
 @click.command()
-@click.argument('ip')
 @click.argument('commands', nargs=-1)
-@click.option(
-    '--port', type=click.IntRange(1000, 65535), default=48899, help='Port of the inverter', show_default=True
-)
-@click.option('--verbose/--no-verbose', **OPTION_ARGS_DEFAULT_TRUE)
-@click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_FALSE)
-def print_at_commands(ip, port, commands, verbose, debug):
+@click.option('--ip', **option_kwargs_ip)
+@click.option('--port', **option_kwargs_port)
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def print_at_commands(ip, port, commands, verbosity: int):
     """
     Print one or more AT command values from Inverter.
 
     Use all known AT commands, if no one is given, e.g.:
 
     .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456
 
@@ -164,15 +235,19 @@
 
     wait a while and request the current date time:
 
     .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPTM
 
     (Note: The prefix "AT+" will be added to every command)
     """
-    basic_log_setup(debug=debug)
+    if user_settings is None:
+        print('[yellow]No settings created yet! [green]Call "edit-settings" first!')
+        return
+
+    setup_logging(verbosity=verbosity)
 
     if not commands:
         commands = (
             # 'KEY',  # Set/Get Device Password
             'VER',
             'BVER',  # bootloader version
             'HWVER',  # hardware version
@@ -211,15 +286,21 @@
             'NTPRF',  # NTP request interval in min (?)
             'NTPEN',  # Enable/Disable NTP Server
             'WSDNS',  # Set/Get the DNS Server address
             'DEVICENUM',  # Set/Get Device Link Num
             'DEVSELCTL',  # Set/Get Web Device List Info
         )
 
-    config = Config(inverter_name=None, host=ip, port=port, verbose=verbose, debug=debug)
+    config = make_config(
+        user_settings=user_settings,
+        verbosity=verbosity,
+        ip=ip,
+        port=port,
+        inverter=None,
+    )
 
     with InverterSock(config) as inv_sock:
         try:
             inv_sock.connect()
         except ReadInverterError as err:
             print(f'[red]{err}')
             sys.exit(1)
@@ -230,33 +311,42 @@
             print(f'[green]{result}')
 
 
 cli.add_command(print_at_commands)
 
 
 @click.command()
-@click.argument('ip')
-@click.option(
-    '--port', type=click.IntRange(1000, 65535), default=48899, help='Port of the inverter', show_default=True
-)
+@click.option('--ip', **option_kwargs_ip)
+@click.option('--port', **option_kwargs_port)
 @click.option('--register', default="0x16", help='Start address', show_default=True)
-@click.option('--verbose/--no-verbose', **OPTION_ARGS_DEFAULT_TRUE)
-@click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_TRUE)
-def set_time(ip, port, register, verbose, debug):
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def set_time(ip, port, register, verbosity: int):
     """
     Set current date time in the inverter device.
 
     Default start address is 0x16, so that this will be filled:
         0x16 - year + month
         0x17 - day + hour
         0x18 - minute + second
     """
-    address = convert_address_option(raw_address=register, debug=debug)
-
-    config = Config(inverter_name=None, host=ip, port=port, verbose=verbose, debug=debug)
+    if user_settings is None:
+        print('[yellow]No settings created yet! [green]Call "edit-settings" first!')
+        return
+
+    setup_logging(verbosity=verbosity)
+
+    address = convert_address_option(raw_address=register, debug=bool(verbosity))
+
+    config = make_config(
+        user_settings=user_settings,
+        verbosity=verbosity,
+        ip=ip,
+        port=port,
+        inverter=None,
+    )
 
     with InverterSock(config) as inv_sock:
         try:
             inv_sock.connect()
         except ReadInverterError as err:
             print(f'[red]{err}')
             sys.exit(1)
@@ -273,40 +363,49 @@
         print(f'[green]{result}')
 
 
 cli.add_command(set_time)
 
 
 @click.command()
-@click.argument('ip')
-@click.option(
-    '--port', type=click.IntRange(1000, 65535), default=48899, help='Port of the inverter', show_default=True
-)
+@click.option('--ip', **option_kwargs_ip)
+@click.option('--port', **option_kwargs_port)
 @click.argument('register')
 @click.argument('length', type=click.IntRange(1, 100))
-@click.option('--verbose/--no-verbose', **OPTION_ARGS_DEFAULT_TRUE)
-@click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_FALSE)
-def read_register(ip, port, register, length, verbose, debug):
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def read_register(ip, port, register, length, verbosity: int):
     """
     Read register(s) from the inverter
 
     e.g.: read 3 registers starting from 0x16:
 
         .../inverter-connect$ ./cli.py read-register 192.168.123.456 0x16 3
 
     e.g.: read the first 32 registers:
 
     .../inverter-connect$ ./cli.py read-register 192.168.123.456 0 32
 
     The start address can be pass as decimal number or as hex string, e.g.: 0x123
     """
+    if user_settings is None:
+        print('[yellow]No settings created yet! [green]Call "edit-settings" first!')
+        return
+
+    setup_logging(verbosity=verbosity)
+
     print(f'Read {length} register(s) from {register=!r} ({ip}:{port})')
-    address = convert_address_option(raw_address=register, debug=debug)
+    address = convert_address_option(raw_address=register, debug=bool(verbosity))
 
-    config = Config(inverter_name=None, host=ip, port=port, verbose=verbose, debug=debug)
+    config = make_config(
+        user_settings=user_settings,
+        verbosity=verbosity,
+        ip=ip,
+        port=port,
+        inverter=None,
+    )
 
     with InverterSock(config) as inv_sock:
         try:
             inv_sock.connect()
         except ReadInverterError as err:
             print(f'[red]{err}')
             sys.exit(1)
@@ -318,116 +417,62 @@
 
 
 ######################################################################################################
 # MQTT
 
 
 @click.command()
-@click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_FALSE)
-def store_settings(debug):
-    """
-    Store MQTT server settings.
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def test_mqtt_connection(verbosity: int):
     """
-    basic_log_setup(debug=debug)
-
-    try:
-        settings: MqttSettings = get_mqtt_settings()
-    except FileNotFoundError:
-        print('No settings stored, yet. ok.')
-        print()
-        print('Input settings:')
-    else:
-        print('Current settings:')
-        pprint(settings.anonymized())
-        print()
-        print('Input new settings:')
-
-    host = input('host (e.g.: "test.mosquitto.org"): ')
-    if not host:
-        print('Host is needed! Abort.')
-        sys.exit(1)
-
-    port = input('port (default: 1883): ')
-    if port:
-        port = int(port)
-    else:
-        port = 1883
-    user_name = input('user name: ')
-    password = getpass.getpass('password: ')
-
-    settings = MqttSettings(host=host, port=port, user_name=user_name, password=password)
-    file_path = store_mqtt_settings(settings)
-    print(f'MQTT server settings stored into: {file_path}')
-
-
-cli.add_command(store_settings)
-
-
-@click.command()
-@click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_FALSE)
-def debug_settings(debug):
-    """
-    Display (anonymized) MQTT server username and password
+    Test connection to MQTT Server
     """
-    basic_log_setup(debug=debug)
-    settings: MqttSettings = get_mqtt_settings()
-    pprint(settings.anonymized())
-
-
-cli.add_command(debug_settings)
+    if user_settings is None:
+        print('[yellow]No settings created yet! [green]Call "edit-settings" first!')
+        return
 
+    setup_logging(verbosity=verbosity)
 
-@click.command()
-@click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_FALSE)
-def test_mqtt_connection(debug):
-    """
-    Test connection to MQTT Server
-    """
-    basic_log_setup(debug=debug)
-    settings: MqttSettings = get_mqtt_settings()
-    mqttc = get_connected_client(settings=settings, verbose=True)
+    mqttc = get_connected_client(settings=user_settings.mqtt, verbose=True)
     mqttc.loop_start()
     mqttc.loop_stop()
     mqttc.disconnect()
     print('\n[green]Test succeed[/green], bye ;)')
 
 
 cli.add_command(test_mqtt_connection)
 
 
 @click.command()
-@click.argument('ip')
-@click.option(
-    '--port',
-    type=click.IntRange(1000, 65535),
-    default=48899,
-    help='Port of the inverter',
-    show_default=True,
-    required=True,
-)
-@click.option('--inverter', **INVERTER_NAME)
-@click.option('--log/--no-log', **OPTION_ARGS_DEFAULT_TRUE)
-@click.option('--verbose/--no-verbose', **OPTION_ARGS_DEFAULT_TRUE)
-@click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_FALSE)
-def publish_loop(ip, port, inverter, log, verbose, debug):
+@click.option('--ip', **option_kwargs_ip)
+@click.option('--port', **option_kwargs_port)
+@click.option('--inverter', **option_kwargs_inverter_name)
+@click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
+def publish_loop(ip, port, inverter, verbosity: int):
     """
     Publish current data via MQTT for Home Assistant (endless loop)
 
     The "Daily Production" count will be cleared in the night,
     by set the current date time via AT-command.
     """
-    if log:
-        basic_log_setup(debug=debug)
-
-    config = Config(inverter_name=inverter, host=ip, port=port, verbose=verbose, debug=debug)
-
-    mqtt_settings: MqttSettings = get_mqtt_settings()
-    pprint(mqtt_settings.anonymized())
+    if user_settings is None:
+        print('[yellow]No settings created yet! [green]Call "edit-settings" first!')
+        return
+
+    setup_logging(verbosity=verbosity)
+
+    config = make_config(
+        user_settings=user_settings,
+        verbosity=verbosity,
+        ip=ip,
+        port=port,
+        inverter=inverter,
+    )
     try:
-        publish_forever(mqtt_settings=mqtt_settings, config=config, verbose=verbose)
+        publish_forever(config=config, verbosity=verbosity)
     except KeyboardInterrupt:
         print('Bye, bye')
 
 
 cli.add_command(publish_loop)
```

### Comparing `inverter-connect-0.6.1/inverter/cli/dev.py` & `inverter-connect-0.7.0rc1/inverter/cli/dev.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,24 +2,29 @@
     CLI for development
 """
 import logging
 import sys
 from pathlib import Path
 
 import rich_click as click
+import tomlkit
 from bx_py_utils.path import assert_is_file
+from ha_services.toml_settings.serialize import dataclass2toml
 from manageprojects.utilities import code_style
 from manageprojects.utilities.publish import publish_package
 from manageprojects.utilities.subprocess_utils import verbose_check_call
 from manageprojects.utilities.version_info import print_version
 from rich import print  # noqa; noqa
 from rich_click import RichGroup
+from tomlkit import TOMLDocument
 
 import inverter
 from inverter import constants
+from inverter.constants import USER_SETTINGS_PATH
+from inverter.user_settings import UserSettings
 
 
 logger = logging.getLogger(__name__)
 
 
 PACKAGE_ROOT = Path(inverter.__file__).parent.parent
 assert_is_file(PACKAGE_ROOT / 'pyproject.toml')
@@ -298,14 +303,37 @@
     # Pseudo command, because the version always printed on every CLI call ;)
     sys.exit(0)
 
 
 cli.add_command(version)
 
 
+######################################################################################################
+@click.command()
+def create_default_settings():
+    """
+    Create a default user settings file. (Used by CI pipeline ;)
+    """
+    settings_path = Path(USER_SETTINGS_PATH).expanduser()
+    if settings_path.is_file():
+        print(f'[green]Use settings file already exists here: {settings_path}')
+        return
+
+    document: TOMLDocument = dataclass2toml(instance=UserSettings())
+    doc_str = tomlkit.dumps(document, sort_keys=False)
+
+    settings_path.write_text(doc_str, encoding='UTF-8')
+    print(f'[green]Default settings file created here: {settings_path}')
+
+
+cli.add_command(create_default_settings)
+
+######################################################################################################
+
+
 def main():
     print_version(inverter)
 
     if len(sys.argv) >= 2:
         # Check if we just pass a command call
         command = sys.argv[1]
         if command == 'test':
```

### Comparing `inverter-connect-0.6.1/inverter/connection.py` & `inverter-connect-0.7.0rc1/inverter/connection.py`

 * *Files 9% similar despite different names*

```diff
@@ -197,39 +197,39 @@
         self.sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
         self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self.sock.settimeout(self.config.timeout)
 
         self.init_inventer()
 
     def send(self, *, command: bytes):
-        if self.config.debug:
+        if self.config.verbosity > 1:
             print(f'send: {command}', end='...', flush=True)
 
         try:
             self.sock.sendto(command, (self.config.host, self.config.port))
         except socket.gaierror as err:
             raise ReadInverterError(f'{err} (Hint: Check {self.config.host}:{self.config.port})')
 
-        if self.config.debug:
+        if self.config.verbosity > 1:
             print('OK', flush=True)
 
         time.sleep(self.config.pause)
 
     def recv_command(self, *, command: bytes, buffer_size=1024):
         self.send(command=command)
 
-        if self.config.debug:
+        if self.config.verbosity > 1:
             print('recv', end='...', flush=True)
 
         try:
             data = self.sock.recv(buffer_size)
         except (TimeoutError, socket.timeout) as err:
             raise ReadTimeout(f'Get no response from {self.config.host}: {err}')
         else:
-            if self.config.debug:
+            if self.config.verbosity > 1:
                 print(f'{data}', flush=True)
 
             return data
 
     def at_command(self, command: str, buffer_size=1024):
         assert not command.startswith('AT+'), f'Remove "AT+" prefix from: {command=}'
         assert not command.endswith('\n'), f'Line ending found in: {command=}'
@@ -263,34 +263,34 @@
             return False
 
         print('\nSigning off with "AT+Q"', end='...')
         self.send(command=b'AT+Q\n')
         print('Goodbye ;)\n')
 
     def read(self, *, start_register: int, length: int) -> ModbusResponse:
-        if self.config.debug:
+        if self.config.verbosity > 1:
             print(f'Read {length} value(s) from start register: {hex(start_register)}')
 
         command = parameter2modbus_at_command(
             start_register=start_register,
             length=length,
             modbus_function=AT_READ_FUNC_NUMBER,
         )
-        if self.config.debug:
+        if self.config.verbosity > 1:
             print(f'AT command: {command}')
 
         data: str = self.cleaned_at_command(command=command)
         try:
             response: ModbusResponse = parse_modbus_response(data=data)
         except ParseModbusValueError as err:
             raise ParseModbusValueError(f'parse error: {data=}: {err}')
         return response
 
     def read_paremeter(self, *, parameter: Parameter) -> ModbusReadResult:
-        if self.config.debug:
+        if self.config.verbosity > 1:
             print(parameter)
 
         try:
             response: ModbusResponse = self.read(
                 start_register=parameter.start_register,
                 length=parameter.length,
             )
@@ -298,21 +298,21 @@
             # Modbus register value is: b'no data'
             result = ModbusReadResult(parameter=parameter, parsed_value='no data')
         else:
             result: ModbusReadResult = make_modbus_result(response=response, parameter=parameter)
         return result
 
     def write(self, *, address: int, values: list[int, ...]):
-        if self.config.debug:
+        if self.config.verbosity > 1:
             print(f'Write {" ".join(hex(value) for value in values)} to {hex(address)}')
 
         command = parameter2modbus_at_command(
             start_register=address,
             length=len(values),
             modbus_function=AT_WRITE_FUNC_NUMBER,
             values=values,
         )
-        if self.config.debug:
+        if self.config.verbosity > 1:
             print(f'AT command: {command}')
 
         data: str = self.cleaned_at_command(command=command)
         return data
```

### Comparing `inverter-connect-0.6.1/inverter/daily_reset.py` & `inverter-connect-0.7.0rc1/inverter/daily_reset.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.1/inverter/data_types.py` & `inverter-connect-0.7.0rc1/inverter/data_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from __future__ import annotations
 
 import dataclasses
+import logging
 from datetime import datetime, time
 from enum import Enum
 from pathlib import Path
 from typing import Callable
 
 import msgspec
+from ha_services.mqtt4homeassistant.data_classes import MqttSettings
 from rich import print
 
 from inverter.constants import BASE_PATH, TYPE_MAP
 
 
+logger = logging.getLogger(__name__)
+
+
 class ValueType(Enum):
     READ_OUT = 'read out'
     COMPUTED = 'computed'
 
 
 @dataclasses.dataclass
 class InverterValue:
@@ -53,25 +58,25 @@
     parameter: Parameter
     parsed_value: float | str
     response: ModbusResponse = None
 
 
 @dataclasses.dataclass
 class Config:
-    inverter_name: str | None
+    verbosity: int
+    host: str
+    port: int
+    mqtt_settings: MqttSettings
 
-    host: str | None = None
-    port: int = 48899
+    inverter_name: str | None
 
     pause: float = 0.1
     timeout: int = 5
 
     init_cmd: bytes = b'WIFIKIT-214028-READ'
-    verbose: bool = True
-    debug: bool = False
 
     daily_production_name: str = 'Daily Production'  # Must be the same as in yaml config!
     reset_needed_start: time = time(hour=1)
     reset_needed_end: time = time(hour=3)
 
     # Will be set by post init:
     definition_file_path: Path = None
@@ -87,15 +92,15 @@
 
             self.validation_file_path = BASE_PATH / 'definitions' / f'{self.inverter_name}_validations.yaml'
             if not self.validation_file_path.is_file():
                 raise FileNotFoundError(
                     f'Wrong inverter name: {self.inverter_name!r}: File not found: {self.validation_file_path}'
                 )
 
-        if self.verbose or self.debug:
+        if self.verbosity > 1:
             print(self)
 
 
 @dataclasses.dataclass
 class ResetState:
     started: datetime
     set_time_count: int = 0
```

### Comparing `inverter-connect-0.6.1/inverter/definitions/deye_2mppt.yaml` & `inverter-connect-0.7.0rc1/inverter/definitions/deye_2mppt.yaml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.1/inverter/definitions.py` & `inverter-connect-0.7.0rc1/inverter/definitions.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.1/inverter/exceptions.py` & `inverter-connect-0.7.0rc1/inverter/exceptions.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.1/inverter/publish_loop.py` & `inverter-connect-0.7.0rc1/inverter/publish_loop.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import logging
 import time
 from datetime import datetime
 
+from ha_services.mqtt4homeassistant.converter import values2mqtt_payload
+from ha_services.mqtt4homeassistant.data_classes import HaValue, HaValues
+from ha_services.mqtt4homeassistant.mqtt import HaMqttPublisher
 from rich import print  # noqa
 
 from inverter.api import Inverter
 from inverter.constants import ERROR_STR_NO_DATA
 from inverter.daily_reset import DailyProductionReset
 from inverter.data_types import Config, InverterInfo, InverterValue, ResetState
 from inverter.exceptions import ReadInverterError, ReadTimeout, ValidationError
-from inverter.mqtt4homeassistant.converter import values2mqtt_payload
-from inverter.mqtt4homeassistant.data_classes import HaValue, HaValues, MqttSettings
-from inverter.mqtt4homeassistant.mqtt import HaMqttPublisher
+from inverter.utilities.cli import exit_with_human_error
 
 
 logger = logging.getLogger(__name__)
 
 
-def publish_forever(*, mqtt_settings: MqttSettings, config: Config, verbose):
-    publisher = HaMqttPublisher(settings=mqtt_settings, verbose=verbose, config_count=1)
+def publish_forever(*, config: Config, verbosity):
+    mqtt_settings = config.mqtt_settings
+    try:
+        publisher = HaMqttPublisher(settings=mqtt_settings, verbose=bool(verbosity), config_count=1)
+    except Exception as err:
+        exit_with_human_error(hint=f'given {mqtt_settings!r} is wrong?!?', print_traceback=err)
 
     reset_state = ResetState(started=datetime.now())
 
     while True:
         try:
             with Inverter(config=config) as inverter:
                 inverter.connect()
```

### Comparing `inverter-connect-0.6.1/inverter/tests/test_api.py` & `inverter-connect-0.7.0rc1/inverter/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.1/inverter/tests/test_cli.py` & `inverter-connect-0.7.0rc1/inverter/tests/test_cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,29 +7,37 @@
 
 class CliTestCase(BaseTestCase):
     def test_print_at_commands_invalid_ip(self):
         with self.assertRaises(ClickInvokeCliException) as cm:
             invoke_click(
                 cli,
                 'print-at-commands',
+                '--ip',
                 '123.456.789.666',  # <<< not a valid IPv4 -> socket.gaierror will be raised
             )
 
         result: Result = cm.exception.result
         self.assert_in_content(
             got=result.stdout,
-            parts=('[Errno -2]', '(Hint: Check 123.456.789.666:48899)'),
+            parts=(
+                'gaierror: [Errno -2]',
+                "Is the given ip='123.456.789.666' is wrong?!?",
+            ),
         )
 
     def test_print_values_invalid_ip(self):
         with self.assertRaises(ClickInvokeCliException) as cm:
             invoke_click(
                 cli,
                 'print-values',
+                '--ip',
                 '123.456.789.666',  # <<< not a valid IPv4 -> socket.gaierror will be raised
             )
 
         result: Result = cm.exception.result
         self.assert_in_content(
             got=result.stdout,
-            parts=('[Errno -2]', '(Hint: Check 123.456.789.666:48899)'),
+            parts=(
+                'gaierror: [Errno -2]',
+                "Is the given ip='123.456.789.666' is wrong?!?",
+            ),
         )
```

### Comparing `inverter-connect-0.6.1/inverter/tests/test_connect.py` & `inverter-connect-0.7.0rc1/inverter/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.1/inverter/tests/test_daily_reset.py` & `inverter-connect-0.7.0rc1/inverter/tests/test_daily_reset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 from datetime import datetime, timedelta
 from unittest import TestCase
 
 from freezegun import freeze_time
 
 from inverter.daily_reset import DailyProductionReset
-from inverter.data_types import Config, InverterValue, ResetState, ValueType
+from inverter.data_types import InverterValue, ResetState, ValueType
+from inverter.tests import fixtures
 
 
 class DailyProductionResetTestCase(TestCase):
     @freeze_time('2020-01-01T00:00:00+0000', as_kwarg='frozen_time')
     def test_happy_path(self, frozen_time):
         start_dt = datetime.now()
 
@@ -22,15 +23,15 @@
             def __init__(self):
                 self.inv_sock = self
 
             def write(self, *, address, values):
                 self.writes.append((address, values))
 
         inverter = InverterMock()
-        config = Config(inverter_name=None, verbose=False)
+        config = fixtures.get_config()
 
         with DailyProductionReset(reset_state, inverter, config) as daily_production_reset:
             self.assertEqual(
                 daily_production_reset.reset_state,
                 ResetState(started=start_dt, set_time_count=0, successful_count=0, reset_needed=False),
             )
```

### Comparing `inverter-connect-0.6.1/inverter/tests/test_definitions.py` & `inverter-connect-0.7.0rc1/inverter/tests/test_definitions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from unittest import TestCase
 
-from inverter.data_types import Config, Parameter
+from inverter.data_types import Parameter
 from inverter.definitions import get_definition, get_parameter
+from inverter.tests import fixtures
 from inverter.utilities.modbus_converter import parse_number
 
 
 class DefinitionsTestCase(TestCase):
     def test_get_definition(self):
-        config = Config(inverter_name='deye_2mppt', verbose=False)
+        config = fixtures.get_config()
+
         result = get_definition(config=config)
         self.assertIsInstance(result, list)
         example = result[0]['items'][0]
         self.assertEqual(
             example,
             {
                 'class': 'voltage',
@@ -22,15 +24,16 @@
                 'scale': 0.1,
                 'state_class': 'measurement',
                 'uom': 'V',
             },
         )
 
     def test_get_parameter(self):
-        config = Config(inverter_name='deye_2mppt', verbose=False)
+        config = fixtures.get_config()
+
         parameters = get_parameter(config=config)
         self.assertIsInstance(parameters, list)
         example = parameters[0]
         self.assertEqual(
             example,
             Parameter(
                 start_register=109,
```

### Comparing `inverter-connect-0.6.1/inverter/tests/test_project_setup.py` & `inverter-connect-0.7.0rc1/inverter/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.1/inverter/tests/test_validators.py` & `inverter-connect-0.7.0rc1/inverter/tests/test_validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 from unittest import TestCase
 
-from inverter.data_types import Config, InverterValue, ValueType
+from inverter.data_types import InverterValue, ValueType
 from inverter.exceptions import ValidationError
+from inverter.tests import fixtures
 from inverter.validators import InverterValueValidator
 
 
 class ValidatorsTestCase(TestCase):
     def test_happy_path(self):
-        config = Config(inverter_name='deye_2mppt', verbose=False)
+        config = fixtures.get_config()
         validator = InverterValueValidator(config=config)
 
         with self.assertLogs(logger=None, level=logging.DEBUG) as logs:
             validator(
                 inverter_value=InverterValue(
                     type=ValueType.COMPUTED,
                     name='Total Power',
```

### Comparing `inverter-connect-0.6.1/inverter/utilities/cli.py` & `inverter-connect-0.7.0rc1/inverter/utilities/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,16 @@
+from __future__ import annotations
+
+import sys
+
 from bx_py_utils.iteration import chunk_iterable
 from rich import print  # noqa
 from rich.console import Console
+from rich.highlighter import ReprHighlighter
+from rich.panel import Panel
 from rich.table import Table
 
 from inverter.data_types import ModbusResponse
 from inverter.exceptions import ModbusNoData, ModbusNoHexData
 
 
 def convert_address_option(raw_address: str, debug: bool = True) -> int:
@@ -61,7 +67,47 @@
         print(f'\nResult (in hex): [cyan]{response.data_hex}\n')
 
         print_hex_table(
             address=start_register,
             data_hex=response.data_hex,
             title=f'[green][bold]{length} value(s) from {hex(start_register)}',
         )
+
+
+def exit_with_human_error(
+    *,
+    hint: str,
+    title='Hint',
+    exit_code=-1,
+    print_traceback: BaseException | None = None,
+    HintHighlighterClass=ReprHighlighter,
+    hint_border_style='bright_yellow',
+    hint_padding=(2, 5),
+):
+    """
+    TODO: Move to a shared package!
+    """
+    console = Console()
+    console.print('\n')
+
+    if print_traceback is not None:
+        assert isinstance(print_traceback, BaseException), f'Not a exception: {print_traceback!r}'
+        console.print_exception(show_locals=True)
+
+    console.print()
+
+    if HintHighlighterClass is not None:
+        highlighter = HintHighlighterClass()
+        hint = highlighter(text=hint)
+
+    console.print(
+        Panel(
+            hint,
+            title=f'[bright][green]{title}',
+            border_style=hint_border_style,
+            expand=False,
+            padding=hint_padding,
+        )
+    )
+    console.print()
+
+    sys.exit(exit_code)
```

### Comparing `inverter-connect-0.6.1/inverter/utilities/modbus_converter.py` & `inverter-connect-0.7.0rc1/inverter/utilities/modbus_converter.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.1/inverter/validators.py` & `inverter-connect-0.7.0rc1/inverter/validators.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.1/inverter_connect.egg-info/PKG-INFO` & `inverter-connect-0.7.0rc1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: inverter-connect
-Version: 0.6.1
-Summary: Get information from Deye Microinverter
-Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
-License: GPL-3.0-or-later
-Project-URL: Documentation, https://github.com/jedie/inverter-connect
-Project-URL: Source, https://github.com/jedie/inverter-connect
-Requires-Python: <4,>=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 # inverter
 
 [![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/inverter-connect/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/inverter-connect)
 [![inverter-connect @ PyPi](https://img.shields.io/pypi/v/inverter-connect?label=inverter-connect%20%40%20PyPi)](https://pypi.org/project/inverter-connect/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/pyproject.toml)
 [![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/LICENSE)
@@ -21,14 +9,21 @@
 Get information from Deye Microinverter
 
 The whole thing is just a learning exercise for now. We will see.
 
 
 # quickstart
 
+## overview
+
+* clone the sources
+* Bootstrap and create default user settings by just call `./cli.py edit-settings`
+* Change the settings for your needs
+* ...use the commands... ;)
+
 Currently just clone the project and just start the cli (that will create a virtualenv and installs every dependencies)
 
 Note: Please enable https://www.piwheels.org/ if you are on a Raspberry Pi !
 
 e.g.:
 ```bash
 ~$ git clone https://github.com/jedie/inverter-connect.git
@@ -43,20 +38,20 @@
 Usage: ./cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
 │ debug-settings           Display (anonymized) MQTT server username and password                  │
+│ edit-settings            Edit the settings file. On first call: Create the default one.          │
 │ print-at-commands        Print one or more AT command values from Inverter.                      │
 │ print-values             Print all known register values from Inverter, e.g.:                    │
 │ publish-loop             Publish current data via MQTT for Home Assistant (endless loop)         │
 │ read-register            Read register(s) from the inverter                                      │
 │ set-time                 Set current date time in the inverter device.                           │
-│ store-settings           Store MQTT server settings.                                             │
 │ test-mqtt-connection     Test connection to MQTT Server                                          │
 │ version                  Print version and exit                                                  │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
@@ -65,61 +60,63 @@
 
 ## publish-loop
 
 Help from `./cli.py print-values --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated publish-loop help start ✂✂✂)
 ```
-Usage: ./cli.py publish-loop [OPTIONS] IP
+Usage: ./cli.py publish-loop [OPTIONS]
 
  Publish current data via MQTT for Home Assistant (endless loop)
  The "Daily Production" count will be cleared in the night, by set the current date time via
  AT-command.
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ *  --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                │
-│                                                              [default: 48899; 1000<=x<=65535]    │
-│                                                              [required]                          │
-│ *  --inverter                TEXT                            Prefix of yaml config files in      │
-│                                                              inverter/definitions/               │
-│                                                              [default: deye_2mppt]               │
-│                                                              [required]                          │
-│    --log/--no-log                                            [default: log]                      │
-│    --verbose/--no-verbose                                    [default: verbose]                  │
-│    --debug/--no-debug                                        [default: no-debug]                 │
-│    --help                                                    Show this message and exit.         │
+│ *  --ip             TEXT                     IP address of your inverter [required]              │
+│ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
+│                                              [required]                                          │
+│ *  --inverter       TEXT                     Prefix of yaml config files in                      │
+│                                              inverter/definitions/                               │
+│                                              [default: deye_2mppt]                               │
+│                                              [required]                                          │
+│    --verbosity  -v  INTEGER RANGE [0<=x<=3]  Verbosity level; Accepts integer value e.g.:        │
+│                                              "--verbose 2" or can be count e.g.: "-vv"           │
+│                                              [default: 1; 0<=x<=3]                               │
+│    --help                                    Show this message and exit.                         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated publish-loop help end ✂✂✂)
 
 
 ----
 
 
 ## print-values
 
 Help from `./cli.py print-values --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated print-values help start ✂✂✂)
 ```
-Usage: ./cli.py print-values [OPTIONS] IP
+Usage: ./cli.py print-values [OPTIONS]
 
  Print all known register values from Inverter, e.g.:
  .../inverter-connect$ ./cli.py print-values 192.168.123.456
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│    --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                │
-│                                                              [default: 48899; 1000<=x<=65535]    │
-│ *  --inverter                TEXT                            Prefix of yaml config files in      │
-│                                                              inverter/definitions/               │
-│                                                              [default: deye_2mppt]               │
-│                                                              [required]                          │
-│    --verbose/--no-verbose                                    [default: verbose]                  │
-│    --debug/--no-debug                                        [default: no-debug]                 │
-│    --help                                                    Show this message and exit.         │
+│ *  --ip             TEXT                     IP address of your inverter [required]              │
+│ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
+│                                              [required]                                          │
+│ *  --inverter       TEXT                     Prefix of yaml config files in                      │
+│                                              inverter/definitions/                               │
+│                                              [default: deye_2mppt]                               │
+│                                              [required]                                          │
+│    --verbosity  -v  INTEGER RANGE [0<=x<=3]  Verbosity level; Accepts integer value e.g.:        │
+│                                              "--verbose 2" or can be count e.g.: "-vv"           │
+│                                              [default: 1; 0<=x<=3]                               │
+│    --help                                    Show this message and exit.                         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated print-values help end ✂✂✂)
 
 Example output of `print-values` call:
 
 ![print-values](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-55.png "2023-04-28_08-55.png")
@@ -129,15 +126,15 @@
 
 ## print-at-commands
 
 Help from `./cli.py print-at-commands --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated print-at-commands help start ✂✂✂)
 ```
-Usage: ./cli.py print-at-commands [OPTIONS] IP [COMMANDS]...
+Usage: ./cli.py print-at-commands [OPTIONS] [COMMANDS]...
 
  Print one or more AT command values from Inverter.
  Use all known AT commands, if no one is given, e.g.:
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456
  Or specify one or more AT-commands, e.g.:
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 WEBVER .../inverter-connect$
  ./cli.py print-at-commands 192.168.123.456 WEBVER WEBU
@@ -145,19 +142,21 @@
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPSER=192.168.1.1 NTPEN=on
  NTPSER NTPEN
  wait a while and request the current date time:
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPTM
  (Note: The prefix "AT+" will be added to every command)
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                   │
-│                                                           [default: 48899; 1000<=x<=65535]       │
-│ --verbose/--no-verbose                                    [default: verbose]                     │
-│ --debug/--no-debug                                        [default: no-debug]                    │
-│ --help                                                    Show this message and exit.            │
+│ *  --ip             TEXT                     IP address of your inverter [required]              │
+│ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
+│                                              [required]                                          │
+│    --verbosity  -v  INTEGER RANGE [0<=x<=3]  Verbosity level; Accepts integer value e.g.:        │
+│                                              "--verbose 2" or can be count e.g.: "-vv"           │
+│                                              [default: 1; 0<=x<=3]                               │
+│    --help                                    Show this message and exit.                         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated print-at-commands help end ✂✂✂)
 
 Example output of `print-at-commands` call:
 
 ![print-at-commands](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-57.png "2023-04-28_08-57.png")
@@ -167,29 +166,31 @@
 
 ## read-register
 
 Help from `./cli.py read-register --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated read-register help start ✂✂✂)
 ```
-Usage: ./cli.py read-register [OPTIONS] IP REGISTER LENGTH
+Usage: ./cli.py read-register [OPTIONS] REGISTER LENGTH
 
  Read register(s) from the inverter
  e.g.: read 3 registers starting from 0x16:
  .../inverter-connect$ ./cli.py read-register 192.168.123.456 0x16 3
  e.g.: read the first 32 registers:
  .../inverter-connect$ ./cli.py read-register 192.168.123.456 0 32
  The start address can be pass as decimal number or as hex string, e.g.: 0x123
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                   │
-│                                                           [default: 48899; 1000<=x<=65535]       │
-│ --verbose/--no-verbose                                    [default: verbose]                     │
-│ --debug/--no-debug                                        [default: no-debug]                    │
-│ --help                                                    Show this message and exit.            │
+│ *  --ip             TEXT                     IP address of your inverter [required]              │
+│ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
+│                                              [required]                                          │
+│    --verbosity  -v  INTEGER RANGE [0<=x<=3]  Verbosity level; Accepts integer value e.g.:        │
+│                                              "--verbose 2" or can be count e.g.: "-vv"           │
+│                                              [default: 1; 0<=x<=3]                               │
+│    --help                                    Show this message and exit.                         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated read-register help end ✂✂✂)
 
 Example output of `read-register` call:
 
 ![read-register](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-53.png "2023-04-28_08-53.png")
@@ -212,14 +213,15 @@
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
 │ check-code-style            Check code style by calling darker + flake8                          │
 │ coverage                    Run and show coverage.                                               │
+│ create-default-settings     Create a default user settings file. (Used by CI pipeline ;)         │
 │ fix-code-style              Fix code style of all inverter source code files via darker          │
 │ install                     Run pip-sync and install 'inverter' via pip as editable.             │
 │ mypy                        Run Mypy (configured in pyproject.toml)                              │
 │ publish                     Build and upload this project to PyPi                                │
 │ safety                      Run safety check against current requirements files                  │
 │ test                        Run unittests                                                        │
 │ tox                         Run tox                                                              │
```

### Comparing `inverter-connect-0.6.1/inverter_connect.egg-info/SOURCES.txt` & `inverter-connect-0.7.0rc1/inverter_connect.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -17,44 +17,38 @@
 inverter/connection.py
 inverter/constants.py
 inverter/daily_reset.py
 inverter/data_types.py
 inverter/definitions.py
 inverter/exceptions.py
 inverter/publish_loop.py
+inverter/user_settings.py
 inverter/validators.py
+inverter/verbosity.py
 inverter/.github/workflows/tests.yml
 inverter/cli/__init__.py
 inverter/cli/cli_app.py
 inverter/cli/dev.py
 inverter/definitions/deye_2mppt.yaml
 inverter/definitions/deye_2mppt_validations.yaml
-inverter/mqtt4homeassistant/__init__.py
-inverter/mqtt4homeassistant/converter.py
-inverter/mqtt4homeassistant/data_classes.py
-inverter/mqtt4homeassistant/mqtt.py
-inverter/mqtt4homeassistant/tests/__init__.py
-inverter/mqtt4homeassistant/tests/test_converter.py
-inverter/mqtt4homeassistant/tests/test_doctests.py
-inverter/mqtt4homeassistant/utilities/__init__.py
-inverter/mqtt4homeassistant/utilities/string_utils.py
 inverter/tests/__init__.py
+inverter/tests/fixtures.py
 inverter/tests/test_api.py
 inverter/tests/test_cli.py
 inverter/tests/test_connect.py
 inverter/tests/test_daily_reset.py
 inverter/tests/test_definitions.py
 inverter/tests/test_doctests.py
 inverter/tests/test_project_setup.py
 inverter/tests/test_readme.py
+inverter/tests/test_user_settings.py
+inverter/tests/test_user_settings_migrate_old_settings_1.snapshot.toml
 inverter/tests/test_validators.py
 inverter/utilities/__init__.py
 inverter/utilities/cli.py
-inverter/utilities/credentials.py
-inverter/utilities/log_setup.py
 inverter/utilities/modbus_converter.py
 inverter_connect.egg-info/PKG-INFO
 inverter_connect.egg-info/SOURCES.txt
 inverter_connect.egg-info/dependency_links.txt
 inverter_connect.egg-info/entry_points.txt
 inverter_connect.egg-info/requires.txt
 inverter_connect.egg-info/top_level.txt
```

### Comparing `inverter-connect-0.6.1/pyproject.toml` & `inverter-connect-0.7.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 license = {text = "GPL-3.0-or-later"}
 readme = "README.md"
 authors = [
     {name = 'Jens Diemer', email = 'inverter-connect@jensdiemer.de'}
 ]
 requires-python = ">=3.9,<4"
 dependencies = [
+    "ha-services", # https://github.com/jedie/ha-services
     "paho-mqtt",  # https://pypi.org/project/paho-mqtt/
     "msgspec",  # https://github.com/jcrist/msgspec
     "pyyaml",  # https://github.com/yaml/pyyaml
     "bx_py_utils",  # https://github.com/boxine/bx_py_utils
     "click",  # https://github.com/pallets/click/
     "rich-click",  # https://github.com/ewels/rich-click
     "rich",  # https://github.com/Textualize/rich
```

### Comparing `inverter-connect-0.6.1/requirements.dev.txt` & `inverter-connect-0.7.0rc1/requirements.dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -55,23 +55,24 @@
     --hash=sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171 \
     --hash=sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269
     # via pip-tools
 bx-py-utils==80 \
     --hash=sha256:34c4f5e4e1199014a83139aa4285a85f84274a982f9a9a8eae056fd9848a42f7 \
     --hash=sha256:59f3d641c516fdf75d47ea86cd84fe6405d07fc7761074dcbbb967b6962dcc09
     # via
+    #   ha-services
     #   inverter-connect (pyproject.toml)
     #   manageprojects
 cachetools==5.3.0 \
     --hash=sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14 \
     --hash=sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4
     # via tox
-certifi==2022.12.7 \
-    --hash=sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3 \
-    --hash=sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18
+certifi==2023.5.7 \
+    --hash=sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7 \
+    --hash=sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716
     # via requests
 cffi==1.15.1 \
     --hash=sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5 \
     --hash=sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef \
     --hash=sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104 \
     --hash=sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426 \
     --hash=sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405 \
@@ -220,14 +221,15 @@
     # via requests
 click==8.1.3 \
     --hash=sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e \
     --hash=sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48
     # via
     #   black
     #   cookiecutter
+    #   ha-services
     #   inverter-connect (pyproject.toml)
     #   manageprojects
     #   pip-tools
     #   rich-click
     #   safety
 codespell==2.2.4 \
     --hash=sha256:0b4620473c257d9cde1ff8998b26b2bb209a35c2b7489f5dc3436024298ce83a \
@@ -349,14 +351,18 @@
     --hash=sha256:2863ac8ec19d6ec8d29e760546e6ced644baf6dff3c7cdc77e03abbd29b80f14 \
     --hash=sha256:2bd1b37043ad88a3f3c3c34a76fc0b64d24e5f03d36ea6b48cb69cc642bff17e
     # via darker
 freezegun==1.2.2 \
     --hash=sha256:cd22d1ba06941384410cd967d8a99d5ae2442f57dfafeff2fda5de8dc5c05446 \
     --hash=sha256:ea1b963b993cb9ea195adbd893a48d573fda951b0da64f60883d7e988b606c9f
     # via inverter-connect (pyproject.toml)
+ha-services==0.0.1 \
+    --hash=sha256:9ab060d3afed22ab83176179dc2808ad8b30b7df34b9940897e0ffc5face92ec \
+    --hash=sha256:eeb6a6c30988338ef8aec49bd7f5bf42b764d38452f5051603d7e0b21ed0426c
+    # via inverter-connect (pyproject.toml)
 idna==3.4 \
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
     # via requests
 importlib-metadata==6.6.0 \
     --hash=sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed \
     --hash=sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705
@@ -489,15 +495,17 @@
     --hash=sha256:d03861f0d271b696faefb1a885ea0c7dc7db70baaa05c7f18086f2b9085d1cb8 \
     --hash=sha256:d469aede5d986223d6ec9a8d0713156f96fd6b427b12e14f81d26627a47687b9 \
     --hash=sha256:d85e9bfd1441216010c084626d968e96a3d88d762959c5eb430de62076cd7fe9 \
     --hash=sha256:decd1d2015d340ebfd58f29ed2916e118ca255b6a94fc1787a236a2654dfd8ff \
     --hash=sha256:eee59e73982ca0d730f8d4e8fb5f01da9fa466490dea43ea1bcfa23b8a8bbc0d \
     --hash=sha256:f97006b9c9e24e9677fb84f43586fb4d03a72eb426199656a1c24775c62b9fe4 \
     --hash=sha256:ff7c987330e2be62eb8811bc2da33507e8edeb761f4fd343f2fa5fdafce4f989
-    # via inverter-connect (pyproject.toml)
+    # via
+    #   ha-services
+    #   inverter-connect (pyproject.toml)
 mypy==1.2.0 \
     --hash=sha256:023fe9e618182ca6317ae89833ba422c411469156b690fde6a315ad10695a521 \
     --hash=sha256:031fc69c9a7e12bcc5660b74122ed84b3f1c505e762cc4296884096c6d8ee140 \
     --hash=sha256:2de7babe398cb7a85ac7f1fd5c42f396c215ab3eff731b4d761d68d0f6a80f48 \
     --hash=sha256:2e93a8a553e0394b26c4ca683923b85a69f7ccdc0139e6acd1354cc884fe0128 \
     --hash=sha256:390bc685ec209ada4e9d35068ac6988c60160b2b703072d2850457b62499e336 \
     --hash=sha256:3a2d219775a120581a0ae8ca392b31f238d452729adbcb6892fa89688cb8306a \
@@ -536,15 +544,17 @@
     #   build
     #   dparse
     #   pyproject-api
     #   safety
     #   tox
 paho-mqtt==1.6.1 \
     --hash=sha256:2a8291c81623aec00372b5a85558a372c747cbca8e9934dfe218638b8eefc26f
-    # via inverter-connect (pyproject.toml)
+    # via
+    #   ha-services
+    #   inverter-connect (pyproject.toml)
 pathspec==0.11.1 \
     --hash=sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687 \
     --hash=sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293
     # via black
 pip-tools==6.13.0 \
     --hash=sha256:50943f151d87e752abddec8158622c34ad7f292e193836e90e30d87da60b19d9 \
     --hash=sha256:61d46bd2eb8016ed4a924e196e6e5b0a268cd3babd79e593048720db23522bb1
@@ -601,17 +611,17 @@
     # via
     #   arrow
     #   freezegun
 python-slugify==8.0.1 \
     --hash=sha256:70ca6ea68fe63ecc8fa4fcf00ae651fc8a5d02d93dcd12ae6d4fc7ca46c4d395 \
     --hash=sha256:ce0d46ddb668b3be82f4ed5e503dbc33dd815d83e2eb6824211310d3fb172a27
     # via cookiecutter
-pyupgrade==3.3.2 \
-    --hash=sha256:bcfed63d38811809f179fd269dec246680b0aaa5bbe662b535826e5fa2275219 \
-    --hash=sha256:c05b82c911934b3a638b29f48f48dc6e0ef6c57c55ec36f2b41ae9dbf6711b4b
+pyupgrade==3.4.0 \
+    --hash=sha256:98b6bee32149f662da1aa038cb9baf93d592ae696059acd613db6ff583583048 \
+    --hash=sha256:f6bcf0d5e59170d178a2630e981d0e7b04d9b13f3c0e7e62f3e6bab582f841e4
     # via inverter-connect (pyproject.toml)
 pyyaml==6.0 \
     --hash=sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf \
     --hash=sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293 \
     --hash=sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b \
     --hash=sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57 \
     --hash=sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b \
@@ -673,27 +683,29 @@
     --hash=sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd \
     --hash=sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c
     # via twine
 rich==13.3.5 \
     --hash=sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c \
     --hash=sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704
     # via
+    #   ha-services
     #   inverter-connect (pyproject.toml)
     #   manageprojects
     #   rich-click
     #   twine
 rich-click==1.6.1 \
     --hash=sha256:0fcf4d1a09029d79322dd814ab0b2e66ac183633037561881d45abae8a161d95 \
     --hash=sha256:f8ff96693ec6e261d1544e9f7d9a5811c5ef5d74c8adb4978430fc0dac16777e
     # via
+    #   ha-services
     #   inverter-connect (pyproject.toml)
     #   manageprojects
-ruamel-yaml==0.17.23 \
-    --hash=sha256:40e549c264e799d8e4cd9e54e869ffa60c9436e1ef497500b08fbda3b92a1517 \
-    --hash=sha256:605510839d5af3ae730f3ed6408b7004c83f97aa2b732f6f366da7c2fc2f0d9c
+ruamel-yaml==0.17.24 \
+    --hash=sha256:90e398ee24524ebe20fc48cd1861cedd25520457b9a36cfb548613e57fde30a0 \
+    --hash=sha256:f251bd9096207af604af69d6495c3c650a3338d0493d27b04bc55477d7a884ed
     # via safety
 ruamel-yaml-clib==0.2.7 \
     --hash=sha256:045e0626baf1c52e5527bd5db361bc83180faaba2ff586e763d3d5982a876a9e \
     --hash=sha256:15910ef4f3e537eea7fe45f8a5d19997479940d9196f357152a09031c5be59f3 \
     --hash=sha256:184faeaec61dbaa3cace407cffc5819f7b977e75360e8d5ca19461cd851a5fc5 \
     --hash=sha256:1f08fd5a2bea9c4180db71678e850b995d2a5f4537be0e94557668cf0f5f9497 \
     --hash=sha256:2aa261c29a5545adfef9296b7e33941f46aa5bbd21164228e833412af4c9c75f \
@@ -769,15 +781,17 @@
     #   mypy
     #   pyproject-api
     #   pyproject-hooks
     #   tox
 tomlkit==0.11.8 \
     --hash=sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171 \
     --hash=sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3
-    # via manageprojects
+    # via
+    #   ha-services
+    #   manageprojects
 tox==4.5.1 \
     --hash=sha256:5a2eac5fb816779dfdf5cb00fecbc27eb0524e4626626bb1de84747b24cacc56 \
     --hash=sha256:d25a2e6cb261adc489604fafd76cd689efeadfa79709965e965668d6d3f63046
     # via inverter-connect (pyproject.toml)
 twine==4.0.2 \
     --hash=sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8 \
     --hash=sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8
```

### Comparing `inverter-connect-0.6.1/requirements.txt` & `inverter-connect-0.7.0rc1/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,28 @@
 # by the following command:
 #
 #    ./cli.py update
 #
 bx-py-utils==80 \
     --hash=sha256:34c4f5e4e1199014a83139aa4285a85f84274a982f9a9a8eae056fd9848a42f7 \
     --hash=sha256:59f3d641c516fdf75d47ea86cd84fe6405d07fc7761074dcbbb967b6962dcc09
-    # via inverter-connect (pyproject.toml)
+    # via
+    #   ha-services
+    #   inverter-connect (pyproject.toml)
 click==8.1.3 \
     --hash=sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e \
     --hash=sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48
     # via
+    #   ha-services
     #   inverter-connect (pyproject.toml)
     #   rich-click
+ha-services==0.0.1 \
+    --hash=sha256:9ab060d3afed22ab83176179dc2808ad8b30b7df34b9940897e0ffc5face92ec \
+    --hash=sha256:eeb6a6c30988338ef8aec49bd7f5bf42b764d38452f5051603d7e0b21ed0426c
+    # via inverter-connect (pyproject.toml)
 markdown-it-py==2.2.0 \
     --hash=sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30 \
     --hash=sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1
     # via rich
 mdurl==0.1.2 \
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
     --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
@@ -48,18 +55,22 @@
     --hash=sha256:d03861f0d271b696faefb1a885ea0c7dc7db70baaa05c7f18086f2b9085d1cb8 \
     --hash=sha256:d469aede5d986223d6ec9a8d0713156f96fd6b427b12e14f81d26627a47687b9 \
     --hash=sha256:d85e9bfd1441216010c084626d968e96a3d88d762959c5eb430de62076cd7fe9 \
     --hash=sha256:decd1d2015d340ebfd58f29ed2916e118ca255b6a94fc1787a236a2654dfd8ff \
     --hash=sha256:eee59e73982ca0d730f8d4e8fb5f01da9fa466490dea43ea1bcfa23b8a8bbc0d \
     --hash=sha256:f97006b9c9e24e9677fb84f43586fb4d03a72eb426199656a1c24775c62b9fe4 \
     --hash=sha256:ff7c987330e2be62eb8811bc2da33507e8edeb761f4fd343f2fa5fdafce4f989
-    # via inverter-connect (pyproject.toml)
+    # via
+    #   ha-services
+    #   inverter-connect (pyproject.toml)
 paho-mqtt==1.6.1 \
     --hash=sha256:2a8291c81623aec00372b5a85558a372c747cbca8e9934dfe218638b8eefc26f
-    # via inverter-connect (pyproject.toml)
+    # via
+    #   ha-services
+    #   inverter-connect (pyproject.toml)
 pygments==2.15.1 \
     --hash=sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c \
     --hash=sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1
     # via rich
 pyyaml==6.0 \
     --hash=sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf \
     --hash=sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293 \
@@ -102,13 +113,20 @@
     --hash=sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174 \
     --hash=sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5
     # via inverter-connect (pyproject.toml)
 rich==13.3.5 \
     --hash=sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c \
     --hash=sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704
     # via
+    #   ha-services
     #   inverter-connect (pyproject.toml)
     #   rich-click
 rich-click==1.6.1 \
     --hash=sha256:0fcf4d1a09029d79322dd814ab0b2e66ac183633037561881d45abae8a161d95 \
     --hash=sha256:f8ff96693ec6e261d1544e9f7d9a5811c5ef5d74c8adb4978430fc0dac16777e
-    # via inverter-connect (pyproject.toml)
+    # via
+    #   ha-services
+    #   inverter-connect (pyproject.toml)
+tomlkit==0.11.8 \
+    --hash=sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171 \
+    --hash=sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3
+    # via ha-services
```

