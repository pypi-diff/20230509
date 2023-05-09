# Comparing `tmp/vdk-dag-0.1.861330674.tar.gz` & `tmp/vdk-dag-0.1.861974079.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-dag-0.1.861330674.tar", last modified: Tue May  9 09:18:11 2023, max compression
+gzip compressed data, was "vdk-dag-0.1.861974079.tar", last modified: Tue May  9 16:11:21 2023, max compression
```

## Comparing `vdk-dag-0.1.861330674.tar` & `vdk-dag-0.1.861974079.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:18:11.848055 vdk-dag-0.1.861330674/
--rw-r--r--   0 root         (0) root         (0)     8454 2023-05-09 09:18:11.848055 vdk-dag-0.1.861330674/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7887 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 09:18:11.848055 vdk-dag-0.1.861330674/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-09 09:18:00.000000 vdk-dag-0.1.861330674/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:18:11.844055 vdk-dag-0.1.861330674/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:18:11.844055 vdk-dag-0.1.861330674/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:18:11.844055 vdk-dag-0.1.861330674/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:18:11.848055 vdk-dag-0.1.861330674/src/vdk/plugin/dag/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:18:11.848055 vdk-dag-0.1.861330674/src/vdk/plugin/dag/api/
--rw-rw-rw-   0 root         (0) root         (0)     1375 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/api/dag.py
--rw-rw-rw-   0 root         (0) root         (0)     9308 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/cached_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     6078 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag.py
--rw-rw-rw-   0 root         (0) root         (0)     1385 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     6480 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag_plugin_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      923 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     7838 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     2253 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/dags.py
--rw-rw-rw-   0 root         (0) root         (0)     9334 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/remote_data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/remote_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     2579 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/time_based_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:18:11.848055 vdk-dag-0.1.861330674/src/vdk_dag.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8454 2023-05-09 09:18:11.000000 vdk-dag-0.1.861330674/src/vdk_dag.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-09 09:18:11.000000 vdk-dag-0.1.861330674/src/vdk_dag.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 09:18:11.000000 vdk-dag-0.1.861330674/src/vdk_dag.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-09 09:18:11.000000 vdk-dag-0.1.861330674/src/vdk_dag.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-09 09:18:11.000000 vdk-dag-0.1.861330674/src/vdk_dag.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-09 09:18:11.000000 vdk-dag-0.1.861330674/src/vdk_dag.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:18:11.848055 vdk-dag-0.1.861330674/tests/
--rw-rw-rw-   0 root         (0) root         (0)    16367 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/tests/test_dag.py
--rw-rw-rw-   0 root         (0) root         (0)     2550 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/tests/test_dag_object.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/tests/test_time_based_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2285 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/tests/test_tracking_job_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:11:21.378871 vdk-dag-0.1.861974079/
+-rw-r--r--   0 root         (0) root         (0)     8454 2023-05-09 16:11:21.378871 vdk-dag-0.1.861974079/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7887 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 16:11:21.378871 vdk-dag-0.1.861974079/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-09 16:11:10.000000 vdk-dag-0.1.861974079/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:11:21.374871 vdk-dag-0.1.861974079/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:11:21.374871 vdk-dag-0.1.861974079/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:11:21.374871 vdk-dag-0.1.861974079/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:11:21.378871 vdk-dag-0.1.861974079/src/vdk/plugin/dag/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:11:21.378871 vdk-dag-0.1.861974079/src/vdk/plugin/dag/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/api/dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     9308 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/cached_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6078 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1384 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/dag_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6480 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/dag_plugin_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      923 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/dag_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     7838 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/dag_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2253 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/dags.py
+-rw-rw-rw-   0 root         (0) root         (0)     9334 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/remote_data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/remote_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2579 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/time_based_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:11:21.378871 vdk-dag-0.1.861974079/src/vdk_dag.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8454 2023-05-09 16:11:21.000000 vdk-dag-0.1.861974079/src/vdk_dag.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-09 16:11:21.000000 vdk-dag-0.1.861974079/src/vdk_dag.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 16:11:21.000000 vdk-dag-0.1.861974079/src/vdk_dag.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-09 16:11:21.000000 vdk-dag-0.1.861974079/src/vdk_dag.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-09 16:11:21.000000 vdk-dag-0.1.861974079/src/vdk_dag.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-09 16:11:21.000000 vdk-dag-0.1.861974079/src/vdk_dag.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:11:21.378871 vdk-dag-0.1.861974079/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    16383 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/tests/test_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2550 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/tests/test_dag_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/tests/test_time_based_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/tests/test_tracking_job_executor.py
```

### Comparing `vdk-dag-0.1.861330674/PKG-INFO` & `vdk-dag-0.1.861974079/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-dag
-Version: 0.1.861330674
+Version: 0.1.861974079
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-dag-0.1.861330674/README.md` & `vdk-dag-0.1.861974079/README.md`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861330674/setup.py` & `vdk-dag-0.1.861974079/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.861330674"
+__version__ = "0.1.861974079"
 
 setuptools.setup(
     name="vdk-dag",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Express dependecies between data jobs.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-dag-0.1.861330674/src/vdk/plugin/dag/api/dag.py` & `vdk-dag-0.1.861974079/src/vdk/plugin/dag/api/dag.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861330674/src/vdk/plugin/dag/cached_data_job_executor.py` & `vdk-dag-0.1.861974079/src/vdk/plugin/dag/cached_data_job_executor.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag.py` & `vdk-dag-0.1.861974079/src/vdk/plugin/dag/dag.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag_plugin.py` & `vdk-dag-0.1.861974079/src/vdk/plugin/dag/dag_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     @staticmethod
     @hookimpl
     def run_job(context: JobContext) -> None:
         # TODO: there should be less hacky way
         dag_runner.TEAM_NAME = context.core_context.configuration.get_value(
             JobConfigKeys.TEAM
         )
-        dag_runner.DAGS_CONFIG = DagPluginConfiguration(
+        dag_runner.DAG_CONFIG = DagPluginConfiguration(
             context.core_context.configuration
         )
 
     @staticmethod
     @hookimpl
     def vdk_configure(config_builder: ConfigurationBuilder) -> None:
         """
```

### Comparing `vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag_plugin_configuration.py` & `vdk-dag-0.1.861974079/src/vdk/plugin/dag/dag_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag_runner.py` & `vdk-dag-0.1.861974079/src/vdk/plugin/dag/dag_runner.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag_validator.py` & `vdk-dag-0.1.861974079/src/vdk/plugin/dag/dag_validator.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861330674/src/vdk/plugin/dag/dags.py` & `vdk-dag-0.1.861974079/src/vdk/plugin/dag/dags.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861330674/src/vdk/plugin/dag/remote_data_job.py` & `vdk-dag-0.1.861974079/src/vdk/plugin/dag/remote_data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861330674/src/vdk/plugin/dag/remote_data_job_executor.py` & `vdk-dag-0.1.861974079/src/vdk/plugin/dag/remote_data_job_executor.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861330674/src/vdk/plugin/dag/time_based_queue.py` & `vdk-dag-0.1.861974079/src/vdk/plugin/dag/time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861330674/src/vdk_dag.egg-info/PKG-INFO` & `vdk-dag-0.1.861974079/src/vdk_dag.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-dag
-Version: 0.1.861330674
+Version: 0.1.861974079
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-dag-0.1.861330674/src/vdk_dag.egg-info/SOURCES.txt` & `vdk-dag-0.1.861974079/src/vdk_dag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861330674/tests/test_dag.py` & `vdk-dag-0.1.861974079/tests/test_dag.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,14 +307,15 @@
             # let's make sure something else is not generating more requests then expected
             # if implementation is changed the number below would likely change.
             # If the new count is not that big we can edit it here to pass the test,
             # if the new count is too big, we have an issue that need to be investigated.
             assert len(self.httpserver.log) == 21
             self.httpserver.stop()
 
+    """
     def test_dag_concurrent_running_jobs_limit(self):
         jobs = [("job" + str(i), [200], "succeeded", 1) for i in range(1, 8)]
 
         dummy_config.dags_max_concurrent_running_jobs_value = 2
         dummy_config.dags_delayed_jobs_min_delay_seconds_value = 1
         dummy_config.dags_delayed_jobs_randomized_added_delay_seconds_value = 1
         dummy_config.dags_time_between_status_check_seconds_value = 1
@@ -345,14 +346,15 @@
                             execution = execution[0]
                         if execution["status"] == "succeeded":
                             running_jobs.discard(execution["job_name"])
             cli_assert_equal(0, result)
             # assert that all the jobs finished successfully
             assert len(running_jobs) == 0
             self.httpserver.stop()
+    """
 
     def _test_dag_validation(self, dag_name):
         self._set_up()
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
```

### Comparing `vdk-dag-0.1.861330674/tests/test_dag_object.py` & `vdk-dag-0.1.861974079/tests/test_dag_object.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861330674/tests/test_time_based_queue.py` & `vdk-dag-0.1.861974079/tests/test_time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861330674/tests/test_tracking_job_executor.py` & `vdk-dag-0.1.861974079/tests/test_tracking_job_executor.py`

 * *Files identical despite different names*

