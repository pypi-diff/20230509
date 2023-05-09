# Comparing `tmp/pwl-chat-python-1.3.8.tar.gz` & `tmp/pwl-chat-python-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl-chat-python-1.3.8.tar", last modified: Tue May  9 03:13:28 2023, max compression
+gzip compressed data, was "pwl-chat-python-1.3.9.tar", last modified: Tue May  9 03:17:27 2023, max compression
```

## Comparing `pwl-chat-python-1.3.8.tar` & `pwl-chat-python-1.3.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 03:13:28.585281 pwl-chat-python-1.3.8/
--rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-09 02:39:53.000000 pwl-chat-python-1.3.8/LICENSE
--rw-r--r--   0 fangcong   (501) staff       (20)     2009 2023-05-09 03:13:28.584754 pwl-chat-python-1.3.8/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)     1410 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.8/README.md
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 03:13:28.574552 pwl-chat-python-1.3.8/pwl_chat_python.egg-info/
--rw-r--r--   0 fangcong   (501) staff       (20)     2009 2023-05-09 03:13:28.000000 pwl-chat-python-1.3.8/pwl_chat_python.egg-info/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)      549 2023-05-09 03:13:28.000000 pwl-chat-python-1.3.8/pwl_chat_python.egg-info/SOURCES.txt
--rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-05-09 03:13:28.000000 pwl-chat-python-1.3.8/pwl_chat_python.egg-info/dependency_links.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       49 2023-05-09 03:13:28.000000 pwl-chat-python-1.3.8/pwl_chat_python.egg-info/entry_points.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-09 03:13:28.000000 pwl-chat-python-1.3.8/pwl_chat_python.egg-info/requires.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       31 2023-05-09 03:13:28.000000 pwl-chat-python-1.3.8/pwl_chat_python.egg-info/top_level.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-05-09 03:13:28.585438 pwl-chat-python-1.3.8/setup.cfg
--rw-r--r--   0 fangcong   (501) staff       (20)     3546 2023-05-09 02:50:53.000000 pwl-chat-python-1.3.8/setup.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 03:13:28.575068 pwl-chat-python-1.3.8/src/
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 03:13:28.577741 pwl-chat-python-1.3.8/src/api/
--rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.8/src/api/__api__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1993 2023-05-09 03:08:13.000000 pwl-chat-python-1.3.8/src/api/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1735 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.8/src/api/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1120 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.8/src/api/user.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 03:13:28.582650 pwl-chat-python-1.3.8/src/core/
--rw-r--r--   0 fangcong   (501) staff       (20)     2625 2023-05-09 03:08:05.000000 pwl-chat-python-1.3.8/src/core/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1623 2023-05-09 03:09:09.000000 pwl-chat-python-1.3.8/src/core/blacklist.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1818 2023-05-09 03:07:55.000000 pwl-chat-python-1.3.8/src/core/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1954 2023-05-09 02:23:28.000000 pwl-chat-python-1.3.8/src/core/cli.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1630 2023-05-09 02:39:43.000000 pwl-chat-python-1.3.8/src/core/config.py
--rw-r--r--   0 fangcong   (501) staff       (20)     4435 2023-05-09 03:07:44.000000 pwl-chat-python-1.3.8/src/core/redpacket.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1360 2023-05-09 03:07:35.000000 pwl-chat-python-1.3.8/src/core/user.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1226 2023-05-09 03:07:39.000000 pwl-chat-python-1.3.8/src/core/websocket.py
--rw-r--r--   0 fangcong   (501) staff       (20)      991 2023-05-09 03:12:35.000000 pwl-chat-python-1.3.8/src/main.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 03:13:28.583756 pwl-chat-python-1.3.8/src/utils/
--rw-r--r--   0 fangcong   (501) staff       (20)      739 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.8/src/utils/utils.py
--rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-05-09 03:13:17.000000 pwl-chat-python-1.3.8/src/utils/version.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 03:17:27.752756 pwl-chat-python-1.3.9/
+-rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-09 02:39:53.000000 pwl-chat-python-1.3.9/LICENSE
+-rw-r--r--   0 fangcong   (501) staff       (20)     2009 2023-05-09 03:17:27.752286 pwl-chat-python-1.3.9/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)     1410 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.9/README.md
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 03:17:27.738728 pwl-chat-python-1.3.9/pwl_chat_python.egg-info/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2009 2023-05-09 03:17:27.000000 pwl-chat-python-1.3.9/pwl_chat_python.egg-info/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)      549 2023-05-09 03:17:27.000000 pwl-chat-python-1.3.9/pwl_chat_python.egg-info/SOURCES.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-05-09 03:17:27.000000 pwl-chat-python-1.3.9/pwl_chat_python.egg-info/dependency_links.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       49 2023-05-09 03:17:27.000000 pwl-chat-python-1.3.9/pwl_chat_python.egg-info/entry_points.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-09 03:17:27.000000 pwl-chat-python-1.3.9/pwl_chat_python.egg-info/requires.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       31 2023-05-09 03:17:27.000000 pwl-chat-python-1.3.9/pwl_chat_python.egg-info/top_level.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-05-09 03:17:27.752897 pwl-chat-python-1.3.9/setup.cfg
+-rw-r--r--   0 fangcong   (501) staff       (20)     3546 2023-05-09 02:50:53.000000 pwl-chat-python-1.3.9/setup.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 03:17:27.739265 pwl-chat-python-1.3.9/src/
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 03:17:27.742782 pwl-chat-python-1.3.9/src/api/
+-rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.9/src/api/__api__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1993 2023-05-09 03:08:13.000000 pwl-chat-python-1.3.9/src/api/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1743 2023-05-09 03:16:36.000000 pwl-chat-python-1.3.9/src/api/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1124 2023-05-09 03:16:34.000000 pwl-chat-python-1.3.9/src/api/user.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 03:17:27.750229 pwl-chat-python-1.3.9/src/core/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2625 2023-05-09 03:08:05.000000 pwl-chat-python-1.3.9/src/core/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1623 2023-05-09 03:09:09.000000 pwl-chat-python-1.3.9/src/core/blacklist.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1818 2023-05-09 03:07:55.000000 pwl-chat-python-1.3.9/src/core/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1958 2023-05-09 03:16:59.000000 pwl-chat-python-1.3.9/src/core/cli.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1630 2023-05-09 02:39:43.000000 pwl-chat-python-1.3.9/src/core/config.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     4435 2023-05-09 03:07:44.000000 pwl-chat-python-1.3.9/src/core/redpacket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1360 2023-05-09 03:07:35.000000 pwl-chat-python-1.3.9/src/core/user.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1226 2023-05-09 03:17:10.000000 pwl-chat-python-1.3.9/src/core/websocket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)      991 2023-05-09 03:12:35.000000 pwl-chat-python-1.3.9/src/main.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 03:17:27.751450 pwl-chat-python-1.3.9/src/utils/
+-rw-r--r--   0 fangcong   (501) staff       (20)      739 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.9/src/utils/utils.py
+-rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-05-09 03:17:16.000000 pwl-chat-python-1.3.9/src/utils/version.py
```

### Comparing `pwl-chat-python-1.3.8/LICENSE` & `pwl-chat-python-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.8/PKG-INFO` & `pwl-chat-python-1.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.3.8
+Version: 1.3.9
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pwl-chat-python-1.3.8/README.md` & `pwl-chat-python-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.8/pwl_chat_python.egg-info/PKG-INFO` & `pwl-chat-python-1.3.9/pwl_chat_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.3.8
+Version: 1.3.9
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pwl-chat-python-1.3.8/pwl_chat_python.egg-info/SOURCES.txt` & `pwl-chat-python-1.3.9/pwl_chat_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.8/setup.py` & `pwl-chat-python-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.8/src/api/__init__.py` & `pwl-chat-python-1.3.9/src/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.8/src/api/chatroom.py` & `pwl-chat-python-1.3.9/src/api/chatroom.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import json
 import random
-from utils.utils import UA, HOST
-from utils.version import __version__
+from src.utils.utils import UA, HOST
+from src.utils.version import __version__
 from .__api__ import Base
 
 
 class ChatRoom(Base):
 
     def more(self, page: int = 1) -> None | dict:
         if self.api_key == '':
```

### Comparing `pwl-chat-python-1.3.8/src/api/user.py` & `pwl-chat-python-1.3.9/src/api/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import requests
 import json
 
-from utils.utils import UA, HOST
+from src.utils.utils import UA, HOST
 from .__api__ import Base
 
 
 class User(Base):
 
     def get_user_info(self, username: str) -> None | dict:
         if self.api_key == '':
```

### Comparing `pwl-chat-python-1.3.8/src/core/__init__.py` & `pwl-chat-python-1.3.9/src/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.8/src/core/blacklist.py` & `pwl-chat-python-1.3.9/src/core/blacklist.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.8/src/core/chatroom.py` & `pwl-chat-python-1.3.9/src/core/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.8/src/core/cli.py` & `pwl-chat-python-1.3.9/src/core/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import _thread
 from .blacklist import *
 from .config import GLOBAL_CONFIG
 from .user import *
-from utils.utils import *
+from src.utils.utils import *
 
 
 
 
 def init_sys_in(api: FishPi):
     _thread.start_new_thread(console_input, (api,))
```

### Comparing `pwl-chat-python-1.3.8/src/core/config.py` & `pwl-chat-python-1.3.9/src/core/config.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.8/src/core/redpacket.py` & `pwl-chat-python-1.3.9/src/core/redpacket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.8/src/core/user.py` & `pwl-chat-python-1.3.9/src/core/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.8/src/core/websocket.py` & `pwl-chat-python-1.3.9/src/core/websocket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.8/src/main.py` & `pwl-chat-python-1.3.9/src/main.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.8/src/utils/utils.py` & `pwl-chat-python-1.3.9/src/utils/utils.py`

 * *Files identical despite different names*

