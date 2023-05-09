# Comparing `tmp/test_rest_api-0.0.0.0.30.tar.gz` & `tmp/test_rest_api-0.0.0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_rest_api-0.0.0.0.30.tar", last modified: Fri May  5 09:44:52 2023, max compression
+gzip compressed data, was "test_rest_api-0.0.0.0.31.tar", last modified: Tue May  9 05:44:11 2023, max compression
```

## Comparing `test_rest_api-0.0.0.0.30.tar` & `test_rest_api-0.0.0.0.31.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.227249 test_rest_api-0.0.0.0.30/
--rw-r--r--   0 trjose     (501) staff       (20)     1067 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.30/LICENSE
--rw-r--r--   0 trjose     (501) staff       (20)    64379 2023-05-05 09:44:52.226955 test_rest_api-0.0.0.0.30/PKG-INFO
--rw-r--r--   0 trjose     (501) staff       (20)    62656 2023-05-02 07:11:18.000000 test_rest_api-0.0.0.0.30/README.md
--rw-r--r--   0 trjose     (501) staff       (20)       38 2023-05-05 09:44:52.227383 test_rest_api-0.0.0.0.30/setup.cfg
--rw-r--r--   0 trjose     (501) staff       (20)     2946 2023-05-05 09:43:30.000000 test_rest_api-0.0.0.0.30/setup.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.198647 test_rest_api-0.0.0.0.30/test_rest_api/
--rw-r--r--   0 trjose     (501) staff       (20)      242 2023-04-25 18:38:10.000000 test_rest_api-0.0.0.0.30/test_rest_api/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1608 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.30/test_rest_api/__main__.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.202980 test_rest_api-0.0.0.0.30/test_rest_api/assertion/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-20 18:34:45.000000 test_rest_api-0.0.0.0.30/test_rest_api/assertion/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1675 2023-04-28 10:04:23.000000 test_rest_api-0.0.0.0.30/test_rest_api/assertion/assertion.py
--rw-r--r--   0 trjose     (501) staff       (20)      107 2023-04-25 18:29:05.000000 test_rest_api-0.0.0.0.30/test_rest_api/assertion/exception.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.205098 test_rest_api-0.0.0.0.30/test_rest_api/global_variables/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.30/test_rest_api/global_variables/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      116 2023-04-25 18:28:31.000000 test_rest_api-0.0.0.0.30/test_rest_api/global_variables/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)     4044 2023-04-25 18:18:31.000000 test_rest_api-0.0.0.0.30/test_rest_api/global_variables/global_variables.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.207795 test_rest_api-0.0.0.0.30/test_rest_api/reporting/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-25 09:45:47.000000 test_rest_api-0.0.0.0.30/test_rest_api/reporting/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)    35380 2023-04-26 10:08:07.000000 test_rest_api-0.0.0.0.30/test_rest_api/reporting/html.py
--rw-r--r--   0 trjose     (501) staff       (20)     5427 2023-04-26 10:06:51.000000 test_rest_api-0.0.0.0.30/test_rest_api/reporting/report.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.212058 test_rest_api-0.0.0.0.30/test_rest_api/rest_api/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:34:23.000000 test_rest_api-0.0.0.0.30/test_rest_api/rest_api/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      177 2023-04-25 18:31:18.000000 test_rest_api-0.0.0.0.30/test_rest_api/rest_api/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      423 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.30/test_rest_api/rest_api/method.py
--rw-r--r--   0 trjose     (501) staff       (20)      579 2023-04-25 14:33:03.000000 test_rest_api-0.0.0.0.30/test_rest_api/rest_api/response.py
--rw-r--r--   0 trjose     (501) staff       (20)     6616 2023-04-26 07:15:33.000000 test_rest_api-0.0.0.0.30/test_rest_api/rest_api/rest_api.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.213826 test_rest_api-0.0.0.0.30/test_rest_api/settings/
--rw-r--r--   0 trjose     (501) staff       (20)       29 2023-04-26 09:34:57.000000 test_rest_api-0.0.0.0.30/test_rest_api/settings/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      149 2023-04-25 14:29:54.000000 test_rest_api-0.0.0.0.30/test_rest_api/settings/logging.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.219941 test_rest_api-0.0.0.0.30/test_rest_api/testing/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:03:23.000000 test_rest_api-0.0.0.0.30/test_rest_api/testing/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     3520 2023-04-28 09:43:49.000000 test_rest_api-0.0.0.0.30/test_rest_api/testing/bug.py
--rw-r--r--   0 trjose     (501) staff       (20)    14090 2023-04-28 11:51:16.000000 test_rest_api-0.0.0.0.30/test_rest_api/testing/decorator.py
--rw-r--r--   0 trjose     (501) staff       (20)      112 2023-04-25 18:31:32.000000 test_rest_api-0.0.0.0.30/test_rest_api/testing/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)    12905 2023-04-26 10:09:41.000000 test_rest_api-0.0.0.0.30/test_rest_api/testing/runner.py
--rw-r--r--   0 trjose     (501) staff       (20)     2696 2023-05-02 05:37:13.000000 test_rest_api-0.0.0.0.30/test_rest_api/testing/traceback.py
--rw-r--r--   0 trjose     (501) staff       (20)      785 2023-04-26 09:40:30.000000 test_rest_api-0.0.0.0.30/test_rest_api/testing/utils.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.225867 test_rest_api-0.0.0.0.30/test_rest_api/utils/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.30/test_rest_api/utils/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      943 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.30/test_rest_api/utils/aiohttp_session.py
--rw-r--r--   0 trjose     (501) staff       (20)      247 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.30/test_rest_api/utils/decorator_hints.py
--rw-r--r--   0 trjose     (501) staff       (20)     1369 2023-04-26 10:50:21.000000 test_rest_api-0.0.0.0.30/test_rest_api/utils/error_msg.py
--rw-r--r--   0 trjose     (501) staff       (20)     2032 2023-04-28 11:35:57.000000 test_rest_api-0.0.0.0.30/test_rest_api/utils/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      606 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.30/test_rest_api/utils/logger.py
--rw-r--r--   0 trjose     (501) staff       (20)     1322 2023-04-19 12:03:08.000000 test_rest_api-0.0.0.0.30/test_rest_api/utils/string_color.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-05 09:44:52.200929 test_rest_api-0.0.0.0.30/test_rest_api.egg-info/
--rw-r--r--   0 trjose     (501) staff       (20)    64379 2023-05-05 09:44:52.000000 test_rest_api-0.0.0.0.30/test_rest_api.egg-info/PKG-INFO
--rw-r--r--   0 trjose     (501) staff       (20)     1328 2023-05-05 09:44:52.000000 test_rest_api-0.0.0.0.30/test_rest_api.egg-info/SOURCES.txt
--rw-r--r--   0 trjose     (501) staff       (20)        1 2023-05-05 09:44:52.000000 test_rest_api-0.0.0.0.30/test_rest_api.egg-info/dependency_links.txt
--rw-r--r--   0 trjose     (501) staff       (20)       29 2023-05-05 09:44:52.000000 test_rest_api-0.0.0.0.30/test_rest_api.egg-info/requires.txt
--rw-r--r--   0 trjose     (501) staff       (20)       14 2023-05-05 09:44:52.000000 test_rest_api-0.0.0.0.30/test_rest_api.egg-info/top_level.txt
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.893003 test_rest_api-0.0.0.0.31/
+-rw-r--r--   0 trjose     (501) staff       (20)     1067 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.31/LICENSE
+-rw-r--r--   0 trjose     (501) staff       (20)    64379 2023-05-09 05:44:11.892716 test_rest_api-0.0.0.0.31/PKG-INFO
+-rw-r--r--   0 trjose     (501) staff       (20)    62656 2023-05-02 07:11:18.000000 test_rest_api-0.0.0.0.31/README.md
+-rw-r--r--   0 trjose     (501) staff       (20)       38 2023-05-09 05:44:11.893108 test_rest_api-0.0.0.0.31/setup.cfg
+-rw-r--r--   0 trjose     (501) staff       (20)     2946 2023-05-09 05:43:56.000000 test_rest_api-0.0.0.0.31/setup.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.878530 test_rest_api-0.0.0.0.31/test_rest_api/
+-rw-r--r--   0 trjose     (501) staff       (20)      242 2023-04-25 18:38:10.000000 test_rest_api-0.0.0.0.31/test_rest_api/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1608 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.31/test_rest_api/__main__.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.882562 test_rest_api-0.0.0.0.31/test_rest_api/assertion/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-20 18:34:45.000000 test_rest_api-0.0.0.0.31/test_rest_api/assertion/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1675 2023-04-28 10:04:23.000000 test_rest_api-0.0.0.0.31/test_rest_api/assertion/assertion.py
+-rw-r--r--   0 trjose     (501) staff       (20)      107 2023-04-25 18:29:05.000000 test_rest_api-0.0.0.0.31/test_rest_api/assertion/exception.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.883596 test_rest_api-0.0.0.0.31/test_rest_api/global_variables/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.31/test_rest_api/global_variables/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      116 2023-04-25 18:28:31.000000 test_rest_api-0.0.0.0.31/test_rest_api/global_variables/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)     4044 2023-04-25 18:18:31.000000 test_rest_api-0.0.0.0.31/test_rest_api/global_variables/global_variables.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.884741 test_rest_api-0.0.0.0.31/test_rest_api/reporting/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-25 09:45:47.000000 test_rest_api-0.0.0.0.31/test_rest_api/reporting/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)    35380 2023-04-26 10:08:07.000000 test_rest_api-0.0.0.0.31/test_rest_api/reporting/html.py
+-rw-r--r--   0 trjose     (501) staff       (20)     5427 2023-04-26 10:06:51.000000 test_rest_api-0.0.0.0.31/test_rest_api/reporting/report.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.886592 test_rest_api-0.0.0.0.31/test_rest_api/rest_api/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:34:23.000000 test_rest_api-0.0.0.0.31/test_rest_api/rest_api/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      177 2023-04-25 18:31:18.000000 test_rest_api-0.0.0.0.31/test_rest_api/rest_api/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      423 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.31/test_rest_api/rest_api/method.py
+-rw-r--r--   0 trjose     (501) staff       (20)      579 2023-04-25 14:33:03.000000 test_rest_api-0.0.0.0.31/test_rest_api/rest_api/response.py
+-rw-r--r--   0 trjose     (501) staff       (20)     6725 2023-05-09 05:40:02.000000 test_rest_api-0.0.0.0.31/test_rest_api/rest_api/rest_api.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.887307 test_rest_api-0.0.0.0.31/test_rest_api/settings/
+-rw-r--r--   0 trjose     (501) staff       (20)       29 2023-04-26 09:34:57.000000 test_rest_api-0.0.0.0.31/test_rest_api/settings/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      149 2023-04-25 14:29:54.000000 test_rest_api-0.0.0.0.31/test_rest_api/settings/logging.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.889695 test_rest_api-0.0.0.0.31/test_rest_api/testing/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:03:23.000000 test_rest_api-0.0.0.0.31/test_rest_api/testing/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     3520 2023-04-28 09:43:49.000000 test_rest_api-0.0.0.0.31/test_rest_api/testing/bug.py
+-rw-r--r--   0 trjose     (501) staff       (20)    14090 2023-04-28 11:51:16.000000 test_rest_api-0.0.0.0.31/test_rest_api/testing/decorator.py
+-rw-r--r--   0 trjose     (501) staff       (20)      112 2023-04-25 18:31:32.000000 test_rest_api-0.0.0.0.31/test_rest_api/testing/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)    12905 2023-04-26 10:09:41.000000 test_rest_api-0.0.0.0.31/test_rest_api/testing/runner.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2696 2023-05-02 05:37:13.000000 test_rest_api-0.0.0.0.31/test_rest_api/testing/traceback.py
+-rw-r--r--   0 trjose     (501) staff       (20)      785 2023-04-26 09:40:30.000000 test_rest_api-0.0.0.0.31/test_rest_api/testing/utils.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.892057 test_rest_api-0.0.0.0.31/test_rest_api/utils/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.31/test_rest_api/utils/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      943 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.31/test_rest_api/utils/aiohttp_session.py
+-rw-r--r--   0 trjose     (501) staff       (20)      247 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.31/test_rest_api/utils/decorator_hints.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1369 2023-04-26 10:50:21.000000 test_rest_api-0.0.0.0.31/test_rest_api/utils/error_msg.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2032 2023-04-28 11:35:57.000000 test_rest_api-0.0.0.0.31/test_rest_api/utils/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      606 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.31/test_rest_api/utils/logger.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1322 2023-04-19 12:03:08.000000 test_rest_api-0.0.0.0.31/test_rest_api/utils/string_color.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-05-09 05:44:11.881413 test_rest_api-0.0.0.0.31/test_rest_api.egg-info/
+-rw-r--r--   0 trjose     (501) staff       (20)    64379 2023-05-09 05:44:11.000000 test_rest_api-0.0.0.0.31/test_rest_api.egg-info/PKG-INFO
+-rw-r--r--   0 trjose     (501) staff       (20)     1328 2023-05-09 05:44:11.000000 test_rest_api-0.0.0.0.31/test_rest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 trjose     (501) staff       (20)        1 2023-05-09 05:44:11.000000 test_rest_api-0.0.0.0.31/test_rest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 trjose     (501) staff       (20)       29 2023-05-09 05:44:11.000000 test_rest_api-0.0.0.0.31/test_rest_api.egg-info/requires.txt
+-rw-r--r--   0 trjose     (501) staff       (20)       14 2023-05-09 05:44:11.000000 test_rest_api-0.0.0.0.31/test_rest_api.egg-info/top_level.txt
```

### Comparing `test_rest_api-0.0.0.0.30/LICENSE` & `test_rest_api-0.0.0.0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.30/PKG-INFO` & `test_rest_api-0.0.0.0.31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_rest_api
-Version: 0.0.0.0.30
+Version: 0.0.0.0.31
 Summary: Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests
 Home-page: https://github.com/troymjose/test_rest_api
 Author: Troy M Jose
 Author-email: 
 Project-URL: Source, https://github.com/troymjose/test_rest_api
 Project-URL: Tracker, https://github.com/troymjose/test_rest_api/issues
 Keywords: test,unittest,restapi,testframework,asyncio,async,asynchronous,testingframework,rest,api,python,python3,testing,unittesting,automation,automationtest,automationtesting,restapitest,restapitesting,restapiunittest,restapiunittesting,restapiautomation,restapiautomationtest,restapiautomationtesting,apitest,apitesting,apiunittest,apiunittesting,apiautomation,apiautomationtest,apiautomationtesting
```

### Comparing `test_rest_api-0.0.0.0.30/README.md` & `test_rest_api-0.0.0.0.31/README.md`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.30/setup.py` & `test_rest_api-0.0.0.0.31/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Get README.md details
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = '\n' + f.read()
 
 # Setup
 setup(name='test_rest_api',
-      version='0.0.0.0.30',
+      version='0.0.0.0.31',
       author='Troy M Jose',
       author_email='',
       url='https://github.com/troymjose/test_rest_api',
       bugtrack_url='https://github.com/troymjose/test_rest_api/issues',
       project_urls={
           'Source': 'https://github.com/troymjose/test_rest_api',
           'Tracker': 'https://github.com/troymjose/test_rest_api/issues',
```

### Comparing `test_rest_api-0.0.0.0.30/test_rest_api/__main__.py` & `test_rest_api-0.0.0.0.31/test_rest_api/__main__.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.30/test_rest_api/assertion/assertion.py` & `test_rest_api-0.0.0.0.31/test_rest_api/assertion/assertion.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.30/test_rest_api/global_variables/global_variables.py` & `test_rest_api-0.0.0.0.31/test_rest_api/global_variables/global_variables.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.30/test_rest_api/reporting/html.py` & `test_rest_api-0.0.0.0.31/test_rest_api/reporting/html.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.30/test_rest_api/reporting/report.py` & `test_rest_api-0.0.0.0.31/test_rest_api/reporting/report.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.30/test_rest_api/rest_api/response.py` & `test_rest_api-0.0.0.0.31/test_rest_api/rest_api/response.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.30/test_rest_api/rest_api/rest_api.py` & `test_rest_api-0.0.0.0.31/test_rest_api/rest_api/rest_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,16 @@
 """
 
     async def _create_response(self, response: ClientResponse) -> RestApiResponse:
         """
         Create response instance object from aiohttp async response
         """
         # Retrieve the response body in JSON
-        body = await response.json()
+        # Only supports application/json content type
+        body = await response.json() if response.content_type == 'application/json' else {}
         # Get the other response parameters
         status_code, headers, content_type = response.status, dict(response.headers), response.content_type
         # Create and return the RestApiResponse instance object
         rest_api_response = RestApiResponse(status_code=status_code,
                                             content_type=content_type,
                                             body=body,
                                             headers=headers,
```

### Comparing `test_rest_api-0.0.0.0.30/test_rest_api/testing/bug.py` & `test_rest_api-0.0.0.0.31/test_rest_api/testing/bug.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.30/test_rest_api/testing/decorator.py` & `test_rest_api-0.0.0.0.31/test_rest_api/testing/decorator.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.30/test_rest_api/testing/runner.py` & `test_rest_api-0.0.0.0.31/test_rest_api/testing/runner.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.30/test_rest_api/testing/traceback.py` & `test_rest_api-0.0.0.0.31/test_rest_api/testing/traceback.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.30/test_rest_api/testing/utils.py` & `test_rest_api-0.0.0.0.31/test_rest_api/testing/utils.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.30/test_rest_api/utils/aiohttp_session.py` & `test_rest_api-0.0.0.0.31/test_rest_api/utils/aiohttp_session.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.30/test_rest_api/utils/error_msg.py` & `test_rest_api-0.0.0.0.31/test_rest_api/utils/error_msg.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.30/test_rest_api/utils/exception.py` & `test_rest_api-0.0.0.0.31/test_rest_api/utils/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.30/test_rest_api/utils/logger.py` & `test_rest_api-0.0.0.0.31/test_rest_api/utils/logger.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.30/test_rest_api/utils/string_color.py` & `test_rest_api-0.0.0.0.31/test_rest_api/utils/string_color.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.30/test_rest_api.egg-info/PKG-INFO` & `test_rest_api-0.0.0.0.31/test_rest_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-rest-api
-Version: 0.0.0.0.30
+Version: 0.0.0.0.31
 Summary: Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests
 Home-page: https://github.com/troymjose/test_rest_api
 Author: Troy M Jose
 Author-email: 
 Project-URL: Source, https://github.com/troymjose/test_rest_api
 Project-URL: Tracker, https://github.com/troymjose/test_rest_api/issues
 Keywords: test,unittest,restapi,testframework,asyncio,async,asynchronous,testingframework,rest,api,python,python3,testing,unittesting,automation,automationtest,automationtesting,restapitest,restapitesting,restapiunittest,restapiunittesting,restapiautomation,restapiautomationtest,restapiautomationtesting,apitest,apitesting,apiunittest,apiunittesting,apiautomation,apiautomationtest,apiautomationtesting
```

### Comparing `test_rest_api-0.0.0.0.30/test_rest_api.egg-info/SOURCES.txt` & `test_rest_api-0.0.0.0.31/test_rest_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

