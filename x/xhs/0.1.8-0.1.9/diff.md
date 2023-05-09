# Comparing `tmp/xhs-0.1.8.tar.gz` & `tmp/xhs-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhs-0.1.8.tar", last modified: Mon May  8 03:51:06 2023, max compression
+gzip compressed data, was "xhs-0.1.9.tar", last modified: Tue May  9 04:18:27 2023, max compression
```

## Comparing `xhs-0.1.8.tar` & `xhs-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:51:06.000518 xhs-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-08 03:50:52.000000 xhs-0.1.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-08 03:50:52.000000 xhs-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-08 03:50:52.000000 xhs-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-08 03:51:06.000518 xhs-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-08 03:50:52.000000 xhs-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 03:50:52.000000 xhs-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-08 03:51:06.000518 xhs-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-08 03:50:52.000000 xhs-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:51:06.000518 xhs-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-08 03:50:52.000000 xhs-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-08 03:50:52.000000 xhs-0.1.8/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-05-08 03:50:52.000000 xhs-0.1.8/tests/test_xhs.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-08 03:50:52.000000 xhs-0.1.8/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:51:06.000518 xhs-0.1.8/xhs/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-08 03:50:52.000000 xhs-0.1.8/xhs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-08 03:50:52.000000 xhs-0.1.8/xhs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21200 2023-05-08 03:50:52.000000 xhs-0.1.8/xhs/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-08 03:50:52.000000 xhs-0.1.8/xhs/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-05-08 03:50:52.000000 xhs-0.1.8/xhs/help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:51:06.000518 xhs-0.1.8/xhs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-08 03:51:05.000000 xhs-0.1.8/xhs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 03:51:05.000000 xhs-0.1.8/xhs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 03:51:05.000000 xhs-0.1.8/xhs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 03:51:05.000000 xhs-0.1.8/xhs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 03:51:05.000000 xhs-0.1.8/xhs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-08 03:51:05.000000 xhs-0.1.8/xhs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:18:27.348841 xhs-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-09 04:18:15.000000 xhs-0.1.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-09 04:18:15.000000 xhs-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-09 04:18:15.000000 xhs-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-09 04:18:27.348841 xhs-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-09 04:18:15.000000 xhs-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 04:18:15.000000 xhs-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-09 04:18:27.348841 xhs-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-09 04:18:15.000000 xhs-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:18:27.344841 xhs-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-09 04:18:15.000000 xhs-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-09 04:18:15.000000 xhs-0.1.9/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-05-09 04:18:15.000000 xhs-0.1.9/tests/test_xhs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-09 04:18:15.000000 xhs-0.1.9/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:18:27.344841 xhs-0.1.9/xhs/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-09 04:18:15.000000 xhs-0.1.9/xhs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-09 04:18:15.000000 xhs-0.1.9/xhs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21231 2023-05-09 04:18:15.000000 xhs-0.1.9/xhs/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-09 04:18:15.000000 xhs-0.1.9/xhs/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11752 2023-05-09 04:18:15.000000 xhs-0.1.9/xhs/help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:18:27.344841 xhs-0.1.9/xhs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-09 04:18:27.000000 xhs-0.1.9/xhs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-09 04:18:27.000000 xhs-0.1.9/xhs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 04:18:27.000000 xhs-0.1.9/xhs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 04:18:27.000000 xhs-0.1.9/xhs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 04:18:27.000000 xhs-0.1.9/xhs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-09 04:18:27.000000 xhs-0.1.9/xhs.egg-info/top_level.txt
```

### Comparing `xhs-0.1.8/CHANGELOG.md` & `xhs-0.1.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 
 ## dev
 
 - Improve documentation
 - Add more test function
 
+## 0.1.9
+
+### Fixed
+
+- fixed get videos key error
+
 ## 0.1.8
 
 ### Added
 
 - add get img and video to help
 
 ### Changed
```

### Comparing `xhs-0.1.8/LICENSE` & `xhs-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xhs-0.1.8/PKG-INFO` & `xhs-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.1.8
+Version: 0.1.9
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xhs-0.1.8/README.md` & `xhs-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `xhs-0.1.8/setup.py` & `xhs-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.8/tests/__init__.py` & `xhs-0.1.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.8/tests/test_help.py` & `xhs-0.1.9/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.8/tests/test_xhs.py` & `xhs-0.1.9/tests/test_xhs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-import requests
 
 from xhs import FeedType, IPBlockError, XhsClient
 
 from . import test_cookie
 from .utils import beauty_print
 
 
@@ -15,15 +14,15 @@
 def test_xhs_client_init():
     xhs_client = XhsClient()
     assert xhs_client
 
 
 def test_cookie_setter_getter():
     xhs_client = XhsClient()
-    cd = requests.utils.dict_from_cookiejar(xhs_client.session.cookies)
+    cd = xhs_client.cookie_dict
     beauty_print(cd)
     assert "web_session" in cd
 
 
 def test_get_note_by_id(xhs_client: XhsClient):
     note_id = "6413cf6b00000000270115b5"
     data = xhs_client.get_note_by_id(note_id)
```

### Comparing `xhs-0.1.8/xhs/core.py` & `xhs-0.1.9/xhs/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from enum import Enum
 from typing import NamedTuple
 
 import requests
 
 from xhs.exception import DataFetchError, IPBlockError
 
-from .help import (cookie_jar_to_cookie_str, cookie_str_to_cookie_dict,
-                   download_file, get_imgs_url_from_note, get_search_id,
-                   get_valid_path_name, get_video_url_from_note, sign,
+from .help import (cookie_jar_to_cookie_str, download_file,
+                   get_imgs_url_from_note, get_search_id, get_valid_path_name,
+                   get_video_url_from_note, sign,
                    update_session_cookies_from_cookie)
 
 
 class FeedType(Enum):
     # 推荐
     RECOMMEND = "homefeed_recommend"
     # 穿搭
@@ -114,19 +114,22 @@
     @property
     def cookie(self):
         return cookie_jar_to_cookie_str(self.__session)
 
     @cookie.setter
     def cookie(self, cookie: str):
         update_session_cookies_from_cookie(self.__session, cookie)
-        cookie_dict = cookie_str_to_cookie_dict(self.cookie)
-        if "web_session" not in cookie_dict:
+        if "web_session" not in self.cookie_dict:
             self.activate()
 
     @property
+    def cookie_dict(self):
+        return requests.utils.dict_from_cookiejar(self.session.cookies)
+
+    @property
     def session(self):
         return self.__session
 
     @property
     def user_agent(self):
         return self.__session.headers.get("user-agent")
```

### Comparing `xhs-0.1.8/xhs/help.py` & `xhs-0.1.9/xhs/help.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,16 @@
     if not note.get("video"):
         return ""
     origin_video_key = note['video']['consumer']['origin_video_key']
     return f"{random.choice(video_cdns)}/{origin_video_key}"
 
 
 def get_video_urls_from_note(note) -> list:
+    if not note.get("video"):
+        return []
     origin_video_key = note['video']['consumer']['origin_video_key']
     return [f"{cdn}/{origin_video_key}?imageView2/format/{format}" for cdn in video_cdns]
 
 
 def download_file(url: str, filename: str):
     with requests.get(url, stream=True) as r:
         r.raise_for_status()
```

### Comparing `xhs-0.1.8/xhs.egg-info/PKG-INFO` & `xhs-0.1.9/xhs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.1.8
+Version: 0.1.9
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
```

