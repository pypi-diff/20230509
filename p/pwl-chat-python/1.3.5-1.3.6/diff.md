# Comparing `tmp/pwl-chat-python-1.3.5.tar.gz` & `tmp/pwl-chat-python-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl-chat-python-1.3.5.tar", last modified: Mon May  8 09:10:54 2023, max compression
+gzip compressed data, was "pwl-chat-python-1.3.6.tar", last modified: Tue May  9 02:50:56 2023, max compression
```

## Comparing `pwl-chat-python-1.3.5.tar` & `pwl-chat-python-1.3.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:10:54.147136 pwl-chat-python-1.3.5/
--rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-08 06:12:10.000000 pwl-chat-python-1.3.5/LICENSE
--rw-r--r--   0 fangcong   (501) staff       (20)     1999 2023-05-08 09:10:54.146561 pwl-chat-python-1.3.5/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)     1400 2023-05-08 02:08:19.000000 pwl-chat-python-1.3.5/README.md
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:10:54.136424 pwl-chat-python-1.3.5/api/
--rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/api/__api__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1992 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/api/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1735 2023-05-08 06:43:12.000000 pwl-chat-python-1.3.5/api/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1120 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/api/user.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:10:54.140741 pwl-chat-python-1.3.5/core/
--rw-r--r--   0 fangcong   (501) staff       (20)     2239 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/core/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1623 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/core/blacklist.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1822 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/core/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1966 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/core/cli.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1633 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/core/config.py
--rw-r--r--   0 fangcong   (501) staff       (20)     4435 2023-05-08 03:41:01.000000 pwl-chat-python-1.3.5/core/redpacket.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1356 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/core/user.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1230 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/core/websocket.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:10:54.141224 pwl-chat-python-1.3.5/main/
--rw-r--r--   0 fangcong   (501) staff       (20)      967 2023-05-08 09:06:58.000000 pwl-chat-python-1.3.5/main/main.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:10:54.144505 pwl-chat-python-1.3.5/pwl_chat_python.egg-info/
--rw-r--r--   0 fangcong   (501) staff       (20)     1999 2023-05-08 09:10:54.000000 pwl-chat-python-1.3.5/pwl_chat_python.egg-info/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)      494 2023-05-08 09:10:54.000000 pwl-chat-python-1.3.5/pwl_chat_python.egg-info/SOURCES.txt
--rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-05-08 09:10:54.000000 pwl-chat-python-1.3.5/pwl_chat_python.egg-info/dependency_links.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       50 2023-05-08 09:10:54.000000 pwl-chat-python-1.3.5/pwl_chat_python.egg-info/entry_points.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-08 09:10:54.000000 pwl-chat-python-1.3.5/pwl_chat_python.egg-info/requires.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       20 2023-05-08 09:10:54.000000 pwl-chat-python-1.3.5/pwl_chat_python.egg-info/top_level.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-05-08 09:10:54.147329 pwl-chat-python-1.3.5/setup.cfg
--rw-r--r--   0 fangcong   (501) staff       (20)     3532 2023-05-08 09:10:37.000000 pwl-chat-python-1.3.5/setup.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-08 09:10:54.145745 pwl-chat-python-1.3.5/utils/
--rw-r--r--   0 fangcong   (501) staff       (20)      739 2023-05-07 14:52:29.000000 pwl-chat-python-1.3.5/utils/utils.py
--rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-05-08 09:10:50.000000 pwl-chat-python-1.3.5/utils/version.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 02:50:56.886134 pwl-chat-python-1.3.6/
+-rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-09 02:39:53.000000 pwl-chat-python-1.3.6/LICENSE
+-rw-r--r--   0 fangcong   (501) staff       (20)     2009 2023-05-09 02:50:56.885623 pwl-chat-python-1.3.6/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)     1410 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.6/README.md
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 02:50:56.874889 pwl-chat-python-1.3.6/pwl_chat_python.egg-info/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2009 2023-05-09 02:50:56.000000 pwl-chat-python-1.3.6/pwl_chat_python.egg-info/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)      549 2023-05-09 02:50:56.000000 pwl-chat-python-1.3.6/pwl_chat_python.egg-info/SOURCES.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-05-09 02:50:56.000000 pwl-chat-python-1.3.6/pwl_chat_python.egg-info/dependency_links.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       49 2023-05-09 02:50:56.000000 pwl-chat-python-1.3.6/pwl_chat_python.egg-info/entry_points.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-09 02:50:56.000000 pwl-chat-python-1.3.6/pwl_chat_python.egg-info/requires.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       31 2023-05-09 02:50:56.000000 pwl-chat-python-1.3.6/pwl_chat_python.egg-info/top_level.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-05-09 02:50:56.886354 pwl-chat-python-1.3.6/setup.cfg
+-rw-r--r--   0 fangcong   (501) staff       (20)     3546 2023-05-09 02:50:53.000000 pwl-chat-python-1.3.6/setup.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 02:50:56.875672 pwl-chat-python-1.3.6/src/
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 02:50:56.878186 pwl-chat-python-1.3.6/src/api/
+-rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.6/src/api/__api__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1989 2023-05-09 02:48:49.000000 pwl-chat-python-1.3.6/src/api/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1735 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.6/src/api/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1120 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.6/src/api/user.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 02:50:56.883068 pwl-chat-python-1.3.6/src/core/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2621 2023-05-09 02:37:39.000000 pwl-chat-python-1.3.6/src/core/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1619 2023-05-09 02:23:15.000000 pwl-chat-python-1.3.6/src/core/blacklist.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1814 2023-05-09 02:23:19.000000 pwl-chat-python-1.3.6/src/core/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1954 2023-05-09 02:23:28.000000 pwl-chat-python-1.3.6/src/core/cli.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1630 2023-05-09 02:39:43.000000 pwl-chat-python-1.3.6/src/core/config.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     4431 2023-05-09 02:23:37.000000 pwl-chat-python-1.3.6/src/core/redpacket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1352 2023-05-09 02:23:41.000000 pwl-chat-python-1.3.6/src/core/user.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1222 2023-05-09 02:23:48.000000 pwl-chat-python-1.3.6/src/core/websocket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)      967 2023-05-09 02:39:19.000000 pwl-chat-python-1.3.6/src/main.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 02:50:56.884861 pwl-chat-python-1.3.6/src/utils/
+-rw-r--r--   0 fangcong   (501) staff       (20)      739 2023-05-09 02:18:14.000000 pwl-chat-python-1.3.6/src/utils/utils.py
+-rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-05-09 02:39:35.000000 pwl-chat-python-1.3.6/src/utils/version.py
```

### Comparing `pwl-chat-python-1.3.5/LICENSE` & `pwl-chat-python-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.5/PKG-INFO` & `pwl-chat-python-1.3.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.3.5
+Version: 1.3.6
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -68,15 +68,15 @@
 在 `config.ini`中配置摸鱼派账号登陆信息
 
 ### 第三步
 
 执行
 
 ~~~bash
-python main.py
+python main/main.py
 ~~~
 
 后台执行
 
 ~~~bash
-nohup python -u main.py >> pwl.log 2>&1 &
+nohup python -u main/main.py >> pwl.log 2>&1 &
 ~~~
```

### Comparing `pwl-chat-python-1.3.5/README.md` & `pwl-chat-python-1.3.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 在 `config.ini`中配置摸鱼派账号登陆信息
 
 ### 第三步
 
 执行
 
 ~~~bash
-python main.py
+python main/main.py
 ~~~
 
 后台执行
 
 ~~~bash
-nohup python -u main.py >> pwl.log 2>&1 &
+nohup python -u main/main.py >> pwl.log 2>&1 &
 ~~~
```

### Comparing `pwl-chat-python-1.3.5/api/__init__.py` & `pwl-chat-python-1.3.6/src/api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-from api.chatroom import ChatRoom
+from .chatroom import ChatRoom
 from utils.utils import UA, HOST
 from .__api__ import Base
 from .user import User
 import sys
 import requests
 import hashlib
 import json
```

### Comparing `pwl-chat-python-1.3.5/api/chatroom.py` & `pwl-chat-python-1.3.6/src/api/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.5/api/user.py` & `pwl-chat-python-1.3.6/src/api/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.3.5/core/__init__.py` & `pwl-chat-python-1.3.6/src/core/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 import json
 
 from api import FishPi
-from core.chatroom import init_soliloquize
-from core.cli import init_sys_in
-from core.config import GLOBAL_CONFIG, RedPacketConfig, AuthConfig, RepeatConfig
+from .chatroom import init_soliloquize
+from .cli import init_sys_in
+from .config import GLOBAL_CONFIG, RedPacketConfig, AuthConfig, RepeatConfig
 import configparser
 import os
-import sys
 
 
 def __init__(api: FishPi):
+    file_path = f'{os.getcwd()}/config.ini'
     config = configparser.ConfigParser()
     try:
         print("配置读取中")
-        config.read(f'{os.getcwd()}/config.ini', encoding='utf-8')
-        GLOBAL_CONFIG.auth_config = __init_login_auth_config(config)
-        GLOBAL_CONFIG.redpacket_config = __int_redpacket_var(config)
-        GLOBAL_CONFIG.repeat_config = __init_repeat_config(config)
+        if not os.path.exists(file_path):
+            print("config.ini配置文件不存在")
+            __init_default_config()
+        else:
+            config.read(file_path, encoding='utf-8')
+            GLOBAL_CONFIG.auth_config = __init_login_auth_config(config)
+            GLOBAL_CONFIG.redpacket_config = __int_redpacket_var(config)
+            GLOBAL_CONFIG.repeat_config = __init_repeat_config(config)
     except:
-        print("请检查config.ini配置文件是否合法")
-        sys.exit(1)
+        print("config.ini配置文件不合法")
+        __init_default_config()
     init_soliloquize(api)
     init_sys_in(api)
 
 
+def __init_default_config():
+    print("加载默认配置文件")
+    GLOBAL_CONFIG.auth_config = AuthConfig()
+    GLOBAL_CONFIG.redpacket_config = RedPacketConfig()
+    GLOBAL_CONFIG.repeat_config = RepeatConfig()
+
+
 def __int_redpacket_var(config) -> RedPacketConfig:
     ret = RedPacketConfig()
     if config.getint('redPacket', 'rate') > 0:
         ret.rate = config.getint('redPacket', 'rate')
     ret.red_packet_switch = config.getboolean(
         'redPacket', 'openRedPacket')
     ret.heartbeat = config.getboolean(
```

### Comparing `pwl-chat-python-1.3.5/core/blacklist.py` & `pwl-chat-python-1.3.6/src/core/blacklist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import os
 import re
 from api import FishPi
-from core.config import GLOBAL_CONFIG
+from .config import GLOBAL_CONFIG
 
 
 def unban_someone(api: FishPi, username):
     if not GLOBAL_CONFIG.repeat_config.blacklist.__contains__(username):
         print(username + '不在黑名单中')
         return
     user_info = api.user.get_user_info(username)
```

### Comparing `pwl-chat-python-1.3.5/core/chatroom.py` & `pwl-chat-python-1.3.6/src/core/chatroom.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 import random
 import schedule
 from api import FishPi
-from core.config import GLOBAL_CONFIG
-from core.redpacket import rush_redpacket
+from .config import GLOBAL_CONFIG
+from .redpacket import rush_redpacket
 
 
 REPEAT_POOL = {}  # 复读池
 
 
 def init_soliloquize(api: FishPi):
     if GLOBAL_CONFIG.repeat_config.soliloquize_switch:
```

### Comparing `pwl-chat-python-1.3.5/core/cli.py` & `pwl-chat-python-1.3.6/src/core/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import _thread
-from core.blacklist import *
-from core.config import GLOBAL_CONFIG
-from core.user import *
+from .blacklist import *
+from .config import GLOBAL_CONFIG
+from .user import *
 from utils.utils import *
 
 
 
 
 def init_sys_in(api: FishPi):
     _thread.start_new_thread(console_input, (api,))
```

### Comparing `pwl-chat-python-1.3.5/core/config.py` & `pwl-chat-python-1.3.6/src/core/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 class RedPacketConfig(object):
-    def __init__(self, red_packet_switch=True, heartbeat=False, smart_mode=False, threshold=0.5, adventure_mode=False,
-                 timeout=5, rate=3):
+    def __init__(self, red_packet_switch=True, heartbeat=True, smart_mode=True, threshold=0.5, adventure_mode=True,
+                 timeout=7, rate=3):
         self.red_packet_switch = red_packet_switch
         self.heartbeat = heartbeat
         self.smart_mode = smart_mode
         self.threshold = threshold
         self.adventure_mode = adventure_mode
         self.timeout = timeout
         self.rate = rate
```

### Comparing `pwl-chat-python-1.3.5/core/redpacket.py` & `pwl-chat-python-1.3.6/src/core/redpacket.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from api import FishPi
 import json
 import time
 
-from core.config import GLOBAL_CONFIG
+from .config import GLOBAL_CONFIG
 
 
 def __open_redpacket_render(username, redpacket: dict) -> None:
     who = redpacket['who']
     for i in who:
         if i['userName'] == username:
             if i['userMoney'] < 0:
```

### Comparing `pwl-chat-python-1.3.5/core/user.py` & `pwl-chat-python-1.3.6/src/core/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
 import time
 from api import FishPi
 from utils.utils import *
-from core.config import GLOBAL_CONFIG
+from .config import GLOBAL_CONFIG
 
 
 def render_user_info(userInfo):
     print("用户ID: " + userInfo['oId'])
     print("用户名: " + userInfo['userName'])
     print("用户签名: " + userInfo['userIntro'])
     print("用户编号: " + str(userInfo['userNo']))
```

### Comparing `pwl-chat-python-1.3.5/core/websocket.py` & `pwl-chat-python-1.3.6/src/core/websocket.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import rel
 import time
 import schedule
 import websocket
 import _thread
 
 from api import FishPi
-from core.chatroom import listener
-from core.config import GLOBAL_CONFIG
+from .chatroom import listener
+from .config import GLOBAL_CONFIG
 
 __api = FishPi()
 def on_message(ws, message):
     json_body = json.loads(message)
     listener(__api, json_body)
```

### Comparing `pwl-chat-python-1.3.5/main/main.py` & `pwl-chat-python-1.3.6/src/main.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 import click
-from api import FishPi
 from core import __init__
 from core.config import GLOBAL_CONFIG, AuthConfig
 from core.user import login
 from core.websocket import start
 from utils.version import __version__
+from api import FishPi
 
 
 def run(params: dict):
     api = FishPi()
     __init__(api)
     if params:
         GLOBAL_CONFIG.auth_config = AuthConfig.build(params)
```

### Comparing `pwl-chat-python-1.3.5/pwl_chat_python.egg-info/PKG-INFO` & `pwl-chat-python-1.3.6/pwl_chat_python.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.3.5
+Version: 1.3.6
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -68,15 +68,15 @@
 在 `config.ini`中配置摸鱼派账号登陆信息
 
 ### 第三步
 
 执行
 
 ~~~bash
-python main.py
+python main/main.py
 ~~~
 
 后台执行
 
 ~~~bash
-nohup python -u main.py >> pwl.log 2>&1 &
+nohup python -u main/main.py >> pwl.log 2>&1 &
 ~~~
```

### Comparing `pwl-chat-python-1.3.5/setup.py` & `pwl-chat-python-1.3.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Note: To use the 'upload' functionality of this file, you must:
 #   $ pipenv install twine --dev
 
 import io
 import os
 import sys
 from shutil import rmtree
-from utils.version import __version__
+from src.utils.version import __version__
 
 from setuptools import setup, Command
 
 # Package meta-data.
 NAME = 'pwl-chat-python'
 DESCRIPTION = '摸鱼派聊天室python客户端'
 URL = 'https://github.com/gakkiyomi/pwl-chat-python'
@@ -92,15 +92,15 @@
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    packages=['api', 'core', 'utils', 'main'],
+    packages=['src', 'src/api', 'src/core', 'src/utils'],
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['mypackage'],
 
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
     install_requires=REQUIRED,
@@ -118,12 +118,12 @@
     ],
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
     },
     entry_points={
         'console_scripts': [
-            'pwl-chat-python = main.main:cli',
+            'pwl-chat-python = src.main:cli',
         ],
     }
 
 )
```

### Comparing `pwl-chat-python-1.3.5/utils/utils.py` & `pwl-chat-python-1.3.6/src/utils/utils.py`

 * *Files identical despite different names*

