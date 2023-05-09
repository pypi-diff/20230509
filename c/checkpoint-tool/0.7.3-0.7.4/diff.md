# Comparing `tmp/checkpoint_tool-0.7.3.tar.gz` & `tmp/checkpoint_tool-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkpoint_tool-0.7.3.tar", max compression
+gzip compressed data, was "checkpoint_tool-0.7.4.tar", max compression
```

## Comparing `checkpoint_tool-0.7.3.tar` & `checkpoint_tool-0.7.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     7146 2023-05-09 00:58:27.328907 checkpoint_tool-0.7.3/README.md
--rw-r--r--   0        0        0      628 2023-05-08 16:37:27.127303 checkpoint_tool-0.7.3/checkpoint/__init__.py
--rw-r--r--   0        0        0     2435 2023-05-09 01:03:53.977120 checkpoint_tool-0.7.3/checkpoint/app.py
--rw-r--r--   0        0        0     4004 2023-05-03 13:31:12.624944 checkpoint_tool-0.7.3/checkpoint/database.py
--rw-r--r--   0        0        0     7168 2023-05-09 00:56:30.108576 checkpoint_tool-0.7.3/checkpoint/graph.py
--rw-r--r--   0        0        0    10978 2023-05-09 00:55:48.411714 checkpoint_tool-0.7.3/checkpoint/task.py
--rw-r--r--   0        0        0     1461 2023-05-03 14:04:28.456816 checkpoint_tool-0.7.3/checkpoint/types.py
--rw-r--r--   0        0        0      676 2023-05-09 01:07:06.182237 checkpoint_tool-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     8000 1970-01-01 00:00:00.000000 checkpoint_tool-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     7222 2023-05-09 01:08:27.319327 checkpoint_tool-0.7.4/README.md
+-rw-r--r--   0        0        0      628 2023-05-08 16:37:27.127303 checkpoint_tool-0.7.4/checkpoint/__init__.py
+-rw-r--r--   0        0        0     2763 2023-05-09 01:19:11.117797 checkpoint_tool-0.7.4/checkpoint/app.py
+-rw-r--r--   0        0        0     4004 2023-05-03 13:31:12.624944 checkpoint_tool-0.7.4/checkpoint/database.py
+-rw-r--r--   0        0        0     7168 2023-05-09 00:56:30.108576 checkpoint_tool-0.7.4/checkpoint/graph.py
+-rw-r--r--   0        0        0    10978 2023-05-09 00:55:48.411714 checkpoint_tool-0.7.4/checkpoint/task.py
+-rw-r--r--   0        0        0     1461 2023-05-03 14:04:28.456816 checkpoint_tool-0.7.4/checkpoint/types.py
+-rw-r--r--   0        0        0      676 2023-05-09 01:21:38.550790 checkpoint_tool-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     8076 1970-01-01 00:00:00.000000 checkpoint_tool-0.7.4/PKG-INFO
```

### Comparing `checkpoint_tool-0.7.3/README.md` & `checkpoint_tool-0.7.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -29,30 +29,30 @@
     # Inside a task, we first declare the values that must be computed upstream with the descriptor `Req`.
     # In this example, `Choose(n, k)` depends on `Choose(n - 1, k - 1)` and `Choose(n - 1, k)`,
     # so it requires two `int` values.
     # Either the type annotation `Requires[...]` or the assignment `= Req()` may be omitted.
     prev1: Requires[int] = Req()
     prev2: Requires[int] = Req()
 
-    def init(self, n: int, k: int):
+    def build_task(self, n: int, k: int):
         # The prerequisite tasks and the other instance attributes are prepared here.
         # It thus recursively defines all the tasks we need to run this task,
         # i.e., the entire upstream workflow.
 
         if 0 < k < n:
             self.prev1 = Choose(n - 1, k - 1)
             self.prev2 = Choose(n - 1, k)
         elif k == 0 or k == n:
             # We can just pass a value to a requirement slot directly without running tasks.
             self.prev1 = Const(0)
             self.prev2 = Const(1)
         else:
             raise ValueError(f'{(n, k)}')
 
-    def main(self) -> int:
+    def run_task(self) -> int:
         # Here we define the main computation of the task,
         # which is delayed until it is necessary.
 
         # The return values of the prerequisite tasks are accessible via the descriptors:
         return self.prev1 + self.prev2
 
 # To run the task as well as upstream workflow, use the `run_graph()` method.
@@ -82,67 +82,67 @@
 ```
 
 ### Limitations of Task I/O
 
 The arguments of the `init` method can be anything JSON serializable:
 ```python
 class T1(Task):
-    def init(self, **param1):
+    def build_task(self, **param1):
         ...
     ...
 
 class T2(Task):
-    def init(self, **param2):
+    def build_task(self, **param2):
         ...
     ...
 
 class T3(Task):
     x1 = Req()
     x2 = Req()
 
-    def init(self, json_params):
+    def build_task(self, json_params):
         self.x1 = T1(**json_params['param1'])
         self.x2 = T2(**json_params['param2'])
 
-    def main(self):
+    def run_task(self):
         ...
 
 result = T3({'param1': { ... }, 'param2': { ... }}).run_graph()
 ```
 
 Otherwise they can be passed via `Task` and `Req`:
 ```python
 Dataset = ...  # Some complex data structure
 Model = ...    # Some complex data structure
 
 class LoadDataset(Task):
-    def init(self):
+    def build_task(self):
         pass
 
-    def main(self) -> Dataset:
+    def run_task(self) -> Dataset:
         ...
 
 class TrainModel(Task):
     dataset: Requires[Datset]
 
-    def init(self, dataset_task: Task[Dataset]):
+    def build_task(self, dataset_task: Task[Dataset]):
         self.dataset = dataset_task
 
-    def main(self) -> Model:
+    def run_task(self) -> Model:
         ...
     
 class ScoreModel(Task):
     dataset: Requires[Datset]
     model: Requires[Model]
 
-    def init(self, dataset_task: Task[Dataset], model_task: Task[Model]):
+    def build_task(self, dataset_task: Task[Dataset], model_task: Task[Model]):
         self.dataset = dataset_task
         self.model = model_task
 
-    def main(self) -> float:
+    def run_task(self) -> float:
         ...
 
 
 dataset_task = LoadDataset()
 model_task = TrainModel(dataset)
 score_task = ScoreModel(dataset, model)
 print(score_task.run_graph()
@@ -152,18 +152,18 @@
 ```python
 from checkpoint import RequiresDict
 
 
 class SummarizeScores(Task):
     scores: RequiresDict[str, float] = Req()  # Again, type annotation or assignment may be omitted.
 
-    def init(self, task_dict: dict[str, Task[float]]):
+    def build_task(self, task_dict: dict[str, Task[float]]):
         self.scores = task_dict
 
-    def main(self) -> float:
+    def run_task(self) -> float:
         return sum(self.scores.values()) / len(self.scores)  # We have access to the dict of the results.
 ```
 
 The output of the `main` method should be serializable with `cloudpickle`.
 Large outputs can be stored with compression via `zlib`:
 ```python
 class LargeOutputTask(Task, compress_level=-1):
@@ -179,15 +179,15 @@
 ```python
 from checkpoint import DataPath
 
 class TrainModel(Task):
     model_path = DataPath('model.bin')
     ...
 
-    def main(self) -> str:
+    def run_task(self) -> str:
         ...
         model.save(self.model_path)  # Gives `Path('.../model.bin')`
         return self.model_path
 ```
 
 ### Execution policy configuration
```

### Comparing `checkpoint_tool-0.7.3/checkpoint/__init__.py` & `checkpoint_tool-0.7.4/checkpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.3/checkpoint/app.py` & `checkpoint_tool-0.7.4/checkpoint/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,24 @@
 @click.argument('taskfile', type=Path)
 @click.option('-e', '--entrypoint', default='Main', help='Task name for entrypoint.')
 @click.option('-t', '--exec-type', type=click.Choice(['process', 'thread']), default='process')
 @click.option('-w', '--max-workers', type=int, default=-1)
 @click.option('--cache-dir', type=Path, default=None)
 @click.option('--rate-limits', type=json.loads, default=None, help='JSON dictionary for rate_limits.')
 @click.option('-D', '--detect-source-change', is_flag=True, help='Automatically discard the cache per task once the source code (AST) is changed.')
-def main(taskfile: Path, entrypoint: str, exec_type: str, max_workers: int, cache_dir: Path | None, rate_limits: dict[str, Any] | None, detect_source_change: bool):
+@click.option('--dont-force-entrypoint', is_flag=True, help='Do nothing if the cache of the entripoint task is up-to-date.')
+def main(taskfile: Path,
+         entrypoint: str,
+         exec_type: str,
+         max_workers: int,
+         cache_dir: Path | None,
+         rate_limits: dict[str, Any] | None,
+         detect_source_change: bool,
+         dont_force_entrypoint: bool
+         ) -> int:
     # Set arguments as environment variables
     # os.environ['CP_EXECUTOR'] = exec_type
     # os.environ['CP_MAX_WORKERS'] = str(max_workers)
     # os.environ['CP_CACHE_DIR'] = str(taskfile.parent / '.cache') if cache_dir is None else str(cache_dir)
     # os.environ['CP_DETECT_SOURCE_CHANGE'] = str(int(detect_source_change))
     Context.executor_name = exec_type
     Context.max_workers = max_workers
@@ -42,16 +51,19 @@
     # sys.modules[module_name] = module
     # spec.loader.exec_module(module)
 
     # Run the main task
     entrypoint_fn = getattr(module, entrypoint)
     assert issubclass(entrypoint_fn, TaskType), \
             f'Taskfile `{taskfile}` should contain a task(factory) `{entrypoint}`, but found `{entrypoint_fn}`.'
-    task = entrypoint_fn()
-    _, stats = task.run_graph_with_stats(rate_limits=rate_limits)
+    entrypoint_task = entrypoint_fn()
+    if not dont_force_entrypoint:
+        entrypoint_task.clear_task()
+    _, stats = entrypoint_task.run_graph_with_stats(rate_limits=rate_limits)
+
     print('Execution summary:')
     pprint.pprint(stats['stats'], sort_dicts=False)
     return 0
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `checkpoint_tool-0.7.3/checkpoint/database.py` & `checkpoint_tool-0.7.4/checkpoint/database.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.3/checkpoint/graph.py` & `checkpoint_tool-0.7.4/checkpoint/graph.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.3/checkpoint/task.py` & `checkpoint_tool-0.7.4/checkpoint/task.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.3/checkpoint/types.py` & `checkpoint_tool-0.7.4/checkpoint/types.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.3/pyproject.toml` & `checkpoint_tool-0.7.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkpoint-tool"
-version = "0.7.3"
+version = "0.7.4"
 description = "A lightweight workflow management tool written in pure Python"
 authors = ["Kohei Miyaguchi <koheimiyaguchi@gmail.com>"]
 license = "MIT License"
 homepage = "https://github.com/koheimiya/checkpoint"
 repository = "https://github.com/koheimiya/checkpoint"
 readme = "README.md"
 packages = [{include = "checkpoint"}]
```

### Comparing `checkpoint_tool-0.7.3/PKG-INFO` & `checkpoint_tool-0.7.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkpoint-tool
-Version: 0.7.3
+Version: 0.7.4
 Summary: A lightweight workflow management tool written in pure Python
 Home-page: https://github.com/koheimiya/checkpoint
 License: MIT
 Author: Kohei Miyaguchi
 Author-email: koheimiyaguchi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -51,30 +51,30 @@
     # Inside a task, we first declare the values that must be computed upstream with the descriptor `Req`.
     # In this example, `Choose(n, k)` depends on `Choose(n - 1, k - 1)` and `Choose(n - 1, k)`,
     # so it requires two `int` values.
     # Either the type annotation `Requires[...]` or the assignment `= Req()` may be omitted.
     prev1: Requires[int] = Req()
     prev2: Requires[int] = Req()
 
-    def init(self, n: int, k: int):
+    def build_task(self, n: int, k: int):
         # The prerequisite tasks and the other instance attributes are prepared here.
         # It thus recursively defines all the tasks we need to run this task,
         # i.e., the entire upstream workflow.
 
         if 0 < k < n:
             self.prev1 = Choose(n - 1, k - 1)
             self.prev2 = Choose(n - 1, k)
         elif k == 0 or k == n:
             # We can just pass a value to a requirement slot directly without running tasks.
             self.prev1 = Const(0)
             self.prev2 = Const(1)
         else:
             raise ValueError(f'{(n, k)}')
 
-    def main(self) -> int:
+    def run_task(self) -> int:
         # Here we define the main computation of the task,
         # which is delayed until it is necessary.
 
         # The return values of the prerequisite tasks are accessible via the descriptors:
         return self.prev1 + self.prev2
 
 # To run the task as well as upstream workflow, use the `run_graph()` method.
@@ -104,67 +104,67 @@
 ```
 
 ### Limitations of Task I/O
 
 The arguments of the `init` method can be anything JSON serializable:
 ```python
 class T1(Task):
-    def init(self, **param1):
+    def build_task(self, **param1):
         ...
     ...
 
 class T2(Task):
-    def init(self, **param2):
+    def build_task(self, **param2):
         ...
     ...
 
 class T3(Task):
     x1 = Req()
     x2 = Req()
 
-    def init(self, json_params):
+    def build_task(self, json_params):
         self.x1 = T1(**json_params['param1'])
         self.x2 = T2(**json_params['param2'])
 
-    def main(self):
+    def run_task(self):
         ...
 
 result = T3({'param1': { ... }, 'param2': { ... }}).run_graph()
 ```
 
 Otherwise they can be passed via `Task` and `Req`:
 ```python
 Dataset = ...  # Some complex data structure
 Model = ...    # Some complex data structure
 
 class LoadDataset(Task):
-    def init(self):
+    def build_task(self):
         pass
 
-    def main(self) -> Dataset:
+    def run_task(self) -> Dataset:
         ...
 
 class TrainModel(Task):
     dataset: Requires[Datset]
 
-    def init(self, dataset_task: Task[Dataset]):
+    def build_task(self, dataset_task: Task[Dataset]):
         self.dataset = dataset_task
 
-    def main(self) -> Model:
+    def run_task(self) -> Model:
         ...
     
 class ScoreModel(Task):
     dataset: Requires[Datset]
     model: Requires[Model]
 
-    def init(self, dataset_task: Task[Dataset], model_task: Task[Model]):
+    def build_task(self, dataset_task: Task[Dataset], model_task: Task[Model]):
         self.dataset = dataset_task
         self.model = model_task
 
-    def main(self) -> float:
+    def run_task(self) -> float:
         ...
 
 
 dataset_task = LoadDataset()
 model_task = TrainModel(dataset)
 score_task = ScoreModel(dataset, model)
 print(score_task.run_graph()
@@ -174,18 +174,18 @@
 ```python
 from checkpoint import RequiresDict
 
 
 class SummarizeScores(Task):
     scores: RequiresDict[str, float] = Req()  # Again, type annotation or assignment may be omitted.
 
-    def init(self, task_dict: dict[str, Task[float]]):
+    def build_task(self, task_dict: dict[str, Task[float]]):
         self.scores = task_dict
 
-    def main(self) -> float:
+    def run_task(self) -> float:
         return sum(self.scores.values()) / len(self.scores)  # We have access to the dict of the results.
 ```
 
 The output of the `main` method should be serializable with `cloudpickle`.
 Large outputs can be stored with compression via `zlib`:
 ```python
 class LargeOutputTask(Task, compress_level=-1):
@@ -201,15 +201,15 @@
 ```python
 from checkpoint import DataPath
 
 class TrainModel(Task):
     model_path = DataPath('model.bin')
     ...
 
-    def main(self) -> str:
+    def run_task(self) -> str:
         ...
         model.save(self.model_path)  # Gives `Path('.../model.bin')`
         return self.model_path
 ```
 
 ### Execution policy configuration
```

