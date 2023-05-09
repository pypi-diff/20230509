# Comparing `tmp/aioinsta-1.2.tar.gz` & `tmp/aioinsta-1.3.tar.gz`

## Comparing `aioinsta-1.2.tar` & `aioinsta-1.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/__init__.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/challenge.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/client.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/enums.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/exceptions.py
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/extractors.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/helpers.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/idcodec.py
--rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/login.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/media.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/password.py
--rw-r--r--   0        0        0     7754 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/request.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/user.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/types/media.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/types/user.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 aioinsta-1.2/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 aioinsta-1.2/LICENSE
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aioinsta-1.2/README.md
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 aioinsta-1.2/pyproject.toml
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 aioinsta-1.2/PKG-INFO
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 aioinsta-1.3/aioinsta/__init__.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 aioinsta-1.3/aioinsta/challenge.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 aioinsta-1.3/aioinsta/client.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 aioinsta-1.3/aioinsta/enums.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 aioinsta-1.3/aioinsta/exceptions.py
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 aioinsta-1.3/aioinsta/extractors.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 aioinsta-1.3/aioinsta/helpers.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 aioinsta-1.3/aioinsta/idcodec.py
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 aioinsta-1.3/aioinsta/login.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 aioinsta-1.3/aioinsta/media.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 aioinsta-1.3/aioinsta/parametrs.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 aioinsta-1.3/aioinsta/password.py
+-rw-r--r--   0        0        0     7766 2020-02-02 00:00:00.000000 aioinsta-1.3/aioinsta/request.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 aioinsta-1.3/aioinsta/user.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 aioinsta-1.3/aioinsta/types/media.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 aioinsta-1.3/aioinsta/types/user.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 aioinsta-1.3/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 aioinsta-1.3/LICENSE
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aioinsta-1.3/README.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 aioinsta-1.3/pyproject.toml
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 aioinsta-1.3/PKG-INFO
```

### Comparing `aioinsta-1.2/aioinsta/challenge.py` & `aioinsta-1.3/aioinsta/challenge.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.2/aioinsta/extractors.py` & `aioinsta-1.3/aioinsta/extractors.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.2/aioinsta/helpers.py` & `aioinsta-1.3/aioinsta/helpers.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.2/aioinsta/idcodec.py` & `aioinsta-1.3/aioinsta/idcodec.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.2/aioinsta/login.py` & `aioinsta-1.3/aioinsta/login.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.2/aioinsta/media.py` & `aioinsta-1.3/aioinsta/media.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.2/aioinsta/password.py` & `aioinsta-1.3/aioinsta/password.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.2/aioinsta/request.py` & `aioinsta-1.3/aioinsta/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import random
 import time
 from urllib.parse import urljoin
 
 from aiohttp import ClientSession
 from aiohttp.client_exceptions import ContentTypeError
 
-from aioinsta import config, login
+from aioinsta import parametrs, login
 from aioinsta.enums import ErrorTypes
 from aioinsta.exceptions import ChallengeRequired, RateLimit
 from aioinsta.helpers import generate_uuid
 
 
 class PrivateRequestClient:
     def __init__(self, login_client: "login.Login"):
@@ -52,15 +52,15 @@
             return dict(response=response, headers=response_headers)
 
     async def close(self):
         return await self.session.close()
 
     def set_user_agent(self, user_agent: str | None = None):
         data = dict(self.login_client.device_settings, locale=self.login_client.locale)
-        self.login_client.user_agent = user_agent or config.USER_AGENT_BASE.format(
+        self.login_client.user_agent = user_agent or parametrs.USER_AGENT_BASE.format(
             **data
         )
         self.login_client.settings["user_agent"] = self.login_client.user_agent
 
     def base_headers(self):
         locale = self.login_client.locale.replace("-", "_")
         accept_language = ["en-US"]
@@ -128,15 +128,15 @@
         self,
         method: str,
         path: str,
         data: dict | None = None,
         params: dict | None = None,
         raise_for_status: bool = False,
     ):
-        url = urljoin(config.API_DOMAIN + "api/v1/", path)
+        url = urljoin(parametrs.API_DOMAIN + "api/v1/", path)
         try:
             response = await self._request(
                 method=method,
                 url=url,
                 data=data,
                 params=params,
                 headers=self.base_headers(),
@@ -178,12 +178,12 @@
 
     async def public_a1_request(
         self,
         method: str,
         path: str,
         params: dict | None = None,
     ):
-        url = urljoin(config.PUBLIC_API_DOMAIN, path)
+        url = urljoin(parametrs.PUBLIC_API_DOMAIN, path)
         params = params or {}
         params.update({"__a": 1, "__d": "dis"})
         response = await self.public_request(method=method, url=url, params=params)
         return response.get("response").get("graphql")
```

### Comparing `aioinsta-1.2/aioinsta/user.py` & `aioinsta-1.3/aioinsta/user.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.2/aioinsta/types/media.py` & `aioinsta-1.3/aioinsta/types/media.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.2/aioinsta/types/user.py` & `aioinsta-1.3/aioinsta/types/user.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.2/.gitignore` & `aioinsta-1.3/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 main.py
-config.py
 .idea
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
```

### Comparing `aioinsta-1.2/LICENSE` & `aioinsta-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aioinsta-1.2/pyproject.toml` & `aioinsta-1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -26,7 +26,10 @@
 [tool.hatch.version]
 path = "aioinsta/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
     "/aioinsta",
 ]
+
+[tool.isort]
+profile = "black"
```

### Comparing `aioinsta-1.2/PKG-INFO` & `aioinsta-1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioinsta
-Version: 1.2
+Version: 1.3
 Summary: Tool for parse instagram data
 Project-URL: Homepage, https://github.com/sheldygg/aioinsta
 Author: sheldy
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

