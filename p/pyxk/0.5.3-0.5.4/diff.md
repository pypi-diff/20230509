# Comparing `tmp/pyxk-0.5.3.tar.gz` & `tmp/pyxk-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxk-0.5.3.tar", last modified: Tue May  9 07:19:15 2023, max compression
+gzip compressed data, was "pyxk-0.5.4.tar", last modified: Tue May  9 09:35:36 2023, max compression
```

## Comparing `pyxk-0.5.3.tar` & `pyxk-0.5.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 07:19:15.593999 pyxk-0.5.3/
--rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.5.3/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-09 07:19:15.593999 pyxk-0.5.3/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.5.3/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 07:19:15.583999 pyxk-0.5.3/pyxk/
--rw-rw----   0 root         (0) everybody  (9997)       53 2023-05-08 09:38:07.000000 pyxk-0.5.3/pyxk/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 07:19:15.593999 pyxk-0.5.3/pyxk/aclient/
--rw-rw----   0 root         (0) everybody  (9997)       90 2023-05-08 07:54:13.000000 pyxk-0.5.3/pyxk/aclient/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    15036 2023-05-09 03:25:00.000000 pyxk-0.5.3/pyxk/aclient/client.py
--rw-rw----   0 root         (0) everybody  (9997)      699 2023-04-30 15:43:19.000000 pyxk-0.5.3/pyxk/aclient/typedef.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 07:19:15.593999 pyxk-0.5.3/pyxk/aes/
--rw-rw----   0 root         (0) everybody  (9997)       79 2023-04-10 03:10:37.000000 pyxk-0.5.3/pyxk/aes/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3633 2023-05-08 07:57:14.000000 pyxk-0.5.3/pyxk/aes/_fmtdata.py
--rw-rw----   0 root         (0) everybody  (9997)     4695 2023-05-08 07:56:51.000000 pyxk-0.5.3/pyxk/aes/cryptor.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 07:19:15.593999 pyxk-0.5.3/pyxk/m3u8downloader/
--rw-rw----   0 root         (0) everybody  (9997)       66 2023-05-08 07:55:15.000000 pyxk-0.5.3/pyxk/m3u8downloader/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     2300 2023-05-09 07:15:49.000000 pyxk-0.5.3/pyxk/m3u8downloader/enter_point.py
--rw-rw----   0 root         (0) everybody  (9997)     4821 2023-05-08 07:56:03.000000 pyxk-0.5.3/pyxk/m3u8downloader/m3u8download.py
--rw-rw----   0 root         (0) everybody  (9997)     2968 2023-05-08 04:33:43.000000 pyxk-0.5.3/pyxk/m3u8downloader/m3u8parse.py
--rw-rw----   0 root         (0) everybody  (9997)    10817 2023-05-09 07:07:43.000000 pyxk-0.5.3/pyxk/m3u8downloader/main.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 07:19:15.593999 pyxk-0.5.3/pyxk/requests/
--rw-rw----   0 root         (0) everybody  (9997)      247 2023-05-08 07:57:36.000000 pyxk-0.5.3/pyxk/requests/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     7480 2023-05-08 07:58:19.000000 pyxk-0.5.3/pyxk/requests/api.py
--rw-rw----   0 root         (0) everybody  (9997)     3309 2023-05-09 03:19:15.000000 pyxk-0.5.3/pyxk/requests/entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)    14682 2023-05-09 03:23:24.000000 pyxk-0.5.3/pyxk/requests/sessions.py
--rw-rw----   0 root         (0) everybody  (9997)    18965 2023-05-08 09:56:53.000000 pyxk-0.5.3/pyxk/utils.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 07:19:15.593999 pyxk-0.5.3/pyxk.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-09 07:19:15.000000 pyxk-0.5.3/pyxk.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      627 2023-05-09 07:19:15.000000 pyxk-0.5.3/pyxk.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-09 07:19:15.000000 pyxk-0.5.3/pyxk.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       99 2023-05-09 07:19:15.000000 pyxk-0.5.3/pyxk.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       55 2023-05-09 07:19:15.000000 pyxk-0.5.3/pyxk.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-05-09 07:19:15.000000 pyxk-0.5.3/pyxk.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-09 07:19:15.593999 pyxk-0.5.3/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      927 2023-05-09 07:18:11.000000 pyxk-0.5.3/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 09:35:36.212000 pyxk-0.5.4/
+-rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.5.4/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-09 09:35:36.212000 pyxk-0.5.4/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.5.4/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 09:35:36.192000 pyxk-0.5.4/pyxk/
+-rw-rw----   0 root         (0) everybody  (9997)       53 2023-05-08 09:38:07.000000 pyxk-0.5.4/pyxk/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 09:35:36.202000 pyxk-0.5.4/pyxk/aclient/
+-rw-rw----   0 root         (0) everybody  (9997)       90 2023-05-08 07:54:13.000000 pyxk-0.5.4/pyxk/aclient/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    15040 2023-05-09 09:06:43.000000 pyxk-0.5.4/pyxk/aclient/client.py
+-rw-rw----   0 root         (0) everybody  (9997)      699 2023-04-30 15:43:19.000000 pyxk-0.5.4/pyxk/aclient/typedef.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 09:35:36.202000 pyxk-0.5.4/pyxk/aes/
+-rw-rw----   0 root         (0) everybody  (9997)       79 2023-04-10 03:10:37.000000 pyxk-0.5.4/pyxk/aes/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3633 2023-05-08 07:57:14.000000 pyxk-0.5.4/pyxk/aes/_fmtdata.py
+-rw-rw----   0 root         (0) everybody  (9997)     4695 2023-05-08 07:56:51.000000 pyxk-0.5.4/pyxk/aes/cryptor.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 09:35:36.202000 pyxk-0.5.4/pyxk/m3u8downloader/
+-rw-rw----   0 root         (0) everybody  (9997)       66 2023-05-08 07:55:15.000000 pyxk-0.5.4/pyxk/m3u8downloader/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     2312 2023-05-09 08:54:39.000000 pyxk-0.5.4/pyxk/m3u8downloader/enter_point.py
+-rw-rw----   0 root         (0) everybody  (9997)     4821 2023-05-08 07:56:03.000000 pyxk-0.5.4/pyxk/m3u8downloader/m3u8download.py
+-rw-rw----   0 root         (0) everybody  (9997)     2968 2023-05-08 04:33:43.000000 pyxk-0.5.4/pyxk/m3u8downloader/m3u8parse.py
+-rw-rw----   0 root         (0) everybody  (9997)    10951 2023-05-09 08:47:57.000000 pyxk-0.5.4/pyxk/m3u8downloader/main.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 09:35:36.212000 pyxk-0.5.4/pyxk/requests/
+-rw-rw----   0 root         (0) everybody  (9997)      247 2023-05-08 07:57:36.000000 pyxk-0.5.4/pyxk/requests/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     7480 2023-05-08 07:58:19.000000 pyxk-0.5.4/pyxk/requests/api.py
+-rw-rw----   0 root         (0) everybody  (9997)     3309 2023-05-09 03:19:15.000000 pyxk-0.5.4/pyxk/requests/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    14682 2023-05-09 03:23:24.000000 pyxk-0.5.4/pyxk/requests/sessions.py
+-rw-rw----   0 root         (0) everybody  (9997)    18965 2023-05-08 09:56:53.000000 pyxk-0.5.4/pyxk/utils.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 09:35:36.202000 pyxk-0.5.4/pyxk.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-09 09:35:36.000000 pyxk-0.5.4/pyxk.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      627 2023-05-09 09:35:36.000000 pyxk-0.5.4/pyxk.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-09 09:35:36.000000 pyxk-0.5.4/pyxk.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       99 2023-05-09 09:35:36.000000 pyxk-0.5.4/pyxk.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       55 2023-05-09 09:35:36.000000 pyxk-0.5.4/pyxk.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-05-09 09:35:36.000000 pyxk-0.5.4/pyxk.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-09 09:35:36.212000 pyxk-0.5.4/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      927 2023-05-09 09:35:11.000000 pyxk-0.5.4/setup.py
```

### Comparing `pyxk-0.5.3/LICENSE` & `pyxk-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.3/pyxk/aclient/client.py` & `pyxk-0.5.4/pyxk/aclient/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,22 +196,22 @@
                 aiohttp_client_exceptions.ClientOSError,
                 aiohttp_client_exceptions.ClientPayloadError,
                 aiohttp_client_exceptions.ClientConnectorError,
             ):
                 exc_count += 1
                 if exc_count > exc_max:
                     raise
-                warnings.warn("Client Connector Error", stacklevel=4)
+                # warnings.warn("Client Connector Error", stacklevel=4)
                 await asyncio.sleep(1)
             # 服务器拒绝连接
             except aiohttp_client_exceptions.ServerDisconnectedError:
                 exc_count += 1
                 if exc_count > exc_max:
                     raise
-                warnings.warn("Server Disconnected Error", stacklevel=4)
+                # warnings.warn("Server Disconnected Error", stacklevel=4)
                 await asyncio.sleep(1)
             finally:
                 if response and is_close_response:
                     response.close()
         return result
 
     async def gather(
```

### Comparing `pyxk-0.5.3/pyxk/aclient/typedef.py` & `pyxk-0.5.4/pyxk/aclient/typedef.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.3/pyxk/aes/_fmtdata.py` & `pyxk-0.5.4/pyxk/aes/_fmtdata.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.3/pyxk/aes/cryptor.py` & `pyxk-0.5.4/pyxk/aes/cryptor.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.3/pyxk/m3u8downloader/enter_point.py` & `pyxk-0.5.4/pyxk/m3u8downloader/enter_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     # 将参数传递给子命令
     if ctx.invoked_subcommand:
         ctx.obj.update(ctx.params)
         return
     # 没有调用子命令
     if not url:
         url = click.prompt("请输入 m3u8 url", type=str)
-    load_url(url, output=output, reload=reload, reserve=reserve, headers=headers, verify=verify, limit=limit)
+    load_url(url, output=output, reload=reload, reserve=reserve, headers=dict(headers), verify=verify, limit=limit)
 
 @main.command
 @click.pass_obj
 @click.argument("content", type=click.Path(exists=True), metavar="<m3u8 file path>")
 @click.option("-u", "--url", "url", type=str, default=None, help="m3u8 url")
 @click.option("-o", "--output", "output", type=str, default=None, help="M3U8存储路径")
 @click.option("--reload", is_flag=True, help="重载m3u8资源")
@@ -39,11 +39,11 @@
     """下载m3u8资源 - m3u8 content"""
     load_content(
         content=content,
         url=url or obj["url"],
         output=output or obj["output"],
         reload=reload,
         reserve=reserve,
-        headers=headers or obj["headers"],
+        headers=dict(headers or obj["headers"]),
         verify=verify,
         limit=limit or obj["limit"]
     )
```

### Comparing `pyxk-0.5.3/pyxk/m3u8downloader/m3u8download.py` & `pyxk-0.5.4/pyxk/m3u8downloader/m3u8download.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.3/pyxk/m3u8downloader/m3u8parse.py` & `pyxk-0.5.4/pyxk/m3u8downloader/m3u8parse.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.3/pyxk/m3u8downloader/main.py` & `pyxk-0.5.4/pyxk/m3u8downloader/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         # 关闭requests警告
         if self._verify is False:
             import urllib3
             urllib3.disable_warnings()
         content = self.get_m3u8_content(url)
         # 无效m3u8内容
         if not self._is_m3u8_content(content):
-            self._console.print(f"[red b]m3u8 url <{url}> is not available![/]")
+            self._console.print("[red b]m3u8 url is not available!")
             return
         # 解析m3u8
         return self.startparse(content=content, url=url)
 
     def load_content(
         self,
         content: str,
@@ -204,15 +204,17 @@
         # 文件完整路径
         file = self._generate_filename(url, is_m3u8key)
         mode, attr, encoding = "r", "text", "utf-8"
         if is_m3u8key:
             mode, attr, encoding = "rb", "content", None
         # 获取网络资源
         if self._reload or not file or not os.path.isfile(file):
-            response = self._session.get(url, headers=self._headers, verify=self._verify)
+            response = self._session.get(url, headers=self._headers, verify=self._verify, timeout=10)
+            if response.status_code != 200:
+                self._console.print(f"[red]<Response [{response.status_code}] {url}>[/]")
             content = getattr(response, attr)
         # 获取本地资源
         else:
             with open(file, mode, encoding=encoding) as read_fileobj:
                 content = read_fileobj.read()
         return content
```

### Comparing `pyxk-0.5.3/pyxk/requests/api.py` & `pyxk-0.5.4/pyxk/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.3/pyxk/requests/entry_point.py` & `pyxk-0.5.4/pyxk/requests/entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.3/pyxk/requests/sessions.py` & `pyxk-0.5.4/pyxk/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.3/pyxk/utils.py` & `pyxk-0.5.4/pyxk/utils.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.3/pyxk.egg-info/SOURCES.txt` & `pyxk-0.5.4/pyxk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.3/setup.py` & `pyxk-0.5.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyxk",
-    version="0.5.3",
+    version="0.5.4",
     author="pengke",
     install_requires=[
         "requests",
         "pycryptodome",
         "rich",
         "m3u8",
         "aiohttp",
```

