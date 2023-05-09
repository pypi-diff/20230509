# Comparing `tmp/quantum_serverless-0.0.7.tar.gz` & `tmp/quantum_serverless-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantum_serverless-0.0.7.tar", last modified: Thu Apr 20 15:16:54 2023, max compression
+gzip compressed data, was "quantum_serverless-0.0.8.tar", last modified: Tue May  9 19:36:47 2023, max compression
```

## Comparing `quantum_serverless-0.0.7.tar` & `quantum_serverless-0.0.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.131033 quantum_serverless-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-20 15:16:54.131033 quantum_serverless-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.119033 quantum_serverless-0.0.7/quantum_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.127033 quantum_serverless-0.0.7/quantum_serverless/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/core/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/core/program.py
--rw-r--r--   0 runner    (1001) docker     (123)    20595 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/core/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/core/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.127033 quantum_serverless-0.0.7/quantum_serverless/library/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/library/transpiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/quantum_serverless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.127033 quantum_serverless-0.0.7/quantum_serverless/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/serializers/program_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/serializers/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.127033 quantum_serverless-0.0.7/quantum_serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/quantum_serverless/utils/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.123033 quantum_serverless-0.0.7/quantum_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-20 15:16:54.000000 quantum_serverless-0.0.7/quantum_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-20 15:16:54.000000 quantum_serverless-0.0.7/quantum_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:16:54.000000 quantum_serverless-0.0.7/quantum_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-20 15:16:54.000000 quantum_serverless-0.0.7/quantum_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-20 15:16:54.000000 quantum_serverless-0.0.7/quantum_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-20 15:16:54.131033 quantum_serverless-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.127033 quantum_serverless-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.131033 quantum_serverless-0.0.7/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/core/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/core/test_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/core/test_program_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/core/test_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.131033 quantum_serverless-0.0.7/tests/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/library/test_transpiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:54.131033 quantum_serverless-0.0.7/tests/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/serializers/test_program_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/serializers/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/test_quantum_serverless.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-20 15:16:45.000000 quantum_serverless-0.0.7/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.088641 quantum_serverless-0.0.8/quantum_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/quantum_serverless/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/core/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19235 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/core/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/core/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/quantum_serverless/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/library/transpiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/quantum_serverless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/quantum_serverless/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/serializers/program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/serializers/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/quantum_serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/quantum_serverless/utils/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/quantum_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-09 19:36:47.000000 quantum_serverless-0.0.8/quantum_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-09 19:36:47.000000 quantum_serverless-0.0.8/quantum_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:36:47.000000 quantum_serverless-0.0.8/quantum_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-09 19:36:47.000000 quantum_serverless-0.0.8/quantum_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 19:36:47.000000 quantum_serverless-0.0.8/quantum_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/core/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/core/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/core/test_program_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/core/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/library/test_transpiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:47.092640 quantum_serverless-0.0.8/tests/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/serializers/test_program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/serializers/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/test_quantum_serverless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-09 19:36:37.000000 quantum_serverless-0.0.8/tests/utils.py
```

### Comparing `quantum_serverless-0.0.7/quantum_serverless/__init__.py` & `quantum_serverless-0.0.8/quantum_serverless/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,22 @@
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
-"""Quantum serverless."""
+"""
+.. currentmodule:: quantum_serverless
+
+.. autosummary::
+    :toctree: ../stubs/
+
+    QuantumServerless
+"""
 
 from importlib_metadata import version as metadata_version, PackageNotFoundError
 
 from .core import (
     Provider,
     run_qiskit_remote,
     distribute_task,
```

### Comparing `quantum_serverless-0.0.7/quantum_serverless/core/__init__.py` & `quantum_serverless-0.0.8/quantum_serverless/core/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,16 +23,19 @@
 Core abstractions
 -----------------
 
 .. autosummary::
     :toctree: ../stubs/
 
     Provider
+    GatewayProvider
+    KuberayProvider
     ComputeResource
 
+    save_result
     distribute_task
     run_qiskit_remote
     get
     put
     get_refs_by_status
```

### Comparing `quantum_serverless-0.0.7/quantum_serverless/core/constants.py` & `quantum_serverless-0.0.8/quantum_serverless/core/constants.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/quantum_serverless/core/decorators.py` & `quantum_serverless-0.0.8/quantum_serverless/core/decorators.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/quantum_serverless/core/events.py` & `quantum_serverless-0.0.8/quantum_serverless/core/events.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/quantum_serverless/core/job.py` & `quantum_serverless-0.0.8/quantum_serverless/core/job.py`

 * *Files 23% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 
     RuntimeEnv
     Job
 """
 import json
 import logging
 import os
-from typing import Dict, Any
+import tarfile
+from typing import Dict, Any, Optional
 from uuid import uuid4
 
 import ray.runtime_env
 import requests
 from ray.dashboard.modules.job.sdk import JobSubmissionClient
 
 from quantum_serverless.core.constants import (
@@ -43,23 +44,27 @@
     ENV_JOB_GATEWAY_TOKEN,
     ENV_JOB_GATEWAY_HOST,
     ENV_JOB_ID_GATEWAY,
     ENV_GATEWAY_PROVIDER_VERSION,
     GATEWAY_PROVIDER_VERSION_DEFAULT,
 )
 from quantum_serverless.core.program import Program
+from quantum_serverless.exception import QuantumServerlessException
+from quantum_serverless.serializers.program_serializers import QiskitObjectsEncoder
 from quantum_serverless.utils.json import is_jsonable
 
 RuntimeEnv = ray.runtime_env.RuntimeEnv
 
 
 class BaseJobClient:
     """Base class for Job clients."""
 
-    def run_program(self, program: Program) -> "Job":
+    def run_program(
+        self, program: Program, arguments: Optional[Dict[str, Any]] = None
+    ) -> "Job":
         """Runs program."""
         raise NotImplementedError
 
     def status(self, job_id: str):
         """Check status."""
         raise NotImplementedError
 
@@ -96,25 +101,26 @@
 
     def logs(self, job_id: str):
         return self._job_client.get_job_logs(job_id)
 
     def result(self, job_id: str):
         return self.logs(job_id)
 
-    def run_program(self, program: Program):
-        arguments = ""
+    def run_program(self, program: Program, arguments: Optional[Dict[str, Any]] = None):
+        arguments = arguments or {}
+        arguments_string = ""
         if program.arguments is not None:
             arg_list = []
-            for key, value in program.arguments.items():
+            for key, value in arguments.items():
                 if isinstance(value, dict):
                     arg_list.append(f"--{key}='{json.dumps(value)}'")
                 else:
                     arg_list.append(f"--{key}={value}")
-            arguments = " ".join(arg_list)
-        entrypoint = f"python {program.entrypoint} {arguments}"
+            arguments_string = " ".join(arg_list)
+        entrypoint = f"python {program.entrypoint} {arguments_string}"
 
         # set program name so OT can use it as parent span name
         env_vars = {
             **(program.env_vars or {}),
             **{OT_PROGRAM_NAME: program.title},
         }
 
@@ -141,14 +147,51 @@
             version: gateway version
             token: authorization token
         """
         self.host = host
         self.version = version
         self._token = token
 
+    def run_program(
+        self, program: Program, arguments: Optional[Dict[str, Any]] = None
+    ) -> "Job":
+        url = f"{self.host}/api/{self.version}/programs/run/"
+        artifact_file_path = os.path.join(program.working_dir, "artifact.tar")
+
+        with tarfile.open(artifact_file_path, "w") as tar:
+            for filename in os.listdir(program.working_dir):
+                fpath = os.path.join(program.working_dir, filename)
+                tar.add(fpath, arcname=filename)
+
+        with open(artifact_file_path, "rb") as file:
+            response = requests.post(
+                url=url,
+                data={
+                    "title": program.title,
+                    "entrypoint": program.entrypoint,
+                    "arguments": json.dumps(arguments or {}, cls=QiskitObjectsEncoder),
+                    "dependencies": json.dumps(program.dependencies or []),
+                },
+                files={"artifact": file},
+                headers={"Authorization": f"Bearer {self._token}"},
+                timeout=REQUESTS_TIMEOUT,
+            )
+            if not response.ok:
+                raise QuantumServerlessException(
+                    f"Something went wrong with program execution. {response.text}"
+                )
+
+            json_response = json.loads(response.text)
+            job_id = json_response.get("id")
+
+        if os.path.exists(artifact_file_path):
+            os.remove(artifact_file_path)
+
+        return Job(job_id, job_client=self)
+
     def status(self, job_id: str):
         default_status = "Unknown"
         status = default_status
         response = requests.get(
             f"{self.host}/api/{self.version}/jobs/{job_id}/",
             headers={"Authorization": f"Bearer {self._token}"},
             timeout=REQUESTS_TIMEOUT,
@@ -158,15 +201,27 @@
         else:
             logging.warning(
                 "Something went wrong during job status fetching. %s", response.text
             )
         return status
 
     def stop(self, job_id: str):
-        raise NotImplementedError
+        message = ""
+        response = requests.post(
+            f"{self.host}/api/{self.version}/jobs/{job_id}/stop/",
+            headers={"Authorization": f"Bearer {self._token}"},
+            timeout=REQUESTS_TIMEOUT,
+        )
+        if response.ok:
+            message = json.loads(response.text).get("message", None)
+        else:
+            logging.warning(
+                "Something went wrong during job stopping. %s", response.text
+            )
+        return message
 
     def logs(self, job_id: str):
         result = None
         response = requests.get(
             f"{self.host}/api/{self.version}/jobs/{job_id}/logs/",
             headers={"Authorization": f"Bearer {self._token}"},
             timeout=REQUESTS_TIMEOUT,
@@ -183,15 +238,16 @@
         result = None
         response = requests.get(
             f"{self.host}/api/{self.version}/jobs/{job_id}/",
             headers={"Authorization": f"Bearer {self._token}"},
             timeout=REQUESTS_TIMEOUT,
         )
         if response.ok:
-            result = json.loads(response.text).get("result", None)
+            json_result = json.loads(response.text).get("result", "{}")
+            result = json.loads(json_result or "{}")
         else:
             logging.warning(
                 "Something went wrong during job result fetching. %s", response.text
             )
         return result
```

### Comparing `quantum_serverless-0.0.7/quantum_serverless/core/program.py` & `quantum_serverless-0.0.8/quantum_serverless/core/program.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,40 +27,38 @@
     Program
 """
 import dataclasses
 import json
 import logging
 import os
 import tarfile
+import warnings
 from abc import ABC
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional, Dict, List, Any
 
 import requests
 
 from quantum_serverless.core.constants import (
     REPO_HOST_KEY,
     REPO_PORT_KEY,
 )
-
 from quantum_serverless.exception import QuantumServerlessException
-from quantum_serverless.serializers.program_serializers import QiskitObjectsEncoder
-from quantum_serverless.utils.json import is_jsonable
 
 
 @dataclass
 class Program:  # pylint: disable=too-many-instance-attributes
     """Serverless Program.
 
     Args:
         title: program name
         entrypoint: is a script that will be executed as a job
             ex: job.py
-        arguments: arguments for entrypoint script
+        arguments: (deprecated) arguments for entrypoint script
         env_vars: env vars
         dependencies: list of python dependencies to execute a program
         working_dir: directory where entrypoint file is located
         description: description of a program
         version: version of a program
     """
 
@@ -77,19 +75,22 @@
     @classmethod
     def from_json(cls, data: Dict[str, Any]):
         """Reconstructs Program from dictionary."""
         field_names = set(f.name for f in dataclasses.fields(Program))
         return Program(**{k: v for k, v in data.items() if k in field_names})
 
     def __post_init__(self):
-        if self.arguments is not None and not is_jsonable(
-            self.arguments, cls=QiskitObjectsEncoder
-        ):
-            raise QuantumServerlessException(
-                "Arguments provided are not json serializable."
+        if self.arguments is not None:
+            warnings.warn(
+                "Passing `arguments` as constructor argument to `Program` is deprecated "
+                "and will be removed in v0.2. "
+                "Please, consider passing `arguments` to `run_program` "
+                "method of `QuantumServerless` object.",
+                DeprecationWarning,
+                stacklevel=2,
             )
 
 
 class ProgramStorage(ABC):
     """Base program backend to save and load programs from."""
 
     def save_program(self, program: Program) -> bool:
```

### Comparing `quantum_serverless-0.0.7/quantum_serverless/core/provider.py` & `quantum_serverless-0.0.8/quantum_serverless/core/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,16 @@
 
     ComputeResource
     Provider
 """
 import json
 import logging
 import os.path
-import tarfile
 from dataclasses import dataclass
-from typing import Optional, List, Dict
+from typing import Optional, List, Dict, Any
 
 import ray
 import requests
 from ray.dashboard.modules.job.sdk import JobSubmissionClient
 
 from quantum_serverless.core.constants import (
     RAY_IMAGE,
@@ -49,15 +48,14 @@
     RayJobClient,
     GatewayJobClient,
     BaseJobClient,
 )
 from quantum_serverless.core.program import Program
 from quantum_serverless.core.tracing import _trace_env_vars
 from quantum_serverless.exception import QuantumServerlessException
-from quantum_serverless.serializers.program_serializers import QiskitObjectsEncoder
 from quantum_serverless.utils import JsonSerializable
 
 TIMEOUT = 30
 
 
 @dataclass
 class ComputeResource:
@@ -249,28 +247,31 @@
             logging.warning(  # pylint: disable=logging-fstring-interpolation
                 "Job has not been found as no provider "
                 "with remote host has been configured. "
             )
             return None
         return Job(job_id=job_id, job_client=job_client)
 
-    def run_program(self, program: Program) -> Job:
+    def run_program(
+        self, program: Program, arguments: Optional[Dict[str, Any]] = None
+    ) -> Job:
         """Execute a program as a async job.
 
         Example:
             >>> serverless = QuantumServerless()
             >>> program = Program(
             >>>     "job.py",
             >>>     arguments={"arg1": "val1"},
             >>>     dependencies=["requests"]
             >>> )
             >>> job = serverless.run_program(program)
             >>> # <Job | ...>
 
         Args:
+            arguments: arguments to run program with
             program: Program object
 
         Returns:
             Job
         """
         job_client = self.job_client()
 
@@ -278,15 +279,15 @@
             logging.warning(  # pylint: disable=logging-fstring-interpolation
                 f"Job has not been submitted as no provider "
                 f"with remote host has been configured. "
                 f"Selected provider: {self}"
             )
             return None
 
-        return job_client.run_program(program)
+        return job_client.run_program(program, arguments)
 
 
 class KuberayProvider(Provider):
     """Implements CRUD for Kuberay API server."""
 
     def __init__(
         self,
@@ -513,14 +514,16 @@
         super().__init__(name)
         self.host = host
         self.version = version
         self._token = token
         if token is None:
             self._fetch_token(username, password)
 
+        self._job_client = GatewayJobClient(self.host, self._token, self.version)
+
     def get_compute_resources(self) -> List[ComputeResource]:
         raise NotImplementedError("GatewayProvider does not support resources api yet.")
 
     def create_compute_resource(self, resource) -> int:
         raise NotImplementedError("GatewayProvider does not support resources api yet.")
 
     def delete_compute_resource(self, resource) -> int:
@@ -534,73 +537,39 @@
             headers={"Authorization": f"Bearer {self._token}"},
             timeout=REQUESTS_TIMEOUT,
         )
         if response.ok:
             data = json.loads(response.text)
             job = Job(
                 job_id=data.get("id"),
-                job_client=GatewayJobClient(self.host, self._token, self.version),
+                job_client=self._job_client,
             )
         else:
             logging.warning(response.text)
 
         return job
 
-    def run_program(self, program: Program) -> Job:
-        url = f"{self.host}/api/{self.version}/programs/run/"
-        artifact_file_path = os.path.join(program.working_dir, "artifact.tar")
-
-        with tarfile.open(artifact_file_path, "w") as tar:
-            for filename in os.listdir(program.working_dir):
-                fpath = os.path.join(program.working_dir, filename)
-                tar.add(fpath, arcname=filename)
-
-        with open(artifact_file_path, "rb") as file:
-            response = requests.post(
-                url=url,
-                data={
-                    "title": program.title,
-                    "entrypoint": program.entrypoint,
-                    "arguments": json.dumps(
-                        program.arguments or {}, cls=QiskitObjectsEncoder
-                    ),
-                    "dependencies": json.dumps(program.dependencies or []),
-                },
-                files={"artifact": file},
-                headers={"Authorization": f"Bearer {self._token}"},
-                timeout=REQUESTS_TIMEOUT,
-            )
-            if not response.ok:
-                raise QuantumServerlessException(
-                    f"Something went wrong with program execution. {response.text}"
-                )
-
-            json_response = json.loads(response.text)
-            job_id = json_response.get("id")
-
-        if os.path.exists(artifact_file_path):
-            os.remove(artifact_file_path)
-
-        return Job(
-            job_id, job_client=GatewayJobClient(self.host, self._token, self.version)
-        )
+    def run_program(
+        self, program: Program, arguments: Optional[Dict[str, Any]] = None
+    ) -> Job:
+        return self._job_client.run_program(program, arguments)
 
     def get_jobs(self, **kwargs) -> List[Job]:
         jobs = []
         url = f"{self.host}/api/{self.version}/jobs/"
         response = requests.get(
             url,
             headers={"Authorization": f"Bearer {self._token}"},
             timeout=REQUESTS_TIMEOUT,
         )
         if response.ok:
             jobs = [
                 Job(
                     job_id=job.get("id"),
-                    job_client=GatewayJobClient(self.host, self._token, self.version),
+                    job_client=self._job_client,
                 )
                 for job in json.loads(response.text).get("results", [])
             ]
         else:
             logging.warning(response.text)
 
         return jobs
@@ -611,9 +580,9 @@
             data={"username": username, "password": password},
             timeout=REQUESTS_TIMEOUT,
         )
 
         if not gateway_response.ok:
             raise QuantumServerlessException(gateway_response.text)
 
-        gateway_token = json.loads(gateway_response.text).get("access_token")
+        gateway_token = json.loads(gateway_response.text).get("access")
         self._token = gateway_token
```

### Comparing `quantum_serverless-0.0.7/quantum_serverless/core/state.py` & `quantum_serverless-0.0.8/quantum_serverless/core/state.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/quantum_serverless/core/tracing.py` & `quantum_serverless-0.0.8/quantum_serverless/core/tracing.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,20 +26,18 @@
     get_tracer
 """
 
 import os
 from typing import Dict, Optional
 
 from opentelemetry import trace
-from opentelemetry.exporter.jaeger.thrift import JaegerExporter
+from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk.resources import SERVICE_NAME, Resource
 from opentelemetry.sdk.trace import TracerProvider
-from opentelemetry.sdk.trace.export import (
-    SimpleSpanProcessor,
-)
+from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from opentelemetry.trace import Tracer
 from opentelemetry.trace.propagation.tracecontext import TraceContextTextMapPropagator
 
 from quantum_serverless.core.constants import (
     OT_PROGRAM_NAME,
     OT_PROGRAM_NAME_DEFAULT,
     OT_JAEGER_HOST_KEY,
@@ -71,19 +69,18 @@
     resource = Resource(
         attributes={
             SERVICE_NAME: f"qs.{os.environ.get(OT_PROGRAM_NAME, OT_PROGRAM_NAME_DEFAULT)}"
         }
     )
     provider = TracerProvider(resource=resource)
     if agent_host is not None and agent_port is not None:
-        jaeger_exporter = JaegerExporter(
-            agent_host_name=agent_host,
-            agent_port=agent_port,
+        otel_exporter = BatchSpanProcessor(
+            OTLPSpanExporter(endpoint=f"{agent_host}:{agent_port}")
         )
-        provider.add_span_processor(SimpleSpanProcessor(jaeger_exporter))
+        provider.add_span_processor(otel_exporter)
     trace._set_tracer_provider(provider, log=False)  # pylint: disable=protected-access
     return trace.get_tracer(instrumenting_module_name)
 
 
 def _trace_env_vars(env_vars: dict, location: Optional[str] = None):
     """Sets env variables for tracing across executable function.
```

### Comparing `quantum_serverless-0.0.7/quantum_serverless/exception.py` & `quantum_serverless-0.0.8/quantum_serverless/exception.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/quantum_serverless/library/__init__.py` & `quantum_serverless-0.0.8/quantum_serverless/library/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/quantum_serverless/library/transpiler.py` & `quantum_serverless-0.0.8/quantum_serverless/library/transpiler.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/quantum_serverless/quantum_serverless.py` & `quantum_serverless-0.0.8/quantum_serverless/quantum_serverless.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,34 +81,38 @@
         self._allocated_context = None
 
     @property
     def job_client(self):
         """Job client for given provider."""
         return self._selected_provider.job_client()
 
-    def run_program(self, program: Program) -> Optional[Job]:
+    def run_program(
+        self, program: Program, arguments: Optional[Dict[str, Any]] = None
+    ) -> Optional[Job]:
         """Execute a program as a async job
 
         Example:
             >>> serverless = QuantumServerless()
             >>> program = Program(
             >>>     "job.py",
-            >>>     arguments={"arg1": "val1"},
             >>>     dependencies=["requests"]
             >>> )
-            >>> job = serverless.run_program(program)
+            >>> job = serverless.run_program(program, {"arg1": 1})
             >>> # <Job | ...>
 
         Args:
+            arguments: arguments to run program with
             program: Program object
 
         Returns:
             Job
         """
-        return self._selected_provider.run_program(program)
+        if program.arguments is not None:
+            arguments = program.arguments
+        return self._selected_provider.run_program(program, arguments)
 
     def get_job_by_id(self, job_id: str) -> Optional[Job]:
         """Returns job by job id.
 
         Args:
             job_id: job id
```

### Comparing `quantum_serverless-0.0.7/quantum_serverless/serializers/__init__.py` & `quantum_serverless-0.0.8/quantum_serverless/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/quantum_serverless/serializers/program_serializers.py` & `quantum_serverless-0.0.8/quantum_serverless/serializers/program_serializers.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 Quantum serverless program serializers
 ======================================
 
 .. autosummary::
     :toctree: ../stubs/
 
-
+    QiskitObjectsDecoder
+    QiskitObjectsEncoder
 """
 import json
 import os
 from typing import Any, Dict
 
 from qiskit_ibm_runtime import QiskitRuntimeService
 from qiskit_ibm_runtime.utils.json import RuntimeDecoder, RuntimeEncoder
```

### Comparing `quantum_serverless-0.0.7/quantum_serverless/serializers/serializers.py` & `quantum_serverless-0.0.8/quantum_serverless/serializers/serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/quantum_serverless/utils/__init__.py` & `quantum_serverless-0.0.8/quantum_serverless/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/quantum_serverless/utils/json.py` & `quantum_serverless-0.0.8/quantum_serverless/utils/json.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/quantum_serverless.egg-info/SOURCES.txt` & `quantum_serverless-0.0.8/quantum_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/setup.py` & `quantum_serverless-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/tests/core/test_decorator.py` & `quantum_serverless-0.0.8/tests/core/test_decorator.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/tests/core/test_program.py` & `quantum_serverless-0.0.8/tests/core/test_program.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/tests/core/test_program_repository.py` & `quantum_serverless-0.0.8/tests/core/test_program_repository.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/tests/core/test_state.py` & `quantum_serverless-0.0.8/tests/core/test_state.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/tests/library/test_transpiler.py` & `quantum_serverless-0.0.8/tests/library/test_transpiler.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/tests/serializers/test_program_serializers.py` & `quantum_serverless-0.0.8/tests/serializers/test_program_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/tests/serializers/test_serializers.py` & `quantum_serverless-0.0.8/tests/serializers/test_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/tests/test_quantum_serverless.py` & `quantum_serverless-0.0.8/tests/test_quantum_serverless.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.0.7/tests/utils.py` & `quantum_serverless-0.0.8/tests/utils.py`

 * *Files identical despite different names*

