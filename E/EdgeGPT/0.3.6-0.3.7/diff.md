# Comparing `tmp/EdgeGPT-0.3.6.tar.gz` & `tmp/EdgeGPT-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.3.6.tar", last modified: Sun May  7 09:45:55 2023, max compression
+gzip compressed data, was "EdgeGPT-0.3.7.tar", last modified: Tue May  9 15:17:39 2023, max compression
```

## Comparing `EdgeGPT-0.3.6.tar` & `EdgeGPT-0.3.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:45:55.828800 EdgeGPT-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-07 09:45:25.000000 EdgeGPT-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-07 09:45:55.828800 EdgeGPT-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-07 09:45:55.000000 EdgeGPT-0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-07 09:45:55.832800 EdgeGPT-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-07 09:45:25.000000 EdgeGPT-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:45:55.828800 EdgeGPT-0.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:45:55.828800 EdgeGPT-0.3.6/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-07 09:45:55.000000 EdgeGPT-0.3.6/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-07 09:45:55.000000 EdgeGPT-0.3.6/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:45:55.000000 EdgeGPT-0.3.6/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 09:45:55.000000 EdgeGPT-0.3.6/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-07 09:45:55.000000 EdgeGPT-0.3.6/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-07 09:45:55.000000 EdgeGPT-0.3.6/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    29532 2023-05-07 09:45:25.000000 EdgeGPT-0.3.6/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-07 09:45:25.000000 EdgeGPT-0.3.6/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:17:39.477652 EdgeGPT-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-09 15:17:01.000000 EdgeGPT-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-09 15:17:39.477652 EdgeGPT-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-09 15:17:39.000000 EdgeGPT-0.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-09 15:17:39.477652 EdgeGPT-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-09 15:17:01.000000 EdgeGPT-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:17:39.477652 EdgeGPT-0.3.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:17:39.477652 EdgeGPT-0.3.7/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-09 15:17:39.000000 EdgeGPT-0.3.7/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-09 15:17:39.000000 EdgeGPT-0.3.7/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:17:39.000000 EdgeGPT-0.3.7/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-09 15:17:39.000000 EdgeGPT-0.3.7/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-09 15:17:39.000000 EdgeGPT-0.3.7/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-09 15:17:39.000000 EdgeGPT-0.3.7/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30099 2023-05-09 15:17:01.000000 EdgeGPT-0.3.7/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-09 15:17:01.000000 EdgeGPT-0.3.7/src/ImageGen.py
```

### Comparing `EdgeGPT-0.3.6/LICENSE` & `EdgeGPT-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.3.6/PKG-INFO` & `EdgeGPT-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.6
+Version: 0.3.7
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.6 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.7 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.3.6/README.md` & `EdgeGPT-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.3.6/setup.py` & `EdgeGPT-0.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.3.6",
+    version="0.3.7",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.3.6/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.3.7/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.6
+Version: 0.3.7
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.6 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.7 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.3.6/src/EdgeGPT.py` & `EdgeGPT-0.3.7/src/EdgeGPT.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,15 @@
 
     def update(
         self,
         prompt: str,
         conversation_style: CONVERSATION_STYLE_TYPE,
         options: list | None = None,
         webpage_context: str | None = None,
-        search_result: bool = False
+        search_result: bool = False,
     ) -> None:
         """
         Updates request object
         """
         if options is None:
             options = [
                 "deepleo",
@@ -258,25 +258,30 @@
                 },
             ],
             "invocationId": str(self.invocation_id),
             "target": "chat",
             "type": 4,
         }
         if search_result:
-            have_search_result = ["InternalSearchQuery","InternalSearchResult","InternalLoaderMessage","RenderCardRequest"]
-            self.struct["arguments"][0]["allowedMessageTypes"]+=have_search_result
+            have_search_result = [
+                "InternalSearchQuery",
+                "InternalSearchResult",
+                "InternalLoaderMessage",
+                "RenderCardRequest",
+            ]
+            self.struct["arguments"][0]["allowedMessageTypes"] += have_search_result
         if webpage_context:
             self.struct["arguments"][0]["previousMessages"] = [
                 {
                     "author": "user",
                     "description": webpage_context,
                     "contextType": "WebPage",
                     "messageType": "Context",
                     "messageId": "discover-web--page-ping-mriduna-----",
-                }
+                },
             ]
         self.invocation_id += 1
 
 
 class _Conversation:
     """
     Conversation API
@@ -357,18 +362,20 @@
             or os.environ.get("ALL_PROXY")
             or os.environ.get("https_proxy")
             or os.environ.get("HTTPS_PROXY")
             or None
         )
         if proxy is not None and proxy.startswith("socks5h://"):
             proxy = "socks5://" + proxy[len("socks5h://") :]
+        transport = httpx.AsyncHTTPTransport(retries=10)
         async with httpx.AsyncClient(
             proxies=proxy,
             timeout=30,
             headers=HEADERS_INIT_CONVER,
+            transport=transport,
         ) as client:
             for cookie in cookies:
                 client.cookies.set(cookie["name"], cookie["value"])
 
             # Send GET request
             response = await client.get(
                 url=os.environ.get("BING_PROXY_URL")
@@ -415,15 +422,15 @@
         prompt: str,
         wss_link: str,
         cookies: str,
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         raw: bool = False,
         options: dict = None,
         webpage_context: str | None = None,
-        search_result : bool = False
+        search_result: bool = False,
     ) -> Generator[str, None, None]:
         """
         Ask a question to the bot
         """
         if self.wss and not self.wss.closed:
             await self.wss.close()
         # Check if websocket is closed
@@ -437,28 +444,28 @@
         if self.request.invocation_id == 0:
             # Construct a ChatHub request
             self.request.update(
                 prompt=prompt,
                 conversation_style=conversation_style,
                 options=options,
                 webpage_context=webpage_context,
-                search_result=search_result
+                search_result=search_result,
             )
         else:
             async with httpx.AsyncClient() as client:
                 response = await client.post(
                     "https://sydney.bing.com/sydney/UpdateConversation/",
                     json={
                         "messages": [
                             {
                                 "author": "user",
                                 "description": webpage_context,
                                 "contextType": "WebPage",
                                 "messageType": "Context",
-                            }
+                            },
                         ],
                         "conversationId": self.request.conversation_id,
                         "source": "cib",
                         "traceId": _get_ran_hex(32),
                         "participant": {"id": self.request.client_id},
                         "conversationSignature": self.request.conversation_signature,
                     },
@@ -489,15 +496,18 @@
                 response = json.loads(obj)
                 if response.get("type") != 2 and raw:
                     yield False, response
                 elif response.get("type") == 1 and response["arguments"][0].get(
                     "messages",
                 ):
                     if not draw:
-                        if(response["arguments"][0]["messages"][0].get("messageType") == "GenerateContentQuery"):
+                        if (
+                            response["arguments"][0]["messages"][0].get("messageType")
+                            == "GenerateContentQuery"
+                        ):
                             for item in cookies:
                                 if item["name"] == "_U":
                                     U = item["value"]
                             async with ImageGenAsync(U, True) as image_generator:
                                 images = await image_generator.get_images(
                                     response["arguments"][0]["messages"][0]["text"],
                                 )
@@ -514,31 +524,40 @@
                                 + images[3]
                                 + ")"
                             )
                             draw = True
                         if (
                             response["arguments"][0]["messages"][0]["contentOrigin"]
                             != "Apology"
-                        ):
-                            if not draw:
-                                resp_txt = result_text+response["arguments"][0]["messages"][0][
-                                    "adaptiveCards"
-                                ][0]["body"][0].get("text", "")
-                                resp_txt_no_link = result_text+response["arguments"][0]["messages"][
-                                    0
-                                ].get("text", "")
-                                if(response["arguments"][0]["messages"][0].get("messageType")):
-                                    resp_txt = resp_txt+response["arguments"][0]["messages"][0][
+                        ) and not draw:
+                            resp_txt = result_text + response["arguments"][0][
+                                "messages"
+                            ][0]["adaptiveCards"][0]["body"][0].get("text", "")
+                            resp_txt_no_link = result_text + response["arguments"][0][
+                                "messages"
+                            ][0].get("text", "")
+                            if response["arguments"][0]["messages"][0].get(
+                                "messageType",
+                            ):
+                                resp_txt = (
+                                    resp_txt
+                                    + response["arguments"][0]["messages"][0][
                                         "adaptiveCards"
-                                    ][0]["body"][0]["inlines"][0].get("text")+"\n"
-                                    result_text = result_text+response["arguments"][0]["messages"][0][
+                                    ][0]["body"][0]["inlines"][0].get("text")
+                                    + "\n"
+                                )
+                                result_text = (
+                                    result_text
+                                    + response["arguments"][0]["messages"][0][
                                         "adaptiveCards"
-                                    ][0]["body"][0]["inlines"][0].get("text")+"\n"
+                                    ][0]["body"][0]["inlines"][0].get("text")
+                                    + "\n"
+                                )
                         yield False, resp_txt
-                        
+
                 elif response.get("type") == 2:
                     if draw:
                         cache = response["item"]["messages"][1]["adaptiveCards"][0][
                             "body"
                         ][0]["text"]
                         response["item"]["messages"][1]["adaptiveCards"][0]["body"][0][
                             "text"
@@ -548,15 +567,16 @@
                         and resp_txt
                     ):
                         response["item"]["messages"][-1]["text"] = resp_txt_no_link
                         response["item"]["messages"][-1]["adaptiveCards"][0]["body"][0][
                             "text"
                         ] = resp_txt
                         print(
-                            f"Preserved the message from being deleted", file=sys.stderr
+                            "Preserved the message from being deleted",
+                            file=sys.stderr,
                         )
                     final = True
                     yield True, response
 
     async def _initial_handshake(self) -> None:
         await self.wss.send(_append_identifier({"protocol": "json", "version": 1}))
         await self.wss.recv()
@@ -621,55 +641,55 @@
     async def ask(
         self,
         prompt: str,
         wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         options: dict = None,
         webpage_context: str | None = None,
-        search_result: bool = False
+        search_result: bool = False,
     ) -> dict:
         """
         Ask a question to the bot
         """
         async for final, response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
             wss_link=wss_link,
             options=options,
             cookies=self.cookies,
             webpage_context=webpage_context,
-            search_result=search_result
+            search_result=search_result,
         ):
             if final:
                 return response
         await self.chat_hub.wss.close()
         return {}
 
     async def ask_stream(
         self,
         prompt: str,
         wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         raw: bool = False,
         options: dict = None,
         webpage_context: str | None = None,
-        search_result: bool = False
+        search_result: bool = False,
     ) -> Generator[str, None, None]:
         """
         Ask a question to the bot
         """
         async for response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
             wss_link=wss_link,
             raw=raw,
             options=options,
             cookies=self.cookies,
             webpage_context=webpage_context,
-            search_result=search_result
+            search_result=search_result,
         ):
             yield response
 
     async def close(self) -> None:
         """
         Close the connection
         """
```

