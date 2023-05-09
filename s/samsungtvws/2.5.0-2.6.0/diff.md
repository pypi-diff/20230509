# Comparing `tmp/samsungtvws-2.5.0.tar.gz` & `tmp/samsungtvws-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samsungtvws-2.5.0.tar", last modified: Tue Mar 22 21:38:55 2022, max compression
+gzip compressed data, was "samsungtvws-2.6.0.tar", last modified: Tue May  9 19:35:32 2023, max compression
```

## Comparing `samsungtvws-2.5.0.tar` & `samsungtvws-2.6.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2022-03-22 21:38:55.379726 samsungtvws-2.5.0/
--rw-rw-rw-   0        0        0     1091 2021-11-10 22:44:40.000000 samsungtvws-2.5.0/LICENSE
--rw-rw-rw-   0        0        0     5660 2022-03-22 21:38:55.378726 samsungtvws-2.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     5102 2022-03-22 21:36:18.000000 samsungtvws-2.5.0/README.md
--rw-rw-rw-   0        0        0     1235 2022-03-14 21:10:32.000000 samsungtvws-2.5.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2022-03-22 21:38:55.335013 samsungtvws-2.5.0/samsungtvws/
--rw-rw-rw-   0        0        0      934 2021-11-10 22:44:40.000000 samsungtvws-2.5.0/samsungtvws/__init__.py
--rw-rw-rw-   0        0        0    11269 2022-03-14 21:10:32.000000 samsungtvws-2.5.0/samsungtvws/art.py
--rw-rw-rw-   0        0        0     6461 2022-03-22 21:34:57.000000 samsungtvws-2.5.0/samsungtvws/async_connection.py
--rw-rw-rw-   0        0        0     2993 2022-03-22 21:34:57.000000 samsungtvws-2.5.0/samsungtvws/async_remote.py
--rw-rw-rw-   0        0        0     3397 2022-03-14 21:10:32.000000 samsungtvws-2.5.0/samsungtvws/async_rest.py
--rw-rw-rw-   0        0        0      842 2022-03-14 21:10:32.000000 samsungtvws-2.5.0/samsungtvws/command.py
--rw-rw-rw-   0        0        0     9178 2022-03-22 21:34:57.000000 samsungtvws-2.5.0/samsungtvws/connection.py
-drwxrwxrwx   0        0        0        0 2022-03-22 21:38:55.377725 samsungtvws-2.5.0/samsungtvws/encrypted/
--rw-rw-rw-   0        0        0       43 2022-03-14 23:00:20.000000 samsungtvws-2.5.0/samsungtvws/encrypted/__init__.py
--rw-rw-rw-   0        0        0    16325 2022-03-22 21:34:57.000000 samsungtvws-2.5.0/samsungtvws/encrypted/authenticator.py
--rw-rw-rw-   0        0        0      618 2022-03-14 23:00:20.000000 samsungtvws-2.5.0/samsungtvws/encrypted/command.py
--rw-rw-rw-   0        0        0     5885 2022-03-19 17:40:44.000000 samsungtvws-2.5.0/samsungtvws/encrypted/remote.py
--rw-rw-rw-   0        0        0     1780 2022-03-15 00:25:12.000000 samsungtvws-2.5.0/samsungtvws/encrypted/session.py
--rw-rw-rw-   0        0        0     1047 2022-03-22 21:34:57.000000 samsungtvws-2.5.0/samsungtvws/event.py
--rw-rw-rw-   0        0        0      445 2022-03-22 21:34:57.000000 samsungtvws-2.5.0/samsungtvws/exceptions.py
--rw-rw-rw-   0        0        0      730 2022-03-14 21:10:32.000000 samsungtvws-2.5.0/samsungtvws/helper.py
--rw-rw-rw-   0        0        0        0 2022-03-14 21:10:32.000000 samsungtvws-2.5.0/samsungtvws/py.typed
--rw-rw-rw-   0        0        0    11593 2022-03-22 21:34:57.000000 samsungtvws-2.5.0/samsungtvws/remote.py
--rw-rw-rw-   0        0        0     3125 2022-03-14 21:10:32.000000 samsungtvws-2.5.0/samsungtvws/rest.py
--rw-rw-rw-   0        0        0     2777 2022-03-14 21:10:32.000000 samsungtvws-2.5.0/samsungtvws/shortcuts.py
-drwxrwxrwx   0        0        0        0 2022-03-22 21:38:55.347010 samsungtvws-2.5.0/samsungtvws.egg-info/
--rw-rw-rw-   0        0        0     5660 2022-03-22 21:38:54.000000 samsungtvws-2.5.0/samsungtvws.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      721 2022-03-22 21:38:55.000000 samsungtvws-2.5.0/samsungtvws.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-22 21:38:54.000000 samsungtvws-2.5.0/samsungtvws.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2022-03-22 21:38:55.000000 samsungtvws-2.5.0/samsungtvws.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-03-22 21:38:55.000000 samsungtvws-2.5.0/samsungtvws.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-03-22 21:38:55.379726 samsungtvws-2.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1084 2022-03-22 21:36:13.000000 samsungtvws-2.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:35:32.655125 samsungtvws-2.6.0/
+-rw-rw-rw-   0        0        0     1091 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/LICENSE
+-rw-rw-rw-   0        0        0     5660 2023-05-09 19:35:32.654624 samsungtvws-2.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5102 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/README.md
+-rw-rw-rw-   0        0        0     1441 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-09 19:35:32.641113 samsungtvws-2.6.0/samsungtvws/
+-rw-rw-rw-   0        0        0      934 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/samsungtvws/__init__.py
+-rw-rw-rw-   0        0        0    12090 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/samsungtvws/art.py
+-rw-rw-rw-   0        0        0     6405 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/samsungtvws/async_connection.py
+-rw-rw-rw-   0        0        0     2993 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/samsungtvws/async_remote.py
+-rw-rw-rw-   0        0        0     3413 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/samsungtvws/async_rest.py
+-rw-rw-rw-   0        0        0      842 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/samsungtvws/command.py
+-rw-rw-rw-   0        0        0     9176 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/samsungtvws/connection.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:35:32.653623 samsungtvws-2.6.0/samsungtvws/encrypted/
+-rw-rw-rw-   0        0        0       43 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/samsungtvws/encrypted/__init__.py
+-rw-rw-rw-   0        0        0    16325 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/samsungtvws/encrypted/authenticator.py
+-rw-rw-rw-   0        0        0      618 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/samsungtvws/encrypted/command.py
+-rw-rw-rw-   0        0        0     5885 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/samsungtvws/encrypted/remote.py
+-rw-rw-rw-   0        0        0     1780 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/samsungtvws/encrypted/session.py
+-rw-rw-rw-   0        0        0     1047 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/samsungtvws/event.py
+-rw-rw-rw-   0        0        0      445 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/samsungtvws/exceptions.py
+-rw-rw-rw-   0        0        0     1028 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/samsungtvws/helper.py
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/samsungtvws/py.typed
+-rw-rw-rw-   0        0        0    11620 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/samsungtvws/remote.py
+-rw-rw-rw-   0        0        0     3141 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/samsungtvws/rest.py
+-rw-rw-rw-   0        0        0     2777 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/samsungtvws/shortcuts.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:35:32.645116 samsungtvws-2.6.0/samsungtvws.egg-info/
+-rw-rw-rw-   0        0        0     5660 2023-05-09 19:35:32.000000 samsungtvws-2.6.0/samsungtvws.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      721 2023-05-09 19:35:32.000000 samsungtvws-2.6.0/samsungtvws.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 19:35:32.000000 samsungtvws-2.6.0/samsungtvws.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      136 2023-05-09 19:35:32.000000 samsungtvws-2.6.0/samsungtvws.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-09 19:35:32.000000 samsungtvws-2.6.0/samsungtvws.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 19:35:32.655125 samsungtvws-2.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2023-05-09 19:35:24.000000 samsungtvws-2.6.0/setup.py
```

### Comparing `samsungtvws-2.5.0/LICENSE` & `samsungtvws-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `samsungtvws-2.5.0/PKG-INFO` & `samsungtvws-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samsungtvws
-Version: 2.5.0
+Version: 2.6.0
 Summary: Samsung Smart TV WS API wrapper
 Home-page: https://github.com/xchwarze/samsung-tv-ws-api
 Author: Xchwarze
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Provides-Extra: encrypted
 License-File: LICENSE
 
 <p align="center">
     <img src="https://user-images.githubusercontent.com/5860071/47255992-611d9b00-d481-11e8-965d-d9816f254be2.png" width="300px" border="0" />
     <br/>
     <a href="https://github.com/xchwarze/samsung-tv-ws-api/releases/latest">
-        <img src="https://img.shields.io/badge/version-2.5.0-brightgreen.svg?style=flat-square" alt="Version">
+        <img src="https://img.shields.io/badge/version-2.6.0-brightgreen.svg?style=flat-square" alt="Version">
     </a>
     Samsung Smart TV WS API wrapper
 </p>
 
 This project is a library for remote controlling Samsung televisions via a TCP/IP connection.
 
 It currently supports modern (post-2016) TVs with Ethernet or Wi-Fi connectivity. They should be all models with TizenOs.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: samsungtvws Version: 2.5.0 Summary: Samsung Smart
+Metadata-Version: 2.1 Name: samsungtvws Version: 2.6.0 Summary: Samsung Smart
 TV WS API wrapper Home-page: https://github.com/xchwarze/samsung-tv-ws-api
 Author: Xchwarze License: MIT Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Requires-Python: >=3.0.0 Description-Content-Type: text/markdown
 Provides-Extra: async Provides-Extra: encrypted License-File: LICENSE
 [https://user-images.githubusercontent.com/5860071/47255992-611d9b00-d481-11e8-
```

### Comparing `samsungtvws-2.5.0/README.md` & `samsungtvws-2.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <p align="center">
     <img src="https://user-images.githubusercontent.com/5860071/47255992-611d9b00-d481-11e8-965d-d9816f254be2.png" width="300px" border="0" />
     <br/>
     <a href="https://github.com/xchwarze/samsung-tv-ws-api/releases/latest">
-        <img src="https://img.shields.io/badge/version-2.5.0-brightgreen.svg?style=flat-square" alt="Version">
+        <img src="https://img.shields.io/badge/version-2.6.0-brightgreen.svg?style=flat-square" alt="Version">
     </a>
     Samsung Smart TV WS API wrapper
 </p>
 
 This project is a library for remote controlling Samsung televisions via a TCP/IP connection.
 
 It currently supports modern (post-2016) TVs with Ethernet or Wi-Fi connectivity. They should be all models with TizenOs.
```

### Comparing `samsungtvws-2.5.0/samsungtvws/__init__.py` & `samsungtvws-2.6.0/samsungtvws/__init__.py`

 * *Files identical despite different names*

### Comparing `samsungtvws-2.5.0/samsungtvws/art.py` & `samsungtvws-2.6.0/samsungtvws/art.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,19 @@
             event = response.get("event", "*")
             assert event
             self._websocket_event(event, response)
             if event == wait_for_event and wait_for_sub_event:
                 # Check sub event, reset event if it doesn't match
                 data = json.loads(response["data"])
                 sub_event = data.get("event", "*")
+                if sub_event == "error":
+                    raise exceptions.ResponseError(
+                        f"`{request_data['request']}` request failed "
+                        f"with error number {data['error_code']}"
+                    )
                 if sub_event != wait_for_sub_event:
                     event = None
 
         return response
 
     def _get_rest_api(self) -> SamsungTVRest:
         if self._rest_api is None:
@@ -334,7 +339,26 @@
         self._send_art_request(
             {
                 "request": "set_photo_filter",
                 "content_id": content_id,
                 "filter_id": filter_id,
             }
         )
+
+    def get_matte_list(self):
+        response = self._send_art_request(
+            {"request": "get_matte_list"},
+            wait_for_event=D2D_SERVICE_MESSAGE_EVENT,
+        )
+        assert response
+        data = json.loads(response["data"])
+
+        return json.loads(data["matte_type_list"])
+
+    def change_matte(self, content_id, matte_id):
+        self._send_art_request(
+            {
+                "request": "change_matte",
+                "content_id": content_id,
+                "matte_id": matte_id,
+            }
+        )
```

### Comparing `samsungtvws-2.5.0/samsungtvws/async_connection.py` & `samsungtvws-2.6.0/samsungtvws/async_connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,20 +33,20 @@
 from . import connection, exceptions, helper
 from .command import SamsungTVCommand, SamsungTVSleepCommand
 from .event import (
     IGNORE_EVENTS_AT_STARTUP,
     MS_CHANNEL_CONNECT_EVENT,
     MS_CHANNEL_UNAUTHORIZED,
 )
+from .helper import get_ssl_context
 
 _LOGGING = logging.getLogger(__name__)
 
 
 class SamsungTVWSAsyncConnection(connection.SamsungTVWSBaseConnection):
-
     connection: Optional[WebSocketClientProtocol]
     _recv_loop: Optional["asyncio.Task[None]"]
 
     async def __aenter__(self) -> "SamsungTVWSAsyncConnection":
         return self
 
     async def __aexit__(
@@ -63,17 +63,15 @@
             return self.connection
 
         url = self._format_websocket_url(self.endpoint)
 
         _LOGGING.debug("WS url %s", url)
         connect_kwargs: Dict[str, Any] = {}
         if self._is_ssl_connection():
-            ssl_context = ssl.SSLContext()
-            ssl_context.verify_mode = ssl.CERT_NONE
-            connect_kwargs["ssl"] = ssl_context
+            connect_kwargs["ssl"] = get_ssl_context()
         connection = await connect(url, open_timeout=self.timeout, **connect_kwargs)
 
         event: Optional[str] = None
         while event is None or event in IGNORE_EVENTS_AT_STARTUP:
             data = await connection.recv()
             response = helper.process_api_response(data)
             event = response.get("event", "*")
```

### Comparing `samsungtvws-2.5.0/samsungtvws/async_remote.py` & `samsungtvws-2.6.0/samsungtvws/async_remote.py`

 * *Files identical despite different names*

### Comparing `samsungtvws-2.5.0/samsungtvws/async_rest.py` & `samsungtvws-2.6.0/samsungtvws/async_rest.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,18 +57,18 @@
                 future = self.session.delete(
                     url, timeout=self.timeout, verify_ssl=False
                 )
             else:
                 future = self.session.get(url, timeout=self.timeout, verify_ssl=False)
             async with future as resp:
                 return helper.process_api_response(await resp.text())
-        except aiohttp.ClientConnectionError:
+        except aiohttp.ClientConnectionError as err:
             raise exceptions.HttpApiError(
                 "TV unreachable or feature not supported on this model."
-            )
+            ) from err
 
     async def rest_device_info(self) -> Dict[str, Any]:
         _LOGGING.debug("Get device info via rest api")
         return await self._rest_request("")
 
     async def rest_app_status(self, app_id: str) -> Dict[str, Any]:
         _LOGGING.debug("Get app %s status via rest api", app_id)
```

### Comparing `samsungtvws-2.5.0/samsungtvws/command.py` & `samsungtvws-2.6.0/samsungtvws/command.py`

 * *Files identical despite different names*

### Comparing `samsungtvws-2.5.0/samsungtvws/connection.py` & `samsungtvws-2.6.0/samsungtvws/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,14 @@
                     "Your TV does not seem to support v2 API, please try v1 API"
                 )
         else:
             _LOGGING.debug("SamsungTVWS websocket event: %s", response)
 
 
 class SamsungTVWSConnection(SamsungTVWSBaseConnection):
-
     connection: Optional[websocket.WebSocket]
     _recv_loop: Optional[threading.Thread]
 
     def __enter__(self) -> "SamsungTVWSConnection":
         return self
 
     def __exit__(
```

### Comparing `samsungtvws-2.5.0/samsungtvws/encrypted/authenticator.py` & `samsungtvws-2.6.0/samsungtvws/encrypted/authenticator.py`

 * *Files identical despite different names*

### Comparing `samsungtvws-2.5.0/samsungtvws/encrypted/command.py` & `samsungtvws-2.6.0/samsungtvws/encrypted/command.py`

 * *Files identical despite different names*

### Comparing `samsungtvws-2.5.0/samsungtvws/encrypted/remote.py` & `samsungtvws-2.6.0/samsungtvws/encrypted/remote.py`

 * *Files identical despite different names*

### Comparing `samsungtvws-2.5.0/samsungtvws/encrypted/session.py` & `samsungtvws-2.6.0/samsungtvws/encrypted/session.py`

 * *Files identical despite different names*

### Comparing `samsungtvws-2.5.0/samsungtvws/event.py` & `samsungtvws-2.6.0/samsungtvws/event.py`

 * *Files identical despite different names*

### Comparing `samsungtvws-2.5.0/samsungtvws/helper.py` & `samsungtvws-2.6.0/samsungtvws/helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 import base64
 import json
 import logging
-from typing import Any, Dict, Union
+import ssl
+from typing import Any, Dict, Optional, Union
 
 from . import exceptions
 
 _LOGGING = logging.getLogger(__name__)
+_SSL_CONTEXT: Optional[ssl.SSLContext] = None
 
 
 def serialize_string(string: Union[str, bytes]) -> str:
     if isinstance(string, str):
         string = str.encode(string)
 
     return base64.b64encode(string).decode("utf-8")
 
 
 def process_api_response(response: Union[str, bytes]) -> Dict[str, Any]:
     _LOGGING.debug("Processing API response: %s", response)
     try:
         return json.loads(response)  # type:ignore[no-any-return]
-    except json.JSONDecodeError:
+    except json.JSONDecodeError as err:
         raise exceptions.ResponseError(
             "Failed to parse response from TV. Maybe feature not supported on this model"
-        )
+        ) from err
+
+
+def get_ssl_context() -> ssl.SSLContext:
+    global _SSL_CONTEXT
+    if not _SSL_CONTEXT:
+        _SSL_CONTEXT = ssl.SSLContext()
+        _SSL_CONTEXT.verify_mode = ssl.CERT_NONE
+    return _SSL_CONTEXT
```

### Comparing `samsungtvws-2.5.0/samsungtvws/remote.py` & `samsungtvws-2.6.0/samsungtvws/remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,15 @@
         ]
 
     @staticmethod
     def hold_key(key: str, seconds: float) -> List["SamsungTVCommand"]:
         warnings.warn(
             "SendRemoteKey.hold_key is deprecated, please use SendRemoteKey.hold instead",
             DeprecationWarning,
+            stacklevel=2,
         )
         return SendRemoteKey.hold(key, seconds)
 
     # power
     @staticmethod
     def power() -> "SendRemoteKey":
         return SendRemoteKey.click("KEY_POWER")
```

### Comparing `samsungtvws-2.5.0/samsungtvws/rest.py` & `samsungtvws-2.6.0/samsungtvws/rest.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,18 +51,18 @@
             elif method == "PUT":
                 response = requests.put(url, timeout=self.timeout, verify=False)
             elif method == "DELETE":
                 response = requests.delete(url, timeout=self.timeout, verify=False)
             else:
                 response = requests.get(url, timeout=self.timeout, verify=False)
             return helper.process_api_response(response.text)
-        except requests.ConnectionError:
+        except requests.ConnectionError as err:
             raise exceptions.HttpApiError(
                 "TV unreachable or feature not supported on this model."
-            )
+            ) from err
 
     def rest_device_info(self) -> Dict[str, Any]:
         _LOGGING.debug("Get device info via rest api")
         return self._rest_request("")
 
     def rest_app_status(self, app_id: str) -> Dict[str, Any]:
         _LOGGING.debug("Get app %s status via rest api", app_id)
```

### Comparing `samsungtvws-2.5.0/samsungtvws/shortcuts.py` & `samsungtvws-2.6.0/samsungtvws/shortcuts.py`

 * *Files identical despite different names*

### Comparing `samsungtvws-2.5.0/samsungtvws.egg-info/PKG-INFO` & `samsungtvws-2.6.0/samsungtvws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samsungtvws
-Version: 2.5.0
+Version: 2.6.0
 Summary: Samsung Smart TV WS API wrapper
 Home-page: https://github.com/xchwarze/samsung-tv-ws-api
 Author: Xchwarze
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Provides-Extra: encrypted
 License-File: LICENSE
 
 <p align="center">
     <img src="https://user-images.githubusercontent.com/5860071/47255992-611d9b00-d481-11e8-965d-d9816f254be2.png" width="300px" border="0" />
     <br/>
     <a href="https://github.com/xchwarze/samsung-tv-ws-api/releases/latest">
-        <img src="https://img.shields.io/badge/version-2.5.0-brightgreen.svg?style=flat-square" alt="Version">
+        <img src="https://img.shields.io/badge/version-2.6.0-brightgreen.svg?style=flat-square" alt="Version">
     </a>
     Samsung Smart TV WS API wrapper
 </p>
 
 This project is a library for remote controlling Samsung televisions via a TCP/IP connection.
 
 It currently supports modern (post-2016) TVs with Ethernet or Wi-Fi connectivity. They should be all models with TizenOs.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: samsungtvws Version: 2.5.0 Summary: Samsung Smart
+Metadata-Version: 2.1 Name: samsungtvws Version: 2.6.0 Summary: Samsung Smart
 TV WS API wrapper Home-page: https://github.com/xchwarze/samsung-tv-ws-api
 Author: Xchwarze License: MIT Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Requires-Python: >=3.0.0 Description-Content-Type: text/markdown
 Provides-Extra: async Provides-Extra: encrypted License-File: LICENSE
 [https://user-images.githubusercontent.com/5860071/47255992-611d9b00-d481-11e8-
```

### Comparing `samsungtvws-2.5.0/samsungtvws.egg-info/SOURCES.txt` & `samsungtvws-2.6.0/samsungtvws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `samsungtvws-2.5.0/setup.py` & `samsungtvws-2.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def readme():
     with open("README.md") as readme_file:
         return readme_file.read()
 
 
 setup(
     name="samsungtvws",
-    version="2.5.0",
+    version="2.6.0",
     description="Samsung Smart TV WS API wrapper",
     long_description=readme(),
     long_description_content_type="text/markdown",
     author="Xchwarze",
     python_requires=">=3.0.0",
     url="https://github.com/xchwarze/samsung-tv-ws-api",
     package_data={"samsungtvws": ["py.typed"]},
```

