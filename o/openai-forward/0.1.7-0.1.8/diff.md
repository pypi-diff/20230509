# Comparing `tmp/openai_forward-0.1.7.tar.gz` & `tmp/openai_forward-0.1.8.tar.gz`

## Comparing `openai_forward-0.1.7.tar` & `openai_forward-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/__init__.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/__main__.py
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/_base.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/app.py
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/config.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/openai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/content/__init__.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/content/chat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/content/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/routers/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/routers/openai_v1.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/routers/schemas.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 openai_forward-0.1.7/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.1.7/LICENSE
--rw-r--r--   0        0        0     7067 2020-02-02 00:00:00.000000 openai_forward-0.1.7/README.md
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 openai_forward-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 openai_forward-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.1.8/openai_forward/__init__.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 openai_forward-0.1.8/openai_forward/__main__.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 openai_forward-0.1.8/openai_forward/app.py
+-rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 openai_forward-0.1.8/openai_forward/base.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 openai_forward-0.1.8/openai_forward/config.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 openai_forward-0.1.8/openai_forward/openai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.8/openai_forward/content/__init__.py
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 openai_forward-0.1.8/openai_forward/content/chat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.8/openai_forward/content/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.8/openai_forward/routers/__init__.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 openai_forward-0.1.8/openai_forward/routers/openai_v1.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 openai_forward-0.1.8/openai_forward/routers/schemas.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 openai_forward-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.1.8/LICENSE
+-rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 openai_forward-0.1.8/README.md
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 openai_forward-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 openai_forward-0.1.8/PKG-INFO
```

### Comparing `openai_forward-0.1.7/openai_forward/__main__.py` & `openai_forward-0.1.8/openai_forward/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,36 +4,38 @@
 
 
 class Cli:
     @staticmethod
     def run(port=8000,
             workers=1,
             api_key=None,
-            base_url='https://api.openai.com',
-            log_chat='true',
+            base_url=None,
+            log_chat=None,
             route_prefix=None,
             ip_whitelist=None,
             ip_blacklist=None,
             ):
         """ Run forwarding serve.
 
         Parameters
         ----------
 
         port: int, default 8000
         workers: int, default 1
         api_key: str, default None
-        base_url: str, default 'https://api.openai.com'
-        log_chat: str, default 'true'
+        base_url: str, default None
+        log_chat: str, default None
         route_prefix: str, default None
         ip_whitelist: str, default None
         ip_blacklist: str, default None
         """
-        os.environ['OPENAI_BASE_URL'] = base_url
-        os.environ['LOG_CHAT'] = log_chat
+        if base_url:
+            os.environ['OPENAI_BASE_URL'] = base_url
+        if log_chat:
+            os.environ['LOG_CHAT'] = log_chat
         if api_key:
             os.environ['OPENAI_API_KEY'] = api_key
         if route_prefix:
             os.environ['ROUTE_PREFIX'] = route_prefix
         if ip_whitelist:
             os.environ['IP_WHITELIST'] = ip_whitelist
         if ip_blacklist:
```

### Comparing `openai_forward-0.1.7/openai_forward/_base.py` & `openai_forward-0.1.8/openai_forward/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 import os
 from itertools import cycle
 from .content.chat import parse_chat_completions, ChatSaver
 from .config import env2list
 
 
 class OpenaiBase:
-    _base_url = os.environ.get("OPENAI_BASE_URL", "https://api.openai.com").strip()
-    _LOG_CHAT = os.environ.get("LOG_CHAT", "False").lower() == "true"
-    _ROUTE_PREFIX = os.environ.get("ROUTE_PREFIX", "").strip()
-    _default_api_key_list = env2list("OPENAI_API_KEY", sep=" ")
-    _cycle_api_key = cycle(_default_api_key_list)
+    BASE_URL = os.environ.get("OPENAI_BASE_URL", "https://api.openai.com").strip()
+    ROUTE_PREFIX = os.environ.get("ROUTE_PREFIX", "").strip()
+    _LOG_CHAT = os.environ.get("LOG_CHAT", "False").strip().lower() == "true"
+    _openai_api_key_list = env2list("OPENAI_API_KEY", sep=" ")
+    _cycle_api_key = cycle(_openai_api_key_list)
+    _FWD_KEYS = env2list("FORWARD_KEY", sep=" ")
+    _use_forward_key = _openai_api_key_list != [] and _FWD_KEYS != []
     IP_WHITELIST = env2list("IP_WHITELIST", sep=" ")
     IP_BLACKLIST = env2list("IP_BLACKLIST", sep=" ")
 
-    if _ROUTE_PREFIX:
-        if _ROUTE_PREFIX.endswith('/'):
-            _ROUTE_PREFIX = _ROUTE_PREFIX[:-1]
-        if not _ROUTE_PREFIX.startswith('/'):
-            _ROUTE_PREFIX = '/' + _ROUTE_PREFIX
+    if ROUTE_PREFIX:
+        if ROUTE_PREFIX.endswith('/'):
+            ROUTE_PREFIX = ROUTE_PREFIX[:-1]
+        if not ROUTE_PREFIX.startswith('/'):
+            ROUTE_PREFIX = '/' + ROUTE_PREFIX
     timeout = 30
     chatsaver = ChatSaver(save_interval=10)
 
     def validate_request_host(self, ip):
         if self.IP_WHITELIST and ip not in self.IP_WHITELIST:
             raise HTTPException(status_code=status.HTTP_403_FORBIDDEN,
                                 detail=f"Forbidden, ip={ip} not in whitelist!")
@@ -50,55 +52,65 @@
         except Exception as e:
             logger.debug(f"log chat (not) error:\n{e=}")
 
     @classmethod
     async def _reverse_proxy(cls, request: Request):
         client: httpx.AsyncClient = request.app.state.client
         url_path = request.url.path
-        url_path = url_path[len(cls._ROUTE_PREFIX):]
+        url_path = url_path[len(cls.ROUTE_PREFIX):]
         url = httpx.URL(path=url_path, query=request.url.query.encode('utf-8'))
         headers = dict(request.headers)
         auth = headers.pop("authorization", None)
         if auth and str(auth).startswith("Bearer sk-"):
             tmp_headers = {'Authorization': auth}
-        elif cls._default_api_key_list:
-            auth = "Bearer " + next(cls._cycle_api_key)
-            tmp_headers = {'Authorization': auth}
+        elif cls._openai_api_key_list:
+            logger.info(f"Use forward key: {cls._use_forward_key}")
+            if cls._use_forward_key:
+                fk_prefix = "Bearer fk-"
+                logger.info(f"current forward key: {auth}")
+                if auth and str(auth).startswith(fk_prefix) and auth[len("Bearer "):] in cls._FWD_KEYS:
+                    auth = "Bearer " + next(cls._cycle_api_key)
+                    tmp_headers = {'Authorization': auth}
+                else:
+                    tmp_headers = {}
+            else:
+                auth = "Bearer " + next(cls._cycle_api_key)
+                tmp_headers = {'Authorization': auth}
         else:
             tmp_headers = {}
 
-        headers.pop("host", None)
-        headers.update(tmp_headers)
         if cls._LOG_CHAT:
             try:
                 input_info = await request.json()
                 msgs = input_info['messages']
                 cls.chatsaver.add_chat({
                     "host": request.client.host,
                     "model": input_info['model'],
                     "messages": [{msg['role']: msg['content']} for msg in msgs],
                 })
             except Exception as e:
                 logger.debug(f"log chat (not) error:\n{request.client.host=}: {e}")
+
+        headers.pop("host", None)
+        headers.update(tmp_headers)
+
         req = client.build_request(
             request.method, url, headers=headers,
             content=request.stream(),
             timeout=cls.timeout,
         )
-        logger.warning(f"{url=}")
-
         try:
             r = await client.send(req, stream=True)
-        except httpx.ConnectError as e:
+        except (httpx.ConnectError, httpx.ConnectTimeout) as e:
             error_info = f"{type(e)}: {e} | " \
-                         f"Please check if host={request.client.host} can access [{cls._base_url}] successfully."
+                         f"Please check if host={request.client.host} can access [{cls.BASE_URL}] successfully."
             logger.error(error_info)
             raise HTTPException(status_code=status.HTTP_504_GATEWAY_TIMEOUT, detail=error_info)
         except Exception as e:
-            error_info = f"{type(e)}: {str(e)}"
+            error_info = f"{type(e)}: {e}"
             logger.error(error_info)
             raise HTTPException(status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=error_info)
 
         aiter_bytes = cls.aiter_bytes(r) if cls._LOG_CHAT else r.aiter_bytes()
         return StreamingResponse(
             aiter_bytes,
             status_code=r.status_code,
```

### Comparing `openai_forward-0.1.7/openai_forward/app.py` & `openai_forward-0.1.8/openai_forward/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 app = create_app(title="openai_forward", version="1.0")
 openai = Openai()
 use_http2 = False
 
 
 @app.on_event('startup')
 async def startup_event():
-    app.state.client = httpx.AsyncClient(base_url=Openai._base_url, http2=use_http2)
+    app.state.client = httpx.AsyncClient(base_url=Openai.BASE_URL, http2=use_http2)
 
 
 @app.on_event('shutdown')
 async def shutdown_event():
     await app.state.client.aclose()
 
 
-app.add_route(openai._ROUTE_PREFIX + '/{api_path:path}', openai.reverse_proxy,
+app.add_route(openai.ROUTE_PREFIX + '/{api_path:path}', openai.reverse_proxy,
               methods=['GET', 'POST', 'PUT', 'DELETE', 'OPTIONS', 'HEAD', 'PATCH', 'TRACE'])
 app.include_router(router_v1)
```

### Comparing `openai_forward-0.1.7/openai_forward/config.py` & `openai_forward-0.1.8/openai_forward/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 import orjson
 from sparrow import relp
 from typing import Union, List, Dict
 import sys
 import logging
 import os
 import time
-import pytz
 
 
 class InterceptHandler(logging.Handler):
     def emit(self, record):
         # Get corresponding Loguru level if it exists
         try:
             level = logger.level(record.levelname).name
         except ValueError:
             level = record.levelno
 
         # Find caller from where originated the logged message
-        frame, depth = logging.currentframe(), 2
+        frame, depth = logging.currentframe(), 6
         while frame.f_code.co_filename == logging.__file__:
             frame = frame.f_back
             depth += 1
         logger.opt(depth=depth, exception=record.exc_info).log(level, record.getMessage())
 
 
 def setting_log(log_name, multi_process=True):
@@ -35,16 +34,16 @@
 
     logging.root.handlers = [InterceptHandler()]
     for name in logging.root.manager.loggerDict.keys():
         logging.getLogger(name).handlers = []
         logging.getLogger(name).propagate = True
     logger_config = {
         "handlers": [
-            {"sink": sys.stdout},
-            {"sink": f"./Log/{log_name}", "enqueue": multi_process, "rotation": "100 MB"},
+            {"sink": sys.stdout, "level": "DEBUG"},
+            {"sink": f"./Log/{log_name}.log", "enqueue": multi_process, "rotation": "100 MB", "level": "INFO"},
         ],
     }
     logger.configure(**logger_config)
 
 
 def yaml_dump(data, filepath, rel_path=False, mode='w'):
     abs_path = relp(filepath, parents=1) if rel_path else filepath
```

### Comparing `openai_forward-0.1.7/openai_forward/openai.py` & `openai_forward-0.1.8/openai_forward/openai.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from ._base import OpenaiBase
+from .base import OpenaiBase
 from .routers.schemas import OpenAIV1ChatCompletion
 from fastapi import Request
 from .config import setting_log
 
-setting_log(log_name="openai_forward.log")
+setting_log(log_name="openai_forward")
 
 
 class Openai(OpenaiBase):
     def __init__(self):
         if self.IP_BLACKLIST or self.IP_WHITELIST:
             self.validate_host = True
         else:
```

### Comparing `openai_forward-0.1.7/openai_forward/content/chat.py` & `openai_forward-0.1.8/openai_forward/content/chat.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.7/openai_forward/routers/schemas.py` & `openai_forward-0.1.8/openai_forward/routers/schemas.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.7/.gitignore` & `openai_forward-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.7/LICENSE` & `openai_forward-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.7/pyproject.toml` & `openai_forward-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "openai_forward"
-description = "🚀 Openai api forward · OpenAI 接口转发服务 · streaming forward"
+description = "🚀 Openai api forward · OpenAI 接口转发服务 · stream forwarding"
 authors = [
     { name = "kunyuan", email = "beidongjiedeguang@gmail.com" },
 ]
 requires-python = ">=3.6"
 readme = "README.md"
 keywords = ["openai", "chatgpt", "openai-api", "openai-proxy", "forward", "streaming-api", "fastapi", "python"]
 classifiers = [
```

### Comparing `openai_forward-0.1.7/PKG-INFO` & `openai_forward-0.1.8/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: openai_forward
-Version: 0.1.7
-Summary: 🚀 Openai api forward · OpenAI 接口转发服务 · streaming forward
+Version: 0.1.8
+Summary: 🚀 Openai api forward · OpenAI 接口转发服务 · stream forwarding
 Project-URL: Homepage, https://github.com/beidongjiedeguang/openai-forward
 Project-URL: Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-forward
 Project-URL: Issues, https://github.com/beidongjiedeguang/openai-forward/issues
 Project-URL: Source, https://github.com/beidongjiedeguang/openai-forward
 Author-email: kunyuan <beidongjiedeguang@gmail.com>
 License-File: LICENSE
 Keywords: chatgpt,fastapi,forward,openai,openai-api,openai-proxy,python,streaming-api
@@ -27,15 +27,15 @@
 Requires-Dist: revchatgpt; extra == 'chatgpt'
 Provides-Extra: edge
 Requires-Dist: edgegpt; extra == 'edge'
 Provides-Extra: ssl
 Requires-Dist: certbot; extra == 'ssl'
 Description-Content-Type: text/markdown
 
-[**中文**](./README_ZH.md) | **English**
+**中文** | [**English**](./README_EN.md)
 
 <h1 align="center">
     <br>
     OpenAI Forward
     <br>
 </h1>
 <p align="center">
@@ -62,182 +62,240 @@
     </a>
     <a href="https://pypi.org/project/openai_forward/">
         <img alt="pypi downloads" src="https://img.shields.io/pypi/dm/openai_forward">
     </a>
     <a href="https://codecov.io/gh/beidongjiedeguang/openai-forward">
         <img alt="codecov" src="https://codecov.io/gh/beidongjiedeguang/openai-forward/branch/dev/graph/badge.svg">
     </a>
-
 </p>
-This project is designed to solve the problem of some regions being unable to directly access OpenAI. The service is deployed on a server that can access the OpenAI API, and OpenAI requests are forwarded through the service, i.e. a reverse proxy service is set up. 
 
-Test access: https://caloi.top/openai/v1/chat/completions is equivalent to https://api.openai.com/v1/chat/completions  
-Or, to put it another way, https://caloi.top/openai is equivalent to https://api.openai.com.
+
+
+本项目用于解决一些地区无法直接访问OpenAI的问题，将该服务部署在可以正常访问openai
+api的服务器上，通过该服务转发OpenAI的请求。即搭建反向代理服务  
+测试访问：https://caloi.top/openai/v1/chat/completions 将等价于 https://api.openai.com/v1/chat/completions  
+或者说 https://caloi.top/openai 等价于 https://api.openai.com
 
 # Table of Contents
 
 - [Features](#Features)
-- [Usage](#Usage)
-- [Deploy](#Deploy)
-- [Service Usage](#Service-Usage)
-- [Configuration](#Configuration)
-- [Chat Log](#Chat-log)
+- [应用](#应用)
+- [安装部署](#安装部署)
+- [服务调用](#服务调用)
+- [配置选项](#配置选项)
+- [聊天日志](#聊天日志)
+- [高级配置](#高级配置)
 
 # Features
 
-- [x] Supports forwarding of all OpenAI interfaces
-- [x] Request IP verification
-- [x] Streaming Response
-- [x] Supports default API key (cyclic call with multiple API keys)
-- [x] pip installation and deployment
-- [x] Docker deployment
-- [x] Support for multiple worker processes
-- [x] Support for specifying the forwarding routing prefix
+- [x] 支持转发OpenAI所有接口
+- [x] 支持流式响应
+- [x] 实时记录聊天记录(包括流式响应的聊天内容)
+- [x] 支持默认openai api key(多api key 循环调用)
+- [x] 转发api key (在已设置默认openai api key情况下使用)
+- [x] docker部署
+- [x] 支持指定转发路由前缀
+- [x] 支持请求IP验证
 
-# Usage
+# 应用
 
-> Here, the proxy address set up by the individual, https://caloi.top/openai, is used as an example
+> 这里以个人使用该项目搭建好的代理服务 https://caloi.top/openai 为例
 
-### Using in a module
+### [caloi.top](https://caloi.top)
 
+基于开源项目[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)搭建自己的chatgpt服务  
+替换docker启动命令中的 `BASE_URL`为我们自己搭建的代理服务地址
 
-**Python**
+```bash 
+docker run -d \
+    -p 3000:3000 \
+    -e OPENAI_API_KEY="sk-******" \
+    -e BASE_URL="caloi.top/openai" \
+    -e CODE="<your password>" \
+    yidadaa/chatgpt-next-web 
+``` 
 
-```diff
-  import openai
-+ openai.api_base = "https://caloi.top/openai/v1"
-  openai.api_key = "sk-******"
-```
+访问 https://caloi.top 。访问密码为 `beidongjiedeguang`
+
+### 在模块中使用
 
 **JS/TS**
 
 ```diff
   import { Configuration } from "openai";
   
   const configuration = new Configuration({
 + basePath: "https://caloi.top/openai/v1",
   apiKey: "sk-******",
   });
 ```
 
+**Python**
+
+```diff
+  import openai
++ openai.api_base = "https://caloi.top/openai/v1"
+  openai.api_key = "sk-******"
+```
 
 ### Image Generation (DALL-E):
 
-```bash 
-curl --location 'https://caloi.top/openai/v1/images/generations' \ 
---header 'Authorization: Bearer sk-******' \ 
---header 'Content-Type: application/json' \ 
---data '{ 
-    "prompt": "A photo of a cat", 
-    "n": 1, 
+```bash
+curl --location 'https://caloi.top/openai/v1/images/generations' \
+--header 'Authorization: Bearer sk-******' \
+--header 'Content-Type: application/json' \
+--data '{
+    "prompt": "A photo of a cat",
+    "n": 1,
     "size": "512x512"
-}' 
-``` 
+}'
+```
 
-### [chatgpt-web](https://github.com/Chanzhaoyu/chatgpt-web)
+# 安装部署
 
-Modify the `OPENAI_API_BASE_URL` in [Docker Compose](https://github.com/Chanzhaoyu/chatgpt-web#docker-compose) to the
-address of the proxy service we set up:
+提供3种服务部署方式,选择一种即可
 
-```bash 
-OPENAI_API_BASE_URL: https://caloi.top/openai 
-``` 
+## pip
+pip的安装方式目前在使用nginx反向代理时存在Bug, 建议使用Docker方式部署。  
+**安装**
 
-### [ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)
-
-Replace `BASE_URL` in the docker startup command with the address of the proxy service we set up:
+```bash
+pip install openai-forward
+```
 
-```bash 
-docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -e CODE="<your password>" -e BASE_URL="caloi.top/openai" yidadaa/chatgpt-next-web 
-``` 
+**运行转发服务**  
+可通过`--port`指定端口号，默认为`8000`，可通过`--workers`指定工作进程数，默认为`1`
 
+```bash
+openai_forward run --port=9999 --workers=1
+```
 
-# Deploy
+服务就搭建完成了，使用方式只需将`https://api.openai.com` 替换为服务所在端口`http://{ip}:{port}` 即可。
 
-Two deployment methods are provided, just choose one.
+当然也可以将 OPENAI_API_KEY 作为环境变量传入作为默认api key， 这样客户端在请求相关路由时可以无需在Header中传入Authorization。
+带默认api key的启动方式：
 
-## Use `pip`  (recommended)
+```bash
+OPENAI_API_KEY="sk-xxx" openai_forward run --port=9999 --workers=1
+```
 
-**Installation**
+注: 如果既存在默认api key又在请求头中传入了api key，则以请求头中的api key会覆盖默认api key.
 
-```bash 
-pip install openai-forward 
-``` 
+## Docker (推荐)
 
-**Run forwarding service**
-The port number can be specified through `--port`, which defaults to `8000`, and the number of worker processes can be
-specified through `--workers`, which defaults to `1`.
+```bash
+docker run --name="openai-forward" -d -p 9999:8000 beidongjiedeguang/openai-forward:latest 
+```
 
-```bash 
-openai_forward run --port=9999 --workers=1 
-``` 
+将映射宿主机的9999端口，通过`http://{ip}:9999`访问服务。  
+注：同样可以在启动命令中通过-e传入环境变量OPENAI_API_KEY=sk-xxx作为默认api key
 
-The service is now set up, and the usage is to replace `https://api.openai.com` with the port number of the
-service `http://{ip}:{port}`.
+## 源码部署
 
-Of course, OPENAI_API_KEY can also be passed in as an environment variable as the default API key, so that the client
-does not need to pass in the Authorization in the header when requesting the relevant route.
-Startup command with default API key:
+```bash
+git clone https://github.com/beidongjiedeguang/openai-forward.git --depth=1
+cd openai-forward
+```
 
-```bash 
-OPENAI_API_KEY="sk-xxx" openai_forward run --port=9999 --workers=1 
-``` 
+**使用 docker**
 
-Note: If both the default API key and the API key passed in the request header exist, the API key in the request header
-will override the default API key.
+```bash
+docker-compose up
+```
 
-## Use Docker
+**或使用pip**
 
-```bash 
-docker run --name="openai-forward" -d -p 9999:8000 beidongjiedeguang/openai-forward:latest 
-``` 
+```bash
+pip install -e .
+openai-forward run 
+```
 
-The 9999 port of the host is mapped, and the service can be accessed through `http://{ip}:9999`.
-Note: You can also pass in the environment variable OPENAI_API_KEY=sk-xxx as the default API key in the startup command.
+# 服务调用
 
-# Service Usage
+替换openai的api地址为该服务的地址即可，如：
 
-Simply replace the OpenAI API address with the address of the service we set up, such as `Chat Completion`
-```bash 
-https://api.openai.com/v1/chat/completions 
-``` 
+```bash
+https://api.openai.com/v1/chat/completions
+```
 
-Replace with
+替换为
 
-```bash 
-http://{ip}:{port}/v1/chat/completions 
+```bash
+http://{ip}:{port}/v1/chat/completions
 ```
 
-# Configuration
+# 配置选项
 
-**`openai-forward run` Parameter Configuration Options**
+**`openai-forward run`参数配置项**
 
-| Configuration Option | Description | Default Value |
+| 配置项       | 说明 | 默认值 |
 |-----------| --- | :---: |
-| --port    | Service port number | 8000 |
-| --workers | Number of worker processes | 1 |
+| --port    | 服务端口号 | 8000 |
+| --workers | 工作进程数 | 1 |
+
+**环境变量配置项**  
+参考项目根目录下`.env`文件
 
-**Environment Variable Configuration Options**  
-refer to the `.env` file in the project root directory
+| 环境变量            | 说明                                                              |           默认值            |
+|-----------------|-----------------------------------------------------------------|:------------------------:|
+| OPENAI_API_KEY  | 默认openai api key，支持多个默认api key, 以 `sk-` 开头， 以空格分割      |            无             |
+| FORWARD_KEY     | 允许调用方使用该key代替openai api key，支持多个forward key, 以`fk-` 开头, 以空格分割 |      无             |
+| OPENAI_BASE_URL | 转发base url                                                      | `https://api.openai.com` |
+| LOG_CHAT        | 是否记录聊天内容                                                        |          `true`          |
+| ROUTE_PREFIX    | 路由前缀                                                            |            无             |
+| IP_WHITELIST    | ip白名单, 空格分开                                                     |           无            |
+| IP_BLACKLIST    | ip黑名单, 空格分开                                                     |           无            | 
+
+# 聊天日志
+
+保存路径在当前目录下的`Log/`路径中。  
+聊天日志以 `chat_`开头, 默认每5轮对话写入一次文件    
+记录格式为
 
-| Environment Variable  | Description | Default Value |
-|-----------------|------------|:------------------------:|
-| OPENAI_API_KEY  | Default API key, supports multiple default API keys separated by space. | None |
-| OPENAI_BASE_URL | Forwarding base URL | `https://api.openai.com` |
-|LOG_CHAT| Whether to log chat content | `true` |
-|ROUTE_PREFIX| Route prefix | None |
-| IP_WHITELIST    | IP whitelist, separated by space. | None |
-| IP_BLACKLIST    | IP blacklist, separated by space. | None |
-
-# Chat Log
-The saved path is in the `Log/` directory under the current directory.  
-The chat log starts with `chat_` and is written to the file every 5 rounds by default.  
-The recording format is as follows:
 ```text
 {'host': xxx, 'model': xxx, 'message': [{'user': xxx}, {'assistant': xxx}]}
 {'assistant': xxx}
 
 {'host': ...}
 {'assistant': ...}
 
 ...
-```
+```
+
+# 高级配置
+
+**设置api_key为自己设置的forward key**  
+需要配置 OPENAI_API_KEY 和 FORWARD_KEY, 例如
+
+```bash
+OPENAI_API_KEY=sk-*******
+FORWARD_KEY=fk-****** # 这里fk-token由我们自己定义
+```
+这里我们配置了FORWARD_KEY为`fk-******`, 那么后面客户端在调用时只需设置OPENAI_API_KEY为我们自定义的`fk-******` 即可。  
+这样的好处是在使用一些需要输入OPENAI_API_KEY的第三方应用时，我们可以使用`fk-******`搭配proxy使用（如下面的例子） 而无需担心OPENAI_API_KEY被泄露。
+
+**用例:**
+```bash
+curl https://caloi.top/openai/v1/chat/completions \
+  -H "Content-Type: application/json" \
+  -H "Authorization: Bearer fk-******" \
+  -d '{
+    "model": "gpt-3.5-turbo",
+    "messages": [{"role": "user", "content": "Hello!"}]
+  }'
+```
+**Python**
+```diff
+  import openai
++ openai.api_base = "https://caloi.top/openai/v1"
+- openai.api_key = "sk-******"
++ openai.api_key = "fk-******"
+```
+**Web application**
+```bash 
+docker run -d \
+    -p 3000:3000 \
+    -e OPENAI_API_KEY="fk-******" \
+    -e BASE_URL="caloi.top/openai" \
+    -e CODE="<your password>" \
+    yidadaa/chatgpt-next-web 
+```
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: openai_forward Version: 0.1.7 Summary: ð Openai
-api forward Â· OpenAI æ¥å£è½¬åæå¡ Â· streaming forward Project-URL:
+Metadata-Version: 2.1 Name: openai_forward Version: 0.1.8 Summary: ð Openai
+api forward Â· OpenAI æ¥å£è½¬åæå¡ Â· stream forwarding Project-URL:
 Homepage, https://github.com/beidongjiedeguang/openai-forward Project-URL:
 Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-
 forward Project-URL: Issues, https://github.com/beidongjiedeguang/openai-
 forward/issues Project-URL: Source, https://github.com/beidongjiedeguang/
 openai-forward Author-email: kunyuan
 gmail.com> License-File: LICENSE Keywords:
 chatgpt,fastapi,forward,openai,openai-api,openai-proxy,python,streaming-api
@@ -11,83 +11,102 @@
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6 Requires-Dist: fastapi Requires-Dist: httpx Requires-
 Dist: loguru Requires-Dist: orjson Requires-Dist: python-dotenv Requires-Dist:
 pytz Requires-Dist: sparrow-python>=0.1.2 Requires-Dist: uvicorn Provides-
 Extra: bard Requires-Dist: googlebard; extra == 'bard' Provides-Extra: chatgpt
 Requires-Dist: revchatgpt; extra == 'chatgpt' Provides-Extra: edge Requires-
 Dist: edgegpt; extra == 'edge' Provides-Extra: ssl Requires-Dist: certbot;
-extra == 'ssl' Description-Content-Type: text/markdown [**ä¸­æ**](./
-README_ZH.md) | **English**
+extra == 'ssl' Description-Content-Type: text/markdown **ä¸­æ** |
+[**English**](./README_EN.md)
                                     ******
                                 OpenAI Forward
                                      ******
                         OpenAI API æ¥å£è½¬åæå¡
                 The fastest way to deploy openai api forwarding
  [PyPI_version] [License] [Release_(latest_by_date)] [GitHub_repo_size] [docer
                 image_size] [tests] [pypi_downloads] [codecov]
-This project is designed to solve the problem of some regions being unable to
-directly access OpenAI. The service is deployed on a server that can access the
-OpenAI API, and OpenAI requests are forwarded through the service, i.e. a
-reverse proxy service is set up. Test access: https://caloi.top/openai/v1/chat/
-completions is equivalent to https://api.openai.com/v1/chat/completions Or, to
-put it another way, https://caloi.top/openai is equivalent to https://
-api.openai.com. # Table of Contents - [Features](#Features) - [Usage](#Usage) -
-[Deploy](#Deploy) - [Service Usage](#Service-Usage) - [Configuration]
-(#Configuration) - [Chat Log](#Chat-log) # Features - [x] Supports forwarding
-of all OpenAI interfaces - [x] Request IP verification - [x] Streaming Response
-- [x] Supports default API key (cyclic call with multiple API keys) - [x] pip
-installation and deployment - [x] Docker deployment - [x] Support for multiple
-worker processes - [x] Support for specifying the forwarding routing prefix #
-Usage > Here, the proxy address set up by the individual, https://caloi.top/
-openai, is used as an example ### Using in a module **Python** ```diff import
-openai + openai.api_base = "https://caloi.top/openai/v1" openai.api_key = "sk-
-******" ``` **JS/TS** ```diff import { Configuration } from "openai"; const
-configuration = new Configuration({ + basePath: "https://caloi.top/openai/v1",
-apiKey: "sk-******", }); ``` ### Image Generation (DALL-E): ```bash curl --
-location 'https://caloi.top/openai/v1/images/generations' \ --header
+æ¬é¡¹ç®ç¨äºè§£å³ä¸äºå°åºæ æ³ç´æ¥è®¿é®OpenAIçé®é¢ï¼å°è¯¥æå¡é¨ç½²å¨å¯ä»¥æ­£å¸¸è®¿é®openai
+apiçæå¡å¨ä¸ï¼éè¿è¯¥æå¡è½¬åOpenAIçè¯·æ±ãå³æ­å»ºååä»£çæå¡
+æµè¯è®¿é®ï¼https://caloi.top/openai/v1/chat/completions å°ç­ä»·äº https:
+//api.openai.com/v1/chat/completions æèè¯´ https://caloi.top/openai
+ç­ä»·äº https://api.openai.com # Table of Contents - [Features](#Features) -
+[åºç¨](#åºç¨) - [å®è£é¨ç½²](#å®è£é¨ç½²) - [æå¡è°ç¨]
+(#æå¡è°ç¨) - [éç½®éé¡¹](#éç½®éé¡¹) - [èå¤©æ¥å¿](#èå¤©æ¥å¿)
+- [é«çº§éç½®](#é«çº§éç½®) # Features - [x] æ¯æè½¬åOpenAIæææ¥å£
+- [x] æ¯ææµå¼ååº - [x] å®æ¶è®°å½èå¤©è®°å½
+(åæ¬æµå¼ååºçèå¤©åå®¹) - [x] æ¯æé»è®¤openai api key(å¤api key
+å¾ªç¯è°ç¨) - [x] è½¬åapi key (å¨å·²è®¾ç½®é»è®¤openai api
+keyæåµä¸ä½¿ç¨) - [x] dockeré¨ç½² - [x] æ¯ææå®è½¬åè·¯ç±åç¼ -
+[x] æ¯æè¯·æ±IPéªè¯ # åºç¨ >
+è¿éä»¥ä¸ªäººä½¿ç¨è¯¥é¡¹ç®æ­å»ºå¥½çä»£çæå¡ https://caloi.top/openai
+ä¸ºä¾ ### [caloi.top](https://caloi.top) åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web]
+(https://github.com/Yidadaa/ChatGPT-Next-Web)æ­å»ºèªå·±çchatgptæå¡
+æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç
+`BASE_URL`ä¸ºæä»¬èªå·±æ­å»ºçä»£çæå¡å°å ```bash docker run -d \ -
+p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -e BASE_URL="caloi.top/openai" \
+-e CODE="" \ yidadaa/chatgpt-next-web ``` è®¿é® https://caloi.top
+ãè®¿é®å¯ç ä¸º `beidongjiedeguang` ### å¨æ¨¡åä¸­ä½¿ç¨ **JS/TS** ```diff
+import { Configuration } from "openai"; const configuration = new Configuration
+({ + basePath: "https://caloi.top/openai/v1", apiKey: "sk-******", }); ```
+**Python** ```diff import openai + openai.api_base = "https://caloi.top/openai/
+v1" openai.api_key = "sk-******" ``` ### Image Generation (DALL-E): ```bash
+curl --location 'https://caloi.top/openai/v1/images/generations' \ --header
 'Authorization: Bearer sk-******' \ --header 'Content-Type: application/json' \
---data '{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ``` ###
-[chatgpt-web](https://github.com/Chanzhaoyu/chatgpt-web) Modify the
-`OPENAI_API_BASE_URL` in [Docker Compose](https://github.com/Chanzhaoyu/
-chatgpt-web#docker-compose) to the address of the proxy service we set up:
-```bash OPENAI_API_BASE_URL: https://caloi.top/openai ``` ### [ChatGPT-Next-
-Web](https://github.com/Yidadaa/ChatGPT-Next-Web) Replace `BASE_URL` in the
-docker startup command with the address of the proxy service we set up: ```bash
-docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -e CODE="" -
-e BASE_URL="caloi.top/openai" yidadaa/chatgpt-next-web ``` # Deploy Two
-deployment methods are provided, just choose one. ## Use `pip` (recommended)
-**Installation** ```bash pip install openai-forward ``` **Run forwarding
-service** The port number can be specified through `--port`, which defaults to
-`8000`, and the number of worker processes can be specified through `--
-workers`, which defaults to `1`. ```bash openai_forward run --port=9999 --
-workers=1 ``` The service is now set up, and the usage is to replace `https://
-api.openai.com` with the port number of the service `http://{ip}:{port}`. Of
-course, OPENAI_API_KEY can also be passed in as an environment variable as the
-default API key, so that the client does not need to pass in the Authorization
-in the header when requesting the relevant route. Startup command with default
-API key: ```bash OPENAI_API_KEY="sk-xxx" openai_forward run --port=9999 --
-workers=1 ``` Note: If both the default API key and the API key passed in the
-request header exist, the API key in the request header will override the
-default API key. ## Use Docker ```bash docker run --name="openai-forward" -d -
-p 9999:8000 beidongjiedeguang/openai-forward:latest ``` The 9999 port of the
-host is mapped, and the service can be accessed through `http://{ip}:9999`.
-Note: You can also pass in the environment variable OPENAI_API_KEY=sk-xxx as
-the default API key in the startup command. # Service Usage Simply replace the
-OpenAI API address with the address of the service we set up, such as `Chat
-Completion` ```bash https://api.openai.com/v1/chat/completions ``` Replace with
-```bash http://{ip}:{port}/v1/chat/completions ``` # Configuration **`openai-
-forward run` Parameter Configuration Options** | Configuration Option |
-Description | Default Value | |-----------| --- | :---: | | --port | Service
-port number | 8000 | | --workers | Number of worker processes | 1 |
-**Environment Variable Configuration Options** refer to the `.env` file in the
-project root directory | Environment Variable | Description | Default Value |
-|-----------------|------------|:------------------------:| | OPENAI_API_KEY |
-Default API key, supports multiple default API keys separated by space. | None
-| | OPENAI_BASE_URL | Forwarding base URL | `https://api.openai.com` |
-|LOG_CHAT| Whether to log chat content | `true` | |ROUTE_PREFIX| Route prefix |
-None | | IP_WHITELIST | IP whitelist, separated by space. | None | |
-IP_BLACKLIST | IP blacklist, separated by space. | None | # Chat Log The saved
-path is in the `Log/` directory under the current directory. The chat log
-starts with `chat_` and is written to the file every 5 rounds by default. The
-recording format is as follows: ```text {'host': xxx, 'model': xxx, 'message':
-[{'user': xxx}, {'assistant': xxx}]} {'assistant': xxx} {'host': ...}
-{'assistant': ...} ... ```
+--data '{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ``` #
+å®è£é¨ç½² æä¾3ç§æå¡é¨ç½²æ¹å¼,éæ©ä¸ç§å³å¯ ## pip
+pipçå®è£æ¹å¼ç®åå¨ä½¿ç¨nginxååä»£çæ¶å­å¨Bug,
+å»ºè®®ä½¿ç¨Dockeræ¹å¼é¨ç½²ã **å®è£** ```bash pip install openai-forward
+``` **è¿è¡è½¬åæå¡** å¯éè¿`--
+port`æå®ç«¯å£å·ï¼é»è®¤ä¸º`8000`ï¼å¯éè¿`--
+workers`æå®å·¥ä½è¿ç¨æ°ï¼é»è®¤ä¸º`1` ```bash openai_forward run --
+port=9999 --workers=1 ```
+æå¡å°±æ­å»ºå®æäºï¼ä½¿ç¨æ¹å¼åªéå°`https://api.openai.com`
+æ¿æ¢ä¸ºæå¡æå¨ç«¯å£`http://{ip}:{port}` å³å¯ã å½ç¶ä¹å¯ä»¥å°
+OPENAI_API_KEY ä½ä¸ºç¯å¢åéä¼ å¥ä½ä¸ºé»è®¤api keyï¼
+è¿æ ·å®¢æ·ç«¯å¨è¯·æ±ç¸å³è·¯ç±æ¶å¯ä»¥æ éå¨Headerä¸­ä¼ å¥Authorizationã
+å¸¦é»è®¤api keyçå¯å¨æ¹å¼ï¼ ```bash OPENAI_API_KEY="sk-xxx"
+openai_forward run --port=9999 --workers=1 ``` æ³¨: å¦ææ¢å­å¨é»è®¤api
+keyåå¨è¯·æ±å¤´ä¸­ä¼ å¥äºapi keyï¼åä»¥è¯·æ±å¤´ä¸­çapi
+keyä¼è¦çé»è®¤api key. ## Docker (æ¨è) ```bash docker run --
+name="openai-forward" -d -p 9999:8000 beidongjiedeguang/openai-forward:latest
+``` å°æ å°å®¿ä¸»æºç9999ç«¯å£ï¼éè¿`http://{ip}:9999`è®¿é®æå¡ã
+æ³¨ï¼åæ ·å¯ä»¥å¨å¯å¨å½ä»¤ä¸­éè¿-
+eä¼ å¥ç¯å¢åéOPENAI_API_KEY=sk-xxxä½ä¸ºé»è®¤api key ## æºç é¨ç½²
+```bash git clone https://github.com/beidongjiedeguang/openai-forward.git --
+depth=1 cd openai-forward ``` **ä½¿ç¨ docker** ```bash docker-compose up ```
+**æä½¿ç¨pip** ```bash pip install -e . openai-forward run ``` # æå¡è°ç¨
+æ¿æ¢openaiçapiå°åä¸ºè¯¥æå¡çå°åå³å¯ï¼å¦ï¼ ```bash https://
+api.openai.com/v1/chat/completions ``` æ¿æ¢ä¸º ```bash http://{ip}:{port}/v1/
+chat/completions ``` # éç½®éé¡¹ **`openai-forward run`åæ°éç½®é¡¹** |
+éç½®é¡¹ | è¯´æ | é»è®¤å¼ | |-----------| --- | :---: | | --port |
+æå¡ç«¯å£å· | 8000 | | --workers | å·¥ä½è¿ç¨æ° | 1 |
+**ç¯å¢åééç½®é¡¹** åèé¡¹ç®æ ¹ç®å½ä¸`.env`æä»¶ | ç¯å¢åé |
+è¯´æ | é»è®¤å¼ | |-----------------|---------------------------------------
+--------------------------|:------------------------:| | OPENAI_API_KEY |
+é»è®¤openai api keyï¼æ¯æå¤ä¸ªé»è®¤api key, ä»¥ `sk-` å¼å¤´ï¼
+ä»¥ç©ºæ ¼åå² | æ  | | FORWARD_KEY | åè®¸è°ç¨æ¹ä½¿ç¨è¯¥keyä»£æ¿openai
+api keyï¼æ¯æå¤ä¸ªforward key, ä»¥`fk-` å¼å¤´, ä»¥ç©ºæ ¼åå² | æ  | |
+OPENAI_BASE_URL | è½¬åbase url | `https://api.openai.com` | | LOG_CHAT |
+æ¯å¦è®°å½èå¤©åå®¹ | `true` | | ROUTE_PREFIX | è·¯ç±åç¼ | æ  | |
+IP_WHITELIST | ipç½åå, ç©ºæ ¼åå¼ | æ  | | IP_BLACKLIST | ipé»åå,
+ç©ºæ ¼åå¼ | æ  | # èå¤©æ¥å¿ ä¿å­è·¯å¾å¨å½åç®å½ä¸ç`Log/
+`è·¯å¾ä¸­ã èå¤©æ¥å¿ä»¥ `chat_`å¼å¤´,
+é»è®¤æ¯5è½®å¯¹è¯åå¥ä¸æ¬¡æä»¶ è®°å½æ ¼å¼ä¸º ```text {'host': xxx,
+'model': xxx, 'message': [{'user': xxx}, {'assistant': xxx}]} {'assistant':
+xxx} {'host': ...} {'assistant': ...} ... ``` # é«çº§éç½®
+**è®¾ç½®api_keyä¸ºèªå·±è®¾ç½®çforward key** éè¦éç½® OPENAI_API_KEY å
+FORWARD_KEY, ä¾å¦ ```bash OPENAI_API_KEY=sk-******* FORWARD_KEY=fk-****** #
+è¿éfk-tokenç±æä»¬èªå·±å®ä¹ ``` è¿éæä»¬éç½®äºFORWARD_KEYä¸º`fk-
+******`,
+é£ä¹åé¢å®¢æ·ç«¯å¨è°ç¨æ¶åªéè®¾ç½®OPENAI_API_KEYä¸ºæä»¬èªå®ä¹ç`fk-
+******` å³å¯ã
+è¿æ ·çå¥½å¤æ¯å¨ä½¿ç¨ä¸äºéè¦è¾å¥OPENAI_API_KEYçç¬¬ä¸æ¹åºç¨æ¶ï¼æä»¬å¯ä»¥ä½¿ç¨`fk-
+******`æ­éproxyä½¿ç¨ï¼å¦ä¸é¢çä¾å­ï¼
+èæ éæå¿OPENAI_API_KEYè¢«æ³é²ã **ç¨ä¾:** ```bash curl https://
+caloi.top/openai/v1/chat/completions \ -H "Content-Type: application/json" \ -
+H "Authorization: Bearer fk-******" \ -d '{ "model": "gpt-3.5-turbo",
+"messages": [{"role": "user", "content": "Hello!"}] }' ``` **Python** ```diff
+import openai + openai.api_base = "https://caloi.top/openai/v1" -
+openai.api_key = "sk-******" + openai.api_key = "fk-******" ``` **Web
+application** ```bash docker run -d \ -p 3000:3000 \ -e OPENAI_API_KEY="fk-
+******" \ -e BASE_URL="caloi.top/openai" \ -e CODE="" \ yidadaa/chatgpt-next-
+web ```
```

