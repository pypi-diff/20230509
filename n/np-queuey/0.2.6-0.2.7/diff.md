# Comparing `tmp/np_queuey-0.2.6.tar.gz` & `tmp/np_queuey-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_queuey-0.2.6.tar", last modified: Sat May  6 07:26:53 2023, max compression
+gzip compressed data, was "np_queuey-0.2.7.tar", last modified: Tue May  9 05:23:06 2023, max compression
```

## Comparing `np_queuey-0.2.6.tar` & `np_queuey-0.2.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      227 2023-04-19 04:15:23.193498 np_queuey-0.2.6/README.md
--rw-r--r--   0        0        0     2607 2023-05-06 07:26:53.877390 np_queuey-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      133 2023-05-05 20:01:03.151595 np_queuey-0.2.6/src/np_queuey/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.2.6/src/np_queuey/hueys/__init__.py
--rw-r--r--   0        0        0     9098 2023-04-25 20:53:23.800594 np_queuey-0.2.6/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0     1646 2023-05-06 05:36:41.042949 np_queuey-0.2.6/src/np_queuey/hueys/qc.py
--rw-r--r--   0        0        0     4118 2023-05-06 06:34:16.154743 np_queuey-0.2.6/src/np_queuey/hueys/sorting.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.2.6/src/np_queuey/jobs/__init__.py
--rw-r--r--   0        0        0     6934 2023-04-24 19:51:13.132332 np_queuey-0.2.6/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0      262 2023-04-15 22:53:44.311082 np_queuey-0.2.6/src/np_queuey/jobs/run_small_jobs.py
--rw-r--r--   0        0        0      224 2023-04-23 17:09:38.569310 np_queuey-0.2.6/src/np_queuey/jobs/run_sorting.py
--rw-r--r--   0        0        0     1710 2023-05-05 19:56:33.188797 np_queuey-0.2.6/src/np_queuey/jobs/sorting.py
--rw-r--r--   0        0        0      318 2023-05-06 03:57:55.539505 np_queuey-0.2.6/src/np_queuey/queues/__init__.py
--rw-r--r--   0        0        0     3167 2023-05-05 20:05:28.178905 np_queuey-0.2.6/src/np_queuey/queues/huey_job_queue.py
--rw-r--r--   0        0        0    10101 2023-05-06 01:49:49.463859 np_queuey-0.2.6/src/np_queuey/queues/peewee_job_queue.py
--rw-r--r--   0        0        0      174 2023-05-06 03:43:50.132826 np_queuey-0.2.6/src/np_queuey/queues/pipeline_qc_queue.py
--rw-r--r--   0        0        0      445 2023-05-06 06:51:03.263483 np_queuey-0.2.6/src/np_queuey/queues/pipeline_sorting_queue.py
--rw-r--r--   0        0        0    11528 2023-05-06 07:23:22.330815 np_queuey-0.2.6/src/np_queuey/queues/sqlite_isilon_queue.py
--rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.2.6/src/np_queuey/tasks.py
--rw-r--r--   0        0        0     4952 2023-05-06 04:42:59.665481 np_queuey-0.2.6/src/np_queuey/types.py
--rw-r--r--   0        0        0     3651 2023-05-06 07:05:03.336745 np_queuey-0.2.6/src/np_queuey/utils.py
--rw-r--r--   0        0        0      593 2023-04-19 04:15:23.204497 np_queuey-0.2.6/tests/test_huey.py
--rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 np_queuey-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-04-19 04:15:23.193498 np_queuey-0.2.7/README.md
+-rw-r--r--   0        0        0     2560 2023-05-09 05:23:06.850936 np_queuey-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      133 2023-05-05 20:01:03.151595 np_queuey-0.2.7/src/np_queuey/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.2.7/src/np_queuey/hueys/__init__.py
+-rw-r--r--   0        0        0     9098 2023-04-25 20:53:23.800594 np_queuey-0.2.7/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0     1646 2023-05-06 05:36:41.042949 np_queuey-0.2.7/src/np_queuey/hueys/qc.py
+-rw-r--r--   0        0        0     4602 2023-05-09 05:18:07.449224 np_queuey-0.2.7/src/np_queuey/hueys/sorting.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.2.7/src/np_queuey/jobs/__init__.py
+-rw-r--r--   0        0        0     6934 2023-04-24 19:51:13.132332 np_queuey-0.2.7/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0      262 2023-04-15 22:53:44.311082 np_queuey-0.2.7/src/np_queuey/jobs/run_small_jobs.py
+-rw-r--r--   0        0        0      224 2023-04-23 17:09:38.569310 np_queuey-0.2.7/src/np_queuey/jobs/run_sorting.py
+-rw-r--r--   0        0        0     1710 2023-05-05 19:56:33.188797 np_queuey-0.2.7/src/np_queuey/jobs/sorting.py
+-rw-r--r--   0        0        0      318 2023-05-06 03:57:55.539505 np_queuey-0.2.7/src/np_queuey/queues/__init__.py
+-rw-r--r--   0        0        0     3167 2023-05-05 20:05:28.178905 np_queuey-0.2.7/src/np_queuey/queues/huey_job_queue.py
+-rw-r--r--   0        0        0    10101 2023-05-06 01:49:49.463859 np_queuey-0.2.7/src/np_queuey/queues/peewee_job_queue.py
+-rw-r--r--   0        0        0      174 2023-05-06 03:43:50.132826 np_queuey-0.2.7/src/np_queuey/queues/pipeline_qc_queue.py
+-rw-r--r--   0        0        0      445 2023-05-06 06:51:03.263483 np_queuey-0.2.7/src/np_queuey/queues/pipeline_sorting_queue.py
+-rw-r--r--   0        0        0    11527 2023-05-09 03:01:57.995705 np_queuey-0.2.7/src/np_queuey/queues/sqlite_isilon_queue.py
+-rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.2.7/src/np_queuey/tasks.py
+-rw-r--r--   0        0        0     4952 2023-05-06 04:42:59.665481 np_queuey-0.2.7/src/np_queuey/types.py
+-rw-r--r--   0        0        0     3651 2023-05-06 07:05:03.336745 np_queuey-0.2.7/src/np_queuey/utils.py
+-rw-r--r--   0        0        0      593 2023-04-19 04:15:23.204497 np_queuey-0.2.7/tests/test_huey.py
+-rw-r--r--   0        0        0     1708 1970-01-01 00:00:00.000000 np_queuey-0.2.7/PKG-INFO
```

### Comparing `np_queuey-0.2.6/pyproject.toml` & `np_queuey-0.2.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 [project]
 name = "np_queuey"
-version = "0.2.6"
+version = "0.2.7"
 description = "Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "huey>=2.4.5",
-    "peewee>=3.16.1",
-    "sqlite-web>=0.4.1",
     "np-config>=0.4.17",
     "np-logging>=0.5.1",
-    "np-tools>=0.1.2",
+    "np-tools>=0.1.8",
     "np-session>=0.5.1",
     "typing-extensions>=4.5.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `np_queuey-0.2.6/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py` & `np_queuey-0.2.7/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.6/src/np_queuey/hueys/qc.py` & `np_queuey-0.2.7/src/np_queuey/hueys/qc.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.6/src/np_queuey/hueys/sorting.py` & `np_queuey-0.2.7/src/np_queuey/hueys/sorting.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 import subprocess
 import time
 from typing import Generator, NoReturn
 
 import huey as _huey
 import np_logging
 import np_session
+import np_tools
 from typing_extensions import Literal
 
-from np_queuey.utils import get_job, update_status
+from np_queuey.utils import get_job, get_session, update_status
 from np_queuey.queues.pipeline_sorting_queue import (
     PipelineSortingQueue, SortingJob
 )
 from np_queuey.queues.pipeline_qc_queue import PipelineQCQueue
 from np_queuey.types import SessionArgs, JobT, Job
 
 logger = np_logging.getLogger()
@@ -74,26 +75,33 @@
     """Move the sorted folders to the npexp drive
     Assumes D: processing drive - might want to move this to rig for
     specific-config.
     Cannot robocopy with * for folders, so we must do each probe separately.
     """
     job = get_job(session_or_job, SortingJob)
     for probe_folder in probe_folders(job):
-        logger.info('Moving D:/%s to npexp', probe_folder)
+        src = pathlib.Path(f'D:/{probe_folder}')
+        dest = np_session.Session(job.session).npexp_path / probe_folder
+        logger.info(f'Moving {src} to {dest}')
         subprocess.run([
-            'robocopy', f'D:/{probe_folder}', 
-             str(np_session.Session(job.session).npexp_path / probe_folder), 
+            'robocopy', f'{src}', f'{dest}',
              '/MOVE', '/E', '/COPYALL', '/R:0', '/W:0', '/MT:32'
              ], check=False) # return code from robocopy doesn't signal failure      
-        
-
+        if src.exists():
+            np_tools.move(src, dest, ignore_errors=True)
+            
 def remove_raw_data_on_acq_drives(session_or_job: SortingJob | SessionArgs) -> None:
-    job = get_job(session_or_job, SortingJob)
+    session = get_session(session_or_job)
     for drive in ('A:', 'B:'):
-        for path in pathlib.Path(drive).glob(f'{job.session}*'):
+        for path in pathlib.Path(drive).glob(f'{session}*'):
+            npexp_path = session.npexp_path / path.name
+            lims_path = session.lims_path / path.name if hasattr(session, 'lims_path') else None
+            if not npexp_path.exists() and (lims_path is None or not lims_path.exists()):
+                logger.info('Copying %r to npexp', path)
+                np_tools.copy(path, npexp_path)
             logger.info('Removing %r', path)
             shutil.rmtree(path, ignore_errors=True)
 
 def add_job_to_pipeline_qc_queue(session_or_job: Job | SessionArgs) -> None:
     PipelineQCQueue().add_or_update(session_or_job)
 
 def main() -> NoReturn:
```

### Comparing `np_queuey-0.2.6/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py` & `np_queuey-0.2.7/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.6/src/np_queuey/jobs/sorting.py` & `np_queuey-0.2.7/src/np_queuey/jobs/sorting.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.6/src/np_queuey/queues/huey_job_queue.py` & `np_queuey-0.2.7/src/np_queuey/queues/huey_job_queue.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.6/src/np_queuey/queues/peewee_job_queue.py` & `np_queuey-0.2.7/src/np_queuey/queues/peewee_job_queue.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.6/src/np_queuey/queues/sqlite_isilon_queue.py` & `np_queuey-0.2.7/src/np_queuey/queues/sqlite_isilon_queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     table_name: str = 'sqlite_job_queue'
     
     column_definitions: dict[str, str] = JOB_ARGS_TO_SQL_DEFINITIONS
     job_type: Type[Job] = JobDataclass
     """Job class to use for the queue - see `np_queuey.types.Job` protocol for required attributes"""
     
     def __init__(
-        self, 
+        self,
         **kwargs,
         ) -> None:
         """
         Pass in any attributes as kwargs to assign to instance.
         """
         for key, value in kwargs.items():
             setattr(self, key, value)
```

### Comparing `np_queuey-0.2.6/src/np_queuey/types.py` & `np_queuey-0.2.7/src/np_queuey/types.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.6/src/np_queuey/utils.py` & `np_queuey-0.2.7/src/np_queuey/utils.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.6/tests/test_huey.py` & `np_queuey-0.2.7/tests/test_huey.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.6/PKG-INFO` & `np_queuey-0.2.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-queuey
-Version: 0.2.6
+Version: 0.2.7
 Summary: Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows.
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,19 +12,17 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Project-URL: Repository, https://github.com/AllenInstitute/np_queuey
 Project-URL: Bug tracker, https://github.com/AllenInstitute/np_queuey/issues
 Requires-Python: >=3.8
 Requires-Dist: huey>=2.4.5
-Requires-Dist: peewee>=3.16.1
-Requires-Dist: sqlite-web>=0.4.1
 Requires-Dist: np-config>=0.4.17
 Requires-Dist: np-logging>=0.5.1
-Requires-Dist: np-tools>=0.1.2
+Requires-Dist: np-tools>=0.1.8
 Requires-Dist: np-session>=0.5.1
 Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: blue>=0.9.1; extra == "dev"
 Requires-Dist: pytest>=7.2.2; extra == "dev"
 Requires-Dist: mypy>=1.1.1; extra == "dev"
 Requires-Dist: coverage[toml]>=7.2.2; extra == "dev"
 Requires-Dist: pdm>=2.4.9; extra == "dev"
```

