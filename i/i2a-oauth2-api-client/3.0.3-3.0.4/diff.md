# Comparing `tmp/i2a_oauth2_api_client-3.0.3.tar.gz` & `tmp/i2a_oauth2_api_client-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/bartlomiej/workspace/i2a-oauth-sdk/python_sdk/dist/.tmp-taf80yf5/i2a_oauth2_api_client-3.0.3.tar", last modified: Thu Apr 27 14:09:47 2023, max compression
+gzip compressed data, was "i2a_oauth2_api_client-3.0.4.tar", last modified: Tue May  9 10:59:48 2023, max compression
```

## Comparing `i2a_oauth2_api_client-3.0.3.tar` & `i2a_oauth2_api_client-3.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-04-27 14:09:47.313366 i2a_oauth2_api_client-3.0.3/
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1061 2023-03-29 13:29:15.000000 i2a_oauth2_api_client-3.0.3/LICENSE.txt
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       32 2023-04-27 14:08:50.000000 i2a_oauth2_api_client-3.0.3/MANIFEST.in
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      818 2023-04-27 14:09:47.313366 i2a_oauth2_api_client-3.0.3/PKG-INFO
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      433 2023-03-29 13:29:15.000000 i2a_oauth2_api_client-3.0.3/README.md
-drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-04-27 14:09:47.313366 i2a_oauth2_api_client-3.0.3/i2a_oauth2_api_client/
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-03-29 13:29:15.000000 i2a_oauth2_api_client-3.0.3/i2a_oauth2_api_client/__init__.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)    23257 2023-04-25 12:18:20.000000 i2a_oauth2_api_client-3.0.3/i2a_oauth2_api_client/client.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       73 2023-03-29 13:29:15.000000 i2a_oauth2_api_client-3.0.3/i2a_oauth2_api_client/enums.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      270 2023-04-21 15:04:34.000000 i2a_oauth2_api_client-3.0.3/i2a_oauth2_api_client/exceptions.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      936 2023-04-25 14:11:11.000000 i2a_oauth2_api_client-3.0.3/i2a_oauth2_api_client/types.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1050 2023-04-13 10:07:54.000000 i2a_oauth2_api_client-3.0.3/i2a_oauth2_api_client/validators.py
-drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-04-27 14:09:47.313366 i2a_oauth2_api_client-3.0.3/i2a_oauth2_api_client.egg-info/
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      818 2023-04-27 14:09:47.000000 i2a_oauth2_api_client-3.0.3/i2a_oauth2_api_client.egg-info/PKG-INFO
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      466 2023-04-27 14:09:47.000000 i2a_oauth2_api_client-3.0.3/i2a_oauth2_api_client.egg-info/SOURCES.txt
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        1 2023-04-27 14:09:47.000000 i2a_oauth2_api_client-3.0.3/i2a_oauth2_api_client.egg-info/dependency_links.txt
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       17 2023-04-27 14:09:47.000000 i2a_oauth2_api_client-3.0.3/i2a_oauth2_api_client.egg-info/requires.txt
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       28 2023-04-27 14:09:47.000000 i2a_oauth2_api_client-3.0.3/i2a_oauth2_api_client.egg-info/top_level.txt
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       38 2023-04-27 14:09:47.313366 i2a_oauth2_api_client-3.0.3/setup.cfg
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      759 2023-04-27 14:09:07.000000 i2a_oauth2_api_client-3.0.3/setup.py
+drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-05-09 10:59:48.814412 i2a_oauth2_api_client-3.0.4/
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1061 2023-03-29 13:29:15.000000 i2a_oauth2_api_client-3.0.4/LICENSE.txt
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       32 2023-04-27 14:08:50.000000 i2a_oauth2_api_client-3.0.4/MANIFEST.in
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      818 2023-05-09 10:59:48.814412 i2a_oauth2_api_client-3.0.4/PKG-INFO
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      433 2023-03-29 13:29:15.000000 i2a_oauth2_api_client-3.0.4/README.md
+drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-05-09 10:59:48.814412 i2a_oauth2_api_client-3.0.4/i2a_oauth2_api_client/
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-03-29 13:29:15.000000 i2a_oauth2_api_client-3.0.4/i2a_oauth2_api_client/__init__.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)    23331 2023-05-09 10:53:12.000000 i2a_oauth2_api_client-3.0.4/i2a_oauth2_api_client/client.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       73 2023-03-29 13:29:15.000000 i2a_oauth2_api_client-3.0.4/i2a_oauth2_api_client/enums.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      270 2023-04-21 15:04:34.000000 i2a_oauth2_api_client-3.0.4/i2a_oauth2_api_client/exceptions.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      936 2023-04-25 14:11:11.000000 i2a_oauth2_api_client-3.0.4/i2a_oauth2_api_client/types.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1050 2023-04-13 10:07:54.000000 i2a_oauth2_api_client-3.0.4/i2a_oauth2_api_client/validators.py
+drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-05-09 10:59:48.814412 i2a_oauth2_api_client-3.0.4/i2a_oauth2_api_client.egg-info/
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      818 2023-05-09 10:59:48.000000 i2a_oauth2_api_client-3.0.4/i2a_oauth2_api_client.egg-info/PKG-INFO
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      466 2023-05-09 10:59:48.000000 i2a_oauth2_api_client-3.0.4/i2a_oauth2_api_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        1 2023-05-09 10:59:48.000000 i2a_oauth2_api_client-3.0.4/i2a_oauth2_api_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       17 2023-05-09 10:59:48.000000 i2a_oauth2_api_client-3.0.4/i2a_oauth2_api_client.egg-info/requires.txt
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       28 2023-05-09 10:59:48.000000 i2a_oauth2_api_client-3.0.4/i2a_oauth2_api_client.egg-info/top_level.txt
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       38 2023-05-09 10:59:48.814412 i2a_oauth2_api_client-3.0.4/setup.cfg
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      759 2023-05-09 10:59:00.000000 i2a_oauth2_api_client-3.0.4/setup.py
```

### Comparing `i2a_oauth2_api_client-3.0.3/LICENSE.txt` & `i2a_oauth2_api_client-3.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `i2a_oauth2_api_client-3.0.3/PKG-INFO` & `i2a_oauth2_api_client-3.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2a_oauth2_api_client
-Version: 3.0.3
+Version: 3.0.4
 Summary: Sdk for i2a oauth2 api
 Download-URL: https://pypi.org/project/i2a_oauth2_api_client/
 Author: i2a Solutions Inc.
 Author-email: msyta@i2asolutions.com
 License: MIT
 Keywords: I2A Oauth2 Client,I2A Oauth2 Api,I2A Oauth2,Python 3,I2A Oauth2 Api SDK
 Description-Content-Type: text/markdown
```

### Comparing `i2a_oauth2_api_client-3.0.3/i2a_oauth2_api_client/client.py` & `i2a_oauth2_api_client-3.0.4/i2a_oauth2_api_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 import os
-from urllib.parse import urljoin
+from urllib.parse import urljoin, quote
 
 from i2a_oauth2_api_client.exceptions import I2AOauth2ClientException
 from i2a_oauth2_api_client.enums import Environment
 from i2a_oauth2_api_client.types import MeData, TokenData, Page, AppLessS2SI2IdentityData
 from i2a_oauth2_api_client.validators import client_call, server_to_server_call, app_less_server_to_server_call
 
 
@@ -458,16 +458,16 @@
 
     @app_less_server_to_server_call
     def app_less_server_to_server_get_user_identity_details(
         self, username: str, clients_ids: list[str], groups_identifiers: list[str]
     ) -> AppLessS2SI2IdentityData:
         url = self._get_full_url(f'server-to-server/app-less/users_identities/{username}/')
         response = requests.get(url, headers=self.app_less_server_to_server_headers, params={
-            "clients_ids": clients_ids,
-            "groups_identifiers": groups_identifiers
+            "applications_clients_ids": ','.join(clients_ids),
+            "groups_identifiers": ','.join(groups_identifiers),
         })
         if response.status_code == 200:
             return response.json()
         elif response.status_code == 500:
             raise I2AOauth2ClientException(
                 f'App less Server to server get application user group attempt at {url} has failed for unknown reason.'
             )
@@ -477,16 +477,16 @@
     @app_less_server_to_server_call
     def app_less_server_to_server_get_user_identity_list(
         self, clients_ids: list[str], groups_identifiers: list[str],
         page: int = 1, page_size: int = 25
     ) -> Page[AppLessS2SI2IdentityData]:
         url = self._get_full_url(f'server-to-server/app-less/users_identities/')
         response = requests.get(url, headers=self.app_less_server_to_server_headers, params={
-            "clients_ids": clients_ids,
-            "groups_identifiers": groups_identifiers,
+            "applications_clients_ids": ','.join(clients_ids),
+            "groups_identifiers": ','.join(groups_identifiers),
             "page": page,
             "page_size": page_size
         })
         if response.status_code == 200:
             return response.json()
         elif response.status_code == 500:
             raise I2AOauth2ClientException(
```

### Comparing `i2a_oauth2_api_client-3.0.3/i2a_oauth2_api_client/types.py` & `i2a_oauth2_api_client-3.0.4/i2a_oauth2_api_client/types.py`

 * *Files identical despite different names*

### Comparing `i2a_oauth2_api_client-3.0.3/i2a_oauth2_api_client/validators.py` & `i2a_oauth2_api_client-3.0.4/i2a_oauth2_api_client/validators.py`

 * *Files identical despite different names*

### Comparing `i2a_oauth2_api_client-3.0.3/i2a_oauth2_api_client.egg-info/PKG-INFO` & `i2a_oauth2_api_client-3.0.4/i2a_oauth2_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2a-oauth2-api-client
-Version: 3.0.3
+Version: 3.0.4
 Summary: Sdk for i2a oauth2 api
 Download-URL: https://pypi.org/project/i2a_oauth2_api_client/
 Author: i2a Solutions Inc.
 Author-email: msyta@i2asolutions.com
 License: MIT
 Keywords: I2A Oauth2 Client,I2A Oauth2 Api,I2A Oauth2,Python 3,I2A Oauth2 Api SDK
 Description-Content-Type: text/markdown
```

### Comparing `i2a_oauth2_api_client-3.0.3/setup.py` & `i2a_oauth2_api_client-3.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='i2a_oauth2_api_client',
-    version='3.0.3',
+    version='3.0.4',
     description='Sdk for i2a oauth2 api',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='i2a Solutions Inc.',
     author_email='msyta@i2asolutions.com',
```

