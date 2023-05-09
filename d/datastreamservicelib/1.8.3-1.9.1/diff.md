# Comparing `tmp/datastreamservicelib-1.8.3.tar.gz` & `tmp/datastreamservicelib-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datastreamservicelib-1.8.3.tar", last modified: Mon Feb  8 19:37:28 2021, max compression
+gzip compressed data, was "datastreamservicelib-1.9.1.tar", last modified: Wed Feb 24 03:54:50 2021, max compression
```

## Comparing `datastreamservicelib-1.8.3.tar` & `datastreamservicelib-1.9.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1063 2021-02-08 19:37:27.915982 datastreamservicelib-1.8.3/LICENSE
--rw-r--r--   0        0        0      790 2021-02-08 19:37:27.915982 datastreamservicelib-1.8.3/README.rst
--rw-r--r--   0        0        0     1604 2021-02-08 19:37:27.915982 datastreamservicelib-1.8.3/pyproject.toml
--rw-r--r--   0        0        0      192 2021-02-08 19:37:27.915982 datastreamservicelib-1.8.3/src/datastreamservicelib/__init__.py
--rw-r--r--   0        0        0     5571 2021-02-08 19:37:27.915982 datastreamservicelib-1.8.3/src/datastreamservicelib/console.py
--rw-r--r--   0        0        0        0 2021-02-08 19:37:27.915982 datastreamservicelib-1.8.3/src/datastreamservicelib/py.typed
--rw-r--r--   0        0        0     7957 2021-02-08 19:37:27.915982 datastreamservicelib-1.8.3/src/datastreamservicelib/service.py
--rw-r--r--   0        0        0     7870 2021-02-08 19:37:27.915982 datastreamservicelib-1.8.3/src/datastreamservicelib/zmqwrappers.py
--rw-r--r--   0        0        0     2053 2021-02-08 19:37:28.633372 datastreamservicelib-1.8.3/setup.py
--rw-r--r--   0        0        0     1736 2021-02-08 19:37:28.633779 datastreamservicelib-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2021-02-24 03:54:48.953038 datastreamservicelib-1.9.1/LICENSE
+-rw-r--r--   0        0        0     4055 2021-02-24 03:54:48.953038 datastreamservicelib-1.9.1/README.rst
+-rw-r--r--   0        0        0     1657 2021-02-24 03:54:48.953038 datastreamservicelib-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0      192 2021-02-24 03:54:48.953038 datastreamservicelib-1.9.1/src/datastreamservicelib/__init__.py
+-rw-r--r--   0        0        0      695 2021-02-24 03:54:48.953038 datastreamservicelib-1.9.1/src/datastreamservicelib/compat.py
+-rw-r--r--   0        0        0     5571 2021-02-24 03:54:48.957039 datastreamservicelib-1.9.1/src/datastreamservicelib/console.py
+-rw-r--r--   0        0        0        0 2021-02-24 03:54:48.957039 datastreamservicelib-1.9.1/src/datastreamservicelib/py.typed
+-rw-r--r--   0        0        0    10574 2021-02-24 03:54:48.957039 datastreamservicelib-1.9.1/src/datastreamservicelib/service.py
+-rw-r--r--   0        0        0     7870 2021-02-24 03:54:48.957039 datastreamservicelib-1.9.1/src/datastreamservicelib/zmqwrappers.py
+-rw-r--r--   0        0        0     5405 2021-02-24 03:54:50.124558 datastreamservicelib-1.9.1/setup.py
+-rw-r--r--   0        0        0     5001 2021-02-24 03:54:50.125121 datastreamservicelib-1.9.1/PKG-INFO
```

### Comparing `datastreamservicelib-1.8.3/LICENSE` & `datastreamservicelib-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datastreamservicelib-1.8.3/pyproject.toml` & `datastreamservicelib-1.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datastreamservicelib"
-version = "1.8.3"
+version = "1.9.1"
 description = ""
 authors = ["Eero af Heurlin <eero.afheurlin@iki.fi>"]
 homepage = "https://gitlab.com/advian-oss/python-datastreamservicelib/"
 repository = "https://gitlab.com/advian-oss/python-datastreamservicelib/"
 license = "MIT"
 readme = "README.rst"
 
@@ -37,14 +37,17 @@
 [tool.pytest.ini_options]
 junit_family="xunit2"
 addopts="--cov=datastreamservicelib --cov-fail-under=65 --cov-branch"
 
 [tool.pylint.format]
 max-line-length = 120
 
+[tool.pylint.similarities]
+min-similarity-lines = 8
+
 [tool.pylint.messages_control]
 disable=["fixme", "W1202"]
 
 [tool.coverage.run]
 omit = ["tests/*"]
 branch = true
```

### Comparing `datastreamservicelib-1.8.3/src/datastreamservicelib/console.py` & `datastreamservicelib-1.9.1/src/datastreamservicelib/console.py`

 * *Files identical despite different names*

### Comparing `datastreamservicelib-1.8.3/src/datastreamservicelib/service.py` & `datastreamservicelib-1.9.1/src/datastreamservicelib/service.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Baseclasses for services using asyncio as eventloop"""
-from typing import Union, MutableMapping, Any, Optional
+from typing import Union, MutableMapping, Any, Coroutine, Optional
 from pathlib import Path
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 import tempfile
 import logging
+import functools
 
 import signal as posixsignal
 import asyncio
 import toml
 
 from datastreamcorelib.abstract import ZMQSocketType, ZMQSocketDescription
 from datastreamcorelib.utils import create_heartbeat_message
 
 
 from .zmqwrappers import PubSubManager, pubsubmanager_factory
+from .compat import cast_task
 
 LOGGER = logging.getLogger(__name__)
 EXCEPTION_EXITCODE = 200
 SIGNALS_HOOKED = False
 
 
 # See https://github.com/python/mypy/issues/5374 why the typing ignore
@@ -126,15 +128,50 @@
 @dataclass
 class SimpleServiceMixin:
     """Mixin for a bit of automagics for heartbeats, config loading etc"""
 
     configpath: Path
     psmgr: PubSubManager = field(init=False, default_factory=pubsubmanager_factory)
     config: MutableMapping[str, Any] = field(init=False, default_factory=dict)
-    _hbtask: Optional["asyncio.Task[Any]"] = field(init=False, default=None)
+    _tasks: MutableMapping[str, "asyncio.Task[Any]"] = field(init=False, default_factory=dict)
+
+    def create_task(self, coro: Coroutine[Any, Any, Any], *, name: Optional[str] = None) -> "asyncio.Task[Any]":
+        """Helper to wrap asyncios create_task so that we always handle the exception and track long-running tasks"""
+        task = asyncio.get_event_loop().create_task(coro)
+        if name:
+            if name in self._tasks:
+                raise ValueError(f"name {name} is already tracked")
+        else:
+            name = f"Task-{id(task):02x}"
+
+        task = cast_task(task)
+        try:
+            task.set_name(name)
+        except AttributeError:
+            # Ignore the missing method in py36 and add the get_name wrapper
+            task.get_name = functools.partial(lambda retname: retname, name)  # type: ignore
+
+        def report_error_remove_tracking(task: "asyncio.Task[Any]") -> None:
+            """done callback to bubble up errors and remove tracking"""
+            # Remove from tracking (we monkeypatched get_name above)
+            task = cast_task(task)
+            name = task.get_name()
+            del self._tasks[name]
+            # Bubble up any exceptions
+            try:
+                exc = task.exception()
+                if exc:
+                    LOGGER.error("Task {} raised exception {}".format(task, exc))
+                    raise exc
+            except asyncio.CancelledError:
+                LOGGER.error("Task {} did not handle cancellation".format(task))
+
+        self._tasks[name] = task
+        task.add_done_callback(report_error_remove_tracking)
+        return task
 
     async def _heartbeat_task(self) -> None:
         """Send a periodic heartbeat"""
         try:
             while self.psmgr.default_pub_socket and not self.psmgr.default_pub_socket.closed:
                 await self.psmgr.publish_async(create_heartbeat_message())
                 await asyncio.sleep(1)
@@ -151,44 +188,63 @@
         sdesc = ZMQSocketDescription(pub_default, ZMQSocketType.PUB)
         sock = self.psmgr.sockethandler.get_socket(sdesc)
         LOGGER.debug("Setting psmgr@{} default pub socket to {} (sdesc={})".format(hex(id(self.psmgr)), sock, sdesc))
         self.psmgr.default_pub_socket = sock
 
     async def _stop_hbtask_graceful(self) -> None:
         """Stops the hb task if it's active"""
-        if not self._hbtask:
+        if "HEARTBEAT" not in self._tasks:
             return
-        try:
-            if self._hbtask.done():
-                # get the exception if there was any
-                await self._hbtask
-                return
-            self._hbtask.cancel()
-            await self._hbtask
-        except asyncio.CancelledError:
-            LOGGER.warning("got CancelledError even though the task should have handled it")
-        finally:
-            self._hbtask = None
+        await self.stop_named_task_graceful("HEARTBEAT")
 
     async def _restart_hb_task(self) -> None:
         """Stop and recreate hb task"""
         await self._stop_hbtask_graceful()
-        self._hbtask = asyncio.get_event_loop().create_task(self._heartbeat_task())
+        self.create_task(self._heartbeat_task(), name="HEARTBEAT")
 
     def reload(self) -> None:
         """Load configs, restart sockets"""
         self.psmgr.sockethandler.close_all_sockets()
         with self.configpath.open("rt", encoding="utf-8") as filepntr:
             self.config = toml.load(filepntr)
         self._resolve_default_pub_socket()
-        asyncio.get_event_loop().create_task(self._restart_hb_task())
+        self.create_task(self._restart_hb_task())
+
+    async def stop_named_task_graceful(self, taskname: str) -> Optional[Any]:
+        """cancel the named task if it is running and return the result"""
+        if taskname not in self._tasks:
+            LOGGER.warning("task {} not found".format(taskname), stack_info=True)
+            return None
+        task = self._tasks[taskname]
+        return await self.stop_task_graceful(task)
+
+    async def stop_task_graceful(self, task: "asyncio.Task[Any]") -> Any:
+        """cancel the given task if it is running and return the result"""
+        if not task.done():
+            LOGGER.info("Cancelling task {}".format(task))
+            task.cancel()
+        try:
+            return await task
+        except asyncio.CancelledError:
+            LOGGER.error("Task {} did not handle cancellation".format(task))
+
+    async def stop_lingering_tasks(self) -> None:
+        """Stop all still lingering tasks and fetch their results"""
+        # we modify the dictionary during iteration, make a copy of the values
+        for task in list(self._tasks.values()):
+            try:
+                await self.stop_task_graceful(task)
+                LOGGER.info("Task {} stopped".format(task))
+            except Exception:  # pylint: disable=W0703
+                LOGGER.exception("Task {} returned exception".format(task))
 
     async def teardown(self) -> None:
-        """Close all sockets"""
+        """Stop all tasks, close all sockets"""
         await self._stop_hbtask_graceful()
+        await self.stop_lingering_tasks()
         self.psmgr.sockethandler.close_all_sockets()
 
 
 @dataclass
 class SimpleService(SimpleServiceMixin, BaseService):
     """Simple service does a bit of automagics in setup"""
```

### Comparing `datastreamservicelib-1.8.3/src/datastreamservicelib/zmqwrappers.py` & `datastreamservicelib-1.9.1/src/datastreamservicelib/zmqwrappers.py`

 * *Files identical despite different names*

