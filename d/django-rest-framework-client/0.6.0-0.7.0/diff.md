# Comparing `tmp/django-rest-framework-client-0.6.0.tar.gz` & `tmp/django-rest-framework-client-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-rest-framework-client-0.6.0.tar", last modified: Sun Oct 30 19:00:36 2022, max compression
+gzip compressed data, was "django-rest-framework-client-0.7.0.tar", last modified: Tue May  9 04:02:04 2023, max compression
```

## Comparing `django-rest-framework-client-0.6.0.tar` & `django-rest-framework-client-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 19:00:36.357188 django-rest-framework-client-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-10-30 19:00:29.000000 django-rest-framework-client-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-10-30 19:00:29.000000 django-rest-framework-client-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-10-30 19:00:29.000000 django-rest-framework-client-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6016 2022-10-30 19:00:36.357188 django-rest-framework-client-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5023 2022-10-30 19:00:29.000000 django-rest-framework-client-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 19:00:36.357188 django-rest-framework-client-0.6.0/django_rest_framework_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6016 2022-10-30 19:00:36.000000 django-rest-framework-client-0.6.0/django_rest_framework_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-10-30 19:00:36.000000 django-rest-framework-client-0.6.0/django_rest_framework_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-30 19:00:36.000000 django-rest-framework-client-0.6.0/django_rest_framework_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-30 19:00:36.000000 django-rest-framework-client-0.6.0/django_rest_framework_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-30 19:00:36.000000 django-rest-framework-client-0.6.0/django_rest_framework_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-30 19:00:36.000000 django-rest-framework-client-0.6.0/django_rest_framework_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 19:00:36.357188 django-rest-framework-client-0.6.0/drf_client/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-30 19:00:29.000000 django-rest-framework-client-0.6.0/drf_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10469 2022-10-30 19:00:29.000000 django-rest-framework-client-0.6.0/drf_client/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-10-30 19:00:29.000000 django-rest-framework-client-0.6.0/drf_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 19:00:36.357188 django-rest-framework-client-0.6.0/drf_client/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)     3828 2022-10-30 19:00:29.000000 django-rest-framework-client-0.6.0/drf_client/helpers/base_main.py
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-30 19:00:36.357188 django-rest-framework-client-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-10-30 19:00:29.000000 django-rest-framework-client-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:02:04.730999 django-rest-framework-client-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-09 04:01:49.000000 django-rest-framework-client-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-09 04:01:49.000000 django-rest-framework-client-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-09 04:01:49.000000 django-rest-framework-client-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-05-09 04:02:04.730999 django-rest-framework-client-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-09 04:01:49.000000 django-rest-framework-client-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:02:04.726999 django-rest-framework-client-0.7.0/django_rest_framework_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-05-09 04:02:04.000000 django-rest-framework-client-0.7.0/django_rest_framework_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-09 04:02:04.000000 django-rest-framework-client-0.7.0/django_rest_framework_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 04:02:04.000000 django-rest-framework-client-0.7.0/django_rest_framework_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 04:02:04.000000 django-rest-framework-client-0.7.0/django_rest_framework_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 04:02:04.000000 django-rest-framework-client-0.7.0/django_rest_framework_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 04:02:04.000000 django-rest-framework-client-0.7.0/django_rest_framework_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:02:04.726999 django-rest-framework-client-0.7.0/drf_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 04:01:49.000000 django-rest-framework-client-0.7.0/drf_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-05-09 04:01:49.000000 django-rest-framework-client-0.7.0/drf_client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-09 04:01:49.000000 django-rest-framework-client-0.7.0/drf_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:02:04.730999 django-rest-framework-client-0.7.0/drf_client/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-09 04:01:49.000000 django-rest-framework-client-0.7.0/drf_client/helpers/base_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-09 04:02:04.730999 django-rest-framework-client-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-09 04:01:49.000000 django-rest-framework-client-0.7.0/setup.py
```

### Comparing `django-rest-framework-client-0.6.0/CHANGELOG.md` & `django-rest-framework-client-0.7.0/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+### v0.7.0 (2023-05-08)
+
+  * Migrated to Python 3.10, Python 2 is not supported anymore
+  * Resource class methods respect additional `**kwargs` and `extra_headers` parameters and pass them on to the underlying `requests` methods
+  * Fix to support `http://` schema in the server url
+
 ### v0.6.0 (2022-10-30)
 
   * Add USE_DASHES option to automatically replace underscores ("_") with dashes ("-")
   * Refactor to pass options to Resource class
 
 ### v0.5.0 (2022-05-16)
```

### Comparing `django-rest-framework-client-0.6.0/LICENSE` & `django-rest-framework-client-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-rest-framework-client-0.6.0/PKG-INFO` & `django-rest-framework-client-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rest-framework-client
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python client for a DjangoRestFramework based web site
 Home-page: https://github.com/dkarchmer/django-rest-framework-client
 Author: David Karchmer
 Author-email: dkarchmer@gmail.com
 License: MIT
 Keywords: django,djangorestframework,drf,rest-client
 Classifier: Programming Language :: Python
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.10,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Rest Framework Python API Package
 
 [![Build Status](https://travis-ci.org/dkarchmer/django-rest-framework-client.svg?branch=master)](https://travis-ci.org/dkarchmer/django-rest-framework-client)
 [![PyPI version](https://img.shields.io/pypi/v/django-rest-framework-client.svg)](https://pypi.python.org/pypi/django-rest-framework-client)
@@ -195,21 +195,14 @@
 
 ```bash
 python3 -m venv .virtualenv/drf_client
 source .virtualenv/drf_client/bin/activate
 pip install -r requirements-test.txt
 pip install -e .
 
-coverage run --source=iotile_cloud setup.py test
-coverage report -m
-```
-
-You can also use py.test:
-
-```bash
 py.test
 ```
 
 ## CI Deployment
 
 1. Update `setup.py` with new version
 2. Update `CHANGELOG.md` with description of new version
```

### Comparing `django-rest-framework-client-0.6.0/README.md` & `django-rest-framework-client-0.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -171,21 +171,14 @@
 
 ```bash
 python3 -m venv .virtualenv/drf_client
 source .virtualenv/drf_client/bin/activate
 pip install -r requirements-test.txt
 pip install -e .
 
-coverage run --source=iotile_cloud setup.py test
-coverage report -m
-```
-
-You can also use py.test:
-
-```bash
 py.test
 ```
 
 ## CI Deployment
 
 1. Update `setup.py` with new version
 2. Update `CHANGELOG.md` with description of new version
```

### Comparing `django-rest-framework-client-0.6.0/django_rest_framework_client.egg-info/PKG-INFO` & `django-rest-framework-client-0.7.0/django_rest_framework_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rest-framework-client
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python client for a DjangoRestFramework based web site
 Home-page: https://github.com/dkarchmer/django-rest-framework-client
 Author: David Karchmer
 Author-email: dkarchmer@gmail.com
 License: MIT
 Keywords: django,djangorestframework,drf,rest-client
 Classifier: Programming Language :: Python
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.10,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Rest Framework Python API Package
 
 [![Build Status](https://travis-ci.org/dkarchmer/django-rest-framework-client.svg?branch=master)](https://travis-ci.org/dkarchmer/django-rest-framework-client)
 [![PyPI version](https://img.shields.io/pypi/v/django-rest-framework-client.svg)](https://pypi.python.org/pypi/django-rest-framework-client)
@@ -195,21 +195,14 @@
 
 ```bash
 python3 -m venv .virtualenv/drf_client
 source .virtualenv/drf_client/bin/activate
 pip install -r requirements-test.txt
 pip install -e .
 
-coverage run --source=iotile_cloud setup.py test
-coverage report -m
-```
-
-You can also use py.test:
-
-```bash
 py.test
 ```
 
 ## CI Deployment
 
 1. Update `setup.py` with new version
 2. Update `CHANGELOG.md` with description of new version
```

### Comparing `django-rest-framework-client-0.6.0/drf_client/connection.py` & `django-rest-framework-client-0.7.0/drf_client/connection.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,15 +44,15 @@
        'LOGOUT': 'auth/logout/',
        'USE_DASHES': False,
     }
 
 logger = logging.getLogger(__name__)
 
 
-class RestResource(object):
+class RestResource:
     """
     Resource provides the main functionality behind a Django Rest Framework based API. It handles the
     attribute -> url, kwarg -> query param, and other related behind the scenes
     python to HTTP transformations. It's goal is to represent a single resource
     which may or may not have children.
     """
     _store = {}
@@ -160,77 +160,72 @@
 
     def url(self, args=None):
         url = self._store["base_url"]
         if args:
             url += '?{0}'.format(args)
         return url
 
-    def _get_header(self):
+    def _get_headers(self):
         headers = DEFAULT_HEADERS
         if self._store['use_token']:
             if not "token" in self._store:
                 raise RestBaseException('No Token')
             authorization_str = self._options['TOKEN_FORMAT'].format(token=self._store["token"])
             headers['Authorization'] = authorization_str
 
         return headers
 
-    def get(self, **kwargs):
+    def get(self, extra_headers: dict = None, **kwargs):
         args = None
         if 'extra' in kwargs:
             args = kwargs['extra']
-        resp = requests.get(self.url(args), headers=self._get_header())
+        headers = self._get_headers() | extra_headers if extra_headers else self._get_headers()
+
+        resp = requests.get(self.url(args), headers=headers)
         return self._process_response(resp)
 
-    def post(self, data=None, **kwargs):
-        if data:
-            payload = json.dumps(data)
-        else:
-            payload = None
+    def post(self, data: dict = None, extra_headers: dict = None, **kwargs):
+        payload = json.dumps(data) if data and "files" not in kwargs else data
+        headers = self._get_headers() | extra_headers if extra_headers else self._get_headers()
 
-        resp = requests.post(self.url(), data=payload, headers=self._get_header())
+        resp = requests.post(self.url(), data=payload, headers=headers, **kwargs)
         return self._process_response(resp)
 
-    def patch(self, data=None, **kwargs):
-        if data:
-            payload = json.dumps(data)
-        else:
-            payload = None
+    def patch(self, data=None, extra_headers: dict = None, **kwargs):
+        payload = json.dumps(data) if data and "files" not in kwargs else data
+        headers = self._get_headers() | extra_headers if extra_headers else self._get_headers()
 
-        resp = requests.patch(self.url(), data=payload, headers=self._get_header())
+        resp = requests.patch(self.url(), data=payload, headers=headers, **kwargs)
         return self._process_response(resp)
 
-    def put(self, data=None, **kwargs):
-        if data:
-            payload = json.dumps(data)
-        else:
-            payload = None
+    def put(self, data=None, extra_headers: dict = None, **kwargs):
+        payload = json.dumps(data) if data and "files" not in kwargs else data
+        headers = self._get_headers() | extra_headers if extra_headers else self._get_headers()
 
-        resp = requests.put(self.url(), data=payload, headers=self._get_header())
+        resp = requests.put(self.url(), data=payload, headers=headers, **kwargs)
         return self._process_response(resp)
 
-    def delete(self, data=None, **kwargs):
-        if data:
-            payload = json.dumps(data)
-        else:
-            payload = None
+    def delete(self, data=None, extra_headers: dict = None, **kwargs):
+        payload = json.dumps(data) if data and "files" not in kwargs else data
+        headers = self._get_headers() | extra_headers if extra_headers else self._get_headers()
 
-        resp = requests.delete(self.url(), data=payload, headers=self._get_header())
+        resp = requests.delete(self.url(), data=payload, headers=headers, **kwargs)
         if 200 <= resp.status_code <= 299:
             if resp.status_code == 204:
                 return True
             else:
                 return True  # @@@ Should this really be True?
         else:
             return False
 
     def _get_resource(self, **kwargs):
         return self.__class__(**kwargs)
 
-class Api(object):
+
+class Api:
     token = None
     resource_class = RestResource
     use_token = True
     options = None
 
     def __init__(self, options):
         self.options = options
```

### Comparing `django-rest-framework-client-0.6.0/drf_client/exceptions.py` & `django-rest-framework-client-0.7.0/drf_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-client-0.6.0/drf_client/helpers/base_main.py` & `django-rest-framework-client-0.7.0/drf_client/helpers/base_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import sys
 import logging
 import argparse
 import getpass
 
+from urllib.parse import urlparse
+
 from drf_client.connection import Api as RestApi, DEFAULT_HEADERS
 from drf_client.exceptions import HttpClientError
 
 LOG = logging.getLogger(__name__)
 
 
-class BaseMain(object):
+class BaseMain:
     parser = None
     args = None
     api = None
     options = {
         'DOMAIN': None,
         'API_PREFIX': 'api/v1',
         'TOKEN_TYPE': 'jwt',
@@ -92,15 +94,15 @@
         """
         pass
 
     def get_domain(self) -> str:
         """
         Figure out server domain URL based on --server and --customer args
         """
-        if 'https://' not in self.args.server:
+        if not urlparse(self.args.server).scheme:
             return f'https://{self.args.server}'
         return self.args.server
 
     def login(self) -> bool:
         """
         Get password from user and login
         """
```

### Comparing `django-rest-framework-client-0.6.0/setup.py` & `django-rest-framework-client-0.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(name='django-rest-framework-client',
-    version='0.6.0',
+    version='0.7.0',
     description='Python client for a DjangoRestFramework based web site',
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/dkarchmer/django-rest-framework-client',
     author='David Karchmer',
     author_email="dkarchmer@gmail.com",
     license='MIT',
     packages=[
         'drf_client',
         'drf_client.helpers',
     ],
     install_requires=[
         'requests',
     ],
-    python_requires=">=3.8,<4",
+    python_requires=">=3.10,<4",
     keywords=["django", "djangorestframework", "drf", "rest-client",],
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

