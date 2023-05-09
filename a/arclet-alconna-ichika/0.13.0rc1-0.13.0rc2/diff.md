# Comparing `tmp/arclet-alconna-ichika-0.13.0rc1.tar.gz` & `tmp/arclet-alconna-ichika-0.13.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-ichika-0.13.0rc1.tar", last modified: Tue May  9 04:22:45 2023, max compression
+gzip compressed data, was "arclet-alconna-ichika-0.13.0rc2.tar", last modified: Tue May  9 04:37:11 2023, max compression
```

## Comparing `arclet-alconna-ichika-0.13.0rc1.tar` & `arclet-alconna-ichika-0.13.0rc2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet-alconna-ichika-0.13.0rc1/LICENSE
--rw-r--r--   0        0        0     6194 2023-05-09 04:02:48.655669 arclet-alconna-ichika-0.13.0rc1/pyproject.toml
--rw-r--r--   0        0        0     7138 2023-01-30 09:01:24.879470 arclet-alconna-ichika-0.13.0rc1/README.md
--rw-r--r--   0        0        0       80 2023-05-09 04:08:01.631055 arclet-alconna-ichika-0.13.0rc1/src/arclet/alconna/ichika/__init__.py
--rw-r--r--   0        0        0     5696 2023-05-09 04:20:57.228106 arclet-alconna-ichika-0.13.0rc1/src/arclet/alconna/ichika/adapter.py
--rw-r--r--   0        0        0     1256 2023-05-09 04:21:37.796354 arclet-alconna-ichika-0.13.0rc1/src/arclet/alconna/ichika/typings.py
--rw-r--r--   0        0        0     7591 1970-01-01 00:00:00.000000 arclet-alconna-ichika-0.13.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet-alconna-ichika-0.13.0rc2/LICENSE
+-rw-r--r--   0        0        0     6194 2023-05-09 04:32:45.106719 arclet-alconna-ichika-0.13.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     7138 2023-01-30 09:01:24.879470 arclet-alconna-ichika-0.13.0rc2/README.md
+-rw-r--r--   0        0        0       80 2023-05-09 04:08:01.631055 arclet-alconna-ichika-0.13.0rc2/src/arclet/alconna/ichika/__init__.py
+-rw-r--r--   0        0        0     6127 2023-05-09 04:36:47.494072 arclet-alconna-ichika-0.13.0rc2/src/arclet/alconna/ichika/adapter.py
+-rw-r--r--   0        0        0     1256 2023-05-09 04:21:37.796354 arclet-alconna-ichika-0.13.0rc2/src/arclet/alconna/ichika/typings.py
+-rw-r--r--   0        0        0     7591 1970-01-01 00:00:00.000000 arclet-alconna-ichika-0.13.0rc2/PKG-INFO
```

### Comparing `arclet-alconna-ichika-0.13.0rc1/LICENSE` & `arclet-alconna-ichika-0.13.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ichika-0.13.0rc1/pyproject.toml` & `arclet-alconna-ichika-0.13.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arclet-alconna-ichika"
-version = "0.13.0rc1"
+version = "0.13.0rc2"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "ichika>=0.0.5",
 ]
 description = "Support Alconna to BlueGlassBlock/Ichika"
@@ -56,29 +56,29 @@
 [tool.mina.packages.core]
 includes = [
     "src/arclet/alconna/graia",
 ]
 
 [tool.mina.packages.core.project]
 name = "arclet-alconna-graia"
-version = "0.13.0rc1"
+version = "0.13.0rc2"
 description = "Support Alconna to GraiaProject"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
     "alconna",
     "graia",
     "arclet",
     "ariadne",
 ]
 dependencies = [
-    "arclet-alconna<2.0.0, >=1.7.0rc6",
+    "arclet-alconna<2.0.0, >=1.7.0rc7",
     "arclet-alconna-tools<0.7.0, >=0.6.0rc1",
     "tarina>=0.3.3",
     "nepattern<0.6.0, >=0.5.6",
     "creart-graia>=0.1.5",
     "creart>=0.2.1",
     "graia-amnesia>=0.5.0",
     "graia-broadcast>=0.18.2",
@@ -108,20 +108,20 @@
 alconna_behavior = "arclet.alconna.graia.create:AlconnaBehaviorCreator"
 
 [tool.mina.packages.ariadne]
 includes = [
     "src/arclet/alconna/ariadne",
 ]
 raw-dependencies = [
-    "arclet-alconna-graia<0.13.0, >= 0.13.0rc1",
+    "arclet-alconna-graia<0.13.0, >= 0.13.0rc2",
 ]
 
 [tool.mina.packages.ariadne.project]
 name = "arclet-alconna-ariadne"
-version = "0.13.0rc1"
+version = "0.13.0rc2"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "graia-ariadne<1.0.0, >=0.7.14",
 ]
 description = "Support Alconna to GraiaProject/Ariadne"
@@ -149,20 +149,20 @@
 repository = "https://github.com/ArcletProject/Alconna-Graia"
 
 [tool.mina.packages.avilla]
 includes = [
     "src/arclet/alconna/avilla",
 ]
 raw-dependencies = [
-    "arclet-alconna-graia<0.13.0, >= 0.13.0rc1",
+    "arclet-alconna-graia<0.13.0, >= 0.13.0rc2",
 ]
 
 [tool.mina.packages.avilla.project]
 name = "arclet-alconna-avilla"
-version = "0.13.0rc1"
+version = "0.13.0rc2"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "avilla-core>=1.0.0a5",
 ]
 description = "Support Alconna to GraiaProject/Avilla"
@@ -191,20 +191,20 @@
 repository = "https://github.com/ArcletProject/Alconna-Graia"
 
 [tool.mina.packages.ichika]
 includes = [
     "src/arclet/alconna/ichika",
 ]
 raw-dependencies = [
-    "arclet-alconna-graia<0.13.0, >= 0.13.0rc1",
+    "arclet-alconna-graia<0.13.0, >= 0.13.0rc2",
 ]
 
 [tool.mina.packages.ichika.project]
 name = "arclet-alconna-ichika"
-version = "0.13.0rc1"
+version = "0.13.0rc2"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "ichika>=0.0.5",
 ]
 description = "Support Alconna to BlueGlassBlock/Ichika"
```

### Comparing `arclet-alconna-ichika-0.13.0rc1/README.md` & `arclet-alconna-ichika-0.13.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ichika-0.13.0rc1/src/arclet/alconna/ichika/adapter.py` & `arclet-alconna-ichika-0.13.0rc2/src/arclet/alconna/ichika/adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from contextlib import suppress
 from typing import Any, Callable, Iterable
 
+from graia.broadcast.interrupt import Waiter
 from ichika.client import Client
 from ichika.graia import IchikaClientDispatcher, CLIENT_INSTANCE
 from ichika.graia.event import GroupMessage, FriendMessage, MessageEvent
 from ichika.message.elements import At, Text
 from ichika.core import Friend
 from graia.amnesia.message import MessageChain
 from graia.broadcast.builtin.decorators import Depend
@@ -16,14 +17,15 @@
 
 from arclet.alconna import Arparma, argv_config
 
 from ..graia import AlconnaProperty, AlconnaSchema
 from ..graia.argv import MessageChainArgv
 from ..graia.adapter import AlconnaGraiaAdapter
 from ..graia.dispatcher import AlconnaDispatcher, AlconnaOutputMessage
+from ..graia.model import TSource
 from ..graia.utils import listen
 
 AlconnaDispatcher.default_send_handler = lambda x: MessageChain([Text(x)])
 
 
 def resolve_dispatchers_mixin(dispatchers: Iterable[T_Dispatcher]) -> list[T_Dispatcher]:
     """解析 dispatcher list 的 mixin
@@ -37,14 +39,23 @@
     result = []
     for dispatcher in dispatchers:
         result.extend(dispatcher_mixin_handler(dispatcher))
     return result
 
 
 class AlconnaIchikaAdapter(AlconnaGraiaAdapter[MessageEvent]):
+    def completion_waiter(self, interface: DispatcherInterface[TSource], priority: int = 15) -> Waiter:
+        @Waiter.create_using_function(
+            [interface.event.__class__], block_propagation=True, priority=priority,
+        )
+        async def waiter(m: MessageChain):
+            return m
+
+        return waiter  # type: ignore
+
     async def lookup_source(self, interface: DispatcherInterface[MessageEvent]) -> MessageChain:
         return await interface.lookup_param("__message_chain__", MessageChain, MessageChain([Text("Unknown")]))
 
     async def send(
         self,
         dispatcher: AlconnaDispatcher,
         result: Arparma[MessageChain],
```

### Comparing `arclet-alconna-ichika-0.13.0rc1/src/arclet/alconna/ichika/typings.py` & `arclet-alconna-ichika-0.13.0rc2/src/arclet/alconna/ichika/typings.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ichika-0.13.0rc1/PKG-INFO` & `arclet-alconna-ichika-0.13.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-ichika
-Version: 0.13.0rc1
+Version: 0.13.0rc2
 Summary: Support Alconna to BlueGlassBlock/Ichika
 License: AGPL-3.0
 Keywords: alconna,graia,arclet,ichika
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

