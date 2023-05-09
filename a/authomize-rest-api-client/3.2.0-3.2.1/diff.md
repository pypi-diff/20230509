# Comparing `tmp/authomize-rest-api-client-3.2.0.tar.gz` & `tmp/authomize-rest-api-client-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-3.2.0.tar", last modified: Mon May  1 08:34:45 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-3.2.1.tar", last modified: Tue May  9 05:17:30 2023, max compression
```

## Comparing `authomize-rest-api-client-3.2.0.tar` & `authomize-rest-api-client-3.2.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2160 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2040 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10105 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    12633 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    73614 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24531 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   185721 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64932 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-01 08:34:45.000000 authomize-rest-api-client-3.2.0/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-05-01 08:34:45.000000 authomize-rest-api-client-3.2.0/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 08:34:45.000000 authomize-rest-api-client-3.2.0/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      216 2023-05-01 08:34:45.000000 authomize-rest-api-client-3.2.0/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-01 08:34:45.000000 authomize-rest-api-client-3.2.0/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1163 2023-05-01 08:34:44.000000 authomize-rest-api-client-3.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.110172 authomize-rest-api-client-3.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-09 05:17:30.110172 authomize-rest-api-client-3.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2160 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.106172 authomize-rest-api-client-3.2.1/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.106172 authomize-rest-api-client-3.2.1/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.106172 authomize-rest-api-client-3.2.1/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10105 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    12633 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.106172 authomize-rest-api-client-3.2.1/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.106172 authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.106172 authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    73614 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.106172 authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24531 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.106172 authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.106172 authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   185721 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.110172 authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64932 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.110172 authomize-rest-api-client-3.2.1/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-09 05:17:30.000000 authomize-rest-api-client-3.2.1/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-05-09 05:17:30.000000 authomize-rest-api-client-3.2.1/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 05:17:30.000000 authomize-rest-api-client-3.2.1/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      216 2023-05-09 05:17:30.000000 authomize-rest-api-client-3.2.1/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-09 05:17:30.000000 authomize-rest-api-client-3.2.1/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-05-09 05:17:30.110172 authomize-rest-api-client-3.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1163 2023-05-09 05:17:28.000000 authomize-rest-api-client-3.2.1/setup.py
```

### Comparing `authomize-rest-api-client-3.2.0/LICENSE.txt` & `authomize-rest-api-client-3.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.0/README.md` & `authomize-rest-api-client-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.0/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-3.2.1/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.0/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-3.2.1/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.0/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-3.2.1/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.0/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-3.2.1/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.0/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-3.2.1/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.0/setup.py` & `authomize-rest-api-client-3.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='3.2.0',
+        version='3.2.1',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

