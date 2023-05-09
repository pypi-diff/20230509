# Comparing `tmp/arclet-alconna-ariadne-0.13.0rc1.tar.gz` & `tmp/arclet-alconna-ariadne-0.13.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-ariadne-0.13.0rc1.tar", last modified: Tue May  9 04:22:41 2023, max compression
+gzip compressed data, was "arclet-alconna-ariadne-0.13.0rc2.tar", last modified: Tue May  9 04:37:07 2023, max compression
```

## Comparing `arclet-alconna-ariadne-0.13.0rc1.tar` & `arclet-alconna-ariadne-0.13.0rc2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet-alconna-ariadne-0.13.0rc1/LICENSE
--rw-r--r--   0        0        0     6195 2023-05-09 04:02:48.655669 arclet-alconna-ariadne-0.13.0rc1/pyproject.toml
--rw-r--r--   0        0        0     7138 2023-01-30 09:01:24.879470 arclet-alconna-ariadne-0.13.0rc1/README.md
--rw-r--r--   0        0        0       81 2023-02-20 07:51:15.898481 arclet-alconna-ariadne-0.13.0rc1/src/arclet/alconna/ariadne/__init__.py
--rw-r--r--   0        0        0     5307 2023-05-09 04:13:04.624885 arclet-alconna-ariadne-0.13.0rc1/src/arclet/alconna/ariadne/adapter.py
--rw-r--r--   0        0        0     1262 2023-05-08 17:03:36.101915 arclet-alconna-ariadne-0.13.0rc1/src/arclet/alconna/ariadne/typings.py
--rw-r--r--   0        0        0     7584 1970-01-01 00:00:00.000000 arclet-alconna-ariadne-0.13.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet-alconna-ariadne-0.13.0rc2/LICENSE
+-rw-r--r--   0        0        0     6195 2023-05-09 04:32:45.106719 arclet-alconna-ariadne-0.13.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     7138 2023-01-30 09:01:24.879470 arclet-alconna-ariadne-0.13.0rc2/README.md
+-rw-r--r--   0        0        0       81 2023-02-20 07:51:15.898481 arclet-alconna-ariadne-0.13.0rc2/src/arclet/alconna/ariadne/__init__.py
+-rw-r--r--   0        0        0     5673 2023-05-09 04:36:47.505120 arclet-alconna-ariadne-0.13.0rc2/src/arclet/alconna/ariadne/adapter.py
+-rw-r--r--   0        0        0     1262 2023-05-08 17:03:36.101915 arclet-alconna-ariadne-0.13.0rc2/src/arclet/alconna/ariadne/typings.py
+-rw-r--r--   0        0        0     7584 1970-01-01 00:00:00.000000 arclet-alconna-ariadne-0.13.0rc2/PKG-INFO
```

### Comparing `arclet-alconna-ariadne-0.13.0rc1/LICENSE` & `arclet-alconna-ariadne-0.13.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ariadne-0.13.0rc1/pyproject.toml` & `arclet-alconna-ariadne-0.13.0rc2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arclet-alconna-ariadne"
-version = "0.13.0rc1"
+version = "0.13.0rc2"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "graia-ariadne<1.0.0,>=0.7.14",
 ]
 description = "Support Alconna to GraiaProject/Ariadne"
@@ -55,29 +55,29 @@
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
@@ -107,20 +107,20 @@
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
@@ -148,20 +148,20 @@
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
@@ -190,20 +190,20 @@
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

### Comparing `arclet-alconna-ariadne-0.13.0rc1/README.md` & `arclet-alconna-ariadne-0.13.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ariadne-0.13.0rc1/src/arclet/alconna/ariadne/adapter.py` & `arclet-alconna-ariadne-0.13.0rc2/src/arclet/alconna/ariadne/adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,31 +6,37 @@
 from graia.ariadne.app import Ariadne
 from graia.ariadne.dispatcher import ContextDispatcher
 from graia.ariadne.event.message import FriendMessage, GroupMessage, MessageEvent
 from graia.ariadne.message.chain import MessageChain
 from graia.ariadne.message.element import At, Plain
 from graia.ariadne.model import Friend
 from graia.ariadne.util import resolve_dispatchers_mixin
+from graia.ariadne.util.interrupt import AnnotationWaiter
 from graia.broadcast.builtin.decorators import Depend
 from graia.broadcast.exceptions import ExecutionStop
 from graia.broadcast.interfaces.dispatcher import DispatcherInterface
+from graia.broadcast.interrupt import Waiter
 from graia.broadcast.utilles import run_always_await
 
 from arclet.alconna import Arparma, argv_config
 
 from ..graia import AlconnaProperty, AlconnaSchema
 from ..graia.argv import MessageChainArgv
 from ..graia.adapter import AlconnaGraiaAdapter
 from ..graia.dispatcher import AlconnaDispatcher, AlconnaOutputMessage
+from ..graia.model import TSource
 from ..graia.utils import listen
 
 AlconnaDispatcher.default_send_handler = lambda x: MessageChain([Plain(x)])
 
 
 class AlconnaAriadneAdapter(AlconnaGraiaAdapter[MessageEvent]):
+    def completion_waiter(self, interface: DispatcherInterface[TSource], priority: int = 15) -> Waiter:
+        return AnnotationWaiter(MessageChain, [interface.event.__class__], block_propagation=True, priority=priority)
+
     async def lookup_source(self, interface: DispatcherInterface[MessageEvent]) -> MessageChain:
         return await interface.lookup_param("__message_chain__", MessageChain, MessageChain("Unknown"))
 
     async def send(
         self,
         dispatcher: AlconnaDispatcher,
         result: Arparma[MessageChain],
```

### Comparing `arclet-alconna-ariadne-0.13.0rc1/src/arclet/alconna/ariadne/typings.py` & `arclet-alconna-ariadne-0.13.0rc2/src/arclet/alconna/ariadne/typings.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ariadne-0.13.0rc1/PKG-INFO` & `arclet-alconna-ariadne-0.13.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-ariadne
-Version: 0.13.0rc1
+Version: 0.13.0rc2
 Summary: Support Alconna to GraiaProject/Ariadne
 License: AGPL-3.0
 Keywords: alconna,graia,arclet
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

