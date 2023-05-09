# Comparing `tmp/checkpoint_tool-0.7.2.tar.gz` & `tmp/checkpoint_tool-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkpoint_tool-0.7.2.tar", max compression
+gzip compressed data, was "checkpoint_tool-0.7.3.tar", max compression
```

## Comparing `checkpoint_tool-0.7.2.tar` & `checkpoint_tool-0.7.3.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     7146 2023-05-09 00:58:27.328907 checkpoint_tool-0.7.2/README.md
--rw-r--r--   0        0        0      628 2023-05-08 16:37:27.127303 checkpoint_tool-0.7.2/checkpoint/__init__.py
--rw-r--r--   0        0        0     2326 2023-05-09 00:25:34.051079 checkpoint_tool-0.7.2/checkpoint/app.py
--rw-r--r--   0        0        0    23235 2023-05-03 09:41:14.000902 checkpoint_tool-0.7.2/checkpoint/checkpoint_legacy.py
--rw-r--r--   0        0        0     4004 2023-05-03 13:31:12.624944 checkpoint_tool-0.7.2/checkpoint/database.py
--rw-r--r--   0        0        0     7168 2023-05-09 00:56:30.108576 checkpoint_tool-0.7.2/checkpoint/graph.py
--rw-r--r--   0        0        0    10978 2023-05-09 00:55:48.411714 checkpoint_tool-0.7.2/checkpoint/task.py
--rw-r--r--   0        0        0     1461 2023-05-03 14:04:28.456816 checkpoint_tool-0.7.2/checkpoint/types.py
--rw-r--r--   0        0        0      676 2023-05-09 00:58:56.073495 checkpoint_tool-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     8000 1970-01-01 00:00:00.000000 checkpoint_tool-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     7146 2023-05-09 00:58:27.328907 checkpoint_tool-0.7.3/README.md
+-rw-r--r--   0        0        0      628 2023-05-08 16:37:27.127303 checkpoint_tool-0.7.3/checkpoint/__init__.py
+-rw-r--r--   0        0        0     2435 2023-05-09 01:03:53.977120 checkpoint_tool-0.7.3/checkpoint/app.py
+-rw-r--r--   0        0        0     4004 2023-05-03 13:31:12.624944 checkpoint_tool-0.7.3/checkpoint/database.py
+-rw-r--r--   0        0        0     7168 2023-05-09 00:56:30.108576 checkpoint_tool-0.7.3/checkpoint/graph.py
+-rw-r--r--   0        0        0    10978 2023-05-09 00:55:48.411714 checkpoint_tool-0.7.3/checkpoint/task.py
+-rw-r--r--   0        0        0     1461 2023-05-03 14:04:28.456816 checkpoint_tool-0.7.3/checkpoint/types.py
+-rw-r--r--   0        0        0      676 2023-05-09 01:07:06.182237 checkpoint_tool-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     8000 1970-01-01 00:00:00.000000 checkpoint_tool-0.7.3/PKG-INFO
```

### Comparing `checkpoint_tool-0.7.2/README.md` & `checkpoint_tool-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.2/checkpoint/__init__.py` & `checkpoint_tool-0.7.3/checkpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.2/checkpoint/app.py` & `checkpoint_tool-0.7.3/checkpoint/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 from typing import Any
 from pathlib import Path
 import sys
 import json
+import pprint
 
 import click
 
 from .types import Context
 from .task import TaskType
 
 
@@ -42,13 +43,15 @@
     # spec.loader.exec_module(module)
 
     # Run the main task
     entrypoint_fn = getattr(module, entrypoint)
     assert issubclass(entrypoint_fn, TaskType), \
             f'Taskfile `{taskfile}` should contain a task(factory) `{entrypoint}`, but found `{entrypoint_fn}`.'
     task = entrypoint_fn()
-    task.run_graph_with_stats(rate_limits=rate_limits)
+    _, stats = task.run_graph_with_stats(rate_limits=rate_limits)
+    print('Execution summary:')
+    pprint.pprint(stats['stats'], sort_dicts=False)
     return 0
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `checkpoint_tool-0.7.2/checkpoint/database.py` & `checkpoint_tool-0.7.3/checkpoint/database.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.2/checkpoint/graph.py` & `checkpoint_tool-0.7.3/checkpoint/graph.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.2/checkpoint/task.py` & `checkpoint_tool-0.7.3/checkpoint/task.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.2/checkpoint/types.py` & `checkpoint_tool-0.7.3/checkpoint/types.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.2/pyproject.toml` & `checkpoint_tool-0.7.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkpoint-tool"
-version = "0.7.2"
+version = "0.7.3"
 description = "A lightweight workflow management tool written in pure Python"
 authors = ["Kohei Miyaguchi <koheimiyaguchi@gmail.com>"]
 license = "MIT License"
 homepage = "https://github.com/koheimiya/checkpoint"
 repository = "https://github.com/koheimiya/checkpoint"
 readme = "README.md"
 packages = [{include = "checkpoint"}]
```

### Comparing `checkpoint_tool-0.7.2/PKG-INFO` & `checkpoint_tool-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkpoint-tool
-Version: 0.7.2
+Version: 0.7.3
 Summary: A lightweight workflow management tool written in pure Python
 Home-page: https://github.com/koheimiya/checkpoint
 License: MIT
 Author: Kohei Miyaguchi
 Author-email: koheimiyaguchi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

