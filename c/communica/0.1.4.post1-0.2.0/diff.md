# Comparing `tmp/communica-0.1.4.post1.tar.gz` & `tmp/communica-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "communica-0.1.4.post1.tar", last modified: Mon Apr 10 08:34:40 2023, max compression
+gzip compressed data, was "communica-0.2.0.tar", last modified: Tue May  9 20:48:50 2023, max compression
```

## Comparing `communica-0.1.4.post1.tar` & `communica-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 08:34:40.256314 communica-0.1.4.post1/
--rw-rw-rw-   0        0        0      568 2023-03-25 20:48:52.000000 communica-0.1.4.post1/LICENSE.txt
--rw-rw-rw-   0        0        0     2190 2023-04-10 08:34:40.256314 communica-0.1.4.post1/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2023-04-04 20:46:58.000000 communica-0.1.4.post1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 08:34:40.238315 communica-0.1.4.post1/communica/
--rw-rw-rw-   0        0        0      101 2023-02-15 13:48:00.000000 communica-0.1.4.post1/communica/__init__.py
--rw-rw-rw-   0        0        0      130 2023-03-19 21:29:46.000000 communica-0.1.4.post1/communica/clients.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:34:40.248315 communica-0.1.4.post1/communica/connectors/
--rw-rw-rw-   0        0        0      170 2023-03-31 19:34:58.000000 communica-0.1.4.post1/communica/connectors/__init__.py
--rw-rw-rw-   0        0        0     2803 2023-03-24 12:30:50.000000 communica-0.1.4.post1/communica/connectors/_stream_local.py
--rw-rw-rw-   0        0        0     5358 2023-03-30 10:48:08.000000 communica-0.1.4.post1/communica/connectors/base.py
--rw-rw-rw-   0        0        0    22199 2023-04-10 08:11:15.000000 communica-0.1.4.post1/communica/connectors/rabbitmq.py
--rw-rw-rw-   0        0        0     9243 2023-03-30 11:38:51.000000 communica-0.1.4.post1/communica/connectors/stream.py
--rw-rw-rw-   0        0        0      468 2023-03-19 11:58:01.000000 communica-0.1.4.post1/communica/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:34:40.251314 communica-0.1.4.post1/communica/pairs/
--rw-rw-rw-   0        0        0      223 2023-03-19 15:01:07.000000 communica-0.1.4.post1/communica/pairs/__init__.py
--rw-rw-rw-   0        0        0     2667 2023-03-21 21:55:22.000000 communica-0.1.4.post1/communica/pairs/base.py
--rw-rw-rw-   0        0        0    10308 2023-04-10 08:23:55.000000 communica-0.1.4.post1/communica/pairs/route.py
--rw-rw-rw-   0        0        0    15514 2023-04-10 08:02:57.000000 communica-0.1.4.post1/communica/pairs/simple.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:34:40.253315 communica-0.1.4.post1/communica/serializers/
--rw-rw-rw-   0        0        0      176 2023-03-19 20:57:46.000000 communica-0.1.4.post1/communica/serializers/__init__.py
--rw-rw-rw-   0        0        0      657 2023-03-18 18:41:17.000000 communica-0.1.4.post1/communica/serializers/base.py
--rw-rw-rw-   0        0        0      315 2023-03-18 19:40:10.000000 communica-0.1.4.post1/communica/serializers/json.py
--rw-rw-rw-   0        0        0      128 2023-03-19 21:29:36.000000 communica-0.1.4.post1/communica/servers.py
--rw-rw-rw-   0        0        0     3077 2023-04-04 16:50:40.000000 communica-0.1.4.post1/communica/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:34:40.243316 communica-0.1.4.post1/communica.egg-info/
--rw-rw-rw-   0        0        0     2190 2023-04-10 08:34:40.000000 communica-0.1.4.post1/communica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      716 2023-04-10 08:34:40.000000 communica-0.1.4.post1/communica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 08:34:40.000000 communica-0.1.4.post1/communica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-04-10 08:34:40.000000 communica-0.1.4.post1/communica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-10 08:34:40.000000 communica-0.1.4.post1/communica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1056 2023-04-10 08:33:32.000000 communica-0.1.4.post1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-10 08:34:40.256314 communica-0.1.4.post1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-10 08:34:40.255314 communica-0.1.4.post1/tests/
--rw-rw-rw-   0        0        0     1040 2023-04-01 18:26:37.000000 communica-0.1.4.post1/tests/test_connectors.py
--rw-rw-rw-   0        0        0     2940 2023-04-08 16:43:45.000000 communica-0.1.4.post1/tests/test_entities.py
+drwxrwxrwx   0        0        0        0 2023-05-09 20:48:50.988315 communica-0.2.0/
+-rw-rw-rw-   0        0        0      568 2023-03-25 20:48:52.000000 communica-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2231 2023-05-09 20:48:50.987316 communica-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-04-04 20:46:58.000000 communica-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 20:48:50.962316 communica-0.2.0/communica/
+-rw-rw-rw-   0        0        0      101 2023-02-15 13:48:00.000000 communica-0.2.0/communica/__init__.py
+-rw-rw-rw-   0        0        0      130 2023-03-19 21:29:46.000000 communica-0.2.0/communica/clients.py
+drwxrwxrwx   0        0        0        0 2023-05-09 20:48:50.973316 communica-0.2.0/communica/connectors/
+-rw-rw-rw-   0        0        0      170 2023-03-31 19:34:58.000000 communica-0.2.0/communica/connectors/__init__.py
+-rw-rw-rw-   0        0        0     2803 2023-03-24 12:30:50.000000 communica-0.2.0/communica/connectors/_stream_local.py
+-rw-rw-rw-   0        0        0     5455 2023-05-01 12:51:49.000000 communica-0.2.0/communica/connectors/base.py
+-rw-rw-rw-   0        0        0    28038 2023-05-08 07:38:53.000000 communica-0.2.0/communica/connectors/rabbitmq.py
+-rw-rw-rw-   0        0        0    10130 2023-05-04 12:12:20.000000 communica-0.2.0/communica/connectors/stream.py
+-rw-rw-rw-   0        0        0     1945 2023-05-08 09:05:11.000000 communica-0.2.0/communica/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-09 20:48:50.976315 communica-0.2.0/communica/pairs/
+-rw-rw-rw-   0        0        0      223 2023-03-19 15:01:07.000000 communica-0.2.0/communica/pairs/__init__.py
+-rw-rw-rw-   0        0        0     2975 2023-05-04 13:02:31.000000 communica-0.2.0/communica/pairs/base.py
+-rw-rw-rw-   0        0        0     9588 2023-05-08 10:26:04.000000 communica-0.2.0/communica/pairs/route.py
+-rw-rw-rw-   0        0        0    16081 2023-05-08 10:15:06.000000 communica-0.2.0/communica/pairs/simple.py
+drwxrwxrwx   0        0        0        0 2023-05-09 20:48:50.981315 communica-0.2.0/communica/serializers/
+-rw-rw-rw-   0        0        0      242 2023-05-08 07:15:52.000000 communica-0.2.0/communica/serializers/__init__.py
+-rw-rw-rw-   0        0        0     1274 2023-05-09 20:44:57.000000 communica-0.2.0/communica/serializers/adaptix.py
+-rw-rw-rw-   0        0        0      657 2023-03-18 18:41:17.000000 communica-0.2.0/communica/serializers/base.py
+-rw-rw-rw-   0        0        0      315 2023-03-18 19:40:10.000000 communica-0.2.0/communica/serializers/json.py
+-rw-rw-rw-   0        0        0      128 2023-03-19 21:29:36.000000 communica-0.2.0/communica/servers.py
+-rw-rw-rw-   0        0        0     4246 2023-05-08 07:38:20.000000 communica-0.2.0/communica/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 20:48:50.968315 communica-0.2.0/communica.egg-info/
+-rw-rw-rw-   0        0        0     2231 2023-05-09 20:48:50.000000 communica-0.2.0/communica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      811 2023-05-09 20:48:50.000000 communica-0.2.0/communica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 20:48:50.000000 communica-0.2.0/communica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-05-09 20:48:50.000000 communica-0.2.0/communica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-09 20:48:50.000000 communica-0.2.0/communica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1128 2023-05-08 07:10:36.000000 communica-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 20:48:50.988315 communica-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 20:48:50.986315 communica-0.2.0/tests/
+-rw-rw-rw-   0        0        0     2146 2023-05-04 12:13:21.000000 communica-0.2.0/tests/test_connectors.py
+-rw-rw-rw-   0        0        0     6508 2023-05-08 10:49:51.000000 communica-0.2.0/tests/test_entities.py
+-rw-rw-rw-   0        0        0     2481 2023-04-23 14:30:49.000000 communica-0.2.0/tests/test_rmq_conn_check_policy.py
+-rw-rw-rw-   0        0        0     1081 2023-05-08 10:22:35.000000 communica-0.2.0/tests/test_serializers.py
```

### Comparing `communica-0.1.4.post1/LICENSE.txt` & `communica-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `communica-0.1.4.post1/PKG-INFO` & `communica-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: communica
-Version: 0.1.4.post1
+Version: 0.2.0
 Summary: Easy to use IPC library
 Author-email: Elchin Sarkarov <elchin751@gmail.com>
 Project-URL: Homepage, https://github.com/elchinchel/communica-py
 Project-URL: Bug Tracker, https://github.com/elchinchel/communica-py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
 Provides-Extra: df
 Provides-Extra: orjson
+Provides-Extra: adaptix
 Provides-Extra: pydantic
 Provides-Extra: rabbitmq
 License-File: LICENSE.txt
 
 # Easy to use IPC library
 
     This library is still in development process.
```

### Comparing `communica-0.1.4.post1/README.md` & `communica-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `communica-0.1.4.post1/communica/connectors/_stream_local.py` & `communica-0.2.0/communica/connectors/_stream_local.py`

 * *Files identical despite different names*

### Comparing `communica-0.1.4.post1/communica/connectors/base.py` & `communica-0.2.0/communica/connectors/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from abc import abstractmethod, ABC
 from typing import Any, Protocol, Callable, Awaitable, AsyncGenerator
 from typing_extensions import Self
 
 from communica.utils import logger, json_dumpb, json_loadb
 
 
-HandshakeGen = AsyncGenerator['bytes | HandshakeOk', bytes]
+HandshakeGen = AsyncGenerator['dict | HandshakeOk', dict]
 
 
 class Handshaker(Protocol):
     async def __call__(self, connection: 'BaseConnection') -> HandshakeGen: ...
 
 
 class ClientConnectedCB(Protocol):
     def __call__(self, connection: 'BaseConnection'): ...
 
 
 class RequestReceivedCB(Protocol):
-    def __call__(self, metadata: Any, raw_data: bytes): ...
+    def __call__(self, metadata: Any, raw_data: memoryview): ...
 
 
 class HandshakeOk: ...
 
 
 class HandshakeFail(Exception):
     def __init__(self, reason: str) -> None:
@@ -39,15 +39,15 @@
         return cls(obj['reason'])
 
 
 class BaseConnection(ABC):
     __slots__ = ('_alive', '_handshake_result')
 
     @property
-    def is_alive(self):
+    def is_alive(self) -> bool:
         try:
             return self._alive
         except AttributeError:
             return False
 
     def get_handshake_result(self) -> HandshakeOk:
         """
@@ -72,17 +72,19 @@
             handshaker: Handshaker,
             send_message: Callable[[bytes], Awaitable],
             recv_message: Callable[[], Awaitable[bytes]]
     ) -> 'HandshakeOk':
         handshake_gen = handshaker(self)
 
         async def send_to_gen(data):
+            if data is not None:
+                data = json_loadb(data)
             gen_return = await handshake_gen.asend(data)
-            if isinstance(gen_return, bytes):
-                return gen_return
+            if isinstance(gen_return, dict):
+                return json_dumpb(gen_return)
             elif isinstance(gen_return, HandshakeOk):
                 if hasattr(self, '_handshake_result'):
                     raise RuntimeError('Handshake repeated on same connection')
                 self._handshake_result = gen_return
                 return gen_return
             else:
                 raise StopAsyncIteration
```

### Comparing `communica-0.1.4.post1/communica/connectors/rabbitmq.py` & `communica-0.2.0/communica/connectors/rabbitmq.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # cursed.
 
 import asyncio
+import weakref
 
 try:
     import aiormq
-    _HAS_AIORMQ = True
-except ImportError:
-    _HAS_AIORMQ = False
+    _HAVE_AIORMQ = True
+except ModuleNotFoundError:
+    _HAVE_AIORMQ = False
 else:
     from yarl import URL
 
 from enum import Enum
 from typing import Any
 from datetime import datetime, timedelta
 from collections import deque
 
 from typing_extensions import Self
 
 from communica.utils import (
-    NULL_CHAR, json_dumpb, json_loadb, HasLoopMixin
+    NULL_CHAR, HasLoopMixin, json_dumpb, json_loadb,
+    exc_log_callback
 )
 
 from communica.connectors.base import (
     BaseConnection, BaseConnector,
     RequestReceivedCB, ClientConnectedCB,
     Handshaker, HandshakeFail
 )
@@ -33,68 +35,206 @@
 
 class _MessageType(str, Enum):
     CONNECT_REQUEST = 'communica_client_connect'
     CONNECT_RESPONSE = 'communica_client_connect_ok'
     HS_NEXT = 'communica_handshake_next'
     HS_FAIL = 'communica_handshake_fail'
     HS_DONE = 'communica_handshake_done'
+    LISTENING = 'listening'
     MESSAGE = 'message'
     CLOSE = 'close'
 
 
-_connections: \
-    'dict[URL, aiormq.Connection | asyncio.Future[aiormq.Connection]]' = {}
+_connections: '''dict[
+    URL,
+    aiormq.abc.AbstractConnection | asyncio.Future[aiormq.abc.AbstractConnection]
+]''' = {}
 
 
 def _closed_exceptions():
     return (aiormq.exceptions.ChannelClosed,
             aiormq.exceptions.ConnectionClosed)
 
 
 class MessageWaiter(HasLoopMixin):
-    __slots__ = ('_waiter', '_messages')
+    __slots__ = ('_waiter', '_messages', '_timeout')
 
     @classmethod
     async def new(
             cls,
             chan: 'aiormq.abc.AbstractChannel',
             queue: str,
-            no_ack: bool
+            *,
+            no_ack: bool,
+            timeout: 'int | None' = None
     ):
         inst = cls()
         inst._waiter = None
+        inst._timeout = timeout
         inst._messages = deque()
 
         await chan.basic_consume(queue, inst._callback, no_ack=no_ack)
 
         return inst
 
     async def _callback(self, message: 'aiormq.abc.DeliveredMessage'):
         if not self._waiter or self._waiter.done():
             self._messages.append(message)
         else:
             self._waiter.set_result(message)
             self._waiter = None
 
+    def set_timeout_duration(self, timeout: int):
+        if self._waiter and not self._waiter.done():
+            raise RuntimeError('Waiter not completed')
+        self._timeout = timeout
+
+    def _set_timeout(self, fut: asyncio.Future):
+        if not fut.done():
+            fut.set_exception(asyncio.TimeoutError)
+
     async def wait(self) -> 'aiormq.abc.DeliveredMessage':
         if self._messages:
             return self._messages.popleft()
 
+        if self._waiter and not self._waiter.done():
+            raise RuntimeError(f'Duplicate .wait() call on {self!r}')
+
         self._waiter = self._get_loop().create_future()
+
+        if self._timeout:
+            self._get_loop().call_later(
+                self._timeout, self._set_timeout, self._waiter)
+
         return await self._waiter
 
 
+class ConnectionCheckPolicy(HasLoopMixin):
+    period: float
+
+    def message_sent(self):
+        pass
+
+    def message_received(self):
+        pass
+
+    def replace_conn(self, conn: 'RmqConnection') -> Self:
+        raise NotImplementedError
+
+    def _set_handle(self, period: 'float | None' = None):
+        if period is None:
+            self._last_message = self._loop.time()
+            period = self.period
+        self._handle = self._loop.call_later(period, self._trigger)  # type: ignore
+
+
+class ServerCheckPolicy(ConnectionCheckPolicy):
+    def __init__(self, conn: 'RmqConnection', period: float) -> None:
+        self._get_loop()
+
+        self.period = period
+        self._waiter = self._loop.create_future()
+
+        self._set_handle()
+
+        self._send_task = self._loop.create_task(self._sender())
+        self._send_task.add_done_callback(exc_log_callback)
+        self._conn = weakref.ref(conn, self._get_died_cb())
+
+    def replace_conn(self, conn: 'RmqConnection'):
+        self._conn.__callback__(None, defuse=True)  # type: ignore
+        self._conn = weakref.ref(conn, self._get_died_cb())
+        return self
+
+    def _get_died_cb(self):
+        armed = True
+
+        def conn_died(_, defuse=False):
+            nonlocal armed
+
+            if defuse:
+                armed = False
+            elif armed:
+                self._waiter.set_result(False)
+
+        return conn_died
+
+    def _trigger(self):
+        if self._waiter.done():
+            return
+
+        time_diff = self._loop.time() - self._last_message
+        if time_diff < self.period:
+            self._set_handle(self.period - time_diff)
+            return
+
+        self._handle = None
+        self._waiter.set_result(True)
+        self._waiter = self._loop.create_future()
+
+    async def _sender(self):
+        while (await self._waiter):
+            if (conn := self._conn()) is None:
+                return  # pragma: no cover
+            await conn._send(_MessageType.LISTENING, b'')
+            del(conn)  # deleting reference
+            if self._handle is None:
+                self._set_handle()
+
+    def message_sent(self):
+        if self._handle is None:
+            self._set_handle()
+        else:
+            self._last_message = self._loop.time()
+
+
+class ClientCheckPolicy(ConnectionCheckPolicy):
+    def __init__(self, conn: 'RmqConnection', period: float) -> None:
+        self._get_loop()
+
+        self.period = period
+        self._set_handle()
+
+        self._conn = weakref.ref(conn)
+        self._close_task = None
+
+    def replace_conn(self, conn: 'RmqConnection'):
+        self._conn = weakref.ref(conn)
+        return self
+
+    def _trigger(self):
+        if (conn := self._conn()) is None:
+            return
+
+        time_diff = self._loop.time() - self._last_message
+        if time_diff < self.period:
+            self._set_handle(self.period - time_diff)
+            return
+
+        self._close_task = self._loop.create_task(conn.close())
+
+    def message_received(self):
+        if self._close_task is None:
+            self._last_message = self._loop.time()
+
+
 class RmqConnection(BaseConnection):
-    __slots__ = ('_connector', '_rmq_chan', '_ready',
-                 '_recv_queue', '_send_queue')
+    __slots__ = ('_connector', '_rmq_chan', '_ready', '_closing',
+                 '_recv_queue', '_send_queue', '_check_policy',
+                 '__weakref__')
 
     _ready: asyncio.Event
+    _closing: 'asyncio.Future | None'
     _rmq_chan: 'aiormq.abc.AbstractChannel'
     _connector: 'RmqConnector'
 
+    @property
+    def is_alive(self):
+        return self._ready.is_set()
+
     @classmethod
     async def _do_handshake_and_create_connection(
             cls,
             chan: 'aiormq.abc.AbstractChannel',
             connector: 'RmqConnector',
             handshaker: Handshaker,
             resp_waiter: MessageWaiter,
@@ -131,54 +271,69 @@
                     message_type=_MessageType.HS_FAIL
                 )
             )
             raise
 
         inst._ready = asyncio.Event()
         inst._ready.set()
+        inst._closing = None
         inst._connector = connector
 
         return inst
 
+    def __repr__(self) -> str:
+        cls_name = self.__class__.__name__
+        if self._ready:
+            state = f'on channel {self._rmq_chan.number}'
+        else:
+            state = 'not ready'
+        return f'<{cls_name} {state}>'
+
     def _set_run_data(
             self,
             chan: 'aiormq.abc.AbstractChannel',
+            policy: ConnectionCheckPolicy,
             recv_queue: str,
             send_queue: str
     ):
         self._rmq_chan = chan
+        self._check_policy = policy
         self._recv_queue, self._send_queue = recv_queue, send_queue
 
     def update(self, connection: Self) -> None:
         if self._connector._connect_id != connection._connector._connect_id:
             raise ValueError('Got connection with different connect_id')
         if connection._rmq_chan.is_closed:
             raise ValueError('Got connection with closed channel')
+
         self._ready.set()
+        self._closing = None
         self._rmq_chan = connection._rmq_chan
+        self._check_policy = connection._check_policy.replace_conn(self)
 
     async def send(self, metadata: Any, raw_data: bytes):
         body = json_dumpb(metadata) + NULL_CHAR + raw_data
         try:
-            await self._send(body)
+            await self._send(_MessageType.MESSAGE, body)
         except _closed_exceptions():
             self._ready.clear()
-            await self._send(body)  # retry once after channel opened
+            await self._send(_MessageType.MESSAGE, body)  # retry once after channel opened
         except aiormq.exceptions.AMQPError:
             self._ready.clear()
             raise
+        self._check_policy.message_sent()
 
-    async def _send(self, body: bytes):
+    async def _send(self, msg_type: _MessageType, body: bytes):
         await self._ready.wait()
         await self._rmq_chan.basic_publish(
             body,
             exchange=self._connector.exchange,
             routing_key=self._send_queue,
             properties=aiormq.spec.Basic.Properties(
-                message_type=_MessageType.MESSAGE,
+                message_type=msg_type,
             )
         )
 
     async def run_until_fail(
             self,
             request_received_cb: RequestReceivedCB
     ) -> None:
@@ -193,72 +348,87 @@
             await self._rmq_chan.basic_ack(message.delivery_tag)
 
         waiter = await MessageWaiter.new(self._rmq_chan,
                                          self._recv_queue, no_ack=False)
 
         while not self._rmq_chan.is_closed:
             message = await waiter.wait()
-            print(message.header.properties.message_type)
+
+            self._check_policy.message_received()
 
             if message.header.properties.message_type == _MessageType.MESSAGE:
                 null_pos = message.body.find(NULL_CHAR)
                 if null_pos == -1:
                     await ack_message(message)
                     await self._close(True)
                     raise ValueError('Got message without metadata separator')
 
                 metadata = json_loadb(message.body[:null_pos])
                 request_received_cb(metadata, message.body[null_pos+1:])
                 await ack_message(message)
 
+            elif message.header.properties.message_type == _MessageType.LISTENING:
+                await ack_message(message)
+                continue
+
             elif message.header.properties.message_type == _MessageType.CLOSE:
+                await ack_message(message)
+
                 timestamp = message.header.properties.timestamp
+
                 if timestamp is None:
-                    await ack_message(message)
                     await self._close(True)
                     raise ValueError('Got close request without timestamp')
-                await ack_message(message)
+
                 if datetime.now() - timestamp > timedelta(seconds=5):
                     continue
+
                 await self._close(False)
                 return
 
             else:
                 await ack_message(message)
                 await self._close(True)
                 message_type = message.header.properties.message_type
                 raise ValueError('Unknown message in message queue, '
                                 f'got type {message_type!r}')
 
     async def close(self) -> None:
         await self._close(True)
 
     async def _close(self, send_close_request: bool):
+        if self._closing:
+            return await self._closing
+
         if not self._ready.is_set():
             return
+
         self._ready.clear()
 
         if self._rmq_chan.is_closed or self._rmq_chan.connection.is_closed:
             return
 
+        self._closing = asyncio.get_running_loop().create_future()
         try:
             if send_close_request:
                 await self._rmq_chan.basic_publish(
                     b'',
                     exchange=self._connector.exchange,
                     routing_key=self._send_queue,
                     properties=aiormq.spec.Basic.Properties(
                         timestamp=datetime.now(),
                         message_type=_MessageType.CLOSE,
                     )
                 )
             await self._rmq_chan.close()
-            await self._connector._check_connection_use()
-        except _closed_exceptions():
+        except _closed_exceptions() + (asyncio.CancelledError,):
             return
+        finally:
+            await self._connector._check_connection_use()
+            self._closing.set_result(None)
 
 
 class RmqServer(asyncio.AbstractServer):
     @property
     def exchange(self):
         return self._connector._exchange
 
@@ -266,43 +436,50 @@
             self,
             connector: 'RmqConnector',
             rmq_chan: 'aiormq.abc.AbstractChannel',
             handshaker: Handshaker,
             client_connected_cb: ClientConnectedCB
     ) -> None:
         self._chan = rmq_chan
+        self._closing = None
         self._connector = connector
         self._handshaker = handshaker
         self._client_connected_cb = client_connected_cb
 
     def is_serving(self):
         """Return True if the server is accepting connections."""
         return not self._chan.is_closed
 
     def close(self):
         async def close_channel():
             if not self._chan.is_closed:
                 await self._chan.close()
             await self._connector._check_connection_use()
-            del(self._close_task)
+            if self._closing is not asyncio.current_task():
+                raise RuntimeError('Server closing task changed')
+            self._closing = None
 
-        self._close_task = asyncio.create_task(close_channel())
+        if not self._closing or self._closing.done():
+            self._closing = asyncio.create_task(close_channel())
 
     async def wait_closed(self):
-        if not hasattr(self, '_close_task'):
+        if not self._closing or self._closing.done():
             raise RuntimeError('wait_closed() should be '
                                'called right after close() method')
-        await self._close_task
+        await self._closing
 
     async def _on_connect(self, message: 'aiormq.abc.DeliveredMessage'):
         if message.header.properties.message_type != _MessageType.CONNECT_REQUEST:
+            await self._connector._ack_message(self._chan, message)
             raise ValueError('Unknown message in connect request queue')
 
         if message.header.properties.reply_to is None:
+            await self._connector._ack_message(self._chan, message)
             raise ValueError('Reply queue not specified in connect request')
+
         hs_to_cli_queue = message.header.properties.reply_to
         connect_id = json_loadb(message.body)
 
         hs_to_srv_queue = await self._connector._queue_declare_and_bind(
             self._chan, exclusive=True
         )
 
@@ -312,18 +489,18 @@
             routing_key=hs_to_cli_queue,
             properties=aiormq.spec.Basic.Properties(
                 message_type=_MessageType.CONNECT_RESPONSE,
                 reply_to=hs_to_srv_queue
             )
         )
 
-        await self._chan.basic_ack(message.delivery_tag)  # type: ignore
+        await self._connector._ack_message(self._chan, message)
 
-        resp_waiter = await MessageWaiter.new(self._chan,
-                                              hs_to_srv_queue, no_ack=True)
+        resp_waiter = await MessageWaiter.new(self._chan, hs_to_srv_queue,
+                                              no_ack=True, timeout=10)
 
         try:
             conn = await RmqConnection._do_handshake_and_create_connection(
                 self._chan,
                 self._connector,
                 self._handshaker,
                 resp_waiter,
@@ -334,15 +511,14 @@
         finally:
             if not self._chan.is_closed:
                 await self._chan.queue_delete(hs_to_srv_queue)
 
         to_cli_queue, to_srv_queue = \
             self._connector._get_transport_queue_names(connect_id)
 
-
         await self._connector._queue_declare_and_bind(
             self._chan, name=to_cli_queue, durable=True
         )
         await self._connector._queue_declare_and_bind(
             self._chan, name=to_srv_queue, durable=True
         )
 
@@ -353,15 +529,18 @@
             properties=aiormq.spec.Basic.Properties(
                 message_type=_MessageType.HS_DONE
             )
         )
 
         # open new to prevent server's chan to be closed by connection
         run_chan = await self._connector._open_channel()
-        conn._set_run_data(run_chan, to_srv_queue, to_cli_queue)
+        policy = \
+            ServerCheckPolicy(conn, self._connector.CONNECTION_CHECK_PERIOD)
+        conn._set_run_data(run_chan, policy, to_srv_queue, to_cli_queue)
+
         self._client_connected_cb(conn)
 
     async def start_serving(self):
         queue_name = self._connector._get_connect_queue_name()
 
         await self._connector._queue_declare_and_bind(
             self._chan, queue_name, durable=True
@@ -389,14 +568,19 @@
 
         Failure to comply with these rules
         leads to unclosed queues growth and message loss.
     """
 
     _TYPE = 'RABBITMQ'
 
+    CONNECTION_CHECK_PERIOD = 20
+    """every X seconds server sends message to client,
+    if client did not got any message in (this period * 1.5),
+    it closes connection"""
+
     __slots__ = ('_url', '_address', '_connect_id',
                  '_exchange', '_exchange_declared')
 
     @property
     def exchange(self):
         return self._exchange
 
@@ -415,15 +599,15 @@
               Format specified at https://www.rabbitmq.com/uri-spec.html.
             address (str): unique identifier for client-server pair.
               If more than one server with same address bound to same exchange,
               behaviour undefined.
             connect_id (str): unique identifier of connecting process.
               Must be set for clients.
         """
-        if not _HAS_AIORMQ:
+        if not _HAVE_AIORMQ:
             raise ImportError('RmqConnector requires aiormq library. '
                               'Install communica with [rabbitmq] extra.')
 
         if connect_id is not None and len(address + connect_id) > 224:
             raise ValueError('Max address + connect_id length is 224 characters')
 
         self._url = URL(url)
@@ -495,14 +679,16 @@
         if message.header.properties.message_type != _MessageType.CONNECT_RESPONSE:
             raise ValueError('Unknown message in connect response queue')
 
         if message.header.properties.reply_to is None:
             raise ValueError('Server queue not specified in connect response')
         hs_to_srv_queue = message.header.properties.reply_to
 
+        resp_waiter.set_timeout_duration(10)
+
         try:
             conn = await RmqConnection._do_handshake_and_create_connection(
                 chan,
                 self,
                 handshaker,
                 resp_waiter,
                 hs_to_srv_queue
@@ -518,15 +704,16 @@
         if message.header.properties.message_type != _MessageType.HS_DONE:
             message_type = message.header.properties.message_type
             raise ValueError(f'Got message with "{message_type}" type '
                               'instead of handshake confirmation')
 
         to_cli_queue, to_srv_queue = \
             self._get_transport_queue_names(self._connect_id)  # type: ignore
-        conn._set_run_data(chan, to_cli_queue, to_srv_queue)
+        policy = ClientCheckPolicy(conn, self.CONNECTION_CHECK_PERIOD * 1.5)
+        conn._set_run_data(chan, policy, to_cli_queue, to_srv_queue)
 
         return conn
 
     async def client_connect(self, handshaker: Handshaker) -> BaseConnection:
         if self._connect_id is None:
             raise TypeError('Cannot connect to server. For those, who connect, '
                             'connect_id parameter must be set. '
@@ -544,15 +731,14 @@
 
             return await self._client_connect(handshaker, chan)
         except Exception:
             if not chan.is_closed:
                 await chan.close()
             raise
 
-
     async def cleanup(self):
         """
         Drop all pending messages and
         delete queues with connector's connect_id
 
         If connect_id is None, noop
         """
@@ -561,16 +747,16 @@
 
         for queue in self._get_transport_queue_names(self._connect_id):
             chan = await self._open_channel()
             try:
                 await chan.queue_purge(queue)
                 await chan.queue_delete(queue)
             except aiormq.exceptions.ChannelNotFoundEntity:
-                # channel will be closed by server if we try to delete unknown queue
-                continue
+                # channel will be closed by server when trying to delete unknown queue
+                await asyncio.wait([chan.closing])
             await chan.close()
 
         await self._check_connection_use()
 
     def dump_state(self) -> str:
         """Unsupported for this connector"""
         raise TypeError('This method unsupported cause user and password '
@@ -578,57 +764,56 @@
 
     @classmethod
     def from_state(cls, state: str) -> Self:
         """Unsupported for this connector"""
         raise TypeError('This method unsupported cause user and password '
                         'are not encrypted in dump, which is insecure')
 
+    async def _ack_message(self, chan, message):
+        await chan.basic_ack(message.delivery_tag)
+
     async def _open_channel(self):
         # there are two limits for simultaneously opened channels:
         # 65k defined by AMQP protocol (channel number range),
         # which cause 'while not (some channel closed)' loop in conn.channel()
         # and 'max-channels' limit set by AMQP server
-        # (RabbitMQ 3.11 default is 2047), which cause connection termination
+        # (RabbitMQ 3.11 default is 2048), which cause connection termination
         # it's unlikely to happen, but i'll keep this in mind ( in comment :D )
 
         if (conn := _connections.get(self._url)) is None:
             fut = asyncio.get_running_loop().create_future()
             _connections[self._url] = fut
             try:
                 conn = await aiormq.connect(self._url)
             except Exception as e:
                 fut.set_exception(e)
                 del(_connections[self._url])
                 raise
             else:
                 fut.set_result(conn)
-                _connections[self._url] = conn  # type: ignore
+                _connections[self._url] = conn
 
         elif isinstance(conn, asyncio.Future):
             conn = await conn
 
         elif conn.is_closed:
             del(_connections[self._url])
             return await self._open_channel()
 
         return await conn.channel()
 
     async def _check_connection_use(self):
-        print('check connection called')
         conn = _connections.get(self._url)
         if conn is None or isinstance(conn, asyncio.Future):
             return
 
         for chan in conn.channels.values():
             if chan is not None and not chan.is_closed:
-                print(repr(chan), chan.is_closed)
                 return
-        print('deleting')
         del(_connections[self._url])
-        print(_connections)
         await conn.close()
 
     async def _queue_declare_and_bind(
             self,
             chan: 'aiormq.abc.AbstractChannel',
             name: str = '',
             **declare_kwargs
```

### Comparing `communica-0.1.4.post1/communica/connectors/stream.py` & `communica-0.2.0/communica/connectors/stream.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import asyncio
 
 from ssl import SSLContext
-from abc import abstractmethod
+from abc import ABC, abstractmethod
 from struct import Struct
-from typing import Optional, Any
+from typing import Sequence, Optional, Any
 
 from typing_extensions import Self
 
 from communica.utils import (
     INT32MAX, NULL_CHAR, ETX_CHAR,
     MessageQueue, logger, json_dumpb, json_loadb
 )
@@ -25,14 +25,60 @@
     'TcpConnector',
     'LocalConnector'
 )
 
 DEFAULT_STREAM_HWM = 32
 
 
+class Frame(ABC):
+    __slots__ = ()
+
+    CODE: bytes
+
+    _frames = {}
+
+    def __init_subclass__(cls) -> None:
+        cls._frames[cls.CODE] = cls
+
+    @abstractmethod
+    def to_bytes(self) -> bytes:
+        raise NotImplementedError
+
+    @classmethod
+    @abstractmethod
+    def _load(cls, data: Sequence[bytes]):
+        raise NotImplementedError
+
+    @classmethod
+    def from_bytes(cls, data: Sequence[bytes]) -> 'Frame':
+        try:
+            frame = cls._frames[data[0]]
+        except ValueError:
+            raise ValueError('Unknown protocol') from None
+
+        return frame._load(data[1:])
+
+
+class MessageFrame(Frame):
+    CODE = b'\x01'
+
+    _header_packer = Struct(
+        '!I'  # message length
+         'H'  # data start index
+    )
+    _pack_header = _header_packer.pack
+    _header_size = _header_packer.size
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def to_bytes(self) -> bytes:
+        return self.CODE + b''
+
+
 class StreamConnection(BaseConnection):
     __slots__ = ('reader', 'writer', 'connector', '_send_queue')
 
     reader: asyncio.StreamReader
     writer: asyncio.StreamWriter
     connector: 'BaseStreamConnector'
 
@@ -92,28 +138,27 @@
     async def _run_connection(self, request_received_cb: RequestReceivedCB):
         is_closing = self.writer.is_closing
         readexactly = self.reader.readexactly
         header_size = self._header_packer.size
         header_unpack = self._header_packer.unpack
 
         write_task = asyncio.create_task(self._send_runner())
-
         try:
             while not is_closing():
                 header = await readexactly(header_size)
                 chunk_len, data_start = header_unpack(header)
-                chunk = await readexactly(chunk_len)
+                chunk = memoryview(await readexactly(chunk_len))
 
-                # XXX: попробовать с memoryview
                 request_received_cb(json_loadb(chunk[:data_start]), chunk[data_start:])
         except Exception as e:
-            logger.debug(f'Connection broken: {e!r}')
+            logger.debug('Connection broken: %r', e)
             raise
         finally:
             write_task.cancel()
+            await asyncio.wait([write_task])
 
         return None
 
     async def _send_runner(self):
         header_pack = self._header_packer.pack
 
         while True:
@@ -197,18 +242,14 @@
 
 class TcpConnector(BaseStreamConnector):
     _TYPE = 'TcpConnector'
 
     __slots__ = ('host', 'port', 'ssl')
 
     def __init__(self, host: str, port: int, ssl: Optional[SSLContext] = None):
-        import warnings
-        warnings.warn(
-            'This connector unstable and may lead to message loss'
-        )
         self.host = host
         self.port = port
         self.ssl = ssl
 
     def repr_address(self) -> str:
         return f'{self.host}:{self.port}'
```

### Comparing `communica-0.1.4.post1/communica/pairs/base.py` & `communica-0.2.0/communica/pairs/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,42 +6,50 @@
 from typing_extensions import Self
 
 from communica.utils import HasLoopMixin, logger
 from communica.connectors.base import BaseConnector
 
 
 class BaseEntity(ABC, HasLoopMixin):
-    __slots__ = ('connector', '_stop_event')
+    __slots__ = ('connector', '_closed', '_stop_event')
 
     connector: BaseConnector
 
     def __init__(self, connector: BaseConnector) -> None:
         self.connector = connector
 
     def __repr__(self) -> str:
         return f'{type(self).__name__}()'
 
     async def run(self):
         """Run until .stop() is called."""
         if hasattr(self, '_stop_event'):
-            RuntimeError('.run() must be called only once on same object')
+            raise RuntimeError('.run() must be called only once on same object')
 
+        self._closed = asyncio.get_event_loop().create_future()
         self._stop_event = asyncio.Event()
         try:
             async with self:
                 print(f'Running {self!r} on {self.connector.repr_address()}')
                 await self._stop_event.wait()
         finally:
             del(self._stop_event)
+            self._closed.set_result(None)
 
     def stop(self):
         """If .run() was called, it returns, otherwise this method does nothing"""
         if hasattr(self, '_stop_event'):
             self._stop_event.set()
 
+    async def wait_stop(self):
+        """Call .stop() and wait until closed"""
+        if hasattr(self, '_stop_event'):
+            self.stop()
+            await self._closed
+
     @abstractmethod
     async def init(self) -> Self:
         raise NotImplementedError
 
     @abstractmethod
     async def close(self) -> None:
         raise NotImplementedError
```

### Comparing `communica-0.1.4.post1/communica/pairs/route.py` & `communica-0.2.0/communica/pairs/route.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import asyncio
 
 from uuid import uuid4
-from typing import (
-    Callable, Protocol, TypedDict, Any, cast
-)
+from typing import TypedDict, Any, cast
 
-from communica.exceptions import RequesterError, ResponderError
+from communica.exceptions import ReqError, RespError, SerializerError
 from communica.serializers import BaseSerializer, default_serializer
 from communica.connectors.base import (
     BaseConnection, BaseConnector,
     HandshakeOk, HandshakeFail, HandshakeGen
 )
-from communica.utils import logger
+from communica.utils import TaskSet, logger
 
 
 from communica.pairs.base import SyncHandlerType, AsyncHandlerType
 from communica.pairs.simple import (
     ReqRepClient, ReqRepServer,
     RequestType, RequestHandler,
     ReqRepMessageFlow, ServerHandshakeOk
@@ -34,22 +32,22 @@
     route: str
 
 
 class RouteMessageFlow(ReqRepMessageFlow):
     __slots__ = ('routes', 'fallback_task_set', '_response_serializers',)
 
     routes: 'dict[str, tuple[RequestHandler, BaseSerializer]]'
-    fallback_task_set: 'set[asyncio.Task]'
+    fallback_task_set: TaskSet
 
     _response_serializers: 'dict[str, BaseSerializer]'
 
     def __init__(self):
         super().__init__()
         self.routes = {}
-        self.fallback_task_set = set()
+        self.fallback_task_set = TaskSet()
         self._response_serializers = {}
 
     def update_route(
             self,
             route: str,
             handler: 'SyncHandlerType | AsyncHandlerType',
             serializer: 'BaseSerializer | None'
@@ -63,23 +61,22 @@
             try:
                 route_handle = self.routes[metadata['route']]
                 task_set = route_handle[0].running_tasks
             except KeyError:
                 route_handle = None
                 task_set = self.fallback_task_set
 
-            runner_task = self._get_loop().create_task(
-                self.handle_request(route_handle, metadata, raw_data))
-            runner_task.add_done_callback(task_set.discard)
-            task_set.add(runner_task)
+            task_set.create_task_with_exc_log(
+                self.handle_request(route_handle, metadata, raw_data)
+            )
         else:
             try:
                 serializer = self._response_serializers[metadata['route']]
-            except KeyError:
-                # this is possible, for example, after program restart.
+            except KeyError:  # pragma: no cover
+                # this is possible after program restart.
                 # just log and skip, cause we don't have a routine,
                 # waiting for this response
                 logger.warning('Got response with not requested '
                               f'route ({metadata["route"]})')
                 return
             self._handle_response(serializer, metadata, raw_data)
 
@@ -88,47 +85,39 @@
             route_handle: 'tuple[RequestHandler, BaseSerializer] | None',
             req_meta: Metadata,
             raw_data: bytes
         ):
         if route_handle is not None:
             handler, serializer = route_handle
             resp_meta, resp_data = await self._handle_request(
-                handler, req_meta, serializer.load(raw_data)
+                handler, serializer, req_meta, raw_data
             )
         else:
+            serializer = default_serializer
             resp_meta = req_meta.copy()
-            resp_data = {'msg': f'Route "{req_meta["route"]}" not exists'}
             resp_meta['type'] = RequestType.RESP_ERR_REQUESTER
+            resp_data = \
+                ReqError(f'Route "{req_meta["route"]}" not exists').to_dict()
 
-        req_type = req_meta['type']
-        resp_type = resp_meta['type']
-
-        if resp_type == RequestType.RESP_OK:
-            if req_type == RequestType.REQ_REP:
-                await self._connection.send(
-                    resp_meta, serializer.dump(resp_data))  # pyright: reportUnboundVariable=false
-
-        elif req_type == RequestType.REQ_THROW:
-            logger.warning('Error occured while handling request, but '
-                           'requester don\'t know about this:\n' + resp_data['msg'])
+        await self._send_response(req_meta, resp_meta, resp_data, serializer)
 
     async def request(
             self,
             route: str,
             serializer: 'BaseSerializer | None',
             data: Any
     ) -> bytes:
-        request_id, fut = self.create_response_waiter()
+        request_id, fut = self._create_response_waiter()
 
         serializer = serializer or default_serializer
         if (saved_serializer := self._response_serializers.get(route)) is None:
             self._response_serializers[route] = serializer
-        elif saved_serializer != serializer:
-            raise TypeError('You should always use the same serializer for the '
-                           f'same route ({saved_serializer!r} '
+        elif saved_serializer is not serializer:
+            raise TypeError('You should always use the same serializer for '
+                           f'the same route ({saved_serializer!r} '
                             'has already been used earlier)')
 
         await self._connection.send(
             Metadata(id=request_id, type=RequestType.REQ_REP, route=route),
             serializer.dump(data)
         )
 
@@ -147,27 +136,26 @@
 
 
 class RouteClient(ReqRepClient):
     """
     Pair for RouteServer.
     """
 
-    __slots__ = ('_routes',)
+    __slots__ = ()
 
     _flow: RouteMessageFlow
 
     def __init__(
             self,
             connector: BaseConnector,
             client_id: 'str | None' = None
     ) -> None:
         super().__init__(connector)
 
         self._flow = RouteMessageFlow()
-        self._routes = []
 
         self._run_task = None
         self._client_id = client_id or uuid4().hex
 
     def route_handler(
             self,
             route: str,
@@ -178,15 +166,14 @@
 
         Args:
             route: Handler identifier.
             serializer: Defaults to JsonSerializer.
         """
         def decorator(endpoint: 'SyncHandlerType | AsyncHandlerType'):
             self._flow.update_route(route, endpoint, serializer)
-            self._routes.append((route, endpoint, serializer))
 
         return decorator
 
     async def request(
             self,
             route: str,
             data: Any,
@@ -252,21 +239,18 @@
                 if isinstance(flow, RouteMessageFlow):
                     flow.update_route(route, endpoint, serializer)
             self._routes.append((route, endpoint, serializer))
 
         return decorator
 
     def _cancel_handler_tasks(self, flow: RouteMessageFlow):
-        for task in flow.fallback_task_set:
-            task.cancel()
+        flow.fallback_task_set.cancel()
 
         for handler, _ in flow.routes.values():
-            for task in handler.running_tasks:
-                if task is not asyncio.tasks.current_task():
-                    task.cancel()
+            handler.running_tasks.cancel()
 
     def _on_client_connect(self, connection: BaseConnection):
         loop = self._get_loop()
         handshake_result = cast(ServerHandshakeOk, connection.get_handshake_result())
         client_id = handshake_result.client_id
 
         flow = self._known_clients.get(client_id)
```

### Comparing `communica-0.1.4.post1/communica/pairs/simple.py` & `communica-0.2.0/communica/pairs/simple.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,25 +5,24 @@
 from enum import Enum
 from uuid import uuid4, uuid1
 from typing import TypedDict, Any, cast
 from inspect import iscoroutinefunction
 from traceback import format_exc
 from dataclasses import dataclass
 
-from communica.exceptions import RequesterError, ResponderError
 from communica.serializers import BaseSerializer, default_serializer
+from communica.exceptions import (
+    ReqError, RespError, UnknownError, SerializerError
+)
 from communica.connectors.base import (
     BaseConnection, BaseConnector,
     HandshakeOk, HandshakeGen
 )
 from communica.utils import (
-    cycle_range, json_dumpb, iscallable,
-    HasLoopMixin,
-    INT32RANGE,
-    logger
+    HasLoopMixin, TaskSet, iscallable, logger
 )
 
 from communica.pairs.base import (
     BaseClient, BaseServer,
     SyncHandlerType, AsyncHandlerType
 )
 
@@ -36,17 +35,20 @@
 
 class RequestType(int, Enum):
     REQ_REP = 1
     REQ_THROW = 2
 
     RESP_OK = 11
 
-    RESP_ERR_REQUESTER = 31
-    RESP_ERR_RESPONDER = 41
-    RESP_ERR_UNKNOWN = 42
+    RESP_ERR_UNKNOWN = 30
+
+    RESP_ERR_REQUESTER = 41
+    RESP_ERR_DATA_LOAD = 42
+
+    RESP_ERR_RESPONDER = 51
 
 
 @dataclass
 class ServerHandshakeOk(HandshakeOk):
     client_id: str
 
 
@@ -56,44 +58,43 @@
 
 
 class RequestHandler:
     __slots__ = ('is_async', 'endpoint', 'running_tasks')
 
     is_async: bool
     endpoint: 'SyncHandlerType | AsyncHandlerType'
-    running_tasks: 'set[asyncio.Task]'
+    running_tasks: TaskSet
 
     def __init__(self, endpoint: 'SyncHandlerType | AsyncHandlerType') -> None:
         if not iscallable(endpoint):
             raise TypeError('Request handler must be function, '
                             'coroutine function or method')
         self.is_async = iscoroutinefunction(endpoint)
         self.endpoint = endpoint
-        self.running_tasks = set()
+        self.running_tasks = TaskSet()
 
 
 class ReqRepMessageFlow(HasLoopMixin):
     __slots__ = (
-        '_connection', '_id_counter', '_response_waiters'
+        '_connection', '_response_waiters'
     )
 
     _response_waiters: 'dict[str, asyncio.Future]'
 
     def __init__(self):
-        self._id_counter = cycle_range(*INT32RANGE)
         self._response_waiters = {}
 
     def update_connection(self, connection: BaseConnection):
         try:
             self._connection.update(connection)
         except AttributeError:
             self._connection = connection
         return self._connection
 
-    def create_response_waiter(self):
+    def _create_response_waiter(self):
         request_id = uuid1().hex
 
         fut = self._get_loop().create_future()
         self._response_waiters[request_id] = fut
         fut.add_done_callback(lambda _: self._response_waiters.pop(request_id, None))
 
         return request_id, fut
@@ -119,49 +120,92 @@
                 # requester's error, cause responder can't do
                 # anything about it after sending response
                 fut.set_exception(e)
             return
 
         data = default_serializer.load(raw_data)
         if req_type == RequestType.RESP_ERR_REQUESTER:
-            fut.set_exception(RequesterError(data['msg']))
+            fut.set_exception(ReqError.from_dict(data))
         elif req_type == RequestType.RESP_ERR_RESPONDER:
-            fut.set_exception(ResponderError(data['msg']))
+            fut.set_exception(RespError.from_dict(data))
         elif req_type == RequestType.RESP_ERR_UNKNOWN:
-            fut.set_exception(ResponderError(data['msg']))  # XXX (че по исключению)
+            fut.set_exception(UnknownError.from_dict(data))
+        elif req_type == RequestType.RESP_ERR_DATA_LOAD:
+            fut.set_exception(SerializerError.from_dict(data))
         else:
-            logger.critical(f"{metadata['type'] = }, чзх")
-            fut.set_exception(Exception('каво нахуй'))
+            logger.critical(f"{metadata = }, wtf")
+            fut.set_exception(
+                UnknownError(f'Got unknown response type: {metadata["type"]}')
+            )
 
     async def _handle_request(
             self,
             handler: RequestHandler,
+            serializer: BaseSerializer,
             metadata: Metadata,
-            data: Any
+            raw_data: Any
     ) -> 'tuple[dict, Any]':
         resp_meta = metadata.copy()
 
         try:
+            data = serializer.load(raw_data)
+            print(data)
+        except Exception as e:
+            resp_meta['type'] = RequestType.RESP_ERR_DATA_LOAD
+            resp_data = SerializerError(repr(e)).to_dict()
+            return resp_meta, resp_data  # type: ignore
+
+        try:
             if handler.is_async:
                 resp_data = await handler.endpoint(data)
             else:
                 resp_data = handler.endpoint(data)
             resp_meta['type'] = RequestType.RESP_OK
-        except RequesterError as e:
-            resp_data = {'msg': e.message}
+
+        except ReqError as e:
+            resp_data = e.to_dict()
             resp_meta['type'] = RequestType.RESP_ERR_REQUESTER
-        except ResponderError as e:
-            resp_data = {'msg': e.message}
+
+        except RespError as e:
+            resp_data = e.to_dict()
             resp_meta['type'] = RequestType.RESP_ERR_RESPONDER
+
         except Exception as e:
-            resp_data = {'msg': f'fuck you, there is {e!r}'}
+            resp_data = UnknownError(repr(e)).to_dict()
             resp_meta['type'] = RequestType.RESP_ERR_UNKNOWN
 
         return resp_meta, resp_data  # type: ignore
 
+    async def _send_response(
+            self,
+            req_meta,
+            resp_meta,
+            resp_data,
+            serializer: BaseSerializer
+    ):
+        if req_meta['type'] == RequestType.REQ_REP:
+            if resp_meta['type'] > RequestType.RESP_OK:
+                serializer = default_serializer
+
+            try:
+                raw_data = serializer.dump(resp_data)
+            except Exception:
+                logger.error('Can\'t serialize response:\n%s', format_exc())
+
+                raw_data = default_serializer.dump(
+                    RespError('Response serialize error').to_dict()
+                )
+                resp_meta['type'] = RequestType.RESP_ERR_RESPONDER
+
+            await self._connection.send(resp_meta, raw_data)
+
+        elif resp_meta['type'] > RequestType.RESP_ERR_UNKNOWN:
+            logger.warning('Error occured while handling request, but '
+                           'requester don\'t know about this:\n' + resp_data['msg'])
+
 
 class SimpleMessageFlow(ReqRepMessageFlow):
     __slots__ = ('handler', 'serializer')
 
     def __init__(
             self,
             handler: 'SyncHandlerType | AsyncHandlerType',
@@ -169,41 +213,30 @@
     ):
         super().__init__()
         self.handler = RequestHandler(handler)
         self.serializer = serializer
 
     def dispatch(self, metadata: Metadata, raw_data: bytes):
         if metadata['type'] < RequestType.RESP_OK:
-            data = self.serializer.load(raw_data)
-            runner_task = self._get_loop().create_task(
-                self.handle_request(metadata, data))
-            runner_task.add_done_callback(self.handler.running_tasks.discard)
-            self.handler.running_tasks.add(runner_task)
+            self.handler.running_tasks.create_task_with_exc_log(
+                self.handle_request(metadata, raw_data)
+            )
         else:
             self._handle_response(self.serializer, metadata, raw_data)
 
-    async def handle_request(self, req_meta: Metadata, data: Any):
+    async def handle_request(self, req_meta: Metadata, raw_data: bytes):
         resp_meta, resp_data = await self._handle_request(
-            self.handler, req_meta, data
+            self.handler, self.serializer, req_meta, raw_data
+        )
+        await self._send_response(
+            req_meta, resp_meta, resp_data, self.serializer
         )
-
-        req_type = req_meta['type']
-        resp_type = resp_meta['type']
-
-        if resp_type == RequestType.RESP_OK:
-            if req_type == RequestType.REQ_REP:
-                await self._connection.send(
-                    resp_meta, self.serializer.dump(resp_data))
-
-        elif req_type == RequestType.REQ_THROW:
-            logger.warning('Error occured while handling request, but '
-                           'requester don\'t know about this:\n' + format_exc())
 
     async def request(self, data: Any) -> bytes:
-        request_id, fut = self.create_response_waiter()
+        request_id, fut = self._create_response_waiter()
 
         await self._connection.send(
             Metadata(id=request_id, type=RequestType.REQ_REP),
             self.serializer.dump(data)
         )
 
         return await fut
@@ -249,15 +282,14 @@
             raise
         return self
 
     async def close(self) -> None:
         if self._run_task is not None:
             await self._flow._connection.close()
             self._run_task.cancel()
-        self.stop()
 
     async def _connection_keeper(self):
         while True:
             try:
                 new_conn = await self.connector.client_connect(self._handshaker)
             except Exception as e:
                 logger.warning('Connect failed: %s', repr(e))
@@ -276,22 +308,22 @@
             await asyncio.sleep(1)
 
     async def _handshaker(self, connection: BaseConnection) -> HandshakeGen:
         client_hello = {
             'client_id': self._client_id
         }
 
-        server_hello = json.loads((yield json_dumpb(client_hello)))
+        server_hello = (yield client_hello)
 
         yield HandshakeOk()
 
 
 class SimpleClient(ReqRepClient):
     """
-    Работает в паре с SimpleServer.
+    Pair to SimpleServer.
 
     Has only one optional request handler.
     """
 
     __slots__ = ('serializer',)
 
     serializer: BaseSerializer
@@ -313,15 +345,15 @@
 
         self._flow = SimpleMessageFlow(handler, serializer)
 
         self._client_id = client_id or uuid4().hex
         self._run_task = None
 
     def _not_defined_handler(self, data: Any):
-        raise ResponderError('Client side not defined handler for server requests')
+        raise RespError('Client side not defined handler for server requests')
 
     async def request(self, data: Any) -> bytes:
         """Send request, wait response."""
         return await self._flow.request(data)
 
     async def throw(self, data: Any) -> None:
         """Send request without waiting response."""
@@ -332,46 +364,46 @@
     __slots__ = ('_server', '_known_clients', '_client_conn_runners')
 
     _server: asyncio.AbstractServer
     _known_clients: 'dict[str, ReqRepMessageFlow | asyncio.Future[ReqRepMessageFlow]]'
     _client_conn_runners: 'dict[str, asyncio.Task]'
 
     async def init(self):
-        self._server = await self.connector.server_start(
-            self._handshaker, self._on_client_connect)
+        if not hasattr(self, '_server') or not self._server.is_serving():
+            self._server = await self.connector.server_start(
+                self._handshaker, self._on_client_connect)
         return self
 
     async def close(self) -> None:
+        self._server.close()
+        await self._server.wait_closed()
+
         for client_id, flow in self._known_clients.items():
             if isinstance(flow, ReqRepMessageFlow):
                 self._cancel_handler_tasks(flow)
                 await flow._connection.close()
-            # XXX: проблемы с RMQ коннектором: отмена conn.close()
-            # вызывает повторную отправку Close фрейма, что ломает соединение
             if (conn_task := self._client_conn_runners.get(client_id)):
                 conn_task.cancel()
-        self._server.close()
-        await self._server.wait_closed()
 
     async def _handshaker(self, connection: BaseConnection) -> HandshakeGen:
         server_hello = {
             'hello': 'hello'
         }
 
-        client_hello = json.loads((yield json_dumpb(server_hello)))
+        client_hello = (yield server_hello)
 
         client_id = client_hello['client_id']
         yield ServerHandshakeOk(client_id=client_id)
 
     async def _get_client_flow(self, client_id: 'str | None') -> Any:
         if client_id is None:
             while not self._known_clients:
                 await asyncio.sleep(1)
 
-            import random
+            import random  # XXX
 
             flow = random.choice(list(self._known_clients.values()))
             if isinstance(flow, ReqRepMessageFlow):
                 return flow
             return await flow
 
         flow = self._known_clients.get(client_id)
@@ -394,15 +426,15 @@
     @abstractmethod
     def _on_client_connect(self, connection: BaseConnection):
         raise NotImplementedError
 
 
 class SimpleServer(ReqRepServer):
     """
-    Работает в паре с SimpleClient.
+    Pair to SimpleClient.
 
     Has only one request handler.
     """
 
     __slots__ = ('_handler', '_serializer')
 
     _handler: 'SyncHandlerType | AsyncHandlerType'
@@ -420,17 +452,15 @@
         self._handler = handler
         self.connector = connector
         self._serializer = serializer
         self._known_clients = {}
         self._client_conn_runners = {}
 
     def _cancel_handler_tasks(self, flow: SimpleMessageFlow):
-        for task in flow.handler.running_tasks:
-            if task is not asyncio.tasks.current_task():
-                task.cancel()
+        flow.handler.running_tasks.cancel()
 
     def _on_client_connect(self, connection: BaseConnection):
         loop = self._get_loop()
         handshake_result = cast(ServerHandshakeOk, connection.get_handshake_result())
         client_id = handshake_result.client_id
 
         flow = self._known_clients.get(client_id)
@@ -447,21 +477,21 @@
         self._client_conn_runners[client_id] = task
 
     async def request(self, data: Any, client_id: 'str | None' = None) -> bytes:
         """
         Send request, wait response.
 
         Args:
-            client_id: If omitted or None, random client will be chosen
+            client_id: If omitted or None, random connected client will be chosen
         """
         flow = await self._get_client_flow(client_id)
         return await flow.request(data)
 
     async def throw(self, data: Any, client_id: 'str | None' = None) -> None:
         """
         Send request without waiting response.
 
         Args:
-            client_id: If omitted or None, random client will be chosen
+            client_id: If omitted or None, random connected client will be chosen
         """
         flow = await self._get_client_flow(client_id)
         return await flow.throw(data)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `communica-0.1.4.post1/communica/serializers/base.py` & `communica-0.2.0/communica/serializers/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.1.4.post1/communica.egg-info/PKG-INFO` & `communica-0.2.0/communica.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: communica
-Version: 0.1.4.post1
+Version: 0.2.0
 Summary: Easy to use IPC library
 Author-email: Elchin Sarkarov <elchin751@gmail.com>
 Project-URL: Homepage, https://github.com/elchinchel/communica-py
 Project-URL: Bug Tracker, https://github.com/elchinchel/communica-py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
 Provides-Extra: df
 Provides-Extra: orjson
+Provides-Extra: adaptix
 Provides-Extra: pydantic
 Provides-Extra: rabbitmq
 License-File: LICENSE.txt
 
 # Easy to use IPC library
 
     This library is still in development process.
```

### Comparing `communica-0.1.4.post1/pyproject.toml` & `communica-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "communica"
-version = "0.1.4.post1"
+version = "0.2.0"
 authors = [
   { name="Elchin Sarkarov", email="elchin751@gmail.com" },
 ]
 description = "Easy to use IPC library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -13,16 +13,19 @@
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: POSIX",
   "Operating System :: Microsoft :: Windows",
 ]
 dependencies = ["typing-extensions"]
 
 [project.optional-dependencies]
+test = [ "pytest", "pytest-cov", "pytest-asyncio" ]
+
 df = ["dataclass-factory"]
 orjson = ["orjson"]
+adaptix = ["adaptix"]
 pydantic = ["pydantic"]
 rabbitmq = ["aiormq", "yarl"]
 
 [project.urls]
 "Homepage" = "https://github.com/elchinchel/communica-py"
 "Bug Tracker" = "https://github.com/elchinchel/communica-py/issues"
```

