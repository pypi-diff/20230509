# Comparing `tmp/slurm-parallel-0.1.1.tar.gz` & `tmp/slurm-parallel-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurm-parallel-0.1.1.tar", last modified: Mon May  8 18:37:01 2023, max compression
+gzip compressed data, was "slurm-parallel-0.1.2.tar", last modified: Mon May  8 22:52:32 2023, max compression
```

## Comparing `slurm-parallel-0.1.1.tar` & `slurm-parallel-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 18:37:01.947971 slurm-parallel-0.1.1/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1065 2023-05-01 18:25:25.000000 slurm-parallel-0.1.1/LICENSE
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      110 2023-05-01 22:51:25.000000 slurm-parallel-0.1.1/MANIFEST.in
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-08 18:37:01.932850 slurm-parallel-0.1.1/PKG-INFO
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       83 2023-05-01 18:25:25.000000 slurm-parallel-0.1.1/README.md
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      702 2023-05-08 18:33:43.000000 slurm-parallel-0.1.1/pyproject.toml
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       38 2023-05-08 18:37:01.950252 slurm-parallel-0.1.1/setup.cfg
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 18:37:00.077666 slurm-parallel-0.1.1/src/
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 18:37:01.020038 slurm-parallel-0.1.1/src/slurm_parallel/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      110 2023-05-01 20:47:47.000000 slurm-parallel-0.1.1/src/slurm_parallel/__init__.py
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       37 2023-05-08 18:25:50.000000 slurm-parallel-0.1.1/src/slurm_parallel/cleanup.sh
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       61 2023-05-02 01:39:05.000000 slurm-parallel-0.1.1/src/slurm_parallel/config.toml
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      478 2023-05-08 18:21:00.000000 slurm-parallel-0.1.1/src/slurm_parallel/run.py
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       35 2023-05-08 18:16:02.000000 slurm-parallel-0.1.1/src/slurm_parallel/run.sh
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     7680 2023-05-08 18:17:46.000000 slurm-parallel-0.1.1/src/slurm_parallel/slurm.py
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     2099 2023-05-08 17:39:51.000000 slurm-parallel-0.1.1/src/slurm_parallel/utils.py
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 18:37:01.307776 slurm-parallel-0.1.1/src/slurm_parallel.egg-info/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-08 18:36:59.000000 slurm-parallel-0.1.1/src/slurm_parallel.egg-info/PKG-INFO
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      466 2023-05-08 18:36:59.000000 slurm-parallel-0.1.1/src/slurm_parallel.egg-info/SOURCES.txt
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)        1 2023-05-08 18:36:59.000000 slurm-parallel-0.1.1/src/slurm_parallel.egg-info/dependency_links.txt
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       15 2023-05-08 18:36:59.000000 slurm-parallel-0.1.1/src/slurm_parallel.egg-info/requires.txt
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       15 2023-05-08 18:36:59.000000 slurm-parallel-0.1.1/src/slurm_parallel.egg-info/top_level.txt
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 18:37:01.862653 slurm-parallel-0.1.1/test/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1182 2023-05-08 18:25:32.000000 slurm-parallel-0.1.1/test/test.py
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 22:52:32.905858 slurm-parallel-0.1.2/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1065 2023-05-01 18:25:25.000000 slurm-parallel-0.1.2/LICENSE
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      110 2023-05-01 22:51:25.000000 slurm-parallel-0.1.2/MANIFEST.in
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-08 22:52:32.896736 slurm-parallel-0.1.2/PKG-INFO
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       83 2023-05-01 18:25:25.000000 slurm-parallel-0.1.2/README.md
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      702 2023-05-08 22:51:15.000000 slurm-parallel-0.1.2/pyproject.toml
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       38 2023-05-08 22:52:32.910459 slurm-parallel-0.1.2/setup.cfg
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 22:52:32.522474 slurm-parallel-0.1.2/src/
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 22:52:32.644523 slurm-parallel-0.1.2/src/slurm_parallel/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      110 2023-05-01 20:47:47.000000 slurm-parallel-0.1.2/src/slurm_parallel/__init__.py
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       37 2023-05-08 18:25:50.000000 slurm-parallel-0.1.2/src/slurm_parallel/cleanup.sh
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       61 2023-05-02 01:39:05.000000 slurm-parallel-0.1.2/src/slurm_parallel/config.toml
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      903 2023-05-08 22:43:51.000000 slurm-parallel-0.1.2/src/slurm_parallel/run.py
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       62 2023-05-08 22:38:35.000000 slurm-parallel-0.1.2/src/slurm_parallel/run.sh
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     7971 2023-05-08 22:48:09.000000 slurm-parallel-0.1.2/src/slurm_parallel/slurm.py
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     2099 2023-05-08 17:39:51.000000 slurm-parallel-0.1.2/src/slurm_parallel/utils.py
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 22:52:32.794035 slurm-parallel-0.1.2/src/slurm_parallel.egg-info/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-08 22:52:32.000000 slurm-parallel-0.1.2/src/slurm_parallel.egg-info/PKG-INFO
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      466 2023-05-08 22:52:32.000000 slurm-parallel-0.1.2/src/slurm_parallel.egg-info/SOURCES.txt
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)        1 2023-05-08 22:52:32.000000 slurm-parallel-0.1.2/src/slurm_parallel.egg-info/dependency_links.txt
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       15 2023-05-08 22:52:32.000000 slurm-parallel-0.1.2/src/slurm_parallel.egg-info/requires.txt
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       15 2023-05-08 22:52:32.000000 slurm-parallel-0.1.2/src/slurm_parallel.egg-info/top_level.txt
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 22:52:32.862539 slurm-parallel-0.1.2/test/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1121 2023-05-08 22:48:37.000000 slurm-parallel-0.1.2/test/test.py
```

### Comparing `slurm-parallel-0.1.1/LICENSE` & `slurm-parallel-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slurm-parallel-0.1.1/PKG-INFO` & `slurm-parallel-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurm-parallel
-Version: 0.1.1
+Version: 0.1.2
 Summary: Easy parallelization of python functions on SLURM using job arrays.
 Author: Ho Yin Chau
 License: MIT License
         
         Copyright (c) 2023 hchau630
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `slurm-parallel-0.1.1/pyproject.toml` & `slurm-parallel-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0"] # editable install using setuptool available since v64.0.0
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "slurm-parallel"
-version = "0.1.1"
+version = "0.1.2"
 description = "Easy parallelization of python functions on SLURM using job arrays."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [
     {name = "Ho Yin Chau"},
 ]
```

### Comparing `slurm-parallel-0.1.1/src/slurm_parallel/slurm.py` & `slurm-parallel-0.1.2/src/slurm_parallel/slurm.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,21 +38,21 @@
             
     funcname = func.__name__
     filename = inspect.getsourcefile(func)
     
     if table is None:
         table = funcname
 
-    def run_task(tmp_file):
+    def run_task(tmp_filename):
         n_tasks = int(os.environ['SLURM_ARRAY_TASK_COUNT'])
         task_id = int(os.environ['SLURM_ARRAY_TASK_ID'])
         
         logger.info(f"Running task {task_id}...")
         
-        with open(tmp_file, 'r') as f:
+        with open(tmp_filename, 'r') as f:
             configs = json.load(f)
             
         config_indices = range(task_id, len(configs), n_tasks)
         
         logger.info(f"Config indices: {config_indices}")
 
         for i in config_indices:
@@ -72,19 +72,22 @@
                     else:
                         result = {column: v for v in result}
 
                 database[table].append(config | result)
 
                 logger.info(f"Saved output of config {i}.")
     
-    def remote(configs, max_n_tasks=max_n_tasks, tmp_dir=tmp_dir, out_dir=out_dir, out_file=out_file, time_per_config=time_per_config, **kwargs):
+    def remote(configs, logging_kwargs=None, max_n_tasks=max_n_tasks, tmp_dir=tmp_dir, out_dir=out_dir, out_file=out_file, time_per_config=time_per_config, **kwargs):
         for k in kwargs:
             if k not in allowed_args:
                 raise KeyError(f"remote got an unexpected argument '{k}'")
                 
+        if logging_kwargs is None:
+            logging_kwargs = {}
+                
         if max_n_tasks is None:
             completed_process = subprocess.run(
                 ['scontrol', 'show', 'config'],
                 capture_output=True,
                 check=True,
             )
             max_n_tasks = int(re.search('MaxArraySize\s*= (\d*)', completed_process.stdout.decode("utf-8")).group(1))
@@ -118,23 +121,28 @@
             'array': f'0-{n_tasks-1}',
             'output': out_dir / out_file,
             'parsable': True,
             'job_name': f'{pathlib.Path(filename).stem}_{funcname}',
         } | default_kwargs | kwargs
         run_options = utils.to_cmd_options(**run_kwargs)
         
+        logging_kwargs = {
+            'capture_warnings': True
+        } | logging_kwargs
+        logging_options = utils.to_cmd_options(**logging_kwargs)
+        
         try:
             with tempfile.NamedTemporaryFile(dir=tmp_dir, mode='w', delete=False) as f:
                 json.dump(configs, f)
                 
-            tmp_file = pathlib.Path(f.name)
-            logger.info(f"Saved configs to tmp file {tmp_file}.")
+            tmp_filename = f.name
+            logger.info(f"Saved configs to tmp file {tmp_filename}.")
             
             completed_process = subprocess.run(
-                ["sbatch", *run_options, str(run_script), str(run_py_script), filename, funcname, str(tmp_file)],
+                ["sbatch", *run_options, run_script, run_py_script, filename, funcname, tmp_filename, *logging_options],
                 capture_output=True,
                 check=True,
             )
         
             run_PID = completed_process.stdout.decode("utf-8").split('\n')[-2]
 
             logger.info(f"Submitted job to cluster to run {funcname} with job ID {run_PID}.")
@@ -148,21 +156,21 @@
                 'output': out_dir / "cleanup.out",
                 'parsable': True,
                 'job_name': f'{pathlib.Path(filename).stem}_{funcname}_cleanup',
             }
             cleanup_options = utils.to_cmd_options(**cleanup_kwargs)
 
             completed_process = subprocess.run(
-                ["sbatch", *cleanup_options, str(cleanup_script), str(tmp_file)],
+                ["sbatch", *cleanup_options, cleanup_script, tmp_filename],
                 capture_output=True,
                 check=True,
             )
             
         except Exception as err:
-            tmp_file.unlink()
+            pathlib.Path(tmp_filename).unlink()
             raise err
         
         cleanup_PID = completed_process.stdout.decode("utf-8").split('\n')[-2]
         
         logger.info(f"Submitted job to cluster to run cleanup with command job ID {cleanup_PID}.")
         logger.debug(f"Submission command: {completed_process.args}")
```

### Comparing `slurm-parallel-0.1.1/src/slurm_parallel/utils.py` & `slurm-parallel-0.1.2/src/slurm_parallel/utils.py`

 * *Files identical despite different names*

### Comparing `slurm-parallel-0.1.1/src/slurm_parallel.egg-info/PKG-INFO` & `slurm-parallel-0.1.2/src/slurm_parallel.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurm-parallel
-Version: 0.1.1
+Version: 0.1.2
 Summary: Easy parallelization of python functions on SLURM using job arrays.
 Author: Ho Yin Chau
 License: MIT License
         
         Copyright (c) 2023 hchau630
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `slurm-parallel-0.1.1/test/test.py` & `slurm-parallel-0.1.2/test/test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-import logging
 import time
 
 import sqlalchemy as sa
 import dfdb
 import hyclib as lib
 
 import slurm_parallel as sp
 
-lib.logging.basic_config()
-logger = logging.getLogger()
-logger.setLevel('DEBUG')
-
 db = dfdb.Database(database='test/data/test.db')
 
 @sp.parallelize(mem_per_cpu='1gb', c=1, partition='ctn')
 def print_results():
     df = db['results'].fetch()
     print(df)
 
@@ -37,12 +32,12 @@
     
     configs = [
         {'a': 1, 'b': 2},
         {'a': 3, 'b': 4},
         {'a': 5, 'b': 6},
         {'a': 7, 'b': 8},
     ]
-    job = func.remote(configs, wait=False, max_n_tasks=3)
+    job = func.remote(configs, wait=False, max_n_tasks=3, logging_kwargs=dict(level='DEBUG'))
     print_results.remote([{}], dependency=f'afterany:{job}')
 
 if __name__ == '__main__':
     main()
```

