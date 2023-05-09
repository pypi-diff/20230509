# Comparing `tmp/cgiw-0.1.5.tar.gz` & `tmp/cgiw-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgiw-0.1.5.tar", last modified: Tue May  9 13:16:01 2023, max compression
+gzip compressed data, was "cgiw-0.1.6.tar", last modified: Tue May  9 13:29:28 2023, max compression
```

## Comparing `cgiw-0.1.5.tar` & `cgiw-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-09 13:16:01.917287 cgiw-0.1.5/
--rw-rw-r--   0 james     (1000) james     (1000)    35149 2023-01-05 15:28:28.000000 cgiw-0.1.5/LICENSE
--rw-rw-r--   0 james     (1000) james     (1000)     1629 2023-05-09 13:16:01.917287 cgiw-0.1.5/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)     1117 2023-01-22 20:57:29.000000 cgiw-0.1.5/README.md
--rw-rw-r--   0 james     (1000) james     (1000)      584 2023-05-09 13:15:16.000000 cgiw-0.1.5/pyproject.toml
--rw-rw-r--   0 james     (1000) james     (1000)       38 2023-05-09 13:16:01.917287 cgiw-0.1.5/setup.cfg
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-09 13:16:01.909287 cgiw-0.1.5/src/
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-09 13:16:01.913287 cgiw-0.1.5/src/cgiw/
--rw-rw-r--   0 james     (1000) james     (1000)       21 2023-01-16 23:30:07.000000 cgiw-0.1.5/src/cgiw/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)      238 2023-01-22 20:04:01.000000 cgiw-0.1.5/src/cgiw/composers.py
--rw-rw-r--   0 james     (1000) james     (1000)      872 2023-01-22 20:45:17.000000 cgiw-0.1.5/src/cgiw/decorators.py
--rw-rw-r--   0 james     (1000) james     (1000)      438 2023-04-11 12:49:00.000000 cgiw-0.1.5/src/cgiw/exceptions.py
--rw-rw-r--   0 james     (1000) james     (1000)      785 2023-05-09 13:14:20.000000 cgiw-0.1.5/src/cgiw/handler.py
--rw-rw-r--   0 james     (1000) james     (1000)      415 2023-05-09 13:14:01.000000 cgiw-0.1.5/src/cgiw/logger.py
--rw-rw-r--   0 james     (1000) james     (1000)     1364 2023-04-11 13:07:34.000000 cgiw-0.1.5/src/cgiw/parsers.py
--rw-rw-r--   0 james     (1000) james     (1000)      581 2023-02-24 22:19:27.000000 cgiw-0.1.5/src/cgiw/responses.py
--rw-rw-r--   0 james     (1000) james     (1000)      749 2023-04-11 12:44:30.000000 cgiw-0.1.5/src/cgiw/run.py
--rw-rw-r--   0 james     (1000) james     (1000)      516 2023-01-22 20:49:49.000000 cgiw-0.1.5/src/cgiw/types.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-09 13:16:01.913287 cgiw-0.1.5/src/cgiw.egg-info/
--rw-rw-r--   0 james     (1000) james     (1000)     1629 2023-05-09 13:16:01.000000 cgiw-0.1.5/src/cgiw.egg-info/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)      499 2023-05-09 13:16:01.000000 cgiw-0.1.5/src/cgiw.egg-info/SOURCES.txt
--rw-rw-r--   0 james     (1000) james     (1000)        1 2023-05-09 13:16:01.000000 cgiw-0.1.5/src/cgiw.egg-info/dependency_links.txt
--rw-rw-r--   0 james     (1000) james     (1000)        5 2023-05-09 13:16:01.000000 cgiw-0.1.5/src/cgiw.egg-info/top_level.txt
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-09 13:16:01.917287 cgiw-0.1.5/tests/
--rw-rw-r--   0 james     (1000) james     (1000)      529 2023-01-22 20:02:27.000000 cgiw-0.1.5/tests/test_composers.py
--rw-rw-r--   0 james     (1000) james     (1000)     1054 2023-04-11 13:03:07.000000 cgiw-0.1.5/tests/test_decorators.py
--rw-rw-r--   0 james     (1000) james     (1000)      876 2023-04-11 13:04:06.000000 cgiw-0.1.5/tests/test_handler.py
--rw-rw-r--   0 james     (1000) james     (1000)     1033 2023-01-09 23:56:09.000000 cgiw-0.1.5/tests/test_parsers.py
--rw-rw-r--   0 james     (1000) james     (1000)      700 2023-01-22 20:49:00.000000 cgiw-0.1.5/tests/test_responses.py
--rw-rw-r--   0 james     (1000) james     (1000)     1127 2023-04-11 12:55:38.000000 cgiw-0.1.5/tests/test_run.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-09 13:29:28.177688 cgiw-0.1.6/
+-rw-rw-r--   0 james     (1000) james     (1000)    35149 2023-01-05 15:28:28.000000 cgiw-0.1.6/LICENSE
+-rw-rw-r--   0 james     (1000) james     (1000)     1629 2023-05-09 13:29:28.177688 cgiw-0.1.6/PKG-INFO
+-rw-rw-r--   0 james     (1000) james     (1000)     1117 2023-01-22 20:57:29.000000 cgiw-0.1.6/README.md
+-rw-rw-r--   0 james     (1000) james     (1000)      584 2023-05-09 13:28:52.000000 cgiw-0.1.6/pyproject.toml
+-rw-rw-r--   0 james     (1000) james     (1000)       38 2023-05-09 13:29:28.177688 cgiw-0.1.6/setup.cfg
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-09 13:29:28.169687 cgiw-0.1.6/src/
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-09 13:29:28.173687 cgiw-0.1.6/src/cgiw/
+-rw-rw-r--   0 james     (1000) james     (1000)       21 2023-01-16 23:30:07.000000 cgiw-0.1.6/src/cgiw/__init__.py
+-rw-rw-r--   0 james     (1000) james     (1000)      238 2023-01-22 20:04:01.000000 cgiw-0.1.6/src/cgiw/composers.py
+-rw-rw-r--   0 james     (1000) james     (1000)      872 2023-01-22 20:45:17.000000 cgiw-0.1.6/src/cgiw/decorators.py
+-rw-rw-r--   0 james     (1000) james     (1000)      438 2023-04-11 12:49:00.000000 cgiw-0.1.6/src/cgiw/exceptions.py
+-rw-rw-r--   0 james     (1000) james     (1000)      824 2023-05-09 13:28:44.000000 cgiw-0.1.6/src/cgiw/handler.py
+-rw-rw-r--   0 james     (1000) james     (1000)      420 2023-05-09 13:23:05.000000 cgiw-0.1.6/src/cgiw/logger.py
+-rw-rw-r--   0 james     (1000) james     (1000)     1364 2023-04-11 13:07:34.000000 cgiw-0.1.6/src/cgiw/parsers.py
+-rw-rw-r--   0 james     (1000) james     (1000)      581 2023-02-24 22:19:27.000000 cgiw-0.1.6/src/cgiw/responses.py
+-rw-rw-r--   0 james     (1000) james     (1000)      749 2023-04-11 12:44:30.000000 cgiw-0.1.6/src/cgiw/run.py
+-rw-rw-r--   0 james     (1000) james     (1000)      516 2023-01-22 20:49:49.000000 cgiw-0.1.6/src/cgiw/types.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-09 13:29:28.173687 cgiw-0.1.6/src/cgiw.egg-info/
+-rw-rw-r--   0 james     (1000) james     (1000)     1629 2023-05-09 13:29:28.000000 cgiw-0.1.6/src/cgiw.egg-info/PKG-INFO
+-rw-rw-r--   0 james     (1000) james     (1000)      499 2023-05-09 13:29:28.000000 cgiw-0.1.6/src/cgiw.egg-info/SOURCES.txt
+-rw-rw-r--   0 james     (1000) james     (1000)        1 2023-05-09 13:29:28.000000 cgiw-0.1.6/src/cgiw.egg-info/dependency_links.txt
+-rw-rw-r--   0 james     (1000) james     (1000)        5 2023-05-09 13:29:28.000000 cgiw-0.1.6/src/cgiw.egg-info/top_level.txt
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-09 13:29:28.177688 cgiw-0.1.6/tests/
+-rw-rw-r--   0 james     (1000) james     (1000)      529 2023-01-22 20:02:27.000000 cgiw-0.1.6/tests/test_composers.py
+-rw-rw-r--   0 james     (1000) james     (1000)     1054 2023-04-11 13:03:07.000000 cgiw-0.1.6/tests/test_decorators.py
+-rw-rw-r--   0 james     (1000) james     (1000)      876 2023-04-11 13:04:06.000000 cgiw-0.1.6/tests/test_handler.py
+-rw-rw-r--   0 james     (1000) james     (1000)     1033 2023-01-09 23:56:09.000000 cgiw-0.1.6/tests/test_parsers.py
+-rw-rw-r--   0 james     (1000) james     (1000)      700 2023-01-22 20:49:00.000000 cgiw-0.1.6/tests/test_responses.py
+-rw-rw-r--   0 james     (1000) james     (1000)     1127 2023-04-11 12:55:38.000000 cgiw-0.1.6/tests/test_run.py
```

### Comparing `cgiw-0.1.5/LICENSE` & `cgiw-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.5/PKG-INFO` & `cgiw-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgiw
-Version: 0.1.5
+Version: 0.1.6
 Summary: A framework for building python cgi scripts
 Author-email: James Rao <jamesnarayanrao@gmail.com>
 Project-URL: Homepage, https://github.com/JamesRao98/cgiw
 Project-URL: Bug Tracker, https://github.com/JamesRao98/cgiw/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cgiw-0.1.5/README.md` & `cgiw-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.5/pyproject.toml` & `cgiw-0.1.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cgiw"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="James Rao", email="jamesnarayanrao@gmail.com" },
 ]
 description = "A framework for building python cgi scripts"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `cgiw-0.1.5/src/cgiw/decorators.py` & `cgiw-0.1.6/src/cgiw/decorators.py`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.5/src/cgiw/handler.py` & `cgiw-0.1.6/src/cgiw/handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Optional, Any
+from traceback import format_exc
 
 from .types import QueryType, HeadersType, GetHandlerType, PostHandlerType, ReturnType
 from .exceptions import ApiException
 from .logger import log
 
 
 def handle(method: str, query: QueryType, headers: HeadersType, body: Optional[Any] = None, get: Optional[GetHandlerType] = None, post: Optional[PostHandlerType] = None) -> ReturnType:
@@ -10,11 +11,11 @@
         if method == 'POST' and post:
             return post(query, headers, body)
         elif method == 'GET' and get:
             return get(query, headers)
     except ApiException as e:
         raise e
     except Exception as e:
-        log(str(e))
+        log(format_exc())
         raise ApiException(500, 'Internal Service Error', message='An Unknown Error Has Occurred')
 
     return ({'Status': '405 Method Not Allowed'}, '')
```

### Comparing `cgiw-0.1.5/src/cgiw/parsers.py` & `cgiw-0.1.6/src/cgiw/parsers.py`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.5/src/cgiw/responses.py` & `cgiw-0.1.6/src/cgiw/responses.py`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.5/src/cgiw/run.py` & `cgiw-0.1.6/src/cgiw/run.py`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.5/src/cgiw/types.py` & `cgiw-0.1.6/src/cgiw/types.py`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.5/src/cgiw.egg-info/PKG-INFO` & `cgiw-0.1.6/src/cgiw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgiw
-Version: 0.1.5
+Version: 0.1.6
 Summary: A framework for building python cgi scripts
 Author-email: James Rao <jamesnarayanrao@gmail.com>
 Project-URL: Homepage, https://github.com/JamesRao98/cgiw
 Project-URL: Bug Tracker, https://github.com/JamesRao98/cgiw/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cgiw-0.1.5/tests/test_composers.py` & `cgiw-0.1.6/tests/test_composers.py`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.5/tests/test_decorators.py` & `cgiw-0.1.6/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.5/tests/test_handler.py` & `cgiw-0.1.6/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.5/tests/test_parsers.py` & `cgiw-0.1.6/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.5/tests/test_responses.py` & `cgiw-0.1.6/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.5/tests/test_run.py` & `cgiw-0.1.6/tests/test_run.py`

 * *Files identical despite different names*

