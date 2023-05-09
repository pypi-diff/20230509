# Comparing `tmp/checkpoint_tool-0.7.4.tar.gz` & `tmp/checkpoint_tool-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkpoint_tool-0.7.4.tar", max compression
+gzip compressed data, was "checkpoint_tool-0.7.5.tar", max compression
```

## Comparing `checkpoint_tool-0.7.4.tar` & `checkpoint_tool-0.7.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     7222 2023-05-09 01:08:27.319327 checkpoint_tool-0.7.4/README.md
--rw-r--r--   0        0        0      628 2023-05-08 16:37:27.127303 checkpoint_tool-0.7.4/checkpoint/__init__.py
--rw-r--r--   0        0        0     2763 2023-05-09 01:19:11.117797 checkpoint_tool-0.7.4/checkpoint/app.py
--rw-r--r--   0        0        0     4004 2023-05-03 13:31:12.624944 checkpoint_tool-0.7.4/checkpoint/database.py
--rw-r--r--   0        0        0     7168 2023-05-09 00:56:30.108576 checkpoint_tool-0.7.4/checkpoint/graph.py
--rw-r--r--   0        0        0    10978 2023-05-09 00:55:48.411714 checkpoint_tool-0.7.4/checkpoint/task.py
--rw-r--r--   0        0        0     1461 2023-05-03 14:04:28.456816 checkpoint_tool-0.7.4/checkpoint/types.py
--rw-r--r--   0        0        0      676 2023-05-09 01:21:38.550790 checkpoint_tool-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     8076 1970-01-01 00:00:00.000000 checkpoint_tool-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     7153 2023-05-09 01:45:57.090652 checkpoint_tool-0.7.5/README.md
+-rw-r--r--   0        0        0      608 2023-05-09 01:50:05.066517 checkpoint_tool-0.7.5/checkpoint/__init__.py
+-rw-r--r--   0        0        0     2763 2023-05-09 01:19:11.117797 checkpoint_tool-0.7.5/checkpoint/app.py
+-rw-r--r--   0        0        0     4004 2023-05-03 13:31:12.624944 checkpoint_tool-0.7.5/checkpoint/database.py
+-rw-r--r--   0        0        0     7214 2023-05-09 01:48:29.158359 checkpoint_tool-0.7.5/checkpoint/graph.py
+-rw-r--r--   0        0        0    10996 2023-05-09 01:49:51.784680 checkpoint_tool-0.7.5/checkpoint/task.py
+-rw-r--r--   0        0        0     1461 2023-05-03 14:04:28.456816 checkpoint_tool-0.7.5/checkpoint/types.py
+-rw-r--r--   0        0        0      676 2023-05-09 01:49:27.861375 checkpoint_tool-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     8007 1970-01-01 00:00:00.000000 checkpoint_tool-0.7.5/PKG-INFO
```

### Comparing `checkpoint_tool-0.7.4/README.md` & `checkpoint_tool-0.7.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -168,29 +168,27 @@
 ```python
 class LargeOutputTask(Task, compress_level=-1):
     ...
 ```
 
 ### Data directories
 
-Use `DataPath(name)` to get a fresh path dedicated to each task.
-The parent directory is automatically created at
+Use `task.task_directory` to get a fresh path dedicated to each task.
+The directory is automatically created at
 `{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{task_name}/data/{cryptic_task_id}`
 and the contents of the directory are cleared at each task call and persist until the task is cleared.
 ```python
-from checkpoint import DataPath
-
 class TrainModel(Task):
-    model_path = DataPath('model.bin')
     ...
 
     def run_task(self) -> str:
         ...
-        model.save(self.model_path)  # Gives `Path('.../model.bin')`
-        return self.model_path
+        model_path = self.task_directory / 'model.bin'
+        model.save(model_path)
+        return model_path
 ```
 
 ### Execution policy configuration
 
 One can control the task execution with `concurrent.futures.Executor` class:
 ```python
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
@@ -214,15 +212,15 @@
     ...
 
 # Queue-level concurrency control
 SomeDownstreamTask().run_graph(rate_limits={'<gpu>': 1})
 SomeDownstreamTask().run_graph(rate_limits={'<memory>': 1})
 
 # Task-level concurrency control
-SomeDownstreamTask().run_graph(rate_limits={TaskUsingGPU.task_config.name: 1})
+SomeDownstreamTask().run_graph(rate_limits={TaskUsingGPU.task_name: 1})
 
 ```
 
 ### Commandline tool
 We can use checkpoint-tool from commandline like `python -m checkpoint.app path/to/taskfile.py`, where `taskfile.py` defines the `main` task as follows:
 ```python
 # taskfile.py
```

### Comparing `checkpoint_tool-0.7.4/checkpoint/__init__.py` & `checkpoint_tool-0.7.5/checkpoint/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,14 @@
     - Automatic cache/data management (source code change detection, cache/data dependency tracking).
     - Task queue with rate limits.
 
 Limitations:
     - No priority-based scheduling.
 """
 from .types import Context
-from .task import infer_task_type, Task, TaskLike, Req, Requires, RequiresList, RequiresDict, Const, DataPath
+from .task import infer_task_type, Task, TaskLike, Req, Requires, RequiresList, RequiresDict, Const
 
 
 __EXPORT__ = [
-        infer_task_type, Task, Req, Requires, RequiresList, RequiresDict, Const, DataPath, TaskLike,
+        infer_task_type, Task, Req, Requires, RequiresList, RequiresDict, Const, TaskLike,
         Context
         ]
```

### Comparing `checkpoint_tool-0.7.4/checkpoint/app.py` & `checkpoint_tool-0.7.5/checkpoint/app.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.4/checkpoint/database.py` & `checkpoint_tool-0.7.5/checkpoint/database.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.4/checkpoint/graph.py` & `checkpoint_tool-0.7.5/checkpoint/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,16 @@
             # Submit all leaf tasks
             leftover: dict[ChannelLabels, list[TaskKey]] = {}
             for queue, keys in standby.items():
                 if any(q in rate_limits for q in queue):
                     free = min(rate_limits[q] - occupied[q] for q in queue if q in rate_limits)
                     to_submit, to_hold = keys[:free], keys[free:]
                     for q in queue:
-                        occupied[q] += len(to_submit)
+                        if q in occupied:
+                            occupied[q] += len(to_submit)
                     if to_hold:
                         leftover[queue] = to_hold
                 else:
                     to_submit = keys
 
                 for key in to_submit:
                     future = executor.submit(_run_task, queue, cloudpickle.dumps(graph.get_task(key)))
```

### Comparing `checkpoint_tool-0.7.4/checkpoint/task.py` & `checkpoint_tool-0.7.5/checkpoint/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     def get_prerequisites(self) -> Sequence[TaskWorker[Any]]:
         cls = self.config.task_class
         inst = self.instance
         prerequisites: list[TaskWorker[Any]] = []
         for _, v in inspect.getmembers(cls):
             if isinstance(v, Req):
-                prerequisites.extend([task.task_worker for task in v.get_task_list(inst)])
+                prerequisites.extend([task._task_worker for task in v.get_task_list(inst)])
         assert all(isinstance(p, TaskWorker) for p in prerequisites)
         return prerequisites
 
     def peek_timestamp(self) -> datetime | None:
         try:
             return self.config.db.load_timestamp(self.arg_key)
         except KeyError:
@@ -128,22 +128,25 @@
         return out
 
     def get_result(self) -> R:
         return self.config.db.load(self.arg_key)
 
     def clear(self) -> None:
         db = self.config.db
-        db.delete(self.arg_key)
+        try:
+            db.delete(self.arg_key)
+        except KeyError:
+            pass
         directory = self._directory_uninit
         if directory.exists():
             shutil.rmtree(directory)
 
 
 class TaskType(Generic[P, R], ABC):
-    task_config: TaskConfig[P, R]
+    _task_config: TaskConfig[P, R]
 
     @abstractmethod
     def build_task(self, *args: P.args, **kwargs: P.kwargs) -> None:
         pass
 
     @abstractmethod
     def run_task(self) -> R:
@@ -168,28 +171,37 @@
         ann = inspect.get_annotations(cls, eval_str=True)
         for k, v in ann.items():
             if get_origin(v) is Req and getattr(cls, k, None) is None:
                 req = Req()
                 req.__set_name__(None, k)
                 setattr(cls, k, req)
 
-        cls.task_config = TaskConfig(task_class=cls, channels=channels, compress_level=compress_level)
+        cls._task_config = TaskConfig(task_class=cls, channels=channels, compress_level=compress_level)
         super().__init_subclass__(**kwargs)
 
     def __init__(self, *args: P.args, **kwargs: P.kwargs) -> None:
-        self.task_worker: TaskWorker[R] = TaskWorker.make(
-                self.task_config, self, *args, **kwargs
+        self._task_worker: TaskWorker[R] = TaskWorker.make(
+                self._task_config, self, *args, **kwargs
                 )
 
     @classmethod
+    @property
+    def task_name(cls) -> str:
+        return cls._task_config.name
+
+    @property
+    def task_directory(self) -> Path:
+        return self._task_worker.directory
+
+    @classmethod
     def clear_all_tasks(cls) -> None:
-        cls.task_config.clear_all()
+        cls._task_config.clear_all()
 
     def clear_task(self) -> None:
-        self.task_worker.clear()
+        self._task_worker.clear()
 
     def run_graph(
             self, *,
             executor: Executor | None = None,
             max_workers: int | None = None,
             rate_limits: dict[str, int] | None = None,
             detect_source_change: bool | None = None,
@@ -207,27 +219,25 @@
             max_workers: int | None = None,
             rate_limits: dict[str, int] | None = None,
             detect_source_change: bool | None = None,
             dump_generations: bool = False
             ) -> tuple[R, dict[str, Any]]:
         if detect_source_change is None:
             detect_source_change = Context.detect_source_change
-        graph = TaskGraph.build_from(self.task_worker, detect_source_change=detect_source_change)
+        graph = TaskGraph.build_from(self._task_worker, detect_source_change=detect_source_change)
 
         if executor is None:
             executor = Context.get_executor(max_workers=max_workers)
         else:
             assert max_workers is None
         stats = run_task_graph(graph=graph, executor=executor, rate_limits=rate_limits, dump_graphs=dump_generations)
-        return self.task_worker.get_result(), stats
+        return self._task_worker.get_result(), stats
 
 
 class TaskClassProtocol(Protocol[P, R]):
-    task_config: ClassVar[TaskConfig]
-    task_worker: TaskWorker
     def build_task(self, *args: P.args, **kwargs: P.kwargs) -> None: ...
     def run_task(self) -> R: ...
 
 
 def infer_task_type(cls: Type[TaskClassProtocol[P, R]]) -> Type[TaskType[P, R]]:
     assert issubclass(cls, TaskType), f'{cls} must inherit from {TaskType} to infer task type.'
     return cast(Type[TaskType[P, R]], cls)
@@ -247,15 +257,15 @@
     arguments = _normalize_arguments(fn, *args, **kwargs)
     return cast(Json, json.dumps(arguments, separators=(',', ':'), sort_keys=True, cls=CustomJSONEncoder))
 
 
 class CustomJSONEncoder(json.JSONEncoder):
     def default(self, o):
         if isinstance(o, TaskType):
-            return {'__task__': o.task_worker.to_tuple()}
+            return {'__task__': o._task_worker.to_tuple()}
         else:
             # Let the base class default method raise the TypeError
             return super().default(o)
 
 
 class Req(Generic[T, R]):
     def __set_name__(self, _: Any, name: str) -> None:
@@ -269,20 +279,25 @@
     def __get__(self: Req[TaskLike[U], U], obj: TaskType[..., Any], _=None) -> U: ...
     @overload
     def __get__(self: Req[list[TaskLike[U]], list[U]], obj: TaskType[..., Any], _=None) -> list[U]: ...
     @overload
     def __get__(self: Req[dict[K, TaskLike[U]], dict[K, U]], obj: TaskType[..., Any], _=None) -> dict[K, U]: ...
     def __get__(self, obj: TaskType[..., Any], _=None) -> Any:
         x = getattr(obj, self.private_name)
+
+        def get_worker(task: Task[Any]) -> TaskWorker[Any]:
+            assert isinstance(task, TaskType)
+            return task._task_worker
+
         if isinstance(x, TaskType):
-            return x.task_worker.get_result()
+            return get_worker(x).get_result()
         elif isinstance(x, list):
-            return [t.task_worker.get_result() for t in x]
+            return [get_worker(t).get_result() for t in x]
         elif isinstance(x, dict):
-            return {k: v.task_worker.get_result() for k, v in x.items()}
+            return {k: get_worker(v).get_result() for k, v in x.items()}
         elif isinstance(x, Const):
             return x.value
         else:
             raise TypeError(f'Unsupported requirement type: {type(x)}')
 
     def get_task_list(self, obj: TaskType[..., Any]) -> list[TaskType[..., Any]]:
         x = getattr(obj, self.private_name, None)
@@ -310,20 +325,7 @@
 Task = TaskType[..., R]
 TaskLike = Task[R] | Const[R]
 
 
 Requires = Req[TaskLike[R], R]
 RequiresList = Req[Sequence[TaskLike[R]], list[R]]
 RequiresDict = Req[Mapping[K, TaskLike[R]], dict[K, R]]
-
-
-class DataPath:
-    def __init__(self, name: str) -> None:
-        self.name = name
-
-    def __get__(self, obj: TaskType[..., Any], _=None) -> Path:
-        return obj.task_worker.directory / self.name
-
-
-class DataDir:
-    def __get__(self, obj: TaskType[..., Any], _=None) -> Path:
-        return obj.task_worker.directory
```

### Comparing `checkpoint_tool-0.7.4/checkpoint/types.py` & `checkpoint_tool-0.7.5/checkpoint/types.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.4/pyproject.toml` & `checkpoint_tool-0.7.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkpoint-tool"
-version = "0.7.4"
+version = "0.7.5"
 description = "A lightweight workflow management tool written in pure Python"
 authors = ["Kohei Miyaguchi <koheimiyaguchi@gmail.com>"]
 license = "MIT License"
 homepage = "https://github.com/koheimiya/checkpoint"
 repository = "https://github.com/koheimiya/checkpoint"
 readme = "README.md"
 packages = [{include = "checkpoint"}]
```

### Comparing `checkpoint_tool-0.7.4/PKG-INFO` & `checkpoint_tool-0.7.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkpoint-tool
-Version: 0.7.4
+Version: 0.7.5
 Summary: A lightweight workflow management tool written in pure Python
 Home-page: https://github.com/koheimiya/checkpoint
 License: MIT
 Author: Kohei Miyaguchi
 Author-email: koheimiyaguchi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -190,29 +190,27 @@
 ```python
 class LargeOutputTask(Task, compress_level=-1):
     ...
 ```
 
 ### Data directories
 
-Use `DataPath(name)` to get a fresh path dedicated to each task.
-The parent directory is automatically created at
+Use `task.task_directory` to get a fresh path dedicated to each task.
+The directory is automatically created at
 `{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{task_name}/data/{cryptic_task_id}`
 and the contents of the directory are cleared at each task call and persist until the task is cleared.
 ```python
-from checkpoint import DataPath
-
 class TrainModel(Task):
-    model_path = DataPath('model.bin')
     ...
 
     def run_task(self) -> str:
         ...
-        model.save(self.model_path)  # Gives `Path('.../model.bin')`
-        return self.model_path
+        model_path = self.task_directory / 'model.bin'
+        model.save(model_path)
+        return model_path
 ```
 
 ### Execution policy configuration
 
 One can control the task execution with `concurrent.futures.Executor` class:
 ```python
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
@@ -236,15 +234,15 @@
     ...
 
 # Queue-level concurrency control
 SomeDownstreamTask().run_graph(rate_limits={'<gpu>': 1})
 SomeDownstreamTask().run_graph(rate_limits={'<memory>': 1})
 
 # Task-level concurrency control
-SomeDownstreamTask().run_graph(rate_limits={TaskUsingGPU.task_config.name: 1})
+SomeDownstreamTask().run_graph(rate_limits={TaskUsingGPU.task_name: 1})
 
 ```
 
 ### Commandline tool
 We can use checkpoint-tool from commandline like `python -m checkpoint.app path/to/taskfile.py`, where `taskfile.py` defines the `main` task as follows:
 ```python
 # taskfile.py
```

