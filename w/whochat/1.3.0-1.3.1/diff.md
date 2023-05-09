# Comparing `tmp/whochat-1.3.0.tar.gz` & `tmp/whochat-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whochat-1.3.0.tar", last modified: Thu Mar  9 10:25:06 2023, max compression
+gzip compressed data, was "whochat-1.3.1.tar", last modified: Tue May  9 01:34:30 2023, max compression
```

## Comparing `whochat-1.3.0.tar` & `whochat-1.3.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-03-09 10:25:06.266451 whochat-1.3.0/
--rw-r--r--   0 luming     (501) staff       (20)     1514 2023-01-29 06:35:29.000000 whochat-1.3.0/LICENSE
--rw-r--r--   0 luming     (501) staff       (20)       55 2023-01-29 06:35:29.000000 whochat-1.3.0/MANIFEST.in
--rw-r--r--   0 luming     (501) staff       (20)     7287 2023-03-09 10:25:06.266545 whochat-1.3.0/PKG-INFO
--rw-r--r--   0 luming     (501) staff       (20)     6634 2023-03-09 10:24:41.000000 whochat-1.3.0/README.md
--rw-r--r--   0 luming     (501) staff       (20)     1274 2023-03-09 10:25:06.266869 whochat-1.3.0/setup.cfg
--rw-r--r--   0 luming     (501) staff       (20)       38 2023-03-09 09:22:00.000000 whochat-1.3.0/setup.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-03-09 10:25:06.260591 whochat-1.3.0/whochat/
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-03-09 10:25:06.263028 whochat-1.3.0/whochat/ComWeChatRobot/
--rw-r--r--   0 luming     (501) staff       (20)   165376 2023-02-13 09:38:48.000000 whochat-1.3.0/whochat/ComWeChatRobot/CWeChatRobot.exe
--rw-r--r--   0 luming     (501) staff       (20)   293888 2023-02-13 09:38:48.000000 whochat-1.3.0/whochat/ComWeChatRobot/DWeChatRobot.dll
--rw-r--r--   0 luming     (501) staff       (20)      472 2023-02-13 09:38:48.000000 whochat-1.3.0/whochat/ComWeChatRobot/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)       65 2023-03-09 10:24:41.000000 whochat-1.3.0/whochat/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)      107 2023-01-29 06:35:29.000000 whochat-1.3.0/whochat/__main__.py
--rw-r--r--   0 luming     (501) staff       (20)      608 2023-02-13 09:38:48.000000 whochat-1.3.0/whochat/_comtypes.py
--rw-r--r--   0 luming     (501) staff       (20)     6413 2023-02-13 09:38:48.000000 whochat-1.3.0/whochat/abc.py
--rw-r--r--   0 luming     (501) staff       (20)    17254 2023-02-23 08:03:54.000000 whochat-1.3.0/whochat/bot.py
--rw-r--r--   0 luming     (501) staff       (20)     4145 2023-03-09 09:19:54.000000 whochat-1.3.0/whochat/cli.py
--rw-r--r--   0 luming     (501) staff       (20)      127 2023-01-29 06:35:29.000000 whochat-1.3.0/whochat/logger.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-03-09 10:25:06.264539 whochat-1.3.0/whochat/messages/
--rw-r--r--   0 luming     (501) staff       (20)        0 2023-01-29 06:35:29.000000 whochat-1.3.0/whochat/messages/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)      447 2023-02-18 10:04:21.000000 whochat-1.3.0/whochat/messages/constants.py
--rw-r--r--   0 luming     (501) staff       (20)     6875 2023-01-29 06:35:29.000000 whochat-1.3.0/whochat/messages/tcp.py
--rw-r--r--   0 luming     (501) staff       (20)     6832 2023-02-17 09:24:18.000000 whochat-1.3.0/whochat/messages/websocket.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-03-09 10:25:06.265254 whochat-1.3.0/whochat/rpc/
--rw-r--r--   0 luming     (501) staff       (20)       22 2023-01-29 06:35:29.000000 whochat-1.3.0/whochat/rpc/__init__.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-03-09 10:25:06.265626 whochat-1.3.0/whochat/rpc/clients/
--rw-r--r--   0 luming     (501) staff       (20)        0 2023-02-15 09:25:20.000000 whochat-1.3.0/whochat/rpc/clients/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)     4253 2023-02-17 09:06:37.000000 whochat-1.3.0/whochat/rpc/clients/websocket.py
--rw-r--r--   0 luming     (501) staff       (20)     1823 2023-02-16 01:33:48.000000 whochat-1.3.0/whochat/rpc/docs.py
--rw-r--r--   0 luming     (501) staff       (20)     9767 2023-02-20 07:55:44.000000 whochat-1.3.0/whochat/rpc/handlers.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-03-09 10:25:06.266167 whochat-1.3.0/whochat/rpc/servers/
--rw-r--r--   0 luming     (501) staff       (20)        0 2023-01-29 06:35:29.000000 whochat-1.3.0/whochat/rpc/servers/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)      930 2023-01-29 06:35:29.000000 whochat-1.3.0/whochat/rpc/servers/http.py
--rw-r--r--   0 luming     (501) staff       (20)     1165 2023-02-16 08:42:16.000000 whochat-1.3.0/whochat/rpc/servers/websocket.py
--rw-r--r--   0 luming     (501) staff       (20)     1108 2023-01-29 06:35:29.000000 whochat-1.3.0/whochat/signals.py
--rw-r--r--   0 luming     (501) staff       (20)     3091 2023-02-20 09:32:17.000000 whochat-1.3.0/whochat/utils.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-03-09 10:25:06.261482 whochat-1.3.0/whochat.egg-info/
--rw-r--r--   0 luming     (501) staff       (20)     7287 2023-03-09 10:25:06.000000 whochat-1.3.0/whochat.egg-info/PKG-INFO
--rw-r--r--   0 luming     (501) staff       (20)      850 2023-03-09 10:25:06.000000 whochat-1.3.0/whochat.egg-info/SOURCES.txt
--rw-r--r--   0 luming     (501) staff       (20)        1 2023-03-09 10:25:06.000000 whochat-1.3.0/whochat.egg-info/dependency_links.txt
--rw-r--r--   0 luming     (501) staff       (20)       50 2023-03-09 10:25:06.000000 whochat-1.3.0/whochat.egg-info/entry_points.txt
--rw-r--r--   0 luming     (501) staff       (20)       98 2023-03-09 10:25:06.000000 whochat-1.3.0/whochat.egg-info/requires.txt
--rw-r--r--   0 luming     (501) staff       (20)        8 2023-03-09 10:25:06.000000 whochat-1.3.0/whochat.egg-info/top_level.txt
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-09 01:34:30.518422 whochat-1.3.1/
+-rw-r--r--   0 luming     (501) staff       (20)     1514 2023-01-29 06:35:29.000000 whochat-1.3.1/LICENSE
+-rw-r--r--   0 luming     (501) staff       (20)       55 2023-01-29 06:35:29.000000 whochat-1.3.1/MANIFEST.in
+-rw-r--r--   0 luming     (501) staff       (20)     7287 2023-05-09 01:34:30.518512 whochat-1.3.1/PKG-INFO
+-rw-r--r--   0 luming     (501) staff       (20)     6634 2023-03-09 10:27:55.000000 whochat-1.3.1/README.md
+-rw-r--r--   0 luming     (501) staff       (20)     1284 2023-05-09 01:34:30.518855 whochat-1.3.1/setup.cfg
+-rw-r--r--   0 luming     (501) staff       (20)       38 2023-03-09 09:22:00.000000 whochat-1.3.1/setup.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-09 01:34:30.514279 whochat-1.3.1/whochat/
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-09 01:34:30.516096 whochat-1.3.1/whochat/ComWeChatRobot/
+-rw-r--r--   0 luming     (501) staff       (20)   165376 2023-02-13 09:38:48.000000 whochat-1.3.1/whochat/ComWeChatRobot/CWeChatRobot.exe
+-rw-r--r--   0 luming     (501) staff       (20)   293888 2023-02-13 09:38:48.000000 whochat-1.3.1/whochat/ComWeChatRobot/DWeChatRobot.dll
+-rw-r--r--   0 luming     (501) staff       (20)      472 2023-02-13 09:38:48.000000 whochat-1.3.1/whochat/ComWeChatRobot/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)       65 2023-05-09 01:34:19.000000 whochat-1.3.1/whochat/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)      107 2023-01-29 06:35:29.000000 whochat-1.3.1/whochat/__main__.py
+-rw-r--r--   0 luming     (501) staff       (20)      608 2023-02-13 09:38:48.000000 whochat-1.3.1/whochat/_comtypes.py
+-rw-r--r--   0 luming     (501) staff       (20)     6413 2023-02-13 09:38:48.000000 whochat-1.3.1/whochat/abc.py
+-rw-r--r--   0 luming     (501) staff       (20)    17254 2023-04-28 02:15:11.000000 whochat-1.3.1/whochat/bot.py
+-rw-r--r--   0 luming     (501) staff       (20)     4109 2023-04-25 10:04:39.000000 whochat-1.3.1/whochat/cli.py
+-rw-r--r--   0 luming     (501) staff       (20)      590 2023-04-25 10:04:39.000000 whochat-1.3.1/whochat/logger.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-09 01:34:30.516755 whochat-1.3.1/whochat/messages/
+-rw-r--r--   0 luming     (501) staff       (20)        0 2023-01-29 06:35:29.000000 whochat-1.3.1/whochat/messages/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)      447 2023-03-09 10:27:55.000000 whochat-1.3.1/whochat/messages/constants.py
+-rw-r--r--   0 luming     (501) staff       (20)     6875 2023-01-29 06:35:29.000000 whochat-1.3.1/whochat/messages/tcp.py
+-rw-r--r--   0 luming     (501) staff       (20)     6857 2023-04-25 09:55:38.000000 whochat-1.3.1/whochat/messages/websocket.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-09 01:34:30.517275 whochat-1.3.1/whochat/rpc/
+-rw-r--r--   0 luming     (501) staff       (20)       22 2023-01-29 06:35:29.000000 whochat-1.3.1/whochat/rpc/__init__.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-09 01:34:30.517713 whochat-1.3.1/whochat/rpc/clients/
+-rw-r--r--   0 luming     (501) staff       (20)        0 2023-03-09 10:27:55.000000 whochat-1.3.1/whochat/rpc/clients/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)     4314 2023-04-25 10:04:51.000000 whochat-1.3.1/whochat/rpc/clients/websocket.py
+-rw-r--r--   0 luming     (501) staff       (20)     1823 2023-03-09 10:27:55.000000 whochat-1.3.1/whochat/rpc/docs.py
+-rw-r--r--   0 luming     (501) staff       (20)     9767 2023-03-09 10:27:55.000000 whochat-1.3.1/whochat/rpc/handlers.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-09 01:34:30.518228 whochat-1.3.1/whochat/rpc/servers/
+-rw-r--r--   0 luming     (501) staff       (20)        0 2023-01-29 06:35:29.000000 whochat-1.3.1/whochat/rpc/servers/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)      930 2023-01-29 06:35:29.000000 whochat-1.3.1/whochat/rpc/servers/http.py
+-rw-r--r--   0 luming     (501) staff       (20)     1138 2023-04-25 09:55:38.000000 whochat-1.3.1/whochat/rpc/servers/websocket.py
+-rw-r--r--   0 luming     (501) staff       (20)      311 2023-04-25 10:04:39.000000 whochat-1.3.1/whochat/settings.py
+-rw-r--r--   0 luming     (501) staff       (20)     1108 2023-01-29 06:35:29.000000 whochat-1.3.1/whochat/signals.py
+-rw-r--r--   0 luming     (501) staff       (20)     3091 2023-03-09 10:27:55.000000 whochat-1.3.1/whochat/utils.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-09 01:34:30.515163 whochat-1.3.1/whochat.egg-info/
+-rw-r--r--   0 luming     (501) staff       (20)     7287 2023-05-09 01:34:30.000000 whochat-1.3.1/whochat.egg-info/PKG-INFO
+-rw-r--r--   0 luming     (501) staff       (20)      870 2023-05-09 01:34:30.000000 whochat-1.3.1/whochat.egg-info/SOURCES.txt
+-rw-r--r--   0 luming     (501) staff       (20)        1 2023-05-09 01:34:30.000000 whochat-1.3.1/whochat.egg-info/dependency_links.txt
+-rw-r--r--   0 luming     (501) staff       (20)       50 2023-05-09 01:34:30.000000 whochat-1.3.1/whochat.egg-info/entry_points.txt
+-rw-r--r--   0 luming     (501) staff       (20)      107 2023-05-09 01:34:30.000000 whochat-1.3.1/whochat.egg-info/requires.txt
+-rw-r--r--   0 luming     (501) staff       (20)        8 2023-05-09 01:34:30.000000 whochat-1.3.1/whochat.egg-info/top_level.txt
```

### Comparing `whochat-1.3.0/LICENSE` & `whochat-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whochat-1.3.0/PKG-INFO` & `whochat-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whochat
-Version: 1.3.0
+Version: 1.3.1
 Summary: 一个命令就可启用的微信机器人
 Home-page: https://github.com/amchii/whochat
 Author: Amchii
 Author-email: finethankuandyou@gmail.com
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/amchii/whochat
 Classifier: Intended Audience :: Developers
```

### Comparing `whochat-1.3.0/README.md` & `whochat-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `whochat-1.3.0/setup.cfg` & `whochat-1.3.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 	comtypes
 	psutil
 	click
 	websockets
 	jsonrpcserver
 	jsonrpcclient
 	schedule
+	pydantic
 
 [options.package_data]
 whochat.ComWeChatRobot = 
 	CWeChatRobot.exe
 	DWeChatRobot.dll
 
 [options.extras_require]
```

### Comparing `whochat-1.3.0/whochat/ComWeChatRobot/CWeChatRobot.exe` & `whochat-1.3.1/whochat/ComWeChatRobot/CWeChatRobot.exe`

 * *Files identical despite different names*

### Comparing `whochat-1.3.0/whochat/ComWeChatRobot/DWeChatRobot.dll` & `whochat-1.3.1/whochat/ComWeChatRobot/DWeChatRobot.dll`

 * *Files identical despite different names*

### Comparing `whochat-1.3.0/whochat/_comtypes.py` & `whochat-1.3.1/whochat/_comtypes.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.0/whochat/abc.py` & `whochat-1.3.1/whochat/abc.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.0/whochat/bot.py` & `whochat-1.3.1/whochat/bot.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.0/whochat/cli.py` & `whochat-1.3.1/whochat/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 def whochat(log_level: str):
     """
     微信机器人
 
     使用<子命令> --help查看使用说明
     """
     logger = logging.getLogger("whochat")
-    logging.getLevelName(log_level)
     logger.setLevel(log_level.upper())
 
 
 @whochat.command()
 def version():
     """显示程序和支持微信的版本信息"""
     from whochat import __version__
```

### Comparing `whochat-1.3.0/whochat/messages/tcp.py` & `whochat-1.3.1/whochat/messages/tcp.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.0/whochat/messages/websocket.py` & `whochat-1.3.1/whochat/messages/websocket.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import re
 import warnings
 from collections import deque
 from functools import partial
 from typing import Awaitable, Callable, List
 
 import websockets
-from websockets.legacy.client import WebSocketClientProtocol
+import websockets.client
+import websockets.server
 from websockets.typing import Data
 
 from whochat import _comtypes as comtypes
 from whochat.abc import RobotEventSinkABC
 from whochat.bot import WechatBotFactory
 from whochat.signals import Signal
 from whochat.utils import EventWaiter
@@ -45,15 +46,15 @@
                 data["extrainfo"] = None
             else:
                 data["extrainfo"] = self._parse_extrainfo(data["extrainfo"])
         except (json.JSONDecodeError, TypeError) as e:
             logger.warning("接收消息错误: ")
             logger.exception(e)
             return
-        logger.info(f"收到消息: {data}")
+        logger.debug(f"收到消息: {data}")
         self.deque_.append(data)
 
 
 class WechatMessageWebsocketServer:
     def __init__(
         self,
         wx_pids: List[int],
@@ -86,15 +87,15 @@
             if self.welcome:
                 await websocket.send("hello")
             await websocket.wait_closed()
             self.clients.remove(websocket)
             logger.info(f"Connection from {websocket.remote_address} was closed")
 
     async def serve_websocket(self):
-        async with websockets.serve(
+        async with websockets.server.serve(
             self.handler, self.ws_host, self.ws_port, **self.extra_kwargs
         ) as ws_server:
             logger.info(f"开始运行微信Websocket服务，地址为：<{self.ws_host}:{self.ws_port}>")
             self.ws_server = ws_server
             async with ws_server:
                 await self._stop_websocket.wait()
             logger.info("Websocket服务已停止")
@@ -152,15 +153,15 @@
         while not self._stop_broadcast:
             data = await self.queue.get()
             if not self._stop_broadcast:
                 self.broadcast(json.dumps(data))
         logger.info("广播已停止")
 
     def broadcast(self, data):
-        logger.info(f"广播消息：{data}")
+        logger.debug(f"广播消息：{data}")
         websockets.broadcast(self.clients, data)
 
     def shutdown(self):
         logger.info("停止服务中...")
         self.stop_websocket()
         self.stop_broadcast()
         self.stop_receive_msg()
@@ -188,15 +189,15 @@
         self,
         ws_uri: str,
     ):
         self.ws_uri = ws_uri
 
     async def start_consumer(self, on_message: Callable[[Data], Awaitable]):
         logger.info("Starting message consumer...")
-        async for websocket in websockets.connect(self.ws_uri):
-            websocket: WebSocketClientProtocol
+        async for websocket in websockets.client.connect(self.ws_uri):
+            websocket: "websockets.client.WebSocketClientProtocol"
             logger.info(f"Websocket client bind on {websocket.local_address}")
             try:
                 async for message in websocket:
                     await on_message(message)
             except websockets.ConnectionClosed:
                 continue
```

### Comparing `whochat-1.3.0/whochat/rpc/clients/websocket.py` & `whochat-1.3.1/whochat/rpc/clients/websocket.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import logging
 import time
 from collections import defaultdict
 from functools import partial
 from typing import Any, Dict
 
 import websockets
+import websockets.client
 from jsonrpcclient import request as req
-from websockets.legacy.client import WebSocketClientProtocol
 
 from whochat.rpc.handlers import make_rpc_methods
 
 logger = logging.getLogger("whochat")
 
 
 class unset:  # noqa
@@ -37,36 +37,40 @@
             logger.info(
                 f"Current size of results: {len(self._results)}, will remove {removable} items"
             )
             for k in list(self._results.keys())[:removable]:
                 self._results.pop(k, None)
             await asyncio.sleep(1)
 
-    async def start_sender(self, websocket: WebSocketClientProtocol):
+    async def start_sender(
+        self, websocket: "websockets.client.WebSocketClientProtocol"
+    ):
         while not websocket.closed:
             request_dict = await self.send_queue.get()
-            logger.info(f"SEND: {request_dict}")
+            logger.debug(f"SEND: {request_dict}")
             await websocket.send(json.dumps(request_dict))
 
-    async def start_receiver(self, websocket: WebSocketClientProtocol):
+    async def start_receiver(
+        self, websocket: "websockets.client.WebSocketClientProtocol"
+    ):
         async for message in websocket:
-            logger.info(f"RECV: {message}")
+            logger.debug(f"RECV: {message}")
             try:
                 response_dict = json.loads(message)
                 if "result" in response_dict:
                     self._results[response_dict["id"]] = response_dict["result"]
                 elif "error" in response_dict:
                     logger.error(response_dict["error"])
             except json.JSONDecodeError:
                 continue
 
     async def start_consumer(self):
         logger.info("Starting rpc client consumer")
-        async for websocket in websockets.connect(self.ws_uri):
-            websocket: WebSocketClientProtocol
+        async for websocket in websockets.client.connect(self.ws_uri):
+            websocket: "websockets.client.WebSocketClientProtocol"
             logger.info(f"Websocket client bind on {websocket.local_address}")
             try:
                 await asyncio.gather(
                     self.start_receiver(websocket),
                     self.start_sender(websocket),
                 )
             except websockets.ConnectionClosed:
```

### Comparing `whochat-1.3.0/whochat/rpc/docs.py` & `whochat-1.3.1/whochat/rpc/docs.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.0/whochat/rpc/handlers.py` & `whochat-1.3.1/whochat/rpc/handlers.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.0/whochat/rpc/servers/http.py` & `whochat-1.3.1/whochat/rpc/servers/http.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.0/whochat/rpc/servers/websocket.py` & `whochat-1.3.1/whochat/rpc/servers/websocket.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import asyncio
 import logging
 
-import websockets
+import websockets.server
 from jsonrpcserver import async_dispatch
-from websockets.legacy.server import WebSocketServerProtocol
 
 from whochat.signals import Signal
 
 logger = logging.getLogger("whochat")
 
 
 async def dispatch_in_task(websocket, request):
     res = await async_dispatch(request)
     await websocket.send(res)
 
 
-async def handler(websocket: WebSocketServerProtocol):
+async def handler(websocket: "websockets.server.WebSocketServerProtocol"):
     logger.info(f"Accept connection from {websocket.remote_address}")
     while not websocket.closed:
         request = await websocket.recv()
         asyncio.create_task(dispatch_in_task(websocket, request))
 
     logger.info(f"Connection from {websocket.remote_address} was closed")
 
@@ -31,10 +30,10 @@
         logger.info("正在停止微信机器人RPC websocket服务...")
         stop_event.set()
         from whochat.bot import WechatBotFactory
 
         WechatBotFactory.exit()
 
     Signal.register_sigint(shutdown)
-    async with websockets.serve(handler, host, port):
+    async with websockets.server.serve(handler, host, port):
         logger.info(f"运行微信机器人RPC websocket服务, 地址为<{host}:{port}>")
         await stop_event.wait()
```

### Comparing `whochat-1.3.0/whochat/signals.py` & `whochat-1.3.1/whochat/signals.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.0/whochat/utils.py` & `whochat-1.3.1/whochat/utils.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.0/whochat.egg-info/PKG-INFO` & `whochat-1.3.1/whochat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whochat
-Version: 1.3.0
+Version: 1.3.1
 Summary: 一个命令就可启用的微信机器人
 Home-page: https://github.com/amchii/whochat
 Author: Amchii
 Author-email: finethankuandyou@gmail.com
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/amchii/whochat
 Classifier: Intended Audience :: Developers
```

### Comparing `whochat-1.3.0/whochat.egg-info/SOURCES.txt` & `whochat-1.3.1/whochat.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 whochat/__init__.py
 whochat/__main__.py
 whochat/_comtypes.py
 whochat/abc.py
 whochat/bot.py
 whochat/cli.py
 whochat/logger.py
+whochat/settings.py
 whochat/signals.py
 whochat/utils.py
 whochat.egg-info/PKG-INFO
 whochat.egg-info/SOURCES.txt
 whochat.egg-info/dependency_links.txt
 whochat.egg-info/entry_points.txt
 whochat.egg-info/requires.txt
```

