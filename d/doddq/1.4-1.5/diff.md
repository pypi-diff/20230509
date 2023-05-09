# Comparing `tmp/doddq-1.4.tar.gz` & `tmp/doddq-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doddq-1.4.tar", last modified: Sun Sep  4 18:35:45 2022, max compression
+gzip compressed data, was "doddq-1.5.tar", last modified: Tue May  9 15:12:26 2023, max compression
```

## Comparing `doddq-1.4.tar` & `doddq-1.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-09-04 18:35:45.439211 doddq-1.4/
--rw-rw-rw-   0        0        0     1091 2021-11-29 00:59:00.000000 doddq-1.4/LICENSE.md
--rw-rw-rw-   0        0        0       29 2021-11-29 01:24:02.000000 doddq-1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      987 2022-09-04 18:35:45.440210 doddq-1.4/PKG-INFO
--rw-rw-rw-   0        0        0      463 2022-02-23 11:18:04.000000 doddq-1.4/README.md
--rw-rw-rw-   0        0        0      110 2021-11-29 01:56:28.000000 doddq-1.4/pyproject.toml
--rw-rw-rw-   0        0        0      660 2022-09-04 18:35:45.442209 doddq-1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-09-04 18:35:45.408244 doddq-1.4/src/
-drwxrwxrwx   0        0        0        0 2022-09-04 18:35:45.419232 doddq-1.4/src/doddq/
--rw-rw-rw-   0        0        0        0 2021-11-29 01:55:10.000000 doddq-1.4/src/doddq/__init__.py
--rw-rw-rw-   0        0        0     9562 2022-08-26 23:22:50.000000 doddq-1.4/src/doddq/helpers.py
--rw-rw-rw-   0        0        0     2505 2022-08-25 09:36:25.000000 doddq-1.4/src/doddq/rodeo.py
-drwxrwxrwx   0        0        0        0 2022-09-04 18:35:45.438213 doddq-1.4/src/doddq.egg-info/
--rw-rw-rw-   0        0        0      987 2022-09-04 18:35:45.000000 doddq-1.4/src/doddq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2022-09-04 18:35:45.000000 doddq-1.4/src/doddq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-04 18:35:45.000000 doddq-1.4/src/doddq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-09-04 18:35:45.000000 doddq-1.4/src/doddq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 15:12:26.204281 doddq-1.5/
+-rw-rw-rw-   0        0        0     1091 2021-11-29 00:59:00.000000 doddq-1.5/LICENSE.md
+-rw-rw-rw-   0        0        0       29 2021-11-29 01:24:02.000000 doddq-1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      955 2023-05-09 15:12:26.204281 doddq-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-05-09 15:05:29.000000 doddq-1.5/README.md
+-rw-rw-rw-   0        0        0      110 2021-11-29 01:56:28.000000 doddq-1.5/pyproject.toml
+-rw-rw-rw-   0        0        0      689 2023-05-09 15:12:26.206278 doddq-1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 15:12:26.118349 doddq-1.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 15:12:26.176310 doddq-1.5/src/doddq/
+-rw-rw-rw-   0        0        0        0 2021-11-29 01:55:10.000000 doddq-1.5/src/doddq/__init__.py
+-rw-rw-rw-   0        0        0     9599 2023-05-09 00:19:56.000000 doddq-1.5/src/doddq/helpers.py
+-rw-rw-rw-   0        0        0     2505 2023-05-09 15:08:16.000000 doddq-1.5/src/doddq/rodeo.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:12:26.202284 doddq-1.5/src/doddq.egg-info/
+-rw-rw-rw-   0        0        0      955 2023-05-09 15:12:26.000000 doddq-1.5/src/doddq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-05-09 15:12:26.000000 doddq-1.5/src/doddq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 15:12:26.000000 doddq-1.5/src/doddq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-09 15:12:26.000000 doddq-1.5/src/doddq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-09 15:12:26.000000 doddq-1.5/src/doddq.egg-info/top_level.txt
```

### Comparing `doddq-1.4/LICENSE.md` & `doddq-1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `doddq-1.4/PKG-INFO` & `doddq-1.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: doddq
-Version: 1.4
-Summary: A simple library for use with Qiskit. Requires NumPy!
+Version: 1.5
+Summary: A simple library for use with Qiskit.
 Home-page: https://github.com/tomdodd4598/doddq
 Author: Tom Dodd
 Author-email: joedodd35@gmail.com
 Project-URL: Issues, https://github.com/tomdodd4598/doddq/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,14 @@
 DoddQ
 =====
 
 
 Summary
 -------
 
-A simple library for use with Qiskit. Requires NumPy! Available as the ['doddq'](https://pypi.org/project/doddq/) package (`pip install doddq`).
+A simple library for use with Qiskit. Available as the ['doddq'](https://pypi.org/project/doddq/) package (`pip install doddq`).
 
 
 Permissions
 -----------
 
 In practice, the license on any code I write means very little, but for those who want a some semblance of formality, let it be stated that all code is available under the [MIT License](https://github.com/tomdodd4598/doddq/blob/main/LICENSE.md).
```

### Comparing `doddq-1.4/src/doddq/helpers.py` & `doddq-1.5/src/doddq/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 from qiskit.circuit.library import XGate, YGate, ZGate
 from qiskit.extensions import HamiltonianGate
 from qiskit.providers import Backend
 from qiskit.quantum_info import Operator
 from qiskit.result import Result
 from typing import Any, Callable
 
+pool_size = max(1, mp.cpu_count() - 1)
+
 
 def get_mp_pool() -> mp.Pool:
-    return mp.Pool(mp.cpu_count())
+    return mp.Pool(pool_size)
 
 
 def mp_starmap(function: Callable, *args, chunksize=mp.cpu_count()) -> Any:
     pool = get_mp_pool()
     return pool.starmap(function, *args, chunksize=chunksize)
```

### Comparing `doddq-1.4/src/doddq/rodeo.py` & `doddq-1.5/src/doddq/rodeo.py`

 * *Files identical despite different names*

### Comparing `doddq-1.4/src/doddq.egg-info/PKG-INFO` & `doddq-1.5/src/doddq.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: doddq
-Version: 1.4
-Summary: A simple library for use with Qiskit. Requires NumPy!
+Version: 1.5
+Summary: A simple library for use with Qiskit.
 Home-page: https://github.com/tomdodd4598/doddq
 Author: Tom Dodd
 Author-email: joedodd35@gmail.com
 Project-URL: Issues, https://github.com/tomdodd4598/doddq/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,14 @@
 DoddQ
 =====
 
 
 Summary
 -------
 
-A simple library for use with Qiskit. Requires NumPy! Available as the ['doddq'](https://pypi.org/project/doddq/) package (`pip install doddq`).
+A simple library for use with Qiskit. Available as the ['doddq'](https://pypi.org/project/doddq/) package (`pip install doddq`).
 
 
 Permissions
 -----------
 
 In practice, the license on any code I write means very little, but for those who want a some semblance of formality, let it be stated that all code is available under the [MIT License](https://github.com/tomdodd4598/doddq/blob/main/LICENSE.md).
```

