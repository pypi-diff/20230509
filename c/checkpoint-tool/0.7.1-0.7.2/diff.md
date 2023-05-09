# Comparing `tmp/checkpoint_tool-0.7.1.tar.gz` & `tmp/checkpoint_tool-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkpoint_tool-0.7.1.tar", max compression
+gzip compressed data, was "checkpoint_tool-0.7.2.tar", max compression
```

## Comparing `checkpoint_tool-0.7.1.tar` & `checkpoint_tool-0.7.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6998 2023-05-08 16:31:17.720383 checkpoint_tool-0.7.1/README.md
--rw-r--r--   0        0        0      628 2023-05-08 16:37:27.127303 checkpoint_tool-0.7.1/checkpoint/__init__.py
--rw-r--r--   0        0        0     2325 2023-05-08 16:42:33.005130 checkpoint_tool-0.7.1/checkpoint/app.py
--rw-r--r--   0        0        0    23235 2023-05-03 09:41:14.000902 checkpoint_tool-0.7.1/checkpoint/checkpoint_legacy.py
--rw-r--r--   0        0        0     4004 2023-05-03 13:31:12.624944 checkpoint_tool-0.7.1/checkpoint/database.py
--rw-r--r--   0        0        0     6933 2023-05-04 14:52:06.276241 checkpoint_tool-0.7.1/checkpoint/graph.py
--rw-r--r--   0        0        0    10493 2023-05-08 16:36:35.511414 checkpoint_tool-0.7.1/checkpoint/task.py
--rw-r--r--   0        0        0     1461 2023-05-03 14:04:28.456816 checkpoint_tool-0.7.1/checkpoint/types.py
--rw-r--r--   0        0        0      676 2023-05-08 16:42:22.147879 checkpoint_tool-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     7852 1970-01-01 00:00:00.000000 checkpoint_tool-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     7146 2023-05-09 00:58:27.328907 checkpoint_tool-0.7.2/README.md
+-rw-r--r--   0        0        0      628 2023-05-08 16:37:27.127303 checkpoint_tool-0.7.2/checkpoint/__init__.py
+-rw-r--r--   0        0        0     2326 2023-05-09 00:25:34.051079 checkpoint_tool-0.7.2/checkpoint/app.py
+-rw-r--r--   0        0        0    23235 2023-05-03 09:41:14.000902 checkpoint_tool-0.7.2/checkpoint/checkpoint_legacy.py
+-rw-r--r--   0        0        0     4004 2023-05-03 13:31:12.624944 checkpoint_tool-0.7.2/checkpoint/database.py
+-rw-r--r--   0        0        0     7168 2023-05-09 00:56:30.108576 checkpoint_tool-0.7.2/checkpoint/graph.py
+-rw-r--r--   0        0        0    10978 2023-05-09 00:55:48.411714 checkpoint_tool-0.7.2/checkpoint/task.py
+-rw-r--r--   0        0        0     1461 2023-05-03 14:04:28.456816 checkpoint_tool-0.7.2/checkpoint/types.py
+-rw-r--r--   0        0        0      676 2023-05-09 00:58:56.073495 checkpoint_tool-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     8000 1970-01-01 00:00:00.000000 checkpoint_tool-0.7.2/PKG-INFO
```

### Comparing `checkpoint_tool-0.7.1/README.md` & `checkpoint_tool-0.7.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -51,34 +51,34 @@
     def main(self) -> int:
         # Here we define the main computation of the task,
         # which is delayed until it is necessary.
 
         # The return values of the prerequisite tasks are accessible via the descriptors:
         return self.prev1 + self.prev2
 
-# To run tasks, use the `run_task()` method.
-ans = Choose(6, 3).worker.run_task()  # `ans` should be 6 Choose 3, which is 20.
+# To run the task as well as upstream workflow, use the `run_graph()` method.
+ans = Choose(6, 3).run_graph()  # `ans` should be 6 Choose 3, which is 20.
 
 # It greedily executes all the necessary tasks as parallel as possible
-# and then spits out the return value of the task on which we call `run_task()`.
+# and then spits out the return value of the task on which we call `run_graph()`.
 # The return values of the intermediate tasks are cached at
 # `{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{task_name}/...`
 # and reused on the fly whenever possible.
 ```
 
 ### Deleting cache
 
 It is possible to selectively discard cache: 
 ```python
 # After some modificaiton of `Choose(3, 3)`,
 # selectively discard the cache corresponding to the modification.
 Choose(3, 3).clear_task()
 
 # `ans` is recomputed tracing back to the computation of `Choose(3, 3)`.
-ans = Choose(6, 3).run_task()
+ans = Choose(6, 3).run_graph()
 
 # Delete all the cache associated with `Choose`,
 # equivalent to `rm -r {$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.Choose`.
 Choose.clear_all_tasks()            
 ```
 
 ### Limitations of Task I/O
@@ -102,15 +102,15 @@
     def init(self, json_params):
         self.x1 = T1(**json_params['param1'])
         self.x2 = T2(**json_params['param2'])
 
     def main(self):
         ...
 
-result = T3({'param1': { ... }, 'param2': { ... }}).run_task()
+result = T3({'param1': { ... }, 'param2': { ... }}).run_graph()
 ```
 
 Otherwise they can be passed via `Task` and `Req`:
 ```python
 Dataset = ...  # Some complex data structure
 Model = ...    # Some complex data structure
 
@@ -141,15 +141,15 @@
     def main(self) -> float:
         ...
 
 
 dataset_task = LoadDataset()
 model_task = TrainModel(dataset)
 score_task = ScoreModel(dataset, model)
-print(score_task.run_task()
+print(score_task.run_graph()
 ```
 
 `Req` accepts a list/dict of tasks and automatically unfolds it.
 ```python
 from checkpoint import RequiresDict
 
 
@@ -195,35 +195,39 @@
 ```python
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 
 class MyTask(Task):
     ...
 
 # Limit the number of parallel workers
-MyTask().run(executor=ProcessPoolExecutor(max_workers=2))
+MyTask().run_graph(executor=ProcessPoolExecutor(max_workers=2))
 
 # Thread-based parallelism
-MyTask().run(executor=ThreadPoolExecutor())
+MyTask().run_graph(executor=ThreadPoolExecutor())
 ```
 
-One can also control the concurrency at a task/queue level:
+One can also control the concurrency at a task/channel level:
 ```python
-class TaskUsingGPU(Task, queue='gpu'):
+class TaskUsingGPU(Task, channel='<gpu>'):
     ...
 
-class AnotherTaskUsingGPU(Task, queue='gpu'):
+class AnotherTaskUsingGPU(Task, channel=['<gpu>', '<memory>']):
     ...
 
-SomeDownstreamTask().run(rate_limits={'gpu': 1})  # Queue-level concurrency control
-SomeDownstreamTask().run(rate_limits={MemoryIntensiveTask.queue: 1})  # Task-level concurrency control
+# Queue-level concurrency control
+SomeDownstreamTask().run_graph(rate_limits={'<gpu>': 1})
+SomeDownstreamTask().run_graph(rate_limits={'<memory>': 1})
+
+# Task-level concurrency control
+SomeDownstreamTask().run_graph(rate_limits={TaskUsingGPU.task_config.name: 1})
 
 ```
 
 ### Commandline tool
-We can use checkpoint-tool from commandline like `python -m checkpoint path/to/taskfile.py`, where `taskfile.py` defines the `main` task as follows:
+We can use checkpoint-tool from commandline like `python -m checkpoint.app path/to/taskfile.py`, where `taskfile.py` defines the `main` task as follows:
 ```python
 # taskfile.py
 
 class Main(Task):
     ...
 ```
 The command runs the `Main()` task and stores the cache right next to `taskfile.py` as `.cache/checkpoint/...`.
```

### Comparing `checkpoint_tool-0.7.1/checkpoint/__init__.py` & `checkpoint_tool-0.7.2/checkpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.1/checkpoint/app.py` & `checkpoint_tool-0.7.2/checkpoint/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,13 +42,13 @@
     # spec.loader.exec_module(module)
 
     # Run the main task
     entrypoint_fn = getattr(module, entrypoint)
     assert issubclass(entrypoint_fn, TaskType), \
             f'Taskfile `{taskfile}` should contain a task(factory) `{entrypoint}`, but found `{entrypoint_fn}`.'
     task = entrypoint_fn()
-    task.run_task_with_stats(rate_limits=rate_limits)
+    task.run_graph_with_stats(rate_limits=rate_limits)
     return 0
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `checkpoint_tool-0.7.1/checkpoint/checkpoint_legacy.py` & `checkpoint_tool-0.7.2/checkpoint/checkpoint_legacy.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.1/checkpoint/database.py` & `checkpoint_tool-0.7.2/checkpoint/database.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.1/checkpoint/graph.py` & `checkpoint_tool-0.7.2/checkpoint/graph.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,18 +12,21 @@
 
 from .types import Json, TaskKey
 
 
 LOGGER = logging.getLogger(__name__)
 
 
+ChannelLabels = tuple[str, ...]
+
+
 @runtime_checkable
 class TaskHandlerProtocol(Protocol):
     @property
-    def queue(self) -> str: ...
+    def channels(self) -> ChannelLabels: ...
     @property
     def source_timestamp(self) -> datetime: ...
     def to_tuple(self) -> TaskKey: ...
     def get_prerequisites(self) -> Sequence[TaskHandlerProtocol]: ...
     def peek_timestamp(self) -> datetime | None: ...
     def set_result(self) -> None: ...
 
@@ -84,35 +87,35 @@
         self.G.remove_nodes_from(to_remove)
 
     def _transitive_reduction(self) -> None:
         TR = nx.transitive_reduction(self.G)
         TR.add_nodes_from(self.G.nodes(data=True))
         self.G = TR
 
-    def get_initial_tasks(self) -> dict[str, list[TaskKey]]:
+    def get_initial_tasks(self) -> dict[ChannelLabels, list[TaskKey]]:
         leaves = [x for x in self.G if self.G.in_degree(x) == 0]
-        return self._group_by_queue(leaves)
+        return self._group_by_channels(leaves)
 
-    def _group_by_queue(self, nodes: list[TaskKey]) -> dict[str, list[TaskKey]]:
+    def _group_by_channels(self, nodes: list[TaskKey]) -> dict[ChannelLabels, list[TaskKey]]:
         out = defaultdict(list)
         for x in nodes:
-            out[self.get_task(x).queue].append(x)
+            out[self.get_task(x).channels].append(x)
         return out
 
-    def pop_with_new_leaves(self, x: TaskKey, disallow_non_leaf: bool = True) -> dict[str, list[TaskKey]]:
+    def pop_with_new_leaves(self, x: TaskKey, disallow_non_leaf: bool = True) -> dict[ChannelLabels, list[TaskKey]]:
         if disallow_non_leaf:
             assert not list(self.G.predecessors(x))
 
         new_leaves: list[TaskKey] = []
         for y in self.G.successors(x):
             if self.G.in_degree(y) == 1:
                 new_leaves.append(y)
 
         self.G.remove_node(x)
-        return self._group_by_queue(new_leaves)
+        return self._group_by_channels(new_leaves)
 
     def get_nodes_by_task(self) -> dict[str, list[Json]]:
         out: dict[str, list[Json]] = defaultdict(list)
         for x in self.G:
             path, args = x
             out[path].append(args)
         return dict(out)
@@ -133,33 +136,34 @@
     # Read concurrency budgets
     if rate_limits is None:
         rate_limits = {}
     occupied = {k: 0 for k in rate_limits}
 
     # Execute tasks
     standby = graph.get_initial_tasks()
-    in_process: set[Future[tuple[str, TaskKey]]] = set()
+    in_process: set[Future[tuple[ChannelLabels, TaskKey]]] = set()
     with executor as executor:
         while standby or in_process:
             # Log some stats
             LOGGER.info(
                     f'nodes: {graph.size}, '
                     f'standby: {len(standby)}, '
                     f'in_process: {len(in_process)}'
                     )
             if dump_graphs:
                 info['generations'].append(graph.get_nodes_by_task())
 
             # Submit all leaf tasks
-            leftover: dict[str, list[TaskKey]] = {}
+            leftover: dict[ChannelLabels, list[TaskKey]] = {}
             for queue, keys in standby.items():
-                if queue in rate_limits:
-                    free = rate_limits[queue] - occupied[queue]
+                if any(q in rate_limits for q in queue):
+                    free = min(rate_limits[q] - occupied[q] for q in queue if q in rate_limits)
                     to_submit, to_hold = keys[:free], keys[free:]
-                    occupied[queue] += len(to_submit)
+                    for q in queue:
+                        occupied[q] += len(to_submit)
                     if to_hold:
                         leftover[queue] = to_hold
                 else:
                     to_submit = keys
 
                 for key in to_submit:
                     future = executor.submit(_run_task, queue, cloudpickle.dumps(graph.get_task(key)))
@@ -170,29 +174,30 @@
 
             # Update graph
             standby = defaultdict(list, leftover)
             for done_future in done:
                 queue_done, x_done = done_future.result()
 
                 # Update occupied
-                if queue_done in occupied:
-                    occupied[queue_done] -= 1
-                    assert occupied[queue_done] >= 0
+                for q in queue_done:
+                    if q in occupied:
+                        occupied[q] -= 1
+                        assert occupied[q] >= 0
 
                 # Remove node from graph
                 ys = graph.pop_with_new_leaves(x_done)
 
                 # Update standby
                 for queue, task in ys.items():
                     standby[queue].extend(task)
 
     # Sanity check
     assert graph.size == 0, f'Graph is not empty. Should not happen.'
     assert all(n == 0 for n in occupied.values()), 'Incorrect task count. Should not happen.'
     return info
 
 
-def _run_task(queue: str, task_data: bytes) -> tuple[str, TaskKey]:  # queue, (dbname, key)
+def _run_task(queue: ChannelLabels, task_data: bytes) -> tuple[ChannelLabels, TaskKey]:  # queue, (dbname, key)
     task = cloudpickle.loads(task_data)
     assert isinstance(task, TaskHandlerProtocol)
     task.set_result()
     return queue, task.to_tuple()
```

### Comparing `checkpoint_tool-0.7.1/checkpoint/task.py` & `checkpoint_tool-0.7.2/checkpoint/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
+from collections.abc import Iterable
 from typing import Callable, ClassVar, Generic, Mapping, Protocol, Self, Sequence, Type, TypeVar, Any, cast, overload, get_origin
 from typing_extensions import ParamSpec
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 from concurrent.futures import Executor
 import ast
@@ -32,22 +33,22 @@
 
 
 class TaskConfig(Generic[P, R]):
     """ Information specific to a task class (not instance) """
     def __init__(
             self,
             task_class: Type[TaskType[P, R]],
-            queue: str | None,
+            channels: tuple[str, ...],
             compress_level: int,
             ) -> None:
 
         self.task_class = task_class
         self.name = _serialize_function(task_class)
         self.db = Database.make(name=self.name, compress_level=compress_level)
-        self.queue = queue if queue is not None else f'<{self.name}>'
+        self.channels = (self.name,) + channels
         self.worker_registry: dict[Json, TaskWorker[R]] = {}
 
         source = inspect.getsource(task_class)
         formatted_source = ast.unparse(ast.parse(source))
         self.source_timestamp = self.db.update_source_if_necessary(formatted_source)
 
     @property
@@ -57,32 +58,32 @@
     def clear_all(self) -> None:
         self.db.clear()
 
 
 class TaskWorker(Generic[R]):
     @classmethod
     def make(cls, config: TaskConfig[P, R], instance: TaskType[P, R], *args: P.args, **kwargs: P.kwargs) -> Self:
-        arg_key = _serialize_arguments(instance.init, *args, **kwargs)
+        arg_key = _serialize_arguments(instance.build_task, *args, **kwargs)
         worker = config.worker_registry.get(arg_key, None)
         if worker is not None:
             return worker
 
-        instance.init(*args, **kwargs)
+        instance.build_task(*args, **kwargs)
         worker = TaskWorker[R](config=config, instance=instance, arg_key=arg_key)
         config.worker_registry[arg_key] = worker
         return worker
 
     def __init__(self, config: TaskConfig[..., R], instance: TaskType[..., R], arg_key: Json) -> None:
         self.config = config
         self.instance = instance
         self.arg_key = arg_key
 
     @property
-    def queue(self) -> str:
-        return self.config.queue
+    def channels(self) -> tuple[str, ...]:
+        return self.config.channels
 
     @property
     def source_timestamp(self) -> datetime:
         return self.config.source_timestamp
 
     def to_tuple(self) -> TaskKey:
         return (self.config.name, self.arg_key)
@@ -103,15 +104,15 @@
         except KeyError:
             return None
 
     def set_result(self) -> None:
         db = self.config.db
         if self.directory.exists():
             shutil.rmtree(self.directory)
-        out = self.instance.main()
+        out = self.instance.run_task()
         db.save(self.arg_key, out)
 
     @property
     def _relative_path(self) -> str:
         _, arg_str = self.to_tuple()
         id_ = base64.urlsafe_b64encode(zlib.compress(arg_str.encode(), level=9)).decode().replace('=', '')
         return os.path.join(*[id_[i:i+255] for i in range(0, len(id_), 255)])
@@ -137,63 +138,74 @@
             shutil.rmtree(directory)
 
 
 class TaskType(Generic[P, R], ABC):
     task_config: TaskConfig[P, R]
 
     @abstractmethod
-    def init(self, *args: P.args, **kwargs: P.kwargs) -> None:
+    def build_task(self, *args: P.args, **kwargs: P.kwargs) -> None:
         pass
 
     @abstractmethod
-    def main(self) -> R:
+    def run_task(self) -> R:
         pass
 
     def __init_subclass__(cls, **kwargs: Any) -> None:
-        queue = kwargs.pop('queue', None)
+        _channel = kwargs.pop('channel', None)
+        channels: tuple[str, ...]
+        if isinstance(_channel, str):
+            channels = (_channel,)
+        elif isinstance(_channel, Iterable):
+            channels = tuple(_channel)
+            assert all(isinstance(q, str) for q in channels)
+        elif _channel is None:
+            channels = tuple()
+        else:
+            raise ValueError('Invalid channel value:', _channel)
+
         compress_level = kwargs.pop('compress_level', 0)
 
         # Fill missing requirement
         ann = inspect.get_annotations(cls, eval_str=True)
         for k, v in ann.items():
             if get_origin(v) is Req and getattr(cls, k, None) is None:
                 req = Req()
                 req.__set_name__(None, k)
                 setattr(cls, k, req)
 
-        cls.task_config = TaskConfig(task_class=cls, queue=queue, compress_level=compress_level)
+        cls.task_config = TaskConfig(task_class=cls, channels=channels, compress_level=compress_level)
         super().__init_subclass__(**kwargs)
 
     def __init__(self, *args: P.args, **kwargs: P.kwargs) -> None:
         self.task_worker: TaskWorker[R] = TaskWorker.make(
                 self.task_config, self, *args, **kwargs
                 )
 
     @classmethod
     def clear_all_tasks(cls) -> None:
         cls.task_config.clear_all()
 
     def clear_task(self) -> None:
         self.task_worker.clear()
 
-    def run_task(
+    def run_graph(
             self, *,
             executor: Executor | None = None,
             max_workers: int | None = None,
             rate_limits: dict[str, int] | None = None,
             detect_source_change: bool | None = None,
             ) -> R:
-        return self.run_task_with_stats(
+        return self.run_graph_with_stats(
                 executor=executor,
                 max_workers=max_workers,
                 rate_limits=rate_limits,
                 detect_source_change=detect_source_change
                 )[0]
 
-    def run_task_with_stats(
+    def run_graph_with_stats(
             self, *,
             executor: Executor | None = None,
             max_workers: int | None = None,
             rate_limits: dict[str, int] | None = None,
             detect_source_change: bool | None = None,
             dump_generations: bool = False
             ) -> tuple[R, dict[str, Any]]:
@@ -208,16 +220,16 @@
         stats = run_task_graph(graph=graph, executor=executor, rate_limits=rate_limits, dump_graphs=dump_generations)
         return self.task_worker.get_result(), stats
 
 
 class TaskClassProtocol(Protocol[P, R]):
     task_config: ClassVar[TaskConfig]
     task_worker: TaskWorker
-    def init(self, *args: P.args, **kwargs: P.kwargs) -> None: ...
-    def main(self) -> R: ...
+    def build_task(self, *args: P.args, **kwargs: P.kwargs) -> None: ...
+    def run_task(self) -> R: ...
 
 
 def infer_task_type(cls: Type[TaskClassProtocol[P, R]]) -> Type[TaskType[P, R]]:
     assert issubclass(cls, TaskType), f'{cls} must inherit from {TaskType} to infer task type.'
     return cast(Type[TaskType[P, R]], cls)
```

### Comparing `checkpoint_tool-0.7.1/checkpoint/types.py` & `checkpoint_tool-0.7.2/checkpoint/types.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.1/pyproject.toml` & `checkpoint_tool-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkpoint-tool"
-version = "0.7.1"
+version = "0.7.2"
 description = "A lightweight workflow management tool written in pure Python"
 authors = ["Kohei Miyaguchi <koheimiyaguchi@gmail.com>"]
 license = "MIT License"
 homepage = "https://github.com/koheimiya/checkpoint"
 repository = "https://github.com/koheimiya/checkpoint"
 readme = "README.md"
 packages = [{include = "checkpoint"}]
```

### Comparing `checkpoint_tool-0.7.1/PKG-INFO` & `checkpoint_tool-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkpoint-tool
-Version: 0.7.1
+Version: 0.7.2
 Summary: A lightweight workflow management tool written in pure Python
 Home-page: https://github.com/koheimiya/checkpoint
 License: MIT
 Author: Kohei Miyaguchi
 Author-email: koheimiyaguchi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -73,34 +73,34 @@
     def main(self) -> int:
         # Here we define the main computation of the task,
         # which is delayed until it is necessary.
 
         # The return values of the prerequisite tasks are accessible via the descriptors:
         return self.prev1 + self.prev2
 
-# To run tasks, use the `run_task()` method.
-ans = Choose(6, 3).worker.run_task()  # `ans` should be 6 Choose 3, which is 20.
+# To run the task as well as upstream workflow, use the `run_graph()` method.
+ans = Choose(6, 3).run_graph()  # `ans` should be 6 Choose 3, which is 20.
 
 # It greedily executes all the necessary tasks as parallel as possible
-# and then spits out the return value of the task on which we call `run_task()`.
+# and then spits out the return value of the task on which we call `run_graph()`.
 # The return values of the intermediate tasks are cached at
 # `{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{task_name}/...`
 # and reused on the fly whenever possible.
 ```
 
 ### Deleting cache
 
 It is possible to selectively discard cache: 
 ```python
 # After some modificaiton of `Choose(3, 3)`,
 # selectively discard the cache corresponding to the modification.
 Choose(3, 3).clear_task()
 
 # `ans` is recomputed tracing back to the computation of `Choose(3, 3)`.
-ans = Choose(6, 3).run_task()
+ans = Choose(6, 3).run_graph()
 
 # Delete all the cache associated with `Choose`,
 # equivalent to `rm -r {$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.Choose`.
 Choose.clear_all_tasks()            
 ```
 
 ### Limitations of Task I/O
@@ -124,15 +124,15 @@
     def init(self, json_params):
         self.x1 = T1(**json_params['param1'])
         self.x2 = T2(**json_params['param2'])
 
     def main(self):
         ...
 
-result = T3({'param1': { ... }, 'param2': { ... }}).run_task()
+result = T3({'param1': { ... }, 'param2': { ... }}).run_graph()
 ```
 
 Otherwise they can be passed via `Task` and `Req`:
 ```python
 Dataset = ...  # Some complex data structure
 Model = ...    # Some complex data structure
 
@@ -163,15 +163,15 @@
     def main(self) -> float:
         ...
 
 
 dataset_task = LoadDataset()
 model_task = TrainModel(dataset)
 score_task = ScoreModel(dataset, model)
-print(score_task.run_task()
+print(score_task.run_graph()
 ```
 
 `Req` accepts a list/dict of tasks and automatically unfolds it.
 ```python
 from checkpoint import RequiresDict
 
 
@@ -217,35 +217,39 @@
 ```python
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 
 class MyTask(Task):
     ...
 
 # Limit the number of parallel workers
-MyTask().run(executor=ProcessPoolExecutor(max_workers=2))
+MyTask().run_graph(executor=ProcessPoolExecutor(max_workers=2))
 
 # Thread-based parallelism
-MyTask().run(executor=ThreadPoolExecutor())
+MyTask().run_graph(executor=ThreadPoolExecutor())
 ```
 
-One can also control the concurrency at a task/queue level:
+One can also control the concurrency at a task/channel level:
 ```python
-class TaskUsingGPU(Task, queue='gpu'):
+class TaskUsingGPU(Task, channel='<gpu>'):
     ...
 
-class AnotherTaskUsingGPU(Task, queue='gpu'):
+class AnotherTaskUsingGPU(Task, channel=['<gpu>', '<memory>']):
     ...
 
-SomeDownstreamTask().run(rate_limits={'gpu': 1})  # Queue-level concurrency control
-SomeDownstreamTask().run(rate_limits={MemoryIntensiveTask.queue: 1})  # Task-level concurrency control
+# Queue-level concurrency control
+SomeDownstreamTask().run_graph(rate_limits={'<gpu>': 1})
+SomeDownstreamTask().run_graph(rate_limits={'<memory>': 1})
+
+# Task-level concurrency control
+SomeDownstreamTask().run_graph(rate_limits={TaskUsingGPU.task_config.name: 1})
 
 ```
 
 ### Commandline tool
-We can use checkpoint-tool from commandline like `python -m checkpoint path/to/taskfile.py`, where `taskfile.py` defines the `main` task as follows:
+We can use checkpoint-tool from commandline like `python -m checkpoint.app path/to/taskfile.py`, where `taskfile.py` defines the `main` task as follows:
 ```python
 # taskfile.py
 
 class Main(Task):
     ...
 ```
 The command runs the `Main()` task and stores the cache right next to `taskfile.py` as `.cache/checkpoint/...`.
```

