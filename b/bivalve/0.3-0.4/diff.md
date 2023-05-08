# Comparing `tmp/bivalve-0.3.tar.gz` & `tmp/bivalve-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bivalve-0.3.tar", last modified: Sun May  7 09:56:58 2023, max compression
+gzip compressed data, was "bivalve-0.4.tar", last modified: Mon May  8 23:47:02 2023, max compression
```

## Comparing `bivalve-0.3.tar` & `bivalve-0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-07 09:56:58.565713 bivalve-0.3/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1064 2023-05-07 09:56:58.565713 bivalve-0.3/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      434 2023-04-04 02:24:44.000000 bivalve-0.3/README.md
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-07 09:56:58.565713 bivalve-0.3/bivalve/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-04 02:24:44.000000 bivalve-0.3/bivalve/__init__.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     8092 2023-05-07 09:30:11.000000 bivalve-0.3/bivalve/agent.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5699 2023-05-07 08:43:55.000000 bivalve-0.3/bivalve/aio.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-07 09:56:58.565713 bivalve-0.3/bivalve/example/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-04 02:24:44.000000 bivalve-0.3/bivalve/example/__init__.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      802 2023-05-07 07:36:46.000000 bivalve-0.3/bivalve/example/bridge.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2281 2023-05-07 09:30:37.000000 bivalve-0.3/bivalve/example/client.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1731 2023-05-07 09:30:35.000000 bivalve-0.3/bivalve/example/server.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2990 2023-05-07 05:59:39.000000 bivalve-0.3/bivalve/logging.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1799 2023-05-07 06:10:19.000000 bivalve-0.3/bivalve/nio.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1502 2023-05-07 06:02:08.000000 bivalve-0.3/bivalve/util.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-07 09:56:58.565713 bivalve-0.3/bivalve.egg-info/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1064 2023-05-07 09:56:58.000000 bivalve-0.3/bivalve.egg-info/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      350 2023-05-07 09:56:58.000000 bivalve-0.3/bivalve.egg-info/SOURCES.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-05-07 09:56:58.000000 bivalve-0.3/bivalve.egg-info/dependency_links.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        8 2023-05-07 09:56:58.000000 bivalve-0.3/bivalve.egg-info/top_level.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-05-07 09:56:58.565713 bivalve-0.3/setup.cfg
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1194 2023-05-07 09:55:39.000000 bivalve-0.3/setup.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-08 23:47:02.351697 bivalve-0.4/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1064 2023-05-08 23:47:02.351697 bivalve-0.4/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      434 2023-04-04 02:24:44.000000 bivalve-0.4/README.md
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-08 23:47:02.351697 bivalve-0.4/bivalve/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-04 02:24:44.000000 bivalve-0.4/bivalve/__init__.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     8090 2023-05-08 21:02:29.000000 bivalve-0.4/bivalve/agent.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5886 2023-05-08 23:44:21.000000 bivalve-0.4/bivalve/aio.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-08 23:47:02.351697 bivalve-0.4/bivalve/example/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-04 02:24:44.000000 bivalve-0.4/bivalve/example/__init__.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      802 2023-05-07 07:36:46.000000 bivalve-0.4/bivalve/example/bridge.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2281 2023-05-07 09:30:37.000000 bivalve-0.4/bivalve/example/client.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1731 2023-05-07 09:30:35.000000 bivalve-0.4/bivalve/example/server.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2990 2023-05-07 05:59:39.000000 bivalve-0.4/bivalve/logging.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1799 2023-05-07 06:10:19.000000 bivalve-0.4/bivalve/nio.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1502 2023-05-07 06:02:08.000000 bivalve-0.4/bivalve/util.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-08 23:47:02.351697 bivalve-0.4/bivalve.egg-info/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1064 2023-05-08 23:47:02.000000 bivalve-0.4/bivalve.egg-info/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      350 2023-05-08 23:47:02.000000 bivalve-0.4/bivalve.egg-info/SOURCES.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-05-08 23:47:02.000000 bivalve-0.4/bivalve.egg-info/dependency_links.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        8 2023-05-08 23:47:02.000000 bivalve-0.4/bivalve.egg-info/top_level.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-05-08 23:47:02.351697 bivalve-0.4/setup.cfg
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1194 2023-05-08 23:46:05.000000 bivalve-0.4/setup.py
```

### Comparing `bivalve-0.3/PKG-INFO` & `bivalve-0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bivalve
-Version: 0.3
+Version: 0.4
 Summary: A bi-directional shell-like socket protocol framework using asyncio.
 Home-page: https://github.com/lainproliant/bivalve
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: network sockets protocol shell
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bivalve-0.3/bivalve/agent.py` & `bivalve-0.4/bivalve/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         log.info("Outbound peer connection on {host}:{port} (ssl={ssl}) established.")
         self.add_connection(conn)
         return conn
 
     def bridge(self) -> Connection:
         if self._max_peers and len(self._conn_ctx_map) >= self._max_peers:
             log.warning(
-                f"Cancelled outbound connection: maximum number of peers reached ({self._max_peers})."
+                f"Cancelled bridge connection: maximum number of peers reached ({self._max_peers})."
             )
             raise RuntimeError("Maximum number of peer connections reached.")
 
         send_queue: asyncio.Queue[str] = asyncio.Queue()
         recv_queue: asyncio.Queue[str] = asyncio.Queue()
 
         our_conn = BridgeConnection(send_queue, recv_queue)
```

### Comparing `bivalve-0.3/bivalve/aio.py` & `bivalve-0.4/bivalve/aio.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,19 @@
 
     ID = BaseID
 
     def __init__(self, id: ID):
         self.id = id
         self.alive = AtomicValue(True)
 
+    @classmethod
+    async def connect(cls, host: str, port: int, ssl=None) -> "Connection":
+        stream = Stream.connect(host, port, ssl=ssl)
+        return StreamConnection(stream)
+
     async def close(self):
         if await self.alive():
             await self.alive.set(False)
 
     async def send(self, *argv):
         assert argv
         assert len(argv) > 0
```

### Comparing `bivalve-0.3/bivalve/example/bridge.py` & `bivalve-0.4/bivalve/example/bridge.py`

 * *Files identical despite different names*

### Comparing `bivalve-0.3/bivalve/example/client.py` & `bivalve-0.4/bivalve/example/client.py`

 * *Files identical despite different names*

### Comparing `bivalve-0.3/bivalve/example/server.py` & `bivalve-0.4/bivalve/example/server.py`

 * *Files identical despite different names*

### Comparing `bivalve-0.3/bivalve/logging.py` & `bivalve-0.4/bivalve/logging.py`

 * *Files identical despite different names*

### Comparing `bivalve-0.3/bivalve/nio.py` & `bivalve-0.4/bivalve/nio.py`

 * *Files identical despite different names*

### Comparing `bivalve-0.3/bivalve/util.py` & `bivalve-0.4/bivalve/util.py`

 * *Files identical despite different names*

### Comparing `bivalve-0.3/bivalve.egg-info/PKG-INFO` & `bivalve-0.4/bivalve.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bivalve
-Version: 0.3
+Version: 0.4
 Summary: A bi-directional shell-like socket protocol framework using asyncio.
 Home-page: https://github.com/lainproliant/bivalve
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: network sockets protocol shell
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bivalve-0.3/setup.py` & `bivalve-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="bivalve",
-    version="0.3",
+    version="0.4",
     description="A bi-directional shell-like socket protocol framework using asyncio.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lainproliant/bivalve",
     author="Lain Musgrove (lainproliant)",
     author_email="lainproliant@gmail.com",
     license="BSD",
```

