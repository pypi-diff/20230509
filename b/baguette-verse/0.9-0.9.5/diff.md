# Comparing `tmp/baguette_verse-0.9.tar.gz` & `tmp/baguette_verse-0.9.5.tar.gz`

## Comparing `baguette_verse-0.9.tar` & `baguette_verse-0.9.5.tar`

### file list

```diff
@@ -1,42 +1,66 @@
--rw-r--r--   0        0        0    22934 2020-02-02 00:00:00.000000 baguette_verse-0.9/bake.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 baguette_verse-0.9/metalib.py
--rw-r--r--   0        0        0    19314 2020-02-02 00:00:00.000000 baguette_verse-0.9/toast.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/__init__.py
--rw-r--r--   0        0        0    21861 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/rack.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/__init__.py
--rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/call_archiver.py
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/compiler.py
--rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/cuckoo_api_list.md
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/find_sample.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/logger.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/source/__init__.py
--rw-r--r--   0        0        0    12971 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/source/build.py
--rw-r--r--   0        0        0    15989 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/source/colors.py
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/source/config.py
--rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/source/database.py
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/source/event.py
--rw-r--r--   0        0        0     9276 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/source/filters.py
--rw-r--r--   0        0        0    34169 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/source/graph.py
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/source/record.py
--rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/source/utils.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/source/types/__init__.py
--rw-r--r--   0        0        0    33526 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/source/types/data.py
--rw-r--r--   0        0        0    18209 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/source/types/execution.py
--rw-r--r--   0        0        0    22279 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/source/types/filesystem.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/source/types/imports.py
--rw-r--r--   0        0        0    23975 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/source/types/network.py
--rw-r--r--   0        0        0    27885 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/bakery/source/types/registry.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/croutons/__init__.py
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/croutons/extractor.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/croutons/metalib/__init__.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/croutons/metalib/evaluator.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/croutons/metalib/interact.py
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/croutons/metalib/utils.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/croutons/source/__init__.py
--rw-r--r--   0        0        0    33339 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/croutons/source/metagraph.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 baguette_verse-0.9/baguette/croutons/source/utils.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 baguette_verse-0.9/.gitignore
--rw-r--r--   0        0        0    35123 2020-02-02 00:00:00.000000 baguette_verse-0.9/LICENSE
--rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 baguette_verse-0.9/README.md
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 baguette_verse-0.9/pyproject.toml
--rw-r--r--   0        0        0    48651 2020-02-02 00:00:00.000000 baguette_verse-0.9/PKG-INFO
+-rw-r--r--   0        0        0    22934 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/bake.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/metalib.py
+-rw-r--r--   0        0        0    19314 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/toast.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/__init__.py
+-rw-r--r--   0        0        0    21861 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/rack.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/__init__.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/compiler.py
+-rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/cuckoo_api_list.md
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/logger.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/__init__.py
+-rw-r--r--   0        0        0    13059 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/build.py
+-rw-r--r--   0        0        0    16047 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/colors.py
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/config.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/event.py
+-rw-r--r--   0        0        0     9276 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/filters.py
+-rw-r--r--   0        0        0    32413 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/graph.py
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/record.py
+-rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/utils.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/__init__.py
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/utils.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/data/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/data/__proc__.py
+-rw-r--r--   0        0        0    13178 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/data/entities.py
+-rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/data/integration.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/data/relations.py
+-rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/data/utils.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/execution/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/execution/__proc__.py
+-rw-r--r--   0        0        0     9835 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/execution/entities.py
+-rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/execution/integration.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/execution/relations.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/execution/utils.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/filesystem/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/filesystem/__proc__.py
+-rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/filesystem/entities.py
+-rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/filesystem/integration.py
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/filesystem/relations.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/imports/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/imports/__proc__.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/imports/entities.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/imports/integration.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/imports/relations.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/network/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/network/__proc__.py
+-rw-r--r--   0        0        0    10216 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/network/entities.py
+-rw-r--r--   0        0        0     9921 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/network/integration.py
+-rw-r--r--   0        0        0     5198 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/network/relations.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/registry/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/registry/__proc__.py
+-rw-r--r--   0        0        0    10597 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/registry/entities.py
+-rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/registry/integration.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/registry/relations.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/croutons/__init__.py
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/croutons/extractor.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/croutons/metalib/__init__.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/croutons/metalib/evaluator.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/croutons/metalib/interact.py
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/croutons/metalib/utils.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/croutons/source/__init__.py
+-rw-r--r--   0        0        0    31599 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/croutons/source/metagraph.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/croutons/source/utils.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/.gitignore
+-rw-r--r--   0        0        0    35123 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/LICENSE
+-rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/README.md
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0    48653 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/PKG-INFO
```

### Comparing `baguette_verse-0.9/bake.py` & `baguette_verse-0.9.5/bake.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9/toast.py` & `baguette_verse-0.9.5/toast.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9/baguette/rack.py` & `baguette_verse-0.9.5/baguette/rack.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9/baguette/bakery/compiler.py` & `baguette_verse-0.9.5/baguette/bakery/compiler.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9/baguette/bakery/cuckoo_api_list.md` & `baguette_verse-0.9.5/baguette/bakery/cuckoo_api_list.md`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9/baguette/bakery/logger.py` & `baguette_verse-0.9.5/baguette/bakery/logger.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9/baguette/bakery/source/build.py` & `baguette_verse-0.9.5/baguette/bakery/source/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from io import IOBase
 from ..logger import logger
-from typing import Dict, Iterator, List, Type, TypeVar
-from ..source.utils import *
-from ..source.graph import Graph
-from ..source.event import Event
+from typing import Any, Dict, Iterator, TypeVar
+from .utils import *
+from .graph import Graph
+from .event import Event
+from .types.execution.entities import Process, Call
 import os
 from threading import Lock
 
 
 
 
 
@@ -59,16 +60,16 @@
     def __init__(self, data : str | IOBase | dict) -> None:
         if isinstance(data, str):
             try:
                 data = open(data, "r")
             except:
                 raise 
         if isinstance(data, IOBase):
+            from json import load, JSONDecodeError
             try:
-                from json import load, JSONDecodeError
                 data = load(data)
                 logger.info("File loaded and structured.")
             except JSONDecodeError:
                 data = {}
                 logger.error("JSON file has strutural problems.")
         if not isinstance(data, dict):
             raise TypeError("Expected dict or json file, got " + repr(data.__class__.__name__))
@@ -105,15 +106,16 @@
         Returns the host machine's IP address.
         """
         import re
         expr = re.compile(r"\[cuckoo.core.resultserver\] DEBUG: Now tracking machine (\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}) for task #\d+\n")
         for line in self.data["debug"]["cuckoo"]:
             if expr.search(line):
                 match = expr.search(line)
-                return match.group(1)
+                if match:
+                    return match.group(1)
         logger.warning("Could not find the host's IP address.")
         return ""
     
     def sample_file_path(self) -> str:
         """
         Finds the name of the sample file in the report and returns its absolute path in the execution environment.
         """
@@ -131,23 +133,23 @@
                     return p.executable
         raise RuntimeError("Could not find malware process")
         
 
     @chrono
     def build(self) -> None:
         BuildingPhase("Initialization", 0).throw()
-        from ..source.graph import Graph
-        from ..source.types.execution import Thread, Call, FollowedBy, Process, NextSignificantCall
-        from ..source.types.network import Host, SpawnedProcess
-        from ..source.types.filesystem import File, declare_existing_file
-        from ..source.graph import find_or_create
+        from .graph import Graph
+        from .types.execution import Thread, Call, FollowedBy, Process, NextSignificantCall
+        from .types.network import Host, SpawnedProcess
+        from .types.filesystem.integration import declare_existing_file
+        from .graph import find_or_create
+        from .types.execution.utils import CallHandler
         self.graph = Graph()
 
         with self.graph:
-            self.machine : Host = None
 
             BuildingPhase("Network Discovery", 0).throw()
             logger.info("Identifying machines.")
 
             for machine in self.machines():
                 h = Host()
                 h.address = machine["ip"]
@@ -211,15 +213,15 @@
             logger.info("Sorting calls based on time.")
             calls.sort(key = lambda a : a.time)
 
             # Interpreting each Call
             BuildingPhase("Call Interpretation", 0).throw()
             logger.info("Integrating {} calls.".format(N_calls))
             for a in calls:
-                a.integrate()
+                CallHandler.integrate_chain(a)
                 self._progress += 1
             
             # Linking processes to host
             BuildingPhase("Process Attribution", 0).throw()
             logger.info("Linking root processes to host machine.")
             p : Process
             for p in Process:
@@ -228,15 +230,15 @@
             
             # Making skip links
             BuildingPhase("Call Skip-Linking", 0).throw()
             logger.info("Adding skip links in system call sequences")
             for t in Thread:
                 last = t.first
                 new = last
-                while new != None:
+                while new and last:
                     if new is not last:
                         for l in new.edges:
                             if not isinstance(l, FollowedBy):
                                 NextSignificantCall(last, new)
                                 last = new
                                 break
                     next_call = None
@@ -253,17 +255,17 @@
 
     @chrono
     def flush_graph(self):
 
         logger.info("Flushing graph.")
 
         from ..source.graph import Vertex, UniqueVertex, Edge, Arrow
-        Self = TypeVar("Self")
+        Self = TypeVar("Self", bound = type)
 
-        def subclass_iterator(cls : Self) -> List[Type[Self]]:
+        def subclass_iterator(cls : Self) -> Iterator[Self]:
             for c in cls.__subclasses__():
                 yield c
                 for ci in subclass_iterator(c):
                     yield ci
         
         for cls in subclass_iterator(Vertex):
             if cls != UniqueVertex:
@@ -271,15 +273,15 @@
                 cls.add_vertices_to_graph(self.graph)
         for cls in subclass_iterator(Edge):
             if cls != Arrow:
                 logger.debug("Adding {} {} edges to the graph.".format(len(cls), cls.__name__))
                 cls.add_edges_to_graph(self.graph)
 
     @chrono
-    def process_to_vertex(self, process : dict) -> "Process":
+    def process_to_vertex(self, process : dict) -> Process:
         from ..source.graph import find_or_create
         from ..source.types.execution import Process, Thread, Call, HasChildProcess, HasThread, HasFirstCall, FollowedBy
         from ..source.types.imports import Import, HasImport
         p : Process
         t : Thread
         a : Call
         p, _ = find_or_create(Process, PID = process["pid"])
@@ -304,31 +306,32 @@
             a = self.api_to_vertex(ci)
             a.thread = t
             if t.first == None:
                 t.first = a
                 t.last = a
                 t.Ncalls = 1
                 HasFirstCall(t, a)
-            else:
+            elif t.last:
                 FollowedBy(t.last, a)
                 t.last = a
                 t.Ncalls += 1
             self._progress += 1
 
         for t in p.threads:
-            t.start = t.first.time
-            t.stop = t.last.time
+            if t.first and t.last:
+                t.start = t.first.time
+                t.stop = t.last.time
         
         p.start = min((t.start for t in p.threads), default=p.start)
         p.stop = max((t.stop for t in p.threads), default=p.start)
 
         return p
 
     @chrono
-    def api_to_vertex(self, call : dict) -> "Call":
+    def api_to_vertex(self, call : dict) -> Call:
         from ..source.record import record
         from ..source.types.execution import Call
         a = Call()
         a.name = call["api"]
         a.category = call["category"]
         a.stacktrace = tuple(call["stacktrace"])
         a.status = call["status"]
@@ -349,8 +352,8 @@
         b = Builder(file)
     except:
         raise TypeError("Expected file, got " + repr(file.__class__.__name__))
     b.build()
     return b.graph
 
 
-__all__ = ["Builder", "build", "os", "avg", "dev"]
+__all__ = ["Builder", "build"]
```

### Comparing `baguette_verse-0.9/baguette/bakery/source/colors.py` & `baguette_verse-0.9.5/baguette/bakery/source/colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 __all__ = ["chart", "Color"]
 
 
 
 
 
-chart = {
+__chart_init = {
     'black' : (0.0, 0.0, 0.0),
     'navy' : (0.0, 0.0, 0.5019607843137255),
     'darkblue' : (0.0, 0.0, 0.5450980392156862),
     'mediumblue' : (0.0, 0.0, 0.803921568627451),
     'blue' : (0.0, 0.0, 1.0),
     'darkgreen' : (0.0, 0.39215686274509803, 0.0),
     'green' : (0.0, 0.5019607843137255, 0.0),
@@ -148,25 +148,27 @@
     'snow' : (1.0, 0.9803921568627451, 0.9803921568627451),
     'yellow' : (1.0, 1.0, 0.0),
     'lightyellow' : (1.0, 1.0, 0.8784313725490196),
     'ivory' : (1.0, 1.0, 0.9411764705882353),
     'white' : (1.0, 1.0, 1.0)
 }
 
+chart : dict[str, "Color"] = {}
+
 
 
 
 
 class ColorType(type):
 
     """
     This is the class for the Color class. It allows to find colors by name.
     """
 
-    def __getattribute__(self, name: str) -> Any:
+    def __getattribute__(self, name: str) -> "Color":
         """
         Implements getattr(Color, name).
         """
         try:
             return super().__getattribute__(name)
         except AttributeError:
             if name in chart:
@@ -314,15 +316,14 @@
         return Color, (self.R, self.G, self.B)
     
     @staticmethod
     def average(*colors : "Color") -> "Color":
         """
         Returns the average of all the given colors.
         """
-        colors = list(colors)
         R, G, B = sum(c.R for c in colors), sum(c.G for c in colors), sum(c.B for c in colors)
         n = len(colors)
         return Color(R / n, G / n, B / n)
     
     @staticmethod
     def linear(colors : Iterable["Color"], weights : Iterable[float]) -> "Color":
         """
@@ -332,13 +333,11 @@
         R, G, B = sum(c.R * w for c, w in zip(colors, weights)), sum(c.G * w for c, w in zip(colors, weights)), sum(c.B * w for c, w in zip(colors, weights))
         return Color(min(1.0, max(0.0, R)), min(1.0, max(0.0, G)), min(1.0, max(0.0, B)))
 
 
 
 
 
-# To convert color vectors of the chart to Color objects
-
-for name, value in chart.items():
-    chart[name] = Color(*value)
+# Convert color vectors of the __chart_init to Color objects in the real chart
+chart.update((name, Color(*value)) for name, value in __chart_init.items())
 
-del Any, Tuple, Union, ColorType, Iterable
+del Any, Tuple, Union, ColorType, Iterable, __chart_init
```

### Comparing `baguette_verse-0.9/baguette/bakery/source/config.py` & `baguette_verse-0.9.5/baguette/bakery/source/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module contains configuration objects for execution graphs.
 """
 
-from typing import Any, Type
+from typing import Any
 from .colors import Color
 from .graph import Vertex, Edge
 from Viper.meta.decorators import hybridmethod
 
 
 
 
@@ -62,38 +62,38 @@
         UnprintableKey = Color(255, 0, 50)
         KeyEntry = Color(0, 255, 255)
         Handle = Color.white
 
     registry.Handle = Color.average(registry.Key, execution.Process)
 
     @hybridmethod
-    def get_color(self, cls : Type[Vertex] | Type[Edge]) -> Color:
+    def get_color(self, cls : type[Vertex] | type[Edge]) -> Color:
         """
         This function returns the color corresponding to the given class of Vertex or Edge.
         """
         from inspect import getmodule
         try:
             return getattr(getattr(self, getmodule(cls).__name__.split(".")[-1]), cls.__name__)
         except AttributeError:
             return self.default
     
     @hybridmethod
-    def has_color(self, cls : Type[Vertex] | Type[Edge]) -> bool:
+    def has_color(self, cls : type[Vertex] | type[Edge]) -> bool:
         """
         This function returns True if the given class of Vertex or Edge has a special color.
         """
         from inspect import getmodule
         try:
             getattr(getattr(self, getmodule(cls).__name__.split(".")[-1]), cls.__name__)
             return True
         except AttributeError:
             return False
         
     @staticmethod
-    def get_config() -> Type["ColorMap"] | "ColorMap":
+    def get_config():
         """
         Returns the globally set ColorMap configuration object.
         """
         return ColorMap.__current
     
     @hybridmethod
     def set_config(self):
@@ -143,38 +143,38 @@
     
     class registry:
         Key = 1.5
         KeyEntry = 1.0
         Handle = 1.0
 
     @hybridmethod
-    def get_size(self, cls : Type[Vertex]) -> float:
+    def get_size(self, cls : type[Vertex]) -> float:
         """
         This function returns the size corresponding to the given class of Vertex.
         """
         from inspect import getmodule
         try:
             return getattr(getattr(self, getmodule(cls).__name__.split(".")[-1]), cls.__name__)
         except AttributeError:
             return self.default
     
     @hybridmethod
-    def has_size(self, cls : Type[Vertex]) -> bool:
+    def has_size(self, cls : type[Vertex]) -> bool:
         """
         This function returns True if the given class of Vertex has a special size.
         """
         from inspect import getmodule
         try:
             getattr(getattr(self, getmodule(cls).__name__.split(".")[-1]), cls.__name__)
             return True
         except AttributeError:
             return False
         
     @staticmethod
-    def get_config() -> Type["SizeMap"] | "SizeMap":
+    def get_config():
         """
         Returns the globally set SizeMap configuration object.
         """
         return SizeMap.__current
     
     @hybridmethod
     def set_config(self):
@@ -219,15 +219,15 @@
         try:
             getattr(self, name)
             return True
         except AttributeError:
             return False
     
     @staticmethod
-    def get_config() -> Type["CompilationParameters"] | "CompilationParameters":
+    def get_config():
         """
         Returns the globally set CompilationParameters configuration object.
         """
         return CompilationParameters.__current
     
     @hybridmethod
     def set_config(self):
```

### Comparing `baguette_verse-0.9/baguette/bakery/source/event.py` & `baguette_verse-0.9.5/baguette/bakery/source/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,10 +116,13 @@
             try:
                 Event.__callbacks[cls].remove(callback)
                 return True
             except ValueError:
                 return False
 
 
+
+
+
 Event.__init_subclass__()       # It must initialize itself, as if it was one of its own subclasses.
 
 del Callable, Type, Future, Lock
```

### Comparing `baguette_verse-0.9/baguette/bakery/source/filters.py` & `baguette_verse-0.9.5/baguette/bakery/source/filters.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9/baguette/bakery/source/graph.py` & `baguette_verse-0.9.5/baguette/bakery/source/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 This module defines all graph-related objects.
 """
 
 from threading import RLock, Thread
 from typing import Any, Callable, Dict, Iterable, Iterator, Optional, Set, Tuple, Type, TypeVar, Union
 from .colors import Color
 from Viper.meta.iterable import InstanceReferencingClass
-from .utils import chrono
 
 __all__ = ["Vertex", "UniqueVertex", "Edge", "Arrow", "Graph", "find_or_create"]
 
 
 
 
 
@@ -43,24 +42,24 @@
         if not isinstance(c, Color):
             raise TypeError("Expected color for c, got " + repr(c.__class__.__name__))
         if parent != None and not isinstance(parent, Vertex):
             raise TypeError("Expected vertex for parent, got " + repr(parent.__class__.__name__))
         self.edges : Set[Edge] = set()
         self.color : Color = c
         self.__size : float = SizeMap.get_config().get_size(type(self))
-        self.parent : Vertex = parent
-        self.graph : Graph = None
+        self.parent : Vertex | None = parent
+        self.graph : Graph | None = None
         if parent:
             parent.children += (self, )
-        self.children : Tuple[Vertex] = ()
+        self.children : Tuple[Vertex, ...] = ()
         for g in Graph.active_graphs():
             g.vertices.add(self)
 
     __vertexing = False
-    __comparing : set[tuple["Vertex"]] = set()
+    __comparing : set[tuple["Vertex", ...]] = set()
 
     @property
     def label(self) -> str:
         """
         The label used when plotting this vertex.
         """
         return type(self).__name__
@@ -124,27 +123,30 @@
         """
         Implements self == o
         """
         if self is o:
             return True
         if (self, o) in self.__comparing or (o, self) in self.__comparing:
             return True
-        self.__comparing.add((self, o))
         if type(self) != type(o):
             return False
+        self.__comparing.add((self, o))
         res = all(getattr(self, name) == getattr(o, name) for name in type(self).__slots__)
         self.__comparing.remove((self, o))
         return res
     
     def __reduce__(self) -> str | tuple[Any, ...]:
         """
         Implements dumping of self
         """
         # Note : When serializing a vertex, the edges/arrows should not be serialized. These will be handled independently when serializing a graph.
-        func, args, state = super().__reduce__()
+        pickle_data = super().__reduce__()
+        if isinstance(pickle_data, str):
+            raise TypeError("Expected tuple from parent's __reduce__, got str")
+        func, args, state = pickle_data
         state : dict
         if "edges" in state or "graph" in state:
             raise RuntimeError("Cannot pickle edges or graph of a vertex")
         return type(self), (), state
     
     def __setstate__(self, state : Dict[str, Any]):
         """
@@ -192,58 +194,57 @@
         """
         for e in self.edges:
             if e.source is self:
                 yield e.destination
             else:
                 yield e.source
     
-    def outwards(self) -> Iterator["Arrow"]:
+    def outwards(self) -> Iterator["Vertex"]:
         """
         Iterates over the outwards neighbors of this vertex (neighbors linked by an outgoing arrow).
         """
         for e in self.edges:
             if isinstance(e, Arrow) and e.source is self:
                 yield e.destination
     
-    def inwards(self) -> Iterator["Arrow"]:
+    def inwards(self) -> Iterator["Vertex"]:
         """
         Iterates over the inwards neighbors of this vertex (neighbors linked by an incomming arrow).
         """
         for e in self.edges:
             if isinstance(e, Arrow) and e.destination is self:
                 yield e.source
     
-    def linked(self) -> Iterator["Edge"]:
+    def linked(self) -> Iterator["Vertex"]:
         """
         Iterates over the undirected neighbors if this vertex (neighbors linked by a strict edge).
         """
         for e in self.edges:
             if not isinstance(e, Arrow):
                 yield (e.source if e is not e.source else e.destination)
 
-    def connect(self, o : "Vertex", name : str, *, directional : bool = False, c : Optional[Color] = None) -> None:
+    def connect(self, o : "Vertex", *, directional : bool = False, c : Optional[Color] = None) -> None:
         """
         Links this vertex to another. Directional indicates if the link should be an arrow instead of an edge.
         """
-        if not isinstance(o, Vertex) or not isinstance(name, str):
-            raise TypeError("Expected vertex, str, got " + repr(o.__class__.__name__) + " and " + repr(name.__class__.__name__))
+        if not isinstance(o, Vertex):
+            raise TypeError("Expected vertex, got " + repr(o.__class__.__name__))
         if not isinstance(directional, bool):
             raise TypeError("Expected bool for directional, got" + repr(directional.__class__.__name__))
         if c == None:
             c = Color.average(self.color, o.color)
         if not isinstance(c, Color):
             raise TypeError("Expected color for c, got " + repr(c.__class__.__name__))
         if directional:
-            e = Arrow(name, self, o, c=c)
+            e = Arrow(self, o, c=c)
         else:
-            e = Edge(name, self, o, c=c)
+            e = Edge(self, o, c=c)
         e.write()
 
     @classmethod
-    @chrono
     def add_vertices_to_graph(cls : Type["Vertex"], G : "Graph", fil : Optional[Callable[["Vertex"], bool]] = None):
         """
         Adds all vertices of this class to a graph.
         If given a filter function fil, only filtered vertices will be added.
         """
         if not isinstance(G, Graph):
             raise TypeError("Expected graph, got " + repr(G.__class__.__name__))
@@ -257,50 +258,28 @@
 
 
 
 
 class UniqueVertex(Vertex):
 
     """
-    Vertices from this class all have different hashes, (but can still compare equals if they have equal custom attributes).
+    Vertices from this class all have different hashes and always compare different (except when they are the same object).
     """
 
-    __N = 0          # Current index
-    __lock = RLock() # The lock used to ensure instance creation is thread-safe
-
-    __slots__ = {
-        "__id" : "The unique identifier of this vertex."
-    }
-
-    def __init__(self, *, c: Color | None = None, parent: Optional["Vertex"] = None) -> None:
-        self.__id = None
-        self.__pickID()
-        super().__init__(c = c, parent = parent)
-
-    def __pickID(self):
-        """
-        Picks a unique id for self if it doesn't have one.
-        """
-        if self.__id == None:
-            with UniqueVertex.__lock:
-                self.__id = UniqueVertex.__N
-                UniqueVertex.__N += 1
-    
     def __hash__(self) -> int:
         """
         Implements hash(self).
         """
-        self.__pickID()
-        return self.__id
+        return id(self)
     
     def __eq__(self, o: object) -> bool:
         """
         Implements self == o.
         """
-        return type(self) == type(o) and self.__id == o.__id
+        return self is o
             
 
 
 
 
 class Edge(metaclass = InstanceReferencingClass):
 
@@ -412,15 +391,15 @@
         from .utils import extract_pickle_slots
         return {name : getattr(self, name) for name in extract_pickle_slots(type(self))}
     
     def __copy__(self) -> "Edge":
         """
         Implements copy(self)
         """
-        # TO-DO
+        raise NotImplementedError
         
     def write(self):
         """
         Writes this edge in the edges sets of both vertices.
         """
         self.source.edges.add(self)
         self.destination.edges.add(self)
@@ -435,17 +414,17 @@
         """
         self.source.edges.discard(self)
         self.destination.edges.discard(self)
         if self.source.graph:
             self.source.graph.edges.discard(self)
         elif self.destination.graph:
             self.destination.graph.edges.discard(self)
+        return self.source, self.destination
     
     @classmethod
-    @chrono
     def add_edges_to_graph(cls : Type["Edge"], G : "Graph", fil : Optional[Callable[["Edge"], bool]] = None):
         """
         Adds all edges of this class to a graph.
         If given a filter function fil, only filtered edges will be added.
         """
         if not isinstance(G, Graph):
             raise TypeError("Expected graph, got " + repr(G.__class__.__name__))
@@ -495,15 +474,14 @@
 
 
 
 
 
 CLS = TypeVar("CLS", bound=Vertex)
 
-@chrono
 def find_or_create(cls : Type[CLS], **kwargs) -> Tuple[CLS, bool]:
     """
     Finds in the given class cls for a vertex which attributes have values matching the given keyword arguments.
     If there is one, returns it. Otherwise, creates it.
     Returns the object and a boolean indicating if the object existed before.
     """
     for ist in cls:
@@ -527,16 +505,14 @@
 
     __slots__ = {
         "vertices" : "The set of vertices in this graph",
         "edges" : "The set of edges in this graph",
         "data" : "A dictionary holding additional data for this graph"
     }
 
-    __hash__ = None
-
     __active_graphs : dict[Thread, list["Graph"]] = {}
 
     def __init__(self) -> None:
         from typing import Any
         self.vertices : Set[Vertex] = set()
         self.edges : Set[Edge] = set()
         self.data : dict[str, Any] = {}
@@ -552,14 +528,20 @@
     
     def __exit__(self, exc_type, exc_value, traceback):
         """
         Implements with self.
         """
         from threading import current_thread
         Graph.__active_graphs[current_thread()].remove(self)
+
+    def __eq__(self, o : object) -> bool:
+        """
+        Implements self == o. Equivalent to self is o.
+        """
+        return self is o
     
     @staticmethod
     def active_graphs() -> list["Graph"]:
         """
         Returns the list of all the active Graphs in the current thread.
         """
         from threading import current_thread
@@ -577,15 +559,14 @@
             raise TypeError("Expected bool for explore, got " + repr(explore.__class__.__name__))
         if v not in self.vertices:
             self.vertices.add(v)
             v.graph = self
             if explore:
                 self.explore(v)
     
-    @chrono
     def explore(self, source : Optional[Vertex] = None) -> None:
         """
         Explores the graph for more linked vertices. If a vertex of the graph is given, only searches starting from that vertex. Otherwise, searches from all vertices.
         """
         if source == None:
             to_explore = self.vertices.copy()
         else:
@@ -635,23 +616,15 @@
     
     @property
     def m(self) -> int:
         """
         The number of edges and arrows.
         """
         return len(self.edges)
-    
-    def diameter(self) -> int:
-        """
-        Returns the diameter of the graph.
-        """
-        import networkx as nx
-        G = self.NetworkX().to_undirected()
-        return nx.diameter(G)
-    
+        
     def append(self, value : Vertex | Edge, explore : bool = False):
         """
         Adds a vertex or an edge to the graph.
         If explore is True, explores the graph from the added vertex or the source vertex of the added edge.
         """
         if not isinstance(explore, bool):
             raise TypeError("Expected bool for explore, got " + repr(explore.__class__.__name__))
@@ -682,15 +655,14 @@
         elif isinstance(value, Edge):
             self.edges.discard(value)
             value.source.edges.discard(value)
             value.destination.edges.discard(value)
         else:
             raise TypeError("Expected edge or vertex, got " + repr(type(value).__name__))
 
-    @chrono
     def extend(self, values : Iterable[Vertex | Edge], explore : bool = False):
         """
         Extends the graph with an iterable of vertices and/or edges.
         """
         from typing import Iterable
         if not isinstance(explore, bool):
             raise TypeError("Expected bool for explore, got " + repr(explore.__class__.__name__))
@@ -769,15 +741,14 @@
     #     for u, e, v in self.pairs():
     #         e = deepcopy(e, memo)
     #         e.source = translation[u]
     #         e.destination = translation[v]
     #         e.write()
     #     return cp
 
-    @chrono
     def export(self, file : str, *, subgraph_supported : bool = False) -> None:
         """
         Writes this graph under the GEXF format into file.
         """
         # List of possible attributes to include in visuals :
         # Node Size : proportional to radius! not surface area!
         # Color : R, G, B
@@ -863,41 +834,10 @@
                     edge_i = ET.SubElement(edges, "edge", source=str(n_ids[u]), target=str(n_ids[v]), type="directed", label="contains", weight="1.0")
                 f.write(head + b"\n")
                 ET.indent(root, "\t")
                 for line in ET.tostringlist(root):
                     f.write(line + b"\n")
         except Exception as E:
             raise
-
-    @chrono
-    def NetworkX(self) -> Union["nx.Graph", "nx.DiGraph", "nx.MultiGraph", "nx.MultiDiGraph"]:
-        """
-        Returns a NeworkX version of this graph.
-        """
-        import networkx as nx
-        multi = False
-        directed = False
-        seen : Set[Tuple[Vertex, Vertex]] = set()
-        for u, e, v in self.pairs():
-            if (u, v) in seen:
-                multi = True
-            if isinstance(e, Arrow):
-                directed = True
-            if multi and directed:
-                break
-        if multi and directed:
-            G = nx.MultiDiGraph()
-        elif multi:
-            G = nx.MultiGraph()
-        elif directed:
-            G = nx.DiGraph()
-        else:
-            G = nx.Graph()
-        for u, e, v in self.pairs():
-            G.add_edge(u, v)        # à améliorer
-        for u in self.vertices:
-            for v in u.children:
-                G.add_edge(u, v)
-        return G
     
 
-del RLock, Any, Callable, Dict, Iterable, Iterator, Optional, Set, Tuple, Type, TypeVar, Union, Color, InstanceReferencingClass, chrono, CLS
+del RLock, Any, Callable, Dict, Iterable, Iterator, Optional, Set, Tuple, Type, TypeVar, Union, Color, InstanceReferencingClass, CLS
```

### Comparing `baguette_verse-0.9/baguette/bakery/source/record.py` & `baguette_verse-0.9.5/baguette/bakery/source/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Any, Dict, Iterable, Union
+# from Viper.frozendict import frozendict
 
 _hashing = set()
 
 class record:
 
     """
     A class to hold key-values informations. Similar to dict but works with attributes instead.
```

### Comparing `baguette_verse-0.9/baguette/bakery/source/utils.py` & `baguette_verse-0.9.5/baguette/bakery/source/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,105 +1,67 @@
-from numbers import Complex
-from typing import Any, Callable, Generic, Iterable, Iterator, ParamSpec, Sequence, Set, Type, TypeVar
-import pathlib
+"""
+This module adds some useful functions and classes for the compilation of BAGUETTE graphs.
+"""
 
+import pathlib
+from functools import cache
+from typing import (Any, Callable, Generic, Iterable, Iterator, ParamSpec, Set,
+                    TypeVar)
 
 from Viper.debugging.chrono import Chrono
-chrono = Chrono()
-chrono.enabled = False
-del Chrono
-
-
 
+from .graph import Edge, Vertex
 
+__all__ = ["chrono", "extract_pickle_slots", "path_factory", "is_path", "parse_command_line", "System"]
 
-def avg(*s : Complex | Sequence[Complex], **kwargs : Any) -> Complex:
-    """
-    Returns the average of a series of numbers. Works like min/max without the key argument.
-    """
-    for k in kwargs:
-        if k != "default":
-            raise TypeError(repr(k) + " is an invalid keyword argument for avg()")
-    if len(s) == 0:
-        raise TypeError("avg expected at least 1 argument, got 0")
-    if len(s) == 1:
-        s = s[0]
-    n, m = 0, 0
-    for e in s:
-        n += 1
-        m += e
-    if n == 0:
-        if "default" in kwargs:
-            return kwargs["default"]
-        raise ZeroDivisionError("avg() arg is an empty sequence")
-    return n / m
 
 
-def dev(*s : Complex | Sequence[Complex], **kwargs : Any) -> Complex:
-    """
-    Returns the standart deviation of a series of numbers. Works like min/max without the key argument.
-    """
-    for k in kwargs:
-        if k != "default":
-            raise TypeError(repr(k) + " is an invalid keyword argument for dev()")
-    s = list(s)
-    if len(s) == 0:
-        if "default" in kwargs:
-            return kwargs["default"]
-        raise ZeroDivisionError("dev() arg is an empty sequence")
-    a = avg(s)
-    return avg((x - a) ** 2 for x in s) ** 0.5
 
 
-class extract:
+chrono = Chrono()
+chrono.enabled = False
 
-    def __init__(self, *keys : Any) -> None:
-        self.keys = keys
-    
-    def __call__(self, c : dict) -> Any:
-        for k in self.keys:
-            c = c[k]
-        return c
 
 
-def pretty_print(c : list | dict):
-    """
-    JSON style pretty print.
-    """
-    import json
-    print(json.dumps(c, indent="\t"))
 
 
-def extract_pickle_slots(o : type) -> Set[str]:
+@cache
+def extract_pickle_slots(o : type[Vertex | Edge]) -> Set[str]:
+    s : set[str]
     if not hasattr(o, "__pickle_slots__"):
         s = set()
     else:
-        s = set(o.__pickle_slots__)
+        s = set(o.__pickle_slots__) # type: ignore
+    for b in s:
+        if not isinstance(b, str):
+            raise RuntimeError("__pickle_slots__ should only contain str, got a " + repr(type(b).__name__))
     return s.union(*[extract_pickle_slots(b) for b in o.__bases__])
 
 
 def path_factory(path : str) -> pathlib.PurePath:
     """
     Returns the correct path factory class for the given graph (Either WindowsPurePath or PosixPurePath).
     """
+    from pathlib import PurePosixPath, PureWindowsPath
+
     from .graph import Graph
-    from pathlib import PureWindowsPath, PurePosixPath
     platform = Graph.active_graphs()[-1].data["platform"].lower() if Graph.active_graphs() else "windows"
     if "windows" in platform:
         return PureWindowsPath(path)
     else:
         return PurePosixPath(path)
 
 
 def is_path(s : str) -> bool:
     """
     Returns True if the given string represents a path for the current platform.
     """
+    from pathlib import PurePosixPath, PureWindowsPath
+
     from .graph import Graph
-    from pathlib import PureWindowsPath, PurePosixPath
     platform = Graph.active_graphs()[-1].data["platform"].lower() if Graph.active_graphs() else "windows"
     if "windows" in platform:
         forbidden = set("<>\"|?*")
         if forbidden.intersection(s):           # Contains characters that are forbidden in Windows paths.
             return False
         if s.startswith("-") or s.startswith("/"):  # Could be a path, but it is more likely to be flag
             return False
@@ -115,19 +77,21 @@
         try:
             if PurePosixPath(s).is_reserved():
                 return False
             return True
         except:
             return False
         
+
 def parse_command_line(s : str) -> list[str]:
     """
     Parses command line with the syntax of the current platform's shell. Returns the argument vector.
     """
     import re
+
     from .graph import Graph
 
     platform = Graph.active_graphs()[-1].data["platform"].lower() if Graph.active_graphs() else "windows"
     if "windows" not in platform:
         RE_CMD_LEX = r'''"((?:\\["\\]|[^"])*)"|'([^']*)'|(\\.)|(&&?|\|\|?|\d?\>|[<])|([^\s'"\\&|<>]+)|(\s+)|(.)'''
     else:
         RE_CMD_LEX = r'''"((?:""|\\["\\]|[^"])*)"?()|(\\\\(?=\\*")|\\")|(&&?|\|\|?|\d?>|[<])|([^\s"&|<>]+)|(\s+)|(.)'''
@@ -196,15 +160,15 @@
                     raise RuntimeError("Trying to collapse non-quantum object.")
                 system.remove(self.__particule)         # type: ignore
                 if not system:  # The system has fully collapsed : time for callbacks
                     for cb, args, kwargs in collapse:
                         cb(*args, **kwargs)
                     collapse.clear()
         
-        self.Entangled : Type[Particule[P]] = Particule
+        self.Entangled : type[Particule[P]] = Particule
 
     def __contains__(self, p : P) -> bool:
         return p in self.__system
     
     def __len__(self) -> int:
         return len(self.__system)
     
@@ -243,8 +207,14 @@
         Removes all callbacks to the given function.
         """
         to_pop = []
         for i, (cbi, argsi, kwargsi) in enumerate(self.__at_collapse):
             if cb == cbi:
                 to_pop.append(i)
         for i in reversed(to_pop):
-            self.__at_collapse.pop(i)
+            self.__at_collapse.pop(i)
+
+
+
+
+
+del pathlib, cache, Any, Callable, Iterable, Iterator, ParamSpec, Set, TypeVar, Chrono, Edge, Vertex, CB_Args
```

### Comparing `baguette_verse-0.9/baguette/bakery/source/types/imports.py` & `baguette_verse-0.9.5/baguette/bakery/source/types/imports/entities.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """
-This module defines the Vertices and Edges that are related to importations.
+This module contains Vertex subclasses for this behavioral package.
 """
 
-from ...logger import logger
-from typing import Optional
-from ..colors import Color
-from ..graph import Edge, UniqueVertex, Vertex
-from .filesystem import NewFile, File
-from .execution import Process
-from ..utils import chrono
+from ....logger import logger
+from ...colors import Color
+from ...graph import UniqueVertex, Vertex
 
-__all__ = ["Import", "HasImport", "IsFile"]
+__all__ = ["Import"]
 
 
 
 
 
-logger.debug("Loading imports library.")
+logger.info("Loading entities from {} library.".format(__name__.rpartition(".")[0].rpartition(".")[2]))
 
 class Import(UniqueVertex):
     
     """
     An import vertex. Shows the use of a DLL or equivalent.
     """
 
@@ -39,30 +35,30 @@
     __suspicious_keyword_names = {
         "crypt",
         "advapi",
         "kernel",
         "sock"
     }
 
-    def __init__(self, *, c: Color | None = None, parent: Optional[Vertex] = None) -> None:
+    def __init__(self, *, c: Color | None = None, parent: Vertex | None = None) -> None:
         super().__init__(c=c, parent=parent)
         self.__name : str = ""
         self.path : str = ""
         self.length : int = 0
 
     @property
     def name(self) -> str:
         """
         The name of the imported library.
         """
         return self.__name
 
     @name.setter
     def name(self, n : str):
-        from ..config import ColorMap
+        from ...config import ColorMap
         if not isinstance(n, str):
             raise TypeError("Expected str, got " + repr(type(n).__name__))
         self.__name = n
         self.color = ColorMap.get_config().imports.Import
         for kw in self.__suspicious_keyword_names:
             if kw in n.lower():
                 self.color = ColorMap.get_config().imports.SuspiciousImport
@@ -75,56 +71,8 @@
         """
         return "Import {}".format(self.__name.lower())
     
 
 
 
 
-class HasImport(Edge):
-
-    """
-    This kind of edge indicates that a process imported something.
-    """
-
-    label : str = ""
-
-    source : Process
-    destination : Import
-
-
-
-
-
-class IsFile(Edge):
-
-    """
-    This kind of edge indicates that an import corresponds to an existing file object.
-    """
-
-    label : str = ""
-
-    source : Import
-    destination : File
-
-
-
-
-
-@chrono
-def link(e : NewFile):
-    from ..graph import find_or_create
-    if e.file.path.suffix.lower().endswith(".dll"):
-        I, ok = find_or_create(Import, path = e.file.name)
-        if not ok:
-            import re
-            expr1 = re.compile(r"([a-zA-Z0-9_.]+)(\..*?)$")
-            match = expr1.search(e.file.name)
-            if match:
-                I.name = match.group(1).lower()
-            else:
-                I.name = e.file.name
-        IsFile(I, e.file)
-
-NewFile.add_callback(link)
-
-
-del logger, Optional, Color, UniqueVertex, Vertex, NewFile, chrono, link
+del Color, UniqueVertex, Vertex, logger
```

### Comparing `baguette_verse-0.9/baguette/croutons/extractor.py` & `baguette_verse-0.9.5/baguette/croutons/extractor.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9/baguette/croutons/metalib/evaluator.py` & `baguette_verse-0.9.5/baguette/croutons/metalib/evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,29 +43,32 @@
         """
         return self.__code
     
     @code.setter
     def code(self, code : str):
         if not isinstance(code, str):
             raise TypeError("Expected str, got " + repr(type(code).__class__))
+        old_code = self.__code
         try:
-            old_code, self.__code = self.__code, code
+            self.__code = code
             self.__compile()
         except SyntaxError as E:
             self.__code = old_code
             raise SyntaxError("Cannot set function code as it contains a syntax error.") from E
         self.__code = code
     
     def __str__(self) -> str:
         return "lambda x : " + self.__code
     
     def __repr__(self) -> str:
         return "Evaluator(" + repr(self.__code) + ")"
     
     def __call__(self, x : X) -> R:
+        if not self.__compiled:
+            raise RuntimeError("Tried to call an empty Evaluator")
         try:
             return self.__compiled(x)
         except BaseException as E:
             raise E from None
     
     def __getstate__(self) -> dict[str, Any]:
         return {"code" : self.__code}
```

### Comparing `baguette_verse-0.9/baguette/croutons/metalib/interact.py` & `baguette_verse-0.9.5/baguette/croutons/metalib/interact.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9/baguette/croutons/metalib/utils.py` & `baguette_verse-0.9.5/baguette/croutons/metalib/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9/baguette/croutons/source/metagraph.py` & `baguette_verse-0.9.5/baguette/croutons/source/metagraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-from typing import Any, Callable, Generic, Iterable, Iterator, Optional, TypeVar
+"""
+This module defines MetaGraphs, MetaVertices, MetaEdges and MetaArrows.
+"""
+
+from typing import Any, Callable, Iterable, Iterator, Optional, Self
 from ...bakery.source.graph import Arrow, Edge, Graph, UniqueVertex, Vertex
 from ...bakery.source.colors import Color
 from ...bakery.source.types.execution import *
 from ...bakery.source.types.network import *
 from ...bakery.source.types.filesystem import *
 
 
 
-V = TypeVar("V", bound=Vertex)
 
-class MetaVertex(UniqueVertex, Generic[V]):
+
+class MetaVertex(UniqueVertex):
 
     """
     This class describes a type vertex. One or multiple Vertex subclasses can be associated to it.
     """
 
     @classmethod
     def __class_getitem__(cls, cls_init):
         try:
             Mv = cls()
             Mv.cls = cls_init
             return Mv
-        except:
-            return super().__class_getitem__(cls_init)
+        except BaseException as E:
+            raise E from None
 
     __slots__ = {
         "__class" : "The class that this MetaVertex represents.",
         "__condition" : "An additional condition function. Takes a Vertex as an input and tells whether or not it can be a valid match (does not need to check type)",
         "__color" : "The Color forcefully set to this MetaVertex."
     }
 
@@ -63,22 +67,22 @@
     def color(self, c : Color):
         from ...bakery.source.colors import Color
         if not isinstance(c, Color):
             raise TypeError("Expected Color, got " + repr(type(c).__name__))
         self.__color = c
     
     @property
-    def cls(self) -> type[V]:
+    def cls(self) -> type[Vertex]:
         """
         The class that his vertex represents.
         """
         return self.__class
     
     @cls.setter
-    def cls(self, cls : type[V]):
+    def cls(self, cls : type[Vertex]):
         """
         Sets the class associated with this vertex.
         """
         from typing import _UnionGenericAlias
         from types import UnionType
         from .utils import class_union
         from ...bakery.source.graph import Vertex
@@ -95,22 +99,22 @@
                 if not isinstance(c, type) or not issubclass(c, Vertex):
                     raise TypeError("Expected subclasses of Vertex , got " + repr(c))
             self.__class = cls
         else:
             raise TypeError("Expected subclass of Vertex , got " + repr(cls))
 
     @property
-    def condition(self) -> Callable[[Vertex], bool]:
+    def condition(self) -> Callable[[Vertex], bool] | bool:
         """
         An additional condition to check when trying to match a Vertex to this MetaVertex.
         """
         return self.__condition
     
     @condition.setter
-    def condition(self, cond : Callable[[Vertex], bool]):
+    def condition(self, cond : Callable[[Vertex], bool] | bool):
         """
         Sets the additional condition function for this MetaVertex.
         """
         if not callable(cond) and not isinstance(cond, bool):
             raise TypeError("Expected callable or bool, got " + repr(type(cond).__name__))
         self.__condition = cond
     
@@ -139,32 +143,21 @@
     def __repr__(self) -> str:
         return type(self).__name__ + "[" + self.__get_cls_str() + "]" + ("{" + str(self.__condition) + "}" if callable(self.__condition) else "")
     
 
 
 
 
-E = TypeVar("E", bound=Edge)
-
-class MetaEdge(Edge, Generic[E]):
+class MetaEdge(Edge):
 
     """
     This class describes a type edge. One or multiple Edge subclasses can be associated to it.
     Note that a MetaEdge can represent a subclass of Arrow and in this case, the match can be made in both directions.
     """
 
-    @classmethod
-    def __class_getitem__(cls, cls_init):
-        try:
-            Mv = cls()
-            Mv.cls = cls_init
-            return Mv
-        except:
-            return super().__class_getitem__(cls_init)
-
     __slots__ = {
         "__class" : "The class that this MetaEdge represents.",
         "__condition" : "An additional condition function. Takes an Edge as an input and tells whether or not it can be a valid match (does not need to check type)",
         "__color" : "The Color forcefully set to this MetaVertex."
     }
 
     __pickle_slots__ = {
@@ -203,22 +196,22 @@
     def color(self, c : Color):
         from ...bakery.source.colors import Color
         if not isinstance(c, Color):
             raise TypeError("Expected Color, got " + repr(type(c).__name__))
         self.__color = c
     
     @property
-    def cls(self) -> type[E]:
+    def cls(self) -> type[Edge]:
         """
         The class that his edge represents.
         """
         return self.__class
     
     @cls.setter
-    def cls(self, cls : type[E]):
+    def cls(self, cls : type[Edge]):
         """
         Sets the class associated with this edge.
         """
         from typing import _UnionGenericAlias
         from types import UnionType
         from .utils import class_union
         from ...bakery.source.graph import Edge
@@ -233,22 +226,22 @@
         elif isinstance(cls, UnionType):
             for c in cls.__args__:
                 if not isinstance(c, type) or not issubclass(c, Edge):
                     raise TypeError("Expected subclasses of Edge , got " + repr(c))
             self.__class = cls
         
     @property
-    def condition(self) -> Callable[[Edge], bool]:
+    def condition(self) -> Callable[[Edge], bool] | bool:
         """
         An additional condition to check when trying to match an Edge to this MetaEdge.
         """
         return self.__condition
     
     @condition.setter
-    def condition(self, cond : Callable[[Edge], bool]):
+    def condition(self, cond : Callable[[Edge], bool] | bool):
         """
         Sets the additional condition function for this MetaEdge.
         """
         if not callable(cond) and not isinstance(cond, bool):
             raise TypeError("Expected callable or bool, got " + repr(type(cond).__name__))
         self.__condition = cond
     
@@ -273,27 +266,25 @@
 
     def __str__(self) -> str:
         return type(self).__name__ + "[" + self.__get_cls_str() + "]" + ("*" if callable(self.__condition) else "")
     
     def __repr__(self) -> str:
         return type(self).__name__ + "[" + self.__get_cls_str() + "]" + ("{" + str(self.__condition) + "}" if callable(self.__condition) else "")
 
-    def __getitem__(self, cls : type[E]) -> "MetaEdge":
+    def __getitem__(self, cls : type[Edge]) -> Self:
         try:
             self.__class = cls
             return self
         except BaseException as E:
             raise E from None
 
 
 
 
-A = TypeVar("A", bound=Arrow)
-
-class MetaArrow(Arrow, MetaEdge, Generic[A]):
+class MetaArrow(Arrow, MetaEdge):
 
     """
     This class describes a type arrow. One or multiple Arrow subclasses can be associated to it.
     """
 
     __slots__ = {
         "__class" : "The class that this MetaArrow represents.",
@@ -307,22 +298,22 @@
 
     def __init__(self, source: MetaVertex, destination: MetaVertex, *, c: Color | None = None, auto_write: bool = True) -> None:
         super().__init__(source, destination, c=c, auto_write=auto_write)
         self.__class : type[Arrow] = Arrow
         self.__condition : Callable[[Arrow], bool] | bool = True
     
     @property
-    def cls(self) -> type[A]:
+    def cls(self) -> type[Arrow]:
         """
         The class that his arrow represents.
         """
         return self.__class
     
     @cls.setter
-    def cls(self, cls : type[A] | Iterable[type[A]]):
+    def cls(self, cls : type[Arrow]):
         """
         Sets the class associated with this arrow.
         """
         from typing import _UnionGenericAlias
         from types import UnionType
         from .utils import class_union
         from ...bakery.source.graph import Arrow
@@ -337,30 +328,30 @@
         elif isinstance(cls, UnionType):
             for c in cls.__args__:
                 if not isinstance(c, type) or not issubclass(c, Arrow):
                     raise TypeError("Expected subclasses of Arrow , got " + repr(c))
             self.__class = cls
 
     @property
-    def condition(self) -> Callable[[Arrow], bool]:
+    def condition(self) -> Callable[[Arrow], bool] | bool:
         """
         An additional condition to check when trying to match an Arrow to this MetaArrow.
         """
         return self.__condition
     
     @condition.setter
-    def condition(self, cond : Callable[[Arrow], bool]):
+    def condition(self, cond : Callable[[Arrow], bool] | bool):
         """
         Sets the additional condition function for this MetaArrow.
         """
         if not callable(cond) and not isinstance(cond, bool):
             raise TypeError("Expected callable or bool, got " + repr(type(cond).__name__))
         self.__condition = cond
     
-    def match(self, a : Arrow) -> bool:
+    def match(self, a : Edge) -> bool:
         """
         Returns True if the Arrow a has a matching type.
         """
         return isinstance(a, self.__class) and (self.__condition(a) if callable(self.__condition) else self.__condition)
 
     def __get_cls_str(self) -> str:
         """
@@ -377,26 +368,26 @@
     
     def __str__(self) -> str:
         return type(self).__name__ + "[" + self.__get_cls_str() + "]" + ("*" if callable(self.__condition) else "")
     
     def __repr__(self) -> str:
         return type(self).__name__ + "[" + self.__get_cls_str() + "]" + ("{" + str(self.__condition) + "}" if callable(self.__condition) else "")
     
-    def __getitem__(self, cls : type[A]) -> "MetaArrow":
+    def __getitem__(self, cls : type[Arrow]) -> Self:
         try:
             self.__class = cls
             return self
         except BaseException as E:
             raise E from None
     
 
 
 
 
-class MetaGraph(Graph, Generic[V, E, A]):
+class MetaGraph(Graph):
 
     """
     This particular type of graph can only contain MetaVertices, MetaEdges or MetaArrows. It can be used for normal graph exploration.
     """
 
     __slots__ = {
         "__named_objects" : "A dict holding named vertices and edges."
@@ -406,73 +397,77 @@
     edges : set[MetaEdge | MetaArrow]
 
     def __init__(self, g : Graph = Graph()) -> None:
         if not isinstance(g, Graph):
             raise TypeError("Exepcted Graph, got " + repr(type(g).__name__))
         super().__init__()
         self.__named_objects : dict[str, MetaEdge | MetaVertex] = {}
-        translation_table : dict[Vertex | Edge, MetaVertex | MetaEdge] = {}
+        vertex_translation_table : dict[Vertex, MetaVertex] = {}
+        edge_translation_table : dict[Edge, MetaEdge] = {}
         for v, e, u in g.pairs():
-            if v in translation_table:
-                Mv = translation_table[v]
+            if v in vertex_translation_table:
+                Mv = vertex_translation_table[v]
             else:
                 Mv = MetaVertex()
                 Mv.cls = type(v)
-                translation_table[v] = Mv
+                vertex_translation_table[v] = Mv
                 self.append(Mv)
-            if u in translation_table:
-                Mu = translation_table[u]
+            if u in vertex_translation_table:
+                Mu = vertex_translation_table[u]
             else:
                 Mu = MetaVertex()
                 Mu.cls = type(u)
-                translation_table[u] = Mu
+                vertex_translation_table[u] = Mu
                 self.append(Mu)
-            if e in translation_table:
-                Me = translation_table[e]
+            if e in edge_translation_table:
+                Me = edge_translation_table[e]
             else:
                 Me = MetaEdge(Mv, Mu)
                 Me.cls = type(e)
-                translation_table[e] = Me
+                edge_translation_table[e] = Me
                 self.append(Me)
     
     @property
     def names(self) -> list[str]:
         """
         Returns the list of names for named Meta{Vertices, Edges, Arrows} available in this MetaGraph.
         """
         return list(self.__named_objects)
 
-    def add_vertex(self, v: MetaVertex[V], explore: bool = True) -> None:
-        if not isinstance(V, MetaVertex):
+    def add_vertex(self, v: MetaVertex, explore: bool = True) -> None:
+        if not isinstance(v, MetaVertex):
             raise TypeError("Expected MetaVertex, got " + repr(type(v).__name__))
         return super().add_vertex(v, explore)
 
-    def pairs(self) -> Iterator[tuple[V, E | A, V]]:
-        return super().pairs()
+    def pairs(self) -> Iterator[tuple[MetaVertex, MetaEdge, MetaVertex]]:
+        for u, e, v in super().pairs():
+            if not isinstance(u, MetaVertex) or not isinstance(e, MetaEdge) or not isinstance(v, MetaVertex):
+                raise TypeError("Got a normal Vertex/Edge in a MetaGraph")
+            yield u, e, v
     
-    def append(self, value: V | E | A, explore: bool = False):
+    def append(self, value: MetaVertex | MetaEdge, explore: bool = False):
         if not isinstance(value, MetaVertex | MetaEdge | MetaArrow):
             raise TypeError("Expected MetaVertex, MetaEdge or MetaArrow, got " + repr(type(value).__name__))
         return super().append(value, explore)
     
-    def extend(self, values: Iterable[V | E | A], explore: bool = False):
+    def extend(self, values: Iterable[MetaVertex | MetaEdge], explore: bool = False):
         from typing import Iterable
         if not isinstance(explore, bool):
             raise TypeError("Expected bool for explore, got " + repr(explore.__class__.__name__))
         if not isinstance(values, Iterable):
             raise TypeError("Expected iterable, got " + repr(values.__class__.__name__))
-        def checked():
+        def __checked():
             for v in values:
                 if not isinstance(v, MetaVertex | MetaEdge | MetaArrow):
                     raise TypeError("Expected iterable of MetaVertex, MetaEdge or MetaArrow, got " + repr(type(v).__name__))
                 yield v
-        return super().extend(checked(), explore)
+        return super().extend(__checked(), explore)
 
     def __dir__(self) -> list[str]:
-        return super().__dir__() + self.names
+        return list(super().__dir__()) + self.names
     
     def __getattribute__(self, name: str) -> Any:
         try:
             return super().__getattribute__(name)
         except AttributeError as e:
             if name not in self.__named_objects:
                 raise e from None
@@ -720,62 +715,14 @@
         #     g.extend(dg.values())
         #     yield g
 
 
 
 
 
-def metapath(*cls : type[Vertex], bidirectional : bool = True) -> MetaGraph:
-    
-    """
-    Builds a path-like MetaGraph using the given arguments. They should be a sequence of alternating Vertex subclasses and Edge/Arrow subclasses.
-    If birectional is True, arrow types will be interpreted by MetaEdges and thus can be matched in both ways (a matching graph might not be an oriented path).
-    Otherwise, direction is preserved.
-    """
-
-    if not isinstance(bidirectional, bool):
-        raise TypeError("Expected bool for bidirectional, got " + repr(type(bidirectional).__name__))
-
-    p = MetaGraph()
-    l = list(cls)
-
-    for i, cli in enumerate(l):
-        if i % 2 == 0:  # Should be a Vertex type
-            if not isinstance(cli, type) or not issubclass(cli, Vertex):
-                raise TypeError("Expected alternating Vertex subclasses and Edge/Arrow subclasses, got " + repr(cli))
-        else:           # Should be an Edge or Arrow
-            if not isinstance(cli, type) or not issubclass(cli, Edge | Arrow):
-                raise TypeError("Expected alternating Vertex subclasses and Edge/Arrow subclasses, got " + repr(cli))
-    
-    vertices = []
-    for i, cli in enumerate(l):
-        if i % 2 == 0:
-            Mv = MetaVertex()
-            Mv.cls = cli
-            vertices.append(Mv)
-    
-    edges = []
-    for i, cli in enumerate(l):
-        if i % 2 == 1:
-            if not bidirectional and issubclass(cli, Arrow):
-                Ma = MetaArrow(vertices[i // 2], vertices[i // 2 + 1])
-                Ma.cls = cli
-                edges.append(Ma)
-            else:
-                Me = MetaEdge(vertices[i // 2], vertices[i // 2 + 1])
-                Me.cls = cli
-                edges.append(Me)
-    
-    p.extend(vertices)
-    p.extend(edges)
-
-    return p
-
-
-
 # N = 0
 
 # class Square(UniqueVertex):
 #     def __init__(self, *, c: Color = Color.blue, parent: Optional["Vertex"] = None) -> None:
 #         global N
 #         super().__init__(c=c, parent=parent)
 #         self.label = type(self).__name__[0]+str(N)
```

### Comparing `baguette_verse-0.9/.gitignore` & `baguette_verse-0.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9/LICENSE` & `baguette_verse-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9/README.md` & `baguette_verse-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9/pyproject.toml` & `baguette_verse-0.9.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "baguette-verse"
-version = "0.9"
+version = "0.9.5"
 authors = [
   { name="Vincent Raulin", email="vincent.raulin@inria.fr" },
 ]
 description = "A malware behavioral analysis framework centered around BAGUETTE!"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
 ]
 dependencies =  [
-  "viper_lib>=0.5.1",
+  "viper_lib>=0.5.4",
   "python-magic; platform_system != 'Windows'",
   "python-magic-bin; platform_system == 'Windows'",
   "Levenshtein"
 ]
 
 [project.scripts]
 bake = "bake:main"
```

### Comparing `baguette_verse-0.9/PKG-INFO` & `baguette_verse-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baguette-verse
-Version: 0.9
+Version: 0.9.5
 Summary: A malware behavioral analysis framework centered around BAGUETTE!
 Project-URL: Repository, https://gitlab.inria.fr/vraulin/baguette-verse
 Project-URL: Bug Tracker, https://gitlab.inria.fr/vraulin/baguette-verse/-/issues
 Author-email: Vincent Raulin <vincent.raulin@inria.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
@@ -670,15 +670,15 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: levenshtein
 Requires-Dist: python-magic-bin; platform_system == 'Windows'
 Requires-Dist: python-magic; platform_system != 'Windows'
-Requires-Dist: viper-lib>=0.5.1
+Requires-Dist: viper-lib>=0.5.4
 Description-Content-Type: text/markdown
 
 # BAGUETTE-VERSE
 
 This is the BAGUETTE framework. BAGUETTE stands for **Behavioral Analysis Graph Using Execution Traces Towards Explanability**.
 BAGUETTE is a **heterogeneous graph** data structure used to represent the **behavior of malware samples**.
```

