# Comparing `tmp/slurm-parallel-0.1.2.tar.gz` & `tmp/slurm-parallel-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurm-parallel-0.1.2.tar", last modified: Mon May  8 22:52:32 2023, max compression
+gzip compressed data, was "slurm-parallel-0.1.3.tar", last modified: Tue May  9 07:38:36 2023, max compression
```

## Comparing `slurm-parallel-0.1.2.tar` & `slurm-parallel-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 22:52:32.905858 slurm-parallel-0.1.2/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1065 2023-05-01 18:25:25.000000 slurm-parallel-0.1.2/LICENSE
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      110 2023-05-01 22:51:25.000000 slurm-parallel-0.1.2/MANIFEST.in
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-08 22:52:32.896736 slurm-parallel-0.1.2/PKG-INFO
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       83 2023-05-01 18:25:25.000000 slurm-parallel-0.1.2/README.md
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      702 2023-05-08 22:51:15.000000 slurm-parallel-0.1.2/pyproject.toml
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       38 2023-05-08 22:52:32.910459 slurm-parallel-0.1.2/setup.cfg
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 22:52:32.522474 slurm-parallel-0.1.2/src/
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 22:52:32.644523 slurm-parallel-0.1.2/src/slurm_parallel/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      110 2023-05-01 20:47:47.000000 slurm-parallel-0.1.2/src/slurm_parallel/__init__.py
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       37 2023-05-08 18:25:50.000000 slurm-parallel-0.1.2/src/slurm_parallel/cleanup.sh
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       61 2023-05-02 01:39:05.000000 slurm-parallel-0.1.2/src/slurm_parallel/config.toml
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      903 2023-05-08 22:43:51.000000 slurm-parallel-0.1.2/src/slurm_parallel/run.py
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       62 2023-05-08 22:38:35.000000 slurm-parallel-0.1.2/src/slurm_parallel/run.sh
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     7971 2023-05-08 22:48:09.000000 slurm-parallel-0.1.2/src/slurm_parallel/slurm.py
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     2099 2023-05-08 17:39:51.000000 slurm-parallel-0.1.2/src/slurm_parallel/utils.py
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 22:52:32.794035 slurm-parallel-0.1.2/src/slurm_parallel.egg-info/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-08 22:52:32.000000 slurm-parallel-0.1.2/src/slurm_parallel.egg-info/PKG-INFO
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      466 2023-05-08 22:52:32.000000 slurm-parallel-0.1.2/src/slurm_parallel.egg-info/SOURCES.txt
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)        1 2023-05-08 22:52:32.000000 slurm-parallel-0.1.2/src/slurm_parallel.egg-info/dependency_links.txt
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       15 2023-05-08 22:52:32.000000 slurm-parallel-0.1.2/src/slurm_parallel.egg-info/requires.txt
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       15 2023-05-08 22:52:32.000000 slurm-parallel-0.1.2/src/slurm_parallel.egg-info/top_level.txt
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 22:52:32.862539 slurm-parallel-0.1.2/test/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1121 2023-05-08 22:48:37.000000 slurm-parallel-0.1.2/test/test.py
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-09 07:38:36.384932 slurm-parallel-0.1.3/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1065 2023-05-01 18:25:25.000000 slurm-parallel-0.1.3/LICENSE
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      150 2023-05-09 05:30:00.000000 slurm-parallel-0.1.3/MANIFEST.in
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-09 07:38:36.378884 slurm-parallel-0.1.3/PKG-INFO
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       83 2023-05-01 18:25:25.000000 slurm-parallel-0.1.3/README.md
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      714 2023-05-09 07:37:51.000000 slurm-parallel-0.1.3/pyproject.toml
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       38 2023-05-09 07:38:36.387165 slurm-parallel-0.1.3/setup.cfg
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-09 07:38:35.801493 slurm-parallel-0.1.3/src/
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-09 07:38:36.252032 slurm-parallel-0.1.3/src/slurm_parallel/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      110 2023-05-01 20:47:47.000000 slurm-parallel-0.1.3/src/slurm_parallel/__init__.py
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       37 2023-05-08 18:25:50.000000 slurm-parallel-0.1.3/src/slurm_parallel/cleanup.sh
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       61 2023-05-02 01:39:05.000000 slurm-parallel-0.1.3/src/slurm_parallel/config.toml
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      918 2023-05-09 07:36:00.000000 slurm-parallel-0.1.3/src/slurm_parallel/run.py
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       28 2023-05-09 04:55:29.000000 slurm-parallel-0.1.3/src/slurm_parallel/run.sh
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)    11218 2023-05-09 07:37:31.000000 slurm-parallel-0.1.3/src/slurm_parallel/slurm.py
+-rwxr-xr-x   0 hc3190   (413786699) domain users (413600513)     1050 2023-05-09 05:29:06.000000 slurm-parallel-0.1.3/src/slurm_parallel/summarize.sh
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     2099 2023-05-08 17:39:51.000000 slurm-parallel-0.1.3/src/slurm_parallel/utils.py
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-09 07:38:36.275006 slurm-parallel-0.1.3/src/slurm_parallel.egg-info/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-09 07:38:35.000000 slurm-parallel-0.1.3/src/slurm_parallel.egg-info/PKG-INFO
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      498 2023-05-09 07:38:35.000000 slurm-parallel-0.1.3/src/slurm_parallel.egg-info/SOURCES.txt
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)        1 2023-05-09 07:38:35.000000 slurm-parallel-0.1.3/src/slurm_parallel.egg-info/dependency_links.txt
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       20 2023-05-09 07:38:35.000000 slurm-parallel-0.1.3/src/slurm_parallel.egg-info/requires.txt
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       15 2023-05-09 07:38:35.000000 slurm-parallel-0.1.3/src/slurm_parallel.egg-info/top_level.txt
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-09 07:38:36.281202 slurm-parallel-0.1.3/test/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1406 2023-05-09 07:35:16.000000 slurm-parallel-0.1.3/test/test.py
```

### Comparing `slurm-parallel-0.1.2/LICENSE` & `slurm-parallel-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `slurm-parallel-0.1.2/PKG-INFO` & `slurm-parallel-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurm-parallel
-Version: 0.1.2
+Version: 0.1.3
 Summary: Easy parallelization of python functions on SLURM using job arrays.
 Author: Ho Yin Chau
 License: MIT License
         
         Copyright (c) 2023 hchau630
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `slurm-parallel-0.1.2/pyproject.toml` & `slurm-parallel-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0"] # editable install using setuptool available since v64.0.0
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "slurm-parallel"
-version = "0.1.2"
+version = "0.1.3"
 description = "Easy parallelization of python functions on SLURM using job arrays."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [
     {name = "Ho Yin Chau"},
 ]
@@ -16,11 +16,12 @@
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9",
 ]
 dependencies = [
     'hyclib>=0.1.14',
+    'tqdm',
 ]
 
 [project.urls]
 repository = "https://github.com/hchau630/slurm-parallel"
```

### Comparing `slurm-parallel-0.1.2/src/slurm_parallel/run.py` & `slurm-parallel-0.1.3/src/slurm_parallel/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+import logging
 
 import hyclib as lib
 
 from slurm_parallel.utils import import_from_file_path
 
 def main():
     parser = argparse.ArgumentParser('run.py')
```

### Comparing `slurm-parallel-0.1.2/src/slurm_parallel/slurm.py` & `slurm-parallel-0.1.3/src/slurm_parallel/slurm.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,36 +6,40 @@
 import logging
 import pathlib
 import tempfile
 import datetime
 import os
 import copy
 import math
+import time
+import warnings
 from string import Template
 from importlib import resources
 
+from tqdm import tqdm
 import hyclib as lib
 
 from . import config, utils
 
 logger = logging.getLogger(__name__)
 run_script = resources.files('slurm_parallel').joinpath('run.sh')
 run_py_script = resources.files('slurm_parallel').joinpath('run.py')
-cleanup_script = resources.files('slurm_parallel').joinpath('cleanup.sh')
+summarize_script = resources.files('slurm_parallel').joinpath('summarize.sh')
+# cleanup_script = resources.files('slurm_parallel').joinpath('cleanup.sh')
 
-allowed_args = {'A', 'account', 'acctg_freq', 'batch', 'bb', 'bbf', 'b', 'begin', 'D', 'chdir', 'cluster_constraint', 'M', 'clusters', 'comment', 'C', 'constraint', 'container', 'container_id', 'contiguous', 'S', 'core-spec', 'cores_per_socket', 'cpu_freq', 'cpus_per_gpu', 'c', 'cpus_per_task', 'deadline', 'delay_boot', 'd', 'dependency', 'm', 'distribution', 'e', 'error', 'x', 'exclude', 'exclusive', 'export', 'export_file', 'extra', 'B', 'extra_node_info', 'get_user_env', 'gid', 'gpu_bind', 'gpu_freq', 'G', 'gpus', 'gpus_per_node', 'gpus_per_socket', 'gpus_per_task', 'gres', 'gres_flags', 'h', 'help', 'hint', 'H', 'hold', 'ignore_pbs', 'i', 'input', 'J', 'job_name', 'kill_on_invalid_dep', 'L', 'licenses', 'mail_type', 'mail_user', 'mcs_label', 'mem', 'mem_bind', 'mem_per_cpu', 'mem_per_gpu', 'mincpus', 'network', 'nice', 'k', 'no_kill', 'no_requeue', 'F', 'nodefile', 'w', 'nodelist', 'N', 'nodes', 'n', 'ntasks', 'ntasks_per_core', 'ntasks_per_gpu', 'ntasks_per_node', 'ntasks_per_socket', 'open_mode', 'O', 'overcommit', 's', 'oversubscribe', 'p', 'partition', 'power', 'prefer', 'priority', 'profile', 'propagate', 'q', 'qos', 'Q', 'quiet', 'reboot', 'requeue', 'reservation', 'signal', 'sockets_per_node', 'spread_job', 'switches', 'test_only', 'thread_spec', 'threads_per_core', 't', 'time', 'time_min', 'tmp', 'tres_per_task', 'uid', 'usage', 'use_min_nodes', 'v', 'verbose', 'V', 'version', 'W', 'wait', 'wait_all_nodes', 'wckey', 'wrap'}
+allowed_args = {'A', 'account', 'acctg_freq', 'batch', 'bb', 'bbf', 'b', 'begin', 'D', 'chdir', 'cluster_constraint', 'M', 'clusters', 'comment', 'C', 'constraint', 'container', 'container_id', 'contiguous', 'S', 'core-spec', 'cores_per_socket', 'cpu_freq', 'cpus_per_gpu', 'c', 'cpus_per_task', 'deadline', 'delay_boot', 'd', 'dependency', 'm', 'distribution', 'e', 'error', 'x', 'exclude', 'exclusive', 'export', 'export_file', 'extra', 'B', 'extra_node_info', 'get_user_env', 'gid', 'gpu_bind', 'gpu_freq', 'G', 'gpus', 'gpus_per_node', 'gpus_per_socket', 'gpus_per_task', 'gres', 'gres_flags', 'h', 'help', 'hint', 'H', 'hold', 'ignore_pbs', 'i', 'input', 'J', 'job_name', 'kill_on_invalid_dep', 'L', 'licenses', 'mail_type', 'mail_user', 'mcs_label', 'mem', 'mem_bind', 'mem_per_cpu', 'mem_per_gpu', 'mincpus', 'network', 'nice', 'k', 'no_kill', 'no_requeue', 'F', 'nodefile', 'w', 'nodelist', 'N', 'nodes', 'n', 'ntasks', 'ntasks_per_core', 'ntasks_per_gpu', 'ntasks_per_node', 'ntasks_per_socket', 'open_mode', 'O', 'overcommit', 's', 'oversubscribe', 'p', 'partition', 'power', 'prefer', 'priority', 'profile', 'propagate', 'q', 'qos', 'Q', 'quiet', 'reboot', 'requeue', 'reservation', 'signal', 'sockets_per_node', 'spread_job', 'switches', 'test_only', 'thread_spec', 'threads_per_core', 't', 'time', 'time_min', 'tmp', 'tres_per_task', 'uid', 'usage', 'use_min_nodes', 'v', 'verbose', 'V', 'version', 'wait_all_nodes', 'wckey', 'wrap'}
 
 __all__ = ['parallelize']
 
 class StringTemplate(Template):
     delimiter = '%'
     idpattern = "(?a-i:[sF])" # ASCII-only, don't ignore case
 
 @lib.functools.parametrized
-def parallelize(func, database=None, table=None, columns=None, max_n_tasks=None, tmp_dir=None, out_dir=None, out_file=None, time_per_config=30, **default_kwargs):
+def parallelize(func, database=None, table=None, columns=None, max_n_tasks=None, tmp_dir=None, out_dir=None, out_file=None, time_per_config=30, wait=True, progress_dt=5, **default_kwargs):
     for k in default_kwargs:
         if k not in allowed_args:
             raise KeyError(f"parallelize got an unexpected argument '{k}'")
             
     funcname = func.__name__
     filename = inspect.getsourcefile(func)
     
@@ -72,15 +76,15 @@
                     else:
                         result = {column: v for v in result}
 
                 database[table].append(config | result)
 
                 logger.info(f"Saved output of config {i}.")
     
-    def remote(configs, logging_kwargs=None, max_n_tasks=max_n_tasks, tmp_dir=tmp_dir, out_dir=out_dir, out_file=out_file, time_per_config=time_per_config, **kwargs):
+    def remote(configs, logging_kwargs=None, max_n_tasks=max_n_tasks, tmp_dir=tmp_dir, out_dir=out_dir, out_file=out_file, time_per_config=time_per_config, wait=wait, progress_dt=progress_dt, **kwargs):
         for k in kwargs:
             if k not in allowed_args:
                 raise KeyError(f"remote got an unexpected argument '{k}'")
                 
         if logging_kwargs is None:
             logging_kwargs = {}
                 
@@ -100,14 +104,20 @@
 
         if out_file is None:
             out_file = config['out_file']
             
         if not isinstance(time_per_config, datetime.timedelta):
             time_per_config = datetime.timedelta(minutes=time_per_config)
             
+        if not wait:
+            raise NotImplementedError()
+            
+        if progress_dt < 1:
+            warnings.warn("progress_dt less than 1 second, this may potentially cause server performance issues due to frequent polling.")
+            
         pathlib.Path(tmp_dir).mkdir(parents=True, exist_ok=True)
         out_dir = StringTemplate(out_dir).safe_substitute(s=pathlib.Path(filename).stem, F=funcname)
         out_dir = pathlib.Path(datetime.datetime.now().strftime(out_dir))
         out_dir.mkdir(parents=True, exist_ok=True)
         out_file = StringTemplate(out_file).safe_substitute(s=pathlib.Path(filename).stem, F=funcname)
         
         n_configs = len(configs)
@@ -116,68 +126,124 @@
         
         run_kwargs = {
             'c': 2,
             'mem_per_cpu': '2gb',
             'time': lib.datetime.strftime(time_per_task, '%d-%H:%M:%S'),
             'array': f'0-{n_tasks-1}',
             'output': out_dir / out_file,
-            'parsable': True,
+            'parsable': not wait,
+            'wait': wait,
             'job_name': f'{pathlib.Path(filename).stem}_{funcname}',
         } | default_kwargs | kwargs
         run_options = utils.to_cmd_options(**run_kwargs)
         
         logging_kwargs = {
             'capture_warnings': True
         } | logging_kwargs
         logging_options = utils.to_cmd_options(**logging_kwargs)
         
-        try:
-            with tempfile.NamedTemporaryFile(dir=tmp_dir, mode='w', delete=False) as f:
+        with tempfile.TemporaryDirectory(dir=tmp_dir) as new_tmp_dir:
+            tmp_filename = pathlib.Path(new_tmp_dir) / 'config.json'
+            
+            with open(tmp_filename, 'w') as f:
                 json.dump(configs, f)
                 
-            tmp_filename = f.name
-            logger.info(f"Saved configs to tmp file {tmp_filename}.")
+            logger.debug(f"Saved configs to tmp file {tmp_filename}.")
+            
+            args = ["sbatch", *run_options, run_script, run_py_script, filename, funcname, tmp_filename, *logging_options]
+            logger.debug(f"Invoking subprocess with arguments {args}")
+            
+            success = False
+            try:
+                with subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE, bufsize=1, text=True) as p:
+                    for line in p.stdout:
+                        match = re.search('Submitted batch job ([0-9]{6})', line)
+                        if match is not None:
+                            run_PID = match.group(1)
+                            break
+
+                    logger.info(f'Submitted batch job {run_PID} for {pathlib.Path(filename).stem}.{funcname}')
+
+                    n = 0
+                    with tqdm(total=n_tasks) as t:
+                        while True:
+                            summary = subprocess.run([summarize_script, run_PID], capture_output=True, check=True, text=True)
+                            n_completed = summary.stdout.count('COMPLETED')
+                            n_failed = summary.stdout.count('FAILED')
+                            n_running = summary.stdout.count('RUNNING')
+
+                            t.update(n=(n_completed + n_failed - n))
+                            t.set_postfix(n_completed=n_completed, n_failed=n_failed, n_running=n_running)
+
+                            n = n_completed + n_failed
+
+                            if n >= n_tasks:
+                                break
+
+                            time.sleep(progress_dt)
+                            
+                if p.returncode != 0:
+                    raise subprocess.CalledProcessError(p.returncode, p.args)
+                    
+            except Exception as err:
+                raise err
+                
+            else:
+                success = True
+                
+            finally:
+                if not success:
+                    subprocess.run(['scancel', run_PID], check=True)
+                    logger.info(f"Ensured batch job {run_PID} for {pathlib.Path(filename).stem}.{funcname} is cancelled.")
             
-            completed_process = subprocess.run(
-                ["sbatch", *run_options, run_script, run_py_script, filename, funcname, tmp_filename, *logging_options],
-                capture_output=True,
-                check=True,
-            )
         
-            run_PID = completed_process.stdout.decode("utf-8").split('\n')[-2]
-
-            logger.info(f"Submitted job to cluster to run {funcname} with job ID {run_PID}.")
-            logger.debug(f"Submission command: {completed_process.args}")
+#         try:
+#             with tempfile.NamedTemporaryFile(dir=tmp_dir, mode='w', delete=False) as f:
+#                 json.dump(configs, f)
+                
+#             tmp_filename = f.name
+#             logger.info(f"Saved configs to tmp file {tmp_filename}.")
             
-            cleanup_kwargs = {
-                'c': 1,
-                'mem_per_cpu': '1mb',
-                'time': 1, # 1 minute
-                'dependency': f'afterany:{run_PID}',
-                'output': out_dir / "cleanup.out",
-                'parsable': True,
-                'job_name': f'{pathlib.Path(filename).stem}_{funcname}_cleanup',
-            }
-            cleanup_options = utils.to_cmd_options(**cleanup_kwargs)
+#             args = ["sbatch", *run_options, run_script, run_py_script, filename, funcname, tmp_filename, *logging_options]
+#             logger.debug(f"Invoking subprocess with arguments {args}")
+            
+#             completed_process = subprocess.run(args, capture_output=not wait, check=True)
+            
+#             if wait:
+#                 pathlib.Path(tmp_filename).unlink(missing_ok=True)
+#                 logger.info(f"{tmp_filename} removed")
+                
+#             else:
+#                 run_PID = completed_process.stdout.decode("utf-8").split('\n')[-2]
+#                 print(f"Submitted batch job {run_PID}")
+            
+#                 cleanup_kwargs = {
+#                     'c': 1,
+#                     'mem_per_cpu': '1mb',
+#                     'time': 1, # 1 minute
+#                     'dependency': f'afterany:{run_PID}',
+#                     'output': out_dir / "cleanup.out",
+#                     'parsable': True,
+#                     'job_name': f'{pathlib.Path(filename).stem}_{funcname}_cleanup',
+#                 }
+#                 cleanup_options = utils.to_cmd_options(**cleanup_kwargs)
 
-            completed_process = subprocess.run(
-                ["sbatch", *cleanup_options, cleanup_script, tmp_filename],
-                capture_output=True,
-                check=True,
-            )
+#                 args = ["sbatch", *cleanup_options, cleanup_script, tmp_filename]
+#                 logger.debug(f"Invoking subprocess with arguments {args}")
+                
+#                 completed_process = subprocess.run(args, capture_output=True, check=True)
+                
+#                 cleanup_PID = completed_process.stdout.decode("utf-8").split('\n')[-2]
+#                 logger.debug(f"Submitted cleanup batch job with job ID {cleanup_PID}")
+                
+#                 return run_PID
             
-        except Exception as err:
-            pathlib.Path(tmp_filename).unlink()
-            raise err
-        
-        cleanup_PID = completed_process.stdout.decode("utf-8").split('\n')[-2]
-        
-        logger.info(f"Submitted job to cluster to run cleanup with command job ID {cleanup_PID}.")
-        logger.debug(f"Submission command: {completed_process.args}")
-        
-        return run_PID
+#         except Exception as err:
+#             pathlib.Path(tmp_filename).unlink(missing_ok=True)
+#             logger.info(f"{tmp_filename} removed")
+#             raise err
     
     func.run_task = run_task
     func.remote = remote
     
     return func
```

### Comparing `slurm-parallel-0.1.2/src/slurm_parallel/utils.py` & `slurm-parallel-0.1.3/src/slurm_parallel/utils.py`

 * *Files identical despite different names*

### Comparing `slurm-parallel-0.1.2/src/slurm_parallel.egg-info/PKG-INFO` & `slurm-parallel-0.1.3/src/slurm_parallel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurm-parallel
-Version: 0.1.2
+Version: 0.1.3
 Summary: Easy parallelization of python functions on SLURM using job arrays.
 Author: Ho Yin Chau
 License: MIT License
         
         Copyright (c) 2023 hchau630
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `slurm-parallel-0.1.2/test/test.py` & `slurm-parallel-0.1.3/test/test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,35 @@
+import logging
 import time
 
 import sqlalchemy as sa
 import dfdb
 import hyclib as lib
 
 import slurm_parallel as sp
 
 db = dfdb.Database(database='test/data/test.db')
+logger = logging.getLogger()
 
 @sp.parallelize(mem_per_cpu='1gb', c=1, partition='ctn')
 def print_results():
     df = db['results'].fetch()
     print(df)
 
 @sp.parallelize(database=db, table='results', columns='result', mem_per_cpu='1gb', c=1, partition='ctn')
 def func(a, b):
-    # time.sleep(30)
+    # time.sleep(20)
+    # if a == 5:
+    #     raise RuntimeError()
     return a + b
 
 def main():
+    lib.logging.basic_config()
+    logger.setLevel('DEBUG')
+    
     if 'results' in db:
         del db['results']
         
     db['results'] = dfdb.TableDef(
         sa.Column('id', sa.Integer(), primary_key=True),
         sa.Column('a', sa.Integer()),
         sa.Column('b', sa.Integer()),
@@ -32,12 +39,15 @@
     
     configs = [
         {'a': 1, 'b': 2},
         {'a': 3, 'b': 4},
         {'a': 5, 'b': 6},
         {'a': 7, 'b': 8},
     ]
-    job = func.remote(configs, wait=False, max_n_tasks=3, logging_kwargs=dict(level='DEBUG'))
-    print_results.remote([{}], dependency=f'afterany:{job}')
+    # job = func.remote(configs, wait=False, max_n_tasks=3, logging_kwargs=dict(level='DEBUG'))
+    # print_results.remote([{}], wait=False, dependency=f'afterany:{job}')
+    
+    func.remote(configs, max_n_tasks=3, logging_kwargs=dict(level='DEBUG'))
+    print_results.remote([{}])
 
 if __name__ == '__main__':
     main()
```

