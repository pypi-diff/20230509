# Comparing `tmp/arclet-alconna-ariadne-0.12.2.tar.gz` & `tmp/arclet-alconna-ariadne-0.13.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-ariadne-0.12.2.tar", last modified: Thu Mar 16 13:13:35 2023, max compression
+gzip compressed data, was "arclet-alconna-ariadne-0.13.0rc1.tar", last modified: Tue May  9 04:22:41 2023, max compression
```

## Comparing `arclet-alconna-ariadne-0.12.2.tar` & `arclet-alconna-ariadne-0.13.0rc1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet-alconna-ariadne-0.12.2/LICENSE
--rw-r--r--   0        0        0     5080 2023-03-16 13:09:47.631022 arclet-alconna-ariadne-0.12.2/pyproject.toml
--rw-r--r--   0        0        0     7138 2023-01-30 09:01:24.879470 arclet-alconna-ariadne-0.12.2/README.md
--rw-r--r--   0        0        0       81 2023-02-20 07:51:15.898481 arclet-alconna-ariadne-0.12.2/src/arclet/alconna/ariadne/__init__.py
--rw-r--r--   0        0        0     5145 2023-03-16 12:15:30.937377 arclet-alconna-ariadne-0.12.2/src/arclet/alconna/ariadne/adapter.py
--rw-r--r--   0        0        0     1250 2023-01-20 16:49:08.207930 arclet-alconna-ariadne-0.12.2/src/arclet/alconna/ariadne/typings.py
--rw-r--r--   0        0        0     7581 1970-01-01 00:00:00.000000 arclet-alconna-ariadne-0.12.2/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet-alconna-ariadne-0.13.0rc1/LICENSE
+-rw-r--r--   0        0        0     6195 2023-05-09 04:02:48.655669 arclet-alconna-ariadne-0.13.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     7138 2023-01-30 09:01:24.879470 arclet-alconna-ariadne-0.13.0rc1/README.md
+-rw-r--r--   0        0        0       81 2023-02-20 07:51:15.898481 arclet-alconna-ariadne-0.13.0rc1/src/arclet/alconna/ariadne/__init__.py
+-rw-r--r--   0        0        0     5307 2023-05-09 04:13:04.624885 arclet-alconna-ariadne-0.13.0rc1/src/arclet/alconna/ariadne/adapter.py
+-rw-r--r--   0        0        0     1262 2023-05-08 17:03:36.101915 arclet-alconna-ariadne-0.13.0rc1/src/arclet/alconna/ariadne/typings.py
+-rw-r--r--   0        0        0     7584 1970-01-01 00:00:00.000000 arclet-alconna-ariadne-0.13.0rc1/PKG-INFO
```

### Comparing `arclet-alconna-ariadne-0.12.2/LICENSE` & `arclet-alconna-ariadne-0.13.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ariadne-0.12.2/README.md` & `arclet-alconna-ariadne-0.13.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ariadne-0.12.2/src/arclet/alconna/ariadne/adapter.py` & `arclet-alconna-ariadne-0.13.0rc1/src/arclet/alconna/ariadne/adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,47 +11,49 @@
 from graia.ariadne.model import Friend
 from graia.ariadne.util import resolve_dispatchers_mixin
 from graia.broadcast.builtin.decorators import Depend
 from graia.broadcast.exceptions import ExecutionStop
 from graia.broadcast.interfaces.dispatcher import DispatcherInterface
 from graia.broadcast.utilles import run_always_await
 
-from arclet.alconna import Arparma
+from arclet.alconna import Arparma, argv_config
 
 from ..graia import AlconnaProperty, AlconnaSchema
+from ..graia.argv import MessageChainArgv
 from ..graia.adapter import AlconnaGraiaAdapter
-from ..graia.analyser import MessageChainContainer
 from ..graia.dispatcher import AlconnaDispatcher, AlconnaOutputMessage
 from ..graia.utils import listen
 
+AlconnaDispatcher.default_send_handler = lambda x: MessageChain([Plain(x)])
+
 
 class AlconnaAriadneAdapter(AlconnaGraiaAdapter[MessageEvent]):
     async def lookup_source(self, interface: DispatcherInterface[MessageEvent]) -> MessageChain:
         return await interface.lookup_param("__message_chain__", MessageChain, MessageChain("Unknown"))
 
     async def send(
         self,
         dispatcher: AlconnaDispatcher,
         result: Arparma[MessageChain],
         output_text: str | None = None,
         source: MessageEvent | None = None,
+        exclude: bool = True,
     ) -> AlconnaProperty[MessageEvent]:
         if not isinstance(source, MessageEvent) or (result.matched or not output_text):
             return AlconnaProperty(result, None, source)
-        id_ = str(source.source.id) if source else '_'
-        cache = self.output_cache.setdefault(id_, set())
-        if dispatcher.command in cache:
-            return AlconnaProperty(result, None, source)
-        cache.clear()
-        cache.add(dispatcher.command)
+        if exclude:
+            id_ = str(source.source.id) if source else '_'
+            cache = self.output_cache.setdefault(id_, set())
+            if dispatcher.command in cache:
+                return AlconnaProperty(result, None, source)
+            cache.clear()
+            cache.add(dispatcher.command)
         if dispatcher.send_flag == "stay":
             return AlconnaProperty(result, output_text, source)
         if dispatcher.send_flag == "reply":
-            from graia.ariadne.app import Ariadne
-
             app: Ariadne = Ariadne.current()
             help_message: MessageChain = await run_always_await(dispatcher.converter, output_text)
             if isinstance(source, GroupMessage):
                 await app.send_group_message(source.sender.group, help_message)
             else:
                 await app.send_message(source.sender, help_message)  # type: ignore
         elif dispatcher.send_flag == "post":
@@ -105,12 +107,14 @@
             buffer.setdefault("dispatchers", []).append(dispatcher)
             listen(*events)(func)  # noqa
             return AlconnaSchema(dispatcher.command)
 
         return wrapper
 
 
-MessageChainContainer.config(
-    filter_out=["Source", "File", "Quote"]
+argv_config(
+    target=MessageChainArgv,
+    filter_out=["Source", "File", "Quote"],
+    checker=lambda x: isinstance(x, MessageChain),
+    to_text=lambda x: x.text if x.__class__ is Plain else None,
+    converter=lambda x: MessageChain(x)
 )
-MessageChainContainer.__message_chain_class__ = MessageChain
-MessageChainContainer.__text_element_class__ = Plain
```

### Comparing `arclet-alconna-ariadne-0.12.2/src/arclet/alconna/ariadne/typings.py` & `arclet-alconna-ariadne-0.13.0rc1/src/arclet/alconna/ariadne/typings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from nepattern import (
     URL,
     BasePattern,
     PatternModel,
-    UnionArg,
+    UnionPattern,
 )
 from nepattern.main import INTEGER
 from graia.ariadne.message.element import Image, At
 
 ImgOrUrl = (
-    UnionArg(
+    UnionPattern(
         [
             BasePattern(
                 model=PatternModel.TYPE_CONVERT,
                 origin=str,
                 converter=lambda _, x: x.url,
                 alias="img",
                 accepts=[Image],
@@ -23,15 +23,15 @@
     @ "img_url"
 )
 """
 内置类型, 允许传入图片元素(Image)或者链接(URL)，返回链接
 """
 
 AtID = (
-    UnionArg(
+    UnionPattern(
         [
             BasePattern(
                 model=PatternModel.TYPE_CONVERT,
                 origin=int,
                 alias="At",
                 accepts=[At],
                 converter=lambda _, x: x.target,
```

### Comparing `arclet-alconna-ariadne-0.12.2/PKG-INFO` & `arclet-alconna-ariadne-0.13.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-ariadne
-Version: 0.12.2
+Version: 0.13.0rc1
 Summary: Support Alconna to GraiaProject/Ariadne
 License: AGPL-3.0
 Keywords: alconna,graia,arclet
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

