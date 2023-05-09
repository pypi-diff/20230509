# Comparing `tmp/robocorp_tasks-0.1.7.tar.gz` & `tmp/robocorp_tasks-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_tasks-0.1.7.tar", max compression
+gzip compressed data, was "robocorp_tasks-0.2.0.tar", max compression
```

## Comparing `robocorp_tasks-0.1.7.tar` & `robocorp_tasks-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     4922 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/README.md
--rw-r--r--   0        0        0     1266 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      721 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/__init__.py
--rw-r--r--   0        0        0       79 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/__main__.py
--rw-r--r--   0        0        0     4237 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_argdispatch.py
--rw-r--r--   0        0        0     1230 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_callback.py
--rw-r--r--   0        0        0     5048 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_collect_tasks.py
--rw-r--r--   0        0        0     5908 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_commands.py
--rw-r--r--   0        0        0      638 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_decorators.py
--rw-r--r--   0        0        0      182 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_exceptions.py
--rw-r--r--   0        0        0      599 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_hooks.py
--rw-r--r--   0        0        0     4985 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_log_auto_setup.py
--rw-r--r--   0        0        0      461 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_log_output_setup.py
--rw-r--r--   0        0        0     1790 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_protocols.py
--rw-r--r--   0        0        0     5053 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_task.py
--rw-r--r--   0        0        0      809 2023-05-05 11:49:59.131328 robocorp_tasks-0.1.7/src/robocorp/tasks/cli.py
--rw-r--r--   0        0        0     5667 1970-01-01 00:00:00.000000 robocorp_tasks-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     4922 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/README.md
+-rw-r--r--   0        0        0     1265 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3113 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/__init__.py
+-rw-r--r--   0        0        0       79 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/__main__.py
+-rw-r--r--   0        0        0     4495 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_argdispatch.py
+-rw-r--r--   0        0        0     1457 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_callback.py
+-rw-r--r--   0        0        0     5120 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_collect_tasks.py
+-rw-r--r--   0        0        0     7689 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_commands.py
+-rw-r--r--   0        0        0     2245 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_config.py
+-rw-r--r--   0        0        0      182 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_exceptions.py
+-rw-r--r--   0        0        0     1123 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_hooks.py
+-rw-r--r--   0        0        0     1367 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_lifecycle.py
+-rw-r--r--   0        0        0     5267 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_log_auto_setup.py
+-rw-r--r--   0        0        0      461 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_log_output_setup.py
+-rw-r--r--   0        0        0     3738 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_protocols.py
+-rw-r--r--   0        0        0     5487 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_task.py
+-rw-r--r--   0        0        0      809 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/cli.py
+-rw-r--r--   0        0        0     5666 1970-01-01 00:00:00.000000 robocorp_tasks-0.2.0/PKG-INFO
```

### Comparing `robocorp_tasks-0.1.7/README.md` & `robocorp_tasks-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.7/pyproject.toml` & `robocorp_tasks-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-tasks"
-version = "0.1.7"
+version = "0.2.0"
 description = "The automation framework for Python"
 authors = [
 	"Fabio Zadrozny <fabio@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robocorp/tasks", from = "src"}]
 classifiers = [
@@ -13,15 +13,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-robocorp-log = "0.0.15"
+robocorp-log = "0.1.0"
 # robocorp-log = {path = "../log/", develop = true}
 
 [tool.mypy]
 mypy_path = "src:tests"
 
 [[tool.mypy.overrides]]
 module = "setuptools.*"
```

### Comparing `robocorp_tasks-0.1.7/src/robocorp/tasks/_argdispatch.py` & `robocorp_tasks-0.2.0/src/robocorp/tasks/_argdispatch.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             default=".",
         )
         run_parser.add_argument(
             "-t",
             "--task",
             dest="task_name",
             help="The name of the task that should be run.",
-            default="",
+            action="append",
         )
         run_parser.add_argument(
             "-o",
             "--output-dir",
             dest="output_dir",
             help="The directory where the logging output files will be stored.",
             default="./output",
@@ -98,14 +98,21 @@
             help="Can be used so that log messages are also sent to the 'stdout' (if not specified the RC_LOG_OUTPUT_STDOUT is also queried).",
             dest="log_output_to_stdout",
             type=str,
             choices=["no", "json"],
             default="",
         )
 
+        run_parser.add_argument(
+            "--no-status-rc",
+            help="When set, if running tasks has an error inside the task the return code of the process is 0.",
+            dest="no_status_rc",
+            action="store_true",
+        )
+
         # List tasks
         list_parser = subparsers.add_parser(
             "list",
             help="Provides output to stdout with json contents of the tasks available.",
         )
         list_parser.add_argument(
             dest="path",
```

### Comparing `robocorp_tasks-0.1.7/src/robocorp/tasks/_callback.py` & `robocorp_tasks-0.2.0/src/robocorp/tasks/_callback.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from logging import getLogger
 
 logger = getLogger(__name__)
 
 
-class _OnExitContextManager:
+class OnExitContextManager:
     def __init__(self, on_exit):
         self.on_exit = on_exit
 
     def __enter__(self):
         pass
 
     def __exit__(self, exc_type, exc_val, exc_tb):
@@ -17,28 +17,36 @@
 class Callback(object):
     """
     Note that it's thread safe to register/unregister callbacks while callbacks
     are being notified, but it's not thread-safe to register/unregister at the
     same time in multiple threads.
     """
 
-    def __init__(self):
+    def __init__(self, reversed=False):
         self.raise_exceptions = False
+        self._reversed = reversed
         self._callbacks = ()
 
     def register(self, callback):
         self._callbacks = self._callbacks + (callback,)
 
         # Enable using as a context manager to automatically call the unregister.
-        return _OnExitContextManager(lambda: self.unregister(callback))
+        return OnExitContextManager(lambda: self.unregister(callback))
 
     def unregister(self, callback):
         self._callbacks = tuple(x for x in self._callbacks if x != callback)
 
+    def __len__(self):
+        return len(self._callbacks)
+
     def __call__(self, *args, **kwargs):
-        for c in self._callbacks:
+        if self._reversed:
+            iter_in = reversed(self._callbacks)
+        else:
+            iter_in = self._callbacks
+        for c in iter_in:
             try:
                 c(*args, **kwargs)
             except:
                 logger.exception(f"Error calling: {c}.")
                 if self.raise_exceptions:
                     raise
```

### Comparing `robocorp_tasks-0.1.7/src/robocorp/tasks/_collect_tasks.py` & `robocorp_tasks-0.2.0/src/robocorp/tasks/_collect_tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Iterator, List, Callable, Dict
+from typing import Iterator, List, Callable, Dict, Sequence
 from types import ModuleType
 import sys
 from robocorp.tasks._protocols import ITask
 
 
 def module_name_from_path(path: Path, root: Path) -> str:
     """
@@ -88,28 +88,30 @@
     mod = importlib.util.module_from_spec(spec)
     sys.modules[module_name] = mod
     spec.loader.exec_module(mod)  # type: ignore[union-attr]
     insert_missing_modules(sys.modules, module_name)
     return mod
 
 
-def collect_tasks(path: Path, task_name: str = "") -> Iterator[ITask]:
+def collect_tasks(path: Path, task_names: Sequence[str] = ()) -> Iterator[ITask]:
     """
     Note: collecting tasks is not thread-safe.
     """
     from robocorp.tasks import _hooks
     from robocorp.tasks._task import Task
 
-    _hooks.before_collect_tasks(path, task_name)
+    task_names_as_set = set(task_names)
+
+    _hooks.before_collect_tasks(path, task_names_as_set)
 
     def accept_task(task: ITask):
-        if not task_name:
+        if not task_names:
             return True
 
-        return task.name == task_name
+        return task.name in task_names
 
     methods_marked_as_tasks_found: List[Callable] = []
 
     _hooks.on_task_func_found.register(methods_marked_as_tasks_found.append)
 
     try:
         if path.is_dir():
```

### Comparing `robocorp_tasks-0.1.7/src/robocorp/tasks/_log_auto_setup.py` & `robocorp_tasks-0.2.0/src/robocorp/tasks/_log_auto_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Optional, List, Any
+from typing import Optional, List, Any, Tuple
 
 from ._protocols import ITask
 from robocorp import log
 
 
-def read_filters_from_pyproject_toml(context, path: Path) -> log.BaseConfig:
+def read_pyproject_toml(context, path: Path) -> Optional[Tuple[Path, dict]]:
     while True:
         pyproject = path / "pyproject.toml"
         try:
             if pyproject.exists():
                 break
         except OSError:
             continue
 
         parent = path.parent
         if parent == path or not parent:
             # Couldn't find pyproject.toml
-            return log.ConfigFilesFiltering()
+            return None
         path = parent
 
     try:
         toml_contents = pyproject.read_text(encoding="utf-8")
     except Exception:
         raise OSError(f"Could not read the contents of: {pyproject}.")
 
-    obj: Any
+    pyproject_toml: Any = None
     try:
         try:
             import tomllib  # type: ignore
         except ImportError:
             import tomli as tomllib  # type: ignore
 
-        obj = tomllib.loads(toml_contents)
+        pyproject_toml = tomllib.loads(toml_contents)
     except Exception:
         raise RuntimeError(f"Could not interpret the contents of {pyproject} as toml.")
+    return pyproject, pyproject_toml
 
+
+def read_filters_from_pyproject_toml(
+    context, pyproject: Path, pyproject_toml_contents: dict
+) -> log.BaseConfig:
+    if not pyproject_toml_contents:
+        log.ConfigFilesFiltering()
+
+    obj: Any = pyproject_toml_contents
     filters: List[log.Filter] = []
     if isinstance(obj, dict):
         # Filter(name="RPA", kind=FilterKind.log_on_project_call),
         # Filter("selenium", FilterKind.log_on_project_call),
         # Filter("SeleniumLibrary", FilterKind.log_on_project_call),
 
         read_parts: List[str] = []
```

### Comparing `robocorp_tasks-0.1.7/src/robocorp/tasks/_task.py` & `robocorp_tasks-0.2.0/src/robocorp/tasks/_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,19 +23,40 @@
     @property
     def lineno(self):
         return self.method.__code__.co_firstlineno
 
     def run(self):
         self.method()
 
+    @property
+    def failed(self):
+        return self.status in (Status.ERROR, Status.FAIL)
+
     def __typecheckself__(self) -> None:
         from robocorp.tasks._protocols import check_implements
 
         _: ITask = check_implements(self)
 
+    def __str__(self):
+        return f"Task({self.name}, status: {self.status})"
+
+    __repr__ = __str__
+
+
+class _TaskContext:
+    _current_task: Optional[ITask] = None
+
+
+def set_current_task(task: Optional[ITask]):
+    _TaskContext._current_task = task
+
+
+def get_current_task() -> Optional[ITask]:
+    return _TaskContext._current_task
+
 
 class Context:
     # Some regular message (generated by the framework).
     KIND_REGULAR = ConsoleMessageKind.REGULAR
 
     # Some message which deserves a bit more attention (generated by the framework).
     KIND_IMPORTANT = ConsoleMessageKind.IMPORTANT
```

### Comparing `robocorp_tasks-0.1.7/src/robocorp/tasks/cli.py` & `robocorp_tasks-0.2.0/src/robocorp/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.7/PKG-INFO` & `robocorp_tasks-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: robocorp-tasks
-Version: 0.1.7
+Version: 0.2.0
 Summary: The automation framework for Python
 Author: Fabio Zadrozny
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Dist: robocorp-log (==0.0.15)
+Requires-Dist: robocorp-log (==0.1.0)
 Description-Content-Type: text/markdown
 
 # robocorp-tasks
 
 `robocorp-tasks` is a Python framework designed to simplify the development 
 of Python automations.
```

