# Comparing `tmp/pyxk-0.5.2.tar.gz` & `tmp/pyxk-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxk-0.5.2.tar", last modified: Mon Apr 10 03:09:59 2023, max compression
+gzip compressed data, was "pyxk-0.5.3.tar", last modified: Tue May  9 07:19:15 2023, max compression
```

## Comparing `pyxk-0.5.2.tar` & `pyxk-0.5.3.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 03:09:59.266989 pyxk-0.5.2/
--rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.5.2/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)      343 2023-04-10 03:09:59.266989 pyxk-0.5.2/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.5.2/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 03:09:59.266989 pyxk-0.5.2/pyxk/
--rw-rw----   0 root         (0) everybody  (9997)      726 2023-04-10 02:29:14.000000 pyxk-0.5.2/pyxk/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    15453 2023-04-10 03:02:22.000000 pyxk-0.5.2/pyxk/aclient.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 03:09:59.266989 pyxk-0.5.2/pyxk/aes/
--rw-rw----   0 root         (0) everybody  (9997)       79 2023-02-24 04:10:40.000000 pyxk-0.5.2/pyxk/aes/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3639 2023-04-06 15:25:24.000000 pyxk-0.5.2/pyxk/aes/_fmtdata.py
--rw-rw----   0 root         (0) everybody  (9997)     4701 2023-04-06 15:27:39.000000 pyxk-0.5.2/pyxk/aes/cryptor.py
--rw-rw----   0 root         (0) everybody  (9997)      954 2023-04-09 12:40:57.000000 pyxk-0.5.2/pyxk/lazy_loader.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 03:09:59.266989 pyxk-0.5.2/pyxk/m3u8/
--rw-rw----   0 root         (0) everybody  (9997)       82 2023-03-16 14:08:36.000000 pyxk-0.5.2/pyxk/m3u8/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     8292 2023-03-16 12:13:38.000000 pyxk-0.5.2/pyxk/m3u8/_download.py
--rw-rw----   0 root         (0) everybody  (9997)     3199 2023-03-16 16:35:49.000000 pyxk-0.5.2/pyxk/m3u8/_entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)     7791 2023-03-16 16:35:32.000000 pyxk-0.5.2/pyxk/m3u8/_m3u8.py
--rw-rw----   0 root         (0) everybody  (9997)     4504 2023-03-17 04:00:18.000000 pyxk-0.5.2/pyxk/m3u8/_parser.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 03:09:59.266989 pyxk-0.5.2/pyxk/requests/
--rw-rw----   0 root         (0) everybody  (9997)      235 2023-04-06 15:53:39.000000 pyxk-0.5.2/pyxk/requests/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     5598 2023-04-06 16:07:00.000000 pyxk-0.5.2/pyxk/requests/_entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)     7514 2023-03-31 10:17:41.000000 pyxk-0.5.2/pyxk/requests/api.py
--rw-rw----   0 root         (0) everybody  (9997)    21859 2023-04-06 15:20:21.000000 pyxk-0.5.2/pyxk/requests/sessions.py
--rw-rw----   0 root         (0) everybody  (9997)    12202 2023-04-09 12:40:57.000000 pyxk-0.5.2/pyxk/utils.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 03:09:59.266989 pyxk-0.5.2/pyxk.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      343 2023-04-10 03:09:59.000000 pyxk-0.5.2/pyxk.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      539 2023-04-10 03:09:59.000000 pyxk-0.5.2/pyxk.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-10 03:09:59.000000 pyxk-0.5.2/pyxk.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       91 2023-04-10 03:09:59.000000 pyxk-0.5.2/pyxk.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       55 2023-04-10 03:09:59.000000 pyxk-0.5.2/pyxk.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-04-10 03:09:59.000000 pyxk-0.5.2/pyxk.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-10 03:09:59.266989 pyxk-0.5.2/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      917 2023-04-10 03:09:51.000000 pyxk-0.5.2/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 07:19:15.593999 pyxk-0.5.3/
+-rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.5.3/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-09 07:19:15.593999 pyxk-0.5.3/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.5.3/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 07:19:15.583999 pyxk-0.5.3/pyxk/
+-rw-rw----   0 root         (0) everybody  (9997)       53 2023-05-08 09:38:07.000000 pyxk-0.5.3/pyxk/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 07:19:15.593999 pyxk-0.5.3/pyxk/aclient/
+-rw-rw----   0 root         (0) everybody  (9997)       90 2023-05-08 07:54:13.000000 pyxk-0.5.3/pyxk/aclient/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    15036 2023-05-09 03:25:00.000000 pyxk-0.5.3/pyxk/aclient/client.py
+-rw-rw----   0 root         (0) everybody  (9997)      699 2023-04-30 15:43:19.000000 pyxk-0.5.3/pyxk/aclient/typedef.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 07:19:15.593999 pyxk-0.5.3/pyxk/aes/
+-rw-rw----   0 root         (0) everybody  (9997)       79 2023-04-10 03:10:37.000000 pyxk-0.5.3/pyxk/aes/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3633 2023-05-08 07:57:14.000000 pyxk-0.5.3/pyxk/aes/_fmtdata.py
+-rw-rw----   0 root         (0) everybody  (9997)     4695 2023-05-08 07:56:51.000000 pyxk-0.5.3/pyxk/aes/cryptor.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 07:19:15.593999 pyxk-0.5.3/pyxk/m3u8downloader/
+-rw-rw----   0 root         (0) everybody  (9997)       66 2023-05-08 07:55:15.000000 pyxk-0.5.3/pyxk/m3u8downloader/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     2300 2023-05-09 07:15:49.000000 pyxk-0.5.3/pyxk/m3u8downloader/enter_point.py
+-rw-rw----   0 root         (0) everybody  (9997)     4821 2023-05-08 07:56:03.000000 pyxk-0.5.3/pyxk/m3u8downloader/m3u8download.py
+-rw-rw----   0 root         (0) everybody  (9997)     2968 2023-05-08 04:33:43.000000 pyxk-0.5.3/pyxk/m3u8downloader/m3u8parse.py
+-rw-rw----   0 root         (0) everybody  (9997)    10817 2023-05-09 07:07:43.000000 pyxk-0.5.3/pyxk/m3u8downloader/main.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 07:19:15.593999 pyxk-0.5.3/pyxk/requests/
+-rw-rw----   0 root         (0) everybody  (9997)      247 2023-05-08 07:57:36.000000 pyxk-0.5.3/pyxk/requests/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     7480 2023-05-08 07:58:19.000000 pyxk-0.5.3/pyxk/requests/api.py
+-rw-rw----   0 root         (0) everybody  (9997)     3309 2023-05-09 03:19:15.000000 pyxk-0.5.3/pyxk/requests/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    14682 2023-05-09 03:23:24.000000 pyxk-0.5.3/pyxk/requests/sessions.py
+-rw-rw----   0 root         (0) everybody  (9997)    18965 2023-05-08 09:56:53.000000 pyxk-0.5.3/pyxk/utils.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 07:19:15.593999 pyxk-0.5.3/pyxk.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-09 07:19:15.000000 pyxk-0.5.3/pyxk.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      627 2023-05-09 07:19:15.000000 pyxk-0.5.3/pyxk.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-09 07:19:15.000000 pyxk-0.5.3/pyxk.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       99 2023-05-09 07:19:15.000000 pyxk-0.5.3/pyxk.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       55 2023-05-09 07:19:15.000000 pyxk-0.5.3/pyxk.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-05-09 07:19:15.000000 pyxk-0.5.3/pyxk.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-09 07:19:15.593999 pyxk-0.5.3/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      927 2023-05-09 07:18:11.000000 pyxk-0.5.3/setup.py
```

### Comparing `pyxk-0.5.2/LICENSE` & `pyxk-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.2/pyxk/aclient.py` & `pyxk-0.5.3/pyxk/aclient/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,451 +1,470 @@
-import re
-import sys
-import types
-import typing
 import asyncio
+import warnings
+from typing import (
+    Any,
+    List,
+    Tuple,
+    Union,
+    Optional,
+    Mapping,
+    Pattern
+)
+from types import MethodType
 from itertools import zip_longest
 from multidict import CIMultiDict
-from asyncio import AbstractEventLoop as EventLoop
 
+import aiohttp
 from yarl import URL
-from lxml import etree
-from aiohttp import (
-    ClientTimeout,
-    TCPConnector,
-    ClientSession as Session
+from aiohttp import client_exceptions as aiohttp_client_exceptions
+try:
+    import chardet as _chardet
+except ImportError:
+    import charset_normalizer as _chardet
+from parsel.selector import Selector, LXML_SUPPORTS_HUGE_TREE
+
+from pyxk.aclient.typedef import (
+    StrOrURL,
+    Session,
+    Response,
+    EventLoop,
+    CIMDict,
+    Timeout,
+    ResponseSelector,
+    RequestCallback
 )
-import aiohttp.client_exceptions
-import rich.live as rich_live
-import rich.console as rich_console
-import rich.progress as rich_progress
-from aiohttp.client_reqrep import ClientResponse as Response
-
 from pyxk.utils import get_user_agent
-from pyxk.lazy_loader import LazyLoader
 
-rich_box = LazyLoader("rich_box", globals(), "rich.box")
-rich_panel = LazyLoader("rich_panel", globals(), "rich.panel")
-rich_table = LazyLoader("rich_table", globals(), "rich.table")
 
 
+__all__ = ["chardet", "Client"]
+
+def chardet(byte: bytes):
+    """字符编码判断"""
+    return _chardet.detect(byte)
 
-class AsyncSession:
 
+class Client:
+    """
+    异步下载器 - 类变量
+
+    :params: limit : 并发数量
+    :params: timeout : 请求超时时间
+    :params: headers : 请求头
+    :params: verify_ssl : ssl验证
+    :params: start_urls : 请求入口urls
+    :params: user_agnet : User-Agent
+    :params: aiohttp_kwargs : aiohttp.ClientSession 实例化参数
+    :params: retry_status_code : 请求状态码，包含在列表中的进行重新发送
+    :params: error_status_code: 请求状态码，包含在列表中直接抛出错误
+
+    __init__ parameters - 实例化参数
+
+    :params: loop : asyncio event loop
+    :params: session : aiohttp client_session
+    :params: base_url : base_url
+    """
     limit: int = 16
-    timeout: typing.Union[int, float, dict] = {
-        "total": 8,
-        "connect": None,
-        "sock_read": None,
-        "sock_connect": None
-    }
-    headers: typing.Union[dict, CIMultiDict] = {}
-    start_urls: list = []
-    user_agent: str = get_user_agent("android")
-    aiohttp_kwargs: dict = {}
+    timeout: Timeout = 7
+    headers: Optional[Union[dict, CIMDict]] = None
+    verify_ssl: bool = True
+    start_urls: Union[List[str], List[Tuple[str, dict]]] = []
+    user_agent: str = get_user_agent("windows")
+    aiohttp_kwargs: Optional[dict] = None
+    retry_status_code: Optional[list] = None
+    error_status_code: Optional[list] = None
 
     def __init__(
         self,
         *,
         loop: EventLoop=None,
-        session: Session=None
-    ):
-        self._loop: EventLoop = loop
-        self._session: Session = session
-
-    async def start(self):
-        """运行开始之前调用"""
-
-    async def stop(self):
-        """运行完成之后调用"""
+        session: Session=None,
+        base_url: StrOrURL=None,
+    ) -> None:
+        self._loop = loop
+        self._session = session
+        self._base_url = self.set_base_url(base_url)
 
     @classmethod
-    def run(cls, **kwargs) -> typing.Union[object, list]:
-        """类方法: 协程入口 run, 应该从这里开始
+    def run(cls, **kwargs):
+        """
+        异步下载器 运行入口 - 应该从此方法运行
 
-        Return: ClientSession, [..., ...]
-        返回值: 当前类的实例化, 协程运行结果列表
+        :params: **kwargs : 实例化参数
         """
-        # Event loop
-        if not isinstance(kwargs.get("loop", None), EventLoop):
+        if not kwargs.__contains__("loop"):
             loop = asyncio.new_event_loop()
             asyncio.set_event_loop(loop)
-            kwargs["loop"] = loop
-        # Instance
+            kwargs.__setitem__("loop", loop)
         self = cls(**kwargs)
-        result: list = self._loop.run_until_complete(self.async_start())
+        # run
+        self.loop.run_until_complete(self.async_start())
         # close event loop
-        if isinstance(self._loop, EventLoop):
-            self._loop.close()
-        return self, result
+        self.loop.close()
+        return self
 
     async def async_start(self):
+        """开启异步下载器"""
+        # 创建 aiohttp session
         try:
-            # event loop
-            if (
-                not isinstance(self._loop, EventLoop)
-                or self._loop.is_closed() is True
-            ):
-                self._loop = asyncio.get_event_loop()
-                asyncio.set_event_loop(self._loop)
-            # create aiohttp.ClientSession
-            if not (
-                isinstance(self._session, Session)
-                and self._session.closed is False
-            ):
-                self._session = await self.create_client_session()
-
-            # run - self.open
+            # 创建 aiohttp session
+            await self.create_aiohttp_session()
             await self.start()
-            result: list = await self.start_request()
+            result = await self.start_request()
+            # 运行结束返回值 传递给 completed
+            await self.completed(result)
         finally:
             await self.async_close()
-        return result
 
     async def async_close(self):
-        await self.stop()
-        # close aiohttp.ClientSession
-        if isinstance(self._session, Session):
-            await self._session.close()
-
-    async def create_client_session(self):
-        "创建 aiohttp.ClientSession"
-        return Session(loop=self._loop, headers=self.merge_headers(), **self.merge_aiohttp_kwargs())
-
-    @property
-    def loop(self) -> EventLoop:
-        return self._loop
-
-    def merge_headers(self) -> CIMultiDict:
-        """aiohttp.ClientSession Headers"""
-        user_agent = self.user_agent if isinstance(self.user_agent, str) else get_user_agent("android")
-        headers = CIMultiDict(self.headers or {})
-        headers.setdefault("User-Agent", user_agent)
-        return headers
-
-    def merge_aiohttp_kwargs(self) -> dict:
-        """aiohttp.ClientSession aiohttp_kwargs"""
-        aiohttp_kwargs = self.aiohttp_kwargs.copy()
-        timeout_kwargs = dict(
-            total=100,
-            connect=None,
-            sock_read=None,
-            sock_connect=None
-        )
-        if isinstance(self.timeout, (int, float)):
-            timeout_kwargs["total"] = self.timeout
-        elif isinstance(self.timeout, dict):
-            timeout_kwargs.update(self.timeout)
-
-        timeout = ClientTimeout(**timeout_kwargs)
-        connector = TCPConnector(limit=self.limit)
-        aiohttp_kwargs.setdefault("timeout", timeout)
-        aiohttp_kwargs.setdefault("connector", connector)
-        return aiohttp_kwargs
+        """关闭异步下载器"""
+        await self.close()
+        if self.session:
+            await self.session.close()
+
+    async def start_request(self) -> list:
+        """发送 start_urls 链接"""
+        # 判断 start_urls 是否为空
+        if not self.start_urls:
+            raise NotImplementedError(f"{self.__class__.__name__}.start_urls is empty! (must be a 'list')")
+        cb_kwargs_list, start_urls = [], []
+        for item in self.start_urls:
+            if isinstance(item, (list, tuple)) and len(item) == 2:
+                url, cb_kwargs = item
+            else:
+                url, cb_kwargs = item, None
+            start_urls.append(url)
+            cb_kwargs_list.append(cb_kwargs)
+            if not self._base_url:
+                self._base_url = self.set_base_url(url)
+        result = await self.gather(*start_urls, callback=self.parse, cb_kwargs_list=cb_kwargs_list)
+        return result
 
     async def request(
         self,
-        url: str,
-        callback: callable=None,
+        url: StrOrURL,
+        *,
+        callback: RequestCallback=None,
         method: str="GET",
-        cb_kwargs: dict=None,
+        cb_kwargs: Optional[dict]=None,
         **kwargs
-    ):
-        """异步Request方法
+    ) -> Any:
+        """
+        异步请求发送
 
-        :params: url
-        :params: callback: 回调函数
-        :params: method: 请求方法
-        :params: cb_kwargs: 回调函数关键词参数
-        :params: **kwargs: 异步请求参数
+        :params: url : url地址
+        :params: callback : 响应response 回调函数(函数是异步的)
+        :params: method : 请求方法
+        :params: cb_kwargs : 回调函数 自定义参数
+        :params: **kwargs : 异步请求额外参数
         """
+        url = self.build_url(url)
+        exc_count, exc_max = 0, 30
+        response, is_close_response = None, False
         cb_kwargs = cb_kwargs if isinstance(cb_kwargs, dict) else {}
         while True:
             try:
-                async with self._session.request(method=method, url=url, **kwargs) as response:
-                    response = add_response_method(response)
-                    if callable(callback):
-                        result = await callback(response=response, **cb_kwargs)
-                        return result
-                    return response
+                response = result = await self.session.request(method=method, url=url, **kwargs)
+                # 错误request状态码捕获
+                if (
+                    isinstance(self.error_status_code, (list, tuple))
+                    and response.status in self.error_status_code
+                ):
+                    raise aiohttp.InvalidURL(
+                        f"invalid url:{str(response.url)!r}, status_code: {response.status!r}"
+                    )
+                # request状态码捕获 并重试
+                if (
+                    isinstance(self.retry_status_code, (list, tuple))
+                    and response.status in self.retry_status_code
+                ):
+                    await asyncio.sleep(1)
+                    continue
+                # response 添加方法
+                add_method_to_response(response)
+                if callable(callback):
+                    result = await callback(response, **cb_kwargs)
+                    is_close_response = True
+                break
             # 请求超时 重试
             except asyncio.exceptions.TimeoutError:
+                exc_count += 1
+                if exc_count > exc_max:
+                    raise
                 await asyncio.sleep(1)
             # 连接错误 重试
             except (
-                aiohttp.client_exceptions.ClientOSError,
-                aiohttp.client_exceptions.ClientPayloadError,
-                aiohttp.client_exceptions.ClientConnectorError,
+                aiohttp_client_exceptions.ClientOSError,
+                aiohttp_client_exceptions.ClientPayloadError,
+                aiohttp_client_exceptions.ClientConnectorError,
             ):
-                await asyncio.sleep(2)
+                exc_count += 1
+                if exc_count > exc_max:
+                    raise
+                warnings.warn("Client Connector Error", stacklevel=4)
+                await asyncio.sleep(1)
             # 服务器拒绝连接
-            except aiohttp.client_exceptions.ServerDisconnectedError:
-                await asyncio.sleep(2)
+            except aiohttp_client_exceptions.ServerDisconnectedError:
+                exc_count += 1
+                if exc_count > exc_max:
+                    raise
+                warnings.warn("Server Disconnected Error", stacklevel=4)
+                await asyncio.sleep(1)
+            finally:
+                if response and is_close_response:
+                    response.close()
+        return result
 
-    async def gather_urls(
+    async def gather(
         self,
         *urls,
-        callback: callable=None,
+        callback: RequestCallback=None,
         method: str="GET",
-        cb_kwargs_list: typing.List[dict]=None,
-        return_exceptions: bool=False,
+        cb_kwargs_list: List[dict]=None,
+        return_exceptions=False,
         **kwargs
-    ):
-        """异步Request gather方法 异步发送大量url
+    ) -> list:
+        """
+        收集 url列表，创建异步任务 并发发送
 
-        :params: *urls: url列表
-        :params: callback: 回调函数
-        :params: method: 请求方法
-        :params: cb_kwargs_list: 回调函数关键词参数 列表
-        :params: return_exceptions: 异常传递 若为真,异常将不抛出 传递值返回结果中
-        :params: **kwargs: 异步请求参数
+        :params: *urls : url 并发集合
+        :params: callback : 回调函数
+        :params: method : 请求方法
+        :params: cb_kwargs_list : 回调函数参数列表
+        :params: return_exceptions : 错误传递
+        :params: **kwargs : 请求参数
         """
+        # cb_kwargs_list
         if isinstance(cb_kwargs_list, dict):
-            cb_kwargs_list = [cb_kwargs_list]
-        elif not isinstance(cb_kwargs_list, list):
+            cb_kwargs_list = [cb_kwargs_list for _ in enumerate(urls)]
+        elif not isinstance(cb_kwargs_list, (list, tuple)):
             cb_kwargs_list = []
-        tasks = [
+
+        request_tasks = [
             self.request(
-                url=url,
-                callback=callback,
-                method=method,
-                cb_kwargs=dict(cb_kwargs),
-                **kwargs
+                url, callback=callback, method=method, cb_kwargs=cb_kwargs, **kwargs
             )
             for url, cb_kwargs in zip_longest(urls, cb_kwargs_list, fillvalue={})
         ]
-        return await asyncio.gather(*tasks, return_exceptions=return_exceptions)
-
-    async def start_request(self):
-        """异步请求入口方法"""
-        if not self.start_urls:
-            raise NotImplementedError(f"{self.__class__.__name__}.start_urls is empty(Must be a 'list')")
-        tasks = [
-            self.request(url, callback=self.parse)
-            for url in self.start_urls
-        ]
-        result = await asyncio.gather(*tasks)
+        result = await asyncio.gather(
+            *request_tasks,
+            return_exceptions=return_exceptions
+        )
         return result
 
-    async def parse(self, response: Response):
-        """默认解析方法
+    async def create_aiohttp_session(self) -> None:
+        """创建 aiohttp session"""
+        headers = self.merge_headers()
+        aiohttp_kwargs = self.merge_aiohttp_kwargs()
+        self.session = aiohttp.ClientSession(
+            loop=self.loop, headers=headers, **aiohttp_kwargs
+        )
 
-        :params: response: 异步请求响应
-        :参数传递可以使用 cb_kwargs
-        """
-        raise NotImplementedError(f"'{self.__class__.__name__}.parse' not implemented")
+    def merge_headers(self) -> CIMDict:
+        """合并 headers"""
+        headers = CIMultiDict(self.headers or {})
+        headers.setdefault("User-Agent", self.user_agent)
+        return headers
 
-    async def sleep(self, delay: typing.Union[int, float]=0, result: any=None):
-        return await asyncio.sleep(delay, result=result)
+    def merge_aiohttp_kwargs(self) -> dict:
+        """合并 aiohttp kwargs"""
+        aiohttp_kwargs = dict(self.aiohttp_kwargs or {})
+        # timeout 默认7秒
+        if isinstance(self.timeout, (int, float)) and self.timeout >= 0:
+            timeout = self.timeout
+        elif not isinstance(self.timeout, aiohttp.ClientTimeout):
+            timeout = 7
+        aiohttp_kwargs.setdefault("timeout", aiohttp.ClientTimeout(total=timeout))
+
+        # connector 默认 limit=16
+        if isinstance(self.limit, int) and self.limit >= 0:
+            limit = self.limit
+        else:
+            limit = 16
+        connector = aiohttp.TCPConnector(limit=limit, loop=self.loop, verify_ssl=self.verify_ssl)
+        aiohttp_kwargs.setdefault("connector", connector)
+        return aiohttp_kwargs
 
 
-def add_response_method(response: Response) -> Response:
-    # 为 Response 添加 xpath解析方法
-    async def _xpath(self, _xpath, *, encoding=None, errors="strict", **kwargs):
-        _htmlparse = etree.HTML(await self.text(encoding=encoding, errors=errors))
-        class XpathList(list):
-            def get(self, default=None):
-                if not self:
-                    return default
-                return self[0]
-        return XpathList(_htmlparse.xpath(_xpath, **kwargs))
-
-    # 为 Response 添加 regular 方法
-    async def _regular(self, pattern, flags=0):
-        string = await self.text()
-        return re.search(pattern, string, flags)
-
-    # 为 Response 添加 urljoin 方法
-    def _urljoin(self, _url: typing.Union[str, URL], /) -> str:
-        if isinstance(_url, str):
-            _url = URL(_url)
-        elif not isinstance(_url, URL):
+    def build_url(self, _url) -> StrOrURL:
+        """构造完整url地址"""
+        if not isinstance(_url, (str, URL)):
             return _url
-
+        _url = URL(_url)
         if _url.is_absolute():
-            return _url.human_repr()
-        return self.url.join(_url)
-
-    response.xpath = types.MethodType(_xpath, response)
-    response.re = types.MethodType(_regular, response)
-    response.urljoin = types.MethodType(_urljoin, response)
-    return response
-
-
-default_progress_columns = (
-    rich_progress.SpinnerColumn("line"),
-    rich_progress.TaskProgressColumn("[progress.percentage]{task.percentage:>6.2f}%"),
-    rich_progress.BarColumn(),
-    rich_progress.TextColumn("[progress.description]{task.completed}/{task.total}"),
-    # rich_progress.DownloadColumn(),
-    # rich_progress.TransferSpeedColumn(),
-    rich_progress.TimeElapsedColumn()
-)
-
-
-default_download_progress_columns = (
-    rich_progress.SpinnerColumn("line"),
-    rich_progress.TaskProgressColumn("[progress.percentage]{task.percentage:>6.2f}%"),
-    rich_progress.BarColumn(),
-    #rich_progress.TextColumn("[progress.description]{task.completed}/{task.total}"),
-    rich_progress.DownloadColumn(),
-    # rich_progress.TransferSpeedColumn(),
-    rich_progress.TimeElapsedColumn()
-)
-
-
-def default_live(
-    *,
-    total: int=None,
-    renderable: list=None,
-    progress_column: typing.Union[list, tuple]=None,
-    transient: bool=False,
-    console: rich_console.Console=None,
-    refresh_per_second: int=4,
-    title: str=None,
-    title_align: str=None,
-) -> typing.Tuple[rich_live.Live, rich_progress.Progress, rich_progress.Task]:
-    # total
-    if not isinstance(total, int) or total <= 0:
-        total = None
-    # progress column
-    progress_column = progress_column or default_progress_columns
-    progress = rich_progress.Progress(*progress_column)
-    progress_task = progress.add_task(description="", total=total)
-    # console
-    console = console or rich_console.Console()
-    # transient
-    transient = bool(transient)
-    # renderable
-    if not renderable:
-        live = progress
-    else:
-        # 创建表单
-        live = rich_table.Table(
-            box=rich_box.SIMPLE_HEAD, expand=True, show_header=False
-        )
-        live.add_column(no_wrap=False, justify="center")
-        for item in renderable:
-            live.add_row(f"{item}")
-        live.add_section()
-        live.add_row(progress)
-
-        # 将表单装入板块(panel)中
-        live = rich_panel.Panel(
-            live,
-            border_style="bright_blue",
-            subtitle=f"[dim]Total: {total or 0}[/]",
-            subtitle_align="right",
-            title=title,
-            title_align=title_align,
-        )
-
-    # 装入 live 中进行实时更新
-    live = rich_live.Live(
-        live,
-        transient=transient,
-        console=console,
-        refresh_per_second=refresh_per_second
-    )
-    return live, progress, progress_task
+            return _url
+        if self.base_url and isinstance(self.base_url, URL):
+            return self.base_url.join(_url)
+        return _url
+
+    @staticmethod
+    def set_base_url(url: StrOrURL, /) -> StrOrURL:
+        """设置 base_url"""
+        if url is None:
+            return None
+        if not isinstance(url, (str, URL)):
+            warnings.warn(f"{url!r} invalid base_url", stacklevel=4)
+            return None
+        url = URL(url)
+        if not url.is_absolute():
+            # 不是绝对路径
+            warnings.warn(f"{url.human_repr()!r} not absolute", stacklevel=4)
+            return None
+        return url
 
+    @property
+    def loop(self) -> EventLoop:
+        """Event Loop"""
+        if not self._loop:
+            self._loop = asyncio.get_event_loop()
+            asyncio.set_event_loop(self._loop)
+        elif isinstance(self._loop, asyncio.AbstractEventLoop):
+            if self._loop.is_closed():
+                warnings.warn("Current EventLoop is closed", stacklevel=4)
+        return self._loop
 
-class NovelSpiderTemplate(AsyncSession):
-    """小说爬虫模板文件
+    @loop.setter
+    def loop(self, _loop: EventLoop) -> None:
+        if _loop is None:
+            self._loop = None
+            return
+        if not isinstance(_loop, asyncio.AbstractEventLoop):
+            warnings.warn(f"{_loop!r} invalid EventLoop", stacklevel=4)
+            self._loop = None
+            return
+        self._loop = _loop
+        asyncio.set_event_loop(_loop)
 
-    :params: keyword: 爬虫搜索值
-    """
+    @property
+    def base_url(self) -> StrOrURL:
+        """base_url"""
+        return self._base_url
+
+    @base_url.setter
+    def base_url(self, _url: StrOrURL) -> None:
+        self._base_url = self.set_base_url(_url)
 
-    name: str = None
-    store: str = None
-    start_urls: str = None
-    user_agent: str = get_user_agent("windows")
+    @property
+    def session(self) -> Session:
+        """aiohttp session"""
+        return self._session
+
+    @session.setter
+    def session(self, _session: Session) -> None:
+        if not isinstance(_session, aiohttp.ClientSession):
+            warnings.warn(f"{_session!r} invalid aiohttp session", stacklevel=4)
+            return
+        self._session = _session
+
+    @staticmethod
+    async def sleep(delay: Union[int, float]=0, result: Any=None) -> Any:
+        """异步休眠"""
+        return await asyncio.sleep(delay, result=result)
 
-    def __init__(self, *, keyword: str=None, **kwargs):
-        super().__init__(**kwargs)
-        self._console = rich_console.Console()
-        self._keyword = keyword
-        self.book, self.author = None, None
+    @staticmethod
+    def apparent_encoding(byte: bytes):
+        return chardet(byte)["encoding"]
 
-    async def start_request(self):
-        """异步请求入口方法"""
-        if not self.start_urls:
-            raise NotImplementedError(f"{self.__class__.__name__}.start_urls is empty(Must be a 'str')")
-        if not self.name:
-            raise NotImplementedError(f"{self.__class__.__name__}.name is empty(Must be a 'str')")
-        if not self.store:
-            raise NotImplementedError(f"{self.__class__.__name__}.store is empty(Must be a 'str')")
-        self._console.print(f"[magenta b]{self.name}[/] < {self.start_urls} >\n", justify="center")
-        return await self.request(self.start_urls, self.parse)
+    async def parse(self, response: Response):
+        raise NotImplementedError(f"'{self.__class__.__name__}.parse' not implemented!")
 
-    @property
-    def keyword(self) -> str:
-        """搜索 keyword"""
-        while not(self._keyword and isinstance(self._keyword, str)):
-            self._keyword = self._console.input("[yellow b]搜索书名或作者[/][Exit]: ").strip()
-            if self._keyword.lower() in ("e", "exit"):
-                self._console.print("[red]Exit[/]")
-                sys.exit()
-        return self._keyword
+    async def completed(self, result: list) -> None:
+        """运行完成结果回调函数"""
 
-    def default_print_search_result(self, *col_names: typing.Tuple[str], books_info: typing.Dict[str, dict]):
-        """使用 rich.table 打印搜索结果
+    async def start(self) -> None:
+        """创建 aiohttp session 后调用"""
 
-        :params: *colv_names: table表头 - 表头每列名称
-        :params: books_info: table内容
-        """
-        table = rich_table.Table(
-            caption=f"[dim]< {self._keyword} > Total: {len(books_info)}[/]",
-            caption_justify="right",
-            box=rich_box.ASCII_DOUBLE_HEAD
-        )
-        # table 添加列
-        table.add_column("", no_wrap=False, style="cyan", justify="center")
-        for item in col_names:
-            table.add_column(str(item), justify="center")
-        # table 添加行
-        for index, book in books_info.items():
-            table.add_row(str(index), *[book.get(item, "") for item in col_names])
-        self._console.print(table)
+    async def close(self) -> None:
+        """关闭 aiohttp session 前调用"""
+
+
+async def xpath(
+    self,
+    query: str,
+    namespaces: Optional[Mapping[str, str]] = None,
+    encoding: Optional[str] = None,
+    type: Optional[str] = None,
+    root: Optional[Any] = None,
+    base_url: Optional[str] = None,
+    _expr: Optional[str] = None,
+    huge_tree: bool = LXML_SUPPORTS_HUGE_TREE,
+    errors: str = "strict",
+    **kwargs
+) -> ResponseSelector:
+    text = await self.text(encoding=encoding, errors=errors)
+    selector = Selector(
+        text=text,
+        type=type,
+        _expr=_expr,
+        namespaces=namespaces,
+        root=root,
+        base_url=base_url,
+        huge_tree=huge_tree,
+    )
+    return selector.xpath(query=query, **kwargs)
 
-    def default_print_novel_detail(self, *args: typing.Tuple[str]):
-        """使用 rich.panel 打印小说详情页
+async def css(
+    self,
+    query: str,
+    namespaces: Optional[Mapping[str, str]] = None,
+    encoding: Optional[str] = None,
+    type: Optional[str] = None,
+    root: Optional[Any] = None,
+    base_url: Optional[str] = None,
+    _expr: Optional[str] = None,
+    huge_tree: bool = LXML_SUPPORTS_HUGE_TREE,
+    errors: str = "strict"
+) -> ResponseSelector:
+    text = await self.text(encoding=encoding, errors=errors)
+    selector = Selector(
+        text=text,
+        type=type,
+        _expr=_expr,
+        namespaces=namespaces,
+        root=root,
+        base_url=base_url,
+        huge_tree=huge_tree,
+    )
+    return selector.css(query=query)
 
-        :params: *args: 每行内容
-        """
-        renderable = rich_table.Table(show_header=False, box=rich_box.SIMPLE_HEAD)
-        renderable.add_column(justify="left", overflow="fold",)
-        for item in args:
-            renderable.add_row(item)
-        panel = rich_panel.Panel(renderable, border_style="bright_blue")
-        self._console.print(panel)
+async def re(
+    self,
+    regex: Union[str, Pattern[str]],
+    replace_entities: bool = True,
+    namespaces: Optional[Mapping[str, str]] = None,
+    encoding: Optional[str] = None,
+    type: Optional[str] = None,
+    root: Optional[Any] = None,
+    base_url: Optional[str] = None,
+    _expr: Optional[str] = None,
+    huge_tree: bool = LXML_SUPPORTS_HUGE_TREE,
+    errors: str = "strict",
+) -> ResponseSelector:
+    text = await self.text(encoding=encoding, errors=errors)
+    selector = Selector(
+        text=text,
+        type=type,
+        _expr=_expr,
+        namespaces=namespaces,
+        root=root,
+        base_url=base_url,
+        huge_tree=huge_tree,
+    )
+    return selector.re(regex=regex, replace_entities=replace_entities)
 
-    def select_form_items(
-        self,
-        *items: typing.Tuple[str],
-        description: str=None,
-        exception: typing.List[str]=None,
-        arbitrary: bool=False
-    ):
-        """选择器
-
-        :params: *items: input选择范围
-        :params: description: 说明，介绍
-        :params: exception: 额外的选择范围, 当input输入在其中是返回
-        :params: arbitrary: 任意值返回
+def urljoin(self, _url: Union[str, URL], /) -> StrOrURL:
+    if isinstance(_url, str):
+        _url = URL(_url)
+    elif not isinstance(_url, URL):
+        return _url
+    if _url.is_absolute():
+        return _url
+    return self.url.join(_url)
 
-        注意: 输入 'e' 或者 'exit' 将使用 sys.exit() 关闭程序
-        """
-        # 需要额外处理的参数
-        exception = [str(e).lower() for e in exception or []]
-        exception = set(exception)
-        items = [str(item) for item in items]
-        items.extend(exception)
-        description = description or "[yellow b]请选择: [/]"
-        while True:
-            select = self._console.input(description).strip()
-            if select.lower() in ("e", "exit"):
-                self._console.print("[red]Exit[/]")
-                sys.exit()
-            if select in items or arbitrary:
-                break
-        return select
+def add_method_to_response(response: Response) -> None:
+    """
+    为异步response添加实例方法
+    """
+    response.re = MethodType(re, response)
+    response.css = MethodType(css, response)
+    response.xpath = MethodType(xpath, response)
+    response.urljoin = MethodType(urljoin, response)
```

### Comparing `pyxk-0.5.2/pyxk/aes/_fmtdata.py` & `pyxk-0.5.3/pyxk/aes/_fmtdata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 AES加解密 数据初始化
 """
-from pyxk.lazy_loader import LazyLoader
+from pyxk.utils import LazyLoader
 
 AES = LazyLoader("AES", globals(), "Crypto.Cipher.AES")
 
 
 
 # 目前支持的模式
 MODES = {
```

### Comparing `pyxk-0.5.2/pyxk/aes/cryptor.py` & `pyxk-0.5.3/pyxk/aes/cryptor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 AES 加解密
 """
-from pyxk.lazy_loader import LazyLoader
+from pyxk.utils import LazyLoader
 
 copy = LazyLoader("copy", globals(), "copy")
 AES = LazyLoader("AES", globals(), "Crypto.Cipher.AES")
 typing = LazyLoader("typing", globals(), "typing")
 fmtdata = LazyLoader("fmtdata", globals(), "pyxk.aes._fmtdata")
```

### Comparing `pyxk-0.5.2/pyxk/requests/api.py` & `pyxk-0.5.3/pyxk/requests/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,382 +1,385 @@
 from pyxk.requests.sessions import Session
 
 
-default_timeout = 5
-
 def request(
     method,
     url,
     *,
     params=None,
     data=None,
     headers=None,
     cookies=None,
     files=None,
     auth=None,
-    timeout=None,
+    timeout=5,
     allow_redirects=True,
     proxies=None,
     hooks=None,
     stream=None,
     verify=None,
     cert=None,
     json=None,
-    transient=None,
+    show_status=True,
     user_agent=None
 ):
-    with Session(user_agent=user_agent, transient=transient) as session:
+    with Session(user_agent=user_agent) as session:
         return session.request(
             method=method,
             url=url,
             params=params,
             data=data,
             headers=headers,
             cookies=cookies,
             files=files,
             auth=auth,
-            timeout=timeout or default_timeout,
+            timeout=timeout,
             allow_redirects=allow_redirects,
             proxies=proxies,
             hooks=hooks,
             stream=stream,
             verify=verify,
             cert=cert,
-            json=json
+            json=json,
+            show_status=show_status,
         )
 
 def get(
     url,
     *,
     params=None,
     data=None,
     headers=None,
     cookies=None,
     files=None,
     auth=None,
-    timeout=None,
+    timeout=5,
     allow_redirects=True,
     proxies=None,
     hooks=None,
     stream=None,
     verify=None,
     cert=None,
     json=None,
-    transient=None,
+    show_status=True,
     user_agent=None
 ):
     return request(
         method="GET",
         url=url,
         params=params,
         data=data,
         headers=headers,
         cookies=cookies,
         files=files,
         auth=auth,
-        timeout=timeout or default_timeout,
+        timeout=timeout,
         allow_redirects=allow_redirects,
         proxies=proxies,
         hooks=hooks,
         stream=stream,
         verify=verify,
         cert=cert,
         json=json,
-        transient=transient,
+        show_status=show_status,
         user_agent=user_agent
     )
 
 def post(
     url,
     *,
     params=None,
     data=None,
     headers=None,
     cookies=None,
     files=None,
     auth=None,
-    timeout=None,
+    timeout=5,
     allow_redirects=True,
     proxies=None,
     hooks=None,
     stream=None,
     verify=None,
     cert=None,
     json=None,
-    transient=None,
+    show_status=True,
     user_agent=None
 ):
     return request(
         method="POST",
         url=url,
         params=params,
         data=data,
         headers=headers,
         cookies=cookies,
         files=files,
         auth=auth,
-        timeout=timeout or default_timeout,
+        timeout=timeout,
         allow_redirects=allow_redirects,
         proxies=proxies,
         hooks=hooks,
         stream=stream,
         verify=verify,
         cert=cert,
         json=json,
-        transient=transient,
+        show_status=show_status,
         user_agent=user_agent
     )
 
 def head(
     url,
     *,
     params=None,
     data=None,
     headers=None,
     cookies=None,
     files=None,
     auth=None,
-    timeout=None,
+    timeout=5,
     allow_redirects=False,
     proxies=None,
     hooks=None,
     stream=None,
     verify=None,
     cert=None,
     json=None,
-    transient=None,
+    show_status=True,
     user_agent=None
 ):
     return request(
         method="HEAD",
         url=url,
         params=params,
         data=data,
         headers=headers,
         cookies=cookies,
         files=files,
         auth=auth,
-        timeout=timeout or default_timeout,
+        timeout=timeout,
         allow_redirects=allow_redirects,
         proxies=proxies,
         hooks=hooks,
         stream=stream,
         verify=verify,
         cert=cert,
         json=json,
-        transient=transient,
+        show_status=show_status,
         user_agent=user_agent
     )
 
 def delete(
     url,
     *,
     params=None,
     data=None,
     headers=None,
     cookies=None,
     files=None,
     auth=None,
-    timeout=None,
+    timeout=5,
     allow_redirects=True,
     proxies=None,
     hooks=None,
     stream=None,
     verify=None,
     cert=None,
     json=None,
-    transient=None,
+    show_status=True,
     user_agent=None
 ):
     return request(
         method="DELETE",
         url=url,
         params=params,
         data=data,
         headers=headers,
         cookies=cookies,
         files=files,
         auth=auth,
-        timeout=timeout or default_timeout,
+        timeout=timeout,
         allow_redirects=allow_redirects,
         proxies=proxies,
         hooks=hooks,
         stream=stream,
         verify=verify,
         cert=cert,
         json=json,
-        transient=transient,
+        show_status=show_status,
         user_agent=user_agent
     )
 
 def patch(
     url,
     *,
     params=None,
     data=None,
     headers=None,
     cookies=None,
     files=None,
     auth=None,
-    timeout=None,
+    timeout=5,
     allow_redirects=True,
     proxies=None,
     hooks=None,
     stream=None,
     verify=None,
     cert=None,
     json=None,
-    transient=None,
+    show_status=True,
     user_agent=None
 ):
     return request(
         method="PATCH",
         url=url,
         params=params,
         data=data,
         headers=headers,
         cookies=cookies,
         files=files,
         auth=auth,
-        timeout=timeout or default_timeout,
+        timeout=timeout,
         allow_redirects=allow_redirects,
         proxies=proxies,
         hooks=hooks,
         stream=stream,
         verify=verify,
         cert=cert,
         json=json,
-        transient=transient,
+        show_status=show_status,
         user_agent=user_agent
     )
 
 def put(
     url,
     *,
     params=None,
     data=None,
     headers=None,
     cookies=None,
     files=None,
     auth=None,
-    timeout=None,
+    timeout=5,
     allow_redirects=True,
     proxies=None,
     hooks=None,
     stream=None,
     verify=None,
     cert=None,
     json=None,
-    transient=None,
+    show_status=True,
     user_agent=None
 ):
     return request(
         method="PUT",
         url=url,
         params=params,
         data=data,
         headers=headers,
         cookies=cookies,
         files=files,
         auth=auth,
-        timeout=timeout or default_timeout,
+        timeout=timeout,
         allow_redirects=allow_redirects,
         proxies=proxies,
         hooks=hooks,
         stream=stream,
         verify=verify,
         cert=cert,
         json=json,
-        transient=transient,
+        show_status=show_status,
         user_agent=user_agent
     )
 
 def options(
     url,
     *,
     params=None,
     data=None,
     headers=None,
     cookies=None,
     files=None,
     auth=None,
-    timeout=None,
+    timeout=5,
     allow_redirects=True,
     proxies=None,
     hooks=None,
     stream=None,
     verify=None,
     cert=None,
     json=None,
-    transient=None,
+    show_status=True ,
     user_agent=None
 ):
     return request(
         method="OPTIONS",
         url=url,
         params=params,
         data=data,
         headers=headers,
         cookies=cookies,
         files=files,
         auth=auth,
-        timeout=timeout or default_timeout,
+        timeout=timeout,
         allow_redirects=allow_redirects,
         proxies=proxies,
         hooks=hooks,
         stream=stream,
         verify=verify,
         cert=cert,
         json=json,
-        transient=transient,
+        show_status=show_status,
         user_agent=user_agent
     )
 
-def wget(
+def downloader(
     url,
     method="GET",
     *,
     params=None,
     data=None,
     headers=None,
     cookies=None,
     files=None,
     auth=None,
-    timeout=None,
+    timeout=5,
     allow_redirects=True,
     proxies=None,
     hooks=None,
     stream=True,
     verify=None,
     cert=None,
     json=None,
     transient=False,
     output=None,
-    resume=False,
-    threads=1,
-    user_agent=None
+    restore=False,
+    thread_num=None,
+    user_agent=None,
+    show_status=False
 ):
     try:
-        session = Session(user_agent=user_agent, transient=transient)
-        return session.wget(
+        session = Session(user_agent=user_agent)
+        response = session.downloader(
             method=method,
             url=url,
             params=params,
             data=data,
             headers=headers,
             cookies=cookies,
             files=files,
             auth=auth,
-            timeout=timeout or default_timeout,
+            timeout=timeout,
             allow_redirects=allow_redirects,
             proxies=proxies,
             hooks=hooks,
             stream=stream,
             verify=verify,
             cert=cert,
             json=json,
             output=output,
-            resume=resume,
-            threads=threads
+            show_status=show_status,
+            restore=restore,
+            thread_num=thread_num,
+            transient=transient
         )
     finally:
         session.close()
+    return response
```

