# Comparing `tmp/serviceboot-2.1.2.tar.gz` & `tmp/serviceboot-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/serviceboot-2.1.2.tar", last modified: Wed Apr 26 02:56:32 2023, max compression
+gzip compressed data, was "dist/serviceboot-2.1.3.tar", last modified: Tue May  9 02:58:37 2023, max compression
```

## Comparing `serviceboot-2.1.2.tar` & `serviceboot-2.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-04-26 02:56:32.000000 serviceboot-2.1.2/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2579 2023-04-26 02:56:32.000000 serviceboot-2.1.2/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)     1395 2023-03-23 06:11:41.000000 serviceboot-2.1.2/README.md
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-04-26 02:56:32.000000 serviceboot-2.1.2/serviceboot/
--rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:17:47.000000 serviceboot-2.1.2/serviceboot/__init__.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2764 2023-04-04 03:17:10.000000 serviceboot-2.1.2/serviceboot/build_docker.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     4167 2023-04-03 13:17:50.000000 serviceboot-2.1.2/serviceboot/build_zip.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1376 2022-11-15 06:17:47.000000 serviceboot-2.1.2/serviceboot/command.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     4143 2022-11-15 06:17:47.000000 serviceboot-2.1.2/serviceboot/compile_python.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      417 2022-11-15 06:17:47.000000 serviceboot-2.1.2/serviceboot/config_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3010 2022-11-15 06:17:47.000000 serviceboot-2.1.2/serviceboot/consul_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3171 2022-11-15 06:17:47.000000 serviceboot-2.1.2/serviceboot/oauth_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2790 2022-11-15 06:17:47.000000 serviceboot-2.1.2/serviceboot/onboarding.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      178 2022-11-15 06:17:47.000000 serviceboot-2.1.2/serviceboot/request_info.py
--rw-rw-r--   0 hls       (1000) hls       (1000)    21359 2023-03-23 06:11:41.000000 serviceboot-2.1.2/serviceboot/serviceboot.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1144 2022-11-15 06:17:47.000000 serviceboot-2.1.2/serviceboot/token_service.py
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-04-26 02:56:32.000000 serviceboot-2.1.2/serviceboot.egg-info/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2579 2023-04-26 02:56:32.000000 serviceboot-2.1.2/serviceboot.egg-info/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)      556 2023-04-26 02:56:32.000000 serviceboot-2.1.2/serviceboot.egg-info/SOURCES.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-04-26 02:56:32.000000 serviceboot-2.1.2/serviceboot.egg-info/dependency_links.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       83 2023-04-26 02:56:32.000000 serviceboot-2.1.2/serviceboot.egg-info/entry_points.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       93 2023-04-26 02:56:32.000000 serviceboot-2.1.2/serviceboot.egg-info/requires.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       12 2023-04-26 02:56:32.000000 serviceboot-2.1.2/serviceboot.egg-info/top_level.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-04-26 02:56:32.000000 serviceboot-2.1.2/setup.cfg
--rw-rw-r--   0 hls       (1000) hls       (1000)     2438 2023-04-26 02:56:18.000000 serviceboot-2.1.2/setup.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-09 02:58:37.000000 serviceboot-2.1.3/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-09 02:58:37.000000 serviceboot-2.1.3/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1526 2023-05-09 02:58:34.000000 serviceboot-2.1.3/README.md
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-09 02:58:37.000000 serviceboot-2.1.3/serviceboot/
+-rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:17:47.000000 serviceboot-2.1.3/serviceboot/__init__.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2764 2023-04-04 03:17:10.000000 serviceboot-2.1.3/serviceboot/build_docker.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     4167 2023-04-03 13:17:50.000000 serviceboot-2.1.3/serviceboot/build_zip.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1376 2022-11-15 06:17:47.000000 serviceboot-2.1.3/serviceboot/command.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     4143 2022-11-15 06:17:47.000000 serviceboot-2.1.3/serviceboot/compile_python.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      417 2022-11-15 06:17:47.000000 serviceboot-2.1.3/serviceboot/config_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3010 2022-11-15 06:17:47.000000 serviceboot-2.1.3/serviceboot/consul_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3171 2022-11-15 06:17:47.000000 serviceboot-2.1.3/serviceboot/oauth_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2790 2022-11-15 06:17:47.000000 serviceboot-2.1.3/serviceboot/onboarding.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      178 2022-11-15 06:17:47.000000 serviceboot-2.1.3/serviceboot/request_info.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)    23475 2023-05-09 02:56:33.000000 serviceboot-2.1.3/serviceboot/serviceboot.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1144 2022-11-15 06:17:47.000000 serviceboot-2.1.3/serviceboot/token_service.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-09 02:58:37.000000 serviceboot-2.1.3/serviceboot.egg-info/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-09 02:58:37.000000 serviceboot-2.1.3/serviceboot.egg-info/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)      556 2023-05-09 02:58:37.000000 serviceboot-2.1.3/serviceboot.egg-info/SOURCES.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-09 02:58:37.000000 serviceboot-2.1.3/serviceboot.egg-info/dependency_links.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       83 2023-05-09 02:58:37.000000 serviceboot-2.1.3/serviceboot.egg-info/entry_points.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       93 2023-05-09 02:58:37.000000 serviceboot-2.1.3/serviceboot.egg-info/requires.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       12 2023-05-09 02:58:37.000000 serviceboot-2.1.3/serviceboot.egg-info/top_level.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-09 02:58:37.000000 serviceboot-2.1.3/setup.cfg
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2438 2023-05-09 02:56:33.000000 serviceboot-2.1.3/setup.py
```

### Comparing `serviceboot-2.1.2/PKG-INFO` & `serviceboot-2.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serviceboot
-Version: 2.1.2
+Version: 2.1.3
 Summary: ServiceBoot云原生微服务引擎
 Home-page: https://openi.pcl.ac.cn/cubepy/serviceboot
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # ServiceBoot云原生微服务引擎
         
@@ -17,14 +17,16 @@
         - 普通RESTful API（面向JSON数据格式）。
         - 二进制字节流数据API。
         - 文件上传API。
         - 可视化Web页面访问API。
         - Special API。
         - WebSocket实时通信API。
         
+        在启动ServiceBoot服务时，还可根据配置启动开发者自定义的Python前端服务，例如: Gradio, Streamlit等。
+        
         ## 开源主页 
         
         - https://openi.pcl.ac.cn/cubepy/serviceboot
         
         ## 依赖包主页 
         
         - https://pypi.org/project/serviceboot
```

### Comparing `serviceboot-2.1.2/README.md` & `serviceboot-2.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 - 普通RESTful API（面向JSON数据格式）。
 - 二进制字节流数据API。
 - 文件上传API。
 - 可视化Web页面访问API。
 - Special API。
 - WebSocket实时通信API。
 
+在启动ServiceBoot服务时，还可根据配置启动开发者自定义的Python前端服务，例如: Gradio, Streamlit等。
+
 ## 开源主页 
 
 - https://openi.pcl.ac.cn/cubepy/serviceboot
 
 ## 依赖包主页 
 
 - https://pypi.org/project/serviceboot
```

### Comparing `serviceboot-2.1.2/serviceboot/build_docker.py` & `serviceboot-2.1.3/serviceboot/build_docker.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.2/serviceboot/build_zip.py` & `serviceboot-2.1.3/serviceboot/build_zip.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.2/serviceboot/command.py` & `serviceboot-2.1.3/serviceboot/command.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.2/serviceboot/compile_python.py` & `serviceboot-2.1.3/serviceboot/compile_python.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.2/serviceboot/consul_client.py` & `serviceboot-2.1.3/serviceboot/consul_client.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.2/serviceboot/oauth_client.py` & `serviceboot-2.1.3/serviceboot/oauth_client.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.2/serviceboot/onboarding.py` & `serviceboot-2.1.3/serviceboot/onboarding.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.2/serviceboot/serviceboot.py` & `serviceboot-2.1.3/serviceboot/serviceboot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 # -*- coding: utf-8 -*-
 import json
 import yaml
 import socket
 import logging
 import asyncio
 import platform
+import requests
 import threading
 import tornado.web
 import tornado.ioloop
 import tornado.websocket
 import tornado.httpserver
 import os, sys
 
-
 sys.path.append(os.getcwd())
 use_oop = True
 try:
     # 如果 ./app/ 目录下存在 app_main.py 文件，则模型主程序使用非面向对象模式编程，忽略同目录下的 app_core.py 文件（如果存在）
     from app import app_main
+
     use_oop = False
 except:
     # 如果 ./core/ 目录下存在 model_main.py 文件，则模型主程序使用面向对象模式编程
     from app.app_core import AppCore
+
     use_oop = True
 
 
 class GlobalData:
     def __init__(self):
         self.app_core = None
+        self.port = 80
+        self.python_frontend_port = 7860
 
     def init_global_data(self):
         try:
             self.app_core = AppCore() if use_oop else app_main
             return True
         except Exception as e:
             logging.error(str(e))
@@ -563,14 +567,69 @@
         ip = s.getsockname()[0]
     finally:
         s.close()
 
     return ip
 
 
+def start_python_frontend():
+    try:
+        from app.python_frontend import PythonFrontend
+        python_frontend = PythonFrontend()
+        logging.critical('##################################################')
+        logging.critical(f'    Python frontend started ...')
+        logging.critical(f'    Web access: http://{get_local_ip()}:{g.python_frontend_port}/')
+        logging.critical('##################################################')
+        thread = threading.Thread(target=python_frontend_thread, args=(asyncio.get_event_loop(), python_frontend))
+        thread.setDaemon(True)
+        thread.start()
+    except Exception as e:
+        pass
+
+
+def python_frontend_thread(event_loop, python_frontend):
+    asyncio.set_event_loop(event_loop)
+    kwargs = {
+        'server_name': '0.0.0.0',
+        'server_port': g.python_frontend_port,
+    }
+    python_frontend.launch(**kwargs)
+
+
+def serviceboot_client(body=None):
+    url = f'http://127.0.0.1:{g.port}/api/data'
+    headers = {
+        'Content-Type': 'application/json;charset=UTF-8',
+        'Accept': '*/*',
+    }
+
+    try:
+        res = requests.post(url=url, json=body, headers=headers)
+    except Exception as e:
+        return {
+            'status': 'err',
+            'value': '网络或服务器故障!'
+        }
+
+    if res.status_code != 200:
+        return {
+            'status': 'err',
+            'value': res.text
+        }
+
+    try:
+        # JSON数据，转化成JSON对象
+        result = json.loads(res.text, encoding='utf-8')
+    except:
+        # 非JSON数据（二进制字节流），直接返回
+        result = res.content
+
+    return result
+
+
 def start():
     app_profile = os.environ.get('APP_PROFILE', 'dev').lower()
     log_level = logging.DEBUG if app_profile == 'dev' else logging.ERROR
     logging.basicConfig(level=log_level, format='%(asctime)s - %(levelname)s - %(message)s')
 
     try:
         with open('./application.yml', 'rb') as f:
@@ -598,19 +657,32 @@
             port = 80
     else:
         try:
             port = yml['serviceboot']['port']['prod']
         except:
             logging.error('未指定服务端口号！缺省使用80端口。')
             port = 80
+    g.port = port
 
     if not g.init_global_data():
         logging.error('微服务： {}/{} 初始化失败！'.format(cname, ename))
         return
 
+    try:
+        use_python_frontend = yml['serviceboot']['use_python_frontend']
+    except:
+        use_python_frontend = False
+    # 启动Python前端服务
+    if use_python_frontend:
+        try:
+            g.python_frontend_port = yml['serviceboot']['python_frontend_port']
+        except:
+            g.python_frontend_port = 7860
+        start_python_frontend()
+
     handlers = [
         (r'/management/health', HealthChecker),
         (r'/special/(.*)', SpecialApi),
         (r'/api/data', DataApi),
         (r'/api/stream/(.*)', StreamApi),
         (r'/api/file/(.*)', FileApi),
         (r'/websocket', WebSocketServer),
```

### Comparing `serviceboot-2.1.2/serviceboot/token_service.py` & `serviceboot-2.1.3/serviceboot/token_service.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.2/serviceboot.egg-info/PKG-INFO` & `serviceboot-2.1.3/serviceboot.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serviceboot
-Version: 2.1.2
+Version: 2.1.3
 Summary: ServiceBoot云原生微服务引擎
 Home-page: https://openi.pcl.ac.cn/cubepy/serviceboot
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # ServiceBoot云原生微服务引擎
         
@@ -17,14 +17,16 @@
         - 普通RESTful API（面向JSON数据格式）。
         - 二进制字节流数据API。
         - 文件上传API。
         - 可视化Web页面访问API。
         - Special API。
         - WebSocket实时通信API。
         
+        在启动ServiceBoot服务时，还可根据配置启动开发者自定义的Python前端服务，例如: Gradio, Streamlit等。
+        
         ## 开源主页 
         
         - https://openi.pcl.ac.cn/cubepy/serviceboot
         
         ## 依赖包主页 
         
         - https://pypi.org/project/serviceboot
```

### Comparing `serviceboot-2.1.2/serviceboot.egg-info/SOURCES.txt` & `serviceboot-2.1.3/serviceboot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.2/setup.py` & `serviceboot-2.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(
     name='serviceboot',
-    version='2.1.2',
+    version='2.1.3',
     author='cubeai',
     author_email='cubeai@163.com',
     description='ServiceBoot云原生微服务引擎',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     packages=find_packages(),
```

