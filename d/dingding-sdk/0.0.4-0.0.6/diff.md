# Comparing `tmp/dingding-sdk-0.0.4.tar.gz` & `tmp/dingding-sdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dingding-sdk-0.0.4.tar", last modified: Wed Jun 23 08:11:52 2021, max compression
+gzip compressed data, was "dingding-sdk-0.0.6.tar", last modified: Tue May  9 01:57:53 2023, max compression
```

## Comparing `dingding-sdk-0.0.4.tar` & `dingding-sdk-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,37 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-06-23 08:11:53.000000 dingding-sdk-0.0.4/
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-06-23 08:11:53.000000 dingding-sdk-0.0.4/dingding_sdk.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)        1 2021-06-23 08:11:52.000000 dingding-sdk-0.0.4/dingding_sdk.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      876 2021-06-23 08:11:52.000000 dingding-sdk-0.0.4/dingding_sdk.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)        9 2021-06-23 08:11:52.000000 dingding-sdk-0.0.4/dingding_sdk.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)      449 2021-06-23 08:11:52.000000 dingding-sdk-0.0.4/dingding_sdk.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)       15 2021-06-23 08:11:52.000000 dingding-sdk-0.0.4/dingding_sdk.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2021-06-22 06:24:47.000000 dingding-sdk-0.0.4/dingding_sdk.egg-info/zip-safe
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-06-23 08:11:53.000000 dingding-sdk-0.0.4/dingtalk/
--rwxrwxrwx   0 root         (0) root         (0)    18453 2021-06-23 06:59:46.000000 dingding-sdk-0.0.4/dingtalk/contact.py
--rwxrwxrwx   0 root         (0) root         (0)     2771 2021-06-23 03:40:27.000000 dingding-sdk-0.0.4/dingtalk/core.py
--rwxrwxrwx   0 root         (0) root         (0)      920 2021-06-23 03:27:45.000000 dingding-sdk-0.0.4/dingtalk/dingtalk.py
--rwxrwxrwx   0 root         (0) root         (0)      528 2021-06-23 01:36:35.000000 dingding-sdk-0.0.4/dingtalk/exceptions.py
--rwxrwxrwx   0 root         (0) root         (0)      707 2021-06-22 07:51:27.000000 dingding-sdk-0.0.4/dingtalk/message.py
--rwxrwxrwx   0 root         (0) root         (0)     2224 2021-06-23 03:17:01.000000 dingding-sdk-0.0.4/dingtalk/oauth.py
--rwxrwxrwx   0 root         (0) root         (0)      226 2021-06-23 06:29:36.000000 dingding-sdk-0.0.4/dingtalk/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      876 2021-06-23 08:11:53.000000 dingding-sdk-0.0.4/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       59 2021-06-18 00:50:35.000000 dingding-sdk-0.0.4/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2021-06-23 08:11:53.000000 dingding-sdk-0.0.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1448 2021-06-22 06:25:30.000000 dingding-sdk-0.0.4/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-06-23 08:11:53.000000 dingding-sdk-0.0.4/tests/
--rwxrwxrwx   0 root         (0) root         (0)     5584 2021-06-23 06:55:58.000000 dingding-sdk-0.0.4/tests/test_contact.py
--rwxrwxrwx   0 root         (0) root         (0)      648 2021-06-23 03:28:10.000000 dingding-sdk-0.0.4/tests/test_core.py
--rwxrwxrwx   0 root         (0) root         (0)      754 2021-06-23 03:28:18.000000 dingding-sdk-0.0.4/tests/test_message.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2021-06-18 01:15:56.000000 dingding-sdk-0.0.4/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:57:53.526119 dingding-sdk-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)      825 2023-05-09 01:57:53.526119 dingding-sdk-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-08 02:57:45.000000 dingding-sdk-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:57:53.522119 dingding-sdk-0.0.6/dingding_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      825 2023-05-09 01:57:52.000000 dingding-sdk-0.0.6/dingding_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      687 2023-05-09 01:57:53.000000 dingding-sdk-0.0.6/dingding_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 01:57:52.000000 dingding-sdk-0.0.6/dingding_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-09 01:57:53.000000 dingding-sdk-0.0.6/dingding_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-09 01:57:53.000000 dingding-sdk-0.0.6/dingding_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 02:57:45.000000 dingding-sdk-0.0.6/dingding_sdk.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:57:53.526119 dingding-sdk-0.0.6/dingtalk/
+-rw-r--r--   0 root         (0) root         (0)      226 2023-05-08 05:44:25.000000 dingding-sdk-0.0.6/dingtalk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18453 2023-05-08 13:32:50.000000 dingding-sdk-0.0.6/dingtalk/contact.py
+-rw-r--r--   0 root         (0) root         (0)     3812 2023-05-09 00:58:58.000000 dingding-sdk-0.0.6/dingtalk/core.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-05-09 00:37:27.000000 dingding-sdk-0.0.6/dingtalk/dingtalk.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-05-08 14:04:56.000000 dingding-sdk-0.0.6/dingtalk/document.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-05-08 14:36:30.000000 dingding-sdk-0.0.6/dingtalk/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-05-08 02:57:45.000000 dingding-sdk-0.0.6/dingtalk/hr.py
+-rw-r--r--   0 root         (0) root         (0)     2780 2023-05-08 02:57:45.000000 dingding-sdk-0.0.6/dingtalk/message.py
+-rw-r--r--   0 root         (0) root         (0)     2224 2023-05-08 02:57:45.000000 dingding-sdk-0.0.6/dingtalk/oauth.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-05-09 01:14:29.000000 dingding-sdk-0.0.6/dingtalk/robot.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2023-05-09 01:53:43.000000 dingding-sdk-0.0.6/dingtalk/session.py
+-rw-r--r--   0 root         (0) root         (0)      829 2023-05-08 15:00:28.000000 dingding-sdk-0.0.6/dingtalk/space.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-05-08 02:57:45.000000 dingding-sdk-0.0.6/dingtalk/workflow.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 01:57:53.530119 dingding-sdk-0.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-05-08 02:57:45.000000 dingding-sdk-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 01:57:53.526119 dingding-sdk-0.0.6/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 02:57:45.000000 dingding-sdk-0.0.6/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5584 2023-05-08 02:57:45.000000 dingding-sdk-0.0.6/tests/test_contact.py
+-rw-r--r--   0 root         (0) root         (0)      648 2023-05-08 02:57:45.000000 dingding-sdk-0.0.6/tests/test_core.py
+-rw-r--r--   0 root         (0) root         (0)      773 2023-05-08 03:41:13.000000 dingding-sdk-0.0.6/tests/test_document.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-05-08 02:57:45.000000 dingding-sdk-0.0.6/tests/test_hr.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-05-08 02:57:45.000000 dingding-sdk-0.0.6/tests/test_message.py
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-05-09 01:13:00.000000 dingding-sdk-0.0.6/tests/test_robot.py
+-rw-r--r--   0 root         (0) root         (0)      861 2023-05-09 01:49:34.000000 dingding-sdk-0.0.6/tests/test_session.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2023-05-08 14:05:59.000000 dingding-sdk-0.0.6/tests/test_space.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-05-08 02:57:45.000000 dingding-sdk-0.0.6/tests/test_workflow.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dingding-sdk-0.0.4/dingding_sdk.egg-info/PKG-INFO` & `dingding-sdk-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: dingding-sdk
-Version: 0.0.4
+Version: 0.0.6
 Summary: DingTalk Python SDK
 Home-page: https://github.com/jellyhappy/dingding-sdk
 Author: blackcat
 Author-email: kfx2007@163.com
 License: GNU
-Description: # DingTalk Python SDK
-        
-        author: Kevin Kong 
-        version: 0.0.1
-        
-        
 Keywords: dingding sdk
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Description-Content-Type: text/markdown
+
+# DingTalk Python SDK
+
+author: Kevin Kong 
+version: 0.0.1
+
+
+
```

### Comparing `dingding-sdk-0.0.4/dingtalk/contact.py` & `dingding-sdk-0.0.6/dingtalk/contact.py`

 * *Files identical despite different names*

### Comparing `dingding-sdk-0.0.4/dingtalk/core.py` & `dingding-sdk-0.0.6/dingtalk/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 # @Time    : 2021-06-18
 # @Author  : Kevin Kong (kfx2007@163.com)
 
 import requests
 from hmac import HMAC
 from hashlib import sha256
 from base64 import b64encode
-from .exceptions import DingTalkException
+from .exceptions import DingTalkException, DingTalkV2Exception
 import time
 import logging
 from urllib.parse import quote
 
 URL = "https://oapi.dingtalk.com"
+NEW_URL = "https://api.dingtalk.com"
 
 _logger = logging.getLogger(__name__)
 
 
 class Core(object):
 
     def __get__(self, instance, type):
@@ -73,16 +74,50 @@
     def _sign_corp_request(self, appsecret, timestamp):
         """
         compute signature for third app request.
         """
         signstring = f"{timestamp}\n{self._suitticket}"
         return qoute(b64encode(HMAC(appsecret.encode('utf-8'), signstring, sha256).digest()).decode('utf-8'))
 
-    def _post(self, url, data):
+    def _post(self, url, json=None, data=None, files=None):
         # [FIXME] other two type requests
         access_token = self._get_enterprise_access_token()
         res = requests.post(
-            f"{url}?access_token={access_token}", json=data).json()
+            f"{url}?access_token={access_token}", data=data, json=json, files=files).json()
+        print(res)
         if res['errcode'] != 0:
             _logger.debug(f"[DingTalk Request]:{data}")
             raise DingTalkException(**res)
         return res
+
+    def _v2_get_access_token(self):
+        """
+            get new api access token.
+        """
+        url = f"{NEW_URL}/v1.0/oauth2/accessToken"
+
+        data = {
+            "appKey": self._appkey,
+            "appSecret": self._appsecret
+        }
+
+        res = requests.post(url, json=data).json()
+        return res['accessToken']
+
+    def _v2_post(self, url, json=None, data=None, files=None):
+        """
+            NEW Post
+        """
+        access_token = self._v2_get_access_token()
+        headers = {
+            "x-acs-dingtalk-access-token": access_token,
+            "Content-Type":"application/json"
+        }
+        res = requests.post(
+            url, data=data, json=json, files=files, headers=headers).json()
+        print(url)
+        print(headers)
+        print(json)
+        print(res)
+        if res.get("code"):
+            raise DingTalkV2Exception(**res)
+        return res
```

### Comparing `dingding-sdk-0.0.4/dingtalk/oauth.py` & `dingding-sdk-0.0.6/dingtalk/oauth.py`

 * *Files identical despite different names*

### Comparing `dingding-sdk-0.0.4/PKG-INFO` & `dingding-sdk-0.0.6/dingding_sdk.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: dingding-sdk
-Version: 0.0.4
+Version: 0.0.6
 Summary: DingTalk Python SDK
 Home-page: https://github.com/jellyhappy/dingding-sdk
 Author: blackcat
 Author-email: kfx2007@163.com
 License: GNU
-Description: # DingTalk Python SDK
-        
-        author: Kevin Kong 
-        version: 0.0.1
-        
-        
 Keywords: dingding sdk
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Description-Content-Type: text/markdown
+
+# DingTalk Python SDK
+
+author: Kevin Kong 
+version: 0.0.1
+
+
+
```

### Comparing `dingding-sdk-0.0.4/setup.py` & `dingding-sdk-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `dingding-sdk-0.0.4/tests/test_contact.py` & `dingding-sdk-0.0.6/tests/test_contact.py`

 * *Files identical despite different names*

### Comparing `dingding-sdk-0.0.4/tests/test_core.py` & `dingding-sdk-0.0.6/tests/test_core.py`

 * *Files identical despite different names*

