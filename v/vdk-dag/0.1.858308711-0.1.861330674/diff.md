# Comparing `tmp/vdk-dag-0.1.858308711.tar.gz` & `tmp/vdk-dag-0.1.861330674.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-dag-0.1.858308711.tar", last modified: Fri May  5 11:30:46 2023, max compression
+gzip compressed data, was "vdk-dag-0.1.861330674.tar", last modified: Tue May  9 09:18:11 2023, max compression
```

## Comparing `vdk-dag-0.1.858308711.tar` & `vdk-dag-0.1.861330674.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:30:46.411283 vdk-dag-0.1.858308711/
--rw-r--r--   0 root         (0) root         (0)     8221 2023-05-05 11:30:46.411283 vdk-dag-0.1.858308711/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7654 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 11:30:46.411283 vdk-dag-0.1.858308711/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-05 11:30:36.000000 vdk-dag-0.1.858308711/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:30:46.407283 vdk-dag-0.1.858308711/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:30:46.407283 vdk-dag-0.1.858308711/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:30:46.407283 vdk-dag-0.1.858308711/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:30:46.411283 vdk-dag-0.1.858308711/src/vdk/plugin/dag/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:30:46.411283 vdk-dag-0.1.858308711/src/vdk/plugin/dag/api/
--rw-rw-rw-   0 root         (0) root         (0)     1375 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/api/dag.py
--rw-rw-rw-   0 root         (0) root         (0)     9308 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/cached_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     6078 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag.py
--rw-rw-rw-   0 root         (0) root         (0)     1385 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     6535 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag_plugin_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      923 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     7917 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     2253 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/dags.py
--rw-rw-rw-   0 root         (0) root         (0)     9334 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/remote_data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/remote_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     2579 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/src/vdk/plugin/dag/time_based_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:30:46.411283 vdk-dag-0.1.858308711/src/vdk_dag.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8221 2023-05-05 11:30:46.000000 vdk-dag-0.1.858308711/src/vdk_dag.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-05 11:30:46.000000 vdk-dag-0.1.858308711/src/vdk_dag.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 11:30:46.000000 vdk-dag-0.1.858308711/src/vdk_dag.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-05 11:30:46.000000 vdk-dag-0.1.858308711/src/vdk_dag.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-05 11:30:46.000000 vdk-dag-0.1.858308711/src/vdk_dag.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-05 11:30:46.000000 vdk-dag-0.1.858308711/src/vdk_dag.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:30:46.411283 vdk-dag-0.1.858308711/tests/
--rw-rw-rw-   0 root         (0) root         (0)    16367 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/tests/test_dag.py
--rw-rw-rw-   0 root         (0) root         (0)     2550 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/tests/test_dag_object.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/tests/test_time_based_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2285 2023-05-05 11:30:33.000000 vdk-dag-0.1.858308711/tests/test_tracking_job_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:18:11.848055 vdk-dag-0.1.861330674/
+-rw-r--r--   0 root         (0) root         (0)     8454 2023-05-09 09:18:11.848055 vdk-dag-0.1.861330674/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7887 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 09:18:11.848055 vdk-dag-0.1.861330674/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-09 09:18:00.000000 vdk-dag-0.1.861330674/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:18:11.844055 vdk-dag-0.1.861330674/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:18:11.844055 vdk-dag-0.1.861330674/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:18:11.844055 vdk-dag-0.1.861330674/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:18:11.848055 vdk-dag-0.1.861330674/src/vdk/plugin/dag/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:18:11.848055 vdk-dag-0.1.861330674/src/vdk/plugin/dag/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/api/dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     9308 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/cached_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6078 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6480 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag_plugin_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      923 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     7838 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2253 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/dags.py
+-rw-rw-rw-   0 root         (0) root         (0)     9334 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/remote_data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/remote_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2579 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/src/vdk/plugin/dag/time_based_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:18:11.848055 vdk-dag-0.1.861330674/src/vdk_dag.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8454 2023-05-09 09:18:11.000000 vdk-dag-0.1.861330674/src/vdk_dag.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-09 09:18:11.000000 vdk-dag-0.1.861330674/src/vdk_dag.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 09:18:11.000000 vdk-dag-0.1.861330674/src/vdk_dag.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-09 09:18:11.000000 vdk-dag-0.1.861330674/src/vdk_dag.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-09 09:18:11.000000 vdk-dag-0.1.861330674/src/vdk_dag.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-09 09:18:11.000000 vdk-dag-0.1.861330674/src/vdk_dag.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:18:11.848055 vdk-dag-0.1.861330674/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    16367 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/tests/test_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2550 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/tests/test_dag_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/tests/test_time_based_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2023-05-09 09:17:56.000000 vdk-dag-0.1.861330674/tests/test_tracking_job_executor.py
```

### Comparing `vdk-dag-0.1.858308711/PKG-INFO` & `vdk-dag-0.1.861330674/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: vdk-dag
-Version: 0.1.858308711
-Summary: Express dependecies between data jobs.
-Home-page: https://github.com/vmware/versatile-data-kit
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-
 # VDK DAGs
 
 Express dependencies between data jobs.
 
 A plugin for Versatile Data Kit extends its Job API with an additional feature that allows users to trigger so-called VDK DAGs.
 
 A VDK DAG is a regular Data Job that invokes other Data Jobs using Control Service Execution API.
@@ -50,16 +36,16 @@
         ...
     ]
     DagInput().run_dag(jobs)
 ```
 
 When defining a job to be run following attributes are supported:
 * **job_name**: required, the name of the data job.
-* **team_name:**: optional, the team of the data job. If omitted , it will use the meta job's team.
-* **fail_dag_on_error**: optional, default is true. If true, the meta job will abort and fail if the orchestrated job fails, if false, meta job won't fail and continue.
+* **team_name:**: optional, the team of the data job. If omitted , it will use the DAG's team.
+* **fail_dag_on_error**: optional, default is true. If true, the DAG will abort and fail if the orchestrated job fails, if false, DAG won't fail and continue.
 * **arguments**: optional, the arguments that are passed to the underlying orchestrated data job.
 * **depends_on**: required (can be empty), list of other jobs that the orchestrated job depends on. The job will not be started until depends_on job have finished.
 
 
 ### Example
 
 The following example dependency graph can be implemented with below code.
@@ -122,26 +108,26 @@
         "fail_dag_on_error": True,
         "arguments": {},
         "depends_on": ["job3"]
     },
 ]
 
 
-def run(job_input: IJobInput) - > None:
+def run(job_input: IJobInput) -> None:
     DagInput().run_dag(JOBS_RUN_ORDER)
 ```
 
 
 ### Runtime sequencing
 
 The depends_on key stores the dependencies of each job - the jobs that have to finish before it starts.
-The DAG execution starts from the jobs with empty dependency lists - they start together in parallel.
-But what happens if they are too many? It could cause server overload. In order to avoid such unfortunate situations,
-a limit in the number of concurrent running jobs is set. This limit is
-a [configuration variable](https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-dag/src/vdk/plugin/dag/dag_plugin_configuration.py#L87)
+The DAG execution starts from the jobs with empty dependency lists - they start together in parallel.  \
+But what happens if they are too many? It could cause server overload.  \
+In order to avoid such unfortunate situations, a limit in the number of concurrent running jobs is set.  \
+This limit is a [configuration variable](https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-dag/src/vdk/plugin/dag/dag_plugin_configuration.py#L87)
 that you are able to set according to your needs. When the limit is exceeded, the execution of the rest of the jobs
 is not cancelled but delayed until a spot is freed by one of the running jobs. What's important here is that
 although there are delayed jobs due to the limitation, the overall sequence is not broken.
 
 
 ### Data Job start comparison
 
@@ -153,44 +139,53 @@
 * Started by the user using UI or CLI
    * If a user tries to start a job that is already running, one would get an appropriate error immediately and a
      recommendation to try again later.
 * **Started by a DAG Job**
    * If a DAG job tries to start a job and there is already running such job, the approach of the DAG job would be
      similar to the schedule - retry later but more times.
 
+### Configuration
+
+The configuration variables of the VDK DAGs can be checked by running the command:
+```console
+vdk config-help
+```
+
+You will see all the VDK configuration variables. Search for _DAG_ in order to see the DAGs-related ones.
+
 ### FAQ
 
 
-**Q: Will the DAG retry on Platform Error?**<br>
+**Q: Will the DAG retry on Platform Error?**  \
 A: Yes, as any other job, up to N (configurable by the Control Service) attempts for each job it is orchestrating.
-   See Control Service documentation for more information
+See Control Service documentation for more information.
 
-**Q: If an orchestrated job fails, will the DAG fail?**<br>
-Only if fail_dag_on_error flag is set to True (which is teh default setting if omited)
+**Q: If an orchestrated job fails, will the DAG fail?**  \
+A: Only if fail_dag_on_error flag is set to True (which is the default setting if omitted).
 
 The DAG then will fail with USER error (regardless of how the orchestrated job failed)
 
 
-**Q: Am I able to run the DAG locally?**<br>
+**Q: Am I able to run the DAG locally?**  \
 A: Yes, but the jobs orchestrated must be deployed to the cloud (by the Control Service).
 
-**Q: Is there memory limit of the DAG?**<br>
+**Q: Is there memory limit of the DAG?**  \
 A: The normal per job limits apply for any jobs orchestrated/started by the DAG.
 
-**Q: Is there execution time limit of the DAG?**<br>
+**Q: Is there execution time limit of the DAG?**  \
 A: Yes, the DAG must finish within the same limit as any normal data job.
 The total time of all data jobs started by the DAG must be less than the limit specified.
-The overall limit is controlled by Control Service administrators
+The overall limit is controlled by Control Service administrators.
 
-**Q: Is the DAG going to fail and not trigger the remaining jobs if any of the jobs it is orchestrating fails?**<br>
-A: This is configurable by the end user in the parameter fail_dag_on_error
+**Q: Is the DAG going to fail and not trigger the remaining jobs if any of the jobs it is orchestrating fails?**  \
+A: This is configurable by the end user in the parameter fail_dag_on_error.
 
-**Q: Can I schedule one job to run every hour and use it in the DAG at the same time?**<br>
+**Q: Can I schedule one job to run every hour and use it in the DAG at the same time?**  \
 A: Yes, if the job is already running, the DAG will wait for the concurrent run to finish and then trigger the job again from the DAG,
-If the job is already running as part of the DAG, the concurrent scheduled run will be skipped
+If the job is already running as part of the DAG, the concurrent scheduled run will be skipped.
 
 
 ### Build and testing
 
 ```
 pip install -r requirements.txt
 pip install -e .
```

### Comparing `vdk-dag-0.1.858308711/README.md` & `vdk-dag-0.1.861330674/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: vdk-dag
+Version: 0.1.861330674
+Summary: Express dependecies between data jobs.
+Home-page: https://github.com/vmware/versatile-data-kit
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
 # VDK DAGs
 
 Express dependencies between data jobs.
 
 A plugin for Versatile Data Kit extends its Job API with an additional feature that allows users to trigger so-called VDK DAGs.
 
 A VDK DAG is a regular Data Job that invokes other Data Jobs using Control Service Execution API.
@@ -36,16 +50,16 @@
         ...
     ]
     DagInput().run_dag(jobs)
 ```
 
 When defining a job to be run following attributes are supported:
 * **job_name**: required, the name of the data job.
-* **team_name:**: optional, the team of the data job. If omitted , it will use the meta job's team.
-* **fail_dag_on_error**: optional, default is true. If true, the meta job will abort and fail if the orchestrated job fails, if false, meta job won't fail and continue.
+* **team_name:**: optional, the team of the data job. If omitted , it will use the DAG's team.
+* **fail_dag_on_error**: optional, default is true. If true, the DAG will abort and fail if the orchestrated job fails, if false, DAG won't fail and continue.
 * **arguments**: optional, the arguments that are passed to the underlying orchestrated data job.
 * **depends_on**: required (can be empty), list of other jobs that the orchestrated job depends on. The job will not be started until depends_on job have finished.
 
 
 ### Example
 
 The following example dependency graph can be implemented with below code.
@@ -108,26 +122,26 @@
         "fail_dag_on_error": True,
         "arguments": {},
         "depends_on": ["job3"]
     },
 ]
 
 
-def run(job_input: IJobInput) - > None:
+def run(job_input: IJobInput) -> None:
     DagInput().run_dag(JOBS_RUN_ORDER)
 ```
 
 
 ### Runtime sequencing
 
 The depends_on key stores the dependencies of each job - the jobs that have to finish before it starts.
-The DAG execution starts from the jobs with empty dependency lists - they start together in parallel.
-But what happens if they are too many? It could cause server overload. In order to avoid such unfortunate situations,
-a limit in the number of concurrent running jobs is set. This limit is
-a [configuration variable](https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-dag/src/vdk/plugin/dag/dag_plugin_configuration.py#L87)
+The DAG execution starts from the jobs with empty dependency lists - they start together in parallel.  \
+But what happens if they are too many? It could cause server overload.  \
+In order to avoid such unfortunate situations, a limit in the number of concurrent running jobs is set.  \
+This limit is a [configuration variable](https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-dag/src/vdk/plugin/dag/dag_plugin_configuration.py#L87)
 that you are able to set according to your needs. When the limit is exceeded, the execution of the rest of the jobs
 is not cancelled but delayed until a spot is freed by one of the running jobs. What's important here is that
 although there are delayed jobs due to the limitation, the overall sequence is not broken.
 
 
 ### Data Job start comparison
 
@@ -139,44 +153,53 @@
 * Started by the user using UI or CLI
    * If a user tries to start a job that is already running, one would get an appropriate error immediately and a
      recommendation to try again later.
 * **Started by a DAG Job**
    * If a DAG job tries to start a job and there is already running such job, the approach of the DAG job would be
      similar to the schedule - retry later but more times.
 
+### Configuration
+
+The configuration variables of the VDK DAGs can be checked by running the command:
+```console
+vdk config-help
+```
+
+You will see all the VDK configuration variables. Search for _DAG_ in order to see the DAGs-related ones.
+
 ### FAQ
 
 
-**Q: Will the DAG retry on Platform Error?**<br>
+**Q: Will the DAG retry on Platform Error?**  \
 A: Yes, as any other job, up to N (configurable by the Control Service) attempts for each job it is orchestrating.
-   See Control Service documentation for more information
+See Control Service documentation for more information.
 
-**Q: If an orchestrated job fails, will the DAG fail?**<br>
-Only if fail_dag_on_error flag is set to True (which is teh default setting if omited)
+**Q: If an orchestrated job fails, will the DAG fail?**  \
+A: Only if fail_dag_on_error flag is set to True (which is the default setting if omitted).
 
 The DAG then will fail with USER error (regardless of how the orchestrated job failed)
 
 
-**Q: Am I able to run the DAG locally?**<br>
+**Q: Am I able to run the DAG locally?**  \
 A: Yes, but the jobs orchestrated must be deployed to the cloud (by the Control Service).
 
-**Q: Is there memory limit of the DAG?**<br>
+**Q: Is there memory limit of the DAG?**  \
 A: The normal per job limits apply for any jobs orchestrated/started by the DAG.
 
-**Q: Is there execution time limit of the DAG?**<br>
+**Q: Is there execution time limit of the DAG?**  \
 A: Yes, the DAG must finish within the same limit as any normal data job.
 The total time of all data jobs started by the DAG must be less than the limit specified.
-The overall limit is controlled by Control Service administrators
+The overall limit is controlled by Control Service administrators.
 
-**Q: Is the DAG going to fail and not trigger the remaining jobs if any of the jobs it is orchestrating fails?**<br>
-A: This is configurable by the end user in the parameter fail_dag_on_error
+**Q: Is the DAG going to fail and not trigger the remaining jobs if any of the jobs it is orchestrating fails?**  \
+A: This is configurable by the end user in the parameter fail_dag_on_error.
 
-**Q: Can I schedule one job to run every hour and use it in the DAG at the same time?**<br>
+**Q: Can I schedule one job to run every hour and use it in the DAG at the same time?**  \
 A: Yes, if the job is already running, the DAG will wait for the concurrent run to finish and then trigger the job again from the DAG,
-If the job is already running as part of the DAG, the concurrent scheduled run will be skipped
+If the job is already running as part of the DAG, the concurrent scheduled run will be skipped.
 
 
 ### Build and testing
 
 ```
 pip install -r requirements.txt
 pip install -e .
```

### Comparing `vdk-dag-0.1.858308711/setup.py` & `vdk-dag-0.1.861330674/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.858308711"
+__version__ = "0.1.861330674"
 
 setuptools.setup(
     name="vdk-dag",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Express dependecies between data jobs.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-dag-0.1.858308711/src/vdk/plugin/dag/api/dag.py` & `vdk-dag-0.1.861330674/src/vdk/plugin/dag/api/dag.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.858308711/src/vdk/plugin/dag/cached_data_job_executor.py` & `vdk-dag-0.1.861330674/src/vdk/plugin/dag/cached_data_job_executor.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag.py` & `vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag_plugin.py` & `vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag_plugin_configuration.py` & `vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag_plugin_configuration.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,55 +20,55 @@
 
     def dags_delayed_jobs_min_delay_seconds(self):
         """
         Returns the minimum delay time for a delayed job to be executed in seconds.
 
         :return: the number of seconds for the minimum delay of a delayed job
 
-        :seealso: `META_JOBS_DELAYED_JOBS_MIN_DELAY_SECONDS <https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-meta-jobs/src/vdk/plugin/meta_jobs/meta_configuration.py#L90>`
+        :seealso: `DAGS_DELAYED_JOBS_MIN_DELAY_SECONDS <https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-dag/src/vdk/plugin/dag/dag_plugin_configuration.py#L90>`
         """
         return self.__config.get_value(DAGS_DELAYED_JOBS_MIN_DELAY_SECONDS)
 
     def dags_delayed_jobs_randomized_added_delay_seconds(self):
         """
         Returns the additional randomized delay time in seconds to the minimum delay time of a delayed job.
 
         :return: the number of seconds for the additional randomized delay of the delayed jobs
 
-        :seealso: `META_JOBS_DELAYED_JOBS_RANDOMIZED_ADDED_DELAY_SECONDS <https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-meta-jobs/src/vdk/plugin/meta_jobs/meta_configuration.py#L100>`
+        :seealso: `DAGS_DELAYED_JOBS_RANDOMIZED_ADDED_DELAY_SECONDS <https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-dag/src/vdk/plugin/dag/dag_plugin_configuration.py#L100>`
         """
         return self.__config.get_value(DAGS_DELAYED_JOBS_RANDOMIZED_ADDED_DELAY_SECONDS)
 
     def dags_dag_execution_check_time_period_seconds(self):
         """
         Returns the frequency at which the system checks a DAG execution's status.
 
         :return: the frequency in seconds at which the system checks a DAG execution's status
 
-        :seealso: `META_JOBS_DAG_EXECUTION_CHECK_TIME_PERIOD_SECONDS <https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-meta-jobs/src/vdk/plugin/meta_jobs/meta_configuration.py#L111>`
+        :seealso: `DAGS_DAG_EXECUTION_CHECK_TIME_PERIOD_SECONDS <https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-dag/src/vdk/plugin/dag/dag_plugin_configuration.py#L111>`
         """
         return self.__config.get_value(DAGS_DAG_EXECUTION_CHECK_TIME_PERIOD_SECONDS)
 
     def dags_time_between_status_check_seconds(self):
         """
         Returns the time interval in seconds between status checks for a job.
 
         :return: the number of seconds between status checks for a job.
 
-        :seealso: `META_JOBS_TIME_BETWEEN_STATUS_CHECK_SECONDS <https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-meta-jobs/src/vdk/plugin/meta_jobs/meta_configuration.py#L121>`
+        :seealso: `DAGS_TIME_BETWEEN_STATUS_CHECK_SECONDS <https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-dag/src/vdk/plugin/dag/dag_plugin_configuration.py#L121>`
         """
         return self.__config.get_value(DAGS_TIME_BETWEEN_STATUS_CHECK_SECONDS)
 
     def dags_max_concurrent_running_jobs(self):
         """
         Returns the limit of concurrent running jobs.
 
         :return: the number of maximum concurrent running jobs
 
-        :seealso: `META_JOBS_MAX_CONCURRENT_RUNNING_JOBS <https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-meta-jobs/src/vdk/plugin/meta_jobs/meta_configuration.py#L132>`
+        :seealso: `DAGS_MAX_CONCURRENT_RUNNING_JOBS <https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-dag/src/vdk/plugin/dag/dag_plugin_configuration.py#L132>`
         """
         return self.__config.get_value(DAGS_MAX_CONCURRENT_RUNNING_JOBS)
 
 
 def add_definitions(config_builder: ConfigurationBuilder):
     """
     Defines what configuration settings are needed for the DAGs plugin with reasonable defaults.
```

### Comparing `vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag_runner.py` & `vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag_runner.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.858308711/src/vdk/plugin/dag/dag_validator.py` & `vdk-dag-0.1.861330674/src/vdk/plugin/dag/dag_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,18 +73,16 @@
         self._validate_job_type(job)
         self._validate_allowed_and_required_keys(job)
         self._validate_job_name(job)
         job_name = job.get("job_name")
         self._validate_dependencies(job_name, job["depends_on"])
         if "team_name" in job:
             self._validate_team_name(job_name, job["team_name"])
-        if "fail_meta_job_on_error" in job:
-            self._validate_fail_meta_job_on_error(
-                job_name, job["fail_meta_job_on_error"]
-            )
+        if "fail_dag_on_error" in job:
+            self._validate_fail_dag_on_error(job_name, job["fail_dag_on_error"])
         if "arguments" in job:
             self._validate_arguments(job_name, job["arguments"])
         log.info(f"Successfully validated job: {job_name}")
 
     def _validate_job_type(self, job: Dict):
         if not isinstance(job, dict):
             self._raise_error(
@@ -149,23 +147,21 @@
                 ERROR.TYPE,
                 "The type of the job dict key job_name is not string.",
                 f"Change the Data Job Dict value of team_name. "
                 f"Current type is {type(team_name)}. Expected type is string.",
                 [job_name],
             )
 
-    def _validate_fail_meta_job_on_error(
-        self, job_name: str, fail_meta_job_on_error: bool
-    ):
-        if not isinstance(fail_meta_job_on_error, bool):
+    def _validate_fail_dag_on_error(self, job_name: str, fail_dag_on_error: bool):
+        if not isinstance(fail_dag_on_error, bool):
             self._raise_error(
                 ERROR.TYPE,
                 "The type of the job dict key fail_dag_on_error is not bool (True/False).",
                 f"Change the Data Job Dict value of fail_dag_on_error. Current type"
-                f" is {type(fail_meta_job_on_error)}. Expected type is bool.",
+                f" is {type(fail_dag_on_error)}. Expected type is bool.",
                 [job_name],
             )
 
     def _validate_arguments(self, job_name: str, job_args: dict):
         if not isinstance(job_args, dict):
             self._raise_error(
                 ERROR.TYPE,
```

### Comparing `vdk-dag-0.1.858308711/src/vdk/plugin/dag/dags.py` & `vdk-dag-0.1.861330674/src/vdk/plugin/dag/dags.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.858308711/src/vdk/plugin/dag/remote_data_job.py` & `vdk-dag-0.1.861330674/src/vdk/plugin/dag/remote_data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.858308711/src/vdk/plugin/dag/remote_data_job_executor.py` & `vdk-dag-0.1.861330674/src/vdk/plugin/dag/remote_data_job_executor.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.858308711/src/vdk/plugin/dag/time_based_queue.py` & `vdk-dag-0.1.861330674/src/vdk/plugin/dag/time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.858308711/src/vdk_dag.egg-info/PKG-INFO` & `vdk-dag-0.1.861330674/src/vdk_dag.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-dag
-Version: 0.1.858308711
+Version: 0.1.861330674
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -50,16 +50,16 @@
         ...
     ]
     DagInput().run_dag(jobs)
 ```
 
 When defining a job to be run following attributes are supported:
 * **job_name**: required, the name of the data job.
-* **team_name:**: optional, the team of the data job. If omitted , it will use the meta job's team.
-* **fail_dag_on_error**: optional, default is true. If true, the meta job will abort and fail if the orchestrated job fails, if false, meta job won't fail and continue.
+* **team_name:**: optional, the team of the data job. If omitted , it will use the DAG's team.
+* **fail_dag_on_error**: optional, default is true. If true, the DAG will abort and fail if the orchestrated job fails, if false, DAG won't fail and continue.
 * **arguments**: optional, the arguments that are passed to the underlying orchestrated data job.
 * **depends_on**: required (can be empty), list of other jobs that the orchestrated job depends on. The job will not be started until depends_on job have finished.
 
 
 ### Example
 
 The following example dependency graph can be implemented with below code.
@@ -122,26 +122,26 @@
         "fail_dag_on_error": True,
         "arguments": {},
         "depends_on": ["job3"]
     },
 ]
 
 
-def run(job_input: IJobInput) - > None:
+def run(job_input: IJobInput) -> None:
     DagInput().run_dag(JOBS_RUN_ORDER)
 ```
 
 
 ### Runtime sequencing
 
 The depends_on key stores the dependencies of each job - the jobs that have to finish before it starts.
-The DAG execution starts from the jobs with empty dependency lists - they start together in parallel.
-But what happens if they are too many? It could cause server overload. In order to avoid such unfortunate situations,
-a limit in the number of concurrent running jobs is set. This limit is
-a [configuration variable](https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-dag/src/vdk/plugin/dag/dag_plugin_configuration.py#L87)
+The DAG execution starts from the jobs with empty dependency lists - they start together in parallel.  \
+But what happens if they are too many? It could cause server overload.  \
+In order to avoid such unfortunate situations, a limit in the number of concurrent running jobs is set.  \
+This limit is a [configuration variable](https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-dag/src/vdk/plugin/dag/dag_plugin_configuration.py#L87)
 that you are able to set according to your needs. When the limit is exceeded, the execution of the rest of the jobs
 is not cancelled but delayed until a spot is freed by one of the running jobs. What's important here is that
 although there are delayed jobs due to the limitation, the overall sequence is not broken.
 
 
 ### Data Job start comparison
 
@@ -153,44 +153,53 @@
 * Started by the user using UI or CLI
    * If a user tries to start a job that is already running, one would get an appropriate error immediately and a
      recommendation to try again later.
 * **Started by a DAG Job**
    * If a DAG job tries to start a job and there is already running such job, the approach of the DAG job would be
      similar to the schedule - retry later but more times.
 
+### Configuration
+
+The configuration variables of the VDK DAGs can be checked by running the command:
+```console
+vdk config-help
+```
+
+You will see all the VDK configuration variables. Search for _DAG_ in order to see the DAGs-related ones.
+
 ### FAQ
 
 
-**Q: Will the DAG retry on Platform Error?**<br>
+**Q: Will the DAG retry on Platform Error?**  \
 A: Yes, as any other job, up to N (configurable by the Control Service) attempts for each job it is orchestrating.
-   See Control Service documentation for more information
+See Control Service documentation for more information.
 
-**Q: If an orchestrated job fails, will the DAG fail?**<br>
-Only if fail_dag_on_error flag is set to True (which is teh default setting if omited)
+**Q: If an orchestrated job fails, will the DAG fail?**  \
+A: Only if fail_dag_on_error flag is set to True (which is the default setting if omitted).
 
 The DAG then will fail with USER error (regardless of how the orchestrated job failed)
 
 
-**Q: Am I able to run the DAG locally?**<br>
+**Q: Am I able to run the DAG locally?**  \
 A: Yes, but the jobs orchestrated must be deployed to the cloud (by the Control Service).
 
-**Q: Is there memory limit of the DAG?**<br>
+**Q: Is there memory limit of the DAG?**  \
 A: The normal per job limits apply for any jobs orchestrated/started by the DAG.
 
-**Q: Is there execution time limit of the DAG?**<br>
+**Q: Is there execution time limit of the DAG?**  \
 A: Yes, the DAG must finish within the same limit as any normal data job.
 The total time of all data jobs started by the DAG must be less than the limit specified.
-The overall limit is controlled by Control Service administrators
+The overall limit is controlled by Control Service administrators.
 
-**Q: Is the DAG going to fail and not trigger the remaining jobs if any of the jobs it is orchestrating fails?**<br>
-A: This is configurable by the end user in the parameter fail_dag_on_error
+**Q: Is the DAG going to fail and not trigger the remaining jobs if any of the jobs it is orchestrating fails?**  \
+A: This is configurable by the end user in the parameter fail_dag_on_error.
 
-**Q: Can I schedule one job to run every hour and use it in the DAG at the same time?**<br>
+**Q: Can I schedule one job to run every hour and use it in the DAG at the same time?**  \
 A: Yes, if the job is already running, the DAG will wait for the concurrent run to finish and then trigger the job again from the DAG,
-If the job is already running as part of the DAG, the concurrent scheduled run will be skipped
+If the job is already running as part of the DAG, the concurrent scheduled run will be skipped.
 
 
 ### Build and testing
 
 ```
 pip install -r requirements.txt
 pip install -e .
```

### Comparing `vdk-dag-0.1.858308711/src/vdk_dag.egg-info/SOURCES.txt` & `vdk-dag-0.1.861330674/src/vdk_dag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.858308711/tests/test_dag.py` & `vdk-dag-0.1.861330674/tests/test_dag.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.858308711/tests/test_dag_object.py` & `vdk-dag-0.1.861330674/tests/test_dag_object.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.858308711/tests/test_time_based_queue.py` & `vdk-dag-0.1.861330674/tests/test_time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.858308711/tests/test_tracking_job_executor.py` & `vdk-dag-0.1.861330674/tests/test_tracking_job_executor.py`

 * *Files identical despite different names*

