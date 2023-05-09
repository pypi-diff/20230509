# Comparing `tmp/pwl-chat-python-1.3.6.tar.gz` & `tmp/pwl-chat-python-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl-chat-python-1.3.6.tar", last modified: Tue May  9 02:50:56 2023, max compression
+gzip compressed data, was "pwl-chat-python-1.3.7.tar", last modified: Tue May  9 03:05:12 2023, max compression
```

## Comparing `pwl-chat-python-1.3.6.tar` & `pwl-chat-python-1.3.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 02:50:56.886134 pwl-chat-python-1.3.6/
--rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-09 02:39:53.000000 pwl-chat-python-1.3.6/LICENSE
--rw-r--r--   0 fangcong   (501) staff       (20)     2009 2023-05-09 02:50:56.885623 pwl-chat-python-1.3.6/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)     1410 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.6/README.md
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 02:50:56.874889 pwl-chat-python-1.3.6/pwl_chat_python.egg-info/
--rw-r--r--   0 fangcong   (501) staff       (20)     2009 2023-05-09 02:50:56.000000 pwl-chat-python-1.3.6/pwl_chat_python.egg-info/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)      549 2023-05-09 02:50:56.000000 pwl-chat-python-1.3.6/pwl_chat_python.egg-info/SOURCES.txt
--rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-05-09 02:50:56.000000 pwl-chat-python-1.3.6/pwl_chat_python.egg-info/dependency_links.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       49 2023-05-09 02:50:56.000000 pwl-chat-python-1.3.6/pwl_chat_python.egg-info/entry_points.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-09 02:50:56.000000 pwl-chat-python-1.3.6/pwl_chat_python.egg-info/requires.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       31 2023-05-09 02:50:56.000000 pwl-chat-python-1.3.6/pwl_chat_python.egg-info/top_level.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-05-09 02:50:56.886354 pwl-chat-python-1.3.6/setup.cfg
--rw-r--r--   0 fangcong   (501) staff       (20)     3546 2023-05-09 02:50:53.000000 pwl-chat-python-1.3.6/setup.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 02:50:56.875672 pwl-chat-python-1.3.6/src/
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 02:50:56.878186 pwl-chat-python-1.3.6/src/api/
--rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.6/src/api/__api__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1989 2023-05-09 02:48:49.000000 pwl-chat-python-1.3.6/src/api/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1735 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.6/src/api/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1120 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.6/src/api/user.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 02:50:56.883068 pwl-chat-python-1.3.6/src/core/
--rw-r--r--   0 fangcong   (501) staff       (20)     2621 2023-05-09 02:37:39.000000 pwl-chat-python-1.3.6/src/core/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1619 2023-05-09 02:23:15.000000 pwl-chat-python-1.3.6/src/core/blacklist.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1814 2023-05-09 02:23:19.000000 pwl-chat-python-1.3.6/src/core/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1954 2023-05-09 02:23:28.000000 pwl-chat-python-1.3.6/src/core/cli.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1630 2023-05-09 02:39:43.000000 pwl-chat-python-1.3.6/src/core/config.py
--rw-r--r--   0 fangcong   (501) staff       (20)     4431 2023-05-09 02:23:37.000000 pwl-chat-python-1.3.6/src/core/redpacket.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1352 2023-05-09 02:23:41.000000 pwl-chat-python-1.3.6/src/core/user.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1222 2023-05-09 02:23:48.000000 pwl-chat-python-1.3.6/src/core/websocket.py
--rw-r--r--   0 fangcong   (501) staff       (20)      967 2023-05-09 02:39:19.000000 pwl-chat-python-1.3.6/src/main.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 02:50:56.884861 pwl-chat-python-1.3.6/src/utils/
--rw-r--r--   0 fangcong   (501) staff       (20)      739 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.6/src/utils/utils.py
--rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-05-09 02:39:35.000000 pwl-chat-python-1.3.6/src/utils/version.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 03:05:12.482444 pwl-chat-python-1.3.7/
+-rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-09 02:39:53.000000 pwl-chat-python-1.3.7/LICENSE
+-rw-r--r--   0 fangcong   (501) staff       (20)     2009 2023-05-09 03:05:12.481989 pwl-chat-python-1.3.7/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)     1410 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.7/README.md
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 03:05:12.470645 pwl-chat-python-1.3.7/pwl_chat_python.egg-info/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2009 2023-05-09 03:05:12.000000 pwl-chat-python-1.3.7/pwl_chat_python.egg-info/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)      549 2023-05-09 03:05:12.000000 pwl-chat-python-1.3.7/pwl_chat_python.egg-info/SOURCES.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-05-09 03:05:12.000000 pwl-chat-python-1.3.7/pwl_chat_python.egg-info/dependency_links.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       49 2023-05-09 03:05:12.000000 pwl-chat-python-1.3.7/pwl_chat_python.egg-info/entry_points.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-09 03:05:12.000000 pwl-chat-python-1.3.7/pwl_chat_python.egg-info/requires.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       31 2023-05-09 03:05:12.000000 pwl-chat-python-1.3.7/pwl_chat_python.egg-info/top_level.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-05-09 03:05:12.482579 pwl-chat-python-1.3.7/setup.cfg
+-rw-r--r--   0 fangcong   (501) staff       (20)     3546 2023-05-09 02:50:53.000000 pwl-chat-python-1.3.7/setup.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 03:05:12.471296 pwl-chat-python-1.3.7/src/
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 03:05:12.474721 pwl-chat-python-1.3.7/src/api/
+-rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.7/src/api/__api__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1989 2023-05-09 02:48:49.000000 pwl-chat-python-1.3.7/src/api/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1735 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.7/src/api/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1120 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.7/src/api/user.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 03:05:12.479917 pwl-chat-python-1.3.7/src/core/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2621 2023-05-09 02:37:39.000000 pwl-chat-python-1.3.7/src/core/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1619 2023-05-09 03:04:03.000000 pwl-chat-python-1.3.7/src/core/blacklist.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1814 2023-05-09 03:04:27.000000 pwl-chat-python-1.3.7/src/core/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1954 2023-05-09 02:23:28.000000 pwl-chat-python-1.3.7/src/core/cli.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1630 2023-05-09 02:39:43.000000 pwl-chat-python-1.3.7/src/core/config.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     4431 2023-05-09 02:23:37.000000 pwl-chat-python-1.3.7/src/core/redpacket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1352 2023-05-09 02:23:41.000000 pwl-chat-python-1.3.7/src/core/user.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1222 2023-05-09 02:23:48.000000 pwl-chat-python-1.3.7/src/core/websocket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)      973 2023-05-09 03:04:37.000000 pwl-chat-python-1.3.7/src/main.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 03:05:12.481151 pwl-chat-python-1.3.7/src/utils/
+-rw-r--r--   0 fangcong   (501) staff       (20)      739 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.7/src/utils/utils.py
+-rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-05-09 03:05:00.000000 pwl-chat-python-1.3.7/src/utils/version.py
```

### Comparing `pwl-chat-python-1.3.6/LICENSE` & `pwl-chat-python-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.6/PKG-INFO` & `pwl-chat-python-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.3.6
+Version: 1.3.7
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pwl-chat-python-1.3.6/README.md` & `pwl-chat-python-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.6/pwl_chat_python.egg-info/PKG-INFO` & `pwl-chat-python-1.3.7/pwl_chat_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.3.6
+Version: 1.3.7
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pwl-chat-python-1.3.6/pwl_chat_python.egg-info/SOURCES.txt` & `pwl-chat-python-1.3.7/pwl_chat_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.6/setup.py` & `pwl-chat-python-1.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.6/src/api/__init__.py` & `pwl-chat-python-1.3.7/src/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.6/src/api/chatroom.py` & `pwl-chat-python-1.3.7/src/api/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.6/src/api/user.py` & `pwl-chat-python-1.3.7/src/api/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.6/src/core/__init__.py` & `pwl-chat-python-1.3.7/src/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.6/src/core/blacklist.py` & `pwl-chat-python-1.3.7/src/core/blacklist.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.6/src/core/chatroom.py` & `pwl-chat-python-1.3.7/src/core/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.6/src/core/cli.py` & `pwl-chat-python-1.3.7/src/core/cli.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.6/src/core/config.py` & `pwl-chat-python-1.3.7/src/core/config.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.6/src/core/redpacket.py` & `pwl-chat-python-1.3.7/src/core/redpacket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.6/src/core/user.py` & `pwl-chat-python-1.3.7/src/core/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.6/src/core/websocket.py` & `pwl-chat-python-1.3.7/src/core/websocket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.6/src/main.py` & `pwl-chat-python-1.3.7/src/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 import click
-from core import __init__
-from core.config import GLOBAL_CONFIG, AuthConfig
-from core.user import login
-from core.websocket import start
-from utils.version import __version__
-from api import FishPi
+from .core import __init__
+from .core.config import GLOBAL_CONFIG, AuthConfig
+from .core.user import login
+from .core.websocket import start
+from .utils.version import __version__
+from .api import FishPi
 
 
 def run(params: dict):
     api = FishPi()
     __init__(api)
     if params:
         GLOBAL_CONFIG.auth_config = AuthConfig.build(params)
```

### Comparing `pwl-chat-python-1.3.6/src/utils/utils.py` & `pwl-chat-python-1.3.7/src/utils/utils.py`

 * *Files identical despite different names*

