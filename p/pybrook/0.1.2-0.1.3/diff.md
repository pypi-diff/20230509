# Comparing `tmp/pybrook-0.1.2.tar.gz` & `tmp/pybrook-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybrook-0.1.2.tar", max compression
+gzip compressed data, was "pybrook-0.1.3.tar", max compression
```

## Comparing `pybrook-0.1.2.tar` & `pybrook-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    34916 2023-03-15 11:52:44.410071 pybrook-0.1.2/LICENSE.md
--rw-r--r--   0        0        0      151 2023-03-15 12:02:01.698994 pybrook-0.1.2/README.md
--rw-r--r--   0        0        0      958 2023-03-15 12:06:23.791957 pybrook-0.1.2/pybrook/__init__.py
--rw-r--r--   0        0        0     6237 2023-03-15 12:06:24.093957 pybrook-0.1.2/pybrook/__main__.py
--rw-r--r--   0        0        0     1460 2023-03-15 12:06:23.951957 pybrook-0.1.2/pybrook/config.py
--rw-r--r--   0        0        0      701 2023-03-15 12:06:24.177957 pybrook-0.1.2/pybrook/consumers/__init__.py
--rw-r--r--   0        0        0    10592 2023-03-15 12:34:21.482817 pybrook-0.1.2/pybrook/consumers/base.py
--rw-r--r--   0        0        0     7310 2023-03-15 12:06:24.012957 pybrook-0.1.2/pybrook/consumers/dependency_resolver.py
--rw-r--r--   0        0        0     4541 2023-03-15 12:34:21.511817 pybrook-0.1.2/pybrook/consumers/field_generator.py
--rw-r--r--   0        0        0     5219 2023-03-15 12:34:21.499817 pybrook-0.1.2/pybrook/consumers/splitter.py
--rw-r--r--   0        0        0     6139 2023-03-15 13:02:19.084478 pybrook-0.1.2/pybrook/consumers/worker.py
--rw-r--r--   0        0        0     1720 2023-03-15 12:06:24.115957 pybrook-0.1.2/pybrook/encoding.py
--rw-r--r--   0        0        0      701 2023-03-15 12:06:23.737957 pybrook-0.1.2/pybrook/examples/__init__.py
--rw-r--r--   0        0        0     2571 2023-03-15 12:06:24.032957 pybrook-0.1.2/pybrook/examples/demo.py
--rw-r--r--   0        0        0     2469 2023-03-15 12:06:23.970957 pybrook-0.1.2/pybrook/examples/ztm.py
--rw-r--r--   0        0        0   697071 2023-03-15 11:43:55.678584 pybrook-0.1.2/pybrook/frontend/build/bundle.css
--rw-r--r--   0        0        0   263192 2023-03-15 11:43:55.351585 pybrook-0.1.2/pybrook/frontend/build/bundle.js
--rw-r--r--   0        0        0   875724 2023-03-15 11:43:55.355585 pybrook-0.1.2/pybrook/frontend/build/bundle.js.map
--rw-r--r--   0        0        0     3127 2023-03-15 11:43:55.135586 pybrook-0.1.2/pybrook/frontend/favicon.png
--rw-r--r--   0        0        0      890 2023-03-15 11:43:55.135586 pybrook-0.1.2/pybrook/frontend/global.css
--rw-r--r--   0        0        0      386 2023-03-15 11:43:55.678584 pybrook-0.1.2/pybrook/frontend/index.html
--rw-r--r--   0        0        0    32737 2023-03-15 12:33:14.259023 pybrook-0.1.2/pybrook/models.py
--rw-r--r--   0        0        0     2238 2023-03-15 12:06:24.198957 pybrook-0.1.2/pybrook/schemas.py
--rw-r--r--   0        0        0     1678 2023-03-15 13:02:56.438453 pybrook-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 pybrook-0.1.2/setup.py
--rw-r--r--   0        0        0     1342 1970-01-01 00:00:00.000000 pybrook-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34916 2023-05-09 13:38:36.699045 pybrook-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0     6563 2023-05-09 14:48:44.826974 pybrook-0.1.3/docs/index.md
+-rw-r--r--   0        0        0      958 2023-05-09 13:38:36.706045 pybrook-0.1.3/pybrook/__init__.py
+-rw-r--r--   0        0        0     6237 2023-05-09 13:38:36.706045 pybrook-0.1.3/pybrook/__main__.py
+-rw-r--r--   0        0        0     1461 2023-05-09 13:38:36.706045 pybrook-0.1.3/pybrook/config.py
+-rw-r--r--   0        0        0      701 2023-05-09 13:38:36.706045 pybrook-0.1.3/pybrook/consumers/__init__.py
+-rw-r--r--   0        0        0    10592 2023-05-09 13:38:36.706045 pybrook-0.1.3/pybrook/consumers/base.py
+-rw-r--r--   0        0        0     7310 2023-05-09 13:38:36.707045 pybrook-0.1.3/pybrook/consumers/dependency_resolver.py
+-rw-r--r--   0        0        0     4541 2023-05-09 14:49:20.159821 pybrook-0.1.3/pybrook/consumers/field_generator.py
+-rw-r--r--   0        0        0     5231 2023-05-09 13:38:36.707045 pybrook-0.1.3/pybrook/consumers/splitter.py
+-rw-r--r--   0        0        0     6138 2023-05-09 13:38:36.707045 pybrook-0.1.3/pybrook/consumers/worker.py
+-rw-r--r--   0        0        0     1720 2023-05-09 13:38:36.707045 pybrook-0.1.3/pybrook/encoding.py
+-rw-r--r--   0        0        0      701 2023-05-09 13:38:36.707045 pybrook-0.1.3/pybrook/examples/__init__.py
+-rw-r--r--   0        0        0     2571 2023-05-09 13:38:36.708045 pybrook-0.1.3/pybrook/examples/demo.py
+-rw-r--r--   0        0        0     2469 2023-05-09 13:38:36.708045 pybrook-0.1.3/pybrook/examples/ztm.py
+-rw-r--r--   0        0        0   697071 2023-05-09 13:38:36.712045 pybrook-0.1.3/pybrook/frontend/build/bundle.css
+-rw-r--r--   0        0        0   263192 2023-05-09 13:38:36.715045 pybrook-0.1.3/pybrook/frontend/build/bundle.js
+-rw-r--r--   0        0        0   875724 2023-05-09 13:38:36.724045 pybrook-0.1.3/pybrook/frontend/build/bundle.js.map
+-rw-r--r--   0        0        0     3127 2023-05-09 13:38:36.724045 pybrook-0.1.3/pybrook/frontend/favicon.png
+-rw-r--r--   0        0        0      890 2023-05-09 13:38:36.724045 pybrook-0.1.3/pybrook/frontend/global.css
+-rw-r--r--   0        0        0      386 2023-05-09 13:38:36.724045 pybrook-0.1.3/pybrook/frontend/index.html
+-rw-r--r--   0        0        0    32825 2023-05-09 13:38:36.724045 pybrook-0.1.3/pybrook/models.py
+-rw-r--r--   0        0        0     2238 2023-05-09 13:38:36.725045 pybrook-0.1.3/pybrook/schemas.py
+-rw-r--r--   0        0        0     1711 2023-05-09 14:30:42.261475 pybrook-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7950 1970-01-01 00:00:00.000000 pybrook-0.1.3/setup.py
+-rw-r--r--   0        0        0     7754 1970-01-01 00:00:00.000000 pybrook-0.1.3/PKG-INFO
```

### Comparing `pybrook-0.1.2/LICENSE.md` & `pybrook-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.2/pybrook/__init__.py` & `pybrook-0.1.3/pybrook/__init__.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.2/pybrook/__main__.py` & `pybrook-0.1.3/pybrook/__main__.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.2/pybrook/config.py` & `pybrook-0.1.3/pybrook/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,12 +27,12 @@
 ARTIFICIAL_NAMESPACE = config('ARTIFICIAL_NAMESPACE',
                               str,
                               default='artificial')
 DEFAULT_WORKERS = config('DEFAULT_WORKERS', int, default=4)
 
 WEBSOCKET_XREAD_BLOCK = config('WEBSOCKET_XREAD_BLOCK', int, default=100)
 
-WEBSOCKET_XREAD_COUNT = config('WEBSOCKET_XREAD_COUNT', int, default=100)
+WEBSOCKET_XREAD_COUNT = config('WEBSOCKET_XREAD_COUNT', int, default=1000)
 
 WEBSOCKET_WAIT_TIME = config('WEBSOCKET_WAIT_TIME', float, default=0.01)
 
 WEBSOCKET_PING_INTERVAL = config('WEBSOCKET_PING_INTERVAL', int, default=30)
```

### Comparing `pybrook-0.1.2/pybrook/consumers/__init__.py` & `pybrook-0.1.3/pybrook/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.2/pybrook/consumers/base.py` & `pybrook-0.1.3/pybrook/consumers/base.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.2/pybrook/consumers/dependency_resolver.py` & `pybrook-0.1.3/pybrook/consumers/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.2/pybrook/consumers/field_generator.py` & `pybrook-0.1.3/pybrook/consumers/field_generator.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.2/pybrook/consumers/splitter.py` & `pybrook-0.1.3/pybrook/consumers/splitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             obj_msg_id = execute("INCR", msg_id_key)
             out_stream = f'{SPECIAL_CHAR}{self.namespace}{SPECIAL_CHAR}split'
             message[MSG_ID_FIELD] = f'"{obj_id}:{obj_msg_id}"'
             execute("XADD", out_stream, '*', *chain(*message.items()))
 
         for s in self._input_streams:
             gears_builder("StreamReader").foreach(process_message).register(
-                s, trimStream=False, mode="sync", batch=1000)
+                s, trimStream=False, mode="sync", batch=1000, duration=1)
 
     def register_builder(self, conn: redis.Redis):
         scope = {
             name: value
             for name, value in globals().items()
             if type(value) in {int, list, str, float}  # noqa: WPS516
             and not name.startswith('__')
```

### Comparing `pybrook-0.1.2/pybrook/consumers/worker.py` & `pybrook-0.1.3/pybrook/consumers/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     workers: int = DEFAULT_WORKERS
 
 
 class WorkerManager:
     def __init__(self,
                  consumers: Iterable[BaseStreamConsumer],
                  config: Dict[str, ConsumerConfig] = None,
-                 enable_gears: bool = False):
+                 enable_gears: bool = True):
         self.consumers = consumers
         self.config = config or {}
         self.redis_urls: Set[str] = {c.redis_url for c in consumers}
         self.gears_consumers: List[GearsStreamConsumer] = [
             c for c in consumers if enable_gears and isinstance(c, GearsStreamConsumer)
         ]
         self.regular_consumers: List[BaseStreamConsumer] = [
```

### Comparing `pybrook-0.1.2/pybrook/encoding.py` & `pybrook-0.1.3/pybrook/encoding.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.2/pybrook/examples/__init__.py` & `pybrook-0.1.3/pybrook/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.2/pybrook/examples/demo.py` & `pybrook-0.1.3/pybrook/examples/demo.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.2/pybrook/examples/ztm.py` & `pybrook-0.1.3/pybrook/examples/ztm.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.2/pybrook/frontend/build/bundle.css` & `pybrook-0.1.3/pybrook/frontend/build/bundle.css`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.2/pybrook/frontend/build/bundle.js` & `pybrook-0.1.3/pybrook/frontend/build/bundle.js`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.2/pybrook/frontend/build/bundle.js.map` & `pybrook-0.1.3/pybrook/frontend/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.2/pybrook/frontend/favicon.png` & `pybrook-0.1.3/pybrook/frontend/favicon.png`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.2/pybrook/frontend/global.css` & `pybrook-0.1.3/pybrook/frontend/global.css`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.2/pybrook/models.py` & `pybrook-0.1.3/pybrook/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -542,26 +542,28 @@
                     except asyncio.TimeoutError:
                         ...  # Everything is OK
                     except (fastapi.WebSocketDisconnect, AssertionError):
                         active = False
                     else:
                         last_ping = time()
                 messages = await redis_conn.xread({stream_name: last_msg},
-                                                  count=WEBSOCKET_XREAD_BLOCK,
-                                                  block=WEBSOCKET_XREAD_COUNT)
+                                                  count=WEBSOCKET_XREAD_COUNT,
+                                                  block=WEBSOCKET_XREAD_BLOCK)
                 if messages:
                     # Wiadomości w strumieniach są mapami
                     for m_data in dict(messages)[stream_name]:
                         last_msg, payload = m_data
                         try:
                             await websocket.send_text(
                                 model_cls(
                                     **decode_stream_message(payload)).json())
                         except ConnectionClosedOK:
                             active = False
+                        except RuntimeError:
+                            active = False
             try:
                 await websocket.close()
             except RuntimeError:
                 logger.info('WebSocket connection closed by client')
             else:
                 logger.info('WebSocket connection closed by server')
```

### Comparing `pybrook-0.1.2/pybrook/schemas.py` & `pybrook-0.1.3/pybrook/schemas.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.2/pyproject.toml` & `pybrook-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybrook"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Michał Rokita <mrokita@mrokita.pl>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 [tool.poetry.scripts]
 pybrook = "pybrook.__main__:main"
@@ -25,17 +25,17 @@
 orjson = "^3.6.5"
 locust = "^2.6.1"
 pydantic = "^1.10.6"
 
 
 [tool.poetry.group.dev.dependencies]
 # docs
-mkdocstrings = "^0.17.0"
-mkdocs = "^1.1.2"
-mkdocs-material = "^8.1.8"
+mkdocstrings = {extras = ["python"], version = "^0.20.0"}
+mkdocs = "^1.4.2"
+mkdocs-material = "^9.1.3"
 mike = "^1.0.1"
 livereload = "^2.6.3"
 
 # formatting
 yapf = "^0.31.0"
 isort = "^5.5.1"
```

