# Comparing `tmp/serverless-sdk-0.4.6.tar.gz` & `tmp/serverless-sdk-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-tii8obn0/serverless-sdk-0.4.6.tar", last modified: Fri May  5 17:09:37 2023, max compression
+gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-7l1hlh1m/serverless-sdk-0.4.7.tar", last modified: Tue May  9 14:21:54 2023, max compression
```

## Comparing `serverless-sdk-0.4.6.tar` & `serverless-sdk-0.4.7.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/serverless_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/serverless_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/serverless_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/serverless_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/serverless_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/serverless_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/serverless_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/serverless_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/sls_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/sls_sdk/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/error_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)    16308 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/notice.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/stack_trace_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/warning_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/tests/test_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/tests/test_sdk_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/tests/test_thread_safety.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/serverless_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/serverless_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/serverless_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/serverless_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/serverless_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/serverless_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/serverless_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/serverless_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/sls_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/sls_sdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/error_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/notice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/stack_trace_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/lib/warning_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/sls_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:21:54.000000 serverless-sdk-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/tests/test_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/tests/test_sdk_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-05-09 14:21:22.000000 serverless-sdk-0.4.7/tests/test_thread_safety.py
```

### Comparing `serverless-sdk-0.4.6/PKG-INFO` & `serverless-sdk-0.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.4.6
+Version: 0.4.7
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `serverless-sdk-0.4.6/README.md` & `serverless-sdk-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.6/pyproject.toml` & `serverless-sdk-0.4.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     "version",
 ]
 dependencies = [
     "backports.cached-property", # included in Python >=3.8
     "blinker>=1.5",
     "js-regex<1.1.0,>=1.0.1",
     "typing-extensions>=4.4", # included in Python 3.8 - 3.11
-    "wrapt~=1.15.0",
 ]
 [project.optional-dependencies]
 tests = [
     "aiohttp>=3.8.4",
     "black>=22.12",
     "flask>=2.2.3",
     "importlib_metadata>=5.2", # included in Python >=3.8
@@ -65,14 +64,10 @@
 
 [tool.mypy]
 disable_error_code = "override,assignment,arg-type"
 exclude = [
     '^tests/',
 ]
 
-[[tool.mypy.overrides]]
-module = "wrapt"
-ignore_missing_imports = true
-
 [tool.ruff]
 ignore = ["F401", "E722"]
 #fix = true
```

### Comparing `serverless-sdk-0.4.6/serverless_sdk.egg-info/PKG-INFO` & `serverless-sdk-0.4.7/serverless_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.4.6
+Version: 0.4.7
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `serverless-sdk-0.4.6/serverless_sdk.egg-info/SOURCES.txt` & `serverless-sdk-0.4.7/serverless_sdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -27,10 +27,11 @@
 sls_sdk/lib/warning.py
 sls_sdk/lib/warning_captured_event.py
 sls_sdk/lib/instrumentation/__init__.py
 sls_sdk/lib/instrumentation/flask.py
 sls_sdk/lib/instrumentation/http.py
 sls_sdk/lib/instrumentation/import_hook.py
 sls_sdk/lib/instrumentation/logging.py
+sls_sdk/lib/instrumentation/wrapper.py
 tests/test_sdk.py
 tests/test_sdk_alias.py
 tests/test_thread_safety.py
```

### Comparing `serverless-sdk-0.4.6/sls_sdk/__init__.py` & `serverless-sdk-0.4.7/sls_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.6/sls_sdk/base.py` & `serverless-sdk-0.4.7/sls_sdk/base.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.6/sls_sdk/exceptions.py` & `serverless-sdk-0.4.7/sls_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.6/sls_sdk/lib/captured_event.py` & `serverless-sdk-0.4.7/sls_sdk/lib/captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.6/sls_sdk/lib/emitter.py` & `serverless-sdk-0.4.7/sls_sdk/lib/emitter.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.6/sls_sdk/lib/error.py` & `serverless-sdk-0.4.7/sls_sdk/lib/error.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.6/sls_sdk/lib/error_captured_event.py` & `serverless-sdk-0.4.7/sls_sdk/lib/error_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/flask.py` & `serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/flask.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/http.py` & `serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import contextvars
 import contextlib
 from urllib.parse import urlparse
 from urllib.parse import parse_qs
 from ..error import report as report_error
 from .import_hook import ImportHook
 import sls_sdk
-from wrapt import wrap_function_wrapper, ObjectProxy
+from .wrapper import replace_method
 import io
 from typing import Iterable
 
 SDK = sls_sdk.serverlessSdk
 _IGNORE_FOLLOWING_REQUEST = contextvars.ContextVar("ignore", default=False)
 
 
@@ -411,29 +411,25 @@
             if response_body:
                 trace_span.output = _decode_body(response_body)
         except Exception as ex:
             report_error(ex)
 
     def _install(self, module):
         self._module = module
-        wrap_function_wrapper(
+        replace_method(
             module.connectionpool.HTTPConnectionPool,
             self._target_method,
             self._patched_call,
         )
 
     def _uninstall(self, module):
         _wrapping_method = getattr(
             module.connectionpool.HTTPConnectionPool, self._target_method, None
         )
-        if (
-            _wrapping_method
-            and isinstance(_wrapping_method, ObjectProxy)
-            and hasattr(_wrapping_method, "__wrapped__")
-        ):
+        if hasattr(_wrapping_method, "__wrapped__"):
             setattr(
                 module.connectionpool.HTTPConnectionPool,
                 self._target_method,
                 _wrapping_method.__wrapped__,
             )
         self._module = None
```

### Comparing `serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/import_hook.py` & `serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/import_hook.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/logging.py` & `serverless-sdk-0.4.7/sls_sdk/lib/instrumentation/logging.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.6/sls_sdk/lib/name.py` & `serverless-sdk-0.4.7/sls_sdk/lib/name.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.6/sls_sdk/lib/stack_trace_string.py` & `serverless-sdk-0.4.7/sls_sdk/lib/stack_trace_string.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.6/sls_sdk/lib/tags.py` & `serverless-sdk-0.4.7/sls_sdk/lib/tags.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.6/sls_sdk/lib/trace.py` & `serverless-sdk-0.4.7/sls_sdk/lib/trace.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     PastSpanEndTime,
     FutureSpanEndTime,
 )
 from .emitter import event_emitter
 from .id import generate_id
 from .name import get_resource_name
 from .tags import Tags, convert_tags_to_protobuf
-from wrapt import wrap_function_wrapper
+from .instrumentation.wrapper import replace_method
 
 logger = logging.getLogger(__name__)
 
 
 __all__: Final[List[str]] = [
     "TraceSpan",
 ]
@@ -44,15 +44,15 @@
     # Implementation of item 2 in `resolve_current_span`
     def _thread_ctor_wrapper(actual_start, instance, args, kwargs):
         if not hasattr(instance, "_parent_span"):
             instance._parent_span = _CONTEXT.get() or root_span
         result = actual_start(*args, **kwargs)
         return result
 
-    wrap_function_wrapper(threading_module.Thread, "start", _thread_ctor_wrapper)
+    replace_method(threading_module.Thread, "start", _thread_ctor_wrapper)
 
 
 _import_hook = ImportHook("threading")
 _import_hook.enable(_install_thread_hook)
 
 
 class TraceSpan:
```

### Comparing `serverless-sdk-0.4.6/sls_sdk/lib/warning.py` & `serverless-sdk-0.4.7/sls_sdk/lib/warning.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.6/sls_sdk/lib/warning_captured_event.py` & `serverless-sdk-0.4.7/sls_sdk/lib/warning_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.6/tests/test_sdk.py` & `serverless-sdk-0.4.7/tests/test_sdk.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.6/tests/test_thread_safety.py` & `serverless-sdk-0.4.7/tests/test_thread_safety.py`

 * *Files identical despite different names*

