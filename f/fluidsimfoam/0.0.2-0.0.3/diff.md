# Comparing `tmp/fluidsimfoam-0.0.2.tar.gz` & `tmp/fluidsimfoam-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluidsimfoam-0.0.2.tar", max compression
+gzip compressed data, was "fluidsimfoam-0.0.3.tar", max compression
```

## Comparing `fluidsimfoam-0.0.2.tar` & `fluidsimfoam-0.0.3.tar`

### file list

```diff
@@ -1,41 +1,53 @@
--rw-r--r--   0        0        0     1521 2023-03-02 21:01:46.291446 fluidsimfoam-0.0.2/LICENSE
--rw-r--r--   0        0        0     2121 2023-04-26 15:04:34.458125 fluidsimfoam-0.0.2/README.md
--rw-r--r--   0        0        0     1348 2023-04-26 13:27:25.261100 fluidsimfoam-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1807 2023-04-26 14:23:21.793720 fluidsimfoam-0.0.2/src/fluidsimfoam/__init__.py
--rw-r--r--   0        0        0     1396 2023-04-26 14:37:40.374320 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/__init__.py
--rw-r--r--   0        0        0     1479 2023-04-26 14:37:42.998294 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    12515 2023-04-21 00:50:26.088622 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/__pycache__/ast.cpython-310.pyc
--rw-r--r--   0        0        0     4172 2023-04-26 12:06:21.876324 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/__pycache__/generators.cpython-310.pyc
--rw-r--r--   0        0        0    10425 2023-04-20 19:59:36.408013 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/__pycache__/parser.cpython-310.pyc
--rw-r--r--   0        0        0    11079 2023-04-21 00:50:23.720680 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/ast.py
--rw-r--r--   0        0        0     1080 2023-04-23 15:48:42.099657 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/LICENSE
--rw-r--r--   0        0        0    13165 2023-04-26 14:48:53.674766 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/__init__.py
--rw-r--r--   0        0        0    14349 2023-04-26 14:48:56.026761 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2350 2023-04-24 21:00:37.401533 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/__pycache__/edges.cpython-310.pyc
--rw-r--r--   0        0        0     3091 2023-04-24 20:58:19.530657 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/__pycache__/grading.cpython-310.pyc
--rw-r--r--   0        0        0     1810 2023-04-24 21:00:31.761612 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/edges.py
--rw-r--r--   0        0        0     3426 2023-04-24 20:58:16.942659 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/grading.py
--rw-r--r--   0        0        0     3702 2023-04-26 12:06:20.328322 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/generators.py
--rw-r--r--   0        0        0     1918 2023-04-18 19:23:17.863337 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/grammar.lark
--rw-r--r--   0        0        0     2335 2023-04-18 19:23:17.863337 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/grammar_advanced.lark
--rw-r--r--   0        0        0     9483 2023-04-20 19:59:34.795586 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/parser.py
--rw-r--r--   0        0        0     1283 2023-04-26 12:46:10.782261 fluidsimfoam-0.0.2/src/fluidsimfoam/info.py
--rw-r--r--   0        0        0       70 2023-04-26 12:56:51.898012 fluidsimfoam-0.0.2/src/fluidsimfoam/init_fields.py
--rw-r--r--   0        0        0      737 2023-03-02 21:01:46.299445 fluidsimfoam-0.0.2/src/fluidsimfoam/log.py
--rw-r--r--   0        0        0      310 2023-04-20 19:12:16.643975 fluidsimfoam-0.0.2/src/fluidsimfoam/make.py
--rw-r--r--   0        0        0     1115 2023-03-09 20:43:08.717722 fluidsimfoam-0.0.2/src/fluidsimfoam/next_fluidsim_core.py
--rw-r--r--   0        0        0      208 2023-04-26 13:04:37.103178 fluidsimfoam-0.0.2/src/fluidsimfoam/operators.py
--rw-r--r--   0        0        0       25 2023-03-02 21:01:46.299445 fluidsimfoam-0.0.2/src/fluidsimfoam/output/__init__.py
--rw-r--r--   0        0        0      193 2023-03-02 21:06:12.233495 fluidsimfoam-0.0.2/src/fluidsimfoam/output/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     9044 2023-04-26 13:42:10.597508 fluidsimfoam-0.0.2/src/fluidsimfoam/output/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0    10986 2023-04-26 13:42:06.101527 fluidsimfoam-0.0.2/src/fluidsimfoam/output/base.py
--rw-r--r--   0        0        0      497 2023-03-09 20:43:08.721719 fluidsimfoam-0.0.2/src/fluidsimfoam/resources/__init__.py
--rw-r--r--   0        0        0      870 2023-03-09 20:43:42.985533 fluidsimfoam-0.0.2/src/fluidsimfoam/resources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2759 2023-04-26 14:14:21.141790 fluidsimfoam-0.0.2/src/fluidsimfoam/solvers/__init__.py
--rw-r--r--   0        0        0     2614 2023-04-26 14:14:23.597814 fluidsimfoam-0.0.2/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1642 2023-04-21 01:35:51.333383 fluidsimfoam-0.0.2/src/fluidsimfoam/solvers/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     1683 2023-04-21 01:35:47.023225 fluidsimfoam-0.0.2/src/fluidsimfoam/solvers/base.py
--rw-r--r--   0        0        0      592 2023-04-21 18:34:01.041339 fluidsimfoam-0.0.2/src/fluidsimfoam/tasks.py
--rw-r--r--   0        0        0     1145 2023-03-09 20:43:42.785643 fluidsimfoam-0.0.2/src/fluidsimfoam/util/__pycache__/console.cpython-310.pyc
--rw-r--r--   0        0        0      861 2023-03-09 20:43:08.721719 fluidsimfoam-0.0.2/src/fluidsimfoam/util/console.py
--rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 fluidsimfoam-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1521 2023-03-02 21:01:46.291446 fluidsimfoam-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3951 2023-05-09 12:08:00.518116 fluidsimfoam-0.0.3/README.md
+-rw-r--r--   0        0        0     1429 2023-05-09 13:09:30.236813 fluidsimfoam-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1807 2023-05-09 13:05:24.334349 fluidsimfoam-0.0.3/src/fluidsimfoam/__init__.py
+-rw-r--r--   0        0        0     2195 2023-05-09 12:44:19.739747 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__init__.py
+-rw-r--r--   0        0        0     2527 2023-05-09 12:44:22.103389 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    15511 2023-05-09 12:46:11.206907 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/ast.cpython-310.pyc
+-rw-r--r--   0        0        0     2205 2023-05-09 12:43:04.211446 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/constant_files.cpython-310.pyc
+-rw-r--r--   0        0        0     6100 2023-05-08 19:53:29.031102 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/fields.cpython-310.pyc
+-rw-r--r--   0        0        0     2752 2023-05-08 19:53:29.031102 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes.cpython-310.pyc
+-rw-r--r--   0        0        0     1844 2023-05-05 07:20:02.628943 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes_helper.cpython-310.pyc
+-rw-r--r--   0        0        0     5356 2023-05-09 12:43:04.227444 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/generators.cpython-310.pyc
+-rw-r--r--   0        0        0    10473 2023-05-09 12:43:04.027476 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/parser.cpython-310.pyc
+-rw-r--r--   0        0        0     1082 2023-05-03 21:01:43.908143 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/polymesh.cpython-310.pyc
+-rw-r--r--   0        0        0    15046 2023-05-09 12:44:45.871789 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/ast.py
+-rw-r--r--   0        0        0     1080 2023-04-23 15:48:42.099657 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/LICENSE
+-rw-r--r--   0        0        0    13459 2023-05-05 07:30:16.059861 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/__init__.py
+-rw-r--r--   0        0        0    14477 2023-05-05 07:30:22.743807 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2344 2023-05-05 07:26:24.618314 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/edges.cpython-310.pyc
+-rw-r--r--   0        0        0     3085 2023-05-05 07:26:24.622314 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/grading.cpython-310.pyc
+-rw-r--r--   0        0        0     1810 2023-04-24 21:00:31.761612 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/edges.py
+-rw-r--r--   0        0        0     3426 2023-04-24 20:58:16.942659 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/grading.py
+-rw-r--r--   0        0        0     2135 2023-05-09 12:38:35.919916 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/constant_files.py
+-rw-r--r--   0        0        0     5743 2023-05-08 19:04:20.598143 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/fields.py
+-rw-r--r--   0        0        0     2414 2023-05-08 19:04:20.598143 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/fv_schemes.py
+-rw-r--r--   0        0        0     5070 2023-05-09 12:42:19.787198 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/generators.py
+-rw-r--r--   0        0        0     1918 2023-04-18 19:23:17.863337 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/grammar.lark
+-rw-r--r--   0        0        0     2335 2023-04-18 19:23:17.863337 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/grammar_advanced.lark
+-rw-r--r--   0        0        0     9522 2023-05-09 12:42:41.039310 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/parser.py
+-rw-r--r--   0        0        0      973 2023-05-03 19:26:40.332634 fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/polymesh.py
+-rw-r--r--   0        0        0     1399 2023-05-09 12:54:58.927322 fluidsimfoam-0.0.3/src/fluidsimfoam/info.py
+-rw-r--r--   0        0        0      124 2023-05-09 13:01:28.476575 fluidsimfoam-0.0.3/src/fluidsimfoam/init_fields.py
+-rw-r--r--   0        0        0      747 2023-05-09 13:00:38.420124 fluidsimfoam-0.0.3/src/fluidsimfoam/log.py
+-rw-r--r--   0        0        0      334 2023-05-09 12:56:28.245852 fluidsimfoam-0.0.3/src/fluidsimfoam/make.py
+-rw-r--r--   0        0        0     1185 2023-05-09 12:57:19.118180 fluidsimfoam-0.0.3/src/fluidsimfoam/next_fluidsim_core.py
+-rw-r--r--   0        0        0     1321 2023-05-09 12:57:49.645576 fluidsimfoam-0.0.3/src/fluidsimfoam/operators.py
+-rw-r--r--   0        0        0      137 2023-05-09 12:48:51.690704 fluidsimfoam-0.0.3/src/fluidsimfoam/output/__init__.py
+-rw-r--r--   0        0        0      314 2023-05-09 12:51:06.198419 fluidsimfoam-0.0.3/src/fluidsimfoam/output/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7626 2023-05-09 09:32:45.016908 fluidsimfoam-0.0.3/src/fluidsimfoam/output/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     9206 2023-05-09 09:29:43.622730 fluidsimfoam-0.0.3/src/fluidsimfoam/output/base.py
+-rw-r--r--   0        0        0     1303 2023-05-09 12:58:11.670255 fluidsimfoam-0.0.3/src/fluidsimfoam/params.py
+-rw-r--r--   0        0        0      573 2023-05-09 13:02:35.270502 fluidsimfoam-0.0.3/src/fluidsimfoam/resources/__init__.py
+-rw-r--r--   0        0        0      955 2023-05-09 13:02:39.537858 fluidsimfoam-0.0.3/src/fluidsimfoam/resources/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2765 2023-05-09 13:04:52.906067 fluidsimfoam-0.0.3/src/fluidsimfoam/solvers/__init__.py
+-rw-r--r--   0        0        0     2620 2023-05-09 13:05:27.378825 fluidsimfoam-0.0.3/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1779 2023-05-09 12:51:06.182422 fluidsimfoam-0.0.3/src/fluidsimfoam/solvers/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     1857 2023-05-09 12:49:41.227234 fluidsimfoam-0.0.3/src/fluidsimfoam/solvers/base.py
+-rw-r--r--   0        0        0      714 2023-05-09 12:58:59.894982 fluidsimfoam-0.0.3/src/fluidsimfoam/tasks.py
+-rw-r--r--   0        0        0       76 2023-05-09 12:51:03.050894 fluidsimfoam-0.0.3/src/fluidsimfoam/util/__init__.py
+-rw-r--r--   0        0        0      238 2023-05-09 12:51:06.202419 fluidsimfoam-0.0.3/src/fluidsimfoam/util/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1145 2023-03-09 20:43:42.785643 fluidsimfoam-0.0.3/src/fluidsimfoam/util/__pycache__/console.cpython-310.pyc
+-rw-r--r--   0        0        0      861 2023-03-09 20:43:08.721719 fluidsimfoam-0.0.3/src/fluidsimfoam/util/console.py
+-rw-r--r--   0        0        0     4826 1970-01-01 00:00:00.000000 fluidsimfoam-0.0.3/PKG-INFO
```

### Comparing `fluidsimfoam-0.0.2/LICENSE` & `fluidsimfoam-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.2/pyproject.toml` & `fluidsimfoam-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fluidsimfoam"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python framework for OpenFOAM"
 authors = ["pierre.augier <pierre.augier@univ-grenoble-alpes.fr>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -18,14 +18,15 @@
 rich = "^13.3.3"
 invoke = "^2.0.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.1"
 fluidsimfoam-tgv = { path = "./doc/examples/fluidsimfoam-tgv/", develop = true }
 fluidsimfoam-cbox = { path = "./doc/examples/fluidsimfoam-cbox/", develop = true }
+fluidsimfoam-sed = { path = "./doc/examples/fluidsimfoam-sed/", develop = true }
 pytest-mock = "^3.10.0"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/__init__.py` & `fluidsimfoam-0.0.3/src/fluidsimfoam/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 
 .. rubric:: Sub-packages
 
 .. autosummary::
    :toctree:
 
    foam_input_files
-   output
-   resources
    solvers
+   output
    util
+   resources
 
 .. rubric:: Modules
 
 .. autosummary::
    :toctree:
 
    info
-   init_fields
-   log
    make
-   next_fluidsim_core
+   init_fields
    operators
+   log
    tasks
+   next_fluidsim_core
 
 """
 import importlib.metadata
 
-from fluidsim_core.params import Parameters
+from fluidsimfoam.params import Parameters
 
 from .next_fluidsim_core import path_try_from_fluidsim_path
 
 __version__ = importlib.metadata.version(__package__ or __name__)
 __all__ = ["load", "load_simul", "load_params"]
 
 
@@ -65,15 +65,15 @@
     params.output.HAS_TO_SAVE = False
     params.path_run = path_dir
 
     return Simul(params)
 
 
 def load_params(path_dir="."):
-    """Load a :class:`fluidsim_core.params.Parameters` instance from `path_dir`.
+    """Load a :class:`fluidsim_core.params.Parameters` instance from ``path_dir``
 
     Parameters
     ----------
     path_dir : str or path-like
         Path to a simulation directory.
 
     Returns
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/__pycache__/__init__.cpython-310.pyc` & `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Apr 26 14:37:40 2023 UTC, .py size: 1396 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,158 @@
-00000000: 6f0d 0d0a 0000 0000 3437 4964 7405 0000  o.......47Idt...
+00000000: 6f0d 0d0a 0000 0000 2340 5a64 9308 0000  o.......#@Zd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0011 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
+00000020: 0011 0000 0040 0000 0073 ca00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
-00000040: 6d04 5a04 6d05 5a05 0100 6401 6403 6c06  m.Z.m.Z...d.d.l.
-00000050: 6d07 5a07 6d08 5a08 0100 6700 6404 a201  m.Z.m.Z...g.d...
-00000060: 5a09 6405 5a0a 650a 6401 6406 8502 1900  Z.d.Z.e.d.d.....
-00000070: 5a0a 650b 6407 6408 6409 640a 640b 640c  Z.e.d.d.d.d.d.d.
-00000080: 640d 640e 6409 640f 6410 6411 6412 6410  d.d.d.d.d.d.d.d.
-00000090: 6413 6414 8d0f 5a0c 6415 5300 2916 7a6c  d.d...Z.d.S.).zl
-000000a0: 4f70 656e 464f 414d 2069 6e70 7574 2066  OpenFOAM input f
-000000b0: 696c 6573 0a0a 2e2e 2061 7574 6f73 756d  iles.... autosum
-000000c0: 6d61 7279 3a3a 0a20 2020 3a74 6f63 7472  mary::.   :toctr
-000000d0: 6565 3a0a 0a20 2020 2062 6c6f 636b 6d65  ee:..    blockme
-000000e0: 7368 6865 6c70 6572 0a20 2020 2061 7374  shhelper.    ast
-000000f0: 0a20 2020 2067 656e 6572 6174 6f72 730a  .    generators.
-00000100: 2020 2020 7061 7273 6572 0a0a e901 0000      parser......
-00000110: 0029 04da 0444 6963 74da 0d46 6f61 6d49  .)...Dict..FoamI
-00000120: 6e70 7574 4669 6c65 da04 4c69 7374 da05  nputFile..List..
-00000130: 5661 6c75 6529 02da 0464 756d 70da 0570  Value)...dump..p
-00000140: 6172 7365 2907 7207 0000 0072 0600 0000  arse).r....r....
-00000150: 7203 0000 00da 0e44 4546 4155 4c54 5f48  r......DEFAULT_H
-00000160: 4541 4445 5272 0200 0000 7204 0000 0072  EADERr....r....r
-00000170: 0500 0000 6131 0200 000a 2f2a 2d2d 2d2d  ....a1..../*----
-00000180: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2a2d 2043  ------------*- C
-000001a0: 2b2b 202d 2a2d 2d2d 2d2d 2d2d 2d2d 2d2d  ++ -*-----------
-000001b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000001c0: 2d2d 2d2d 2d2d 2d2a 5c0a 7c20 3d3d 3d3d  -------*\.| ====
-000001d0: 3d3d 3d3d 3d20 2020 2020 2020 2020 2020  =====           
-000001e0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-000001f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000210: 2020 2020 2020 2020 7c0a 7c20 5c5c 2020          |.| \\  
-00000220: 2020 2020 2f20 2046 2069 656c 6420 2020      /  F ield   
-00000230: 2020 2020 2020 7c20 4f70 656e 464f 414d        | OpenFOAM
-00000240: 3a20 5468 6520 4f70 656e 2053 6f75 7263  : The Open Sourc
-00000250: 6520 4346 4420 546f 6f6c 626f 7820 2020  e CFD Toolbox   
-00000260: 2020 2020 2020 2020 7c0a 7c20 205c 5c20          |.|  \\ 
-00000270: 2020 202f 2020 204f 2070 6572 6174 696f     /   O peratio
-00000280: 6e20 2020 2020 7c20 5665 7273 696f 6e3a  n     | Version:
-00000290: 2020 7632 3230 3620 2020 2020 2020 2020    v2206         
-000002a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002b0: 2020 2020 2020 2020 7c0a 7c20 2020 5c5c          |.|   \\
-000002c0: 2020 2f20 2020 2041 206e 6420 2020 2020    /    A nd     
-000002d0: 2020 2020 2020 7c20 5765 6273 6974 653a        | Website:
-000002e0: 2020 7777 772e 6f70 656e 666f 616d 2e63    www.openfoam.c
-000002f0: 6f6d 2020 2020 2020 2020 2020 2020 2020  om              
-00000300: 2020 2020 2020 2020 7c0a 7c20 2020 205c          |.|    \
-00000310: 5c2f 2020 2020 204d 2061 6e69 7075 6c61  \/     M anipula
-00000320: 7469 6f6e 2020 7c20 2020 2020 2020 2020  tion  |         
-00000330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000350: 2020 2020 2020 2020 7c0a 5c2a 2d2d 2d2d          |.\*----
-00000360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000003a0: 2d2d 2d2d 2d2d 2d2a 2f0a e9ff ffff ff5a  -------*/......Z
-000003b0: 0769 636f 466f 616d da09 7374 6172 7454  .icoFoam..startT
-000003c0: 696d 65e9 0000 0000 da07 656e 6454 696d  ime.......endTim
-000003d0: 6567 0000 0000 0000 e03f 677b 14ae 47e1  eg.......?g{..G.
-000003e0: 7a74 3f5a 0874 696d 6553 7465 70e9 1400  zt?Z.timeStep...
-000003f0: 0000 da05 6173 6369 69e9 0600 0000 da03  ....ascii.......
-00000400: 6f66 66da 0767 656e 6572 616c da04 7472  off..general..tr
-00000410: 7565 290f da0b 6170 706c 6963 6174 696f  ue)...applicatio
-00000420: 6e5a 0973 7461 7274 4672 6f6d 720a 0000  nZ.startFromr...
-00000430: 005a 0673 746f 7041 7472 0c00 0000 5a06  .Z.stopAtr....Z.
-00000440: 6465 6c74 6154 5a0c 7772 6974 6543 6f6e  deltaTZ.writeCon
-00000450: 7472 6f6c 5a0d 7772 6974 6549 6e74 6572  trolZ.writeInter
-00000460: 7661 6c5a 0a70 7572 6765 5772 6974 655a  valZ.purgeWriteZ
-00000470: 0b77 7269 7465 466f 726d 6174 5a0e 7772  .writeFormatZ.wr
-00000480: 6974 6550 7265 6369 7369 6f6e 5a10 7772  itePrecisionZ.wr
-00000490: 6974 6543 6f6d 7072 6573 7369 6f6e 5a0a  iteCompressionZ.
-000004a0: 7469 6d65 466f 726d 6174 5a0d 7469 6d65  timeFormatZ.time
-000004b0: 5072 6563 6973 696f 6e5a 1172 756e 5469  PrecisionZ.runTi
-000004c0: 6d65 4d6f 6469 6669 6162 6c65 4e29 0dda  meModifiableN)..
-000004d0: 075f 5f64 6f63 5f5f da03 6173 7472 0200  .__doc__..astr..
-000004e0: 0000 7203 0000 0072 0400 0000 7205 0000  ..r....r....r...
-000004f0: 00da 0670 6172 7365 7272 0600 0000 7207  ...parserr....r.
-00000500: 0000 00da 075f 5f61 6c6c 5f5f 7208 0000  .....__all__r...
-00000510: 00da 0464 6963 745a 1444 4546 4155 4c54  ...dictZ.DEFAULT
-00000520: 5f43 4f4e 5452 4f4c 5f44 4943 54a9 0072  _CONTROL_DICT..r
-00000530: 1900 0000 7219 0000 00fa 4b2f 686f 6d65  ....r.....K/home
-00000540: 2f70 6965 7272 652f 4465 762f 666c 7569  /pierre/Dev/flui
-00000550: 6473 696d 666f 616d 2f73 7263 2f66 6c75  dsimfoam/src/flu
-00000560: 6964 7369 6d66 6f61 6d2f 666f 616d 5f69  idsimfoam/foam_i
-00000570: 6e70 7574 5f66 696c 6573 2f5f 5f69 6e69  nput_files/__ini
-00000580: 745f 5f2e 7079 da08 3c6d 6f64 756c 653e  t__.py..<module>
-00000590: 0100 0000 732e 0000 0004 0018 0c10 0108  ....s...........
-000005a0: 0204 0a0c 0a02 0302 0102 0102 0102 0102  ................
-000005b0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-000005c0: 0102 0102 010a f1                        .......
+00000040: 0100 6403 6404 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
+00000050: 6d07 5a07 6d08 5a08 0100 6403 6405 6c09  m.Z.m.Z...d.d.l.
+00000060: 6d0a 5a0a 6d0b 5a0b 0100 6700 6406 a201  m.Z.m.Z...g.d...
+00000070: 5a0c 4700 6407 6408 8400 6408 6502 8303  Z.G.d.d...d.e...
+00000080: 5a0d 6409 5a0e 650e 6403 640a 8502 1900  Z.d.Z.e.d.d.....
+00000090: 5a0e 650f 640b 640c 6401 640d 640e 640f  Z.e.d.d.d.d.d.d.
+000000a0: 6410 6411 6401 6412 6413 6414 6415 6413  d.d.d.d.d.d.d.d.
+000000b0: 6416 6417 8d0f 5a10 6403 6418 6c11 6d12  d.d...Z.d.d.l.m.
+000000c0: 5a12 6d13 5a13 0100 6403 6419 6c14 6d15  Z.m.Z...d.d.l.m.
+000000d0: 5a15 0100 6403 641a 6c16 6d17 5a17 6d18  Z...d.d.l.m.Z.m.
+000000e0: 5a18 6d19 5a19 0100 6403 641b 6c1a 6d1b  Z.m.Z...d.d.l.m.
+000000f0: 5a1b 0100 641c 5300 291d 7af9 4f70 656e  Z...d.S.).z.Open
+00000100: 464f 414d 2069 6e70 7574 2066 696c 6573  FOAM input files
+00000110: 0a0a 2e2e 2072 7562 7269 633a 3a20 4153  .... rubric:: AS
+00000120: 5420 616e 6420 7061 7273 6572 0a0a 2e2e  T and parser....
+00000130: 2061 7574 6f73 756d 6d61 7279 3a3a 0a20   autosummary::. 
+00000140: 2020 3a74 6f63 7472 6565 3a0a 0a20 2020    :toctree:..   
+00000150: 2061 7374 0a20 2020 2067 656e 6572 6174   ast.    generat
+00000160: 6f72 730a 2020 2020 7061 7273 6572 0a0a  ors.    parser..
+00000170: 2e2e 2072 7562 7269 633a 3a20 4865 6c70  .. rubric:: Help
+00000180: 6572 2074 6f20 6372 6561 7465 2069 6e70  er to create inp
+00000190: 7574 2066 696c 6573 0a0a 2e2e 2061 7574  ut files.... aut
+000001a0: 6f73 756d 6d61 7279 3a3a 0a20 2020 3a74  osummary::.   :t
+000001b0: 6f63 7472 6565 3a0a 0a20 2020 2062 6c6f  octree:..    blo
+000001c0: 636b 6d65 7368 0a20 2020 2066 6965 6c64  ckmesh.    field
+000001d0: 730a 2020 2020 6676 5f73 6368 656d 6573  s.    fv_schemes
+000001e0: 0a20 2020 2063 6f6e 7374 616e 745f 6669  .    constant_fi
+000001f0: 6c65 730a 0ae9 0000 0000 2902 da03 4142  les.......)...AB
+00000200: 43da 0e61 6273 7472 6163 746d 6574 686f  C..abstractmetho
+00000210: 64e9 0100 0000 2904 da04 4469 6374 da0d  d.....)...Dict..
+00000220: 466f 616d 496e 7075 7446 696c 65da 044c  FoamInputFile..L
+00000230: 6973 74da 0556 616c 7565 2902 da04 6475  ist..Value)...du
+00000240: 6d70 da05 7061 7273 6529 0e72 0a00 0000  mp..parse).r....
+00000250: 7209 0000 0072 0600 0000 da0e 4445 4641  r....r......DEFA
+00000260: 554c 545f 4845 4144 4552 7205 0000 0072  ULT_HEADERr....r
+00000270: 0700 0000 7208 0000 00da 0d42 6c6f 636b  ....r......Block
+00000280: 4d65 7368 4469 6374 da0e 566f 6c53 6361  MeshDict..VolSca
+00000290: 6c61 7246 6965 6c64 da0e 566f 6c56 6563  larField..VolVec
+000002a0: 746f 7246 6965 6c64 da0f 4676 5363 6865  torField..FvSche
+000002b0: 6d65 7348 656c 7065 72da 0656 6572 7465  mesHelper..Verte
+000002c0: 78da 0f72 6561 645f 6669 656c 645f 6669  x..read_field_fi
+000002d0: 6c65 da0a 4669 6c65 4865 6c70 6572 6300  le..FileHelperc.
+000002e0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+000002f0: 0000 0040 0000 0073 2800 0000 6500 5a01  ...@...s(...e.Z.
+00000300: 6400 5a02 6401 5a03 6504 6402 6403 8400  d.Z.d.Z.e.d.d...
+00000310: 8301 5a05 6504 6404 6405 8400 8301 5a06  ..Z.e.d.d.....Z.
+00000320: 6406 5300 2907 7212 0000 007a 2341 6273  d.S.).r....z#Abs
+00000330: 7472 6163 7420 636c 6173 7320 666f 7220  tract class for 
+00000340: 2248 656c 7065 7222 206f 626a 6563 7473  "Helper" objects
+00000350: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000360: 0001 0000 0043 0000 00f3 0400 0000 6401  .....C........d.
+00000370: 5300 2902 7a1a 436f 6d70 6c65 7465 2074  S.).z.Complete t
+00000380: 6865 2070 6172 616d 7320 6f62 6a65 6374  he params object
+00000390: 4ea9 00a9 02da 0473 656c 66da 0670 6172  N......self..par
+000003a0: 616d 7372 1400 0000 7214 0000 00fa 4b2f  amsr....r.....K/
+000003b0: 686f 6d65 2f70 6965 7272 652f 4465 762f  home/pierre/Dev/
+000003c0: 666c 7569 6473 696d 666f 616d 2f73 7263  fluidsimfoam/src
+000003d0: 2f66 6c75 6964 7369 6d66 6f61 6d2f 666f  /fluidsimfoam/fo
+000003e0: 616d 5f69 6e70 7574 5f66 696c 6573 2f5f  am_input_files/_
+000003f0: 5f69 6e69 745f 5f2e 7079 da0f 636f 6d70  _init__.py..comp
+00000400: 6c65 7465 5f70 6172 616d 7331 0000 00f3  lete_params1....
+00000410: 0200 0000 0400 7a1a 4669 6c65 4865 6c70  ......z.FileHelp
+00000420: 6572 2e63 6f6d 706c 6574 655f 7061 7261  er.complete_para
+00000430: 6d73 6302 0000 0000 0000 0000 0000 0002  msc.............
+00000440: 0000 0001 0000 0043 0000 0072 1300 0000  .......C...r....
+00000450: 2902 7a24 4d61 6b65 2074 6865 2041 5354  ).z$Make the AST
+00000460: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
+00000470: 6f20 6120 6669 6c65 4e72 1400 0000 7215  o a fileNr....r.
+00000480: 0000 0072 1400 0000 7214 0000 0072 1800  ...r....r....r..
+00000490: 0000 da09 6d61 6b65 5f74 7265 6535 0000  ....make_tree5..
+000004a0: 0072 1a00 0000 7a14 4669 6c65 4865 6c70  .r....z.FileHelp
+000004b0: 6572 2e6d 616b 655f 7472 6565 4e29 07da  er.make_treeN)..
+000004c0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+000004d0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+000004e0: 655f 5fda 075f 5f64 6f63 5f5f 7203 0000  e__..__doc__r...
+000004f0: 0072 1900 0000 721b 0000 0072 1400 0000  .r....r....r....
+00000500: 7214 0000 0072 1400 0000 7218 0000 0072  r....r....r....r
+00000510: 1200 0000 2f00 0000 730c 0000 0008 0004  ..../...s.......
+00000520: 0102 010a 0102 030e 0172 1200 0000 6131  .........r....a1
+00000530: 0200 000a 2f2a 2d2d 2d2d 2d2d 2d2d 2d2d  ..../*----------
+00000540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000550: 2d2d 2d2d 2d2d 2a2d 2043 2b2b 202d 2a2d  ------*- C++ -*-
+00000560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000570: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000580: 2d2a 5c0a 7c20 3d3d 3d3d 3d3d 3d3d 3d20  -*\.| ========= 
+00000590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005a0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+000005b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005d0: 2020 7c0a 7c20 5c5c 2020 2020 2020 2f20    |.| \\      / 
+000005e0: 2046 2069 656c 6420 2020 2020 2020 2020   F ield         
+000005f0: 7c20 4f70 656e 464f 414d 3a20 5468 6520  | OpenFOAM: The 
+00000600: 4f70 656e 2053 6f75 7263 6520 4346 4420  Open Source CFD 
+00000610: 546f 6f6c 626f 7820 2020 2020 2020 2020  Toolbox         
+00000620: 2020 7c0a 7c20 205c 5c20 2020 202f 2020    |.|  \\    /  
+00000630: 204f 2070 6572 6174 696f 6e20 2020 2020   O peration     
+00000640: 7c20 5665 7273 696f 6e3a 2020 7632 3230  | Version:  v220
+00000650: 3620 2020 2020 2020 2020 2020 2020 2020  6               
+00000660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000670: 2020 7c0a 7c20 2020 5c5c 2020 2f20 2020    |.|   \\  /   
+00000680: 2041 206e 6420 2020 2020 2020 2020 2020   A nd           
+00000690: 7c20 5765 6273 6974 653a 2020 7777 772e  | Website:  www.
+000006a0: 6f70 656e 666f 616d 2e63 6f6d 2020 2020  openfoam.com    
+000006b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006c0: 2020 7c0a 7c20 2020 205c 5c2f 2020 2020    |.|    \\/    
+000006d0: 204d 2061 6e69 7075 6c61 7469 6f6e 2020   M anipulation  
+000006e0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+000006f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000710: 2020 7c0a 5c2a 2d2d 2d2d 2d2d 2d2d 2d2d    |.\*----------
+00000720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000760: 2d2a 2f0a e9ff ffff ff5a 0769 636f 466f  -*/......Z.icoFo
+00000770: 616d da09 7374 6172 7454 696d 65da 0765  am..startTime..e
+00000780: 6e64 5469 6d65 6700 0000 0000 00e0 3f67  ndTimeg.......?g
+00000790: 7b14 ae47 e17a 743f 5a08 7469 6d65 5374  {..G.zt?Z.timeSt
+000007a0: 6570 e914 0000 00da 0561 7363 6969 e906  ep.......ascii..
+000007b0: 0000 00da 036f 6666 da07 6765 6e65 7261  .....off..genera
+000007c0: 6cda 0474 7275 6529 0fda 0b61 7070 6c69  l..true)...appli
+000007d0: 6361 7469 6f6e 5a09 7374 6172 7446 726f  cationZ.startFro
+000007e0: 6d72 2100 0000 5a06 7374 6f70 4174 7222  mr!...Z.stopAtr"
+000007f0: 0000 005a 0664 656c 7461 545a 0c77 7269  ...Z.deltaTZ.wri
+00000800: 7465 436f 6e74 726f 6c5a 0d77 7269 7465  teControlZ.write
+00000810: 496e 7465 7276 616c 5a0a 7075 7267 6557  IntervalZ.purgeW
+00000820: 7269 7465 5a0b 7772 6974 6546 6f72 6d61  riteZ.writeForma
+00000830: 745a 0e77 7269 7465 5072 6563 6973 696f  tZ.writePrecisio
+00000840: 6e5a 1077 7269 7465 436f 6d70 7265 7373  nZ.writeCompress
+00000850: 696f 6e5a 0a74 696d 6546 6f72 6d61 745a  ionZ.timeFormatZ
+00000860: 0d74 696d 6550 7265 6369 7369 6f6e 5a11  .timePrecisionZ.
+00000870: 7275 6e54 696d 654d 6f64 6966 6961 626c  runTimeModifiabl
+00000880: 6529 0272 0c00 0000 7210 0000 0029 01da  e).r....r....)..
+00000890: 1243 6f6e 7374 616e 7446 696c 6548 656c  .ConstantFileHel
+000008a0: 7065 7229 0372 0d00 0000 720e 0000 0072  per).r....r....r
+000008b0: 1100 0000 2901 720f 0000 004e 291c 721f  ....).r....N).r.
+000008c0: 0000 00da 0361 6263 7202 0000 0072 0300  .....abcr....r..
+000008d0: 0000 da03 6173 7472 0500 0000 7206 0000  ....astr....r...
+000008e0: 0072 0700 0000 7208 0000 00da 0670 6172  .r....r......par
+000008f0: 7365 7272 0900 0000 720a 0000 00da 075f  serr....r......_
+00000900: 5f61 6c6c 5f5f 7212 0000 0072 0b00 0000  _all__r....r....
+00000910: da04 6469 6374 5a14 4445 4641 554c 545f  ..dictZ.DEFAULT_
+00000920: 434f 4e54 524f 4c5f 4449 4354 5a09 626c  CONTROL_DICTZ.bl
+00000930: 6f63 6b6d 6573 6872 0c00 0000 7210 0000  ockmeshr....r...
+00000940: 005a 0e63 6f6e 7374 616e 745f 6669 6c65  .Z.constant_file
+00000950: 7372 2a00 0000 da06 6669 656c 6473 720d  sr*.....fieldsr.
+00000960: 0000 0072 0e00 0000 7211 0000 005a 0a66  ...r....r....Z.f
+00000970: 765f 7363 6865 6d65 7372 0f00 0000 7214  v_schemesr....r.
+00000980: 0000 0072 1400 0000 7214 0000 0072 1800  ...r....r....r..
+00000990: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000009a0: 733a 0000 0004 0010 1718 0210 0108 0210  s:..............
+000009b0: 1204 0b0c 0a02 0302 0102 0102 0102 0102  ................
+000009c0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+000009d0: 0102 0102 0106 f110 120c 0114 0110 01    ...............
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/__pycache__/ast.cpython-310.pyc` & `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/ast.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 21 00:50:23 2023 UTC, .py size: 11079 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,783 +1,970 @@
-00000000: 6f0d 0d0a 0000 0000 cfdd 4164 472b 0000  o.........AdG+..
+00000000: 6f0d 0d0a 0000 0000 3d40 5a64 c63a 0000  o.......=@Zd.:..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 3c01 0000 6400  .....@...s<...d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c05 6d06 5a06 0100 6700 6405 a201  d.l.m.Z...g.d...
-00000060: 5a07 6406 6407 8400 5a08 6408 6409 8400  Z.d.d...Z.d.d...
-00000070: 5a09 4700 640a 640b 8400 640b 8302 5a0a  Z.G.d.d...d...Z.
-00000080: 4700 640c 640d 8400 640d 650a 8303 5a0b  G.d.d...d.e...Z.
-00000090: 6502 4700 640e 640f 8400 640f 8302 8301  e.G.d.d...d.....
-000000a0: 5a0c 4700 6410 6411 8400 6411 650c 8303  Z.G.d.d...d.e...
-000000b0: 5a0d 6502 4700 6412 6413 8400 6413 650a  Z.e.G.d.d...d.e.
-000000c0: 8303 8301 5a0e 4700 6414 6415 8400 6415  ....Z.G.d.d...d.
-000000d0: 650f 650a 8304 5a10 4700 6416 6417 8400  e.e...Z.G.d.d...
-000000e0: 6417 6511 650a 8304 5a12 4700 6418 6419  d.e.e...Z.G.d.d.
-000000f0: 8400 6419 650f 650a 8304 5a13 4700 641a  ..d.e.e...Z.G.d.
-00000100: 641b 8400 641b 6512 8303 5a14 641c 641d  d...d.e...Z.d.d.
-00000110: 8400 5a15 641e 4400 5d0c 5a16 6517 6514  ..Z.d.D.].Z.e.e.
-00000120: 6506 6516 8301 6515 6516 8301 8303 0100  e.e...e.e.......
-00000130: 7175 4700 641f 6420 8400 6420 650a 8303  quG.d.d ..d e...
-00000140: 5a18 6502 4700 6421 6422 8400 6422 650a  Z.e.G.d!d"..d"e.
-00000150: 8303 8301 5a19 4700 6423 6424 8400 6424  ....Z.G.d#d$..d$
-00000160: 650a 8303 5a1a 6401 5300 2925 e900 0000  e...Z.d.S.)%....
-00000170: 004e 2901 da09 6461 7461 636c 6173 7329  .N)...dataclass)
-00000180: 01da 0664 6564 656e 7429 01da 0a75 6e64  ...dedent)...und
-00000190: 6572 7363 6f72 6529 075a 026b 67da 016d  erscore).Z.kg..m
-000001a0: da01 73da 014b 5a04 6b6d 6f6c da01 41da  ..s..KZ.kmol..A.
-000001b0: 0263 6463 0100 0000 0000 0000 0000 0000  .cdc............
-000001c0: 0900 0000 0800 0000 4300 0000 73d6 0000  ........C...s...
-000001d0: 0064 0167 0164 0214 007d 0164 037d 027c  .d.g.d...}.d.}.|
-000001e0: 0072 697a 0a74 00a0 0164 047c 00a1 02a0  .riz.t...d.|....
-000001f0: 02a1 007d 0357 006e 0f04 0074 0379 2201  ...}.W.n...t.y".
-00000200: 0001 0001 007c 007d 0464 057d 0064 067d  .....|.}.d.}.d.}
-00000210: 0559 006e 1977 007c 007c 0319 007d 057c  .Y.n.w.|.|...}.|
-00000220: 0564 0776 0073 2d4a 0082 017c 0064 007c  .d.v.s-J...|.d.|
-00000230: 0385 0219 007d 047c 007c 0364 0317 0064  .....}.|.|.d...d
-00000240: 0085 0219 007d 0064 087c 0476 0072 4b7c  .....}.d.|.v.rK|
-00000250: 04a0 0464 08a1 015c 027d 067d 0774 057c  ...d...\.}.}.t.|
-00000260: 0783 017d 076e 057c 0464 0302 027d 067d  ...}.n.|.d...}.}
-00000270: 077c 0664 096b 0372 5f74 06a0 077c 06a1  .|.d.k.r_t...|..
-00000280: 017d 087c 027c 0714 007c 017c 083c 007c  .}.|.|...|.|.<.|
-00000290: 0564 066b 0272 6564 036e 0164 0a7d 027c  .d.k.red.n.d.}.|
-000002a0: 0073 097c 0153 0029 0b4e 7201 0000 00e9  .s.|.S.).Nr.....
-000002b0: 0700 0000 e901 0000 007a 045b 2f2e 5dda  .........z.[/.].
-000002c0: 00da 012e 7a02 2f2e fa01 5eda 0131 e9ff  ....z./...^..1..
-000002d0: ffff ff29 08da 0272 65da 0673 6561 7263  ...)...re..searc
-000002e0: 68da 0573 7461 7274 da0e 4174 7472 6962  h..start..Attrib
-000002f0: 7574 6545 7272 6f72 da05 7370 6c69 74da  uteError..split.
-00000300: 0369 6e74 da07 7379 6d62 6f6c 73da 0569  .int..symbols..i
-00000310: 6e64 6578 2909 da05 756e 6974 73da 0672  ndex)...units..r
-00000320: 6573 756c 74da 0473 6967 6e72 1800 0000  esult..signr....
-00000330: 5a08 756e 6974 5f61 6c6c 5a09 6e65 7874  Z.unit_allZ.next
-00000340: 5f6f 7065 72da 0975 6e69 745f 6e61 6d65  _oper..unit_name
-00000350: 5a0a 756e 6974 5f76 616c 7565 5a0a 756e  Z.unit_valueZ.un
-00000360: 6974 5f69 6e64 6578 a900 721d 0000 00fa  it_index..r.....
-00000370: 462f 686f 6d65 2f70 6965 7272 652f 4465  F/home/pierre/De
-00000380: 762f 666c 7569 6473 696d 666f 616d 2f73  v/fluidsimfoam/s
-00000390: 7263 2f66 6c75 6964 7369 6d66 6f61 6d2f  rc/fluidsimfoam/
-000003a0: 666f 616d 5f69 6e70 7574 5f66 696c 6573  foam_input_files
-000003b0: 2f61 7374 2e70 79da 0e73 7472 3266 6f61  /ast.py..str2foa
-000003c0: 6d5f 756e 6974 730a 0000 0073 3000 0000  m_units....s0...
-000003d0: 0a01 0401 0401 0201 1401 0c01 0401 0401  ................
-000003e0: 0801 02fd 0805 0c01 0c01 1001 0801 0e01  ................
-000003f0: 0a01 0a02 0801 0a01 0c01 1001 04ec 0415  ................
-00000400: 721f 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00000410: 0000 0500 0000 0800 0000 4300 0000 73a8  ..........C...s.
-00000420: 0000 0067 007d 0174 0074 017c 0083 0244  ...g.}.t.t.|...D
-00000430: 005d 2f5c 027d 027d 037c 0364 016b 0272  .]/\.}.}.|.d.k.r
-00000440: 1071 077c 0364 016b 0472 1664 026e 0164  .q.|.d.k.r.d.n.d
-00000450: 037d 0474 027c 0383 0164 046b 0272 287c  .}.t.|...d.k.r(|
-00000460: 01a0 037c 049b 007c 029b 009d 02a1 0101  ...|...|........
-00000470: 0071 077c 01a0 037c 049b 007c 029b 0064  .q.|...|...|...d
-00000480: 0574 027c 0383 019b 009d 04a1 0101 0071  .t.|...........q
-00000490: 0764 06a0 047c 01a1 017d 017c 01a0 0564  .d...|...}.|...d
-000004a0: 02a1 0172 497c 0164 0464 0085 0219 007d  ...rI|.d.d.....}
-000004b0: 017c 0153 007c 01a0 0564 03a1 0172 5264  .|.S.|...d...rRd
-000004c0: 077c 0117 007d 017c 0153 0029 084e 7201  .|...}.|.S.).Nr.
-000004d0: 0000 0072 0d00 0000 fa01 2f72 0b00 0000  ...r....../r....
-000004e0: 720e 0000 0072 0c00 0000 720f 0000 0029  r....r....r....)
-000004f0: 06da 037a 6970 7217 0000 00da 0361 6273  ...zipr......abs
-00000500: da06 6170 7065 6e64 da04 6a6f 696e da0a  ..append..join..
-00000510: 7374 6172 7473 7769 7468 2905 da0a 666f  startswith)...fo
-00000520: 616d 5f75 6e69 7473 721a 0000 00da 0673  am_unitsr......s
-00000530: 796d 626f 6cda 0865 7870 6f6e 656e 74da  ymbol..exponent.
-00000540: 086f 7065 7261 746f 7272 1d00 0000 721d  .operatorr....r.
-00000550: 0000 0072 1e00 0000 da0e 666f 616d 5f75  ...r......foam_u
-00000560: 6e69 7473 3273 7472 2500 0000 731e 0000  nits2str%...s...
-00000570: 0004 0112 0108 0102 0110 010c 0114 011e  ................
-00000580: 020a 010a 010c 0104 030a fe08 0104 0172  ...............r
-00000590: 2a00 0000 6300 0000 0000 0000 0000 0000  *...c...........
-000005a0: 0000 0000 0002 0000 0040 0000 0073 1400  .........@...s..
-000005b0: 0000 6500 5a01 6400 5a02 6401 6402 8400  ..e.Z.d.Z.d.d...
-000005c0: 5a03 6403 5300 2904 da04 4e6f 6465 6302  Z.d.S.)...Nodec.
-000005d0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-000005e0: 0000 0043 0000 0073 2000 0000 7400 7c01  ...C...s ...t.|.
-000005f0: 8301 7400 7c00 8301 7500 720e 7c00 6a01  ..t.|...u.r.|.j.
-00000600: 7c01 6a01 6b02 5300 6401 5300 2902 4e46  |.j.k.S.d.S.).NF
-00000610: 2902 da04 7479 7065 da08 5f5f 6469 6374  )...type..__dict
-00000620: 5f5f 2902 da04 7365 6c66 da05 6f74 6865  __)...self..othe
-00000630: 7272 1d00 0000 721d 0000 0072 1e00 0000  rr....r....r....
-00000640: da06 5f5f 6571 5f5f 3800 0000 7306 0000  ..__eq__8...s...
-00000650: 0010 010c 0104 017a 0b4e 6f64 652e 5f5f  .......z.Node.__
-00000660: 6571 5f5f 4e29 04da 085f 5f6e 616d 655f  eq__N)...__name_
-00000670: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000680: 5f71 7561 6c6e 616d 655f 5f72 3000 0000  _qualname__r0...
-00000690: 721d 0000 0072 1d00 0000 721d 0000 0072  r....r....r....r
-000006a0: 1e00 0000 722b 0000 0037 0000 0073 0400  ....r+...7...s..
-000006b0: 0000 0800 0c01 722b 0000 0063 0000 0000  ......r+...c....
-000006c0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-000006d0: 4000 0000 7326 0000 0065 005a 0164 005a  @...s&...e.Z.d.Z
-000006e0: 0264 0864 0264 0384 015a 0364 0464 0584  .d.d.d...Z.d.d..
-000006f0: 005a 0464 0664 0784 005a 0564 0153 0029  .Z.d.d...Z.d.S.)
-00000700: 09da 0d46 6f61 6d49 6e70 7574 4669 6c65  ...FoamInputFile
-00000710: 4e63 0500 0000 0000 0000 0000 0000 0500  Nc..............
-00000720: 0000 0200 0000 4300 0000 731c 0000 007c  ......C...s....|
-00000730: 017c 005f 007c 027c 005f 017c 037c 005f  .|._.|.|._.|.|._
-00000740: 027c 047c 005f 0364 0053 00a9 014e 2904  .|.|._.d.S...N).
-00000750: da04 696e 666f da08 6368 696c 6472 656e  ..info..children
-00000760: da06 6865 6164 6572 da08 636f 6d6d 656e  ..header..commen
-00000770: 7473 2905 722e 0000 0072 3600 0000 7237  ts).r....r6...r7
-00000780: 0000 0072 3800 0000 7239 0000 0072 1d00  ...r8...r9...r..
-00000790: 0000 721d 0000 0072 1e00 0000 da08 5f5f  ..r....r......__
-000007a0: 696e 6974 5f5f 3f00 0000 7308 0000 0006  init__?...s.....
-000007b0: 0106 0106 010a 017a 1646 6f61 6d49 6e70  .......z.FoamInp
-000007c0: 7574 4669 6c65 2e5f 5f69 6e69 745f 5f63  utFile.__init__c
-000007d0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000007e0: 0500 0000 4300 0000 7342 0000 0064 0167  ....C...sB...d.g
-000007f0: 017d 017c 006a 0064 0075 0172 127c 01a0  .}.|.j.d.u.r.|..
-00000800: 0164 027c 006a 009b 0064 039d 03a1 0101  .d.|.j...d......
-00000810: 007c 01a0 0164 047c 006a 029b 0064 059d  .|...d.|.j...d..
-00000820: 03a1 0101 0064 06a0 037c 01a1 0153 0029  .....d...|...S.)
-00000830: 074e 7a0b 496e 7075 7446 696c 6528 0a7a  .Nz.InputFile(.z
-00000840: 0569 6e66 6f3d 7a02 2c0a 7a09 6368 696c  .info=z.,.z.chil
-00000850: 6472 656e 3d7a 020a 2972 0c00 0000 2904  dren=z..)r....).
-00000860: 7236 0000 0072 2300 0000 7237 0000 0072  r6...r#...r7...r
-00000870: 2400 0000 2902 722e 0000 00da 0374 6d70  $...).r......tmp
-00000880: 721d 0000 0072 1d00 0000 721e 0000 00da  r....r....r.....
-00000890: 085f 5f72 6570 725f 5f45 0000 0073 0a00  .__repr__E...s..
-000008a0: 0000 0601 0a01 1401 1401 0a01 7a16 466f  ............z.Fo
-000008b0: 616d 496e 7075 7446 696c 652e 5f5f 7265  amInputFile.__re
-000008c0: 7072 5f5f 6301 0000 0000 0000 0000 0000  pr__c...........
-000008d0: 0009 0000 0008 0000 0043 0000 0073 6a01  .........C...sj.
-000008e0: 0000 6700 7d01 7c00 6a00 6400 7501 7236  ..g.}.|.j.d.u.r6
-000008f0: 6401 6701 7d02 7c00 6a00 a001 a100 4400  d.g.}.|.j.....D.
-00000900: 5d19 5c02 7d03 7d04 6402 7402 7c03 8301  ].\.}.}.d.t.|...
-00000910: 1800 6403 1400 7d05 7c02 a003 6404 7c03  ..d...}.|...d.|.
-00000920: 9b00 7c05 9b00 7c04 9b00 6405 9d05 a101  ..|...|...d.....
-00000930: 0100 710f 7c02 a003 6406 a101 0100 7c01  ..q.|...d.....|.
-00000940: a003 6407 a004 7c02 a101 a101 0100 7c00  ..d...|.......|.
-00000950: 6a05 a001 a100 4400 5d5c 5c02 7d03 7d04  j.....D.]\\.}.}.
-00000960: 7406 7c04 6408 8302 7256 7c04 a007 a100  t.|.d...rV|.....
-00000970: 7d06 7c03 6400 7500 7255 7408 7c04 7409  }.|.d.u.rUt.|.t.
-00000980: 8302 7255 7c06 6405 3700 7d06 6e21 7406  ..rU|.d.7.}.n!t.
-00000990: 7c04 6409 8302 7266 7c03 9b00 640a 7c04  |.d...rf|...d.|.
-000009a0: a00a a100 9b00 6405 9d04 7d06 6e11 7c04  ......d...}.n.|.
-000009b0: 6400 7500 726e 7c03 9b00 7d06 6e09 7c03  d.u.rn|...}.n.|.
-000009c0: 640b 9b04 640a 7c04 9b00 6405 9d04 7d06  d...d.|...d...}.
-000009d0: 7c00 6a0b 6400 7501 7292 7c03 7c00 6a0b  |.j.d.u.r.|.|.j.
-000009e0: 7600 7292 640c 7c00 6a0b 7c03 1900 a00c  v.r.d.|.j.|.....
-000009f0: 6407 640d a102 1700 7d07 7c07 6407 1700  d.d.....}.|.d...
-00000a00: 7c06 1700 7d06 7c01 a003 7c06 a101 0100  |...}.|...|.....
-00000a10: 713b 640e a004 7c01 a101 7d08 7c00 6a0d  q;d...|...}.|.j.
-00000a20: 6400 7501 72a9 7c00 6a0d 6407 1700 7c08  d.u.r.|.j.d...|.
-00000a30: 1700 7d08 7c08 640f 1900 6407 6b03 72b3  ..}.|.d...d.k.r.
-00000a40: 7c08 6407 3700 7d08 7c08 5300 2910 4e7a  |.d.7.}.|.S.).Nz
-00000a50: 0a46 6f61 6d46 696c 650a 7be9 0c00 0000  .FoamFile.{.....
-00000a60: fa01 20fa 0420 2020 20fa 013b da01 7dda  .. ..    ..;..}.
-00000a70: 010a da04 6475 6d70 da17 6475 6d70 5f77  ....dump..dump_w
-00000a80: 6974 686f 7574 5f61 7373 6967 6e6d 656e  ithout_assignmen
-00000a90: 74fa 0220 205a 0331 3473 7a03 2f2f 207a  t..  Z.14sz.// z
-00000aa0: 040a 2f2f 207a 020a 0a72 1000 0000 290e  ..// z...r....).
-00000ab0: 7236 0000 00da 0569 7465 6d73 da03 6c65  r6.....items..le
-00000ac0: 6e72 2300 0000 7224 0000 0072 3700 0000  nr#...r$...r7...
-00000ad0: da07 6861 7361 7474 7272 4300 0000 da0a  ..hasattrrC.....
-00000ae0: 6973 696e 7374 616e 6365 da04 4c69 7374  isinstance..List
-00000af0: 7244 0000 0072 3900 0000 da07 7265 706c  rD...r9.....repl
-00000b00: 6163 6572 3800 0000 2909 722e 0000 0072  acer8...).r....r
-00000b10: 3b00 0000 5a04 746d 7031 da03 6b65 79da  ;...Z.tmp1..key.
-00000b20: 046e 6f64 6572 0600 0000 5a09 636f 6465  .noder....Z.code
-00000b30: 5f6e 6f64 65da 0763 6f6d 6d65 6e74 721a  _node..commentr.
-00000b40: 0000 0072 1d00 0000 721d 0000 0072 1e00  ...r....r....r..
-00000b50: 0000 7243 0000 004c 0000 0073 3a00 0000  ..rC...L...s:...
-00000b60: 0401 0a01 0601 1201 1001 1c01 0a01 1001  ................
-00000b70: 1201 0a01 0801 1202 0801 0280 0a01 1601  ................
-00000b80: 0801 0801 1202 1401 1601 0c01 0c01 0a01  ................
-00000b90: 0a01 0e01 0c01 0801 0401 7a12 466f 616d  ..........z.Foam
-00000ba0: 496e 7075 7446 696c 652e 6475 6d70 a902  InputFile.dump..
-00000bb0: 4e4e a906 7231 0000 0072 3200 0000 7233  NN..r1...r2...r3
-00000bc0: 0000 0072 3a00 0000 723c 0000 0072 4300  ...r:...r<...rC.
-00000bd0: 0000 721d 0000 0072 1d00 0000 721d 0000  ..r....r....r...
-00000be0: 0072 1e00 0000 7234 0000 003e 0000 0073  .r....r4...>...s
-00000bf0: 0800 0000 0800 0a01 0806 0c07 7234 0000  ............r4..
-00000c00: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000c10: 0000 0300 0000 4000 0000 7328 0000 0065  ......@...s(...e
-00000c20: 005a 0164 005a 0255 0065 0365 0464 013c  .Z.d.Z.U.e.e.d.<
-00000c30: 0065 0565 0464 023c 0064 0764 0464 0584  .e.e.d.<.d.d.d..
-00000c40: 015a 0664 0653 0029 08da 0a41 7373 6967  .Z.d.S.)...Assig
-00000c50: 6e6d 656e 74da 046e 616d 65da 0576 616c  nment..name..val
-00000c60: 7565 7201 0000 0063 0200 0000 0000 0000  uer....c........
-00000c70: 0000 0000 0200 0000 0500 0000 4300 0000  ............C...
-00000c80: 7334 0000 0074 007c 006a 0164 0183 0272  s4...t.|.j.d...r
-00000c90: 0c7c 006a 01a0 027c 01a1 0153 007c 0164  .|.j...|...S.|.d
-00000ca0: 0214 007c 006a 039b 0064 037c 006a 019b  ...|.j...d.|.j..
-00000cb0: 0064 049d 0417 0053 00a9 054e 7243 0000  .d.....S...NrC..
-00000cc0: 0072 3e00 0000 7245 0000 0072 4000 0000  .r>...rE...r@...
-00000cd0: 2904 7248 0000 0072 5300 0000 7243 0000  ).rH...rS...rC..
-00000ce0: 0072 5200 0000 a902 722e 0000 00da 0669  .rR.....r......i
-00000cf0: 6e64 656e 7472 1d00 0000 721d 0000 0072  ndentr....r....r
-00000d00: 1e00 0000 7243 0000 0072 0000 0073 0600  ....rC...r...s..
-00000d10: 0000 0c01 0c01 1c02 7a0f 4173 7369 676e  ........z.Assign
-00000d20: 6d65 6e74 2e64 756d 704e a901 7201 0000  ment.dumpN..r...
-00000d30: 0029 0772 3100 0000 7232 0000 0072 3300  .).r1...r2...r3.
-00000d40: 0000 da03 7374 72da 0f5f 5f61 6e6e 6f74  ....str..__annot
-00000d50: 6174 696f 6e73 5f5f da06 6f62 6a65 6374  ations__..object
-00000d60: 7243 0000 0072 1d00 0000 721d 0000 0072  rC...r....r....r
-00000d70: 1d00 0000 721e 0000 0072 5100 0000 6d00  ....r....rQ...m.
-00000d80: 0000 7308 0000 000a 0008 0208 010e 0272  ..s............r
-00000d90: 5100 0000 6300 0000 0000 0000 0000 0000  Q...c...........
-00000da0: 0000 0000 0003 0000 0000 0000 0073 2600  .............s&.
-00000db0: 0000 6500 5a01 6400 5a02 8700 6601 6401  ..e.Z.d.Z...f.d.
-00000dc0: 6402 8408 5a03 6406 6404 6405 8401 5a04  d...Z.d.d.d...Z.
-00000dd0: 8700 0400 5a05 5300 2907 da12 5661 7269  ....Z.S.)...Vari
-00000de0: 6162 6c65 4173 7369 676e 6d65 6e74 6301  ableAssignmentc.
-00000df0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-00000e00: 0000 0003 0000 0073 0e00 0000 7400 8300  .......s....t...
-00000e10: a001 a100 7d01 7c01 5300 7235 0000 00a9  ....}.|.S.r5....
-00000e20: 02da 0573 7570 6572 723c 0000 0029 0272  ...superr<...).r
-00000e30: 2e00 0000 7206 0000 00a9 01da 095f 5f63  ....r........__c
-00000e40: 6c61 7373 5f5f 721d 0000 0072 1e00 0000  lass__r....r....
-00000e50: 723c 0000 007a 0000 0073 0400 0000 0a01  r<...z...s......
-00000e60: 0401 7a1b 5661 7269 6162 6c65 4173 7369  ..z.VariableAssi
-00000e70: 676e 6d65 6e74 2e5f 5f72 6570 725f 5f72  gnment.__repr__r
-00000e80: 0100 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00000e90: 0002 0000 0006 0000 0043 0000 0073 4a00  .........C...sJ.
-00000ea0: 0000 7400 7c00 6a01 6401 8302 7217 7c01  ..t.|.j.d...r.|.
-00000eb0: 6402 1400 7c00 6a02 9b00 6403 7c00 6a01  d...|.j...d.|.j.
-00000ec0: a003 7c01 a101 9b00 6404 9d04 1700 5300  ..|.....d.....S.
-00000ed0: 7c01 6402 1400 7c00 6a02 9b00 6403 7c00  |.d...|.j...d.|.
-00000ee0: 6a01 9b00 6404 9d04 1700 5300 7254 0000  j...d.....S.rT..
-00000ef0: 0029 0472 4800 0000 7253 0000 0072 5200  .).rH...rS...rR.
-00000f00: 0000 7243 0000 0072 5500 0000 721d 0000  ..rC...rU...r...
-00000f10: 0072 1d00 0000 721e 0000 0072 4300 0000  .r....r....rC...
-00000f20: 7e00 0000 7306 0000 000c 0122 011c 027a  ~...s......"...z
-00000f30: 1756 6172 6961 626c 6541 7373 6967 6e6d  .VariableAssignm
-00000f40: 656e 742e 6475 6d70 7257 0000 0029 0672  ent.dumprW...).r
-00000f50: 3100 0000 7232 0000 0072 3300 0000 723c  1...r2...r3...r<
-00000f60: 0000 0072 4300 0000 da0d 5f5f 636c 6173  ...rC.....__clas
-00000f70: 7363 656c 6c5f 5f72 1d00 0000 721d 0000  scell__r....r...
-00000f80: 0072 5e00 0000 721e 0000 0072 5b00 0000  .r^...r....r[...
-00000f90: 7900 0000 7306 0000 0008 000c 0112 0472  y...s..........r
-00000fa0: 5b00 0000 6300 0000 0000 0000 0000 0000  [...c...........
-00000fb0: 0000 0000 0003 0000 0040 0000 00f3 2800  .........@....(.
-00000fc0: 0000 6500 5a01 6400 5a02 6409 6402 6403  ..e.Z.d.Z.d.d.d.
-00000fd0: 8401 5a03 6404 6405 8400 5a04 640a 6407  ..Z.d.d...Z.d.d.
-00000fe0: 6408 8401 5a05 6401 5300 290b da05 5661  d...Z.d.S.)...Va
-00000ff0: 6c75 654e 6304 0000 0000 0000 0000 0000  lueNc...........
-00001000: 0004 0000 0004 0000 0043 0000 0073 2c00  .........C...s,.
-00001010: 0000 7c01 7c00 5f00 7c02 7c00 5f01 7402  ..|.|._.|.|._.t.
-00001020: 7c03 7403 7404 6602 8302 7211 7405 7c03  |.t.t.f...r.t.|.
-00001030: 8301 7d03 7c03 7c00 5f06 6400 5300 7235  ..}.|.|._.d.S.r5
-00001040: 0000 0029 0772 5300 0000 7252 0000 0072  ...).rS...rR...r
-00001050: 4900 0000 da04 6c69 7374 da05 7475 706c  I.....list..tupl
-00001060: 6572 2a00 0000 da09 6469 6d65 6e73 696f  er*.....dimensio
-00001070: 6e29 0472 2e00 0000 7253 0000 0072 5200  n).r....rS...rR.
-00001080: 0000 7265 0000 0072 1d00 0000 721d 0000  ..re...r....r...
-00001090: 0072 1e00 0000 723a 0000 0087 0000 0073  .r....r:.......s
-000010a0: 0a00 0000 0601 0601 0e01 0801 0a01 7a0e  ..............z.
-000010b0: 5661 6c75 652e 5f5f 696e 6974 5f5f 6301  Value.__init__c.
-000010c0: 0000 0000 0000 0000 0000 0001 0000 0007  ................
-000010d0: 0000 0043 0000 0073 9400 0000 7c00 6a00  ...C...s....|.j.
-000010e0: 6400 7501 7219 7c00 6a01 6400 7501 7219  d.u.r.|.j.d.u.r.
-000010f0: 6401 7c00 6a02 9b00 6402 7c00 6a01 9b00  d.|.j...d.|.j...
-00001100: 6403 7c00 6a00 9b00 6404 9d07 5300 7c00  d.|.j...d...S.|.
-00001110: 6a00 6400 7500 722e 7c00 6a01 6400 7501  j.d.u.r.|.j.d.u.
-00001120: 722e 6401 7c00 6a02 9b00 6402 7c00 6a01  r.d.|.j...d.|.j.
-00001130: 9b00 6404 9d05 5300 7c00 6a00 6400 7501  ..d...S.|.j.d.u.
-00001140: 7243 7c00 6a01 6400 7500 7243 6401 7c00  rC|.j.d.u.rCd.|.
-00001150: 6a02 9b00 6405 7c00 6a00 9b00 6404 9d05  j...d.|.j...d...
-00001160: 5300 6401 7c00 6a02 9b00 6406 9d03 5300  S.d.|.j...d...S.
-00001170: 2907 4e7a 0656 616c 7565 287a 082c 206e  ).Nz.Value(z., n
-00001180: 616d 653d 227a 0e22 2c20 6469 6d65 6e73  ame="z.", dimens
-00001190: 696f 6e3d 227a 0222 297a 0d2c 2064 696d  ion="z.")z., dim
-000011a0: 656e 7369 6f6e 3d22 fa01 2929 0372 6500  ension="..)).re.
-000011b0: 0000 7252 0000 0072 5300 0000 a901 722e  ..rR...rS.....r.
-000011c0: 0000 0072 1d00 0000 721d 0000 0072 1e00  ...r....r....r..
-000011d0: 0000 723c 0000 008e 0000 0073 0e00 0000  ..r<.......s....
-000011e0: 1401 1e01 1401 1601 1401 1601 0e02 7a0e  ..............z.
-000011f0: 5661 6c75 652e 5f5f 7265 7072 5f5f 7201  Value.__repr__r.
-00001200: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00001210: 0400 0000 0500 0000 4300 0000 73a8 0000  ........C...s...
-00001220: 007c 006a 0064 0075 0172 1474 017c 006a  .|.j.d.u.r.t.|.j
-00001230: 0083 017d 0264 01a0 0264 0264 0384 007c  ...}.d...d.d...|
-00001240: 0244 0083 01a1 017d 037c 006a 0064 0075  .D.....}.|.j.d.u
-00001250: 0172 2a7c 006a 0364 0075 0172 2a7c 006a  .r*|.j.d.u.r*|.j
-00001260: 039b 0064 047c 039b 0064 057c 006a 049b  ...d.|...d.|.j..
-00001270: 009d 0553 007c 006a 0064 0075 0072 3d7c  ...S.|.j.d.u.r=|
-00001280: 006a 0364 0075 0172 3d7c 006a 039b 0064  .j.d.u.r=|.j...d
-00001290: 017c 006a 049b 009d 0353 007c 006a 0064  .|.j.....S.|.j.d
-000012a0: 0075 0172 507c 006a 0364 0075 0072 5064  .u.rP|.j.d.u.rPd
-000012b0: 067c 039b 0064 057c 006a 049b 009d 0453  .|...d.|.j.....S
-000012c0: 007c 006a 049b 0053 0029 074e 723e 0000  .|.j...S.).Nr>..
-000012d0: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-000012e0: 0000 0300 0000 7300 0000 f318 0000 0081  ......s.........
-000012f0: 007c 005d 077d 0174 007c 0183 0156 0001  .|.].}.t.|...V..
-00001300: 0071 0264 0053 0072 3500 0000 a901 7258  .q.d.S.r5.....rX
-00001310: 0000 00a9 02da 022e 30da 066e 756d 6265  ........0..numbe
-00001320: 7272 1d00 0000 721d 0000 0072 1e00 0000  rr....r....r....
-00001330: da09 3c67 656e 6578 7072 3e9b 0000 00f3  ..<genexpr>.....
-00001340: 0400 0000 0280 1600 7a30 5661 6c75 652e  ........z0Value.
-00001350: 6475 6d70 5f77 6974 686f 7574 5f61 7373  dump_without_ass
-00001360: 6967 6e6d 656e 742e 3c6c 6f63 616c 733e  ignment.<locals>
-00001370: 2e3c 6765 6e65 7870 723e 7a02 205b 7a02  .<genexpr>z. [z.
-00001380: 5d20 fa01 5b29 0572 6500 0000 721f 0000  ] ..[).re...r...
-00001390: 0072 2400 0000 7252 0000 0072 5300 0000  .r$...rR...rS...
-000013a0: 2904 722e 0000 0072 5600 0000 5a0e 6469  ).r....rV...Z.di
-000013b0: 6d65 6e73 696f 6e5f 6c69 7374 5a10 6469  mension_listZ.di
-000013c0: 6d65 6e73 696f 6e5f 6475 6d70 6564 721d  mension_dumpedr.
-000013d0: 0000 0072 1d00 0000 721e 0000 0072 4400  ...r....r....rD.
-000013e0: 0000 9800 0000 7314 0000 000a 010a 0114  ......s.........
-000013f0: 0114 0118 0114 0112 0114 0112 0108 027a  ...............z
-00001400: 1d56 616c 7565 2e64 756d 705f 7769 7468  .Value.dump_with
-00001410: 6f75 745f 6173 7369 676e 6d65 6e74 724f  out_assignmentrO
-00001420: 0000 0072 5700 0000 2906 7231 0000 0072  ...rW...).r1...r
-00001430: 3200 0000 7233 0000 0072 3a00 0000 723c  2...r3...r:...r<
-00001440: 0000 0072 4400 0000 721d 0000 0072 1d00  ...rD...r....r..
-00001450: 0000 721d 0000 0072 1e00 0000 7262 0000  ..r....r....rb..
-00001460: 0085 0000 0073 0800 0000 0800 0a02 0807  .....s..........
-00001470: 0e0a 7262 0000 0063 0000 0000 0000 0000  ..rb...c........
-00001480: 0000 0000 0000 0000 0300 0000 0000 0000  ................
-00001490: 732e 0000 0065 005a 0164 005a 0287 0066  s....e.Z.d.Z...f
-000014a0: 0164 0164 0284 085a 0364 0364 0484 005a  .d.d...Z.d.d...Z
-000014b0: 0464 0864 0664 0784 015a 0587 0004 005a  .d.d.d...Z.....Z
-000014c0: 0653 0029 09da 0c44 696d 656e 7369 6f6e  .S.)...Dimension
-000014d0: 5365 7463 0200 0000 0000 0000 0000 0000  Setc............
-000014e0: 0200 0000 0300 0000 0300 0000 732a 0000  ............s*..
-000014f0: 0074 0064 0164 0284 007c 0144 0083 0183  .t.d.d...|.D....
-00001500: 0173 0d74 0164 0383 0182 0174 0283 00a0  .s.t.d.....t....
-00001510: 037c 01a1 0101 0064 0053 0029 044e 6301  .|.....d.S.).Nc.
-00001520: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00001530: 0000 0073 0000 0073 1a00 0000 8100 7c00  ...s...s......|.
-00001540: 5d08 7d01 7400 7c01 7401 8302 5600 0100  ].}.t.|.t...V...
-00001550: 7102 6400 5300 7235 0000 0029 0272 4900  q.d.S.r5...).rI.
-00001560: 0000 7216 0000 0029 0272 6b00 0000 da04  ..r....).rk.....
-00001570: 656c 656d 721d 0000 0072 1d00 0000 721e  elemr....r....r.
-00001580: 0000 0072 6d00 0000 a800 0000 f304 0000  ...rm...........
-00001590: 0002 8018 007a 2844 696d 656e 7369 6f6e  .....z(Dimension
-000015a0: 5365 742e 5f5f 696e 6974 5f5f 2e3c 6c6f  Set.__init__.<lo
-000015b0: 6361 6c73 3e2e 3c67 656e 6578 7072 3e7a  cals>.<genexpr>z
-000015c0: 1342 6164 207b 666f 616d 5f75 6e69 7473  .Bad {foam_units
-000015d0: 203d 207d 2904 da03 616c 6cda 0a56 616c   = })...all..Val
-000015e0: 7565 4572 726f 7272 5d00 0000 723a 0000  ueErrorr]...r:..
-000015f0: 0029 0272 2e00 0000 7226 0000 0072 5e00  .).r....r&...r^.
-00001600: 0000 721d 0000 0072 1e00 0000 723a 0000  ..r....r....r:..
-00001610: 00a7 0000 0073 0600 0000 1201 0801 1001  .....s..........
-00001620: 7a15 4469 6d65 6e73 696f 6e53 6574 2e5f  z.DimensionSet._
-00001630: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-00001640: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00001650: 7308 0000 0074 007c 0083 0153 0072 3500  s....t.|...S.r5.
-00001660: 0000 2901 722a 0000 0072 6700 0000 721d  ..).r*...rg...r.
-00001670: 0000 0072 1d00 0000 721e 0000 0072 3c00  ...r....r....r<.
-00001680: 0000 ac00 0000 f302 0000 0008 017a 1544  .............z.D
-00001690: 696d 656e 7369 6f6e 5365 742e 5f5f 7265  imensionSet.__re
-000016a0: 7072 5f5f 7201 0000 0063 0200 0000 0000  pr__r....c......
-000016b0: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
-000016c0: 0000 731c 0000 0064 0164 02a0 0064 0364  ..s....d.d...d.d
-000016d0: 0484 007c 0044 0083 01a1 0117 0064 0517  ...|.D.......d..
-000016e0: 0053 0029 064e 726f 0000 0072 3e00 0000  .S.).Nro...r>...
-000016f0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001700: 0003 0000 0073 0000 0072 6800 0000 7235  .....s...rh...r5
-00001710: 0000 0072 6900 0000 726a 0000 0072 1d00  ...ri...rj...r..
-00001720: 0000 721d 0000 0072 1e00 0000 726d 0000  ..r....r....rm..
-00001730: 00b0 0000 0072 6e00 0000 7a37 4469 6d65  .....rn...z7Dime
-00001740: 6e73 696f 6e53 6574 2e64 756d 705f 7769  nsionSet.dump_wi
-00001750: 7468 6f75 745f 6173 7369 676e 6d65 6e74  thout_assignment
-00001760: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
-00001770: 7072 3efa 015d a901 7224 0000 0072 5500  pr>..]..r$...rU.
-00001780: 0000 721d 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-00001790: 0072 4400 0000 af00 0000 f302 0000 001c  .rD.............
-000017a0: 017a 2444 696d 656e 7369 6f6e 5365 742e  .z$DimensionSet.
-000017b0: 6475 6d70 5f77 6974 686f 7574 5f61 7373  dump_without_ass
-000017c0: 6967 6e6d 656e 7472 5700 0000 2907 7231  ignmentrW...).r1
-000017d0: 0000 0072 3200 0000 7233 0000 0072 3a00  ...r2...r3...r:.
-000017e0: 0000 723c 0000 0072 4400 0000 7260 0000  ..r<...rD...r`..
-000017f0: 0072 1d00 0000 721d 0000 0072 5e00 0000  .r....r....r^...
-00001800: 721e 0000 0072 7000 0000 a600 0000 7308  r....rp.......s.
-00001810: 0000 0008 000c 0108 0512 0372 7000 0000  ...........rp...
-00001820: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00001830: 0004 0000 0000 0000 0073 3c00 0000 6500  .........s<...e.
-00001840: 5a01 6400 5a02 640b 8700 6601 6402 6403  Z.d.Z.d...f.d.d.
-00001850: 8409 5a03 6404 6405 8400 5a04 8700 6601  ..Z.d.d...Z...f.
-00001860: 6406 6407 8408 5a05 640c 6409 640a 8401  d.d...Z.d.d.d...
-00001870: 5a06 8700 0400 5a07 5300 290d da04 4469  Z.....Z.S.)...Di
-00001880: 6374 4e63 0400 0000 0000 0000 0000 0000  ctNc............
-00001890: 0400 0000 0400 0000 0300 0000 7322 0000  ............s"..
-000018a0: 007c 027c 005f 007c 037c 005f 0174 0283  .|.|._.|.|._.t..
-000018b0: 006a 0364 0169 007c 01a4 018e 0101 0064  .j.d.i.|.......d
-000018c0: 0053 0029 024e 721d 0000 0029 04da 055f  .S.).Nr....)..._
-000018d0: 6e61 6d65 da0a 5f64 6972 6563 7469 7665  name.._directive
-000018e0: 725d 0000 0072 3a00 0000 2904 722e 0000  r]...r:...).r...
-000018f0: 00da 0464 6174 6172 5200 0000 da09 6469  ...datarR.....di
-00001900: 7265 6374 6976 6572 5e00 0000 721d 0000  rectiver^...r...
-00001910: 0072 1e00 0000 723a 0000 00b4 0000 0073  .r....r:.......s
-00001920: 0600 0000 0601 0601 1601 7a0d 4469 6374  ..........z.Dict
-00001930: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-00001940: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
-00001950: 0000 f306 0000 007c 006a 0053 0072 3500  .......|.j.S.r5.
-00001960: 0000 a901 727a 0000 0072 6700 0000 721d  ....rz...rg...r.
-00001970: 0000 0072 1d00 0000 721e 0000 00da 0867  ...r....r......g
-00001980: 6574 5f6e 616d 65b9 0000 00f3 0200 0000  et_name.........
-00001990: 0601 7a0d 4469 6374 2e67 6574 5f6e 616d  ..z.Dict.get_nam
-000019a0: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
-000019b0: 0000 0200 0000 0300 0000 f30a 0000 0074  ...............t
-000019c0: 0083 00a0 01a1 0053 0072 3500 0000 725c  .......S.r5...r\
-000019d0: 0000 0072 6700 0000 725e 0000 0072 1d00  ...rg...r^...r..
-000019e0: 0000 721e 0000 0072 3c00 0000 bc00 0000  ..r....r<.......
-000019f0: f302 0000 000a 017a 0d44 6963 742e 5f5f  .......z.Dict.__
-00001a00: 7265 7072 5f5f 7201 0000 0063 0200 0000  repr__r....c....
-00001a10: 0000 0000 0000 0000 0b00 0000 0900 0000  ................
-00001a20: 4300 0000 7338 0100 0067 007d 027c 0164  C...s8...g.}.|.d
-00001a30: 0114 007d 037c 006a 0064 0075 0172 287c  ...}.|.j.d.u.r(|
-00001a40: 037c 006a 0017 007d 047c 006a 0164 0075  .|.j...}.|.j.d.u
-00001a50: 0172 1c7c 0464 027c 006a 0117 0037 007d  .r.|.d.|.j...7.}
-00001a60: 047c 02a0 027c 0464 037c 039b 009d 0217  .|...|.d.|......
-00001a70: 0064 0417 00a1 0101 007a 0b74 0364 0564  .d.......z.t.d.d
-00001a80: 0684 007c 0044 0083 0183 017d 0557 006e  ...|.D.....}.W.n
-00001a90: 0b04 0074 0479 3e01 0001 0001 0064 077d  ...t.y>......d.}
-00001aa0: 0559 006e 0177 0064 087d 067c 057c 0617  .Y.n.w.d.}.|.|..
-00001ab0: 007d 077c 00a0 05a1 0044 005d 465c 027d  .}.|.....D.]F\.}
-00001ac0: 087d 0974 067c 0964 0983 0272 5d7c 02a0  .}.t.|.d...r]|..
-00001ad0: 027c 09a0 077c 0164 0817 00a1 01a1 0101  .|...|.d........
-00001ae0: 0071 4974 067c 0964 0a83 0272 717c 02a0  .qIt.|.d...rq|..
-00001af0: 0264 0b7c 089b 0064 027c 09a0 08a1 009b  .d.|...d.|......
-00001b00: 0064 0c9d 05a1 0101 0071 497c 0964 0d6b  .d.......qI|.d.k
-00001b10: 0272 7864 0d7d 0a6e 087c 0774 097c 0883  .rxd.}.n.|.t.|..
-00001b20: 0118 0064 0114 007d 0a7c 02a0 027c 0364  ...d...}.|...|.d
-00001b30: 0b7c 089b 007c 0a9b 007c 099b 0064 0c9d  .|...|...|...d..
-00001b40: 0517 00a1 0101 0071 497c 02a0 027c 0364  .......qI|...|.d
-00001b50: 0e17 00a1 0101 0064 03a0 0a7c 02a1 0153  .......d...|...S
-00001b60: 0029 0f4e 723e 0000 0072 4500 0000 7242  .).Nr>...rE...rB
-00001b70: 0000 00da 017b 6301 0000 0000 0000 0000  .....{c.........
-00001b80: 0000 0002 0000 0003 0000 0073 0000 0072  ...........s...r
-00001b90: 6800 0000 7235 0000 0029 0172 4700 0000  h...r5...).rG...
-00001ba0: 2902 726b 0000 0072 4c00 0000 721d 0000  ).rk...rL...r...
-00001bb0: 0072 1d00 0000 721e 0000 0072 6d00 0000  .r....r....rm...
-00001bc0: c900 0000 726e 0000 007a 1c44 6963 742e  ....rn...z.Dict.
-00001bd0: 6475 6d70 2e3c 6c6f 6361 6c73 3e2e 3c67  dump.<locals>.<g
-00001be0: 656e 6578 7072 3e72 0100 0000 e904 0000  enexpr>r........
-00001bf0: 0072 4300 0000 7244 0000 0072 3f00 0000  .rC...rD...r?...
-00001c00: 7240 0000 0072 0c00 0000 7241 0000 0029  r@...r....rA...)
-00001c10: 0b72 7a00 0000 727b 0000 0072 2300 0000  .rz...r{...r#...
-00001c20: da03 6d61 7872 7400 0000 7246 0000 0072  ..maxrt...rF...r
-00001c30: 4800 0000 7243 0000 0072 4400 0000 7247  H...rC...rD...rG
-00001c40: 0000 0072 2400 0000 290b 722e 0000 0072  ...r$...).r....r
-00001c50: 5600 0000 723b 0000 00da 0b69 6e64 656e  V...r;.....inden
-00001c60: 7461 7469 6f6e da04 6c69 6e65 da0a 6d61  tation..line..ma
-00001c70: 785f 6c65 6e67 7468 5a0d 6465 6661 756c  x_lengthZ.defaul
-00001c80: 745f 7370 6163 65da 0a6e 756d 5f73 7061  t_space..num_spa
-00001c90: 6365 7372 4c00 0000 724d 0000 0072 0600  cesrL...rM...r..
-00001ca0: 0000 721d 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-00001cb0: 0072 4300 0000 bf00 0000 7332 0000 0004  .rC.......s2....
-00001cc0: 0108 010a 010a 010a 010e 0118 0102 0216  ................
-00001cd0: 010c 0108 0102 ff04 0308 0110 010a 0116  ................
-00001ce0: 010a 011e 0108 0206 0110 0220 010e 010a  ........... ....
-00001cf0: 017a 0944 6963 742e 6475 6d70 724f 0000  .z.Dict.dumprO..
-00001d00: 0072 5700 0000 2908 7231 0000 0072 3200  .rW...).r1...r2.
-00001d10: 0000 7233 0000 0072 3a00 0000 7280 0000  ..r3...r:...r...
-00001d20: 0072 3c00 0000 7243 0000 0072 6000 0000  .r<...rC...r`...
-00001d30: 721d 0000 0072 1d00 0000 725e 0000 0072  r....r....r^...r
-00001d40: 1e00 0000 7279 0000 00b3 0000 0073 0a00  ....ry.......s..
-00001d50: 0000 0800 0e01 0805 0c03 1203 7279 0000  ............ry..
-00001d60: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00001d70: 0000 0400 0000 0000 0000 735a 0000 0065  ..........sZ...e
-00001d80: 005a 0164 005a 0264 015a 0364 1287 0066  .Z.d.Z.d.Z.d...f
-00001d90: 0164 0364 0484 095a 0464 0564 0684 005a  .d.d...Z.d.d...Z
-00001da0: 0564 0764 0884 005a 0687 0066 0164 0964  .d.d...Z...f.d.d
-00001db0: 0a84 085a 0764 0b64 0c84 005a 0864 1364  ...Z.d.d...Z.d.d
-00001dc0: 0e64 0f84 015a 0964 1364 1064 1184 015a  .d...Z.d.d.d...Z
-00001dd0: 0a87 0004 005a 0b53 0029 1472 4a00 0000  .....Z.S.).rJ...
-00001de0: 7a1b 5265 7072 6573 656e 7473 2061 6e20  z.Represents an 
-00001df0: 4f70 656e 466f 616d 206c 6973 744e 6303  OpenFoam listNc.
-00001e00: 0000 0000 0000 0000 0000 0003 0000 0003  ................
-00001e10: 0000 0003 0000 0073 1600 0000 7c02 7c00  .......s....|.|.
-00001e20: 5f00 7401 8300 a002 7c01 a101 0100 6400  _.t.....|.....d.
-00001e30: 5300 7235 0000 0029 0372 7a00 0000 725d  S.r5...).rz...r]
-00001e40: 0000 0072 3a00 0000 2903 722e 0000 00da  ...r:...).r.....
-00001e50: 0869 7465 7261 626c 6572 5200 0000 725e  .iterablerR...r^
-00001e60: 0000 0072 1d00 0000 721e 0000 0072 3a00  ...r....r....r:.
-00001e70: 0000 e100 0000 7304 0000 0006 0110 017a  ......s........z
-00001e80: 0d4c 6973 742e 5f5f 696e 6974 5f5f 6301  .List.__init__c.
-00001e90: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00001ea0: 0000 0043 0000 0072 7e00 0000 7235 0000  ...C...r~...r5..
-00001eb0: 0072 7f00 0000 7267 0000 0072 1d00 0000  .r....rg...r....
-00001ec0: 721d 0000 0072 1e00 0000 7280 0000 00e5  r....r....r.....
-00001ed0: 0000 0072 8100 0000 7a0d 4c69 7374 2e67  ...r....z.List.g
-00001ee0: 6574 5f6e 616d 6563 0200 0000 0000 0000  et_namec........
-00001ef0: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
-00001f00: 7348 0000 007c 006a 0064 0075 0072 0a7c  sH...|.j.d.u.r.|
-00001f10: 017c 005f 0064 0053 0074 017c 006a 0074  .|._.d.S.t.|.j.t
-00001f20: 0283 0272 217c 006a 007c 016b 0372 1f7c  ...r!|.j.|.k.r.|
-00001f30: 0164 0117 007c 006a 0017 007c 005f 0064  .d...|.j...|._.d
-00001f40: 0053 0064 0053 0074 0383 0082 0129 024e  .S.d.S.t.....).N
-00001f50: 723e 0000 0029 0472 7a00 0000 7249 0000  r>...).rz...rI..
-00001f60: 0072 5800 0000 da0c 5275 6e74 696d 6545  .rX.....RuntimeE
-00001f70: 7272 6f72 2902 722e 0000 0072 5200 0000  rror).r....rR...
-00001f80: 721d 0000 0072 1d00 0000 721e 0000 00da  r....r....r.....
-00001f90: 0861 6464 5f6e 616d 65e8 0000 0073 0e00  .add_name....s..
-00001fa0: 0000 0a01 0a01 0c01 0a01 1401 04ff 0603  ................
-00001fb0: 7a0d 4c69 7374 2e61 6464 5f6e 616d 6563  z.List.add_namec
-00001fc0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00001fd0: 0200 0000 0300 0000 7282 0000 0072 3500  ........r....r5.
-00001fe0: 0000 725c 0000 0072 6700 0000 725e 0000  ..r\...rg...r^..
-00001ff0: 0072 1d00 0000 721e 0000 0072 3c00 0000  .r....r....r<...
-00002000: f100 0000 7283 0000 007a 0d4c 6973 742e  ....r....z.List.
-00002010: 5f5f 7265 7072 5f5f 6302 0000 0000 0000  __repr__c.......
-00002020: 0000 0000 0002 0000 0003 0000 0003 0000  ................
-00002030: 0073 1400 0000 8700 8701 6602 6401 6402  .s........f.d.d.
-00002040: 8408 8801 4400 8301 5300 2903 4e63 0100  ....D...S.).Nc..
-00002050: 0000 0000 0000 0000 0000 0200 0000 0600  ................
-00002060: 0000 1300 0000 7318 0000 0067 007c 005d  ......s....g.|.]
-00002070: 087d 0188 01a0 007c 0188 00a1 0291 0271  .}.....|.......q
-00002080: 0253 0072 1d00 0000 a901 da0a 5f64 756d  .S.r........_dum
-00002090: 705f 6974 656d 2902 726b 0000 00da 0469  p_item).rk.....i
-000020a0: 7465 6da9 0272 5600 0000 722e 0000 0072  tem..rV...r....r
-000020b0: 1d00 0000 721e 0000 00da 0a3c 6c69 7374  ....r......<list
-000020c0: 636f 6d70 3ef5 0000 0073 0200 0000 1800  comp>....s......
-000020d0: 7a2b 4c69 7374 2e5f 6d61 6b65 5f6c 6973  z+List._make_lis
-000020e0: 745f 7374 7269 6e67 732e 3c6c 6f63 616c  t_strings.<local
-000020f0: 733e 2e3c 6c69 7374 636f 6d70 3e72 1d00  s>.<listcomp>r..
-00002100: 0000 7255 0000 0072 1d00 0000 7291 0000  ..rU...r....r...
-00002110: 0072 1e00 0000 da12 5f6d 616b 655f 6c69  .r......_make_li
-00002120: 7374 5f73 7472 696e 6773 f400 0000 7302  st_strings....s.
-00002130: 0000 0014 017a 174c 6973 742e 5f6d 616b  .....z.List._mak
-00002140: 655f 6c69 7374 5f73 7472 696e 6773 7201  e_list_stringsr.
-00002150: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
-00002160: 0300 0000 0300 0000 4300 0000 7324 0000  ........C...s$..
-00002170: 0074 007c 0164 0183 0272 0a7c 01a0 017c  .t.|.d...r.|...|
-00002180: 02a1 0153 007c 0264 0214 0074 027c 0183  ...S.|.d...t.|..
-00002190: 0117 0053 0029 034e 7243 0000 0072 3e00  ...S.).NrC...r>.
-000021a0: 0000 2903 7248 0000 0072 4300 0000 7258  ..).rH...rC...rX
-000021b0: 0000 0029 0372 2e00 0000 7290 0000 0072  ...).r....r....r
-000021c0: 5600 0000 721d 0000 0072 1d00 0000 721e  V...r....r....r.
-000021d0: 0000 0072 8f00 0000 f700 0000 7306 0000  ...r........s...
-000021e0: 000a 010a 0110 027a 0f4c 6973 742e 5f64  .......z.List._d
-000021f0: 756d 705f 6974 656d 6302 0000 0000 0000  ump_itemc.......
-00002200: 0000 0000 0009 0000 0008 0000 0003 0000  ................
-00002210: 0073 3c01 0000 6700 7d02 8800 6401 1400  .s<...g.}...d...
-00002220: 7d03 8801 6a00 6400 7500 721f 7c02 a001  }...j.d.u.r.|...
-00002230: 8801 6a02 6402 6403 8d01 a101 0100 7c03  ..j.d.d.......|.
-00002240: 6404 1700 6401 a003 7c02 a101 1700 6405  d...d...|.....d.
-00002250: 1700 5300 7c02 a004 7c03 8801 6a00 1700  ..S.|...|...j...
-00002260: 6406 7c03 9b00 9d02 1700 6404 1700 a101  d.|.......d.....
-00002270: 0100 6407 6408 6409 9c02 7d04 8801 6a00  ..d.d.d...}...j.
-00002280: 7c04 a005 a100 7601 7248 7c02 a004 6406  |.....v.rH|...d.
-00002290: a003 8801 a002 8800 640a 1700 a101 a101  ........d.......
-000022a0: a101 0100 6e4a 8801 7292 7c04 8801 6a00  ....nJ..r.|...j.
-000022b0: 1900 7d05 8801 6402 1900 7c05 6b02 7359  ..}...d...|.k.sY
-000022c0: 7406 8801 8301 8201 6700 7d06 6400 7d07  t.......g.}.d.}.
-000022d0: 8801 4400 5d18 7d08 7c08 7c05 6b02 7272  ..D.].}.|.|.k.rr
-000022e0: 7c07 6400 7501 726e 7c06 a004 7c07 a101  |.d.u.rn|...|...
-000022f0: 0100 7c08 6701 7d07 715f 7c07 a004 7c08  ..|.g.}.q_|...|.
-00002300: a101 0100 715f 7c06 a004 7c07 a101 0100  ....q_|...|.....
-00002310: 8701 6601 640b 640c 8408 7c06 4400 8301  ..f.d.d...|.D...
-00002320: 7d06 7c02 a001 8700 6601 640d 640e 8408  }.|.....f.d.d...
-00002330: 7c06 4400 8301 a101 0100 7c02 a004 7c03  |.D.......|...|.
-00002340: 640f 1700 a101 0100 6406 a003 7c02 a101  d.......d...|...
-00002350: 5300 2910 4e72 3e00 0000 7201 0000 00a9  S.).Nr>...r.....
-00002360: 0172 5600 0000 fa01 2872 6600 0000 7242  .rV.....(rf...rB
-00002370: 0000 00da 0368 6578 5a06 7370 6c69 6e65  .....hexZ.spline
-00002380: 2902 da06 626c 6f63 6b73 da05 6564 6765  )...blocks..edge
-00002390: 7372 8500 0000 6301 0000 0000 0000 0000  sr....c.........
-000023a0: 0000 0002 0000 0007 0000 0013 0000 0073  ...............s
-000023b0: 2400 0000 6700 7c00 5d0e 7d01 6400 a000  $...g.|.].}.d...
-000023c0: 8700 6601 6401 6402 8408 7c01 4400 8301  ..f.d.d...|.D...
-000023d0: a101 9102 7102 5300 2903 723e 0000 0063  ....q.S.).r>...c
-000023e0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000023f0: 0400 0000 3300 0000 731a 0000 0081 007c  ....3...s......|
-00002400: 005d 087d 0188 00a0 007c 01a1 0156 0001  .].}.....|...V..
-00002410: 0071 0264 0053 0072 3500 0000 728e 0000  .q.d.S.r5...r...
-00002420: 0029 0272 6b00 0000 da05 5f69 7465 6d72  .).rk....._itemr
-00002430: 6700 0000 721d 0000 0072 1e00 0000 726d  g...r....r....rm
-00002440: 0000 0017 0100 0072 7200 0000 7a27 4c69  .......rr...z'Li
-00002450: 7374 2e64 756d 702e 3c6c 6f63 616c 733e  st.dump.<locals>
-00002460: 2e3c 6c69 7374 636f 6d70 3e2e 3c67 656e  .<listcomp>.<gen
-00002470: 6578 7072 3e72 7700 0000 2902 726b 0000  expr>rw...).rk..
-00002480: 00da 0a69 7465 6d73 5f6c 696e 6572 6700  ...items_linerg.
-00002490: 0000 721d 0000 0072 1e00 0000 7292 0000  ..r....r....r...
-000024a0: 0016 0100 0073 0800 0000 0600 0202 16ff  .....s..........
-000024b0: 06ff 7a1d 4c69 7374 2e64 756d 702e 3c6c  ..z.List.dump.<l
-000024c0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-000024d0: 3e63 0100 0000 0000 0000 0000 0000 0200  >c..............
-000024e0: 0000 0300 0000 3300 0000 7320 0000 0081  ......3...s ....
-000024f0: 007c 005d 0b7d 0188 0064 0017 0064 0114  .|.].}...d...d..
-00002500: 007c 0117 0056 0001 0071 0264 0253 0029  .|...V...q.d.S.)
-00002510: 0372 8500 0000 723e 0000 004e 721d 0000  .r....r>...Nr...
-00002520: 0029 0272 6b00 0000 7288 0000 0072 9400  .).rk...r....r..
-00002530: 0000 721d 0000 0072 1e00 0000 726d 0000  ..r....r....rm..
-00002540: 001a 0100 0073 0400 0000 0280 1e00 7a1c  .....s........z.
-00002550: 4c69 7374 2e64 756d 702e 3c6c 6f63 616c  List.dump.<local
-00002560: 733e 2e3c 6765 6e65 7870 723e 7a02 293b  s>.<genexpr>z.);
-00002570: 2907 727a 0000 00da 0665 7874 656e 6472  ).rz.....extendr
-00002580: 9300 0000 7224 0000 0072 2300 0000 da04  ....r$...r#.....
-00002590: 6b65 7973 7274 0000 0029 0972 2e00 0000  keysrt...).r....
-000025a0: 7256 0000 0072 3b00 0000 7287 0000 005a  rV...r;...r....Z
-000025b0: 0c73 7065 6369 616c 5f6b 6579 735a 0b73  .special_keysZ.s
-000025c0: 7065 6369 616c 5f6b 6579 da05 6c69 6e65  pecial_key..line
-000025d0: 7372 9a00 0000 7290 0000 0072 1d00 0000  sr....r....r....
-000025e0: 7291 0000 0072 1e00 0000 7243 0000 00fd  r....r....rC....
-000025f0: 0000 0073 3800 0000 0401 0801 0a01 1201  ...s8...........
-00002600: 1601 1e02 0a01 0e01 1c01 0401 0a01 0c01  ................
-00002610: 0801 0401 0401 0801 0801 0801 0a01 0801  ................
-00002620: 0c02 0a01 0a01 0202 06fe 1804 0e01 0a01  ................
-00002630: 7a09 4c69 7374 2e64 756d 7072 4f00 0000  z.List.dumprO...
-00002640: 7257 0000 0029 0c72 3100 0000 7232 0000  rW...).r1...r2..
-00002650: 0072 3300 0000 da07 5f5f 646f 635f 5f72  .r3.....__doc__r
-00002660: 3a00 0000 7280 0000 0072 8d00 0000 723c  :...r....r....r<
-00002670: 0000 0072 9300 0000 728f 0000 0072 4300  ...r....r....rC.
-00002680: 0000 7260 0000 0072 1d00 0000 721d 0000  ..r`...r....r...
-00002690: 0072 5e00 0000 721e 0000 0072 4a00 0000  .r^...r....rJ...
-000026a0: de00 0000 7312 0000 0008 0004 010e 0208  ....s...........
-000026b0: 0408 030c 0908 030a 0312 0672 4a00 0000  ...........rJ...
-000026c0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000026d0: 0001 0000 0040 0000 0073 1000 0000 6500  .....@...s....e.
-000026e0: 5a01 6400 5a02 6401 5a03 6402 5300 2903  Z.d.Z.d.Z.d.S.).
-000026f0: da0a 436f 6465 5374 7265 616d 7a22 4120  ..CodeStreamz"A 
-00002700: 6469 6374 696f 6e6e 6172 7920 746f 2073  dictionnary to s
-00002710: 746f 7265 2023 636f 6465 5374 7265 616d  tore #codeStream
-00002720: 4e29 0472 3100 0000 7232 0000 0072 3300  N).r1...r2...r3.
-00002730: 0000 729e 0000 0072 1d00 0000 721d 0000  ..r....r....r...
-00002740: 0072 1d00 0000 721e 0000 0072 9f00 0000  .r....r....r....
-00002750: 1f01 0000 7304 0000 0008 0008 0172 9f00  ....s........r..
-00002760: 0000 6301 0000 0000 0000 0000 0000 0003  ..c.............
-00002770: 0000 0003 0000 0003 0000 0073 2200 0000  ...........s"...
-00002780: 8700 6601 6401 6402 8408 7d01 8700 6601  ..f.d.d...}...f.
-00002790: 6403 6404 8408 7d02 7400 7c01 7c02 8302  d.d...}.t.|.|...
-000027a0: 5300 2905 4e63 0100 0000 0000 0000 0000  S.).Nc..........
-000027b0: 0000 0100 0000 0200 0000 1300 0000 730a  ..............s.
-000027c0: 0000 007c 0088 0019 006a 0053 0072 3500  ...|.....j.S.r5.
-000027d0: 0000 a901 da04 636f 6465 7267 0000 00a9  ......coderg....
-000027e0: 0172 5200 0000 721d 0000 0072 1e00 0000  .rR...r....r....
-000027f0: da03 6765 7424 0100 0072 8300 0000 7a18  ..get$...r....z.
-00002800: 5f6d 616b 655f 616c 6961 732e 3c6c 6f63  _make_alias.<loc
-00002810: 616c 733e 2e67 6574 6302 0000 0000 0000  als>.getc.......
-00002820: 0000 0000 0002 0000 0003 0000 0013 0000  ................
-00002830: 0073 0e00 0000 7c01 7c00 8800 1900 5f00  .s....|.|....._.
-00002840: 6400 5300 7235 0000 0072 a000 0000 2902  d.S.r5...r....).
-00002850: da05 5f73 656c 6672 5300 0000 72a2 0000  .._selfrS...r...
-00002860: 0072 1d00 0000 721e 0000 00da 0373 6574  .r....r......set
-00002870: 2701 0000 f302 0000 000e 017a 185f 6d61  '..........z._ma
-00002880: 6b65 5f61 6c69 6173 2e3c 6c6f 6361 6c73  ke_alias.<locals
-00002890: 3e2e 7365 7429 01da 0870 726f 7065 7274  >.set)...propert
-000028a0: 7929 0372 5200 0000 72a3 0000 0072 a500  y).rR...r....r..
-000028b0: 0000 721d 0000 0072 a200 0000 721e 0000  ..r....r....r...
-000028c0: 00da 0b5f 6d61 6b65 5f61 6c69 6173 2301  ..._make_alias#.
-000028d0: 0000 7306 0000 000c 010c 030a 0372 a800  ..s..........r..
-000028e0: 0000 2904 5a0b 636f 6465 496e 636c 7564  ..).Z.codeInclud
-000028f0: 655a 0b63 6f64 654f 7074 696f 6e73 5a08  eZ.codeOptionsZ.
-00002900: 636f 6465 4c69 6273 72a1 0000 0063 0000  codeLibsr....c..
-00002910: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00002920: 0000 4000 0000 7261 0000 0029 0bda 0443  ..@...ra...)...C
-00002930: 6f64 654e 6304 0000 0000 0000 0000 0000  odeNc...........
-00002940: 0004 0000 0002 0000 0043 0000 0073 1a00  .........C...s..
-00002950: 0000 7c01 7c00 5f00 7401 7c02 8301 7c00  ..|.|._.t.|...|.
-00002960: 5f02 7c03 7c00 5f03 6400 5300 7235 0000  _.|.|._.d.S.r5..
-00002970: 0029 0472 5200 0000 7203 0000 0072 a100  .).rR...r....r..
-00002980: 0000 727d 0000 0029 0472 2e00 0000 7252  ..r}...).r....rR
-00002990: 0000 0072 a100 0000 727d 0000 0072 1d00  ...r....r}...r..
-000029a0: 0000 721d 0000 0072 1e00 0000 723a 0000  ..r....r....r:..
-000029b0: 0032 0100 0073 0600 0000 0601 0a01 0a01  .2...s..........
-000029c0: 7a0d 436f 6465 2e5f 5f69 6e69 745f 5f63  z.Code.__init__c
-000029d0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000029e0: 0500 0000 4300 0000 733e 0000 007c 006a  ....C...s>...|.j
-000029f0: 0064 0075 0072 1064 017c 006a 0164 0064  .d.u.r.d.|.j.d.d
-00002a00: 0285 0219 009b 0064 039d 0353 0064 017c  .......d...S.d.|
-00002a10: 006a 0164 0064 0285 0219 009b 0064 047c  .j.d.d.......d.|
-00002a20: 006a 009b 0064 059d 0553 0029 064e 7a06  .j...d...S.).Nz.
-00002a30: 436f 6465 2822 e914 0000 007a 075b 2e2e  Code(".....z.[..
-00002a40: 2e5d 2229 7a12 5b2e 2e2e 5d22 2c20 6469  .]")z.[...]", di
-00002a50: 7265 6374 6976 653d 7266 0000 0029 0272  rective=rf...).r
-00002a60: 7d00 0000 72a1 0000 0072 6700 0000 721d  }...r....rg...r.
-00002a70: 0000 0072 1d00 0000 721e 0000 0072 3c00  ...r....r....r<.
-00002a80: 0000 3701 0000 7306 0000 000a 0116 011e  ..7...s.........
-00002a90: 017a 0d43 6f64 652e 5f5f 7265 7072 5f5f  .z.Code.__repr__
-00002aa0: 7201 0000 0063 0200 0000 0000 0000 0000  r....c..........
-00002ab0: 0000 0700 0000 0500 0000 4300 0000 738a  ..........C...s.
-00002ac0: 0000 0067 007d 027c 0164 0114 007d 037c  ...g.}.|.d...}.|
-00002ad0: 0164 0217 0064 0114 007d 047c 037c 006a  .d...d...}.|.|.j
-00002ae0: 0017 007d 057c 006a 0164 0075 0172 1d7c  ...}.|.j.d.u.r.|
-00002af0: 0564 017c 006a 0117 0037 007d 057c 02a0  .d.|.j...7.}.|..
-00002b00: 027c 0564 037c 039b 009d 0217 0064 0417  .|.d.|.......d..
-00002b10: 00a1 0101 007c 006a 03a0 0464 03a1 0144  .....|.j...d...D
-00002b20: 005d 097d 067c 02a0 027c 047c 0617 00a1  .].}.|...|.|....
-00002b30: 0101 0071 2f7c 02a0 027c 0364 0517 00a1  ...q/|...|.d....
-00002b40: 0101 0064 03a0 057c 02a1 0153 0029 064e  ...d...|...S.).N
-00002b50: 723e 0000 0072 8500 0000 7242 0000 007a  r>...r....rB...z
-00002b60: 0223 7b7a 0423 7d3b 0a29 0672 5200 0000  .#{z.#};.).rR...
-00002b70: 727d 0000 0072 2300 0000 72a1 0000 0072  r}...r#...r....r
-00002b80: 1500 0000 7224 0000 0029 0772 2e00 0000  ....r$...).r....
-00002b90: 7256 0000 0072 3b00 0000 7287 0000 005a  rV...r;...r....Z
-00002ba0: 0c69 6e64 656e 7461 7469 6f6e 3472 1300  .indentation4r..
-00002bb0: 0000 7288 0000 0072 1d00 0000 721d 0000  ..r....r....r...
-00002bc0: 0072 1e00 0000 7243 0000 003c 0100 0073  .r....rC...<...s
-00002bd0: 1600 0000 0401 0801 0c01 0a01 0a01 0e01  ................
-00002be0: 1801 1001 1001 0e01 0a01 7a09 436f 6465  ..........z.Code
-00002bf0: 2e64 756d 7072 3500 0000 7257 0000 0072  .dumpr5...rW...r
-00002c00: 5000 0000 721d 0000 0072 1d00 0000 721d  P...r....r....r.
-00002c10: 0000 0072 1e00 0000 72a9 0000 0031 0100  ...r....r....1..
-00002c20: 0073 0800 0000 0800 0a01 0805 0e05 72a9  .s............r.
-00002c30: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00002c40: 0000 0000 0300 0000 4000 0000 7261 0000  ........@...ra..
-00002c50: 0029 0bda 044e 616d 654e 6303 0000 0000  .)...NameNc.....
-00002c60: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
-00002c70: 0000 00f3 1000 0000 7c01 7c00 5f00 7c02  ........|.|._.|.
-00002c80: 7c00 5f01 6400 5300 7235 0000 0029 0272  |._.d.S.r5...).r
-00002c90: 5200 0000 7253 0000 0029 0372 2e00 0000  R...rS...).r....
-00002ca0: 7252 0000 0072 5300 0000 721d 0000 0072  rR...rS...r....r
-00002cb0: 1d00 0000 721e 0000 0072 3a00 0000 4c01  ....r....r:...L.
-00002cc0: 0000 f304 0000 0006 010a 017a 0d4e 616d  ...........z.Nam
-00002cd0: 652e 5f5f 696e 6974 5f5f 6301 0000 0000  e.__init__c.....
-00002ce0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00002cf0: 0000 0073 0e00 0000 6401 7c00 6a00 9b00  ...s....d.|.j...
-00002d00: 6402 9d03 5300 2903 4e7a 054e 616d 6528  d...S.).Nz.Name(
-00002d10: 7266 0000 0072 a200 0000 7267 0000 0072  rf...r....rg...r
-00002d20: 1d00 0000 721d 0000 0072 1e00 0000 723c  ....r....r....r<
-00002d30: 0000 0050 0100 0072 a600 0000 7a0d 4e61  ...P...r....z.Na
-00002d40: 6d65 2e5f 5f72 6570 725f 5f72 0100 0000  me.__repr__r....
-00002d50: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00002d60: 0001 0000 0043 0000 0073 0800 0000 7c00  .....C...s....|.
-00002d70: 6a00 9b00 5300 7235 0000 0072 a200 0000  j...S.r5...r....
-00002d80: 7255 0000 0072 1d00 0000 721d 0000 0072  rU...r....r....r
-00002d90: 1e00 0000 7243 0000 0053 0100 0072 7500  ....rC...S...ru.
-00002da0: 0000 7a09 4e61 6d65 2e64 756d 7072 3500  ..z.Name.dumpr5.
-00002db0: 0000 7257 0000 0072 5000 0000 721d 0000  ..rW...rP...r...
-00002dc0: 0072 1d00 0000 721d 0000 0072 1e00 0000  .r....r....r....
-00002dd0: 72ab 0000 004a 0100 0073 0800 0000 0800  r....J...s......
-00002de0: 0a02 0804 0e03 72ab 0000 0063 0000 0000  ......r....c....
-00002df0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00002e00: 4000 0000 7326 0000 0065 005a 0164 005a  @...s&...e.Z.d.Z
-00002e10: 0264 0164 0284 005a 0364 0364 0484 005a  .d.d...Z.d.d...Z
-00002e20: 0464 0964 0664 0784 015a 0564 0853 0029  .d.d.d...Z.d.S.)
-00002e30: 0ada 0944 6972 6563 7469 7665 6303 0000  ...Directivec...
-00002e40: 0000 0000 0000 0000 0003 0000 0002 0000  ................
-00002e50: 0043 0000 0072 ac00 0000 7235 0000 00a9  .C...r....r5....
-00002e60: 0272 7d00 0000 da07 636f 6e74 656e 7429  .r}.....content)
-00002e70: 0372 2e00 0000 727d 0000 0072 b000 0000  .r....r}...r....
-00002e80: 721d 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00002e90: 3a00 0000 5801 0000 72ad 0000 007a 1244  :...X...r....z.D
-00002ea0: 6972 6563 7469 7665 2e5f 5f69 6e69 745f  irective.__init_
-00002eb0: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
-00002ec0: 0000 0300 0000 4300 0000 7312 0000 007c  ......C...s....|
-00002ed0: 006a 009b 0064 017c 006a 019b 009d 0353  .j...d.|.j.....S
-00002ee0: 0029 024e 7245 0000 0072 af00 0000 7267  .).NrE...r....rg
-00002ef0: 0000 0072 1d00 0000 721d 0000 0072 1e00  ...r....r....r..
-00002f00: 0000 723c 0000 005c 0100 0073 0200 0000  ..r<...\...s....
-00002f10: 1201 7a12 4469 7265 6374 6976 652e 5f5f  ..z.Directive.__
-00002f20: 7265 7072 5f5f 7201 0000 0063 0200 0000  repr__r....c....
-00002f30: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00002f40: 4300 0000 731c 0000 007c 0164 0114 007c  C...s....|.d...|
-00002f50: 006a 009b 0064 027c 006a 019b 0064 039d  .j...d.|.j...d..
-00002f60: 0417 0053 0029 044e 723e 0000 0072 4500  ...S.).Nr>...rE.
-00002f70: 0000 7240 0000 0072 af00 0000 7255 0000  ..r@...r....rU..
-00002f80: 0072 1d00 0000 721d 0000 0072 1e00 0000  .r....r....r....
-00002f90: 7243 0000 005f 0100 0072 7800 0000 7a0e  rC..._...rx...z.
-00002fa0: 4469 7265 6374 6976 652e 6475 6d70 4e72  Directive.dumpNr
-00002fb0: 5700 0000 7250 0000 0072 1d00 0000 721d  W...rP...r....r.
-00002fc0: 0000 0072 1d00 0000 721e 0000 0072 ae00  ...r....r....r..
-00002fd0: 0000 5701 0000 7308 0000 0008 0008 0108  ..W...s.........
-00002fe0: 040e 0372 ae00 0000 291b 7211 0000 00da  ...r....).r.....
-00002ff0: 0b64 6174 6163 6c61 7373 6573 7202 0000  .dataclassesr...
-00003000: 00da 0874 6578 7477 7261 7072 0300 0000  ...textwrapr....
-00003010: da0a 696e 666c 6563 7469 6f6e 7204 0000  ..inflectionr...
-00003020: 0072 1700 0000 721f 0000 0072 2a00 0000  .r....r....r*...
-00003030: 722b 0000 0072 3400 0000 7251 0000 0072  r+...r4...rQ...r
-00003040: 5b00 0000 7262 0000 0072 6300 0000 7270  [...rb...rc...rp
-00003050: 0000 00da 0464 6963 7472 7900 0000 724a  .....dictry...rJ
-00003060: 0000 0072 9f00 0000 72a8 0000 0072 7a00  ...r....r....rz.
-00003070: 0000 da07 7365 7461 7474 7272 a900 0000  ....setattrr....
-00003080: 72ab 0000 0072 ae00 0000 721d 0000 0072  r....r....r....r
-00003090: 1d00 0000 721d 0000 0072 1e00 0000 da08  ....r....r......
-000030a0: 3c6d 6f64 756c 653e 0100 0000 7332 0000  <module>....s2..
-000030b0: 0008 000c 010c 010c 0208 0208 0308 1b0e  ................
-000030c0: 1210 0702 2f10 0110 0b02 0c12 0112 2012  ..../......... .
-000030d0: 0d12 2b10 4108 0408 0a16 0110 0302 1912  ..+.A...........
-000030e0: 0114 0c                                  ...
+00000020: 0006 0000 0040 0000 0073 8601 0000 6400  .....@...s....d.
+00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
+00000040: 6d03 5a03 6d04 5a04 0100 6401 6404 6c05  m.Z.m.Z...d.d.l.
+00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
+00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
+00000070: 6407 6c0b 6d0c 5a0c 0100 6401 6408 6c0d  d.l.m.Z...d.d.l.
+00000080: 6d0e 5a0e 0100 6700 6409 a201 5a0f 640a  m.Z...g.d...Z.d.
+00000090: 640b 8400 5a10 640c 640d 8400 5a11 642e  d...Z.d.d...Z.d.
+000000a0: 640f 6410 8401 5a12 4700 6411 6412 8400  d.d...Z.G.d.d...
+000000b0: 6412 8302 5a13 4700 6413 6414 8400 6414  d...Z.G.d.d...d.
+000000c0: 6503 8303 5a14 4700 6415 6416 8400 6416  e...Z.G.d.d...d.
+000000d0: 6513 6514 8304 5a15 6506 4700 6417 6418  e.e...Z.e.G.d.d.
+000000e0: 8400 6418 8302 8301 5a16 4700 6419 641a  ..d.....Z.G.d.d.
+000000f0: 8400 641a 6516 8303 5a17 6506 4700 641b  ..d.e...Z.e.G.d.
+00000100: 641c 8400 641c 6513 8303 8301 5a18 4700  d...d.e.....Z.G.
+00000110: 641d 641e 8400 641e 6519 6513 8304 5a1a  d.d...d.e.e...Z.
+00000120: 4700 641f 6420 8400 6420 651b 6513 6514  G.d.d ..d e.e.e.
+00000130: 8305 5a1c 4700 6421 6422 8400 6422 6519  ..Z.G.d!d"..d"e.
+00000140: 6513 8304 5a1d 4700 6423 6424 8400 6424  e...Z.G.d#d$..d$
+00000150: 651c 8303 5a1e 6425 6426 8400 5a1f 6427  e...Z.d%d&..Z.d'
+00000160: 4400 5d0c 5a20 6521 651e 650e 6520 8301  D.].Z e!e.e.e ..
+00000170: 651f 6520 8301 8303 0100 719a 4700 6428  e.e ......q.G.d(
+00000180: 6429 8400 6429 6513 8303 5a22 6506 4700  d)..d)e...Z"e.G.
+00000190: 642a 642b 8400 642b 6513 8303 8301 5a23  d*d+..d+e.....Z#
+000001a0: 4700 642c 642d 8400 642d 6513 8303 5a24  G.d,d-..d-e...Z$
+000001b0: 6402 5300 292f 7a2e 4162 7374 7261 6374  d.S.)/z.Abstract
+000001c0: 2053 796e 7461 7820 5472 6565 7320 666f   Syntax Trees fo
+000001d0: 7220 4f70 656e 464f 414d 2069 6e70 7574  r OpenFOAM input
+000001e0: 2066 696c 6573 e900 0000 004e 2902 da03   files.....N)...
+000001f0: 4142 43da 0e61 6273 7472 6163 746d 6574  ABC..abstractmet
+00000200: 686f 6429 01da 0964 6174 6163 6c61 7373  hod)...dataclass
+00000210: 2901 da06 4e75 6d62 6572 2901 da06 6465  )...Number)...de
+00000220: 6465 6e74 2901 da08 4f70 7469 6f6e 616c  dent)...Optional
+00000230: 2901 da0a 756e 6465 7273 636f 7265 2907  )...underscore).
+00000240: da02 6b67 da01 6dda 0173 da01 4b5a 046b  ..kg..m..s..KZ.k
+00000250: 6d6f 6cda 0141 da02 6364 6301 0000 0000  mol..A..cdc.....
+00000260: 0000 0000 0000 0009 0000 0008 0000 0043  ...............C
+00000270: 0000 0073 d600 0000 6401 6701 6402 1400  ...s....d.g.d...
+00000280: 7d01 6403 7d02 7c00 7269 7a0a 7400 a001  }.d.}.|.riz.t...
+00000290: 6404 7c00 a102 a002 a100 7d03 5700 6e0f  d.|.......}.W.n.
+000002a0: 0400 7403 7922 0100 0100 0100 7c00 7d04  ..t.y"......|.}.
+000002b0: 6405 7d00 6406 7d05 5900 6e19 7700 7c00  d.}.d.}.Y.n.w.|.
+000002c0: 7c03 1900 7d05 7c05 6407 7600 732d 4a00  |...}.|.d.v.s-J.
+000002d0: 8201 7c00 6400 7c03 8502 1900 7d04 7c00  ..|.d.|.....}.|.
+000002e0: 7c03 6403 1700 6400 8502 1900 7d00 6408  |.d...d.....}.d.
+000002f0: 7c04 7600 724b 7c04 a004 6408 a101 5c02  |.v.rK|...d...\.
+00000300: 7d06 7d07 7405 7c07 8301 7d07 6e05 7c04  }.}.t.|...}.n.|.
+00000310: 6403 0202 7d06 7d07 7c06 6409 6b03 725f  d...}.}.|.d.k.r_
+00000320: 7406 a007 7c06 a101 7d08 7c02 7c07 1400  t...|...}.|.|...
+00000330: 7c01 7c08 3c00 7c05 6406 6b02 7265 6403  |.|.<.|.d.k.red.
+00000340: 6e01 640a 7d02 7c00 7309 7c01 5300 290b  n.d.}.|.s.|.S.).
+00000350: 4e72 0100 0000 e907 0000 00e9 0100 0000  Nr..............
+00000360: 7a04 5b2f 2e5d da00 da01 2e7a 022f 2efa  z.[/.].....z./..
+00000370: 015e da01 31e9 ffff ffff 2908 da02 7265  .^..1.....)...re
+00000380: da06 7365 6172 6368 da05 7374 6172 74da  ..search..start.
+00000390: 0e41 7474 7269 6275 7465 4572 726f 72da  .AttributeError.
+000003a0: 0573 706c 6974 da03 696e 74da 0773 796d  .split..int..sym
+000003b0: 626f 6c73 da05 696e 6465 7829 09da 0575  bols..index)...u
+000003c0: 6e69 7473 da06 7265 7375 6c74 da04 7369  nits..result..si
+000003d0: 676e 721d 0000 005a 0875 6e69 745f 616c  gnr....Z.unit_al
+000003e0: 6c5a 096e 6578 745f 6f70 6572 da09 756e  lZ.next_oper..un
+000003f0: 6974 5f6e 616d 655a 0a75 6e69 745f 7661  it_nameZ.unit_va
+00000400: 6c75 655a 0a75 6e69 745f 696e 6465 78a9  lueZ.unit_index.
+00000410: 0072 2200 0000 fa46 2f68 6f6d 652f 7069  .r"....F/home/pi
+00000420: 6572 7265 2f44 6576 2f66 6c75 6964 7369  erre/Dev/fluidsi
+00000430: 6d66 6f61 6d2f 7372 632f 666c 7569 6473  mfoam/src/fluids
+00000440: 696d 666f 616d 2f66 6f61 6d5f 696e 7075  imfoam/foam_inpu
+00000450: 745f 6669 6c65 732f 6173 742e 7079 da0e  t_files/ast.py..
+00000460: 7374 7232 666f 616d 5f75 6e69 7473 0f00  str2foam_units..
+00000470: 0000 7330 0000 000a 0104 0104 0102 0114  ..s0............
+00000480: 010c 0104 0104 0108 0102 fd08 050c 010c  ................
+00000490: 0110 0108 010e 010a 010a 0208 010a 010c  ................
+000004a0: 0110 0104 ec04 1572 2400 0000 6301 0000  .......r$...c...
+000004b0: 0000 0000 0000 0000 0005 0000 0008 0000  ................
+000004c0: 0043 0000 0073 a800 0000 6700 7d01 7400  .C...s....g.}.t.
+000004d0: 7401 7c00 8302 4400 5d2f 5c02 7d02 7d03  t.|...D.]/\.}.}.
+000004e0: 7c03 6401 6b02 7210 7107 7c03 6401 6b04  |.d.k.r.q.|.d.k.
+000004f0: 7216 6402 6e01 6403 7d04 7402 7c03 8301  r.d.n.d.}.t.|...
+00000500: 6404 6b02 7228 7c01 a003 7c04 9b00 7c02  d.k.r(|...|...|.
+00000510: 9b00 9d02 a101 0100 7107 7c01 a003 7c04  ........q.|...|.
+00000520: 9b00 7c02 9b00 6405 7402 7c03 8301 9b00  ..|...d.t.|.....
+00000530: 9d04 a101 0100 7107 6406 a004 7c01 a101  ......q.d...|...
+00000540: 7d01 7c01 a005 6402 a101 7249 7c01 6404  }.|...d...rI|.d.
+00000550: 6400 8502 1900 7d01 7c01 5300 7c01 a005  d.....}.|.S.|...
+00000560: 6403 a101 7252 6407 7c01 1700 7d01 7c01  d...rRd.|...}.|.
+00000570: 5300 2908 4e72 0100 0000 7212 0000 00fa  S.).Nr....r.....
+00000580: 012f 7210 0000 0072 1300 0000 7211 0000  ./r....r....r...
+00000590: 0072 1400 0000 2906 da03 7a69 7072 1c00  .r....)...zipr..
+000005a0: 0000 da03 6162 73da 0661 7070 656e 64da  ....abs..append.
+000005b0: 046a 6f69 6eda 0a73 7461 7274 7377 6974  .join..startswit
+000005c0: 6829 05da 0a66 6f61 6d5f 756e 6974 7372  h)...foam_unitsr
+000005d0: 1f00 0000 da06 7379 6d62 6f6c da08 6578  ......symbol..ex
+000005e0: 706f 6e65 6e74 da08 6f70 6572 6174 6f72  ponent..operator
+000005f0: 7222 0000 0072 2200 0000 7223 0000 00da  r"...r"...r#....
+00000600: 0e66 6f61 6d5f 756e 6974 7332 7374 722a  .foam_units2str*
+00000610: 0000 0073 1e00 0000 0401 1201 0801 0201  ...s............
+00000620: 1001 0c01 1401 1e02 0a01 0a01 0c01 0403  ................
+00000630: 0afe 0801 0401 722f 0000 00e9 1400 0000  ......r/........
+00000640: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00000650: 0008 0000 0043 0000 0073 4400 0000 7a10  .....C...sD...z.
+00000660: 7400 7c01 7401 6401 6402 8400 7c00 a002  t.|.t.d.d...|...
+00000670: a100 4400 8301 8301 8302 7d01 5700 6e0b  ..D.......}.W.n.
+00000680: 0400 7403 791b 0100 0100 0100 6403 7d01  ..t.y.......d.}.
+00000690: 5900 6e01 7700 6404 7d02 7c01 7c02 1700  Y.n.w.d.}.|.|...
+000006a0: 5300 2905 4e63 0100 0000 0000 0000 0000  S.).Nc..........
+000006b0: 0000 0300 0000 0500 0000 7300 0000 732a  ..........s...s*
+000006c0: 0000 0081 007c 005d 105c 027d 017d 0274  .....|.].\.}.}.t
+000006d0: 007c 0274 0174 0266 0283 0273 0274 037c  .|.t.t.f...s.t.|
+000006e0: 0183 0156 0001 0071 0264 0053 00a9 014e  ...V...q.d.S...N
+000006f0: 2904 da0a 6973 696e 7374 616e 6365 da04  )...isinstance..
+00000700: 4469 6374 da04 4c69 7374 da03 6c65 6e29  Dict..List..len)
+00000710: 03da 022e 30da 036b 6579 da05 7661 6c75  ....0..key..valu
+00000720: 6572 2200 0000 7222 0000 0072 2300 0000  er"...r"...r#...
+00000730: da09 3c67 656e 6578 7072 3e40 0000 0073  ..<genexpr>@...s
+00000740: 0e00 0000 0280 0400 0602 0c01 02fd 0601  ................
+00000750: 0aff 7a2b 5f63 6f6d 7075 7465 5f73 7061  ..z+_compute_spa
+00000760: 6365 735f 746f 5f61 6c69 676e 2e3c 6c6f  ces_to_align.<lo
+00000770: 6361 6c73 3e2e 3c67 656e 6578 7072 3e72  cals>.<genexpr>r
+00000780: 0100 0000 e904 0000 0029 04da 036d 696e  .........)...min
+00000790: da03 6d61 78da 0569 7465 6d73 da0a 5661  ..max..items..Va
+000007a0: 6c75 6545 7272 6f72 2903 da04 6461 7461  lueError)...data
+000007b0: da0a 6d61 785f 6c65 6e67 7468 5a0d 6465  ..max_lengthZ.de
+000007c0: 6661 756c 745f 7370 6163 6572 2200 0000  fault_spacer"...
+000007d0: 7222 0000 0072 2300 0000 da18 5f63 6f6d  r"...r#....._com
+000007e0: 7075 7465 5f73 7061 6365 735f 746f 5f61  pute_spaces_to_a
+000007f0: 6c69 676e 3c00 0000 7318 0000 0002 0102  lign<...s.......
+00000800: 0102 0108 0106 0206 fe08 fe0c 0808 0102  ................
+00000810: ff04 0308 0172 4100 0000 6300 0000 0000  .....rA...c.....
+00000820: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
+00000830: 0000 0073 1400 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00000840: 6401 6402 8400 5a03 6403 5300 2904 da04  d.d...Z.d.S.)...
+00000850: 4e6f 6465 6302 0000 0000 0000 0000 0000  Nodec...........
+00000860: 0002 0000 0003 0000 0043 0000 0073 2000  .........C...s .
+00000870: 0000 7400 7c01 8301 7400 7c00 8301 7500  ..t.|...t.|...u.
+00000880: 720e 7c00 6a01 7c01 6a01 6b02 5300 6401  r.|.j.|.j.k.S.d.
+00000890: 5300 2902 4e46 2902 da04 7479 7065 da08  S.).NF)...type..
+000008a0: 5f5f 6469 6374 5f5f 2902 da04 7365 6c66  __dict__)...self
+000008b0: da05 6f74 6865 7272 2200 0000 7222 0000  ..otherr"...r"..
+000008c0: 0072 2300 0000 da06 5f5f 6571 5f5f 4e00  .r#.....__eq__N.
+000008d0: 0000 7306 0000 0010 010c 0104 017a 0b4e  ..s..........z.N
+000008e0: 6f64 652e 5f5f 6571 5f5f 4e29 04da 085f  ode.__eq__N)..._
+000008f0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000900: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000910: 5f72 4700 0000 7222 0000 0072 2200 0000  _rG...r"...r"...
+00000920: 7222 0000 0072 2300 0000 7242 0000 004d  r"...r#...rB...M
+00000930: 0000 0073 0400 0000 0800 0c01 7242 0000  ...s........rB..
+00000940: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000950: 0000 0800 0000 4000 0000 7350 0000 0065  ......@...sP...e
+00000960: 005a 0164 005a 0209 0109 0209 0164 0e64  .Z.d.Z.......d.d
+00000970: 0365 0364 0465 0465 0319 0064 0565 0465  .e.d.e.e...d.e.e
+00000980: 0319 0066 0664 0664 0784 055a 0564 0864  ...f.d.d...Z.d.d
+00000990: 0984 005a 0664 0f64 0a64 0b84 015a 0765  ...Z.d.d.d...Z.e
+000009a0: 0864 0c64 0d84 0083 015a 0964 0153 0029  .d.d.....Z.d.S.)
+000009b0: 10da 0e4e 6f64 654c 696b 6550 7944 6963  ...NodeLikePyDic
+000009c0: 744e 4672 3f00 0000 da0a 6469 6d65 6e73  tNFr?.....dimens
+000009d0: 696f 6e73 da08 636f 6d6d 656e 7473 6305  ions..commentsc.
+000009e0: 0000 0000 0000 0000 0000 000b 0000 0007  ................
+000009f0: 0000 0043 0000 0073 fa00 0000 7c02 6400  ...C...s....|.d.
+00000a00: 7500 7206 6900 7d02 7c04 6400 7500 720c  u.r.i.}.|.d.u.r.
+00000a10: 6900 7d04 7c01 a000 a100 4400 5d6a 5c02  i.}.|.....D.]j\.
+00000a20: 7d05 7d06 7401 7c06 7402 6400 8301 7403  }.}.t.|.t.d...t.
+00000a30: 6602 8302 7224 7c00 a004 7c05 7c06 a102  f...r$|...|.|...
+00000a40: 0100 7110 7401 7c06 7405 7406 6602 8302  ..q.t.|.t.t.f...
+00000a50: 724d 7c03 6401 7500 7236 7c00 a004 7c05  rM|.d.u.r6|...|.
+00000a60: 7c06 a102 0100 7110 7c02 a007 7c05 7c03  |.....q.|...|.|.
+00000a70: a102 7d07 7401 7c06 7406 8302 7245 7408  ..}.t.|.t...rEt.
+00000a80: 7c06 8301 7d06 7c00 a009 7c05 7c06 7c07  |...}.|...|.|.|.
+00000a90: a103 0100 7110 7401 7c06 740a 8302 7275  ....q.t.|.t...ru
+00000aa0: 7c02 a007 7c05 6400 a102 7d08 7c04 a007  |...|.d...}.|...
+00000ab0: 7c05 6400 a102 7d09 740b 6900 7c05 7c09  |.d...}.t.i.|.|.
+00000ac0: 6402 8d03 7d0a 7c0a 6a0c 7c06 7c08 7c03  d...}.|.j.|.|.|.
+00000ad0: 7c09 6403 8d04 0100 7c00 a00d 7c05 7c0a  |.d.....|...|.|.
+00000ae0: a102 0100 7110 740e 7402 7c06 8301 8301  ....q.t.t.|.....
+00000af0: 8201 6400 5300 2904 4e46 2902 da04 6e61  ..d.S.).NF)...na
+00000b00: 6d65 724d 0000 0029 0372 4c00 0000 da11  merM...).rL.....
+00000b10: 6465 6661 756c 745f 6469 6d65 6e73 696f  default_dimensio
+00000b20: 6e72 4d00 0000 290f 723d 0000 0072 3200  nrM...).r=...r2.
+00000b30: 0000 7243 0000 00da 0373 7472 da09 7365  ..rC.....str..se
+00000b40: 745f 6368 696c 6472 0500 0000 da04 6c69  t_childr......li
+00000b50: 7374 da03 6765 7472 3400 0000 da09 7365  st..getr4.....se
+00000b60: 745f 7661 6c75 65da 0464 6963 7472 3300  t_value..dictr3.
+00000b70: 0000 da14 696e 6974 5f66 726f 6d5f 7079  ....init_from_py
+00000b80: 5f6f 626a 6563 7473 da09 5f73 6574 5f69  _objects.._set_i
+00000b90: 7465 6dda 134e 6f74 496d 706c 656d 656e  tem..NotImplemen
+00000ba0: 7465 6445 7272 6f72 290b 7245 0000 0072  tedError).rE...r
+00000bb0: 3f00 0000 724c 0000 0072 4f00 0000 724d  ?...rL...rO...rM
+00000bc0: 0000 0072 3700 0000 7238 0000 00da 0964  ...r7...r8.....d
+00000bd0: 696d 656e 7369 6f6e 5a0f 6469 6d65 6e73  imensionZ.dimens
+00000be0: 696f 6e73 5f64 6963 745a 0d63 6f6d 6d65  ions_dictZ.comme
+00000bf0: 6e74 735f 6469 6374 da03 6f62 6a72 2200  nts_dict..objr".
+00000c00: 0000 7222 0000 0072 2300 0000 7256 0000  ..r"...r#...rV..
+00000c10: 0055 0000 0073 3600 0000 0807 0401 0801  .U...s6.........
+00000c20: 0401 1001 1201 0e01 0e01 0801 0e01 0c02  ................
+00000c30: 0a01 0801 1001 0a01 0c01 0c01 0e01 0401  ................
+00000c40: 0201 0201 0201 0201 06fc 0e06 0c02 04e9  ................
+00000c50: 7a23 4e6f 6465 4c69 6b65 5079 4469 6374  z#NodeLikePyDict
+00000c60: 2e69 6e69 745f 6672 6f6d 5f70 795f 6f62  .init_from_py_ob
+00000c70: 6a65 6374 7363 0300 0000 0000 0000 0000  jectsc..........
+00000c80: 0000 0300 0000 0500 0000 4300 0000 735a  ..........C...sZ
+00000c90: 0000 0074 007c 0274 0164 0083 0174 0274  ...t.|.t.d...t.t
+00000ca0: 0366 0383 0272 0b6e 1a74 007c 0274 0483  .f...r.n.t.|.t..
+00000cb0: 0272 1774 057c 027c 0164 018d 027d 026e  .r.t.|.|.d...}.n
+00000cc0: 0e74 007c 0274 0683 0272 2374 077c 027c  .t.|.t...r#t.|.|
+00000cd0: 0164 018d 027d 026e 0274 0882 017c 00a0  .d...}.n.t...|..
+00000ce0: 097c 017c 02a1 0201 0064 0053 0029 024e  .|.|.....d.S.).N
+00000cf0: a901 724e 0000 0029 0a72 3200 0000 7243  ..rN...).r2...rC
+00000d00: 0000 0072 5000 0000 7205 0000 0072 5500  ...rP...r....rU.
+00000d10: 0000 7233 0000 0072 5200 0000 7234 0000  ..r3...rR...r4..
+00000d20: 0072 5800 0000 7257 0000 0029 0372 4500  .rX...rW...).rE.
+00000d30: 0000 7237 0000 00da 0563 6869 6c64 7222  ..r7.....childr"
+00000d40: 0000 0072 2200 0000 7223 0000 0072 5100  ...r"...r#...rQ.
+00000d50: 0000 7900 0000 7310 0000 0014 0102 010a  ..y...s.........
+00000d60: 010e 010a 010e 0104 0210 017a 184e 6f64  ...........z.Nod
+00000d70: 654c 696b 6550 7944 6963 742e 7365 745f  eLikePyDict.set_
+00000d80: 6368 696c 6463 0400 0000 0000 0000 0000  childc..........
+00000d90: 0000 0400 0000 0500 0000 4300 0000 7330  ..........C...s0
+00000da0: 0000 0074 007c 0274 0183 0273 097c 0364  ...t.|.t...s.|.d
+00000db0: 0075 0172 1074 027c 027c 017c 0364 018d  .u.r.t.|.|.|.d..
+00000dc0: 037d 027c 00a0 037c 017c 02a1 0201 0064  .}.|...|.|.....d
+00000dd0: 0053 0029 024e 2901 7259 0000 0029 0472  .S.).N).rY...).r
+00000de0: 3200 0000 7205 0000 00da 0556 616c 7565  2...r......Value
+00000df0: 7257 0000 0029 0472 4500 0000 724e 0000  rW...).rE...rN..
+00000e00: 0072 3800 0000 7259 0000 0072 2200 0000  .r8...rY...r"...
+00000e10: 7222 0000 0072 2300 0000 7254 0000 0084  r"...r#...rT....
+00000e20: 0000 0073 0600 0000 1201 0e01 1001 7a18  ...s..........z.
+00000e30: 4e6f 6465 4c69 6b65 5079 4469 6374 2e73  NodeLikePyDict.s
+00000e40: 6574 5f76 616c 7565 6303 0000 0000 0000  et_valuec.......
+00000e50: 0000 0000 0003 0000 0001 0000 0043 0000  .............C..
+00000e60: 0073 0400 0000 6401 5300 2902 7a0b 5365  .s....d.S.).z.Se
+00000e70: 7420 616e 2069 7465 6d4e 7222 0000 00a9  t an itemNr"....
+00000e80: 0372 4500 0000 7237 0000 0072 3800 0000  .rE...r7...r8...
+00000e90: 7222 0000 0072 2200 0000 7223 0000 0072  r"...r"...r#...r
+00000ea0: 5700 0000 8900 0000 7302 0000 0004 007a  W.......s......z
+00000eb0: 184e 6f64 654c 696b 6550 7944 6963 742e  .NodeLikePyDict.
+00000ec0: 5f73 6574 5f69 7465 6d29 034e 464e 7231  _set_item).NFNr1
+00000ed0: 0000 0029 0a72 4800 0000 7249 0000 0072  ...).rH...rI...r
+00000ee0: 4a00 0000 7255 0000 0072 0700 0000 7256  J...rU...r....rV
+00000ef0: 0000 0072 5100 0000 7254 0000 0072 0300  ...rQ...rT...r..
+00000f00: 0000 7257 0000 0072 2200 0000 7222 0000  ..rW...r"...r"..
+00000f10: 0072 2200 0000 7223 0000 0072 4b00 0000  .r"...r#...rK...
+00000f20: 5400 0000 731e 0000 0008 0002 0402 0102  T...s...........
+00000f30: 0104 fb02 0202 fe06 0302 fd06 050a fb08  ................
+00000f40: 240a 0b02 050e 0172 4b00 0000 6300 0000  $......rK...c...
+00000f50: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00000f60: 0040 0000 0073 3600 0000 6500 5a01 6400  .@...s6...e.Z.d.
+00000f70: 5a02 640c 6402 6403 8401 5a03 6404 6405  Z.d.d.d...Z.d.d.
+00000f80: 8400 5a04 6406 6407 8400 5a05 6408 6409  ..Z.d.d...Z.d.d.
+00000f90: 8400 5a06 640a 640b 8400 5a07 6401 5300  ..Z.d.d...Z.d.S.
+00000fa0: 290d da0d 466f 616d 496e 7075 7446 696c  )...FoamInputFil
+00000fb0: 654e 6305 0000 0000 0000 0000 0000 0005  eNc.............
+00000fc0: 0000 0002 0000 0043 0000 0073 2e00 0000  .......C...s....
+00000fd0: 7c01 7c00 5f00 7c02 6400 7500 7209 6900  |.|._.|.d.u.r.i.
+00000fe0: 7d02 7c02 7c00 5f01 7c03 7c00 5f02 7c04  }.|.|._.|.|._.|.
+00000ff0: 7c00 5f03 6400 7c00 5f04 6400 5300 7231  |._.d.|._.d.S.r1
+00001000: 0000 0029 05da 0469 6e66 6fda 0863 6869  ...)...info..chi
+00001010: 6c64 7265 6eda 0668 6561 6465 7272 4d00  ldren..headerrM.
+00001020: 0000 da04 7061 7468 2905 7245 0000 0072  ....path).rE...r
+00001030: 6000 0000 7261 0000 0072 6200 0000 724d  `...ra...rb...rM
+00001040: 0000 0072 2200 0000 7222 0000 0072 2300  ...r"...r"...r#.
+00001050: 0000 da08 5f5f 696e 6974 5f5f 8f00 0000  ....__init__....
+00001060: 730e 0000 0006 0108 0104 0106 0106 0106  s...............
+00001070: 010a 017a 1646 6f61 6d49 6e70 7574 4669  ...z.FoamInputFi
+00001080: 6c65 2e5f 5f69 6e69 745f 5f63 0100 0000  le.__init__c....
+00001090: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+000010a0: 4300 0000 7342 0000 0064 0167 017d 017c  C...sB...d.g.}.|
+000010b0: 006a 0064 0075 0172 127c 01a0 0164 027c  .j.d.u.r.|...d.|
+000010c0: 006a 009b 0064 039d 03a1 0101 007c 01a0  .j...d.......|..
+000010d0: 0164 047c 006a 029b 0064 059d 03a1 0101  .d.|.j...d......
+000010e0: 0064 06a0 037c 01a1 0153 0029 074e 7a0b  .d...|...S.).Nz.
+000010f0: 496e 7075 7446 696c 6528 0a7a 0569 6e66  InputFile(.z.inf
+00001100: 6f3d 7a02 2c0a 7a09 6368 696c 6472 656e  o=z.,.z.children
+00001110: 3d7a 020a 2972 1100 0000 2904 7260 0000  =z..)r....).r`..
+00001120: 0072 2800 0000 7261 0000 0072 2900 0000  .r(...ra...r)...
+00001130: 2902 7245 0000 00da 0374 6d70 7222 0000  ).rE.....tmpr"..
+00001140: 0072 2200 0000 7223 0000 00da 085f 5f72  .r"...r#.....__r
+00001150: 6570 725f 5f98 0000 0073 0a00 0000 0601  epr__....s......
+00001160: 0a01 1401 1401 0a01 7a16 466f 616d 496e  ........z.FoamIn
+00001170: 7075 7446 696c 652e 5f5f 7265 7072 5f5f  putFile.__repr__
+00001180: 6301 0000 0000 0000 0000 0000 000b 0000  c...............
+00001190: 0008 0000 0043 0000 0073 a201 0000 6700  .....C...s....g.
+000011a0: 7d01 7c00 6a00 6400 7501 7236 6401 6701  }.|.j.d.u.r6d.g.
+000011b0: 7d02 7c00 6a00 a001 a100 4400 5d19 5c02  }.|.j.....D.].\.
+000011c0: 7d03 7d04 6402 7402 7c03 8301 1800 6403  }.}.d.t.|.....d.
+000011d0: 1400 7d05 7c02 a003 6404 7c03 9b00 7c05  ..}.|...d.|...|.
+000011e0: 9b00 7c04 9b00 6405 9d05 a101 0100 710f  ..|...d.......q.
+000011f0: 7c02 a003 6406 a101 0100 7c01 a003 6407  |...d.....|...d.
+00001200: a004 7c02 a101 a101 0100 7405 7c00 6a06  ..|.......t.|.j.
+00001210: 6408 6409 8d02 7d06 7c00 6a06 a001 a100  d.d...}.|.j.....
+00001220: 4400 5d71 5c02 7d03 7d04 7407 7c04 640a  D.]q\.}.}.t.|.d.
+00001230: 8302 725d 7c04 a008 a100 7d07 7c03 6400  ..r]|.....}.|.d.
+00001240: 7500 725c 7409 7c04 740a 8302 725c 7c07  u.r\t.|.t...r\|.
+00001250: 6405 3700 7d07 6e2f 7c04 6400 7500 7265  d.7.}.n/|.d.u.re
+00001260: 7c03 9b00 7d07 6e27 7407 7c04 640b 8302  |...}.n't.|.d...
+00001270: 726f 7c04 a00b a100 7d08 6e02 7c04 7d08  ro|.....}.n.|.}.
+00001280: 7c08 640c 6b02 7278 640c 7d05 6e0b 740c  |.d.k.rxd.}.n.t.
+00001290: 640d 7c06 7402 7c03 8301 1800 8302 6403  d.|.t.|.......d.
+000012a0: 1400 7d05 7c03 9b00 7c05 9b00 7c08 9b00  ..}.|...|...|...
+000012b0: 6405 9d04 7d07 7c00 6a0d 6400 7501 72ae  d...}.|.j.d.u.r.
+000012c0: 7c03 7c00 6a0d 7600 72ae 7c00 6a0d 7c03  |.|.j.v.r.|.j.|.
+000012d0: 1900 7d09 7409 7c09 740e 8302 72ae 640e  ..}.t.|.t...r.d.
+000012e0: 7c09 a00f 6407 640f a102 1700 7d09 7c09  |...d.d.....}.|.
+000012f0: 6407 1700 7c07 1700 7d07 7c01 a003 7c07  d...|...}.|...|.
+00001300: a101 0100 7142 6410 a004 7c01 a101 7d0a  ....qBd...|...}.
+00001310: 7c00 6a10 6400 7501 72c5 7c00 6a10 6407  |.j.d.u.r.|.j.d.
+00001320: 1700 7c0a 1700 7d0a 7c0a 6411 1900 6407  ..|...}.|.d...d.
+00001330: 6b03 72cf 7c0a 6407 3700 7d0a 7c0a 5300  k.r.|.d.7.}.|.S.
+00001340: 2912 4e7a 0a46 6f61 6d46 696c 650a 7be9  ).Nz.FoamFile.{.
+00001350: 0c00 0000 da01 20fa 0420 2020 20fa 013b  ...... ..    ..;
+00001360: da01 7dda 010a e90e 0000 0029 0172 4000  ..}........).r@.
+00001370: 0000 da04 6475 6d70 da17 6475 6d70 5f77  ....dump..dump_w
+00001380: 6974 686f 7574 5f61 7373 6967 6e6d 656e  ithout_assignmen
+00001390: 7472 1100 0000 e902 0000 007a 032f 2f20  tr.........z.// 
+000013a0: 7a04 0a2f 2f20 7a02 0a0a 7215 0000 0029  z..// z...r....)
+000013b0: 1172 6000 0000 723d 0000 0072 3500 0000  .r`...r=...r5...
+000013c0: 7228 0000 0072 2900 0000 7241 0000 0072  r(...r)...rA...r
+000013d0: 6100 0000 da07 6861 7361 7474 7272 6e00  a.....hasattrrn.
+000013e0: 0000 7232 0000 0072 3400 0000 726f 0000  ..r2...r4...ro..
+000013f0: 0072 3c00 0000 724d 0000 0072 5000 0000  .r<...rM...rP...
+00001400: da07 7265 706c 6163 6572 6200 0000 290b  ..replacerb...).
+00001410: 7245 0000 0072 6500 0000 5a04 746d 7031  rE...re...Z.tmp1
+00001420: 7237 0000 00da 046e 6f64 6572 0b00 0000  r7.....noder....
+00001430: da0a 6e75 6d5f 7370 6163 6573 da09 636f  ..num_spaces..co
+00001440: 6465 5f6e 6f64 655a 0b6e 6f64 655f 6475  de_nodeZ.node_du
+00001450: 6d70 6564 da07 636f 6d6d 656e 7472 1f00  mped..commentr..
+00001460: 0000 7222 0000 0072 2200 0000 7223 0000  ..r"...r"...r#..
+00001470: 0072 6e00 0000 9f00 0000 7348 0000 0004  .rn.......sH....
+00001480: 010a 0106 0112 0110 011c 010a 0110 010e  ................
+00001490: 0212 010a 0108 0112 0208 0102 8008 0108  ................
+000014a0: 010a 020a 0104 0208 0106 0116 0212 0114  ................
+000014b0: 010a 010a 0110 010c 010c 010a 010a 010e  ................
+000014c0: 010c 0108 0104 017a 1246 6f61 6d49 6e70  .......z.FoamInp
+000014d0: 7574 4669 6c65 2e64 756d 7063 0100 0000  utFile.dumpc....
+000014e0: 0000 0000 0000 0000 0200 0000 0800 0000  ................
+000014f0: 4300 0000 7352 0000 007c 006a 0064 0075  C...sR...|.j.d.u
+00001500: 0072 0974 0164 0183 0182 0174 027c 006a  .r.t.d.....t.|.j
+00001510: 0064 0283 028f 107d 017c 01a0 037c 00a0  .d.....}.|...|..
+00001520: 04a1 00a1 0101 0057 0064 0004 0004 0083  .......W.d......
+00001530: 0301 0064 0053 0031 0073 2277 0101 0001  ...d.S.1.s"w....
+00001540: 0001 0059 0001 0064 0053 0029 034e 7a11  ...Y...d.S.).Nz.
+00001550: 7365 6c66 2e70 6174 6820 6973 204e 6f6e  self.path is Non
+00001560: 65da 0177 2905 7263 0000 0072 3e00 0000  e..w).rc...r>...
+00001570: da04 6f70 656e da05 7772 6974 6572 6e00  ..open..writern.
+00001580: 0000 2902 7245 0000 00da 0466 696c 6572  ..).rE.....filer
+00001590: 2200 0000 7222 0000 0072 2300 0000 da09  "...r"...r#.....
+000015a0: 6f76 6572 7772 6974 65c9 0000 0073 0a00  overwrite....s..
+000015b0: 0000 0a01 0801 0e01 1001 22ff 7a17 466f  ..........".z.Fo
+000015c0: 616d 496e 7075 7446 696c 652e 6f76 6572  amInputFile.over
+000015d0: 7772 6974 6563 0300 0000 0000 0000 0000  writec..........
+000015e0: 0000 0300 0000 0300 0000 4300 0000 730e  ..........C...s.
+000015f0: 0000 007c 027c 006a 007c 013c 0064 0053  ...|.|.j.|.<.d.S
+00001600: 0072 3100 0000 2901 7261 0000 0072 5e00  .r1...).ra...r^.
+00001610: 0000 7222 0000 0072 2200 0000 7223 0000  ..r"...r"...r#..
+00001620: 0072 5700 0000 cf00 0000 f302 0000 000e  .rW.............
+00001630: 017a 1746 6f61 6d49 6e70 7574 4669 6c65  .z.FoamInputFile
+00001640: 2e5f 7365 745f 6974 656d a903 4e4e 4e29  ._set_item..NNN)
+00001650: 0872 4800 0000 7249 0000 0072 4a00 0000  .rH...rI...rJ...
+00001660: 7264 0000 0072 6600 0000 726e 0000 0072  rd...rf...rn...r
+00001670: 7b00 0000 7257 0000 0072 2200 0000 7222  {...rW...r"...r"
+00001680: 0000 0072 2200 0000 7223 0000 0072 5f00  ...r"...r#...r_.
+00001690: 0000 8e00 0000 730c 0000 0008 000a 0108  ......s.........
+000016a0: 0908 0708 2a0c 0672 5f00 0000 6300 0000  ....*..r_...c...
+000016b0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+000016c0: 0040 0000 0073 2800 0000 6500 5a01 6400  .@...s(...e.Z.d.
+000016d0: 5a02 5500 6503 6504 6401 3c00 6505 6504  Z.U.e.e.d.<.e.e.
+000016e0: 6402 3c00 6407 6404 6405 8401 5a06 6406  d.<.d.d.d...Z.d.
+000016f0: 5300 2908 da0a 4173 7369 676e 6d65 6e74  S.)...Assignment
+00001700: 724e 0000 0072 3800 0000 7201 0000 0063  rN...r8...r....c
+00001710: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00001720: 0500 0000 4300 0000 7334 0000 0074 007c  ....C...s4...t.|
+00001730: 006a 0164 0183 0272 0c7c 006a 01a0 027c  .j.d...r.|.j...|
+00001740: 01a1 0153 007c 0164 0214 007c 006a 039b  ...S.|.d...|.j..
+00001750: 0064 037c 006a 019b 0064 049d 0417 0053  .d.|.j...d.....S
+00001760: 00a9 054e 726e 0000 0072 6800 0000 fa02  ...Nrn...rh.....
+00001770: 2020 726a 0000 0029 0472 7100 0000 7238    rj...).rq...r8
+00001780: 0000 0072 6e00 0000 724e 0000 00a9 0272  ...rn...rN.....r
+00001790: 4500 0000 da06 696e 6465 6e74 7222 0000  E.....indentr"..
+000017a0: 0072 2200 0000 7223 0000 0072 6e00 0000  .r"...r#...rn...
+000017b0: d800 0000 7306 0000 000c 010c 011c 027a  ....s..........z
+000017c0: 0f41 7373 6967 6e6d 656e 742e 6475 6d70  .Assignment.dump
+000017d0: 4ea9 0172 0100 0000 2907 7248 0000 0072  N..r....).rH...r
+000017e0: 4900 0000 724a 0000 0072 5000 0000 da0f  I...rJ...rP.....
+000017f0: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5fda  __annotations__.
+00001800: 066f 626a 6563 7472 6e00 0000 7222 0000  .objectrn...r"..
+00001810: 0072 2200 0000 7222 0000 0072 2300 0000  .r"...r"...r#...
+00001820: 727e 0000 00d3 0000 0073 0800 0000 0a00  r~.......s......
+00001830: 0802 0801 0e02 727e 0000 0063 0000 0000  ......r~...c....
+00001840: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00001850: 0000 0000 7326 0000 0065 005a 0164 005a  ....s&...e.Z.d.Z
+00001860: 0287 0066 0164 0164 0284 085a 0364 0664  ...f.d.d...Z.d.d
+00001870: 0464 0584 015a 0487 0004 005a 0553 0029  .d...Z.....Z.S.)
+00001880: 07da 1256 6172 6961 626c 6541 7373 6967  ...VariableAssig
+00001890: 6e6d 656e 7463 0100 0000 0000 0000 0000  nmentc..........
+000018a0: 0000 0200 0000 0200 0000 0300 0000 730e  ..............s.
+000018b0: 0000 0074 0083 00a0 01a1 007d 017c 0153  ...t.......}.|.S
+000018c0: 0072 3100 0000 a902 da05 7375 7065 7272  .r1.......superr
+000018d0: 6600 0000 2902 7245 0000 0072 0b00 0000  f...).rE...r....
+000018e0: a901 da09 5f5f 636c 6173 735f 5f72 2200  ....__class__r".
+000018f0: 0000 7223 0000 0072 6600 0000 e000 0000  ..r#...rf.......
+00001900: 7304 0000 000a 0104 017a 1b56 6172 6961  s........z.Varia
+00001910: 626c 6541 7373 6967 6e6d 656e 742e 5f5f  bleAssignment.__
+00001920: 7265 7072 5f5f 7201 0000 0063 0200 0000  repr__r....c....
+00001930: 0000 0000 0000 0000 0200 0000 0600 0000  ................
+00001940: 4300 0000 734a 0000 0074 007c 006a 0164  C...sJ...t.|.j.d
+00001950: 0183 0272 177c 0164 0214 007c 006a 029b  ...r.|.d...|.j..
+00001960: 0064 037c 006a 01a0 037c 01a1 019b 0064  .d.|.j...|.....d
+00001970: 049d 0417 0053 007c 0164 0214 007c 006a  .....S.|.d...|.j
+00001980: 029b 0064 037c 006a 019b 0064 049d 0417  ...d.|.j...d....
+00001990: 0053 0072 7f00 0000 2904 7271 0000 0072  .S.r....).rq...r
+000019a0: 3800 0000 724e 0000 0072 6e00 0000 7281  8...rN...rn...r.
+000019b0: 0000 0072 2200 0000 7222 0000 0072 2300  ...r"...r"...r#.
+000019c0: 0000 726e 0000 00e4 0000 0073 0600 0000  ..rn.......s....
+000019d0: 0c01 2201 1c02 7a17 5661 7269 6162 6c65  .."...z.Variable
+000019e0: 4173 7369 676e 6d65 6e74 2e64 756d 7072  Assignment.dumpr
+000019f0: 8300 0000 2906 7248 0000 0072 4900 0000  ....).rH...rI...
+00001a00: 724a 0000 0072 6600 0000 726e 0000 00da  rJ...rf...rn....
+00001a10: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7222  .__classcell__r"
+00001a20: 0000 0072 2200 0000 7289 0000 0072 2300  ...r"...r....r#.
+00001a30: 0000 7286 0000 00df 0000 0073 0600 0000  ..r........s....
+00001a40: 0800 0c01 1204 7286 0000 0063 0000 0000  ......r....c....
+00001a50: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00001a60: 4000 0000 f328 0000 0065 005a 0164 005a  @....(...e.Z.d.Z
+00001a70: 0264 0964 0264 0384 015a 0364 0464 0584  .d.d.d...Z.d.d..
+00001a80: 005a 0464 0a64 0764 0884 015a 0564 0153  .Z.d.d.d...Z.d.S
+00001a90: 0029 0b72 5d00 0000 4e63 0400 0000 0000  .).r]...Nc......
+00001aa0: 0000 0000 0000 0400 0000 0400 0000 4300  ..............C.
+00001ab0: 0000 732c 0000 007c 017c 005f 007c 027c  ..s,...|.|._.|.|
+00001ac0: 005f 0174 027c 0374 0374 0466 0283 0272  ._.t.|.t.t.f...r
+00001ad0: 1174 057c 0383 017d 037c 037c 005f 0664  .t.|...}.|.|._.d
+00001ae0: 0053 0072 3100 0000 2907 7238 0000 0072  .S.r1...).r8...r
+00001af0: 4e00 0000 7232 0000 0072 5200 0000 da05  N...r2...rR.....
+00001b00: 7475 706c 6572 2f00 0000 7259 0000 0029  tupler/...rY...)
+00001b10: 0472 4500 0000 7238 0000 0072 4e00 0000  .rE...r8...rN...
+00001b20: 7259 0000 0072 2200 0000 7222 0000 0072  rY...r"...r"...r
+00001b30: 2300 0000 7264 0000 00ed 0000 0073 0a00  #...rd.......s..
+00001b40: 0000 0601 0601 0e01 0801 0a01 7a0e 5661  ............z.Va
+00001b50: 6c75 652e 5f5f 696e 6974 5f5f 6301 0000  lue.__init__c...
+00001b60: 0000 0000 0000 0000 0001 0000 0007 0000  ................
+00001b70: 0043 0000 0073 9400 0000 7c00 6a00 6400  .C...s....|.j.d.
+00001b80: 7501 7219 7c00 6a01 6400 7501 7219 6401  u.r.|.j.d.u.r.d.
+00001b90: 7c00 6a02 9b00 6402 7c00 6a01 9b00 6403  |.j...d.|.j...d.
+00001ba0: 7c00 6a00 9b00 6404 9d07 5300 7c00 6a00  |.j...d...S.|.j.
+00001bb0: 6400 7500 722e 7c00 6a01 6400 7501 722e  d.u.r.|.j.d.u.r.
+00001bc0: 6401 7c00 6a02 9b00 6402 7c00 6a01 9b00  d.|.j...d.|.j...
+00001bd0: 6404 9d05 5300 7c00 6a00 6400 7501 7243  d...S.|.j.d.u.rC
+00001be0: 7c00 6a01 6400 7500 7243 6401 7c00 6a02  |.j.d.u.rCd.|.j.
+00001bf0: 9b00 6405 7c00 6a00 9b00 6404 9d05 5300  ..d.|.j...d...S.
+00001c00: 6401 7c00 6a02 9b00 6406 9d03 5300 2907  d.|.j...d...S.).
+00001c10: 4e7a 0656 616c 7565 287a 082c 206e 616d  Nz.Value(z., nam
+00001c20: 653d 227a 0e22 2c20 6469 6d65 6e73 696f  e="z.", dimensio
+00001c30: 6e3d 227a 0222 297a 0d2c 2064 696d 656e  n="z.")z., dimen
+00001c40: 7369 6f6e 3d22 fa01 2929 0372 5900 0000  sion="..)).rY...
+00001c50: 724e 0000 0072 3800 0000 a901 7245 0000  rN...r8.....rE..
+00001c60: 0072 2200 0000 7222 0000 0072 2300 0000  .r"...r"...r#...
+00001c70: 7266 0000 00f4 0000 0073 0e00 0000 1401  rf.......s......
+00001c80: 1e01 1401 1601 1401 1601 0e02 7a0e 5661  ............z.Va
+00001c90: 6c75 652e 5f5f 7265 7072 5f5f 7201 0000  lue.__repr__r...
+00001ca0: 0063 0200 0000 0000 0000 0000 0000 0500  .c..............
+00001cb0: 0000 0500 0000 4300 0000 73ce 0000 007c  ......C...s....|
+00001cc0: 006a 0064 0075 0172 1474 017c 006a 0083  .j.d.u.r.t.|.j..
+00001cd0: 017d 0264 01a0 0264 0264 0384 007c 0244  .}.d...d.d...|.D
+00001ce0: 0083 01a1 017d 0374 037c 006a 0474 0583  .....}.t.|.j.t..
+00001cf0: 0272 2674 067c 006a 0464 0483 0272 267c  .r&t.|.j.d...r&|
+00001d00: 006a 04a0 07a1 007d 046e 0574 087c 006a  .j.....}.n.t.|.j
+00001d10: 0483 017d 047c 006a 0064 0075 0172 407c  ...}.|.j.d.u.r@|
+00001d20: 006a 0964 0075 0172 407c 006a 099b 0064  .j.d.u.r@|.j...d
+00001d30: 057c 039b 0064 067c 049b 009d 0553 007c  .|...d.|.....S.|
+00001d40: 006a 0064 0075 0072 527c 006a 0964 0075  .j.d.u.rR|.j.d.u
+00001d50: 0172 527c 006a 099b 0064 017c 049b 009d  .rR|.j...d.|....
+00001d60: 0353 007c 006a 0064 0075 0172 647c 006a  .S.|.j.d.u.rd|.j
+00001d70: 0964 0075 0072 6464 077c 039b 0064 067c  .d.u.rdd.|...d.|
+00001d80: 049b 009d 0453 007c 049b 0053 0029 084e  .....S.|...S.).N
+00001d90: 7268 0000 0063 0100 0000 0000 0000 0000  rh...c..........
+00001da0: 0000 0200 0000 0300 0000 7300 0000 f318  ..........s.....
+00001db0: 0000 0081 007c 005d 077d 0174 007c 0183  .....|.].}.t.|..
+00001dc0: 0156 0001 0071 0264 0053 0072 3100 0000  .V...q.d.S.r1...
+00001dd0: a901 7250 0000 00a9 0272 3600 0000 da06  ..rP.....r6.....
+00001de0: 6e75 6d62 6572 7222 0000 0072 2200 0000  numberr"...r"...
+00001df0: 7223 0000 0072 3900 0000 0101 0000 f304  r#...r9.........
+00001e00: 0000 0002 8016 007a 3056 616c 7565 2e64  .......z0Value.d
+00001e10: 756d 705f 7769 7468 6f75 745f 6173 7369  ump_without_assi
+00001e20: 676e 6d65 6e74 2e3c 6c6f 6361 6c73 3e2e  gnment.<locals>.
+00001e30: 3c67 656e 6578 7072 3e72 6e00 0000 7a02  <genexpr>rn...z.
+00001e40: 205b 7a02 5d20 fa01 5b29 0a72 5900 0000   [z.] ..[).rY...
+00001e50: 7224 0000 0072 2900 0000 7232 0000 0072  r$...r)...r2...r
+00001e60: 3800 0000 7242 0000 0072 7100 0000 726e  8...rB...rq...rn
+00001e70: 0000 0072 5000 0000 724e 0000 0029 0572  ...rP...rN...).r
+00001e80: 4500 0000 7282 0000 005a 0e64 696d 656e  E...r....Z.dimen
+00001e90: 7369 6f6e 5f6c 6973 745a 1064 696d 656e  sion_listZ.dimen
+00001ea0: 7369 6f6e 5f64 756d 7065 645a 0c76 616c  sion_dumpedZ.val
+00001eb0: 7565 5f64 756d 7065 6472 2200 0000 7222  ue_dumpedr"...r"
+00001ec0: 0000 0072 2300 0000 726f 0000 00fe 0000  ...r#...ro......
+00001ed0: 0073 1a00 0000 0a01 0a01 1401 1802 0c01  .s..............
+00001ee0: 0a02 1402 1601 1401 1001 1401 1001 0602  ................
+00001ef0: 7a1d 5661 6c75 652e 6475 6d70 5f77 6974  z.Value.dump_wit
+00001f00: 686f 7574 5f61 7373 6967 6e6d 656e 74a9  hout_assignment.
+00001f10: 024e 4e72 8300 0000 2906 7248 0000 0072  .NNr....).rH...r
+00001f20: 4900 0000 724a 0000 0072 6400 0000 7266  I...rJ...rd...rf
+00001f30: 0000 0072 6f00 0000 7222 0000 0072 2200  ...ro...r"...r".
+00001f40: 0000 7222 0000 0072 2300 0000 725d 0000  ..r"...r#...r]..
+00001f50: 00eb 0000 0073 0800 0000 0800 0a02 0807  .....s..........
+00001f60: 0e0a 725d 0000 0063 0000 0000 0000 0000  ..r]...c........
+00001f70: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+00001f80: 732e 0000 0065 005a 0164 005a 0287 0066  s....e.Z.d.Z...f
+00001f90: 0164 0164 0284 085a 0364 0364 0484 005a  .d.d...Z.d.d...Z
+00001fa0: 0464 0864 0664 0784 015a 0587 0004 005a  .d.d.d...Z.....Z
+00001fb0: 0653 0029 09da 0c44 696d 656e 7369 6f6e  .S.)...Dimension
+00001fc0: 5365 7463 0200 0000 0000 0000 0000 0000  Setc............
+00001fd0: 0200 0000 0300 0000 0300 0000 732a 0000  ............s*..
+00001fe0: 0074 0064 0164 0284 007c 0144 0083 0183  .t.d.d...|.D....
+00001ff0: 0173 0d74 0164 0383 0182 0174 0283 00a0  .s.t.d.....t....
+00002000: 037c 01a1 0101 0064 0053 0029 044e 6301  .|.....d.S.).Nc.
+00002010: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00002020: 0000 0073 0000 0073 1a00 0000 8100 7c00  ...s...s......|.
+00002030: 5d08 7d01 7400 7c01 7401 8302 5600 0100  ].}.t.|.t...V...
+00002040: 7102 6400 5300 7231 0000 0029 0272 3200  q.d.S.r1...).r2.
+00002050: 0000 721b 0000 0029 0272 3600 0000 da04  ..r....).r6.....
+00002060: 656c 656d 7222 0000 0072 2200 0000 7223  elemr"...r"...r#
+00002070: 0000 0072 3900 0000 1401 0000 f304 0000  ...r9...........
+00002080: 0002 8018 007a 2844 696d 656e 7369 6f6e  .....z(Dimension
+00002090: 5365 742e 5f5f 696e 6974 5f5f 2e3c 6c6f  Set.__init__.<lo
+000020a0: 6361 6c73 3e2e 3c67 656e 6578 7072 3e7a  cals>.<genexpr>z
+000020b0: 1342 6164 207b 666f 616d 5f75 6e69 7473  .Bad {foam_units
+000020c0: 203d 207d 2904 da03 616c 6c72 3e00 0000   = })...allr>...
+000020d0: 7288 0000 0072 6400 0000 2902 7245 0000  r....rd...).rE..
+000020e0: 0072 2b00 0000 7289 0000 0072 2200 0000  .r+...r....r"...
+000020f0: 7223 0000 0072 6400 0000 1301 0000 7306  r#...rd.......s.
+00002100: 0000 0012 0108 0110 017a 1544 696d 656e  .........z.Dimen
+00002110: 7369 6f6e 5365 742e 5f5f 696e 6974 5f5f  sionSet.__init__
+00002120: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00002130: 0002 0000 0043 0000 0073 0800 0000 7400  .....C...s....t.
+00002140: 7c00 8301 5300 7231 0000 0029 0172 2f00  |...S.r1...).r/.
+00002150: 0000 728f 0000 0072 2200 0000 7222 0000  ..r....r"...r"..
+00002160: 0072 2300 0000 7266 0000 0018 0100 00f3  .r#...rf........
+00002170: 0200 0000 0801 7a15 4469 6d65 6e73 696f  ......z.Dimensio
+00002180: 6e53 6574 2e5f 5f72 6570 725f 5f72 0100  nSet.__repr__r..
+00002190: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
+000021a0: 0000 0005 0000 0043 0000 0073 1c00 0000  .......C...s....
+000021b0: 6401 6402 a000 6403 6404 8400 7c00 4400  d.d...d.d...|.D.
+000021c0: 8301 a101 1700 6405 1700 5300 2906 4e72  ......d...S.).Nr
+000021d0: 9500 0000 7268 0000 0063 0100 0000 0000  ....rh...c......
+000021e0: 0000 0000 0000 0200 0000 0300 0000 7300  ..............s.
+000021f0: 0000 7290 0000 0072 3100 0000 7291 0000  ..r....r1...r...
+00002200: 0072 9200 0000 7222 0000 0072 2200 0000  .r....r"...r"...
+00002210: 7223 0000 0072 3900 0000 1c01 0000 7294  r#...r9.......r.
+00002220: 0000 007a 3744 696d 656e 7369 6f6e 5365  ...z7DimensionSe
+00002230: 742e 6475 6d70 5f77 6974 686f 7574 5f61  t.dump_without_a
+00002240: 7373 6967 6e6d 656e 742e 3c6c 6f63 616c  ssignment.<local
+00002250: 733e 2e3c 6765 6e65 7870 723e fa01 5da9  s>.<genexpr>..].
+00002260: 0172 2900 0000 7281 0000 0072 2200 0000  .r)...r....r"...
+00002270: 7222 0000 0072 2300 0000 726f 0000 001b  r"...r#...ro....
+00002280: 0100 00f3 0200 0000 1c01 7a24 4469 6d65  ..........z$Dime
+00002290: 6e73 696f 6e53 6574 2e64 756d 705f 7769  nsionSet.dump_wi
+000022a0: 7468 6f75 745f 6173 7369 676e 6d65 6e74  thout_assignment
+000022b0: 7283 0000 0029 0772 4800 0000 7249 0000  r....).rH...rI..
+000022c0: 0072 4a00 0000 7264 0000 0072 6600 0000  .rJ...rd...rf...
+000022d0: 726f 0000 0072 8b00 0000 7222 0000 0072  ro...r....r"...r
+000022e0: 2200 0000 7289 0000 0072 2300 0000 7297  "...r....r#...r.
+000022f0: 0000 0012 0100 0073 0800 0000 0800 0c01  .......s........
+00002300: 0805 1203 7297 0000 0063 0000 0000 0000  ....r....c......
+00002310: 0000 0000 0000 0000 0000 0400 0000 0000  ................
+00002320: 0000 7344 0000 0065 005a 0164 005a 0264  ..sD...e.Z.d.Z.d
+00002330: 0d87 0066 0164 0264 0384 095a 0364 0464  ...f.d.d...Z.d.d
+00002340: 0584 005a 0487 0066 0164 0664 0784 085a  ...Z...f.d.d...Z
+00002350: 0564 0e64 0964 0a84 015a 0664 0b64 0c84  .d.d.d...Z.d.d..
+00002360: 005a 0787 0004 005a 0853 0029 0f72 3300  .Z.....Z.S.).r3.
+00002370: 0000 4e63 0500 0000 0000 0000 0000 0000  ..Nc............
+00002380: 0500 0000 0400 0000 0300 0000 7328 0000  ............s(..
+00002390: 007c 027c 005f 007c 037c 005f 017c 047c  .|.|._.|.|._.|.|
+000023a0: 005f 0274 0383 006a 0464 0169 007c 01a4  ._.t...j.d.i.|..
+000023b0: 018e 0101 0064 0053 0029 024e 7222 0000  .....d.S.).Nr"..
+000023c0: 0029 05da 055f 6e61 6d65 da0a 5f64 6972  .)..._name.._dir
+000023d0: 6563 7469 7665 724d 0000 0072 8800 0000  ectiverM...r....
+000023e0: 7264 0000 0029 0572 4500 0000 723f 0000  rd...).rE...r?..
+000023f0: 0072 4e00 0000 da09 6469 7265 6374 6976  .rN.....directiv
+00002400: 6572 4d00 0000 7289 0000 0072 2200 0000  erM...r....r"...
+00002410: 7223 0000 0072 6400 0000 2001 0000 7308  r#...rd... ...s.
+00002420: 0000 0006 0106 0106 0116 017a 0d44 6963  ...........z.Dic
+00002430: 742e 5f5f 696e 6974 5f5f 6301 0000 0000  t.__init__c.....
+00002440: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+00002450: 0000 00f3 0600 0000 7c00 6a00 5300 7231  ........|.j.S.r1
+00002460: 0000 00a9 0172 9f00 0000 728f 0000 0072  .....r....r....r
+00002470: 2200 0000 7222 0000 0072 2300 0000 da08  "...r"...r#.....
+00002480: 6765 745f 6e61 6d65 2601 0000 f302 0000  get_name&.......
+00002490: 0006 017a 0d44 6963 742e 6765 745f 6e61  ...z.Dict.get_na
+000024a0: 6d65 6301 0000 0000 0000 0000 0000 0001  mec.............
+000024b0: 0000 0002 0000 0003 0000 00f3 0a00 0000  ................
+000024c0: 7400 8300 a001 a100 5300 7231 0000 0072  t.......S.r1...r
+000024d0: 8700 0000 728f 0000 0072 8900 0000 7222  ....r....r....r"
+000024e0: 0000 0072 2300 0000 7266 0000 0029 0100  ...r#...rf...)..
+000024f0: 00f3 0200 0000 0a01 7a0d 4469 6374 2e5f  ........z.Dict._
+00002500: 5f72 6570 725f 5f72 0100 0000 6302 0000  _repr__r....c...
+00002510: 0000 0000 0000 0000 000b 0000 0009 0000  ................
+00002520: 0043 0000 0073 5401 0000 6700 7d02 7c01  .C...sT...g.}.|.
+00002530: 6401 1400 7d03 7c00 6a00 6400 7501 7228  d...}.|.j.d.u.r(
+00002540: 7c03 7c00 6a00 1700 7d04 7c00 6a01 6400  |.|.j...}.|.j.d.
+00002550: 7501 721c 7c04 6402 7c00 6a01 1700 3700  u.r.|.d.|.j...7.
+00002560: 7d04 7c02 a002 7c04 6403 7c03 9b00 9d02  }.|...|.d.|.....
+00002570: 1700 6404 1700 a101 0100 7403 7c00 8301  ..d.......t.|...
+00002580: 7d05 7c00 a004 a100 4400 5d60 5c02 7d06  }.|.....D.]`\.}.
+00002590: 7d07 7c00 6a05 6400 7501 7253 7c06 7c00  }.|.j.d.u.rS|.|.
+000025a0: 6a05 7600 7253 7c00 6a05 7c06 1900 7d08  j.v.rS|.j.|...}.
+000025b0: 7406 7c08 7407 8302 7253 7c02 a002 6405  t.|.t...rS|...d.
+000025c0: 7c08 a008 6403 6406 a102 1700 a101 0100  |...d.d.........
+000025d0: 7409 7c07 6407 8302 7263 7c02 a002 7c07  t.|.d...rc|...|.
+000025e0: a00a 7c01 6408 1700 a101 a101 0100 7130  ..|.d.........q0
+000025f0: 7409 7c07 6409 8302 726d 7c07 a00b a100  t.|.d...rm|.....
+00002600: 7d09 6e02 7c07 7d09 7c07 640a 6b02 7276  }.n.|.}.|.d.k.rv
+00002610: 640a 7d0a 6e0b 740c 640b 7c05 740d 7c06  d.}.n.t.d.|.t.|.
+00002620: 8301 1800 8302 6401 1400 7d0a 7c02 a002  ......d...}.|...
+00002630: 7c03 640c 7c06 9b00 7c0a 9b00 7c09 9b00  |.d.|...|...|...
+00002640: 640d 9d05 1700 a101 0100 7130 7c02 a002  d.........q0|...
+00002650: 7c03 640e 1700 a101 0100 7406 7c00 740e  |.d.......t.|.t.
+00002660: 8302 72a5 7c02 640f 0500 1900 640d 3700  ..r.|.d.....d.7.
+00002670: 0300 3c00 6403 a00f 7c02 a101 5300 2910  ..<.d...|...S.).
+00002680: 4e72 6800 0000 7280 0000 0072 6c00 0000  Nrh...r....rl...
+00002690: da01 7b7a 0720 2020 202f 2f20 7a08 0a20  ..{z.    // z.. 
+000026a0: 2020 202f 2f20 726e 0000 0072 3a00 0000     // rn...r:...
+000026b0: 726f 0000 0072 1100 0000 7270 0000 0072  ro...r....rp...r
+000026c0: 6900 0000 726a 0000 0072 6b00 0000 7215  i...rj...rk...r.
+000026d0: 0000 0029 1072 9f00 0000 72a0 0000 0072  ...).r....r....r
+000026e0: 2800 0000 7241 0000 0072 3d00 0000 724d  (...rA...r=...rM
+000026f0: 0000 0072 3200 0000 7250 0000 0072 7200  ...r2...rP...rr.
+00002700: 0000 7271 0000 0072 6e00 0000 726f 0000  ..rq...rn...ro..
+00002710: 0072 3c00 0000 7235 0000 00da 0a43 6f64  .r<...r5.....Cod
+00002720: 6553 7472 6561 6d72 2900 0000 290b 7245  eStreamr)...).rE
+00002730: 0000 0072 8200 0000 7265 0000 00da 0b69  ...r....re.....i
+00002740: 6e64 656e 7461 7469 6f6e da04 6c69 6e65  ndentation..line
+00002750: 7274 0000 0072 3700 0000 7273 0000 0072  rt...r7...rs...r
+00002760: 7600 0000 7275 0000 0072 0b00 0000 7222  v...ru...r....r"
+00002770: 0000 0072 2200 0000 7223 0000 0072 6e00  ...r"...r#...rn.
+00002780: 0000 2c01 0000 7334 0000 0004 0108 010a  ..,...s4........
+00002790: 010a 010a 010e 0118 0108 0210 0114 010a  ................
+000027a0: 010a 0116 010a 0216 010a 020a 0104 0208  ................
+000027b0: 0106 0116 0220 010e 010a 0310 010a 027a  ..... .........z
+000027c0: 0944 6963 742e 6475 6d70 6303 0000 0000  .Dict.dumpc.....
+000027d0: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
+000027e0: 0000 0073 0c00 0000 7c02 7c00 7c01 3c00  ...s....|.|.|.<.
+000027f0: 6400 5300 7231 0000 0072 2200 0000 725e  d.S.r1...r"...r^
+00002800: 0000 0072 2200 0000 7222 0000 0072 2300  ...r"...r"...r#.
+00002810: 0000 7257 0000 0050 0100 0073 0200 0000  ..rW...P...s....
+00002820: 0c01 7a0e 4469 6374 2e5f 7365 745f 6974  ..z.Dict._set_it
+00002830: 656d 727d 0000 0072 8300 0000 2909 7248  emr}...r....).rH
+00002840: 0000 0072 4900 0000 724a 0000 0072 6400  ...rI...rJ...rd.
+00002850: 0000 72a4 0000 0072 6600 0000 726e 0000  ..r....rf...rn..
+00002860: 0072 5700 0000 728b 0000 0072 2200 0000  .rW...r....r"...
+00002870: 7222 0000 0072 8900 0000 7223 0000 0072  r"...r....r#...r
+00002880: 3300 0000 1f01 0000 730c 0000 0008 000e  3.......s.......
+00002890: 0108 060c 030a 0310 2472 3300 0000 6300  ........$r3...c.
+000028a0: 0000 0000 0000 0000 0000 0000 0000 0004  ................
+000028b0: 0000 0000 0000 0073 5a00 0000 6500 5a01  .......sZ...e.Z.
+000028c0: 6400 5a02 6401 5a03 6412 8700 6601 6403  d.Z.d.Z.d...f.d.
+000028d0: 6404 8409 5a04 6405 6406 8400 5a05 6407  d...Z.d.d...Z.d.
+000028e0: 6408 8400 5a06 8700 6601 6409 640a 8408  d...Z...f.d.d...
+000028f0: 5a07 640b 640c 8400 5a08 6413 640e 640f  Z.d.d...Z.d.d.d.
+00002900: 8401 5a09 6413 6410 6411 8401 5a0a 8700  ..Z.d.d.d...Z...
+00002910: 0400 5a0b 5300 2914 7234 0000 007a 1b52  ..Z.S.).r4...z.R
+00002920: 6570 7265 7365 6e74 7320 616e 204f 7065  epresents an Ope
+00002930: 6e46 6f61 6d20 6c69 7374 4e63 0300 0000  nFoam listNc....
+00002940: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+00002950: 0300 0000 7316 0000 007c 027c 005f 0074  ....s....|.|._.t
+00002960: 0183 00a0 027c 01a1 0101 0064 0053 0072  .....|.....d.S.r
+00002970: 3100 0000 2903 729f 0000 0072 8800 0000  1...).r....r....
+00002980: 7264 0000 0029 0372 4500 0000 da08 6974  rd...).rE.....it
+00002990: 6572 6162 6c65 724e 0000 0072 8900 0000  erablerN...r....
+000029a0: 7222 0000 0072 2300 0000 7264 0000 0057  r"...r#...rd...W
+000029b0: 0100 0073 0400 0000 0601 1001 7a0d 4c69  ...s........z.Li
+000029c0: 7374 2e5f 5f69 6e69 745f 5f63 0100 0000  st.__init__c....
+000029d0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+000029e0: 4300 0000 72a2 0000 0072 3100 0000 72a3  C...r....r1...r.
+000029f0: 0000 0072 8f00 0000 7222 0000 0072 2200  ...r....r"...r".
+00002a00: 0000 7223 0000 0072 a400 0000 5b01 0000  ..r#...r....[...
+00002a10: 72a5 0000 007a 0d4c 6973 742e 6765 745f  r....z.List.get_
+00002a20: 6e61 6d65 6302 0000 0000 0000 0000 0000  namec...........
+00002a30: 0002 0000 0003 0000 0043 0000 0073 4800  .........C...sH.
+00002a40: 0000 7c00 6a00 6400 7500 720a 7c01 7c00  ..|.j.d.u.r.|.|.
+00002a50: 5f00 6400 5300 7401 7c00 6a00 7402 8302  _.d.S.t.|.j.t...
+00002a60: 7221 7c00 6a00 7c01 6b03 721f 7c01 6401  r!|.j.|.k.r.|.d.
+00002a70: 1700 7c00 6a00 1700 7c00 5f00 6400 5300  ..|.j...|._.d.S.
+00002a80: 6400 5300 7403 8300 8201 2902 4e72 6800  d.S.t.....).Nrh.
+00002a90: 0000 2904 729f 0000 0072 3200 0000 7250  ..).r....r2...rP
+00002aa0: 0000 00da 0c52 756e 7469 6d65 4572 726f  .....RuntimeErro
+00002ab0: 7229 0272 4500 0000 724e 0000 0072 2200  r).rE...rN...r".
+00002ac0: 0000 7222 0000 0072 2300 0000 da08 6164  ..r"...r#.....ad
+00002ad0: 645f 6e61 6d65 5e01 0000 730e 0000 000a  d_name^...s.....
+00002ae0: 010a 010c 010a 0114 0104 ff06 037a 0d4c  .............z.L
+00002af0: 6973 742e 6164 645f 6e61 6d65 6301 0000  ist.add_namec...
+00002b00: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00002b10: 0003 0000 0072 a600 0000 7231 0000 0072  .....r....r1...r
+00002b20: 8700 0000 728f 0000 0072 8900 0000 7222  ....r....r....r"
+00002b30: 0000 0072 2300 0000 7266 0000 0067 0100  ...r#...rf...g..
+00002b40: 0072 a700 0000 7a0d 4c69 7374 2e5f 5f72  .r....z.List.__r
+00002b50: 6570 725f 5f63 0200 0000 0000 0000 0000  epr__c..........
+00002b60: 0000 0200 0000 0300 0000 0300 0000 7314  ..............s.
+00002b70: 0000 0087 0087 0166 0264 0164 0284 0888  .......f.d.d....
+00002b80: 0144 0083 0153 0029 034e 6301 0000 0000  .D...S.).Nc.....
+00002b90: 0000 0000 0000 0002 0000 0006 0000 0013  ................
+00002ba0: 0000 0073 1800 0000 6700 7c00 5d08 7d01  ...s....g.|.].}.
+00002bb0: 8801 a000 7c01 8800 a102 9102 7102 5300  ....|.......q.S.
+00002bc0: 7222 0000 00a9 01da 0a5f 6475 6d70 5f69  r"......._dump_i
+00002bd0: 7465 6d29 0272 3600 0000 da04 6974 656d  tem).r6.....item
+00002be0: a902 7282 0000 0072 4500 0000 7222 0000  ..r....rE...r"..
+00002bf0: 0072 2300 0000 da0a 3c6c 6973 7463 6f6d  .r#.....<listcom
+00002c00: 703e 6b01 0000 7302 0000 0018 007a 2b4c  p>k...s......z+L
+00002c10: 6973 742e 5f6d 616b 655f 6c69 7374 5f73  ist._make_list_s
+00002c20: 7472 696e 6773 2e3c 6c6f 6361 6c73 3e2e  trings.<locals>.
+00002c30: 3c6c 6973 7463 6f6d 703e 7222 0000 0072  <listcomp>r"...r
+00002c40: 8100 0000 7222 0000 0072 b200 0000 7223  ....r"...r....r#
+00002c50: 0000 00da 125f 6d61 6b65 5f6c 6973 745f  ....._make_list_
+00002c60: 7374 7269 6e67 736a 0100 0073 0200 0000  stringsj...s....
+00002c70: 1401 7a17 4c69 7374 2e5f 6d61 6b65 5f6c  ..z.List._make_l
+00002c80: 6973 745f 7374 7269 6e67 7372 0100 0000  ist_stringsr....
+00002c90: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+00002ca0: 0004 0000 0043 0000 0073 3200 0000 7400  .....C...s2...t.
+00002cb0: 7c01 7401 7402 6602 8302 7211 7403 7c01  |.t.t.f...r.t.|.
+00002cc0: 6401 8302 7211 7c01 a004 7c02 a101 5300  d...r.|...|...S.
+00002cd0: 7c02 6402 1400 7405 7c01 8301 1700 5300  |.d...t.|.....S.
+00002ce0: 2903 4e72 6e00 0000 7268 0000 0029 0672  ).Nrn...rh...).r
+00002cf0: 3200 0000 7242 0000 0072 7e00 0000 7271  2...rB...r~...rq
+00002d00: 0000 0072 6e00 0000 7250 0000 0029 0372  ...rn...rP...).r
+00002d10: 4500 0000 72b1 0000 0072 8200 0000 7222  E...r....r....r"
+00002d20: 0000 0072 2200 0000 7223 0000 0072 b000  ...r"...r#...r..
+00002d30: 0000 6d01 0000 7306 0000 0018 010a 0110  ..m...s.........
+00002d40: 027a 0f4c 6973 742e 5f64 756d 705f 6974  .z.List._dump_it
+00002d50: 656d 6302 0000 0000 0000 0000 0000 0009  emc.............
+00002d60: 0000 0008 0000 0003 0000 0073 3c01 0000  ...........s<...
+00002d70: 6700 7d02 8800 6401 1400 7d03 8801 6a00  g.}...d...}...j.
+00002d80: 6400 7500 721f 7c02 a001 8801 6a02 6402  d.u.r.|.....j.d.
+00002d90: 6403 8d01 a101 0100 7c03 6404 1700 6401  d.......|.d...d.
+00002da0: a003 7c02 a101 1700 6405 1700 5300 7c02  ..|.....d...S.|.
+00002db0: a004 7c03 8801 6a00 1700 6406 7c03 9b00  ..|...j...d.|...
+00002dc0: 9d02 1700 6404 1700 a101 0100 6407 6408  ....d.......d.d.
+00002dd0: 6409 9c02 7d04 8801 6a00 7c04 a005 a100  d...}...j.|.....
+00002de0: 7601 7248 7c02 a004 6406 a003 8801 a002  v.rH|...d.......
+00002df0: 8800 640a 1700 a101 a101 a101 0100 6e4a  ..d...........nJ
+00002e00: 8801 7292 7c04 8801 6a00 1900 7d05 8801  ..r.|...j...}...
+00002e10: 6402 1900 7c05 6b02 7359 7406 8801 8301  d...|.k.sYt.....
+00002e20: 8201 6700 7d06 6400 7d07 8801 4400 5d18  ..g.}.d.}...D.].
+00002e30: 7d08 7c08 7c05 6b02 7272 7c07 6400 7501  }.|.|.k.rr|.d.u.
+00002e40: 726e 7c06 a004 7c07 a101 0100 7c08 6701  rn|...|.....|.g.
+00002e50: 7d07 715f 7c07 a004 7c08 a101 0100 715f  }.q_|...|.....q_
+00002e60: 7c06 a004 7c07 a101 0100 8701 6601 640b  |...|.......f.d.
+00002e70: 640c 8408 7c06 4400 8301 7d06 7c02 a001  d...|.D...}.|...
+00002e80: 8700 6601 640d 640e 8408 7c06 4400 8301  ..f.d.d...|.D...
+00002e90: a101 0100 7c02 a004 7c03 640f 1700 a101  ....|...|.d.....
+00002ea0: 0100 6406 a003 7c02 a101 5300 2910 4e72  ..d...|...S.).Nr
+00002eb0: 6800 0000 7201 0000 00a9 0172 8200 0000  h...r......r....
+00002ec0: fa01 2872 8e00 0000 726c 0000 00da 0368  ..(r....rl.....h
+00002ed0: 6578 5a06 7370 6c69 6e65 2902 da06 626c  exZ.spline)...bl
+00002ee0: 6f63 6b73 da05 6564 6765 7372 3a00 0000  ocks..edgesr:...
+00002ef0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00002f00: 0007 0000 0013 0000 0073 2400 0000 6700  .........s$...g.
+00002f10: 7c00 5d0e 7d01 6400 a000 8700 6601 6401  |.].}.d.....f.d.
+00002f20: 6402 8408 7c01 4400 8301 a101 9102 7102  d...|.D.......q.
+00002f30: 5300 2903 7268 0000 0063 0100 0000 0000  S.).rh...c......
+00002f40: 0000 0000 0000 0200 0000 0400 0000 3300  ..............3.
+00002f50: 0000 731a 0000 0081 007c 005d 087d 0188  ..s......|.].}..
+00002f60: 00a0 007c 01a1 0156 0001 0071 0264 0053  ...|...V...q.d.S
+00002f70: 0072 3100 0000 72af 0000 0029 0272 3600  .r1...r....).r6.
+00002f80: 0000 5a05 5f69 7465 6d72 8f00 0000 7222  ..Z._itemr....r"
+00002f90: 0000 0072 2300 0000 7239 0000 008d 0100  ...r#...r9......
+00002fa0: 0072 9900 0000 7a27 4c69 7374 2e64 756d  .r....z'List.dum
+00002fb0: 702e 3c6c 6f63 616c 733e 2e3c 6c69 7374  p.<locals>.<list
+00002fc0: 636f 6d70 3e2e 3c67 656e 6578 7072 3e72  comp>.<genexpr>r
+00002fd0: 9d00 0000 2902 7236 0000 00da 0a69 7465  ....).r6.....ite
+00002fe0: 6d73 5f6c 696e 6572 8f00 0000 7222 0000  ms_liner....r"..
+00002ff0: 0072 2300 0000 72b3 0000 008c 0100 0073  .r#...r........s
+00003000: 0800 0000 0600 0202 16ff 06ff 7a1d 4c69  ............z.Li
+00003010: 7374 2e64 756d 702e 3c6c 6f63 616c 733e  st.dump.<locals>
+00003020: 2e3c 6c69 7374 636f 6d70 3e63 0100 0000  .<listcomp>c....
+00003030: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00003040: 3300 0000 7320 0000 0081 007c 005d 0b7d  3...s .....|.].}
+00003050: 0188 0064 0017 0064 0114 007c 0117 0056  ...d...d...|...V
+00003060: 0001 0071 0264 0253 0029 0372 3a00 0000  ...q.d.S.).r:...
+00003070: 7268 0000 004e 7222 0000 0029 0272 3600  rh...Nr"...).r6.
+00003080: 0000 72ab 0000 0072 b500 0000 7222 0000  ..r....r....r"..
+00003090: 0072 2300 0000 7239 0000 0090 0100 0073  .r#...r9.......s
+000030a0: 0400 0000 0280 1e00 7a1c 4c69 7374 2e64  ........z.List.d
+000030b0: 756d 702e 3c6c 6f63 616c 733e 2e3c 6765  ump.<locals>.<ge
+000030c0: 6e65 7870 723e 7a02 293b 2907 729f 0000  nexpr>z.);).r...
+000030d0: 00da 0665 7874 656e 6472 b400 0000 7229  ...extendr....r)
+000030e0: 0000 0072 2800 0000 da04 6b65 7973 723e  ...r(.....keysr>
+000030f0: 0000 0029 0972 4500 0000 7282 0000 0072  ...).rE...r....r
+00003100: 6500 0000 72aa 0000 00da 0c73 7065 6369  e...r......speci
+00003110: 616c 5f6b 6579 735a 0b73 7065 6369 616c  al_keysZ.special
+00003120: 5f6b 6579 da05 6c69 6e65 7372 ba00 0000  _key..linesr....
+00003130: 72b1 0000 0072 2200 0000 72b2 0000 0072  r....r"...r....r
+00003140: 2300 0000 726e 0000 0073 0100 0073 3800  #...rn...s...s8.
+00003150: 0000 0401 0801 0a01 1201 1601 1e02 0a01  ................
+00003160: 0e01 1c01 0401 0a01 0c01 0801 0401 0401  ................
+00003170: 0801 0801 0801 0a01 0801 0c02 0a01 0a01  ................
+00003180: 0202 06fe 1804 0e01 0a01 7a09 4c69 7374  ..........z.List
+00003190: 2e64 756d 7072 9600 0000 7283 0000 0029  .dumpr....r....)
+000031a0: 0c72 4800 0000 7249 0000 0072 4a00 0000  .rH...rI...rJ...
+000031b0: da07 5f5f 646f 635f 5f72 6400 0000 72a4  ..__doc__rd...r.
+000031c0: 0000 0072 ae00 0000 7266 0000 0072 b400  ...r....rf...r..
+000031d0: 0000 72b0 0000 0072 6e00 0000 728b 0000  ..r....rn...r...
+000031e0: 0072 2200 0000 7222 0000 0072 8900 0000  .r"...r"...r....
+000031f0: 7223 0000 0072 3400 0000 5401 0000 7312  r#...r4...T...s.
+00003200: 0000 0008 0004 010e 0208 0408 030c 0908  ................
+00003210: 030a 0312 0672 3400 0000 6300 0000 0000  .....r4...c.....
+00003220: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
+00003230: 0000 0073 1000 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00003240: 6401 5a03 6402 5300 2903 72a9 0000 007a  d.Z.d.S.).r....z
+00003250: 2241 2064 6963 7469 6f6e 6e61 7279 2074  "A dictionnary t
+00003260: 6f20 7374 6f72 6520 2363 6f64 6553 7472  o store #codeStr
+00003270: 6561 6d4e 2904 7248 0000 0072 4900 0000  eamN).rH...rI...
+00003280: 724a 0000 0072 bf00 0000 7222 0000 0072  rJ...r....r"...r
+00003290: 2200 0000 7222 0000 0072 2300 0000 72a9  "...r"...r#...r.
+000032a0: 0000 0095 0100 0073 0400 0000 0800 0801  .......s........
+000032b0: 72a9 0000 0063 0100 0000 0000 0000 0000  r....c..........
+000032c0: 0000 0300 0000 0300 0000 0300 0000 7322  ..............s"
+000032d0: 0000 0087 0066 0164 0164 0284 087d 0187  .....f.d.d...}..
+000032e0: 0066 0164 0364 0484 087d 0274 007c 017c  .f.d.d...}.t.|.|
+000032f0: 0283 0253 0029 054e 6301 0000 0000 0000  ...S.).Nc.......
+00003300: 0000 0000 0001 0000 0002 0000 0013 0000  ................
+00003310: 0073 0a00 0000 7c00 8800 1900 6a00 5300  .s....|.....j.S.
+00003320: 7231 0000 00a9 01da 0463 6f64 6572 8f00  r1.......coder..
+00003330: 0000 725b 0000 0072 2200 0000 7223 0000  ..r[...r"...r#..
+00003340: 0072 5300 0000 9a01 0000 72a7 0000 007a  .rS.......r....z
+00003350: 185f 6d61 6b65 5f61 6c69 6173 2e3c 6c6f  ._make_alias.<lo
+00003360: 6361 6c73 3e2e 6765 7463 0200 0000 0000  cals>.getc......
+00003370: 0000 0000 0000 0200 0000 0300 0000 1300  ................
+00003380: 0000 730e 0000 007c 017c 0088 0019 005f  ..s....|.|....._
+00003390: 0064 0053 0072 3100 0000 72c0 0000 0029  .d.S.r1...r....)
+000033a0: 02da 055f 7365 6c66 7238 0000 0072 5b00  ..._selfr8...r[.
+000033b0: 0000 7222 0000 0072 2300 0000 da03 7365  ..r"...r#.....se
+000033c0: 749d 0100 0072 7c00 0000 7a18 5f6d 616b  t....r|...z._mak
+000033d0: 655f 616c 6961 732e 3c6c 6f63 616c 733e  e_alias.<locals>
+000033e0: 2e73 6574 2901 da08 7072 6f70 6572 7479  .set)...property
+000033f0: 2903 724e 0000 0072 5300 0000 72c3 0000  ).rN...rS...r...
+00003400: 0072 2200 0000 725b 0000 0072 2300 0000  .r"...r[...r#...
+00003410: da0b 5f6d 616b 655f 616c 6961 7399 0100  .._make_alias...
+00003420: 0073 0600 0000 0c01 0c03 0a03 72c5 0000  .s..........r...
+00003430: 0029 045a 0b63 6f64 6549 6e63 6c75 6465  .).Z.codeInclude
+00003440: 5a0b 636f 6465 4f70 7469 6f6e 735a 0863  Z.codeOptionsZ.c
+00003450: 6f64 654c 6962 7372 c100 0000 6300 0000  odeLibsr....c...
+00003460: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00003470: 0040 0000 0072 8c00 0000 290b da04 436f  .@...r....)...Co
+00003480: 6465 4e63 0400 0000 0000 0000 0000 0000  deNc............
+00003490: 0400 0000 0200 0000 4300 0000 731a 0000  ........C...s...
+000034a0: 007c 017c 005f 0074 017c 0283 017c 005f  .|.|._.t.|...|._
+000034b0: 027c 037c 005f 0364 0053 0072 3100 0000  .|.|._.d.S.r1...
+000034c0: 2904 724e 0000 0072 0600 0000 72c1 0000  ).rN...r....r...
+000034d0: 0072 a100 0000 2904 7245 0000 0072 4e00  .r....).rE...rN.
+000034e0: 0000 72c1 0000 0072 a100 0000 7222 0000  ..r....r....r"..
+000034f0: 0072 2200 0000 7223 0000 0072 6400 0000  .r"...r#...rd...
+00003500: a801 0000 7306 0000 0006 010a 010a 017a  ....s..........z
+00003510: 0d43 6f64 652e 5f5f 696e 6974 5f5f 6301  .Code.__init__c.
+00003520: 0000 0000 0000 0000 0000 0001 0000 0005  ................
+00003530: 0000 0043 0000 0073 3e00 0000 7c00 6a00  ...C...s>...|.j.
+00003540: 6400 7500 7210 6401 7c00 6a01 6400 6402  d.u.r.d.|.j.d.d.
+00003550: 8502 1900 9b00 6403 9d03 5300 6401 7c00  ......d...S.d.|.
+00003560: 6a01 6400 6402 8502 1900 9b00 6404 7c00  j.d.d.......d.|.
+00003570: 6a00 9b00 6405 9d05 5300 2906 4e7a 0643  j...d...S.).Nz.C
+00003580: 6f64 6528 2272 3000 0000 7a07 5b2e 2e2e  ode("r0...z.[...
+00003590: 5d22 297a 125b 2e2e 2e5d 222c 2064 6972  ]")z.[...]", dir
+000035a0: 6563 7469 7665 3d72 8e00 0000 2902 72a1  ective=r....).r.
+000035b0: 0000 0072 c100 0000 728f 0000 0072 2200  ...r....r....r".
+000035c0: 0000 7222 0000 0072 2300 0000 7266 0000  ..r"...r#...rf..
+000035d0: 00ad 0100 0073 0600 0000 0a01 1601 1e01  .....s..........
+000035e0: 7a0d 436f 6465 2e5f 5f72 6570 725f 5f72  z.Code.__repr__r
+000035f0: 0100 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00003600: 0007 0000 0005 0000 0043 0000 0073 8a00  .........C...s..
+00003610: 0000 6700 7d02 7c01 6401 1400 7d03 7c01  ..g.}.|.d...}.|.
+00003620: 6402 1700 6401 1400 7d04 7c03 7c00 6a00  d...d...}.|.|.j.
+00003630: 1700 7d05 7c00 6a01 6400 7501 721d 7c05  ..}.|.j.d.u.r.|.
+00003640: 6401 7c00 6a01 1700 3700 7d05 7c02 a002  d.|.j...7.}.|...
+00003650: 7c05 6403 7c03 9b00 9d02 1700 6404 1700  |.d.|.......d...
+00003660: a101 0100 7c00 6a03 a004 6403 a101 4400  ....|.j...d...D.
+00003670: 5d09 7d06 7c02 a002 7c04 7c06 1700 a101  ].}.|...|.|.....
+00003680: 0100 712f 7c02 a002 7c03 6405 1700 a101  ..q/|...|.d.....
+00003690: 0100 6403 a005 7c02 a101 5300 2906 4e72  ..d...|...S.).Nr
+000036a0: 6800 0000 723a 0000 0072 6c00 0000 7a02  h...r:...rl...z.
+000036b0: 237b 7a03 237d 3b29 0672 4e00 0000 72a1  #{z.#};).rN...r.
+000036c0: 0000 0072 2800 0000 72c1 0000 0072 1a00  ...r(...r....r..
+000036d0: 0000 7229 0000 0029 0772 4500 0000 7282  ..r)...).rE...r.
+000036e0: 0000 0072 6500 0000 72aa 0000 005a 0c69  ...re...r....Z.i
+000036f0: 6e64 656e 7461 7469 6f6e 3472 1800 0000  ndentation4r....
+00003700: 72ab 0000 0072 2200 0000 7222 0000 0072  r....r"...r"...r
+00003710: 2300 0000 726e 0000 00b2 0100 0073 1600  #...rn.......s..
+00003720: 0000 0401 0801 0c01 0a01 0a01 0e01 1801  ................
+00003730: 1001 1001 0e01 0a01 7a09 436f 6465 2e64  ........z.Code.d
+00003740: 756d 7072 3100 0000 7283 0000 00a9 0672  umpr1...r......r
+00003750: 4800 0000 7249 0000 0072 4a00 0000 7264  H...rI...rJ...rd
+00003760: 0000 0072 6600 0000 726e 0000 0072 2200  ...rf...rn...r".
+00003770: 0000 7222 0000 0072 2200 0000 7223 0000  ..r"...r"...r#..
+00003780: 0072 c600 0000 a701 0000 7308 0000 0008  .r........s.....
+00003790: 000a 0108 050e 0572 c600 0000 6300 0000  .......r....c...
+000037a0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+000037b0: 0040 0000 0072 8c00 0000 290b da04 4e61  .@...r....)...Na
+000037c0: 6d65 4e63 0300 0000 0000 0000 0000 0000  meNc............
+000037d0: 0300 0000 0200 0000 4300 0000 f310 0000  ........C.......
+000037e0: 007c 017c 005f 007c 027c 005f 0164 0053  .|.|._.|.|._.d.S
+000037f0: 0072 3100 0000 2902 724e 0000 0072 3800  .r1...).rN...r8.
+00003800: 0000 2903 7245 0000 0072 4e00 0000 7238  ..).rE...rN...r8
+00003810: 0000 0072 2200 0000 7222 0000 0072 2300  ...r"...r"...r#.
+00003820: 0000 7264 0000 00c2 0100 00f3 0400 0000  ..rd............
+00003830: 0601 0a01 7a0d 4e61 6d65 2e5f 5f69 6e69  ....z.Name.__ini
+00003840: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
+00003850: 0100 0000 0300 0000 4300 0000 730e 0000  ........C...s...
+00003860: 0064 017c 006a 009b 0064 029d 0353 0029  .d.|.j...d...S.)
+00003870: 034e 7a05 4e61 6d65 2872 8e00 0000 725b  .Nz.Name(r....r[
+00003880: 0000 0072 8f00 0000 7222 0000 0072 2200  ...r....r"...r".
+00003890: 0000 7223 0000 0072 6600 0000 c601 0000  ..r#...rf.......
+000038a0: 727c 0000 007a 0d4e 616d 652e 5f5f 7265  r|...z.Name.__re
+000038b0: 7072 5f5f 7201 0000 0063 0200 0000 0000  pr__r....c......
+000038c0: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
+000038d0: 0000 7308 0000 007c 006a 009b 0053 0072  ..s....|.j...S.r
+000038e0: 3100 0000 725b 0000 0072 8100 0000 7222  1...r[...r....r"
+000038f0: 0000 0072 2200 0000 7223 0000 0072 6e00  ...r"...r#...rn.
+00003900: 0000 c901 0000 729b 0000 007a 094e 616d  ......r....z.Nam
+00003910: 652e 6475 6d70 7231 0000 0072 8300 0000  e.dumpr1...r....
+00003920: 72c7 0000 0072 2200 0000 7222 0000 0072  r....r"...r"...r
+00003930: 2200 0000 7223 0000 0072 c800 0000 c001  "...r#...r......
+00003940: 0000 7308 0000 0008 000a 0208 040e 0372  ..s............r
+00003950: c800 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00003960: 0000 0000 0003 0000 0040 0000 0073 2600  .........@...s&.
+00003970: 0000 6500 5a01 6400 5a02 6401 6402 8400  ..e.Z.d.Z.d.d...
+00003980: 5a03 6403 6404 8400 5a04 6409 6406 6407  Z.d.d...Z.d.d.d.
+00003990: 8401 5a05 6408 5300 290a da09 4469 7265  ..Z.d.S.)...Dire
+000039a0: 6374 6976 6563 0300 0000 0000 0000 0000  ctivec..........
+000039b0: 0000 0300 0000 0200 0000 4300 0000 72c9  ..........C...r.
+000039c0: 0000 0072 3100 0000 a902 72a1 0000 00da  ...r1.....r.....
+000039d0: 0763 6f6e 7465 6e74 2903 7245 0000 0072  .content).rE...r
+000039e0: a100 0000 72cd 0000 0072 2200 0000 7222  ....r....r"...r"
+000039f0: 0000 0072 2300 0000 7264 0000 00ce 0100  ...r#...rd......
+00003a00: 0072 ca00 0000 7a12 4469 7265 6374 6976  .r....z.Directiv
+00003a10: 652e 5f5f 696e 6974 5f5f 6301 0000 0000  e.__init__c.....
+00003a20: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+00003a30: 0000 0073 1200 0000 7c00 6a00 9b00 6401  ...s....|.j...d.
+00003a40: 7c00 6a01 9b00 9d03 5300 2902 4e72 8000  |.j.....S.).Nr..
+00003a50: 0000 72cc 0000 0072 8f00 0000 7222 0000  ..r....r....r"..
+00003a60: 0072 2200 0000 7223 0000 0072 6600 0000  .r"...r#...rf...
+00003a70: d201 0000 7302 0000 0012 017a 1244 6972  ....s......z.Dir
+00003a80: 6563 7469 7665 2e5f 5f72 6570 725f 5f72  ective.__repr__r
+00003a90: 0100 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00003aa0: 0002 0000 0005 0000 0043 0000 0073 1c00  .........C...s..
+00003ab0: 0000 7c01 6401 1400 7c00 6a00 9b00 6402  ..|.d...|.j...d.
+00003ac0: 7c00 6a01 9b00 6403 9d04 1700 5300 2904  |.j...d.....S.).
+00003ad0: 4e72 6800 0000 7280 0000 0072 6a00 0000  Nrh...r....rj...
+00003ae0: 72cc 0000 0072 8100 0000 7222 0000 0072  r....r....r"...r
+00003af0: 2200 0000 7223 0000 0072 6e00 0000 d501  "...r#...rn.....
+00003b00: 0000 729e 0000 007a 0e44 6972 6563 7469  ..r....z.Directi
+00003b10: 7665 2e64 756d 704e 7283 0000 0072 c700  ve.dumpNr....r..
+00003b20: 0000 7222 0000 0072 2200 0000 7222 0000  ..r"...r"...r"..
+00003b30: 0072 2300 0000 72cb 0000 00cd 0100 0073  .r#...r........s
+00003b40: 0800 0000 0800 0801 0804 0e03 72cb 0000  ............r...
+00003b50: 0029 0172 3000 0000 2925 72bf 0000 0072  .).r0...)%r....r
+00003b60: 1600 0000 da03 6162 6372 0200 0000 7203  ......abcr....r.
+00003b70: 0000 00da 0b64 6174 6163 6c61 7373 6573  .....dataclasses
+00003b80: 7204 0000 00da 076e 756d 6265 7273 7205  r......numbersr.
+00003b90: 0000 00da 0874 6578 7477 7261 7072 0600  .....textwrapr..
+00003ba0: 0000 da06 7479 7069 6e67 7207 0000 005a  ....typingr....Z
+00003bb0: 0a69 6e66 6c65 6374 696f 6e72 0800 0000  .inflectionr....
+00003bc0: 721c 0000 0072 2400 0000 722f 0000 0072  r....r$...r/...r
+00003bd0: 4100 0000 7242 0000 0072 4b00 0000 725f  A...rB...rK...r_
+00003be0: 0000 0072 7e00 0000 7286 0000 0072 5d00  ...r~...r....r].
+00003bf0: 0000 7252 0000 0072 9700 0000 7255 0000  ..rR...r....rU..
+00003c00: 0072 3300 0000 7234 0000 0072 a900 0000  .r3...r4...r....
+00003c10: 72c5 0000 0072 9f00 0000 da07 7365 7461  r....r......seta
+00003c20: 7474 7272 c600 0000 72c8 0000 0072 cb00  ttrr....r....r..
+00003c30: 0000 7222 0000 0072 2200 0000 7222 0000  ..r"...r"...r"..
+00003c40: 0072 2300 0000 da08 3c6d 6f64 756c 653e  .r#.....<module>
+00003c50: 0100 0000 733e 0000 0004 0008 0210 010c  ....s>..........
+00003c60: 010c 010c 010c 010c 0208 0208 0308 1b0a  ................
+00003c70: 120e 1110 0712 3a02 4510 0110 0b02 0c12  ......:.E.......
+00003c80: 0112 2614 0d12 3510 4108 0408 0a16 0110  ..&...5.A.......
+00003c90: 0302 1912 0114 0c                        .......
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/__pycache__/parser.cpython-310.pyc` & `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/__pycache__/parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 19:59:34 2023 UTC, .py size: 9483 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,652 +1,655 @@
-00000000: 6f0d 0d0a 0000 0000 a699 4164 0b25 0000  o.........Ad.%..
+00000000: 6f0d 0d0a 0000 0000 c13f 5a64 3225 0000  o........?Zd2%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 0001 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c08  m.Z.m.Z...d.d.l.
-00000060: 6d09 5a09 0100 6405 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
+00000020: 0005 0000 0040 0000 0073 0401 0000 6400  .....@...s....d.
+00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
+00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
+00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6401  m.Z.m.Z.m.Z...d.
+00000060: 6405 6c09 6d0a 5a0a 0100 6406 6407 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
 00000080: 6d10 5a10 6d11 5a11 6d12 5a12 6d13 5a13  m.Z.m.Z.m.Z.m.Z.
-00000090: 6d14 5a14 6d15 5a15 0100 6503 6516 8301  m.Z.m.Z...e.e...
-000000a0: a017 a100 6a18 5a19 6519 6407 1b00 a01a  ....j.Z.e.d.....
-000000b0: a100 5a1b 6519 6408 1b00 a01a a100 5a1c  ..Z.e.d.......Z.
-000000c0: 6505 651b 6409 640a 640b 8d03 5a1d 6505  e.e.d.d.d...Z.e.
-000000d0: 651c 6409 640a 640b 8d03 5a1e 651d 651e  e.d.d.d...Z.e.e.
-000000e0: 640c 9c02 5a1f 6501 4700 640d 640e 8400  d...Z.e.G.d.d...
-000000f0: 640e 8302 8301 5a20 641a 6410 6411 8401  d.....Z d.d.d...
-00000100: 5a21 6412 6413 8400 5a22 6414 6415 8400  Z!d.d...Z"d.d...
-00000110: 5a23 6416 6417 8400 5a24 4700 6418 6419  Z#d.d...Z$G.d.d.
-00000120: 8400 6419 6507 8303 5a25 640f 5300 291b  ..d.e...Z%d.S.).
-00000130: e900 0000 0029 01da 0964 6174 6163 6c61  .....)...datacla
-00000140: 7373 2901 da04 5061 7468 2903 da04 4c61  ss)...Path)...La
-00000150: 726b da05 546f 6b65 6eda 0b54 7261 6e73  rk..Token..Trans
-00000160: 666f 726d 6572 2901 da09 4c61 726b 4572  former)...LarkEr
-00000170: 726f 72e9 0100 0000 290b da0a 4173 7369  ror.....)...Assi
-00000180: 676e 6d65 6e74 da04 436f 6465 da0a 436f  gnment..Code..Co
-00000190: 6465 5374 7265 616d da04 4469 6374 da0c  deStream..Dict..
-000001a0: 4469 6d65 6e73 696f 6e53 6574 da09 4469  DimensionSet..Di
-000001b0: 7265 6374 6976 65da 0d46 6f61 6d49 6e70  rective..FoamInp
-000001c0: 7574 4669 6c65 da04 4c69 7374 da04 4e61  utFile..List..Na
-000001d0: 6d65 da05 5661 6c75 65da 1256 6172 6961  me..Value..Varia
-000001e0: 626c 6541 7373 6967 6e6d 656e 747a 0c67  bleAssignmentz.g
-000001f0: 7261 6d6d 6172 2e6c 6172 6b7a 1567 7261  rammar.larkz.gra
-00000200: 6d6d 6172 5f61 6476 616e 6365 642e 6c61  mmar_advanced.la
-00000210: 726b da05 7661 6c75 65da 0562 6173 6963  rk..value..basic
-00000220: 2902 da05 7374 6172 74da 056c 6578 6572  )...start..lexer
-00000230: 2902 da06 7369 6d70 6c65 da08 6164 7661  )...simple..adva
-00000240: 6e63 6564 6300 0000 0000 0000 0000 0000  ncedc...........
-00000250: 0000 0000 0003 0000 0040 0000 0073 3a00  .........@...s:.
-00000260: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
-00000270: 6401 3c00 6402 5a05 6503 6504 6403 3c00  d.<.d.Z.e.e.d.<.
-00000280: 6402 5a06 6503 6504 6404 3c00 6402 5a07  d.Z.e.e.d.<.d.Z.
-00000290: 6508 6504 6405 3c00 6402 5300 2906 da08  e.e.d.<.d.S.)...
-000002a0: 4c69 7374 496e 666f da04 6e61 6d65 4eda  ListInfo..nameN.
-000002b0: 0469 6e66 6fda 0564 7479 7065 da04 7369  .info..dtype..si
-000002c0: 7a65 2909 da08 5f5f 6e61 6d65 5f5f da0a  ze)...__name__..
-000002d0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-000002e0: 616c 6e61 6d65 5f5f da03 7374 72da 0f5f  alname__..str.._
-000002f0: 5f61 6e6e 6f74 6174 696f 6e73 5f5f 721c  _annotations__r.
-00000300: 0000 0072 1d00 0000 721e 0000 00da 0369  ...r....r......i
-00000310: 6e74 a900 7225 0000 0072 2500 0000 fa49  nt..r%...r%....I
-00000320: 2f68 6f6d 652f 7069 6572 7265 2f44 6576  /home/pierre/Dev
-00000330: 2f66 6c75 6964 7369 6d66 6f61 6d2f 7372  /fluidsimfoam/sr
-00000340: 632f 666c 7569 6473 696d 666f 616d 2f66  c/fluidsimfoam/f
-00000350: 6f61 6d5f 696e 7075 745f 6669 6c65 732f  oam_input_files/
-00000360: 7061 7273 6572 2e70 7972 1a00 0000 2000  parser.pyr.... .
-00000370: 0000 730a 0000 000a 0008 020c 010c 0110  ..s.............
-00000380: 0172 1a00 0000 4e63 0200 0000 0000 0000  .r....Nc........
-00000390: 0000 0000 0300 0000 0800 0000 4300 0000  ............C...
-000003a0: 737a 0000 0064 01a0 0064 0264 0384 007c  sz...d...d.d...|
-000003b0: 00a0 0164 01a1 0144 0083 01a1 017d 007c  ...d...D.....}.|
-000003c0: 00a0 0264 01a1 0173 167c 0064 0137 007d  ...d...s.|.d.7.}
-000003d0: 007c 0164 0075 0072 307a 0774 03a0 047c  .|.d.u.r0z.t...|
-000003e0: 00a1 017d 0257 006e 1504 0074 0579 2f01  ...}.W.n...t.y/.
-000003f0: 0001 0001 0074 06a0 047c 00a1 017d 0259  .....t...|...}.Y
-00000400: 006e 0877 0074 077c 0119 00a0 047c 00a1  .n.w.t.|.....|..
-00000410: 017d 0274 0883 00a0 097c 02a1 0153 0029  .}.t.....|...S.)
-00000420: 044e da01 0a63 0100 0000 0000 0000 0000  .N...c..........
-00000430: 0000 0200 0000 0300 0000 7300 0000 7318  ..........s...s.
-00000440: 0000 0081 007c 005d 077d 017c 01a0 00a1  .....|.].}.|....
-00000450: 0056 0001 0071 0264 0053 00a9 014e 2901  .V...q.d.S...N).
-00000460: da06 7273 7472 6970 2902 da02 2e30 da04  ..rstrip)....0..
-00000470: 6c69 6e65 7225 0000 0072 2500 0000 7226  liner%...r%...r&
-00000480: 0000 00da 093c 6765 6e65 7870 723e 2900  .....<genexpr>).
-00000490: 0000 7304 0000 0002 8016 007a 1870 6172  ..s........z.par
-000004a0: 7365 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  se.<locals>.<gen
-000004b0: 6578 7072 3e29 0ada 046a 6f69 6eda 0573  expr>)...join..s
-000004c0: 706c 6974 da08 656e 6473 7769 7468 da0b  plit..endswith..
-000004d0: 6c61 726b 5f70 6172 7365 72da 0570 6172  lark_parser..par
-000004e0: 7365 7207 0000 00da 146c 6172 6b5f 7061  ser......lark_pa
-000004f0: 7273 6572 5f61 6476 616e 6365 64da 0770  rser_advanced..p
-00000500: 6172 7365 7273 da0f 466f 616d 5472 616e  arsers..FoamTran
-00000510: 7366 6f72 6d65 72da 0974 7261 6e73 666f  sformer..transfo
-00000520: 726d 2903 da04 7465 7874 da07 6772 616d  rm)...text..gram
-00000530: 6d61 72da 0474 7265 6572 2500 0000 7225  mar..treer%...r%
-00000540: 0000 0072 2600 0000 7231 0000 0028 0000  ...r&...r1...(..
-00000550: 0073 1600 0000 1a01 0a01 0801 0802 0201  .s..............
-00000560: 0e01 0c01 0e01 02ff 0e03 0c02 7231 0000  ............r1..
-00000570: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-00000580: 0000 0200 0000 4300 0000 7308 0000 007c  ......C...s....|
-00000590: 00a0 00a1 0053 0072 2800 0000 2901 da04  .....S.r(...)...
-000005a0: 6475 6d70 2901 7238 0000 0072 2500 0000  dump).r8...r%...
-000005b0: 7225 0000 0072 2600 0000 7239 0000 0038  r%...r&...r9...8
-000005c0: 0000 00f3 0200 0000 0801 7239 0000 0063  ..........r9...c
-000005d0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000005e0: 0200 0000 4300 0000 730e 0000 0064 0164  ....C...s....d.d
-000005f0: 0284 007c 0044 0083 0153 0029 034e 6301  ...|.D...S.).Nc.
-00000600: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000610: 0000 0053 0000 00f3 1800 0000 6700 7c00  ...S........g.|.
-00000620: 5d08 7d01 7c01 6400 7501 7202 7c01 9102  ].}.|.d.u.r.|...
-00000630: 7102 5300 7228 0000 0072 2500 0000 a902  q.S.r(...r%.....
-00000640: 722a 0000 00da 0469 7465 6d72 2500 0000  r*.....itemr%...
-00000650: 7225 0000 0072 2600 0000 da0a 3c6c 6973  r%...r&.....<lis
-00000660: 7463 6f6d 703e 3d00 0000 f302 0000 0018  tcomp>=.........
-00000670: 007a 2666 696c 7465 725f 6e6f 5f6e 6577  .z&filter_no_new
-00000680: 6c69 6e65 732e 3c6c 6f63 616c 733e 2e3c  lines.<locals>.<
-00000690: 6c69 7374 636f 6d70 3e72 2500 0000 2901  listcomp>r%...).
-000006a0: da05 6974 656d 7372 2500 0000 7225 0000  ..itemsr%...r%..
-000006b0: 0072 2600 0000 da12 6669 6c74 6572 5f6e  .r&.....filter_n
-000006c0: 6f5f 6e65 776c 696e 6573 3c00 0000 7302  o_newlines<...s.
-000006d0: 0000 000e 0172 4100 0000 6301 0000 0000  .....rA...c.....
-000006e0: 0000 0000 0000 0001 0000 0008 0000 0043  ...............C
-000006f0: 0000 0073 2e00 0000 7400 7c00 8301 7d00  ...s....t.|...}.
-00000700: 7a05 7401 7c00 8301 5700 5300 0400 7402  z.t.|...W.S...t.
-00000710: 7916 0100 0100 0100 7403 7c00 8301 0600  y.......t.|.....
-00000720: 5900 5300 7700 7228 0000 0029 0472 2200  Y.S.w.r(...).r".
-00000730: 0000 7224 0000 00da 0a56 616c 7565 4572  ..r$.....ValueEr
-00000740: 726f 72da 0566 6c6f 6174 2901 da06 6e75  ror..float)...nu
-00000750: 6d62 6572 7225 0000 0072 2500 0000 7226  mberr%...r%...r&
-00000760: 0000 00da 125f 636f 6e76 6572 745f 746f  ....._convert_to
-00000770: 5f6e 756d 6265 7240 0000 0073 0c00 0000  _number@...s....
-00000780: 0801 0201 0a01 0c01 0c01 02ff 7245 0000  ............rE..
-00000790: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-000007a0: 0000 0200 0000 4000 0000 73c4 0000 0065  ......@...s....e
-000007b0: 005a 0164 005a 0264 0164 0284 005a 0364  .Z.d.Z.d.d...Z.d
-000007c0: 0364 0484 005a 0464 0564 0684 005a 0564  .d...Z.d.d...Z.d
-000007d0: 0764 0884 005a 0664 0964 0a84 005a 0764  .d...Z.d.d...Z.d
-000007e0: 0b64 0c84 005a 0864 0d64 0e84 005a 0964  .d...Z.d.d...Z.d
-000007f0: 0f64 1084 005a 0a64 1164 1284 005a 0b64  .d...Z.d.d...Z.d
-00000800: 1364 1484 005a 0c64 1564 1684 005a 0d64  .d...Z.d.d...Z.d
-00000810: 1764 1884 005a 0e64 1964 1a84 005a 0f64  .d...Z.d.d...Z.d
-00000820: 1b64 1c84 005a 1064 1d64 1e84 005a 1164  .d...Z.d.d...Z.d
-00000830: 1f64 2084 005a 1264 2164 2284 005a 1364  .d ..Z.d!d"..Z.d
-00000840: 2364 2484 005a 1464 2564 2684 005a 1564  #d$..Z.d%d&..Z.d
-00000850: 2764 2884 005a 1664 2964 2a84 005a 1764  'd(..Z.d)d*..Z.d
-00000860: 2b64 2c84 005a 1864 2d64 2e84 005a 1964  +d,..Z.d-d...Z.d
-00000870: 2f53 0029 3072 3400 0000 6302 0000 0000  /S.)0r4...c.....
-00000880: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
-00000890: 0000 0073 0800 0000 7400 7c01 8301 5300  ...s....t.|...S.
-000008a0: 7228 0000 0029 0172 4500 0000 a902 da04  r(...).rE.......
-000008b0: 7365 6c66 da05 746f 6b65 6e72 2500 0000  self..tokenr%...
-000008c0: 7225 0000 0072 2600 0000 da0d 5349 474e  r%...r&.....SIGN
-000008d0: 4544 5f4e 554d 4245 5249 0000 0072 3a00  ED_NUMBERI...r:.
-000008e0: 0000 7a1d 466f 616d 5472 616e 7366 6f72  ..z.FoamTransfor
-000008f0: 6d65 722e 5349 474e 4544 5f4e 554d 4245  mer.SIGNED_NUMBE
-00000900: 5263 0200 0000 0000 0000 0000 0000 0200  Rc..............
-00000910: 0000 0100 0000 4300 0000 f306 0000 007c  ......C........|
-00000920: 016a 0053 0072 2800 0000 a901 7214 0000  .j.S.r(.....r...
-00000930: 0072 4600 0000 7225 0000 0072 2500 0000  .rF...r%...r%...
-00000940: 7226 0000 00da 0543 4e41 4d45 4c00 0000  r&.....CNAMEL...
-00000950: f302 0000 0006 017a 1546 6f61 6d54 7261  .......z.FoamTra
-00000960: 6e73 666f 726d 6572 2e43 4e41 4d45 6302  nsformer.CNAMEc.
-00000970: 0000 0000 0000 0000 0000 0002 0000 0001  ................
-00000980: 0000 0043 0000 0073 0400 0000 6400 5300  ...C...s....d.S.
-00000990: 7228 0000 0072 2500 0000 a902 7247 0000  r(...r%.....rG..
-000009a0: 00da 056e 6f64 6573 7225 0000 0072 2500  ...nodesr%...r%.
-000009b0: 0000 7226 0000 00da 074e 4557 4c49 4e45  ..r&.....NEWLINE
-000009c0: 4f00 0000 7302 0000 0004 017a 1746 6f61  O...s......z.Foa
-000009d0: 6d54 7261 6e73 666f 726d 6572 2e4e 4557  mTransformer.NEW
-000009e0: 4c49 4e45 6302 0000 0000 0000 0000 0000  LINEc...........
-000009f0: 0002 0000 0001 0000 0043 0000 0072 4a00  .........C...rJ.
-00000a00: 0000 7228 0000 0072 4b00 0000 7246 0000  ..r(...rK...rF..
-00000a10: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
-00000a20: da0e 4553 4341 5045 445f 5354 5249 4e47  ..ESCAPED_STRING
-00000a30: 5200 0000 724d 0000 007a 1e46 6f61 6d54  R...rM...z.FoamT
-00000a40: 7261 6e73 666f 726d 6572 2e45 5343 4150  ransformer.ESCAP
-00000a50: 4544 5f53 5452 494e 4763 0200 0000 0000  ED_STRINGc......
-00000a60: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
-00000a70: 0000 724a 0000 0072 2800 0000 724b 0000  ..rJ...r(...rK..
-00000a80: 0072 4600 0000 7225 0000 0072 2500 0000  .rF...r%...r%...
-00000a90: 7226 0000 00da 0b44 4f55 424c 455f 4e41  r&.....DOUBLE_NA
-00000aa0: 4d45 5500 0000 724d 0000 007a 1b46 6f61  MEU...rM...z.Foa
-00000ab0: 6d54 7261 6e73 666f 726d 6572 2e44 4f55  mTransformer.DOU
-00000ac0: 424c 455f 4e41 4d45 6302 0000 0000 0000  BLE_NAMEc.......
-00000ad0: 0000 0000 0002 0000 0001 0000 0043 0000  .............C..
-00000ae0: 0072 4a00 0000 7228 0000 0072 4b00 0000  .rJ...r(...rK...
-00000af0: 7246 0000 0072 2500 0000 7225 0000 0072  rF...r%...r%...r
-00000b00: 2600 0000 da0b 5452 4950 4c45 5f4e 414d  &.....TRIPLE_NAM
-00000b10: 4558 0000 0072 4d00 0000 7a1b 466f 616d  EX...rM...z.Foam
-00000b20: 5472 616e 7366 6f72 6d65 722e 5452 4950  Transformer.TRIP
-00000b30: 4c45 5f4e 414d 4563 0200 0000 0000 0000  LE_NAMEc........
-00000b40: 0000 0000 0200 0000 0100 0000 4300 0000  ............C...
-00000b50: 724a 0000 0072 2800 0000 724b 0000 0072  rJ...r(...rK...r
-00000b60: 4600 0000 7225 0000 0072 2500 0000 7226  F...r%...r%...r&
-00000b70: 0000 00da 0545 514b 4559 5b00 0000 724d  .....EQKEY[...rM
-00000b80: 0000 007a 1546 6f61 6d54 7261 6e73 666f  ...z.FoamTransfo
-00000b90: 726d 6572 2e45 514b 4559 6302 0000 0000  rmer.EQKEYc.....
-00000ba0: 0000 0000 0000 0002 0000 0001 0000 0043  ...............C
-00000bb0: 0000 0072 4a00 0000 7228 0000 0072 4b00  ...rJ...r(...rK.
-00000bc0: 0000 7246 0000 0072 2500 0000 7225 0000  ..rF...r%...r%..
-00000bd0: 0072 2600 0000 da05 4d41 4352 4f5e 0000  .r&.....MACRO^..
-00000be0: 0072 4d00 0000 7a15 466f 616d 5472 616e  .rM...z.FoamTran
-00000bf0: 7366 6f72 6d65 722e 4d41 4352 4f63 0200  sformer.MACROc..
-00000c00: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00000c10: 0000 4300 0000 f312 0000 0074 0064 0164  ..C........t.d.d
-00000c20: 0284 007c 0144 0083 0183 0153 0029 034e  ...|.D.....S.).N
-00000c30: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000c40: 0005 0000 0053 0000 0073 2400 0000 6700  .....S...s$...g.
-00000c50: 7c00 5d0e 7d01 7400 7c01 7401 8302 720e  |.].}.t.|.t...r.
-00000c60: 7c01 6a02 6400 6b02 7302 7c01 9102 7102  |.j.d.k.s.|...q.
-00000c70: 5300 2901 7250 0000 00a9 03da 0a69 7369  S.).rP.......isi
-00000c80: 6e73 7461 6e63 6572 0500 0000 da04 7479  nstancer......ty
-00000c90: 7065 723c 0000 0072 2500 0000 7225 0000  per<...r%...r%..
-00000ca0: 0072 2600 0000 723e 0000 0063 0000 00f3  .r&...r>...c....
-00000cb0: 1000 0000 0600 0202 0801 02fd 0803 02fd  ................
-00000cc0: 0201 06ff 7a31 466f 616d 5472 616e 7366  ....z1FoamTransf
-00000cd0: 6f72 6d65 722e 6469 6d65 6e73 696f 6e5f  ormer.dimension_
-00000ce0: 7365 742e 3c6c 6f63 616c 733e 2e3c 6c69  set.<locals>.<li
-00000cf0: 7374 636f 6d70 3e29 0172 0d00 0000 a902  stcomp>).r......
-00000d00: 7247 0000 0072 4000 0000 7225 0000 0072  rG...r@...r%...r
-00000d10: 2500 0000 7226 0000 00da 0d64 696d 656e  %...r&.....dimen
-00000d20: 7369 6f6e 5f73 6574 6100 0000 f30a 0000  sion_seta.......
-00000d30: 0002 0106 0102 0204 fe04 ff7a 1d46 6f61  ...........z.Foa
-00000d40: 6d54 7261 6e73 666f 726d 6572 2e64 696d  mTransformer.dim
-00000d50: 656e 7369 6f6e 5f73 6574 6302 0000 0000  ension_setc.....
-00000d60: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
-00000d70: 0000 0073 1c00 0000 7400 7c01 8301 6401  ...s....t.|...d.
-00000d80: 6b03 7208 7401 8201 7402 7c01 6402 1900  k.r.t...t.|.d...
-00000d90: 8301 5300 a903 4e72 0800 0000 7201 0000  ..S...Nr....r...
-00000da0: 0029 03da 036c 656e da0c 5275 6e74 696d  .)...len..Runtim
-00000db0: 6545 7272 6f72 7222 0000 0072 4e00 0000  eErrorr"...rN...
-00000dc0: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
-00000dd0: 0964 6972 6563 7469 7665 6a00 0000 7306  .directivej...s.
-00000de0: 0000 000c 0104 010c 017a 1946 6f61 6d54  .........z.FoamT
-00000df0: 7261 6e73 666f 726d 6572 2e64 6972 6563  ransformer.direc
-00000e00: 7469 7665 6302 0000 0000 0000 0000 0000  tivec...........
-00000e10: 0002 0000 0003 0000 0043 0000 0072 5600  .........C...rV.
-00000e20: 0000 2903 4e63 0100 0000 0000 0000 0000  ..).Nc..........
-00000e30: 0000 0200 0000 0500 0000 5300 0000 732c  ..........S...s,
-00000e40: 0000 0067 007c 005d 127d 0174 007c 0174  ...g.|.].}.t.|.t
-00000e50: 0183 0272 0e7c 016a 0264 006b 0273 027c  ...r.|.j.d.k.s.|
-00000e60: 0164 0175 0172 027c 0191 0271 0253 0029  .d.u.r.|...q.S.)
-00000e70: 0272 5000 0000 4e72 5700 0000 723c 0000  .rP...NrW...r<..
-00000e80: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
-00000e90: 723e 0000 0071 0000 0073 1400 0000 0600  r>...q...s......
-00000ea0: 0202 0801 02fd 0803 02fd 0604 02fc 0201  ................
-00000eb0: 06ff 7a28 466f 616d 5472 616e 7366 6f72  ..z(FoamTransfor
-00000ec0: 6d65 722e 6c69 7374 2e3c 6c6f 6361 6c73  mer.list.<locals
-00000ed0: 3e2e 3c6c 6973 7463 6f6d 703e 2901 7210  >.<listcomp>).r.
-00000ee0: 0000 0072 5b00 0000 7225 0000 0072 2500  ...r[...r%...r%.
-00000ef0: 0000 7226 0000 00da 046c 6973 746f 0000  ..r&.....listo..
-00000f00: 0072 5d00 0000 7a14 466f 616d 5472 616e  .r]...z.FoamTran
-00000f10: 7366 6f72 6d65 722e 6c69 7374 6302 0000  sformer.listc...
-00000f20: 0000 0000 0000 0000 0005 0000 0004 0000  ................
-00000f30: 0043 0000 0073 6200 0000 7c01 6401 1900  .C...sb...|.d...
-00000f40: 7d02 7c02 6a00 6402 6b02 7213 7c02 6a01  }.|.j.d.k.r.|.j.
-00000f50: 7d03 7c01 6403 6400 8502 1900 7d01 6e02  }.|.d.d.....}.n.
-00000f60: 6400 7d03 7c01 4400 5d0f 7d04 7402 7c04  d.}.|.D.].}.t.|.
-00000f70: 6a01 7403 8302 7226 7c04 6a01 a004 7c04  j.t...r&|.j...|.
-00000f80: 6a00 a101 0100 7117 7405 7c03 6404 6405  j.....q.t.|.d.d.
-00000f90: 8400 7c01 4400 8301 8302 5300 2906 4e72  ..|.D.....S.).Nr
-00000fa0: 0100 0000 5a08 466f 616d 4669 6c65 7208  ....Z.FoamFiler.
-00000fb0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000fc0: 0200 0000 0400 0000 5300 0000 f316 0000  ........S.......
-00000fd0: 0069 007c 005d 077d 017c 016a 007c 016a  .i.|.].}.|.j.|.j
-00000fe0: 0193 0271 0253 0072 2500 0000 a902 721b  ...q.S.r%.....r.
-00000ff0: 0000 0072 1400 0000 a902 722a 0000 00da  ...r......r*....
-00001000: 046e 6f64 6572 2500 0000 7225 0000 0072  .noder%...r%...r
-00001010: 2600 0000 da0a 3c64 6963 7463 6f6d 703e  &.....<dictcomp>
-00001020: 8500 0000 f302 0000 0016 007a 2846 6f61  ...........z(Foa
-00001030: 6d54 7261 6e73 666f 726d 6572 2e66 696c  mTransformer.fil
-00001040: 652e 3c6c 6f63 616c 733e 2e3c 6469 6374  e.<locals>.<dict
-00001050: 636f 6d70 3e29 0672 1b00 0000 7214 0000  comp>).r....r...
-00001060: 0072 5800 0000 7210 0000 00da 0861 6464  .rX...r......add
-00001070: 5f6e 616d 6572 0f00 0000 2905 7247 0000  _namer....).rG..
-00001080: 0072 4f00 0000 5a10 6669 7273 745f 6173  .rO...Z.first_as
-00001090: 7369 676e 6d65 6e74 da09 696e 666f 5f64  signment..info_d
-000010a0: 6963 7472 6600 0000 7225 0000 0072 2500  ictrf...r%...r%.
-000010b0: 0000 7226 0000 00da 0466 696c 6579 0000  ..r&.....filey..
-000010c0: 0073 1400 0000 0801 0a01 0601 0e01 0402  .s..............
-000010d0: 0802 0c01 0e01 0280 1402 7a14 466f 616d  ..........z.Foam
-000010e0: 5472 616e 7366 6f72 6d65 722e 6669 6c65  Transformer.file
-000010f0: 6302 0000 0000 0000 0000 0000 0008 0000  c...............
-00001100: 0008 0000 0043 0000 0073 1201 0000 6401  .....C...s....d.
-00001110: 6402 8400 7c01 4400 8301 7d01 6400 7d02  d...|.D...}.d.}.
-00001120: 6400 7d03 7c01 a000 6403 a101 7d04 7401  d.}.|...d...}.t.
-00001130: 7c01 8301 6404 6b02 721b 7c01 6403 1900  |...d.k.r.|.d...
-00001140: 7d05 6e69 7a0c 6405 6402 8400 7c01 4400  }.niz.d.d...|.D.
-00001150: 8301 a002 6406 a101 7d06 5700 6e0b 0400  ....d...}.W.n...
-00001160: 7403 7932 0100 0100 0100 6400 7d02 5900  t.y2......d.}.Y.
-00001170: 6e06 7700 7c01 a000 7c06 a101 7d02 6400  n.w.|...|...}.d.
-00001180: 7d03 7404 6407 6402 8400 7c01 4400 8301  }.t.d.d...|.D...
-00001190: 8301 7249 6408 a005 7c01 a101 7d07 6e24  ..rId...|...}.n$
-000011a0: 7c01 a000 6409 a101 7d07 7404 640a 640b  |...d...}.t.d.d.
-000011b0: 8400 7c01 4400 8301 8301 735e 640c 6402  ..|.D.....s^d.d.
-000011c0: 8400 7c01 4400 8301 7d01 7c01 7265 6408  ..|.D...}.|.red.
-000011d0: a005 7c01 a101 7d03 7406 7c07 7407 8302  ..|...}.t.|.t...
-000011e0: 726d 7c03 7c07 5f08 7c03 6400 7500 7275  rm|.|._.|.d.u.ru
-000011f0: 7c02 6400 7500 737a 7406 7c07 7407 8302  |.d.u.szt.|.t...
-00001200: 727d 7c07 7d05 6e07 7409 7c07 7c03 7c02  r}|.}.n.t.|.|.|.
-00001210: 640d 8d03 7d05 740a 7c04 7c05 8302 5300  d...}.t.|.|...S.
-00001220: 290e 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
-00001230: 0200 0000 0400 0000 5300 0000 723b 0000  ........S...r;..
-00001240: 0072 2800 0000 7225 0000 0072 6500 0000  .r(...r%...re...
-00001250: 7225 0000 0072 2500 0000 7226 0000 0072  r%...r%...r&...r
-00001260: 3e00 0000 8800 0000 723f 0000 007a 3246  >.......r?...z2F
-00001270: 6f61 6d54 7261 6e73 666f 726d 6572 2e76  oamTransformer.v
-00001280: 6172 5f61 7373 6967 6e6d 656e 742e 3c6c  ar_assignment.<l
-00001290: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-000012a0: 3e72 0100 0000 7208 0000 0063 0100 0000  >r....r....c....
-000012b0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-000012c0: 5300 0000 f316 0000 0067 007c 005d 077d  S........g.|.].}
-000012d0: 0174 007c 0174 0183 0291 0271 0253 0072  .t.|.t.....q.S.r
-000012e0: 2500 0000 2902 7258 0000 0072 0d00 0000  %...).rX...r....
-000012f0: a902 722a 0000 00da 0465 6c65 6d72 2500  ..r*.....elemr%.
-00001300: 0000 7225 0000 0072 2600 0000 723e 0000  ..r%...r&...r>..
-00001310: 0090 0000 0073 0600 0000 0600 0a01 06ff  .....s..........
-00001320: 5463 0100 0000 0000 0000 0000 0000 0200  Tc..............
-00001330: 0000 0500 0000 5300 0000 726c 0000 0072  ......S...rl...r
-00001340: 2500 0000 a902 7258 0000 0072 2200 0000  %.....rX...r"...
-00001350: 726d 0000 0072 2500 0000 7225 0000 0072  rm...r%...r%...r
-00001360: 2600 0000 723e 0000 0099 0000 0072 6800  &...r>.......rh.
-00001370: 0000 fa01 20e9 ffff ffff 6301 0000 0000  .... .....c.....
-00001380: 0000 0000 0000 0002 0000 0004 0000 0073  ...............s
-00001390: 0000 0073 1a00 0000 8100 7c00 5d08 7d01  ...s......|.].}.
-000013a0: 7400 7c01 7401 8302 5600 0100 7102 6400  t.|.t...V...q.d.
-000013b0: 5300 7228 0000 0072 6f00 0000 7265 0000  S.r(...ro...re..
-000013c0: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
-000013d0: 722c 0000 009d 0000 0073 0400 0000 0280  r,.......s......
-000013e0: 1800 7a31 466f 616d 5472 616e 7366 6f72  ..z1FoamTransfor
-000013f0: 6d65 722e 7661 725f 6173 7369 676e 6d65  mer.var_assignme
-00001400: 6e74 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  nt.<locals>.<gen
-00001410: 6578 7072 3e63 0100 0000 0000 0000 0000  expr>c..........
-00001420: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
-00001430: 0000 0067 007c 005d 067d 0174 007c 0183  ...g.|.].}.t.|..
-00001440: 0191 0271 0253 0072 2500 0000 2901 7222  ...q.S.r%...).r"
-00001450: 0000 0072 6500 0000 7225 0000 0072 2500  ...re...r%...r%.
-00001460: 0000 7226 0000 0072 3e00 0000 9e00 0000  ..r&...r>.......
-00001470: 7302 0000 0014 0029 0272 1b00 0000 da09  s......).r......
-00001480: 6469 6d65 6e73 696f 6e29 0bda 0370 6f70  dimension)...pop
-00001490: 725f 0000 00da 0569 6e64 6578 7242 0000  r_.....indexrB..
-000014a0: 00da 0361 6c6c 722d 0000 0072 5800 0000  ...allr-...rX...
-000014b0: 7210 0000 00da 055f 6e61 6d65 7212 0000  r......_namer...
-000014c0: 0072 1300 0000 2908 7247 0000 0072 4f00  .r....).rG...rO.
-000014d0: 0000 725c 0000 005a 0d6e 616d 655f 696e  ..r\...Z.name_in
-000014e0: 5f76 616c 7565 721b 0000 0072 1400 0000  _valuer....r....
-000014f0: 5a0f 696e 6465 785f 6469 6d65 6e73 696f  Z.index_dimensio
-00001500: 6eda 0a6c 6173 745f 7661 6c75 6572 2500  n..last_valuer%.
-00001510: 0000 7225 0000 0072 2600 0000 da0e 7661  ..r%...r&.....va
-00001520: 725f 6173 7369 676e 6d65 6e74 8700 0000  r_assignment....
-00001530: 7344 0000 000e 0104 0104 010a 010c 010a  sD..............
-00001540: 0102 0206 0102 0104 ff06 0206 fe0c 0308  ................
-00001550: 0102 ff0a 0304 0212 010c 010a 0212 010e  ................
-00001560: 0104 010a 010a 0106 0112 0204 0104 ff06  ................
-00001570: 0302 0206 0106 ff0a 037a 1e46 6f61 6d54  .........z.FoamT
-00001580: 7261 6e73 666f 726d 6572 2e76 6172 5f61  ransformer.var_a
-00001590: 7373 6967 6e6d 656e 7463 0200 0000 0000  ssignmentc......
-000015a0: 0000 0000 0000 0800 0000 0700 0000 4300  ..............C.
-000015b0: 0000 7316 0100 0074 007c 0183 017d 0164  ..s....t.|...}.d
-000015c0: 007d 0274 017c 0183 0164 016b 0272 1a7c  .}.t.|...d.k.r.|
-000015d0: 01a0 0264 02a1 017d 0374 037c 0374 0469  ...d...}.t.|.t.i
-000015e0: 007c 0364 038d 0283 0253 0067 007d 047c  .|.d.....S.g.}.|
-000015f0: 0144 005d 137d 0574 057c 0574 0683 0272  .D.].}.t.|.t...r
-00001600: 317c 05a0 0764 04a1 0172 317c 01a0 0264  1|...d...r1|...d
-00001610: 01a1 017d 0201 006e 0171 1e74 057c 0164  ...}...n.q.t.|.d
-00001620: 0219 0074 0883 0272 4664 0564 06a0 097c  ...t...rFd.d...|
-00001630: 01a0 0264 02a1 01a1 0117 0064 0717 007d  ...d.......d...}
-00001640: 036e 057c 01a0 0264 02a1 017d 037c 0472  .n.|...d...}.|.r
-00001650: 567c 0364 0664 06a0 097c 04a1 0117 0037  V|.d.d...|.....7
-00001660: 007d 0364 0864 0984 007c 0144 0083 017d  .}.d.d...|.D...}
-00001670: 067c 0644 005d 0f7d 0574 057c 056a 0a74  .|.D.].}.t.|.j.t
-00001680: 0b83 0272 6e7c 056a 0aa0 0c7c 056a 0da1  ...rn|.j...|.j..
-00001690: 0101 0071 5f7c 0264 0075 0172 7a7c 0264  ...q_|.d.u.rz|.d
-000016a0: 0a6b 0272 7a74 0e7d 076e 0274 047d 0774  .k.rzt.}.n.t.}.t
-000016b0: 037c 037c 0764 0b64 0c84 007c 0644 0083  .|.|.d.d...|.D..
-000016c0: 017c 037c 0264 0d8d 0383 0253 0029 0e4e  .|.|.d.....S.).N
-000016d0: 7208 0000 0072 0100 0000 2902 da04 6461  r....r....)...da
-000016e0: 7461 721b 0000 00fa 0123 fa01 2872 7000  tar......#..(rp.
-000016f0: 0000 fa01 2963 0100 0000 0000 0000 0000  ....)c..........
-00001700: 0000 0200 0000 0500 0000 5300 0000 7324  ..........S...s$
-00001710: 0000 0067 007c 005d 0e7d 0174 007c 0164  ...g.|.].}.t.|.d
-00001720: 0083 0272 0274 007c 0164 0183 0272 027c  ...r.t.|.d...r.|
-00001730: 0191 0271 0253 0072 6400 0000 2901 da07  ...q.S.rd...)...
-00001740: 6861 7361 7474 7272 6500 0000 7225 0000  hasattrre...r%..
-00001750: 0072 2500 0000 7226 0000 0072 3e00 0000  .r%...r&...r>...
-00001760: c300 0000 725a 0000 007a 3346 6f61 6d54  ....rZ...z3FoamT
-00001770: 7261 6e73 666f 726d 6572 2e64 6963 745f  ransformer.dict_
-00001780: 6173 7369 676e 6d65 6e74 2e3c 6c6f 6361  assignment.<loca
-00001790: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7a0b  ls>.<listcomp>z.
-000017a0: 2363 6f64 6553 7472 6561 6d63 0100 0000  #codeStreamc....
-000017b0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-000017c0: 5300 0000 7263 0000 0072 2500 0000 7264  S...rc...r%...rd
-000017d0: 0000 0072 6500 0000 7225 0000 0072 2500  ...re...r%...r%.
-000017e0: 0000 7226 0000 0072 6700 0000 d500 0000  ..r&...rg.......
-000017f0: 7268 0000 007a 3346 6f61 6d54 7261 6e73  rh...z3FoamTrans
-00001800: 666f 726d 6572 2e64 6963 745f 6173 7369  former.dict_assi
-00001810: 676e 6d65 6e74 2e3c 6c6f 6361 6c73 3e2e  gnment.<locals>.
-00001820: 3c64 6963 7463 6f6d 703e 2903 7279 0000  <dictcomp>).ry..
-00001830: 0072 1b00 0000 7261 0000 0029 0f72 4100  .r....ra...).rA.
-00001840: 0000 725f 0000 0072 7300 0000 7209 0000  ..r_...rs...r...
-00001850: 0072 0c00 0000 7258 0000 0072 2200 0000  .r....rX...r"...
-00001860: da0a 7374 6172 7473 7769 7468 7262 0000  ..startswithrb..
-00001870: 0072 2d00 0000 7214 0000 0072 1000 0000  .r-...r....r....
-00001880: 7269 0000 0072 1b00 0000 720b 0000 0029  ri...r....r....)
-00001890: 0872 4700 0000 724f 0000 0072 6100 0000  .rG...rO...ra...
-000018a0: 721b 0000 005a 096e 6f64 6573 5f73 7472  r....Z.nodes_str
-000018b0: 7266 0000 005a 0c6e 6f64 6573 5f61 7373  rf...Z.nodes_ass
-000018c0: 6967 6eda 0363 6c73 7225 0000 0072 2500  ign..clsr%...r%.
-000018d0: 0000 7226 0000 00da 0f64 6963 745f 6173  ..r&.....dict_as
-000018e0: 7369 676e 6d65 6e74 ae00 0000 7344 0000  signment....sD..
-000018f0: 0008 0104 010c 020a 0112 0104 0208 0114  ................
-00001900: 010a 0204 0102 800e 011a 010a 0204 0112  ................
-00001910: 0106 0202 0206 fe08 060c 010e 0102 8010  ................
-00001920: 0206 0104 0202 0202 0102 010c 0102 0102  ................
-00001930: 0104 fd04 fe7a 1f46 6f61 6d54 7261 6e73  .....z.FoamTrans
-00001940: 666f 726d 6572 2e64 6963 745f 6173 7369  former.dict_assi
-00001950: 676e 6d65 6e74 6302 0000 0000 0000 0000  gnmentc.........
-00001960: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
-00001970: 2e00 0000 7400 7c01 8301 7d01 7401 7c01  ....t.|...}.t.|.
-00001980: 8301 6401 6b03 720e 7402 7c01 8301 8201  ..d.k.r.t.|.....
-00001990: 6400 7d02 7403 7c02 7c01 6402 1900 8302  d.}.t.|.|.d.....
-000019a0: 5300 725e 0000 0029 0472 4100 0000 725f  S.r^...).rA...r_
-000019b0: 0000 00da 134e 6f74 496d 706c 656d 656e  .....NotImplemen
-000019c0: 7465 6445 7272 6f72 7209 0000 00a9 0372  tedErrorr......r
-000019d0: 4700 0000 724f 0000 0072 1b00 0000 7225  G...rO...r....r%
-000019e0: 0000 0072 2500 0000 7226 0000 00da 0d69  ...r%...r&.....i
-000019f0: 736f 6c61 7465 645f 6c69 7374 db00 0000  solated_list....
-00001a00: 730a 0000 0008 010c 0108 0104 010e 017a  s..............z
-00001a10: 1d46 6f61 6d54 7261 6e73 666f 726d 6572  .FoamTransformer
-00001a20: 2e69 736f 6c61 7465 645f 6c69 7374 6302  .isolated_listc.
-00001a30: 0000 0000 0000 0000 0000 0008 0000 0006  ................
-00001a40: 0000 0043 0000 0073 ac00 0000 7400 7c01  ...C...s....t.|.
-00001a50: 8301 7d01 6400 7d02 7401 7c01 8301 4400  ..}.d.}.t.|...D.
-00001a60: 5d18 5c02 7d03 7d04 7402 7c04 7403 8302  ].\.}.}.t.|.t...
-00001a70: 7222 7c04 6a04 6401 6b02 7222 7405 7c04  r"|.j.d.k.r"t.|.
-00001a80: 8301 6402 6403 8502 1900 7d02 0100 6e01  ..d.d.....}...n.
-00001a90: 710a 7c02 6400 7501 722c 7c01 a006 7c03  q.|.d.u.r,|...|.
-00001aa0: a101 0100 6400 7d05 7407 7c01 8301 6404  ....d.}.t.|...d.
-00001ab0: 6b04 7240 7402 7c01 6403 1900 7408 8302  k.r@t.|.d...t...
-00001ac0: 7240 7c01 a006 6403 a101 7d05 7c01 a006  r@|...d...}.|...
-00001ad0: 6405 a101 7d06 6400 7d07 7c01 724e 6406  d...}.d.}.|.rNd.
-00001ae0: a009 7c01 a101 7d07 740a 7c06 7c07 7c02  ..|...}.t.|.|.|.
-00001af0: 7c05 6407 8d04 5300 2908 4e5a 094c 4953  |.d...S.).NZ.LIS
-00001b00: 545f 5459 5045 e905 0000 0072 7100 0000  T_TYPE.....rq...
-00001b10: 7208 0000 0072 0100 0000 7270 0000 0029  r....r....rp...)
-00001b20: 0472 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-00001b30: 721e 0000 0029 0b72 4100 0000 da09 656e  r....).rA.....en
-00001b40: 756d 6572 6174 6572 5800 0000 7205 0000  umeraterX...r...
-00001b50: 0072 5900 0000 7222 0000 0072 7300 0000  .rY...r"...rs...
-00001b60: 725f 0000 0072 2400 0000 722d 0000 0072  r_...r$...r-...r
-00001b70: 1a00 0000 2908 7247 0000 0072 4f00 0000  ....).rG...rO...
-00001b80: 721d 0000 00da 0569 6e6f 6465 7266 0000  r......inoderf..
-00001b90: 0072 1e00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00001ba0: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
-00001bb0: 096c 6973 745f 696e 666f e200 0000 7322  .list_info....s"
-00001bc0: 0000 0008 0104 0210 0114 0110 0104 0102  ................
-00001bd0: 8008 010a 0104 021a 010a 010a 0204 0204  ................
-00001be0: 010a 0110 027a 1946 6f61 6d54 7261 6e73  .....z.FoamTrans
-00001bf0: 666f 726d 6572 2e6c 6973 745f 696e 666f  former.list_info
-00001c00: 6302 0000 0000 0000 0000 0000 0006 0000  c...............
-00001c10: 0004 0000 0043 0000 0073 aa00 0000 7400  .....C...s....t.
-00001c20: 7c01 8301 7d01 7c01 5c02 7d02 7d03 7401  |...}.|.\.}.}.t.
-00001c30: 7c02 7402 8302 730f 4a00 8201 7c02 6a03  |.t...s.J...|.j.
-00001c40: 7d04 7c04 7d05 7c02 6a04 6400 7501 7220  }.|.}.|.j.d.u.r 
-00001c50: 7c05 6401 7c02 6a04 1700 3700 7d05 7c02  |.d.|.j...7.}.|.
-00001c60: 6a05 6400 7501 722e 7c05 6402 7c02 6a05  j.d.u.r.|.d.|.j.
-00001c70: 9b00 6403 9d03 3700 7d05 7c02 6a06 6400  ..d...7.}.|.j.d.
-00001c80: 7501 723b 7c05 6404 7c02 6a06 9b00 9d02  u.r;|.d.|.j.....
-00001c90: 3700 7d05 7401 7c04 7407 8302 7244 7408  7.}.t.|.t...rDt.
-00001ca0: 7c04 8301 7d04 7401 7c05 7407 8302 724d  |...}.t.|.t...rM
-00001cb0: 7408 7c05 8301 7d05 7c05 7c03 5f09 740a  t.|...}.|.|._.t.
-00001cc0: 7c04 7c03 8302 5300 2905 4e72 7000 0000  |.|...S.).Nrp...
-00001cd0: 7a06 0a4c 6973 743c fa01 3e72 2700 0000  z..List<..>r'...
-00001ce0: 290b 7241 0000 0072 5800 0000 721a 0000  ).rA...rX...r...
-00001cf0: 0072 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-00001d00: 721e 0000 0072 2400 0000 7222 0000 0072  r....r$...r"...r
-00001d10: 7600 0000 7209 0000 0029 0672 4700 0000  v...r....).rG...
-00001d20: 724f 0000 0072 8700 0000 5a08 7468 655f  rO...r....Z.the_
-00001d30: 6c69 7374 721b 0000 005a 0d6e 616d 655f  listr....Z.name_
-00001d40: 696e 7465 726e 616c 7225 0000 0072 2500  internalr%...r%.
-00001d50: 0000 7226 0000 00da 0f6c 6973 745f 6173  ..r&.....list_as
-00001d60: 7369 676e 6d65 6e74 f900 0000 7322 0000  signment....s"..
-00001d70: 0008 0108 020e 0106 0204 010a 020e 010a  ................
-00001d80: 0212 010a 0210 010a 0208 010a 0108 0106  ................
-00001d90: 020a 017a 1f46 6f61 6d54 7261 6e73 666f  ...z.FoamTransfo
-00001da0: 726d 6572 2e6c 6973 745f 6173 7369 676e  rmer.list_assign
-00001db0: 6d65 6e74 6302 0000 0000 0000 0000 0000  mentc...........
-00001dc0: 0003 0000 0007 0000 0043 0000 0073 7000  .........C...sp.
-00001dd0: 0000 6401 6402 8400 7c01 4400 8301 7d01  ..d.d...|.D...}.
-00001de0: 7c01 a000 6403 a101 7d02 7401 7c01 8301  |...d...}.t.|...
-00001df0: 6404 6b02 7221 7402 7c02 7403 7c01 6405  d.k.r!t.|.t.|.d.
-00001e00: 1900 7c01 6403 1900 7c01 6406 1900 8303  ..|.d...|.d.....
-00001e10: 8302 5300 7401 7c01 8301 6407 6b02 7234  ..S.t.|...d.k.r4
-00001e20: 7402 7c02 7403 7c01 6405 1900 7c01 6406  t.|.t.|.d...|.d.
-00001e30: 1900 6408 8d02 8302 5300 7404 7c01 8301  ..d.....S.t.|...
-00001e40: 8201 2909 4e63 0100 0000 0000 0000 0000  ..).Nc..........
-00001e50: 0000 0200 0000 0400 0000 5300 0000 723b  ..........S...r;
-00001e60: 0000 0072 2800 0000 7225 0000 0072 6500  ...r(...r%...re.
-00001e70: 0000 7225 0000 0072 2500 0000 7226 0000  ..r%...r%...r&..
-00001e80: 0072 3e00 0000 1401 0000 723f 0000 007a  .r>.......r?...z
-00001e90: 3846 6f61 6d54 7261 6e73 666f 726d 6572  8FoamTransformer
-00001ea0: 2e64 696d 656e 7369 6f6e 5f61 7373 6967  .dimension_assig
-00001eb0: 6e6d 656e 742e 3c6c 6f63 616c 733e 2e3c  nment.<locals>.<
-00001ec0: 6c69 7374 636f 6d70 3e72 0100 0000 e903  listcomp>r......
-00001ed0: 0000 0072 7100 0000 e9fe ffff ffe9 0200  ...rq...........
-00001ee0: 0000 2901 7272 0000 0029 0572 7300 0000  ..).rr...).rs...
-00001ef0: 725f 0000 0072 0900 0000 7212 0000 0072  r_...r....r....r
-00001f00: 6000 0000 7282 0000 0072 2500 0000 7225  `...r....r%...r%
-00001f10: 0000 0072 2600 0000 da14 6469 6d65 6e73  ...r&.....dimens
-00001f20: 696f 6e5f 6173 7369 676e 6d65 6e74 1301  ion_assignment..
-00001f30: 0000 730e 0000 000e 010a 010c 021e 010c  ..s.............
-00001f40: 011a 0108 027a 2446 6f61 6d54 7261 6e73  .....z$FoamTrans
-00001f50: 666f 726d 6572 2e64 696d 656e 7369 6f6e  former.dimension
-00001f60: 5f61 7373 6967 6e6d 656e 7463 0200 0000  _assignmentc....
-00001f70: 0000 0000 0000 0000 0300 0000 0300 0000  ................
-00001f80: 4300 0000 7336 0000 0064 0164 0284 007c  C...s6...d.d...|
-00001f90: 0144 0083 017d 0174 007c 0183 0164 036b  .D...}.t.|...d.k
-00001fa0: 0372 1174 017c 0183 0182 017c 01a0 0264  .r.t.|.....|...d
-00001fb0: 04a1 017d 0274 037c 0264 0583 0253 0029  ...}.t.|.d...S.)
-00001fc0: 064e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
-00001fd0: 0000 0004 0000 0053 0000 0072 3b00 0000  .......S...r;...
-00001fe0: 7228 0000 0072 2500 0000 7265 0000 0072  r(...r%...re...r
-00001ff0: 2500 0000 7225 0000 0072 2600 0000 723e  %...r%...r&...r>
-00002000: 0000 001f 0100 0072 3f00 0000 7a34 466f  .......r?...z4Fo
-00002010: 616d 5472 616e 7366 6f72 6d65 722e 6d61  amTransformer.ma
-00002020: 6372 6f5f 6173 7369 676e 6d65 6e74 2e3c  cro_assignment.<
-00002030: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00002040: 703e 7208 0000 0072 0100 0000 da00 2904  p>r....r......).
-00002050: 725f 0000 0072 8100 0000 7273 0000 0072  r_...r....rs...r
-00002060: 0900 0000 7282 0000 0072 2500 0000 7225  ....r....r%...r%
-00002070: 0000 0072 2600 0000 da10 6d61 6372 6f5f  ...r&.....macro_
-00002080: 6173 7369 676e 6d65 6e74 1e01 0000 730a  assignment....s.
-00002090: 0000 000e 010c 0108 010a 010a 017a 2046  .............z F
-000020a0: 6f61 6d54 7261 6e73 666f 726d 6572 2e6d  oamTransformer.m
-000020b0: 6163 726f 5f61 7373 6967 6e6d 656e 7463  acro_assignmentc
-000020c0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-000020d0: 0300 0000 4300 0000 734e 0000 0064 0164  ....C...sN...d.d
-000020e0: 0284 007c 0144 0083 017d 0174 007c 0183  ...|.D...}.t.|..
-000020f0: 0164 036b 0372 1174 017c 0183 0182 017c  .d.k.r.t.|.....|
-00002100: 0164 0419 007d 0274 027c 0264 0583 0272  .d...}.t.|.d...r
-00002110: 1e7c 02a0 03a1 007d 027c 0164 0619 009b  .|.....}.|.d....
-00002120: 0064 077c 029b 009d 0353 0029 084e 6301  .d.|.....S.).Nc.
-00002130: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00002140: 0000 0053 0000 0072 3b00 0000 7228 0000  ...S...r;...r(..
-00002150: 0072 2500 0000 7265 0000 0072 2500 0000  .r%...re...r%...
-00002160: 7225 0000 0072 2600 0000 723e 0000 0026  r%...r&...r>...&
-00002170: 0100 0072 3f00 0000 7a30 466f 616d 5472  ...r?...z0FoamTr
-00002180: 616e 7366 6f72 6d65 722e 6571 7561 6c5f  ansformer.equal_
-00002190: 6173 7369 676e 2e3c 6c6f 6361 6c73 3e2e  assign.<locals>.
-000021a0: 3c6c 6973 7463 6f6d 703e 728c 0000 0072  <listcomp>r....r
-000021b0: 0800 0000 7239 0000 0072 0100 0000 fa01  ....r9...r......
-000021c0: 3d29 0472 5f00 0000 7260 0000 0072 7d00  =).r_...r`...r}.
-000021d0: 0000 7239 0000 0029 0372 4700 0000 724f  ..r9...).rG...rO
-000021e0: 0000 0072 1400 0000 7225 0000 0072 2500  ...r....r%...r%.
-000021f0: 0000 7226 0000 00da 0c65 7175 616c 5f61  ..r&.....equal_a
-00002200: 7373 6967 6e25 0100 0073 0e00 0000 0e01  ssign%...s......
-00002210: 0c01 0801 0801 0a01 0801 1201 7a1c 466f  ............z.Fo
-00002220: 616d 5472 616e 7366 6f72 6d65 722e 6571  amTransformer.eq
-00002230: 7561 6c5f 6173 7369 676e 6302 0000 0000  ual_assignc.....
-00002240: 0000 0000 0000 0007 0000 0005 0000 0043  ...............C
-00002250: 0000 0073 6e00 0000 6401 6402 8400 7c01  ...sn...d.d...|.
-00002260: 4400 8301 7d01 7400 7c01 8301 6403 6b02  D...}.t.|...d.k.
-00002270: 7212 7c01 5c02 7d02 7d03 6e17 7c01 a001  r.|.\.}.}.n.|...
-00002280: 6404 a101 7d02 7c01 a001 6404 a101 7d04  d...}.|...d...}.
-00002290: 6405 a002 7c01 a101 7d05 7c04 6406 7c05  d...|...}.|.d.|.
-000022a0: 9b00 6407 9d03 1700 7d03 7c02 6408 1700  ..d.....}.|.d...
-000022b0: 7c03 1700 7d06 7403 7c06 7404 7c02 7c03  |...}.t.|.t.|.|.
-000022c0: 8302 8302 5300 2909 4e63 0100 0000 0000  ....S.).Nc......
-000022d0: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-000022e0: 0000 723b 0000 0072 2800 0000 7225 0000  ..r;...r(...r%..
-000022f0: 0072 6500 0000 7225 0000 0072 2500 0000  .re...r%...r%...
-00002300: 7226 0000 0072 3e00 0000 2f01 0000 723f  r&...r>.../...r?
-00002310: 0000 007a 3846 6f61 6d54 7261 6e73 666f  ...z8FoamTransfo
-00002320: 726d 6572 2e64 6972 6563 7469 7665 5f61  rmer.directive_a
-00002330: 7373 6967 6e6d 656e 742e 3c6c 6f63 616c  ssignment.<local
-00002340: 733e 2e3c 6c69 7374 636f 6d70 3e72 8c00  s>.<listcomp>r..
-00002350: 0000 7201 0000 007a 022c 2072 7b00 0000  ..r....z., r{...
-00002360: 727c 0000 0072 7000 0000 2905 725f 0000  r|...rp...).r_..
-00002370: 0072 7300 0000 722d 0000 0072 0900 0000  .rs...r-...r....
-00002380: 720e 0000 0029 0772 4700 0000 724f 0000  r....).rG...rO..
-00002390: 0072 6100 0000 da07 636f 6e74 656e 745a  .ra.....contentZ
-000023a0: 0d66 756e 6374 696f 6e5f 6e61 6d65 da09  .function_name..
-000023b0: 6172 6775 6d65 6e74 73da 036b 6579 7225  arguments..keyr%
-000023c0: 0000 0072 2500 0000 7226 0000 00da 1464  ...r%...r&.....d
-000023d0: 6972 6563 7469 7665 5f61 7373 6967 6e6d  irective_assignm
-000023e0: 656e 742e 0100 0073 1200 0000 0e01 0c01  ent....s........
-000023f0: 0a01 0a02 0a01 0a01 1001 0c01 1001 7a24  ..............z$
-00002400: 466f 616d 5472 616e 7366 6f72 6d65 722e  FoamTransformer.
-00002410: 6469 7265 6374 6976 655f 6173 7369 676e  directive_assign
-00002420: 6d65 6e74 6302 0000 0000 0000 0000 0000  mentc...........
-00002430: 0005 0000 0007 0000 0043 0000 0073 ac00  .........C...s..
-00002440: 0000 7400 7c01 8301 7d01 6400 7d02 7401  ..t.|...}.d.}.t.
-00002450: 7c01 8301 6401 6b02 7211 7c01 5c02 7d03  |...d.k.r.|.\.}.
-00002460: 7d04 6e19 7401 7c01 8301 6402 6b02 7226  }.n.t.|...d.k.r&
-00002470: 7c01 5c03 7d03 7d02 7d04 7c02 a002 6403  |.\.}.}.}.|...d.
-00002480: a101 7325 7403 7c01 8301 8201 6e04 7403  ..s%t.|.....n.t.
-00002490: 7c01 8301 8201 7404 7c04 8301 7d04 7c04  |.....t.|...}.|.
-000024a0: a002 6404 a101 7244 7c04 a005 6405 6406  ..d...rD|...d.d.
-000024b0: a102 6407 1900 7d04 7c04 a006 6405 6406  ..d...}.|...d.d.
-000024c0: a102 6408 1900 7d04 6e08 7c04 6401 6409  ..d...}.n.|.d.d.
-000024d0: 8502 1900 a007 a100 7d04 7408 7c03 7409  ........}.t.|.t.
-000024e0: 7c03 7c04 7c02 640a 8d03 8302 5300 290b  |.|.|.d.....S.).
-000024f0: 4e72 8c00 0000 728a 0000 0072 7a00 0000  Nr....r....rz...
-00002500: 7a03 237b 0a72 2700 0000 7208 0000 0072  z.#{.r'...r....r
-00002510: 7100 0000 7201 0000 00e9 fdff ffff 2901  q...r.........).
-00002520: 7261 0000 0029 0a72 4100 0000 725f 0000  ra...).rA...r_..
-00002530: 0072 7e00 0000 7281 0000 0072 2200 0000  .r~...r....r"...
-00002540: 722e 0000 00da 0672 7370 6c69 74da 0573  r......rsplit..s
-00002550: 7472 6970 7209 0000 0072 0a00 0000 2905  tripr....r....).
-00002560: 7247 0000 0072 4f00 0000 7261 0000 0072  rG...rO...ra...r
-00002570: 1b00 0000 da04 636f 6465 7225 0000 0072  ......coder%...r
-00002580: 2500 0000 7226 0000 00da 0f63 6f64 655f  %...r&.....code_
-00002590: 6173 7369 676e 6d65 6e74 3a01 0000 7320  assignment:...s 
-000025a0: 0000 0008 0104 010c 010a 010c 010a 010a  ................
-000025b0: 0108 0102 ff08 0308 010a 0110 0112 0110  ................
-000025c0: 0214 017a 1f46 6f61 6d54 7261 6e73 666f  ...z.FoamTransfo
-000025d0: 726d 6572 2e63 6f64 655f 6173 7369 676e  rmer.code_assign
-000025e0: 6d65 6e74 6302 0000 0000 0000 0000 0000  mentc...........
-000025f0: 0002 0000 0003 0000 0043 0000 0073 1a00  .........C...s..
-00002600: 0000 7400 7c01 8301 7d01 7401 7c01 6401  ..t.|...}.t.|.d.
-00002610: 1900 6a02 6402 1700 8301 5300 2903 4e72  ..j.d.....S.).Nr
-00002620: 0100 0000 7227 0000 0029 0372 4100 0000  ....r'...).rA...
-00002630: 7211 0000 0072 1400 0000 7246 0000 0072  r....r....rF...r
-00002640: 2500 0000 7225 0000 0072 2600 0000 da12  %...r%...r&.....
-00002650: 7370 6563 6961 6c5f 6469 7265 6374 6976  special_directiv
-00002660: 6573 4d01 0000 7304 0000 0008 0112 017a  esM...s........z
-00002670: 2246 6f61 6d54 7261 6e73 666f 726d 6572  "FoamTransformer
-00002680: 2e73 7065 6369 616c 5f64 6972 6563 7469  .special_directi
-00002690: 7665 734e 291a 721f 0000 0072 2000 0000  vesN).r....r ...
-000026a0: 7221 0000 0072 4900 0000 724c 0000 0072  r!...rI...rL...r
-000026b0: 5000 0000 7251 0000 0072 5200 0000 7253  P...rQ...rR...rS
-000026c0: 0000 0072 5400 0000 7255 0000 0072 5c00  ...rT...rU...r\.
-000026d0: 0000 7261 0000 0072 6200 0000 726b 0000  ..ra...rb...rk..
-000026e0: 0072 7800 0000 7280 0000 0072 8300 0000  .rx...r....r....
-000026f0: 7287 0000 0072 8900 0000 728d 0000 0072  r....r....r....r
-00002700: 8f00 0000 7291 0000 0072 9500 0000 729a  ....r....r....r.
-00002710: 0000 0072 9b00 0000 7225 0000 0072 2500  ...r....r%...r%.
-00002720: 0000 7225 0000 0072 2600 0000 7234 0000  ..r%...r&...r4..
-00002730: 0048 0000 0073 3000 0000 0800 0801 0803  .H...s0.........
-00002740: 0803 0803 0803 0803 0803 0803 0803 0809  ................
-00002750: 0805 080a 080e 0827 082d 0807 0817 081a  .......'.-......
-00002760: 080b 0807 0809 080c 0c13 7234 0000 0072  ..........r4...r
-00002770: 2800 0000 2926 da0b 6461 7461 636c 6173  (...)&..dataclas
-00002780: 7365 7372 0200 0000 da07 7061 7468 6c69  sesr......pathli
-00002790: 6272 0300 0000 da04 6c61 726b 7204 0000  br......larkr...
-000027a0: 0072 0500 0000 7206 0000 00da 0f6c 6172  .r....r......lar
-000027b0: 6b2e 6578 6365 7074 696f 6e73 7207 0000  k.exceptionsr...
-000027c0: 00da 0361 7374 7209 0000 0072 0a00 0000  ...astr....r....
-000027d0: 720b 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
-000027e0: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
-000027f0: 0000 0072 1200 0000 7213 0000 00da 085f  ...r....r......_
-00002800: 5f66 696c 655f 5fda 0861 6273 6f6c 7574  _file__..absolut
-00002810: 65da 0670 6172 656e 74da 0468 6572 65da  e..parent..here.
-00002820: 0972 6561 645f 7465 7874 7237 0000 005a  .read_textr7...Z
-00002830: 1067 7261 6d6d 6172 5f61 6476 616e 6365  .grammar_advance
-00002840: 6472 3000 0000 7232 0000 0072 3300 0000  dr0...r2...r3...
-00002850: 721a 0000 0072 3100 0000 7239 0000 0072  r....r1...r9...r
-00002860: 4100 0000 7245 0000 0072 3400 0000 7225  A...rE...r4...r%
-00002870: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
-00002880: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00002890: 7324 0000 000c 000c 0114 020c 0134 020e  s$...........4..
-000028a0: 0e0c 020c 010e 020e 010a 0202 0310 010a  ................
-000028b0: 0708 1008 0408 0414 08                   .........
+00000090: 6d14 5a14 6d15 5a15 6d16 5a16 0100 6504  m.Z.m.Z.m.Z...e.
+000000a0: 6517 8301 a018 a100 6a19 5a1a 651a 6408  e.......j.Z.e.d.
+000000b0: 1b00 a01b a100 5a1c 651a 6409 1b00 a01b  ......Z.e.d.....
+000000c0: a100 5a1d 6506 651c 640a 640b 640c 8d03  ..Z.e.e.d.d.d...
+000000d0: 5a1e 6506 651d 640a 640b 640c 8d03 5a1f  Z.e.e.d.d.d...Z.
+000000e0: 651e 651f 640d 9c02 5a20 6502 4700 640e  e.e.d...Z e.G.d.
+000000f0: 640f 8400 640f 8302 8301 5a21 641b 6411  d...d.....Z!d.d.
+00000100: 6412 8401 5a22 6413 6414 8400 5a23 6415  d...Z"d.d...Z#d.
+00000110: 6416 8400 5a24 6417 6418 8400 5a25 4700  d...Z$d.d...Z%G.
+00000120: 6419 641a 8400 641a 6508 8303 5a26 6410  d.d...d.e...Z&d.
+00000130: 5300 291c 7a1f 5061 7273 6572 2066 6f72  S.).z.Parser for
+00000140: 204f 7065 6e46 4f41 4d20 696e 7075 7420   OpenFOAM input 
+00000150: 6669 6c65 73e9 0000 0000 2901 da09 6461  files.....)...da
+00000160: 7461 636c 6173 7329 01da 0450 6174 6829  taclass)...Path)
+00000170: 03da 044c 6172 6bda 0554 6f6b 656e da0b  ...Lark..Token..
+00000180: 5472 616e 7366 6f72 6d65 7229 01da 094c  Transformer)...L
+00000190: 6172 6b45 7272 6f72 e901 0000 0029 0bda  arkError.....)..
+000001a0: 0a41 7373 6967 6e6d 656e 74da 0443 6f64  .Assignment..Cod
+000001b0: 65da 0a43 6f64 6553 7472 6561 6dda 0444  e..CodeStream..D
+000001c0: 6963 74da 0c44 696d 656e 7369 6f6e 5365  ict..DimensionSe
+000001d0: 74da 0944 6972 6563 7469 7665 da0d 466f  t..Directive..Fo
+000001e0: 616d 496e 7075 7446 696c 65da 044c 6973  amInputFile..Lis
+000001f0: 74da 044e 616d 65da 0556 616c 7565 da12  t..Name..Value..
+00000200: 5661 7269 6162 6c65 4173 7369 676e 6d65  VariableAssignme
+00000210: 6e74 7a0c 6772 616d 6d61 722e 6c61 726b  ntz.grammar.lark
+00000220: 7a15 6772 616d 6d61 725f 6164 7661 6e63  z.grammar_advanc
+00000230: 6564 2e6c 6172 6bda 0576 616c 7565 da05  ed.lark..value..
+00000240: 6261 7369 6329 02da 0573 7461 7274 da05  basic)...start..
+00000250: 6c65 7865 7229 02da 0673 696d 706c 655a  lexer)...simpleZ
+00000260: 0861 6476 616e 6365 6463 0000 0000 0000  .advancedc......
+00000270: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
+00000280: 0000 733a 0000 0065 005a 0164 005a 0255  ..s:...e.Z.d.Z.U
+00000290: 0065 0365 0464 013c 0064 025a 0565 0365  .e.e.d.<.d.Z.e.e
+000002a0: 0464 033c 0064 025a 0665 0365 0464 043c  .d.<.d.Z.e.e.d.<
+000002b0: 0064 025a 0765 0865 0464 053c 0064 0253  .d.Z.e.e.d.<.d.S
+000002c0: 0029 06da 084c 6973 7449 6e66 6fda 046e  .)...ListInfo..n
+000002d0: 616d 654e da04 696e 666f da05 6474 7970  ameN..info..dtyp
+000002e0: 65da 0473 697a 6529 09da 085f 5f6e 616d  e..size)...__nam
+000002f0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000300: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0373  .__qualname__..s
+00000310: 7472 da0f 5f5f 616e 6e6f 7461 7469 6f6e  tr..__annotation
+00000320: 735f 5f72 1b00 0000 721c 0000 0072 1d00  s__r....r....r..
+00000330: 0000 da03 696e 74a9 0072 2400 0000 7224  ....int..r$...r$
+00000340: 0000 00fa 492f 686f 6d65 2f70 6965 7272  ....I/home/pierr
+00000350: 652f 4465 762f 666c 7569 6473 696d 666f  e/Dev/fluidsimfo
+00000360: 616d 2f73 7263 2f66 6c75 6964 7369 6d66  am/src/fluidsimf
+00000370: 6f61 6d2f 666f 616d 5f69 6e70 7574 5f66  oam/foam_input_f
+00000380: 696c 6573 2f70 6172 7365 722e 7079 7219  iles/parser.pyr.
+00000390: 0000 0022 0000 0073 0a00 0000 0a00 0802  ..."...s........
+000003a0: 0c01 0c01 1001 7219 0000 004e 6302 0000  ......r....Nc...
+000003b0: 0000 0000 0000 0000 0003 0000 0008 0000  ................
+000003c0: 0043 0000 0073 7a00 0000 6401 a000 6402  .C...sz...d...d.
+000003d0: 6403 8400 7c00 a001 6401 a101 4400 8301  d...|...d...D...
+000003e0: a101 7d00 7c00 a002 6401 a101 7316 7c00  ..}.|...d...s.|.
+000003f0: 6401 3700 7d00 7c01 6400 7500 7230 7a07  d.7.}.|.d.u.r0z.
+00000400: 7403 a004 7c00 a101 7d02 5700 6e15 0400  t...|...}.W.n...
+00000410: 7405 792f 0100 0100 0100 7406 a004 7c00  t.y/......t...|.
+00000420: a101 7d02 5900 6e08 7700 7407 7c01 1900  ..}.Y.n.w.t.|...
+00000430: a004 7c00 a101 7d02 7408 8300 a009 7c02  ..|...}.t.....|.
+00000440: a101 5300 2904 4eda 010a 6301 0000 0000  ..S.).N...c.....
+00000450: 0000 0000 0000 0002 0000 0003 0000 0073  ...............s
+00000460: 0000 0073 1800 0000 8100 7c00 5d07 7d01  ...s......|.].}.
+00000470: 7c01 a000 a100 5600 0100 7102 6400 5300  |.....V...q.d.S.
+00000480: a901 4e29 01da 0672 7374 7269 7029 02da  ..N)...rstrip)..
+00000490: 022e 30da 046c 696e 6572 2400 0000 7224  ..0..liner$...r$
+000004a0: 0000 0072 2500 0000 da09 3c67 656e 6578  ...r%.....<genex
+000004b0: 7072 3e2b 0000 0073 0400 0000 0280 1600  pr>+...s........
+000004c0: 7a18 7061 7273 652e 3c6c 6f63 616c 733e  z.parse.<locals>
+000004d0: 2e3c 6765 6e65 7870 723e 290a da04 6a6f  .<genexpr>)...jo
+000004e0: 696e da05 7370 6c69 74da 0865 6e64 7377  in..split..endsw
+000004f0: 6974 68da 0b6c 6172 6b5f 7061 7273 6572  ith..lark_parser
+00000500: da05 7061 7273 6572 0700 0000 da14 6c61  ..parser......la
+00000510: 726b 5f70 6172 7365 725f 6164 7661 6e63  rk_parser_advanc
+00000520: 6564 da07 7061 7273 6572 73da 0f46 6f61  ed..parsers..Foa
+00000530: 6d54 7261 6e73 666f 726d 6572 da09 7472  mTransformer..tr
+00000540: 616e 7366 6f72 6d29 03da 0474 6578 74da  ansform)...text.
+00000550: 0767 7261 6d6d 6172 da04 7472 6565 7224  .grammar..treer$
+00000560: 0000 0072 2400 0000 7225 0000 0072 3000  ...r$...r%...r0.
+00000570: 0000 2a00 0000 7316 0000 001a 010a 0108  ..*...s.........
+00000580: 0108 0202 010e 010c 010e 0102 ff0e 030c  ................
+00000590: 0272 3000 0000 6301 0000 0000 0000 0000  .r0...c.........
+000005a0: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
+000005b0: 0800 0000 7c00 a000 a100 5300 7227 0000  ....|.....S.r'..
+000005c0: 0029 01da 0464 756d 7029 0172 3700 0000  .)...dump).r7...
+000005d0: 7224 0000 0072 2400 0000 7225 0000 0072  r$...r$...r%...r
+000005e0: 3800 0000 3a00 0000 f302 0000 0008 0172  8...:..........r
+000005f0: 3800 0000 6301 0000 0000 0000 0000 0000  8...c...........
+00000600: 0001 0000 0002 0000 0043 0000 0073 0e00  .........C...s..
+00000610: 0000 6401 6402 8400 7c00 4400 8301 5300  ..d.d...|.D...S.
+00000620: 2903 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
+00000630: 0200 0000 0400 0000 5300 0000 f318 0000  ........S.......
+00000640: 0067 007c 005d 087d 017c 0164 0075 0172  .g.|.].}.|.d.u.r
+00000650: 027c 0191 0271 0253 0072 2700 0000 7224  .|...q.S.r'...r$
+00000660: 0000 00a9 0272 2900 0000 da04 6974 656d  .....r).....item
+00000670: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
+00000680: 0a3c 6c69 7374 636f 6d70 3e3f 0000 00f3  .<listcomp>?....
+00000690: 0200 0000 1800 7a26 6669 6c74 6572 5f6e  ......z&filter_n
+000006a0: 6f5f 6e65 776c 696e 6573 2e3c 6c6f 6361  o_newlines.<loca
+000006b0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7224  ls>.<listcomp>r$
+000006c0: 0000 0029 01da 0569 7465 6d73 7224 0000  ...)...itemsr$..
+000006d0: 0072 2400 0000 7225 0000 00da 1266 696c  .r$...r%.....fil
+000006e0: 7465 725f 6e6f 5f6e 6577 6c69 6e65 733e  ter_no_newlines>
+000006f0: 0000 0073 0200 0000 0e01 7240 0000 0063  ...s......r@...c
+00000700: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000710: 0800 0000 4300 0000 732e 0000 0074 007c  ....C...s....t.|
+00000720: 0083 017d 007a 0574 017c 0083 0157 0053  ...}.z.t.|...W.S
+00000730: 0004 0074 0279 1601 0001 0001 0074 037c  ...t.y.......t.|
+00000740: 0083 0106 0059 0053 0077 0072 2700 0000  .....Y.S.w.r'...
+00000750: 2904 7221 0000 0072 2300 0000 da0a 5661  ).r!...r#.....Va
+00000760: 6c75 6545 7272 6f72 da05 666c 6f61 7429  lueError..float)
+00000770: 01da 066e 756d 6265 7272 2400 0000 7224  ...numberr$...r$
+00000780: 0000 0072 2500 0000 da12 5f63 6f6e 7665  ...r%....._conve
+00000790: 7274 5f74 6f5f 6e75 6d62 6572 4200 0000  rt_to_numberB...
+000007a0: 730c 0000 0008 0102 010a 010c 010c 0102  s...............
+000007b0: ff72 4400 0000 6300 0000 0000 0000 0000  .rD...c.........
+000007c0: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
+000007d0: c400 0000 6500 5a01 6400 5a02 6401 6402  ....e.Z.d.Z.d.d.
+000007e0: 8400 5a03 6403 6404 8400 5a04 6405 6406  ..Z.d.d...Z.d.d.
+000007f0: 8400 5a05 6407 6408 8400 5a06 6409 640a  ..Z.d.d...Z.d.d.
+00000800: 8400 5a07 640b 640c 8400 5a08 640d 640e  ..Z.d.d...Z.d.d.
+00000810: 8400 5a09 640f 6410 8400 5a0a 6411 6412  ..Z.d.d...Z.d.d.
+00000820: 8400 5a0b 6413 6414 8400 5a0c 6415 6416  ..Z.d.d...Z.d.d.
+00000830: 8400 5a0d 6417 6418 8400 5a0e 6419 641a  ..Z.d.d...Z.d.d.
+00000840: 8400 5a0f 641b 641c 8400 5a10 641d 641e  ..Z.d.d...Z.d.d.
+00000850: 8400 5a11 641f 6420 8400 5a12 6421 6422  ..Z.d.d ..Z.d!d"
+00000860: 8400 5a13 6423 6424 8400 5a14 6425 6426  ..Z.d#d$..Z.d%d&
+00000870: 8400 5a15 6427 6428 8400 5a16 6429 642a  ..Z.d'd(..Z.d)d*
+00000880: 8400 5a17 642b 642c 8400 5a18 642d 642e  ..Z.d+d,..Z.d-d.
+00000890: 8400 5a19 642f 5300 2930 7233 0000 0063  ..Z.d/S.)0r3...c
+000008a0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+000008b0: 0200 0000 4300 0000 7308 0000 0074 007c  ....C...s....t.|
+000008c0: 0183 0153 0072 2700 0000 2901 7244 0000  ...S.r'...).rD..
+000008d0: 00a9 02da 0473 656c 66da 0574 6f6b 656e  .....self..token
+000008e0: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
+000008f0: 0d53 4947 4e45 445f 4e55 4d42 4552 4b00  .SIGNED_NUMBERK.
+00000900: 0000 7239 0000 007a 1d46 6f61 6d54 7261  ..r9...z.FoamTra
+00000910: 6e73 666f 726d 6572 2e53 4947 4e45 445f  nsformer.SIGNED_
+00000920: 4e55 4d42 4552 6302 0000 0000 0000 0000  NUMBERc.........
+00000930: 0000 0002 0000 0001 0000 0043 0000 00f3  ...........C....
+00000940: 0600 0000 7c01 6a00 5300 7227 0000 00a9  ....|.j.S.r'....
+00000950: 0172 1400 0000 7245 0000 0072 2400 0000  .r....rE...r$...
+00000960: 7224 0000 0072 2500 0000 da05 434e 414d  r$...r%.....CNAM
+00000970: 454e 0000 00f3 0200 0000 0601 7a15 466f  EN..........z.Fo
+00000980: 616d 5472 616e 7366 6f72 6d65 722e 434e  amTransformer.CN
+00000990: 414d 4563 0200 0000 0000 0000 0000 0000  AMEc............
+000009a0: 0200 0000 0100 0000 4300 0000 7304 0000  ........C...s...
+000009b0: 0064 0053 0072 2700 0000 7224 0000 00a9  .d.S.r'...r$....
+000009c0: 0272 4600 0000 da05 6e6f 6465 7372 2400  .rF.....nodesr$.
+000009d0: 0000 7224 0000 0072 2500 0000 da07 4e45  ..r$...r%.....NE
+000009e0: 574c 494e 4551 0000 0073 0200 0000 0401  WLINEQ...s......
+000009f0: 7a17 466f 616d 5472 616e 7366 6f72 6d65  z.FoamTransforme
+00000a00: 722e 4e45 574c 494e 4563 0200 0000 0000  r.NEWLINEc......
+00000a10: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
+00000a20: 0000 7249 0000 0072 2700 0000 724a 0000  ..rI...r'...rJ..
+00000a30: 0072 4500 0000 7224 0000 0072 2400 0000  .rE...r$...r$...
+00000a40: 7225 0000 00da 0e45 5343 4150 4544 5f53  r%.....ESCAPED_S
+00000a50: 5452 494e 4754 0000 0072 4c00 0000 7a1e  TRINGT...rL...z.
+00000a60: 466f 616d 5472 616e 7366 6f72 6d65 722e  FoamTransformer.
+00000a70: 4553 4341 5045 445f 5354 5249 4e47 6302  ESCAPED_STRINGc.
+00000a80: 0000 0000 0000 0000 0000 0002 0000 0001  ................
+00000a90: 0000 0043 0000 0072 4900 0000 7227 0000  ...C...rI...r'..
+00000aa0: 0072 4a00 0000 7245 0000 0072 2400 0000  .rJ...rE...r$...
+00000ab0: 7224 0000 0072 2500 0000 da0b 444f 5542  r$...r%.....DOUB
+00000ac0: 4c45 5f4e 414d 4557 0000 0072 4c00 0000  LE_NAMEW...rL...
+00000ad0: 7a1b 466f 616d 5472 616e 7366 6f72 6d65  z.FoamTransforme
+00000ae0: 722e 444f 5542 4c45 5f4e 414d 4563 0200  r.DOUBLE_NAMEc..
+00000af0: 0000 0000 0000 0000 0000 0200 0000 0100  ................
+00000b00: 0000 4300 0000 7249 0000 0072 2700 0000  ..C...rI...r'...
+00000b10: 724a 0000 0072 4500 0000 7224 0000 0072  rJ...rE...r$...r
+00000b20: 2400 0000 7225 0000 00da 0b54 5249 504c  $...r%.....TRIPL
+00000b30: 455f 4e41 4d45 5a00 0000 724c 0000 007a  E_NAMEZ...rL...z
+00000b40: 1b46 6f61 6d54 7261 6e73 666f 726d 6572  .FoamTransformer
+00000b50: 2e54 5249 504c 455f 4e41 4d45 6302 0000  .TRIPLE_NAMEc...
+00000b60: 0000 0000 0000 0000 0002 0000 0001 0000  ................
+00000b70: 0043 0000 0072 4900 0000 7227 0000 0072  .C...rI...r'...r
+00000b80: 4a00 0000 7245 0000 0072 2400 0000 7224  J...rE...r$...r$
+00000b90: 0000 0072 2500 0000 da05 4551 4b45 595d  ...r%.....EQKEY]
+00000ba0: 0000 0072 4c00 0000 7a15 466f 616d 5472  ...rL...z.FoamTr
+00000bb0: 616e 7366 6f72 6d65 722e 4551 4b45 5963  ansformer.EQKEYc
+00000bc0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000bd0: 0100 0000 4300 0000 7249 0000 0072 2700  ....C...rI...r'.
+00000be0: 0000 724a 0000 0072 4500 0000 7224 0000  ..rJ...rE...r$..
+00000bf0: 0072 2400 0000 7225 0000 00da 054d 4143  .r$...r%.....MAC
+00000c00: 524f 6000 0000 724c 0000 007a 1546 6f61  RO`...rL...z.Foa
+00000c10: 6d54 7261 6e73 666f 726d 6572 2e4d 4143  mTransformer.MAC
+00000c20: 524f 6302 0000 0000 0000 0000 0000 0002  ROc.............
+00000c30: 0000 0003 0000 0043 0000 00f3 1200 0000  .......C........
+00000c40: 7400 6401 6402 8400 7c01 4400 8301 8301  t.d.d...|.D.....
+00000c50: 5300 2903 4e63 0100 0000 0000 0000 0000  S.).Nc..........
+00000c60: 0000 0200 0000 0500 0000 5300 0000 7324  ..........S...s$
+00000c70: 0000 0067 007c 005d 0e7d 0174 007c 0174  ...g.|.].}.t.|.t
+00000c80: 0183 0272 0e7c 016a 0264 006b 0273 027c  ...r.|.j.d.k.s.|
+00000c90: 0191 0271 0253 0029 0172 4f00 0000 a903  ...q.S.).rO.....
+00000ca0: da0a 6973 696e 7374 616e 6365 7205 0000  ..isinstancer...
+00000cb0: 00da 0474 7970 6572 3b00 0000 7224 0000  ...typer;...r$..
+00000cc0: 0072 2400 0000 7225 0000 0072 3d00 0000  .r$...r%...r=...
+00000cd0: 6500 0000 f310 0000 0006 0002 0208 0102  e...............
+00000ce0: fd08 0302 fd02 0106 ff7a 3146 6f61 6d54  .........z1FoamT
+00000cf0: 7261 6e73 666f 726d 6572 2e64 696d 656e  ransformer.dimen
+00000d00: 7369 6f6e 5f73 6574 2e3c 6c6f 6361 6c73  sion_set.<locals
+00000d10: 3e2e 3c6c 6973 7463 6f6d 703e 2901 720d  >.<listcomp>).r.
+00000d20: 0000 00a9 0272 4600 0000 723f 0000 0072  .....rF...r?...r
+00000d30: 2400 0000 7224 0000 0072 2500 0000 da0d  $...r$...r%.....
+00000d40: 6469 6d65 6e73 696f 6e5f 7365 7463 0000  dimension_setc..
+00000d50: 00f3 0a00 0000 0201 0601 0202 04fe 04ff  ................
+00000d60: 7a1d 466f 616d 5472 616e 7366 6f72 6d65  z.FoamTransforme
+00000d70: 722e 6469 6d65 6e73 696f 6e5f 7365 7463  r.dimension_setc
+00000d80: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000d90: 0300 0000 4300 0000 731c 0000 0074 007c  ....C...s....t.|
+00000da0: 0183 0164 016b 0372 0874 0182 0174 027c  ...d.k.r.t...t.|
+00000db0: 0164 0219 0083 0153 00a9 034e 7208 0000  .d.....S...Nr...
+00000dc0: 0072 0100 0000 2903 da03 6c65 6eda 0c52  .r....)...len..R
+00000dd0: 756e 7469 6d65 4572 726f 7272 2100 0000  untimeErrorr!...
+00000de0: 724d 0000 0072 2400 0000 7224 0000 0072  rM...r$...r$...r
+00000df0: 2500 0000 da09 6469 7265 6374 6976 656c  %.....directivel
+00000e00: 0000 0073 0600 0000 0c01 0401 0c01 7a19  ...s..........z.
+00000e10: 466f 616d 5472 616e 7366 6f72 6d65 722e  FoamTransformer.
+00000e20: 6469 7265 6374 6976 6563 0200 0000 0000  directivec......
+00000e30: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+00000e40: 0000 7255 0000 0029 034e 6301 0000 0000  ..rU...).Nc.....
+00000e50: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
+00000e60: 0000 0073 2c00 0000 6700 7c00 5d12 7d01  ...s,...g.|.].}.
+00000e70: 7400 7c01 7401 8302 720e 7c01 6a02 6400  t.|.t...r.|.j.d.
+00000e80: 6b02 7302 7c01 6401 7501 7202 7c01 9102  k.s.|.d.u.r.|...
+00000e90: 7102 5300 2902 724f 0000 004e 7256 0000  q.S.).rO...NrV..
+00000ea0: 0072 3b00 0000 7224 0000 0072 2400 0000  .r;...r$...r$...
+00000eb0: 7225 0000 0072 3d00 0000 7300 0000 7314  r%...r=...s...s.
+00000ec0: 0000 0006 0002 0208 0102 fd08 0302 fd06  ................
+00000ed0: 0402 fc02 0106 ff7a 2846 6f61 6d54 7261  .......z(FoamTra
+00000ee0: 6e73 666f 726d 6572 2e6c 6973 742e 3c6c  nsformer.list.<l
+00000ef0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00000f00: 3e29 0172 1000 0000 725a 0000 0072 2400  >).r....rZ...r$.
+00000f10: 0000 7224 0000 0072 2500 0000 da04 6c69  ..r$...r%.....li
+00000f20: 7374 7100 0000 725c 0000 007a 1446 6f61  stq...r\...z.Foa
+00000f30: 6d54 7261 6e73 666f 726d 6572 2e6c 6973  mTransformer.lis
+00000f40: 7463 0200 0000 0000 0000 0000 0000 0500  tc..............
+00000f50: 0000 0400 0000 4300 0000 7362 0000 007c  ......C...sb...|
+00000f60: 0164 0119 007d 027c 026a 0064 026b 0272  .d...}.|.j.d.k.r
+00000f70: 137c 026a 017d 037c 0164 0364 0085 0219  .|.j.}.|.d.d....
+00000f80: 007d 016e 0264 007d 037c 0144 005d 0f7d  .}.n.d.}.|.D.].}
+00000f90: 0474 027c 046a 0174 0383 0272 267c 046a  .t.|.j.t...r&|.j
+00000fa0: 01a0 047c 046a 00a1 0101 0071 1774 057c  ...|.j.....q.t.|
+00000fb0: 0364 0464 0584 007c 0144 0083 0183 0253  .d.d...|.D.....S
+00000fc0: 0029 064e 7201 0000 005a 0846 6f61 6d46  .).Nr....Z.FoamF
+00000fd0: 696c 6572 0800 0000 6301 0000 0000 0000  iler....c.......
+00000fe0: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
+00000ff0: 00f3 1600 0000 6900 7c00 5d07 7d01 7c01  ......i.|.].}.|.
+00001000: 6a00 7c01 6a01 9302 7102 5300 7224 0000  j.|.j...q.S.r$..
+00001010: 00a9 0272 1a00 0000 7214 0000 00a9 0272  ...r....r......r
+00001020: 2900 0000 da04 6e6f 6465 7224 0000 0072  ).....noder$...r
+00001030: 2400 0000 7225 0000 00da 0a3c 6469 6374  $...r%.....<dict
+00001040: 636f 6d70 3e87 0000 00f3 0200 0000 1600  comp>...........
+00001050: 7a28 466f 616d 5472 616e 7366 6f72 6d65  z(FoamTransforme
+00001060: 722e 6669 6c65 2e3c 6c6f 6361 6c73 3e2e  r.file.<locals>.
+00001070: 3c64 6963 7463 6f6d 703e 2906 721a 0000  <dictcomp>).r...
+00001080: 0072 1400 0000 7257 0000 0072 1000 0000  .r....rW...r....
+00001090: da08 6164 645f 6e61 6d65 720f 0000 0029  ..add_namer....)
+000010a0: 0572 4600 0000 724e 0000 005a 1066 6972  .rF...rN...Z.fir
+000010b0: 7374 5f61 7373 6967 6e6d 656e 74da 0969  st_assignment..i
+000010c0: 6e66 6f5f 6469 6374 7265 0000 0072 2400  nfo_dictre...r$.
+000010d0: 0000 7224 0000 0072 2500 0000 da04 6669  ..r$...r%.....fi
+000010e0: 6c65 7b00 0000 7314 0000 0008 010a 0106  le{...s.........
+000010f0: 010e 0104 0208 020c 010e 0102 8014 027a  ...............z
+00001100: 1446 6f61 6d54 7261 6e73 666f 726d 6572  .FoamTransformer
+00001110: 2e66 696c 6563 0200 0000 0000 0000 0000  .filec..........
+00001120: 0000 0800 0000 0800 0000 4300 0000 7312  ..........C...s.
+00001130: 0100 0064 0164 0284 007c 0144 0083 017d  ...d.d...|.D...}
+00001140: 0164 007d 0264 007d 037c 01a0 0064 03a1  .d.}.d.}.|...d..
+00001150: 017d 0474 017c 0183 0164 046b 0272 1b7c  .}.t.|...d.k.r.|
+00001160: 0164 0319 007d 056e 697a 0c64 0564 0284  .d...}.niz.d.d..
+00001170: 007c 0144 0083 01a0 0264 06a1 017d 0657  .|.D.....d...}.W
+00001180: 006e 0b04 0074 0379 3201 0001 0001 0064  .n...t.y2......d
+00001190: 007d 0259 006e 0677 007c 01a0 007c 06a1  .}.Y.n.w.|...|..
+000011a0: 017d 0264 007d 0374 0464 0764 0284 007c  .}.d.}.t.d.d...|
+000011b0: 0144 0083 0183 0172 4964 08a0 057c 01a1  .D.....rId...|..
+000011c0: 017d 076e 247c 01a0 0064 09a1 017d 0774  .}.n$|...d...}.t
+000011d0: 0464 0a64 0b84 007c 0144 0083 0183 0173  .d.d...|.D.....s
+000011e0: 5e64 0c64 0284 007c 0144 0083 017d 017c  ^d.d...|.D...}.|
+000011f0: 0172 6564 08a0 057c 01a1 017d 0374 067c  .red...|...}.t.|
+00001200: 0774 0783 0272 6d7c 037c 075f 087c 0364  .t...rm|.|._.|.d
+00001210: 0075 0072 757c 0264 0075 0073 7a74 067c  .u.ru|.d.u.szt.|
+00001220: 0774 0783 0272 7d7c 077d 056e 0774 097c  .t...r}|.}.n.t.|
+00001230: 077c 037c 0264 0d8d 037d 0574 0a7c 047c  .|.|.d...}.t.|.|
+00001240: 0583 0253 0029 0e4e 6301 0000 0000 0000  ...S.).Nc.......
+00001250: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
+00001260: 0072 3a00 0000 7227 0000 0072 2400 0000  .r:...r'...r$...
+00001270: 7264 0000 0072 2400 0000 7224 0000 0072  rd...r$...r$...r
+00001280: 2500 0000 723d 0000 008a 0000 0072 3e00  %...r=.......r>.
+00001290: 0000 7a32 466f 616d 5472 616e 7366 6f72  ..z2FoamTransfor
+000012a0: 6d65 722e 7661 725f 6173 7369 676e 6d65  mer.var_assignme
+000012b0: 6e74 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  nt.<locals>.<lis
+000012c0: 7463 6f6d 703e 7201 0000 0072 0800 0000  tcomp>r....r....
+000012d0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000012e0: 0005 0000 0053 0000 00f3 1600 0000 6700  .....S........g.
+000012f0: 7c00 5d07 7d01 7400 7c01 7401 8302 9102  |.].}.t.|.t.....
+00001300: 7102 5300 7224 0000 0029 0272 5700 0000  q.S.r$...).rW...
+00001310: 720d 0000 00a9 0272 2900 0000 da04 656c  r......r).....el
+00001320: 656d 7224 0000 0072 2400 0000 7225 0000  emr$...r$...r%..
+00001330: 0072 3d00 0000 9200 0000 7306 0000 0006  .r=.......s.....
+00001340: 000a 0106 ff54 6301 0000 0000 0000 0000  .....Tc.........
+00001350: 0000 0002 0000 0005 0000 0053 0000 0072  ...........S...r
+00001360: 6b00 0000 7224 0000 00a9 0272 5700 0000  k...r$.....rW...
+00001370: 7221 0000 0072 6c00 0000 7224 0000 0072  r!...rl...r$...r
+00001380: 2400 0000 7225 0000 0072 3d00 0000 9b00  $...r%...r=.....
+00001390: 0000 7267 0000 00da 0120 e9ff ffff ff63  ..rg..... .....c
+000013a0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000013b0: 0400 0000 7300 0000 731a 0000 0081 007c  ....s...s......|
+000013c0: 005d 087d 0174 007c 0174 0183 0256 0001  .].}.t.|.t...V..
+000013d0: 0071 0264 0053 0072 2700 0000 726e 0000  .q.d.S.r'...rn..
+000013e0: 0072 6400 0000 7224 0000 0072 2400 0000  .rd...r$...r$...
+000013f0: 7225 0000 0072 2b00 0000 9f00 0000 7304  r%...r+.......s.
+00001400: 0000 0002 8018 007a 3146 6f61 6d54 7261  .......z1FoamTra
+00001410: 6e73 666f 726d 6572 2e76 6172 5f61 7373  nsformer.var_ass
+00001420: 6967 6e6d 656e 742e 3c6c 6f63 616c 733e  ignment.<locals>
+00001430: 2e3c 6765 6e65 7870 723e 6301 0000 0000  .<genexpr>c.....
+00001440: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
+00001450: 0000 0073 1400 0000 6700 7c00 5d06 7d01  ...s....g.|.].}.
+00001460: 7400 7c01 8301 9102 7102 5300 7224 0000  t.|.....q.S.r$..
+00001470: 0029 0172 2100 0000 7264 0000 0072 2400  .).r!...rd...r$.
+00001480: 0000 7224 0000 0072 2500 0000 723d 0000  ..r$...r%...r=..
+00001490: 00a0 0000 0073 0200 0000 1400 2902 721a  .....s......).r.
+000014a0: 0000 00da 0964 696d 656e 7369 6f6e 290b  .....dimension).
+000014b0: da03 706f 7072 5e00 0000 da05 696e 6465  ..popr^.....inde
+000014c0: 7872 4100 0000 da03 616c 6c72 2c00 0000  xrA.....allr,...
+000014d0: 7257 0000 0072 1000 0000 da05 5f6e 616d  rW...r......_nam
+000014e0: 6572 1200 0000 7213 0000 0029 0872 4600  er....r....).rF.
+000014f0: 0000 724e 0000 0072 5b00 0000 5a0d 6e61  ..rN...r[...Z.na
+00001500: 6d65 5f69 6e5f 7661 6c75 6572 1a00 0000  me_in_valuer....
+00001510: 7214 0000 005a 0f69 6e64 6578 5f64 696d  r....Z.index_dim
+00001520: 656e 7369 6f6e da0a 6c61 7374 5f76 616c  ension..last_val
+00001530: 7565 7224 0000 0072 2400 0000 7225 0000  uer$...r$...r%..
+00001540: 00da 0e76 6172 5f61 7373 6967 6e6d 656e  ...var_assignmen
+00001550: 7489 0000 0073 4400 0000 0e01 0401 0401  t....sD.........
+00001560: 0a01 0c01 0a01 0202 0601 0201 04ff 0602  ................
+00001570: 06fe 0c03 0801 02ff 0a03 0402 1201 0c01  ................
+00001580: 0a02 1201 0e01 0401 0a01 0a01 0601 1202  ................
+00001590: 0401 04ff 0603 0202 0601 06ff 0a03 7a1e  ..............z.
+000015a0: 466f 616d 5472 616e 7366 6f72 6d65 722e  FoamTransformer.
+000015b0: 7661 725f 6173 7369 676e 6d65 6e74 6302  var_assignmentc.
+000015c0: 0000 0000 0000 0000 0000 0008 0000 0007  ................
+000015d0: 0000 0043 0000 0073 1601 0000 7400 7c01  ...C...s....t.|.
+000015e0: 8301 7d01 6400 7d02 7401 7c01 8301 6401  ..}.d.}.t.|...d.
+000015f0: 6b02 721a 7c01 a002 6402 a101 7d03 7403  k.r.|...d...}.t.
+00001600: 7c03 7404 6900 7c03 6403 8d02 8302 5300  |.t.i.|.d.....S.
+00001610: 6700 7d04 7c01 4400 5d13 7d05 7405 7c05  g.}.|.D.].}.t.|.
+00001620: 7406 8302 7231 7c05 a007 6404 a101 7231  t...r1|...d...r1
+00001630: 7c01 a002 6401 a101 7d02 0100 6e01 711e  |...d...}...n.q.
+00001640: 7405 7c01 6402 1900 7408 8302 7246 6405  t.|.d...t...rFd.
+00001650: 6406 a009 7c01 a002 6402 a101 a101 1700  d...|...d.......
+00001660: 6407 1700 7d03 6e05 7c01 a002 6402 a101  d...}.n.|...d...
+00001670: 7d03 7c04 7256 7c03 6406 6406 a009 7c04  }.|.rV|.d.d...|.
+00001680: a101 1700 3700 7d03 6408 6409 8400 7c01  ....7.}.d.d...|.
+00001690: 4400 8301 7d06 7c06 4400 5d0f 7d05 7405  D...}.|.D.].}.t.
+000016a0: 7c05 6a0a 740b 8302 726e 7c05 6a0a a00c  |.j.t...rn|.j...
+000016b0: 7c05 6a0d a101 0100 715f 7c02 6400 7501  |.j.....q_|.d.u.
+000016c0: 727a 7c02 640a 6b02 727a 740e 7d07 6e02  rz|.d.k.rzt.}.n.
+000016d0: 7404 7d07 7403 7c03 7c07 640b 640c 8400  t.}.t.|.|.d.d...
+000016e0: 7c06 4400 8301 7c03 7c02 640d 8d03 8302  |.D...|.|.d.....
+000016f0: 5300 290e 4e72 0800 0000 7201 0000 0029  S.).Nr....r....)
+00001700: 02da 0464 6174 6172 1a00 0000 fa01 23fa  ...datar......#.
+00001710: 0128 726f 0000 00fa 0129 6301 0000 0000  .(ro.....)c.....
+00001720: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
+00001730: 0000 0073 2400 0000 6700 7c00 5d0e 7d01  ...s$...g.|.].}.
+00001740: 7400 7c01 6400 8302 7202 7400 7c01 6401  t.|.d...r.t.|.d.
+00001750: 8302 7202 7c01 9102 7102 5300 7263 0000  ..r.|...q.S.rc..
+00001760: 0029 01da 0768 6173 6174 7472 7264 0000  .)...hasattrrd..
+00001770: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
+00001780: 723d 0000 00c5 0000 0072 5900 0000 7a33  r=.......rY...z3
+00001790: 466f 616d 5472 616e 7366 6f72 6d65 722e  FoamTransformer.
+000017a0: 6469 6374 5f61 7373 6967 6e6d 656e 742e  dict_assignment.
+000017b0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+000017c0: 6d70 3e7a 0b23 636f 6465 5374 7265 616d  mp>z.#codeStream
+000017d0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000017e0: 0004 0000 0053 0000 0072 6200 0000 7224  .....S...rb...r$
+000017f0: 0000 0072 6300 0000 7264 0000 0072 2400  ...rc...rd...r$.
+00001800: 0000 7224 0000 0072 2500 0000 7266 0000  ..r$...r%...rf..
+00001810: 00d7 0000 0072 6700 0000 7a33 466f 616d  .....rg...z3Foam
+00001820: 5472 616e 7366 6f72 6d65 722e 6469 6374  Transformer.dict
+00001830: 5f61 7373 6967 6e6d 656e 742e 3c6c 6f63  _assignment.<loc
+00001840: 616c 733e 2e3c 6469 6374 636f 6d70 3e29  als>.<dictcomp>)
+00001850: 0372 7800 0000 721a 0000 0072 6000 0000  .rx...r....r`...
+00001860: 290f 7240 0000 0072 5e00 0000 7272 0000  ).r@...r^...rr..
+00001870: 0072 0900 0000 720c 0000 0072 5700 0000  .r....r....rW...
+00001880: 7221 0000 00da 0a73 7461 7274 7377 6974  r!.....startswit
+00001890: 6872 6100 0000 722c 0000 0072 1400 0000  hra...r,...r....
+000018a0: 7210 0000 0072 6800 0000 721a 0000 0072  r....rh...r....r
+000018b0: 0b00 0000 2908 7246 0000 0072 4e00 0000  ....).rF...rN...
+000018c0: 7260 0000 0072 1a00 0000 5a09 6e6f 6465  r`...r....Z.node
+000018d0: 735f 7374 7272 6500 0000 5a0c 6e6f 6465  s_strre...Z.node
+000018e0: 735f 6173 7369 676e da03 636c 7372 2400  s_assign..clsr$.
+000018f0: 0000 7224 0000 0072 2500 0000 da0f 6469  ..r$...r%.....di
+00001900: 6374 5f61 7373 6967 6e6d 656e 74b0 0000  ct_assignment...
+00001910: 0073 4400 0000 0801 0401 0c02 0a01 1201  .sD.............
+00001920: 0402 0801 1401 0a02 0401 0280 0e01 1a01  ................
+00001930: 0a02 0401 1201 0602 0202 06fe 0806 0c01  ................
+00001940: 0e01 0280 1002 0601 0402 0202 0201 0201  ................
+00001950: 0c01 0201 0201 04fd 04fe 7a1f 466f 616d  ..........z.Foam
+00001960: 5472 616e 7366 6f72 6d65 722e 6469 6374  Transformer.dict
+00001970: 5f61 7373 6967 6e6d 656e 7463 0200 0000  _assignmentc....
+00001980: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00001990: 4300 0000 732e 0000 0074 007c 0183 017d  C...s....t.|...}
+000019a0: 0174 017c 0183 0164 016b 0372 0e74 027c  .t.|...d.k.r.t.|
+000019b0: 0183 0182 0164 007d 0274 037c 027c 0164  .....d.}.t.|.|.d
+000019c0: 0219 0083 0253 0072 5d00 0000 2904 7240  .....S.r]...).r@
+000019d0: 0000 0072 5e00 0000 da13 4e6f 7449 6d70  ...r^.....NotImp
+000019e0: 6c65 6d65 6e74 6564 4572 726f 7272 0900  lementedErrorr..
+000019f0: 0000 a903 7246 0000 0072 4e00 0000 721a  ....rF...rN...r.
+00001a00: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
+00001a10: 0000 da0d 6973 6f6c 6174 6564 5f6c 6973  ....isolated_lis
+00001a20: 74dd 0000 0073 0a00 0000 0801 0c01 0801  t....s..........
+00001a30: 0401 0e01 7a1d 466f 616d 5472 616e 7366  ....z.FoamTransf
+00001a40: 6f72 6d65 722e 6973 6f6c 6174 6564 5f6c  ormer.isolated_l
+00001a50: 6973 7463 0200 0000 0000 0000 0000 0000  istc............
+00001a60: 0800 0000 0600 0000 4300 0000 73ac 0000  ........C...s...
+00001a70: 0074 007c 0183 017d 0164 007d 0274 017c  .t.|...}.d.}.t.|
+00001a80: 0183 0144 005d 185c 027d 037d 0474 027c  ...D.].\.}.}.t.|
+00001a90: 0474 0383 0272 227c 046a 0464 016b 0272  .t...r"|.j.d.k.r
+00001aa0: 2274 057c 0483 0164 0264 0385 0219 007d  "t.|...d.d.....}
+00001ab0: 0201 006e 0171 0a7c 0264 0075 0172 2c7c  ...n.q.|.d.u.r,|
+00001ac0: 01a0 067c 03a1 0101 0064 007d 0574 077c  ...|.....d.}.t.|
+00001ad0: 0183 0164 046b 0472 4074 027c 0164 0319  ...d.k.r@t.|.d..
+00001ae0: 0074 0883 0272 407c 01a0 0664 03a1 017d  .t...r@|...d...}
+00001af0: 057c 01a0 0664 05a1 017d 0664 007d 077c  .|...d...}.d.}.|
+00001b00: 0172 4e64 06a0 097c 01a1 017d 0774 0a7c  .rNd...|...}.t.|
+00001b10: 067c 077c 027c 0564 078d 0453 0029 084e  .|.|.|.d...S.).N
+00001b20: 5a09 4c49 5354 5f54 5950 45e9 0500 0000  Z.LIST_TYPE.....
+00001b30: 7270 0000 0072 0800 0000 7201 0000 0072  rp...r....r....r
+00001b40: 6f00 0000 2904 721a 0000 0072 1b00 0000  o...).r....r....
+00001b50: 721c 0000 0072 1d00 0000 290b 7240 0000  r....r....).r@..
+00001b60: 00da 0965 6e75 6d65 7261 7465 7257 0000  ...enumeraterW..
+00001b70: 0072 0500 0000 7258 0000 0072 2100 0000  .r....rX...r!...
+00001b80: 7272 0000 0072 5e00 0000 7223 0000 0072  rr...r^...r#...r
+00001b90: 2c00 0000 7219 0000 0029 0872 4600 0000  ,...r....).rF...
+00001ba0: 724e 0000 0072 1c00 0000 da05 696e 6f64  rN...r......inod
+00001bb0: 6572 6500 0000 721d 0000 0072 1a00 0000  ere...r....r....
+00001bc0: 721b 0000 0072 2400 0000 7224 0000 0072  r....r$...r$...r
+00001bd0: 2500 0000 da09 6c69 7374 5f69 6e66 6fe4  %.....list_info.
+00001be0: 0000 0073 2200 0000 0801 0402 1001 1401  ...s"...........
+00001bf0: 1001 0401 0280 0801 0a01 0402 1a01 0a01  ................
+00001c00: 0a02 0402 0401 0a01 1002 7a19 466f 616d  ..........z.Foam
+00001c10: 5472 616e 7366 6f72 6d65 722e 6c69 7374  Transformer.list
+00001c20: 5f69 6e66 6f63 0200 0000 0000 0000 0000  _infoc..........
+00001c30: 0000 0600 0000 0400 0000 4300 0000 73aa  ..........C...s.
+00001c40: 0000 0074 007c 0183 017d 017c 015c 027d  ...t.|...}.|.\.}
+00001c50: 027d 0374 017c 0274 0283 0273 0f4a 0082  .}.t.|.t...s.J..
+00001c60: 017c 026a 037d 047c 047d 057c 026a 0464  .|.j.}.|.}.|.j.d
+00001c70: 0075 0172 207c 0564 017c 026a 0417 0037  .u.r |.d.|.j...7
+00001c80: 007d 057c 026a 0564 0075 0172 2e7c 0564  .}.|.j.d.u.r.|.d
+00001c90: 027c 026a 059b 0064 039d 0337 007d 057c  .|.j...d...7.}.|
+00001ca0: 026a 0664 0075 0172 3b7c 0564 047c 026a  .j.d.u.r;|.d.|.j
+00001cb0: 069b 009d 0237 007d 0574 017c 0474 0783  .....7.}.t.|.t..
+00001cc0: 0272 4474 087c 0483 017d 0474 017c 0574  .rDt.|...}.t.|.t
+00001cd0: 0783 0272 4d74 087c 0583 017d 057c 057c  ...rMt.|...}.|.|
+00001ce0: 035f 0974 0a7c 047c 0383 0253 0029 054e  ._.t.|.|...S.).N
+00001cf0: 726f 0000 007a 060a 4c69 7374 3cda 013e  ro...z..List<..>
+00001d00: 7226 0000 0029 0b72 4000 0000 7257 0000  r&...).r@...rW..
+00001d10: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00001d20: 721c 0000 0072 1d00 0000 7223 0000 0072  r....r....r#...r
+00001d30: 2100 0000 7275 0000 0072 0900 0000 2906  !...ru...r....).
+00001d40: 7246 0000 0072 4e00 0000 7286 0000 00da  rF...rN...r.....
+00001d50: 0874 6865 5f6c 6973 7472 1a00 0000 5a0d  .the_listr....Z.
+00001d60: 6e61 6d65 5f69 6e74 6572 6e61 6c72 2400  name_internalr$.
+00001d70: 0000 7224 0000 0072 2500 0000 da0f 6c69  ..r$...r%.....li
+00001d80: 7374 5f61 7373 6967 6e6d 656e 74fb 0000  st_assignment...
+00001d90: 0073 2200 0000 0801 0802 0e01 0602 0401  .s".............
+00001da0: 0a02 0e01 0a02 1201 0a02 1001 0a02 0801  ................
+00001db0: 0a01 0801 0602 0a01 7a1f 466f 616d 5472  ........z.FoamTr
+00001dc0: 616e 7366 6f72 6d65 722e 6c69 7374 5f61  ansformer.list_a
+00001dd0: 7373 6967 6e6d 656e 7463 0200 0000 0000  ssignmentc......
+00001de0: 0000 0000 0000 0300 0000 0700 0000 4300  ..............C.
+00001df0: 0000 7370 0000 0064 0164 0284 007c 0144  ..sp...d.d...|.D
+00001e00: 0083 017d 017c 01a0 0064 03a1 017d 0274  ...}.|...d...}.t
+00001e10: 017c 0183 0164 046b 0272 2174 027c 0274  .|...d.k.r!t.|.t
+00001e20: 037c 0164 0519 007c 0164 0319 007c 0164  .|.d...|.d...|.d
+00001e30: 0619 0083 0383 0253 0074 017c 0183 0164  .......S.t.|...d
+00001e40: 076b 0272 3474 027c 0274 037c 0164 0519  .k.r4t.|.t.|.d..
+00001e50: 007c 0164 0619 0064 088d 0283 0253 0074  .|.d...d.....S.t
+00001e60: 047c 0183 0182 0129 094e 6301 0000 0000  .|.....).Nc.....
+00001e70: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
+00001e80: 0000 0072 3a00 0000 7227 0000 0072 2400  ...r:...r'...r$.
+00001e90: 0000 7264 0000 0072 2400 0000 7224 0000  ..rd...r$...r$..
+00001ea0: 0072 2500 0000 723d 0000 0016 0100 0072  .r%...r=.......r
+00001eb0: 3e00 0000 7a38 466f 616d 5472 616e 7366  >...z8FoamTransf
+00001ec0: 6f72 6d65 722e 6469 6d65 6e73 696f 6e5f  ormer.dimension_
+00001ed0: 6173 7369 676e 6d65 6e74 2e3c 6c6f 6361  assignment.<loca
+00001ee0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7201  ls>.<listcomp>r.
+00001ef0: 0000 00e9 0300 0000 7270 0000 00e9 feff  ........rp......
+00001f00: ffff e902 0000 0029 0172 7100 0000 2905  .......).rq...).
+00001f10: 7272 0000 0072 5e00 0000 7209 0000 0072  rr...r^...r....r
+00001f20: 1200 0000 725f 0000 0072 8100 0000 7224  ....r_...r....r$
+00001f30: 0000 0072 2400 0000 7225 0000 00da 1464  ...r$...r%.....d
+00001f40: 696d 656e 7369 6f6e 5f61 7373 6967 6e6d  imension_assignm
+00001f50: 656e 7415 0100 0073 0e00 0000 0e01 0a01  ent....s........
+00001f60: 0c02 1e01 0c01 1a01 0802 7a24 466f 616d  ..........z$Foam
+00001f70: 5472 616e 7366 6f72 6d65 722e 6469 6d65  Transformer.dime
+00001f80: 6e73 696f 6e5f 6173 7369 676e 6d65 6e74  nsion_assignment
+00001f90: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00001fa0: 0003 0000 0043 0000 0073 3600 0000 6401  .....C...s6...d.
+00001fb0: 6402 8400 7c01 4400 8301 7d01 7400 7c01  d...|.D...}.t.|.
+00001fc0: 8301 6403 6b03 7211 7401 7c01 8301 8201  ..d.k.r.t.|.....
+00001fd0: 7c01 a002 6404 a101 7d02 7403 7c02 6405  |...d...}.t.|.d.
+00001fe0: 8302 5300 2906 4e63 0100 0000 0000 0000  ..S.).Nc........
+00001ff0: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
+00002000: 723a 0000 0072 2700 0000 7224 0000 0072  r:...r'...r$...r
+00002010: 6400 0000 7224 0000 0072 2400 0000 7225  d...r$...r$...r%
+00002020: 0000 0072 3d00 0000 2101 0000 723e 0000  ...r=...!...r>..
+00002030: 007a 3446 6f61 6d54 7261 6e73 666f 726d  .z4FoamTransform
+00002040: 6572 2e6d 6163 726f 5f61 7373 6967 6e6d  er.macro_assignm
+00002050: 656e 742e 3c6c 6f63 616c 733e 2e3c 6c69  ent.<locals>.<li
+00002060: 7374 636f 6d70 3e72 0800 0000 7201 0000  stcomp>r....r...
+00002070: 00da 0029 0472 5e00 0000 7280 0000 0072  ...).r^...r....r
+00002080: 7200 0000 7209 0000 0072 8100 0000 7224  r...r....r....r$
+00002090: 0000 0072 2400 0000 7225 0000 00da 106d  ...r$...r%.....m
+000020a0: 6163 726f 5f61 7373 6967 6e6d 656e 7420  acro_assignment 
+000020b0: 0100 0073 0a00 0000 0e01 0c01 0801 0a01  ...s............
+000020c0: 0a01 7a20 466f 616d 5472 616e 7366 6f72  ..z FoamTransfor
+000020d0: 6d65 722e 6d61 6372 6f5f 6173 7369 676e  mer.macro_assign
+000020e0: 6d65 6e74 6302 0000 0000 0000 0000 0000  mentc...........
+000020f0: 0003 0000 0003 0000 0043 0000 0073 4e00  .........C...sN.
+00002100: 0000 6401 6402 8400 7c01 4400 8301 7d01  ..d.d...|.D...}.
+00002110: 7400 7c01 8301 6403 6b03 7211 7401 7c01  t.|...d.k.r.t.|.
+00002120: 8301 8201 7c01 6404 1900 7d02 7402 7c02  ....|.d...}.t.|.
+00002130: 6405 8302 721e 7c02 a003 a100 7d02 7c01  d...r.|.....}.|.
+00002140: 6406 1900 9b00 6407 7c02 9b00 9d03 5300  d.....d.|.....S.
+00002150: 2908 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
+00002160: 0200 0000 0400 0000 5300 0000 723a 0000  ........S...r:..
+00002170: 0072 2700 0000 7224 0000 0072 6400 0000  .r'...r$...rd...
+00002180: 7224 0000 0072 2400 0000 7225 0000 0072  r$...r$...r%...r
+00002190: 3d00 0000 2801 0000 723e 0000 007a 3046  =...(...r>...z0F
+000021a0: 6f61 6d54 7261 6e73 666f 726d 6572 2e65  oamTransformer.e
+000021b0: 7175 616c 5f61 7373 6967 6e2e 3c6c 6f63  qual_assign.<loc
+000021c0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
+000021d0: 8c00 0000 7208 0000 0072 3800 0000 7201  ....r....r8...r.
+000021e0: 0000 00da 013d 2904 725e 0000 0072 5f00  .....=).r^...r_.
+000021f0: 0000 727c 0000 0072 3800 0000 2903 7246  ..r|...r8...).rF
+00002200: 0000 0072 4e00 0000 7214 0000 0072 2400  ...rN...r....r$.
+00002210: 0000 7224 0000 0072 2500 0000 da0c 6571  ..r$...r%.....eq
+00002220: 7561 6c5f 6173 7369 676e 2701 0000 730e  ual_assign'...s.
+00002230: 0000 000e 010c 0108 0108 010a 0108 0112  ................
+00002240: 017a 1c46 6f61 6d54 7261 6e73 666f 726d  .z.FoamTransform
+00002250: 6572 2e65 7175 616c 5f61 7373 6967 6e63  er.equal_assignc
+00002260: 0200 0000 0000 0000 0000 0000 0700 0000  ................
+00002270: 0500 0000 4300 0000 736e 0000 0064 0164  ....C...sn...d.d
+00002280: 0284 007c 0144 0083 017d 0174 007c 0183  ...|.D...}.t.|..
+00002290: 0164 036b 0272 127c 015c 027d 027d 036e  .d.k.r.|.\.}.}.n
+000022a0: 177c 01a0 0164 04a1 017d 027c 01a0 0164  .|...d...}.|...d
+000022b0: 04a1 017d 0464 05a0 027c 01a1 017d 057c  ...}.d...|...}.|
+000022c0: 0464 067c 059b 0064 079d 0317 007d 037c  .d.|...d.....}.|
+000022d0: 0264 0817 007c 0317 007d 0674 037c 0674  .d...|...}.t.|.t
+000022e0: 047c 027c 0383 0283 0253 0029 094e 6301  .|.|.....S.).Nc.
+000022f0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00002300: 0000 0053 0000 0072 3a00 0000 7227 0000  ...S...r:...r'..
+00002310: 0072 2400 0000 7264 0000 0072 2400 0000  .r$...rd...r$...
+00002320: 7224 0000 0072 2500 0000 723d 0000 0031  r$...r%...r=...1
+00002330: 0100 0072 3e00 0000 7a38 466f 616d 5472  ...r>...z8FoamTr
+00002340: 616e 7366 6f72 6d65 722e 6469 7265 6374  ansformer.direct
+00002350: 6976 655f 6173 7369 676e 6d65 6e74 2e3c  ive_assignment.<
+00002360: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00002370: 703e 728c 0000 0072 0100 0000 7a02 2c20  p>r....r....z., 
+00002380: 727a 0000 0072 7b00 0000 726f 0000 0029  rz...r{...ro...)
+00002390: 0572 5e00 0000 7272 0000 0072 2c00 0000  .r^...rr...r,...
+000023a0: 7209 0000 0072 0e00 0000 2907 7246 0000  r....r....).rF..
+000023b0: 0072 4e00 0000 7260 0000 00da 0763 6f6e  .rN...r`.....con
+000023c0: 7465 6e74 da0d 6675 6e63 7469 6f6e 5f6e  tent..function_n
+000023d0: 616d 65da 0961 7267 756d 656e 7473 da03  ame..arguments..
+000023e0: 6b65 7972 2400 0000 7224 0000 0072 2500  keyr$...r$...r%.
+000023f0: 0000 da14 6469 7265 6374 6976 655f 6173  ....directive_as
+00002400: 7369 676e 6d65 6e74 3001 0000 7312 0000  signment0...s...
+00002410: 000e 010c 010a 010a 020a 010a 0110 010c  ................
+00002420: 0110 017a 2446 6f61 6d54 7261 6e73 666f  ...z$FoamTransfo
+00002430: 726d 6572 2e64 6972 6563 7469 7665 5f61  rmer.directive_a
+00002440: 7373 6967 6e6d 656e 7463 0200 0000 0000  ssignmentc......
+00002450: 0000 0000 0000 0500 0000 0700 0000 4300  ..............C.
+00002460: 0000 73ac 0000 0074 007c 0183 017d 0164  ..s....t.|...}.d
+00002470: 007d 0274 017c 0183 0164 016b 0272 117c  .}.t.|...d.k.r.|
+00002480: 015c 027d 037d 046e 1974 017c 0183 0164  .\.}.}.n.t.|...d
+00002490: 026b 0272 267c 015c 037d 037d 027d 047c  .k.r&|.\.}.}.}.|
+000024a0: 02a0 0264 03a1 0173 2574 037c 0183 0182  ...d...s%t.|....
+000024b0: 016e 0474 037c 0183 0182 0174 047c 0483  .n.t.|.....t.|..
+000024c0: 017d 047c 04a0 0264 04a1 0172 447c 04a0  .}.|...d...rD|..
+000024d0: 0564 0564 06a1 0264 0719 007d 047c 04a0  .d.d...d...}.|..
+000024e0: 0664 0564 06a1 0264 0819 007d 046e 087c  .d.d...d...}.n.|
+000024f0: 0464 0164 0985 0219 00a0 07a1 007d 0474  .d.d.........}.t
+00002500: 087c 0374 097c 037c 047c 0264 0a8d 0383  .|.t.|.|.|.d....
+00002510: 0253 0029 0b4e 728c 0000 0072 8a00 0000  .S.).Nr....r....
+00002520: 7279 0000 007a 0323 7b0a 7226 0000 0072  ry...z.#{.r&...r
+00002530: 0800 0000 7270 0000 0072 0100 0000 e9fd  ....rp...r......
+00002540: ffff ff29 0172 6000 0000 290a 7240 0000  ...).r`...).r@..
+00002550: 0072 5e00 0000 727d 0000 0072 8000 0000  .r^...r}...r....
+00002560: 7221 0000 0072 2d00 0000 da06 7273 706c  r!...r-.....rspl
+00002570: 6974 da05 7374 7269 7072 0900 0000 720a  it..stripr....r.
+00002580: 0000 0029 0572 4600 0000 724e 0000 0072  ...).rF...rN...r
+00002590: 6000 0000 721a 0000 00da 0463 6f64 6572  `...r......coder
+000025a0: 2400 0000 7224 0000 0072 2500 0000 da0f  $...r$...r%.....
+000025b0: 636f 6465 5f61 7373 6967 6e6d 656e 743c  code_assignment<
+000025c0: 0100 0073 2000 0000 0801 0401 0c01 0a01  ...s ...........
+000025d0: 0c01 0a01 0a01 0801 02ff 0803 0801 0a01  ................
+000025e0: 1001 1201 1002 1401 7a1f 466f 616d 5472  ........z.FoamTr
+000025f0: 616e 7366 6f72 6d65 722e 636f 6465 5f61  ansformer.code_a
+00002600: 7373 6967 6e6d 656e 7463 0200 0000 0000  ssignmentc......
+00002610: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+00002620: 0000 731a 0000 0074 007c 0183 017d 0174  ..s....t.|...}.t
+00002630: 017c 0164 0119 006a 0264 0217 0083 0153  .|.d...j.d.....S
+00002640: 0029 034e 7201 0000 0072 2600 0000 2903  .).Nr....r&...).
+00002650: 7240 0000 0072 1100 0000 7214 0000 0072  r@...r....r....r
+00002660: 4500 0000 7224 0000 0072 2400 0000 7225  E...r$...r$...r%
+00002670: 0000 00da 1273 7065 6369 616c 5f64 6972  .....special_dir
+00002680: 6563 7469 7665 734f 0100 0073 0400 0000  ectivesO...s....
+00002690: 0801 1201 7a22 466f 616d 5472 616e 7366  ....z"FoamTransf
+000026a0: 6f72 6d65 722e 7370 6563 6961 6c5f 6469  ormer.special_di
+000026b0: 7265 6374 6976 6573 4e29 1a72 1e00 0000  rectivesN).r....
+000026c0: 721f 0000 0072 2000 0000 7248 0000 0072  r....r ...rH...r
+000026d0: 4b00 0000 724f 0000 0072 5000 0000 7251  K...rO...rP...rQ
+000026e0: 0000 0072 5200 0000 7253 0000 0072 5400  ...rR...rS...rT.
+000026f0: 0000 725b 0000 0072 6000 0000 7261 0000  ..r[...r`...ra..
+00002700: 0072 6a00 0000 7277 0000 0072 7f00 0000  .rj...rw...r....
+00002710: 7282 0000 0072 8600 0000 7289 0000 0072  r....r....r....r
+00002720: 8d00 0000 728f 0000 0072 9100 0000 7296  ....r....r....r.
+00002730: 0000 0072 9b00 0000 729c 0000 0072 2400  ...r....r....r$.
+00002740: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
+00002750: 0072 3300 0000 4a00 0000 7330 0000 0008  .r3...J...s0....
+00002760: 0008 0108 0308 0308 0308 0308 0308 0308  ................
+00002770: 0308 0308 0908 0508 0a08 0e08 2708 2d08  ............'.-.
+00002780: 0708 1708 1a08 0b08 0708 0908 0c0c 1372  ...............r
+00002790: 3300 0000 7227 0000 0029 27da 075f 5f64  3...r'...)'..__d
+000027a0: 6f63 5f5f da0b 6461 7461 636c 6173 7365  oc__..dataclasse
+000027b0: 7372 0200 0000 da07 7061 7468 6c69 6272  sr......pathlibr
+000027c0: 0300 0000 5a04 6c61 726b 7204 0000 0072  ....Z.larkr....r
+000027d0: 0500 0000 7206 0000 005a 0f6c 6172 6b2e  ....r....Z.lark.
+000027e0: 6578 6365 7074 696f 6e73 7207 0000 00da  exceptionsr.....
+000027f0: 0361 7374 7209 0000 0072 0a00 0000 720b  .astr....r....r.
+00002800: 0000 0072 0c00 0000 720d 0000 0072 0e00  ...r....r....r..
+00002810: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
+00002820: 0072 1200 0000 7213 0000 00da 085f 5f66  .r....r......__f
+00002830: 696c 655f 5fda 0861 6273 6f6c 7574 65da  ile__..absolute.
+00002840: 0670 6172 656e 74da 0468 6572 65da 0972  .parent..here..r
+00002850: 6561 645f 7465 7874 7236 0000 005a 1067  ead_textr6...Z.g
+00002860: 7261 6d6d 6172 5f61 6476 616e 6365 6472  rammar_advancedr
+00002870: 2f00 0000 7231 0000 0072 3200 0000 7219  /...r1...r2...r.
+00002880: 0000 0072 3000 0000 7238 0000 0072 4000  ...r0...r8...r@.
+00002890: 0000 7244 0000 0072 3300 0000 7224 0000  ..rD...r3...r$..
+000028a0: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
+000028b0: da08 3c6d 6f64 756c 653e 0100 0000 7326  ..<module>....s&
+000028c0: 0000 0004 000c 020c 0114 020c 0134 020e  .............4..
+000028d0: 0e0c 020c 010e 020e 010a 0202 0310 010a  ................
+000028e0: 0708 1008 0408 0414 08                   .........
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/ast.py` & `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/ast.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+"""Abstract Syntax Trees for OpenFOAM input files"""
+
 import re
+from abc import ABC, abstractmethod
 from dataclasses import dataclass
+from numbers import Number
 from textwrap import dedent
+from typing import Optional
 
 from inflection import underscore
 
 symbols = ["kg", "m", "s", "K", "kmol", "A", "cd"]
 
 
 def str2foam_units(units):
@@ -48,27 +53,105 @@
     if result.startswith("."):
         result = result[1:]
     elif result.startswith("/"):
         result = "1" + result
     return result
 
 
+def _compute_spaces_to_align(data, max_length=20):
+    try:
+        max_length = min(
+            max_length,
+            max(
+                len(key)
+                for key, value in data.items()
+                if not isinstance(value, (Dict, List))
+            ),
+        )
+    except ValueError:
+        max_length = 0
+
+    default_space = 4
+    return max_length + default_space
+
+
 class Node:
     def __eq__(self, other):
         if type(other) is type(self):
             return self.__dict__ == other.__dict__
         return False
 
 
-class FoamInputFile(Node):
-    def __init__(self, info, children, header=None, comments=None):
+class NodeLikePyDict(ABC):
+    def init_from_py_objects(
+        self,
+        data: dict,
+        dimensions: Optional[dict] = None,
+        default_dimension=False,
+        comments: Optional[dict] = None,
+    ):
+        if dimensions is None:
+            dimensions = {}
+        if comments is None:
+            comments = {}
+        for key, value in data.items():
+            if isinstance(value, (type(None), str)):
+                self.set_child(key, value)
+            elif isinstance(value, (Number, list)):
+                if default_dimension is False:
+                    self.set_child(key, value)
+                else:
+                    dimension = dimensions.get(key, default_dimension)
+                    if isinstance(value, list):
+                        value = List(value)
+                    self.set_value(key, value, dimension)
+            elif isinstance(value, dict):
+                dimensions_dict = dimensions.get(key, None)
+                comments_dict = comments.get(key, None)
+                obj = Dict({}, name=key, comments=comments_dict)
+                obj.init_from_py_objects(
+                    value,
+                    dimensions=dimensions_dict,
+                    default_dimension=default_dimension,
+                    comments=comments_dict,
+                )
+                self._set_item(key, obj)
+            else:
+                raise NotImplementedError(type(value))
+
+    def set_child(self, key, child):
+        if isinstance(child, (type(None), str, Number)):
+            pass
+        elif isinstance(child, dict):
+            child = Dict(child, name=key)
+        elif isinstance(child, list):
+            child = List(child, name=key)
+        else:
+            raise NotImplementedError
+        self._set_item(key, child)
+
+    def set_value(self, name, value, dimension=None):
+        if isinstance(value, Number) or dimension is not None:
+            value = Value(value, name, dimension=dimension)
+        self._set_item(name, value)
+
+    @abstractmethod
+    def _set_item(self, key, value):
+        """Set an item"""
+
+
+class FoamInputFile(Node, NodeLikePyDict):
+    def __init__(self, info, children=None, header=None, comments=None):
         self.info = info
+        if children is None:
+            children = {}
         self.children = children
         self.header = header
         self.comments = comments
+        self.path = None
 
     def __repr__(self):
         tmp = ["InputFile(\n"]
         if self.info is not None:
             tmp.append(f"info={self.info},\n")
         tmp.append(f"children={self.children}\n)")
         return "".join(tmp)
@@ -78,37 +161,56 @@
         if self.info is not None:
             tmp1 = ["FoamFile\n{"]
             for key, node in self.info.items():
                 s = (12 - len(key)) * " "
                 tmp1.append(f"    {key}{s}{node};")
             tmp1.append("}")
             tmp.append("\n".join(tmp1))
+
+        num_spaces = _compute_spaces_to_align(self.children, max_length=14)
         for key, node in self.children.items():
             if hasattr(node, "dump"):
                 code_node = node.dump()
                 # special for isolated list
                 if key is None and isinstance(node, List):
                     code_node += ";"
-            elif hasattr(node, "dump_without_assignment"):
-                code_node = f"{key}  {node.dump_without_assignment()};"
             elif node is None:
                 code_node = f"{key}"
             else:
-                code_node = f"{key:14s}  {node};"
+                if hasattr(node, "dump_without_assignment"):
+                    node_dumped = node.dump_without_assignment()
+                else:
+                    node_dumped = node
+                if node_dumped == "":
+                    s = ""
+                else:
+                    s = max(2, (num_spaces - len(key))) * " "
+                code_node = f"{key}{s}{node_dumped};"
             if self.comments is not None and key in self.comments:
-                comment = "// " + self.comments[key].replace("\n", "\n// ")
-                code_node = comment + "\n" + code_node
+                comment = self.comments[key]
+                if isinstance(comment, str):
+                    comment = "// " + comment.replace("\n", "\n// ")
+                    code_node = comment + "\n" + code_node
             tmp.append(code_node)
         result = "\n\n".join(tmp)
         if self.header is not None:
             result = self.header + "\n" + result
         if result[-1] != "\n":
             result += "\n"
         return result
 
+    def overwrite(self):
+        if self.path is None:
+            raise ValueError("self.path is None")
+        with open(self.path, "w") as file:
+            file.write(self.dump())
+
+    def _set_item(self, key, value):
+        self.children[key] = value
+
 
 @dataclass
 class Assignment:
     name: str
     value: object
 
     def dump(self, indent=0):
@@ -149,22 +251,28 @@
         else:
             return f"Value({self.value})"
 
     def dump_without_assignment(self, indent=0):
         if self.dimension is not None:
             dimension_list = str2foam_units(self.dimension)
             dimension_dumped = " ".join(str(number) for number in dimension_list)
+
+        if isinstance(self.value, Node) and hasattr(self.value, "dump"):
+            value_dumped = self.value.dump()
+        else:
+            value_dumped = str(self.value)
+
         if self.dimension is not None and self.name is not None:
-            return f"{self.name} [{dimension_dumped}] {self.value}"
+            return f"{self.name} [{dimension_dumped}] {value_dumped}"
         elif self.dimension is None and self.name is not None:
-            return f"{self.name} {self.value}"
+            return f"{self.name} {value_dumped}"
         elif self.dimension is not None and self.name is None:
-            return f"[{dimension_dumped}] {self.value}"
+            return f"[{dimension_dumped}] {value_dumped}"
         else:
-            return f"{self.value}"
+            return f"{value_dumped}"
 
 
 class DimensionSet(list, Node):
     def __init__(self, foam_units):
         if not all(isinstance(elem, int) for elem in foam_units):
             raise ValueError("Bad {foam_units = }")
         super().__init__(foam_units)
@@ -172,18 +280,19 @@
     def __repr__(self):
         return foam_units2str(self)
 
     def dump_without_assignment(self, indent=0):
         return "[" + " ".join(str(number) for number in self) + "]"
 
 
-class Dict(dict, Node):
-    def __init__(self, data, name=None, directive=None):
+class Dict(dict, Node, NodeLikePyDict):
+    def __init__(self, data, name=None, directive=None, comments=None):
         self._name = name
         self._directive = directive
+        self.comments = comments
         super().__init__(**data)
 
     def get_name(self):
         return self._name
 
     def __repr__(self):
         return super().__repr__()
@@ -193,35 +302,44 @@
         indentation = indent * " "
         if self._name is not None:
             line = indentation + self._name
             if self._directive is not None:
                 line += "  " + self._directive
             tmp.append(line + f"\n{indentation}" + "{")
 
-        try:
-            max_length = max(len(key) for key in self)
-        except ValueError:
-            max_length = 0
-
-        default_space = 4
-        num_spaces = max_length + default_space
+        num_spaces = _compute_spaces_to_align(self)
         for key, node in self.items():
+            if self.comments is not None and key in self.comments:
+                comment = self.comments[key]
+                if isinstance(comment, str):
+                    tmp.append("    // " + comment.replace("\n", "\n    // "))
+
             if hasattr(node, "dump"):
                 tmp.append(node.dump(indent + 4))
-            elif hasattr(node, "dump_without_assignment"):
-                tmp.append(f"    {key}  {node.dump_without_assignment()};")
             else:
+                if hasattr(node, "dump_without_assignment"):
+                    code_node = node.dump_without_assignment()
+                else:
+                    code_node = node
                 if node == "":
                     s = ""
                 else:
-                    s = (num_spaces - len(key)) * " "
-                tmp.append(indentation + f"    {key}{s}{node};")
+                    s = max(2, (num_spaces - len(key))) * " "
+                tmp.append(indentation + f"    {key}{s}{code_node};")
         tmp.append(indentation + "}")
+
+        # because OpenFOAM inconsistency
+        if isinstance(self, CodeStream):
+            tmp[-1] += ";"
+
         return "\n".join(tmp)
 
+    def _set_item(self, key, value):
+        self[key] = value
+
 
 class List(list, Node):
     """Represents an OpenFoam list"""
 
     def __init__(self, iterable=None, name=None):
         self._name = name
         super().__init__(iterable)
@@ -241,15 +359,15 @@
     def __repr__(self):
         return super().__repr__()
 
     def _make_list_strings(self, indent):
         return [self._dump_item(item, indent) for item in self]
 
     def _dump_item(self, item, indent=0):
-        if hasattr(item, "dump"):
+        if isinstance(item, (Node, Assignment)) and hasattr(item, "dump"):
             return item.dump(indent)
         else:
             return indent * " " + str(item)
 
     def dump(self, indent=0):
         tmp = []
         indentation = indent * " "
@@ -319,15 +437,15 @@
         indentation4 = (indent + 4) * " "
         start = indentation + self.name
         if self.directive is not None:
             start += " " + self.directive
         tmp.append(start + f"\n{indentation}" + "#{")
         for line in self.code.split("\n"):
             tmp.append(indentation4 + line)
-        tmp.append(indentation + "#};\n")
+        tmp.append(indentation + "#};")
         return "\n".join(tmp)
 
 
 @dataclass
 class Name(Node):
     def __init__(self, name, value=None):
         self.name = name
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/LICENSE` & `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/LICENSE`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/__init__.py` & `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Utility to create blockMeshDict files
+"""Helper to create blockMeshDict files
 
 Taken from https://github.com/takaakiaoki/ofblockmeshdicthelper (Git commit
 58589f1) and modified as follow:
 
 - ``pyupgrade __init__.py --py39-plus``
 - tested (100% coverage) and reproducible (sets sorted)
 - refactor
@@ -113,16 +113,16 @@
     def face(self, index, name=None):
         """Generate Face object
         index is number or keyword to identify the face of Hex
             0 = 'w' = 'xm' = '-100' = (0 4 7 3)
             1 = 'e' = 'xp' = '100' = (1 2 5 6)
             2 = 's' = 'ym' = '0-10' = (0 1 5 4)
             3 = 'n' = 'yp' = '010' = (2 3 7 6)
-            4 = 'b' = 'zm' = '00-1' = (0 3 2 1)
-            5 = 't' = zp' = '001' = (4 5 6 7)
+            4 = 'b' = 'zm' = '00-1' = (0 3 2 1) = "bottom"
+            5 = 't' = 'zp' = '001' = (4 5 6 7) = "top"
         name is given to Face instance. If omitted, name is automatically
             genaratied like ('f-' + self.name + '-w')
         """
         kw_to_index = {
             "w": 0,
             "xm": 0,
             "-100": 0,
@@ -132,17 +132,19 @@
             "s": 2,
             "ym": 2,
             "0-10": 2,
             "n": 3,
             "yp": 3,
             "010": 3,
             "b": 4,
+            "bottom": 4,
             "zm": 4,
             "00-1": 4,
             "t": 5,
+            "top": 5,
             "zp": 5,
             "001": 5,
         }
         index_to_vertex = [
             (0, 4, 7, 3),
             (1, 2, 6, 5),
             (0, 1, 5, 4),
@@ -323,15 +325,20 @@
         self._vertices_in_blockmesh = []
         for b in self.blocks.values():
             for n in b.vnames:
                 v = self.vertices[n]
                 if v.name not in vnames_kept:
                     vnames_kept.add(v.name)
                     self._vertices_in_blockmesh.append(v)
-        if sort:
+        if sort == "as_added":
+            self._vertices_in_blockmesh = []
+            for vname, v in self.vertices.items():
+                if vname in vnames_kept:
+                    self._vertices_in_blockmesh.append(v)
+        elif sort:
             self._vertices_in_blockmesh = sorted(self._vertices_in_blockmesh)
         for i, v in enumerate(self._vertices_in_blockmesh):
             v.index = i
 
     def format_vertices_section(self):
         """format vertices section.
         assign_vertexid() should be called before this method, because
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/__pycache__/__init__.cpython-310.pyc` & `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Apr 26 14:48:53 2023 UTC, .py size: 13165 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,897 +1,905 @@
-00000000: 6f0d 0d0a 0000 0000 d539 4964 6d33 0000  o........9Idm3..
+00000000: 6f0d 0d0a 0000 0000 88b0 5464 9334 0000  o.........Td.4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6404 6405 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6406 6407 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 0100 6406 6408 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6700  m.Z.m.Z.m.Z...g.
 00000080: 6409 a201 5a0f 4700 640a 640b 8400 640b  d...Z.G.d.d...d.
 00000090: 8302 5a10 4700 640c 640d 8400 640d 8302  ..Z.G.d.d...d...
 000000a0: 5a11 4700 640e 640f 8400 640f 8302 5a12  Z.G.d.d...d...Z.
 000000b0: 4700 6410 6411 8400 6411 8302 5a13 4700  G.d.d...d...Z.G.
 000000c0: 6412 6413 8400 6413 8302 5a14 4700 6414  d.d...d...Z.G.d.
 000000d0: 6415 8400 6415 8302 5a15 6416 5300 2917  d...d...Z.d.S.).
-000000e0: 6121 0100 0055 7469 6c69 7479 2074 6f20  a!...Utility to 
-000000f0: 6372 6561 7465 2062 6c6f 636b 4d65 7368  create blockMesh
-00000100: 4469 6374 2066 696c 6573 0a0a 5461 6b65  Dict files..Take
-00000110: 6e20 6672 6f6d 2068 7474 7073 3a2f 2f67  n from https://g
-00000120: 6974 6875 622e 636f 6d2f 7461 6b61 616b  ithub.com/takaak
-00000130: 6961 6f6b 692f 6f66 626c 6f63 6b6d 6573  iaoki/ofblockmes
-00000140: 6864 6963 7468 656c 7065 7220 2847 6974  hdicthelper (Git
-00000150: 2063 6f6d 6d69 740a 3538 3538 3966 3129   commit.58589f1)
-00000160: 2061 6e64 206d 6f64 6966 6965 6420 6173   and modified as
-00000170: 2066 6f6c 6c6f 773a 0a0a 2d20 6060 7079   follow:..- ``py
-00000180: 7570 6772 6164 6520 5f5f 696e 6974 5f5f  upgrade __init__
-00000190: 2e70 7920 2d2d 7079 3339 2d70 6c75 7360  .py --py39-plus`
-000001a0: 600a 2d20 7465 7374 6564 2028 3130 3025  `.- tested (100%
-000001b0: 2063 6f76 6572 6167 6529 2061 6e64 2072   coverage) and r
-000001c0: 6570 726f 6475 6369 626c 6520 2873 6574  eproducible (set
-000001d0: 7320 736f 7274 6564 290a 2d20 7265 6661  s sorted).- refa
-000001e0: 6374 6f72 0a2d 2073 7570 706f 7274 2066  ctor.- support f
-000001f0: 6f72 2063 7963 6c69 6320 626f 756e 6461  or cyclic bounda
-00000200: 7269 6573 0a0a e900 0000 0029 01da 0767  ries.......)...g
-00000210: 726f 7570 6279 2901 da08 5465 6d70 6c61  roupby)...Templa
-00000220: 7465 e902 0000 0029 01da 0e44 4546 4155  te.....)...DEFAU
-00000230: 4c54 5f48 4541 4445 52e9 0100 0000 2902  LT_HEADER.....).
-00000240: da07 4172 6345 6467 65da 0a53 706c 696e  ..ArcEdge..Splin
-00000250: 6545 6467 6529 04da 0b45 6467 6547 7261  eEdge)...EdgeGra
-00000260: 6469 6e67 da07 4772 6164 696e 67da 0d53  ding..Grading..S
-00000270: 696d 706c 6547 7261 6469 6e67 da14 5369  impleGrading..Si
-00000280: 6d70 6c65 4772 6164 696e 6745 6c65 6d65  mpleGradingEleme
-00000290: 6e74 2906 720a 0000 0072 0c00 0000 720b  nt).r....r....r.
-000002a0: 0000 0072 0900 0000 7207 0000 0072 0800  ...r....r....r..
-000002b0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000002c0: 0000 0003 0000 0040 0000 0073 3600 0000  .......@...s6...
-000002d0: 6500 5a01 6400 5a02 640c 6402 6403 8401  e.Z.d.Z.d.d.d...
-000002e0: 5a03 6404 6405 8400 5a04 6406 6407 8400  Z.d.d...Z.d.d...
-000002f0: 5a05 6408 6409 8400 5a06 640a 640b 8400  Z.d.d...Z.d.d...
-00000300: 5a07 6401 5300 290d da06 5665 7274 6578  Z.d.S.)...Vertex
-00000310: 4e63 0600 0000 0000 0000 0000 0000 0600  Nc..............
-00000320: 0000 0200 0000 4300 0000 732a 0000 007c  ......C...s*...|
-00000330: 017c 005f 007c 027c 005f 017c 037c 005f  .|._.|.|._.|.|._
-00000340: 027c 047c 005f 037c 0468 017c 005f 047c  .|.|._.|.h.|._.|
-00000350: 057c 005f 0564 0053 00a9 014e 2906 da01  .|._.d.S...N)...
-00000360: 78da 0179 da01 7ada 046e 616d 65da 0561  x..y..z..name..a
-00000370: 6c69 6173 da05 696e 6465 7829 06da 0473  lias..index)...s
-00000380: 656c 6672 0f00 0000 7210 0000 0072 1100  elfr....r....r..
-00000390: 0000 7212 0000 0072 1400 0000 a900 7216  ..r....r......r.
-000003a0: 0000 00fa 5b2f 686f 6d65 2f70 6965 7272  ....[/home/pierr
-000003b0: 652f 4465 762f 666c 7569 6473 696d 666f  e/Dev/fluidsimfo
-000003c0: 616d 2f73 7263 2f66 6c75 6964 7369 6d66  am/src/fluidsimf
-000003d0: 6f61 6d2f 666f 616d 5f69 6e70 7574 5f66  oam/foam_input_f
-000003e0: 696c 6573 2f62 6c6f 636b 6d65 7368 6865  iles/blockmeshhe
-000003f0: 6c70 6572 2f5f 5f69 6e69 745f 5f2e 7079  lper/__init__.py
-00000400: da08 5f5f 696e 6974 5f5f 1f00 0000 730c  ..__init__....s.
-00000410: 0000 0006 0106 0106 0106 0108 010a 047a  ...............z
-00000420: 0f56 6572 7465 782e 5f5f 696e 6974 5f5f  .Vertex.__init__
-00000430: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000440: 0008 0000 0043 0000 0073 6000 0000 7c00  .....C...s`...|.
-00000450: 6a00 9b00 6401 7c00 6a01 9b00 9d03 7d01  j...d.|.j.....}.
-00000460: 7402 7c00 6a03 8301 6402 6b04 721c 7c01  t.|.j...d.k.r.|.
-00000470: 6403 6401 a004 7405 7c00 6a03 8301 a101  d.d...t.|.j.....
-00000480: 1700 3700 7d01 6404 7c00 6a06 6405 9b04  ..7.}.d.|.j.d...
-00000490: 6401 7c00 6a07 6405 9b04 6401 7c00 6a08  d.|.j.d...d.|.j.
-000004a0: 6405 9b04 6406 7c01 9b00 9d08 5300 2907  d...d.|.....S.).
-000004b0: 4eda 0120 7206 0000 007a 0320 3a20 fa02  N.. r....z. : ..
-000004c0: 2820 fa06 3138 2e31 3567 7a07 2029 2020  ( ..18.15gz. )  
-000004d0: 2f2f 2029 0972 1400 0000 7212 0000 00da  // ).r....r.....
-000004e0: 036c 656e 7213 0000 00da 046a 6f69 6eda  .lenr......join.
-000004f0: 0673 6f72 7465 6472 0f00 0000 7210 0000  .sortedr....r...
-00000500: 0072 1100 0000 2902 7215 0000 00da 0763  .r....).r......c
-00000510: 6f6d 6d65 6e74 7216 0000 0072 1600 0000  ommentr....r....
-00000520: 7217 0000 00da 0666 6f72 6d61 742a 0000  r......format*..
-00000530: 0073 0a00 0000 1201 0e01 1801 2602 02ff  .s..........&...
-00000540: 7a0d 5665 7274 6578 2e66 6f72 6d61 7463  z.Vertex.formatc
-00000550: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000560: 0400 0000 4300 0000 7320 0000 007c 006a  ....C...s ...|.j
-00000570: 007c 006a 017c 006a 0266 037c 016a 007c  .|.j.|.j.f.|.j.|
-00000580: 016a 017c 016a 0266 036b 0053 0072 0e00  .j.|.j.f.k.S.r..
-00000590: 0000 a903 7211 0000 0072 1000 0000 720f  ....r....r....r.
-000005a0: 0000 00a9 0272 1500 0000 da03 7268 7372  .....r......rhsr
-000005b0: 1600 0000 7216 0000 0072 1700 0000 da06  ....r....r......
-000005c0: 5f5f 6c74 5f5f 3200 0000 f302 0000 0020  __lt__2........ 
-000005d0: 017a 0d56 6572 7465 782e 5f5f 6c74 5f5f  .z.Vertex.__lt__
-000005e0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-000005f0: 0004 0000 0043 0000 0073 2000 0000 7c00  .....C...s ...|.
-00000600: 6a00 7c00 6a01 7c00 6a02 6603 7c01 6a00  j.|.j.|.j.f.|.j.
-00000610: 7c01 6a01 7c01 6a02 6603 6b02 5300 720e  |.j.|.j.f.k.S.r.
-00000620: 0000 0072 2100 0000 7222 0000 0072 1600  ...r!...r"...r..
-00000630: 0000 7216 0000 0072 1700 0000 da06 5f5f  ..r....r......__
-00000640: 6571 5f5f 3500 0000 7225 0000 007a 0d56  eq__5...r%...z.V
-00000650: 6572 7465 782e 5f5f 6571 5f5f 6301 0000  ertex.__eq__c...
-00000660: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-00000670: 0043 0000 0073 1400 0000 7400 7c00 6a01  .C...s....t.|.j.
-00000680: 7c00 6a02 7c00 6a03 6603 8301 5300 720e  |.j.|.j.f...S.r.
-00000690: 0000 0029 04da 0468 6173 6872 1100 0000  ...)...hashr....
-000006a0: 7210 0000 0072 0f00 0000 a901 7215 0000  r....r......r...
-000006b0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-000006c0: da08 5f5f 6861 7368 5f5f 3800 0000 7302  ..__hash__8...s.
-000006d0: 0000 0014 017a 0f56 6572 7465 782e 5f5f  .....z.Vertex.__
-000006e0: 6861 7368 5f5f 720e 0000 0029 08da 085f  hash__r....)..._
-000006f0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000700: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000710: 5f72 1800 0000 7220 0000 0072 2400 0000  _r....r ...r$...
-00000720: 7226 0000 0072 2900 0000 7216 0000 0072  r&...r)...r....r
-00000730: 1600 0000 7216 0000 0072 1700 0000 720d  ....r....r....r.
-00000740: 0000 001e 0000 0073 0c00 0000 0800 0a01  .......s........
-00000750: 080b 0808 0803 0c03 720d 0000 0063 0000  ........r....c..
-00000760: 0000 0000 0000 0000 0000 0000 0000 0200  ................
-00000770: 0000 4000 0000 f31c 0000 0065 005a 0164  ..@........e.Z.d
-00000780: 005a 0264 0164 0284 005a 0364 0364 0484  .Z.d.d...Z.d.d..
-00000790: 005a 0464 0553 0029 06da 0550 6f69 6e74  .Z.d.S.)...Point
-000007a0: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
-000007b0: 0002 0000 0043 0000 0073 1600 0000 7c01  .....C...s....|.
-000007c0: 7c00 5f00 7c02 7c00 5f01 7c03 7c00 5f02  |._.|.|._.|.|._.
-000007d0: 6400 5300 720e 0000 00a9 0372 0f00 0000  d.S.r......r....
-000007e0: 7210 0000 0072 1100 0000 2904 7215 0000  r....r....).r...
-000007f0: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
-00000800: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00000810: 1800 0000 3d00 0000 7306 0000 0006 0106  ....=...s.......
-00000820: 010a 017a 0e50 6f69 6e74 2e5f 5f69 6e69  ...z.Point.__ini
-00000830: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
-00000840: 0100 0000 0700 0000 4300 0000 7324 0000  ........C...s$..
-00000850: 0064 017c 006a 0064 029b 0464 037c 006a  .d.|.j.d...d.|.j
-00000860: 0164 029b 0464 037c 006a 0264 029b 0464  .d...d.|.j.d...d
-00000870: 049d 0753 0029 054e 721a 0000 0072 1b00  ...S.).Nr....r..
-00000880: 0000 7219 0000 007a 0220 2972 2f00 0000  ..r....z. )r/...
-00000890: 7228 0000 0072 1600 0000 7216 0000 0072  r(...r....r....r
-000008a0: 1700 0000 7220 0000 0042 0000 0073 0200  ....r ...B...s..
-000008b0: 0000 2401 7a0c 506f 696e 742e 666f 726d  ..$.z.Point.form
-000008c0: 6174 4ea9 0572 2a00 0000 722b 0000 0072  atN..r*...r+...r
-000008d0: 2c00 0000 7218 0000 0072 2000 0000 7216  ,...r....r ...r.
-000008e0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-000008f0: 0000 722e 0000 003c 0000 0073 0600 0000  ..r....<...s....
-00000900: 0800 0801 0c05 722e 0000 0063 0000 0000  ......r....c....
-00000910: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-00000920: 4000 0000 722d 0000 0029 06da 0446 6163  @...r-...)...Fac
-00000930: 6563 0300 0000 0000 0000 0000 0000 0300  ec..............
-00000940: 0000 0200 0000 4300 0000 7310 0000 007c  ......C...s....|
-00000950: 017c 005f 007c 027c 005f 0164 0153 0029  .|._.|.|._.d.S.)
-00000960: 027a 380a 2020 2020 2020 2020 766e 616d  .z8.        vnam
-00000970: 6520 6973 206c 6973 7420 6f72 2074 7570  e is list or tup
-00000980: 6c65 206f 6620 7665 7274 6578 206e 616d  le of vertex nam
-00000990: 6573 0a20 2020 2020 2020 204e 2902 da06  es.        N)...
-000009a0: 766e 616d 6573 7212 0000 0029 0372 1500  vnamesr....).r..
-000009b0: 0000 7232 0000 0072 1200 0000 7216 0000  ..r2...r....r...
-000009c0: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-000009d0: 4700 0000 7304 0000 0006 040a 017a 0d46  G...s........z.F
-000009e0: 6163 652e 5f5f 696e 6974 5f5f 6302 0000  ace.__init__c...
-000009f0: 0000 0000 0000 0000 0004 0000 0007 0000  ................
-00000a00: 0003 0000 0073 4600 0000 6401 a000 8700  .....sF...d.....
-00000a10: 6601 6402 6403 8408 7c00 6a01 4400 8301  f.d.d...|.j.D...
-00000a20: a101 7d02 6401 a000 7c00 6a01 a101 7d03  ..}.d...|.j...}.
-00000a30: 6404 7c02 6405 9b04 6406 7c00 6a02 6405  d.|.d...d.|.j.d.
-00000a40: 9b04 6407 7c03 6405 9b04 6408 9d07 5300  ..d.|.d...d...S.
-00000a50: 2909 fa4b 466f 726d 6174 2069 6e73 7461  )..KFormat insta
-00000a60: 6e63 6520 746f 2064 756d 700a 2020 2020  nce to dump.    
-00000a70: 2020 2020 7665 7274 6963 6573 2069 7320      vertices is 
-00000a80: 6469 6374 206f 6620 6e61 6d65 2074 6f20  dict of name to 
-00000a90: 5665 7274 6578 0a20 2020 2020 2020 2072  Vertex.        r
-00000aa0: 1900 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00000ab0: 0002 0000 0004 0000 0033 0000 00f3 1e00  .........3......
-00000ac0: 0000 8100 7c00 5d0a 7d01 7400 8800 7c01  ....|.].}.t...|.
-00000ad0: 1900 6a01 8301 5600 0100 7102 6400 5300  ..j...V...q.d.S.
-00000ae0: 720e 0000 00a9 02da 0373 7472 7214 0000  r........strr...
-00000af0: 00a9 02da 022e 30da 0276 6ea9 01da 0876  ......0..vn....v
-00000b00: 6572 7469 6365 7372 1600 0000 7217 0000  erticesr....r...
-00000b10: 00da 093c 6765 6e65 7870 723e 5200 0000  ...<genexpr>R...
-00000b20: f304 0000 0002 801c 007a 1e46 6163 652e  .........z.Face.
-00000b30: 666f 726d 6174 2e3c 6c6f 6361 6c73 3e2e  format.<locals>.
-00000b40: 3c67 656e 6578 7072 3efa 0128 da01 737a  <genexpr>..(..sz
-00000b50: 0629 2020 2f2f 20fa 0220 28fa 0129 2903  .)  // .. (..)).
-00000b60: 721d 0000 0072 3200 0000 7212 0000 00a9  r....r2...r.....
-00000b70: 0472 1500 0000 723b 0000 0072 1400 0000  .r....r;...r....
-00000b80: 721f 0000 0072 1600 0000 723a 0000 0072  r....r....r:...r
-00000b90: 1700 0000 7220 0000 004e 0000 0073 0600  ....r ...N...s..
-00000ba0: 0000 1a04 0c01 2001 7a0b 4661 6365 2e66  ...... .z.Face.f
-00000bb0: 6f72 6d61 744e 7230 0000 0072 1600 0000  ormatNr0...r....
-00000bc0: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00000bd0: 3100 0000 4600 0000 7306 0000 0008 0008  1...F...s.......
-00000be0: 010c 0772 3100 0000 6300 0000 0000 0000  ...r1...c.......
-00000bf0: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000c00: 0073 3200 0000 6500 5a01 6400 5a02 6503  .s2...e.Z.d.Z.e.
-00000c10: 6401 6401 6401 8303 6601 6402 6403 8401  d.d.d...f.d.d...
-00000c20: 5a04 6404 6405 8400 5a05 6409 6407 6408  Z.d.d...Z.d.d.d.
-00000c30: 8401 5a06 6406 5300 290a da08 4865 7842  ..Z.d.S.)...HexB
-00000c40: 6c6f 636b 7206 0000 0063 0500 0000 0000  lockr....c......
-00000c50: 0000 0000 0000 0500 0000 0200 0000 4300  ..............C.
-00000c60: 0000 731c 0000 007c 017c 005f 007c 027c  ..s....|.|._.|.|
-00000c70: 005f 017c 037c 005f 027c 047c 005f 0364  ._.|.|._.|.|._.d
-00000c80: 0153 0029 0261 2e01 0000 496e 6974 6961  .S.).a....Initia
-00000c90: 6c69 7a65 2048 6578 426c 6f63 6b20 696e  lize HexBlock in
-00000ca0: 7374 616e 6365 0a20 2020 2020 2020 2076  stance.        v
-00000cb0: 6e61 6d65 7320 6973 2074 6865 2076 6572  names is the ver
-00000cc0: 7465 7820 6e61 6d65 7320 696e 206f 7264  tex names in ord
-00000cd0: 6572 2064 6573 6372 6976 6564 2069 6e0a  er descrived in.
-00000ce0: 2020 2020 2020 2020 2020 2020 6874 7470              http
-00000cf0: 3a2f 2f77 7777 2e6f 7065 6e66 6f61 6d2e  ://www.openfoam.
-00000d00: 6f72 672f 646f 6373 2f75 7365 722f 6d65  org/docs/user/me
-00000d10: 7368 2d64 6573 6372 6970 7469 6f6e 2e70  sh-description.p
-00000d20: 6870 0a20 2020 2020 2020 2063 656c 6c73  hp.        cells
-00000d30: 2069 7320 6e75 6d62 6572 206f 6620 6365   is number of ce
-00000d40: 6c6c 7320 6465 7669 6564 2069 6e74 6f20  lls devied into 
-00000d50: 696e 2065 6163 6820 6469 7265 6374 696f  in each directio
-00000d60: 6e0a 2020 2020 2020 2020 6e61 6d65 2069  n.        name i
-00000d70: 7320 7468 6520 756e 6971 206e 616d 6520  s the uniq name 
-00000d80: 6f66 2074 6865 2062 6c6f 636b 0a20 2020  of the block.   
-00000d90: 2020 2020 2067 7261 6469 6e67 2069 7320       grading is 
-00000da0: 6772 6164 696e 6720 6d65 7468 6f64 2e0a  grading method..
-00000db0: 2020 2020 2020 2020 4e29 0472 3200 0000          N).r2...
-00000dc0: da05 6365 6c6c 7372 1200 0000 da07 6772  ..cellsr......gr
-00000dd0: 6164 696e 6729 0572 1500 0000 7232 0000  ading).r....r2..
-00000de0: 0072 4400 0000 7212 0000 0072 4500 0000  .rD...r....rE...
-00000df0: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00000e00: 1800 0000 5800 0000 7308 0000 0006 0806  ....X...s.......
-00000e10: 0106 010a 017a 1148 6578 426c 6f63 6b2e  .....z.HexBlock.
-00000e20: 5f5f 696e 6974 5f5f 6302 0000 0000 0000  __init__c.......
-00000e30: 0000 0000 0004 0000 0011 0000 0003 0000  ................
-00000e40: 0073 7e00 0000 6401 a000 8700 6601 6402  .s~...d.....f.d.
-00000e50: 6403 8408 7c00 6a01 4400 8301 a101 7d02  d...|.j.D.....}.
-00000e60: 6401 a000 7c00 6a01 a101 7d03 6404 7c02  d...|.j...}.d.|.
-00000e70: 9b00 6405 7c00 6a02 9b00 6406 7c00 6a03  ..d.|.j...d.|.j.
-00000e80: 6407 1900 6408 9b04 6401 7c00 6a03 6409  d...d...d.|.j.d.
-00000e90: 1900 6408 9b04 6401 7c00 6a03 640a 1900  ..d...d.|.j.d...
-00000ea0: 6408 9b04 6405 7c00 6a04 a005 a100 9b00  d...d.|.j.......
-00000eb0: 640b 7c00 6a02 9b00 6406 7c03 9b00 640c  d.|.j...d.|...d.
-00000ec0: 9d11 5300 290d 7233 0000 0072 1900 0000  ..S.).r3...r....
-00000ed0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000ee0: 0004 0000 0033 0000 0072 3400 0000 720e  .....3...r4...r.
-00000ef0: 0000 0072 3500 0000 7237 0000 0072 3a00  ...r5...r7...r:.
-00000f00: 0000 7216 0000 0072 1700 0000 723c 0000  ..r....r....r<..
-00000f10: 0069 0000 0072 3d00 0000 7a22 4865 7842  .i...r=...z"HexB
-00000f20: 6c6f 636b 2e66 6f72 6d61 742e 3c6c 6f63  lock.format.<loc
-00000f30: 616c 733e 2e3c 6765 6e65 7870 723e 7a05  als>.<genexpr>z.
-00000f40: 6865 7820 287a 0229 2072 4000 0000 7201  hex (z.) r@...r.
-00000f50: 0000 00da 0164 7206 0000 0072 0400 0000  .....dr....r....
-00000f60: 7a05 2020 2f2f 2072 4100 0000 2906 721d  z.  // rA...).r.
-00000f70: 0000 0072 3200 0000 7212 0000 0072 4400  ...r2...r....rD.
-00000f80: 0000 7245 0000 0072 2000 0000 7242 0000  ..rE...r ...rB..
-00000f90: 0072 1600 0000 723a 0000 0072 1700 0000  .r....r:...r....
-00000fa0: 7220 0000 0065 0000 0073 2000 0000 1a04  r ...e...s .....
-00000fb0: 0c01 1002 0a01 04ff 0a01 04ff 0a01 04ff  ................
-00000fc0: 0802 04fe 0402 04fe 0202 06fe 02ff 7a0f  ..............z.
-00000fd0: 4865 7842 6c6f 636b 2e66 6f72 6d61 744e  HexBlock.formatN
-00000fe0: 6303 0000 0000 0000 0000 0000 0007 0000  c...............
-00000ff0: 0004 0000 0003 0000 0073 d000 0000 6900  .........s....i.
-00001000: 6401 6402 9301 6403 6402 9301 6404 6402  d.d...d.d...d.d.
-00001010: 9301 6405 6406 9301 6407 6406 9301 6408  ..d.d...d.d...d.
-00001020: 6406 9301 6409 640a 9301 640b 640a 9301  d...d.d...d.d...
-00001030: 640c 640a 9301 640d 640e 9301 640f 640e  d.d...d.d...d.d.
-00001040: 9301 6410 640e 9301 6411 6412 9301 6413  ..d.d...d.d...d.
-00001050: 6412 9301 6414 6412 9301 6415 6416 9301  d...d.d...d.d...
-00001060: 6417 6416 9301 6418 6416 6901 a501 7d03  d.d...d.d.i...}.
-00001070: 6700 6419 a201 7d04 6700 641a a201 7d05  g.d...}.g.d...}.
-00001080: 7400 7c01 7401 8302 724a 7c03 7c01 1900  t.|.t...rJ|.|...
-00001090: 7d01 7402 8700 6601 641b 641c 8408 7c04  }.t...f.d.d...|.
-000010a0: 7c01 1900 4400 8301 8301 7d06 7c02 641d  |...D.....}.|.d.
-000010b0: 7500 7263 7c05 7c01 1900 a003 8800 6a04  u.rc|.|.......j.
-000010c0: a101 7d02 7405 7c06 7c02 8302 5300 291e  ..}.t.|.|...S.).
-000010d0: 61f8 0100 0047 656e 6572 6174 6520 4661  a....Generate Fa
-000010e0: 6365 206f 626a 6563 740a 2020 2020 2020  ce object.      
-000010f0: 2020 696e 6465 7820 6973 206e 756d 6265    index is numbe
-00001100: 7220 6f72 206b 6579 776f 7264 2074 6f20  r or keyword to 
-00001110: 6964 656e 7469 6679 2074 6865 2066 6163  identify the fac
-00001120: 6520 6f66 2048 6578 0a20 2020 2020 2020  e of Hex.       
-00001130: 2020 2020 2030 203d 2027 7727 203d 2027       0 = 'w' = '
-00001140: 786d 2720 3d20 272d 3130 3027 203d 2028  xm' = '-100' = (
-00001150: 3020 3420 3720 3329 0a20 2020 2020 2020  0 4 7 3).       
-00001160: 2020 2020 2031 203d 2027 6527 203d 2027       1 = 'e' = '
-00001170: 7870 2720 3d20 2731 3030 2720 3d20 2831  xp' = '100' = (1
-00001180: 2032 2035 2036 290a 2020 2020 2020 2020   2 5 6).        
-00001190: 2020 2020 3220 3d20 2773 2720 3d20 2779      2 = 's' = 'y
-000011a0: 6d27 203d 2027 302d 3130 2720 3d20 2830  m' = '0-10' = (0
-000011b0: 2031 2035 2034 290a 2020 2020 2020 2020   1 5 4).        
-000011c0: 2020 2020 3320 3d20 276e 2720 3d20 2779      3 = 'n' = 'y
-000011d0: 7027 203d 2027 3031 3027 203d 2028 3220  p' = '010' = (2 
-000011e0: 3320 3720 3629 0a20 2020 2020 2020 2020  3 7 6).         
-000011f0: 2020 2034 203d 2027 6227 203d 2027 7a6d     4 = 'b' = 'zm
-00001200: 2720 3d20 2730 302d 3127 203d 2028 3020  ' = '00-1' = (0 
-00001210: 3320 3220 3129 0a20 2020 2020 2020 2020  3 2 1).         
-00001220: 2020 2035 203d 2027 7427 203d 207a 7027     5 = 't' = zp'
-00001230: 203d 2027 3030 3127 203d 2028 3420 3520   = '001' = (4 5 
-00001240: 3620 3729 0a20 2020 2020 2020 206e 616d  6 7).        nam
-00001250: 6520 6973 2067 6976 656e 2074 6f20 4661  e is given to Fa
-00001260: 6365 2069 6e73 7461 6e63 652e 2049 6620  ce instance. If 
-00001270: 6f6d 6974 7465 642c 206e 616d 6520 6973  omitted, name is
-00001280: 2061 7574 6f6d 6174 6963 616c 6c79 0a20   automatically. 
-00001290: 2020 2020 2020 2020 2020 2067 656e 6172             genar
-000012a0: 6174 6965 6420 6c69 6b65 2028 2766 2d27  atied like ('f-'
-000012b0: 202b 2073 656c 662e 6e61 6d65 202b 2027   + self.name + '
-000012c0: 2d77 2729 0a20 2020 2020 2020 20da 0177  -w').        ..w
-000012d0: 7201 0000 00da 0278 6d7a 042d 3130 30da  r......xmz.-100.
-000012e0: 0165 7206 0000 00da 0278 70da 0331 3030  .er......xp..100
-000012f0: 723f 0000 0072 0400 0000 da02 796d 7a04  r?...r......ymz.
-00001300: 302d 3130 da01 6ee9 0300 0000 da02 7970  0-10..n.......yp
-00001310: 5a03 3031 30da 0162 e904 0000 00da 027a  Z.010..b.......z
-00001320: 6d7a 0430 302d 31da 0174 e905 0000 00da  mz.00-1..t......
-00001330: 027a 705a 0330 3031 2906 2904 7201 0000  .zpZ.001).).r...
-00001340: 0072 5100 0000 e907 0000 0072 4e00 0000  .rQ........rN...
-00001350: 2904 7206 0000 0072 0400 0000 e906 0000  ).r....r........
-00001360: 0072 5400 0000 2904 7201 0000 0072 0600  .rT...).r....r..
-00001370: 0000 7254 0000 0072 5100 0000 2904 7204  ..rT...rQ...).r.
-00001380: 0000 0072 4e00 0000 7256 0000 0072 5700  ...rN...rV...rW.
-00001390: 0000 2904 7201 0000 0072 4e00 0000 7204  ..).r....rN...r.
-000013a0: 0000 0072 0600 0000 2904 7251 0000 0072  ...r....).rQ...r
-000013b0: 5400 0000 7257 0000 0072 5600 0000 2906  T...rW...rV...).
-000013c0: 7a06 662d 7b7d 2d77 fa06 662d 7b7d 2d6e  z.f-{}-w..f-{}-n
-000013d0: 7a06 662d 7b7d 2d73 7258 0000 007a 0666  z.f-{}-srX...z.f
-000013e0: 2d7b 7d2d 627a 0666 2d7b 7d2d 7463 0100  -{}-bz.f-{}-tc..
-000013f0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00001400: 0000 1300 0000 7316 0000 0067 007c 005d  ......s....g.|.]
-00001410: 077d 0188 006a 007c 0119 0091 0271 0253  .}...j.|.....q.S
-00001420: 0072 1600 0000 2901 7232 0000 0029 0272  .r....).r2...).r
-00001430: 3800 0000 da01 6972 2800 0000 7216 0000  8.....ir(...r...
-00001440: 0072 1700 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
-00001450: 703e a500 0000 7302 0000 0016 007a 2148  p>....s......z!H
-00001460: 6578 426c 6f63 6b2e 6661 6365 2e3c 6c6f  exBlock.face.<lo
-00001470: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00001480: 4e29 06da 0a69 7369 6e73 7461 6e63 6572  N)...isinstancer
-00001490: 3600 0000 da05 7475 706c 6572 2000 0000  6.....tupler ...
-000014a0: 7212 0000 0072 3100 0000 2907 7215 0000  r....r1...).r...
-000014b0: 0072 1400 0000 7212 0000 005a 0b6b 775f  .r....r....Z.kw_
-000014c0: 746f 5f69 6e64 6578 5a0f 696e 6465 785f  to_indexZ.index_
-000014d0: 746f 5f76 6572 7465 785a 1669 6e64 6578  to_vertexZ.index
-000014e0: 5f74 6f5f 6465 6661 756c 7473 7566 6669  _to_defaultsuffi
-000014f0: 7872 3200 0000 7216 0000 0072 2800 0000  xr2...r....r(...
-00001500: 7217 0000 00da 0466 6163 6571 0000 0073  r......faceq...s
-00001510: 5a00 0000 020c 0401 02ff 0402 02fe 0403  Z...............
-00001520: 02fd 0404 02fc 0405 02fb 0406 02fa 0407  ................
-00001530: 02f9 0408 02f8 0409 02f7 040a 02f6 040b  ................
-00001540: 02f5 040c 02f4 040d 02f3 040e 02f2 040f  ................
-00001550: 02f1 0410 02f0 0411 02ef 0412 06ee 0814  ................
-00001560: 0808 0a09 0801 1a02 0801 1001 0a01 7a0d  ..............z.
-00001570: 4865 7842 6c6f 636b 2e66 6163 6572 0e00  HexBlock.facer..
-00001580: 0000 2907 722a 0000 0072 2b00 0000 722c  ..).r*...r+...r,
-00001590: 0000 0072 0b00 0000 7218 0000 0072 2000  ...r....r....r .
-000015a0: 0000 725d 0000 0072 1600 0000 7216 0000  ..r]...r....r...
-000015b0: 0072 1600 0000 7217 0000 0072 4300 0000  .r....r....rC...
-000015c0: 5700 0000 7308 0000 0008 0014 0108 0d0e  W...s...........
-000015d0: 0c72 4300 0000 6300 0000 0000 0000 0000  .rC...c.........
-000015e0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-000015f0: 2600 0000 6500 5a01 6400 5a02 6408 6402  &...e.Z.d.Z.d.d.
-00001600: 6403 8401 5a03 6404 6405 8400 5a04 6406  d...Z.d.d...Z.d.
-00001610: 6407 8400 5a05 6401 5300 2909 da08 426f  d...Z.d.S.)...Bo
-00001620: 756e 6461 7279 4e63 0500 0000 0000 0000  undaryNc........
-00001630: 0000 0000 0500 0000 0300 0000 4300 0000  ............C...
-00001640: 733a 0000 007c 017c 005f 007c 027c 005f  s:...|.|._.|.|._
-00001650: 017c 0364 0175 0072 0d67 007d 036e 0874  .|.d.u.r.g.}.n.t
-00001660: 027c 0374 0383 0272 157c 0367 017d 037c  .|.t...r.|.g.}.|
-00001670: 037c 005f 047c 047c 005f 0564 0153 0029  .|._.|.|._.d.S.)
-00001680: 027a c469 6e69 7469 616c 697a 6520 626f  .z.initialize bo
-00001690: 756e 6461 7279 0a20 2020 2020 2020 2074  undary.        t
-000016a0: 7970 655f 2069 7320 7479 7065 206b 6579  ype_ is type key
-000016b0: 776f 7264 2028 7761 6c6c 2c20 7061 7463  word (wall, patc
-000016c0: 682c 2065 6d70 7479 2c20 2e2e 290a 2020  h, empty, ..).  
-000016d0: 2020 2020 2020 6e61 6d65 2069 7320 6e61        name is na
-000016e0: 7665 206f 6620 626f 756e 6461 7279 2065  ve of boundary e
-000016f0: 6d65 6c6d 656e 740a 2020 2020 2020 2020  melment.        
-00001700: 6661 6365 7320 6973 2066 6163 6573 2077  faces is faces w
-00001710: 6869 6368 2061 7265 2061 7070 6c69 6564  hich are applied
-00001720: 2077 6974 6820 7468 6973 2062 6f75 6e64   with this bound
-00001730: 6172 7920 636f 6e64 6974 696f 6e73 0a20  ary conditions. 
-00001740: 2020 2020 2020 204e 2906 da05 7479 7065         N)...type
-00001750: 5f72 1200 0000 725b 0000 0072 3100 0000  _r....r[...r1...
-00001760: da05 6661 6365 73da 096e 6569 6768 626f  ..faces..neighbo
-00001770: 7572 2905 7215 0000 0072 5f00 0000 7212  ur).r....r_...r.
-00001780: 0000 0072 6000 0000 7261 0000 0072 1600  ...r`...ra...r..
-00001790: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
-000017a0: 00ac 0000 0073 1000 0000 0606 0601 0801  .....s..........
-000017b0: 0601 0a01 0601 0601 0a01 7a11 426f 756e  ..........z.Boun
-000017c0: 6461 7279 2e5f 5f69 6e69 745f 5f63 0200  dary.__init__c..
-000017d0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-000017e0: 0000 4300 0000 7310 0000 007c 006a 00a0  ..C...s....|.j..
-000017f0: 017c 01a1 0101 0064 0153 0029 027a 5161  .|.....d.S.).zQa
-00001800: 6464 2066 6163 6520 696e 7374 616e 6365  dd face instance
-00001810: 0a20 2020 2020 2020 2066 6163 6520 6973  .        face is
-00001820: 2061 2046 6163 6520 696e 7374 616e 6365   a Face instance
-00001830: 2028 6e6f 7420 6e61 6d65 2920 746f 2062   (not name) to b
-00001840: 6520 6164 6465 640a 2020 2020 2020 2020  e added.        
-00001850: 4e29 0272 6000 0000 da06 6170 7065 6e64  N).r`.....append
-00001860: 2902 7215 0000 0072 5d00 0000 7216 0000  ).r....r]...r...
-00001870: 0072 1600 0000 7217 0000 00da 0861 6464  .r....r......add
-00001880: 5f66 6163 65bb 0000 0073 0200 0000 1004  _face....s......
-00001890: 7a11 426f 756e 6461 7279 2e61 6464 5f66  z.Boundary.add_f
-000018a0: 6163 6563 0200 0000 0000 0000 0000 0000  acec............
-000018b0: 0400 0000 0800 0000 4300 0000 7382 0000  ........C...s...
-000018c0: 007c 006a 0067 017d 027c 006a 0164 0175  .|.j.g.}.|.j.d.u
-000018d0: 0072 167c 02a0 0264 0264 037c 006a 039b  .r.|...d.d.|.j..
-000018e0: 0064 049d 0317 00a1 0101 006e 107c 02a0  .d.........n.|..
-000018f0: 0264 0264 037c 006a 039b 0064 057c 006a  .d.d.|.j...d.|.j
-00001900: 019b 0064 049d 0517 00a1 0101 007c 006a  ...d.........|.j
-00001910: 0444 005d 0d7d 037c 02a0 0264 067c 03a0  .D.].}.|...d.|..
-00001920: 057c 01a1 019b 009d 02a1 0101 0071 297c  .|...........q)|
-00001930: 02a0 0264 07a1 0101 0064 08a0 067c 02a1  ...d.....d...|..
-00001940: 0153 0029 0972 3300 0000 4e7a 027b 0a7a  .S.).r3...Nz.{.z
-00001950: 0920 2020 2074 7970 6520 7a11 3b0a 2020  .    type z.;.  
-00001960: 2020 6661 6365 730a 2020 2020 287a 163b    faces.    (z.;
-00001970: 0a20 2020 206e 6569 6768 626f 7572 5061  .    neighbourPa
-00001980: 7463 6820 207a 0820 2020 2020 2020 207a  tch  z.        z
-00001990: 0820 2020 2029 3b0a 7dda 010a 2907 7212  .    );.}...).r.
-000019a0: 0000 0072 6100 0000 7262 0000 0072 5f00  ...ra...rb...r_.
-000019b0: 0000 7260 0000 0072 2000 0000 721d 0000  ..r`...r ...r...
-000019c0: 0029 0472 1500 0000 723b 0000 00da 0374  .).r....r;.....t
-000019d0: 6d70 da01 6672 1600 0000 7216 0000 0072  mp..fr....r....r
-000019e0: 1700 0000 7220 0000 00c1 0000 0073 1800  ....r .......s..
-000019f0: 0000 0804 0a01 1a01 0402 0201 1401 02ff  ................
-00001a00: 04ff 0a04 1801 0a01 0a01 7a0f 426f 756e  ..........z.Boun
-00001a10: 6461 7279 2e66 6f72 6d61 74a9 024e 4e29  dary.format..NN)
-00001a20: 0672 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
-00001a30: 7218 0000 0072 6300 0000 7220 0000 0072  r....rc...r ...r
-00001a40: 1600 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
-00001a50: 0000 0072 5e00 0000 ab00 0000 7308 0000  ...r^.......s...
-00001a60: 0008 000a 0108 0f0c 0672 5e00 0000 6300  .........r^...c.
-00001a70: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-00001a80: 0000 0040 0000 0073 bc00 0000 6500 5a01  ...@...s....e.Z.
-00001a90: 6400 5a02 6401 6402 8400 5a03 6403 6404  d.Z.d.d...Z.d.d.
-00001aa0: 8400 5a04 6405 6406 8400 5a05 642a 6408  ..Z.d.d...Z.d*d.
-00001ab0: 6409 8401 5a06 640a 640b 8400 5a07 640c  d...Z.d.d...Z.d.
-00001ac0: 640d 8400 5a08 640e 640f 8400 5a09 650a  d...Z.d.d...Z.e.
-00001ad0: 6410 6410 6410 8303 6601 6411 6412 8401  d.d.d...f.d.d...
-00001ae0: 5a0b 6413 6414 8400 5a0c 6415 6416 8400  Z.d.d...Z.d.d...
-00001af0: 5a0d 642b 6417 6418 8401 5a0e 6419 641a  Z.d+d.d...Z.d.d.
-00001b00: 8400 5a0f 642c 641c 641d 8401 5a10 641e  ..Z.d,d.d...Z.d.
-00001b10: 641f 8400 5a11 6420 6421 8400 5a12 6422  d...Z.d d!..Z.d"
-00001b20: 6423 8400 5a13 6424 6425 8400 5a14 6426  d#..Z.d$d%..Z.d&
-00001b30: 6427 8400 5a15 6516 641b 6602 6428 6429  d'..Z.e.d.f.d(d)
-00001b40: 8401 5a17 6407 5300 292d da0d 426c 6f63  ..Z.d.S.)-..Bloc
-00001b50: 6b4d 6573 6844 6963 7463 0100 0000 0000  kMeshDictc......
-00001b60: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00001b70: 0000 7328 0000 0064 017c 005f 0069 007c  ..s(...d.|._.i.|
-00001b80: 005f 0169 007c 005f 0269 007c 005f 0369  ._.i.|._.i.|._.i
-00001b90: 007c 005f 0464 007c 005f 0564 0053 0029  .|._.d.|._.d.S.)
-00001ba0: 024e 6700 0000 0000 00f0 3f29 06da 1163  .Ng.......?)...c
-00001bb0: 6f6e 7665 7274 5f74 6f5f 6d65 7465 7273  onvert_to_meters
-00001bc0: 723b 0000 00da 0662 6c6f 636b 73da 0565  r;.....blocks..e
-00001bd0: 6467 6573 da0a 626f 756e 6461 7269 6573  dges..boundaries
-00001be0: da16 5f76 6572 7469 6365 735f 696e 5f62  .._vertices_in_b
-00001bf0: 6c6f 636b 6d65 7368 7228 0000 0072 1600  lockmeshr(...r..
-00001c00: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
-00001c10: 00d4 0000 0073 0c00 0000 0601 0601 0601  .....s..........
-00001c20: 0601 0601 0a01 7a16 426c 6f63 6b4d 6573  ......z.BlockMes
-00001c30: 6844 6963 742e 5f5f 696e 6974 5f5f 6302  hDict.__init__c.
-00001c40: 0000 0000 0000 0000 0000 0003 0000 0009  ................
-00001c50: 0000 0043 0000 0073 2400 0000 6401 6402  ...C...s$...d.d.
-00001c60: 6403 6404 6405 6406 6407 6407 6408 9c08  d.d.d.d.d.d.d...
-00001c70: 7d02 7c02 7c01 1900 7c00 5f00 6409 5300  }.|.|...|._.d.S.
-00001c80: 290a 7a22 7365 7420 7365 6c66 2e63 6f6d  ).z"set self.com
-00001c90: 7665 7274 5f74 6f5f 6d65 7465 7273 2062  vert_to_meters b
-00001ca0: 7920 776f 7264 69e8 0300 0072 0600 0000  y wordi....r....
-00001cb0: 677b 14ae 47e1 7a84 3f67 fca9 f1d2 4d62  g{..G.z.?g....Mb
-00001cc0: 503f 678d edb5 a0f7 c6b0 3e67 95d6 26e8  P?g.......>g..&.
-00001cd0: 0b2e 113e 67bb bdd7 d9df 7cdb 3d29 08da  ...>g.....|.=)..
-00001ce0: 026b 6dda 016d da02 636d da02 6d6d da02  .km..m..cm..mm..
-00001cf0: 756d da02 6e6d da01 415a 0841 6e67 7374  um..nm..AZ.Angst
-00001d00: 726f 6d4e a901 7269 0000 0029 0372 1500  romN..ri...).r..
-00001d10: 0000 da06 6d65 7472 6963 5a17 6d65 7472  ....metricZ.metr
-00001d20: 6963 7379 6d5f 746f 5f63 6f6e 7665 7273  icsym_to_convers
-00001d30: 696f 6e72 1600 0000 7216 0000 0072 1700  ionr....r....r..
-00001d40: 0000 da0a 7365 745f 6d65 7472 6963 dc00  ....set_metric..
-00001d50: 0000 7314 0000 0002 0302 0102 0102 0102  ..s.............
-00001d60: 0102 0102 0102 0106 f80e 0a7a 1842 6c6f  ...........z.Blo
-00001d70: 636b 4d65 7368 4469 6374 2e73 6574 5f6d  ckMeshDict.set_m
-00001d80: 6574 7269 6363 0200 0000 0000 0000 0000  etricc..........
-00001d90: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
-00001da0: 0000 007c 017c 005f 0064 0053 0072 0e00  ...|.|._.d.S.r..
-00001db0: 0000 7275 0000 0029 0272 1500 0000 da05  ..ru...).r......
-00001dc0: 7363 616c 6572 1600 0000 7216 0000 0072  scaler....r....r
-00001dd0: 1700 0000 da09 7365 745f 7363 616c 65ea  ......set_scale.
-00001de0: 0000 0073 0200 0000 0a01 7a17 426c 6f63  ...s......z.Bloc
-00001df0: 6b4d 6573 6844 6963 742e 7365 745f 7363  kMeshDict.set_sc
-00001e00: 616c 654e 6305 0000 0000 0000 0000 0000  aleNc...........
-00001e10: 0006 0000 0005 0000 0043 0000 0073 5800  .........C...sX.
-00001e20: 0000 7400 7c01 7401 8302 721b 7402 6401  ..t.|.t...r.t.d.
-00001e30: 6402 8400 7c02 7c03 7c04 6603 4400 8301  d...|.|.|.f.D...
-00001e40: 8301 7215 7403 6403 8301 8201 7c01 7d05  ..r.t.d.....|.}.
-00001e50: 7c05 6a04 7d04 6e07 7401 7c01 7c02 7c03  |.j.}.n.t.|.|.|.
-00001e60: 7c04 8304 7d05 7c05 7c00 6a05 7c04 3c00  |...}.|.|.j.|.<.
-00001e70: 7c00 6a05 7c04 1900 5300 2904 7ab2 6164  |.j.|...S.).z.ad
-00001e80: 6420 7665 7274 6578 2062 7920 636f 6f72  d vertex by coor
-00001e90: 6469 6e61 7465 2061 6e64 2075 6e69 7120  dinate and uniq 
-00001ea0: 6e61 6d65 0a20 2020 2020 2020 2078 2079  name.        x y
-00001eb0: 207a 2069 7320 636f 6f72 6469 6e61 7465   z is coordinate
-00001ec0: 7320 6f66 2076 6572 7465 780a 2020 2020  s of vertex.    
-00001ed0: 2020 2020 6e61 6d65 2069 7320 756e 6971      name is uniq
-00001ee0: 206e 616d 6520 746f 2072 6566 6572 2074   name to refer t
-00001ef0: 6865 2076 6572 7465 780a 2020 2020 2020  he vertex.      
-00001f00: 2020 7265 7475 726e 7320 5665 7274 6578    returns Vertex
-00001f10: 206f 626a 6563 7420 7768 6963 6920 6973   object whici is
-00001f20: 2061 6464 6564 2e0a 2020 2020 2020 2020   added..        
-00001f30: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001f40: 0003 0000 0073 0000 0073 1800 0000 8100  .....s...s......
-00001f50: 7c00 5d07 7d01 7c01 6400 7501 5600 0100  |.].}.|.d.u.V...
-00001f60: 7102 6400 5300 720e 0000 0072 1600 0000  q.d.S.r....r....
-00001f70: 2902 7238 0000 00da 0361 7267 7216 0000  ).r8.....argr...
-00001f80: 0072 1600 0000 7217 0000 0072 3c00 0000  .r....r....r<...
-00001f90: f400 0000 7304 0000 0002 8016 007a 2b42  ....s........z+B
-00001fa0: 6c6f 636b 4d65 7368 4469 6374 2e61 6464  lockMeshDict.add
-00001fb0: 5f76 6572 7465 782e 3c6c 6f63 616c 733e  _vertex.<locals>
-00001fc0: 2e3c 6765 6e65 7870 723e 7a40 7820 6973  .<genexpr>z@x is
-00001fd0: 2061 2056 6572 7465 7820 616e 6420 6061   a Vertex and `a
-00001fe0: 6e79 2861 7267 2069 7320 6e6f 7420 4e6f  ny(arg is not No
-00001ff0: 6e65 2066 6f72 2061 7267 2069 6e20 2879  ne for arg in (y
-00002000: 2c20 7a2c 206e 616d 6529 2960 2906 725b  , z, name))`).r[
-00002010: 0000 0072 0d00 0000 da03 616e 79da 0a56  ...r......any..V
-00002020: 616c 7565 4572 726f 7272 1200 0000 723b  alueErrorr....r;
-00002030: 0000 0029 0672 1500 0000 720f 0000 0072  ...).r....r....r
-00002040: 1000 0000 7211 0000 0072 1200 0000 5a06  ....r....r....Z.
-00002050: 7665 7274 6578 7216 0000 0072 1600 0000  vertexr....r....
-00002060: 7217 0000 00da 0a61 6464 5f76 6572 7465  r......add_verte
-00002070: 78ed 0000 0073 1400 0000 0a06 1801 0201  x....s..........
-00002080: 0201 04ff 0404 0801 0e02 0a01 0a01 7a18  ..............z.
-00002090: 426c 6f63 6b4d 6573 6844 6963 742e 6164  BlockMeshDict.ad
-000020a0: 645f 7665 7274 6578 6302 0000 0000 0000  d_vertexc.......
-000020b0: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-000020c0: 0073 0c00 0000 7c00 6a00 7c01 3d00 6401  .s....|.j.|.=.d.
-000020d0: 5300 2902 7a1f 6465 6c20 6e61 6d65 206b  S.).z.del name k
-000020e0: 6579 2066 726f 6d20 7365 6c66 2e76 6572  ey from self.ver
-000020f0: 7469 6365 734e 723a 0000 0029 0272 1500  ticesNr:...).r..
-00002100: 0000 7212 0000 0072 1600 0000 7216 0000  ..r....r....r...
-00002110: 0072 1700 0000 da0a 6465 6c5f 7665 7274  .r......del_vert
-00002120: 6578 0001 0000 7302 0000 000c 027a 1842  ex....s......z.B
-00002130: 6c6f 636b 4d65 7368 4469 6374 2e64 656c  lockMeshDict.del
-00002140: 5f76 6572 7465 7863 0200 0000 0000 0000  _vertexc........
-00002150: 0000 0000 0600 0000 0400 0000 4700 0000  ............G...
-00002160: 733a 0000 007c 006a 007c 0119 007d 037c  s:...|.j.|...}.|
-00002170: 0244 005d 137d 047c 006a 007c 0419 007d  .D.].}.|.j.|...}
-00002180: 057c 036a 01a0 027c 056a 01a1 0101 007c  .|.j...|.j.....|
-00002190: 037c 006a 007c 043c 0071 0764 0153 0029  .|.j.|.<.q.d.S.)
-000021a0: 027a e274 7265 6174 206e 616d 6531 2c20  .z.treat name1, 
-000021b0: 6e61 6d65 322c 202e 2e2e 2061 7320 7361  name2, ... as sa
-000021c0: 6d65 2070 6f69 6e74 2e0a 0a20 2020 2020  me point...     
-000021d0: 2020 206e 616d 6532 2e61 6c69 6173 2c20     name2.alias, 
-000021e0: 6e61 6d65 332e 616c 6961 732c 202e 2e2e  name3.alias, ...
-000021f0: 2061 7265 206d 6572 6765 6420 7769 7468   are merged with
-00002200: 206e 616d 6531 2e61 6c69 6173 0a20 2020   name1.alias.   
-00002210: 2020 2020 2074 6865 206b 6579 206e 616d       the key nam
-00002220: 6532 2c20 6e61 6d65 332c 202e 2e2e 2069  e2, name3, ... i
-00002230: 6e20 7365 6c66 2e76 6572 7469 6365 7320  n self.vertices 
-00002240: 6172 6520 6b65 7074 2061 6e64 206d 6170  are kept and map
-00002250: 7065 6420 746f 0a20 2020 2020 2020 2073  ped to.        s
-00002260: 616d 6520 5665 7274 6578 2069 6e73 7461  ame Vertex insta
-00002270: 6e63 6520 6173 206e 616d 6531 0a20 2020  nce as name1.   
-00002280: 2020 2020 204e 2903 723b 0000 0072 1300       N).r;...r..
-00002290: 0000 da06 7570 6461 7465 2906 7215 0000  ....update).r...
-000022a0: 00da 056e 616d 6531 da05 6e61 6d65 73da  ...name1..names.
-000022b0: 0176 724d 0000 0072 4700 0000 7216 0000  .vrM...rG...r...
-000022c0: 0072 1600 0000 7217 0000 00da 0d72 6564  .r....r......red
-000022d0: 7563 655f 7665 7274 6578 0401 0000 730c  uce_vertex....s.
-000022e0: 0000 000a 0708 010a 010e 010c 0204 fc7a  ...............z
-000022f0: 1b42 6c6f 636b 4d65 7368 4469 6374 2e72  .BlockMeshDict.r
-00002300: 6564 7563 655f 7665 7274 6578 6301 0000  educe_vertexc...
-00002310: 0000 0000 0000 0000 0007 0000 0005 0000  ................
-00002320: 0043 0000 0073 7800 0000 7400 7401 7c00  .C...sx...t.t.|.
-00002330: 6a02 a003 a100 8301 6401 6402 8400 6403  j.......d.d...d.
-00002340: 8d02 7d01 6700 7d02 7404 7c01 6404 6402  ..}.g.}.t.|.d.d.
-00002350: 8400 8302 4400 5d0b 5c02 7d03 7d04 7c02  ....D.].\.}.}.|.
-00002360: a005 7401 7c04 8301 a101 0100 7116 7c02  ..t.|.......q.|.
-00002370: 4400 5d15 7d05 7406 7c05 8301 6405 6b02  D.].}.t.|...d.k.
-00002380: 722d 7124 6406 6407 8400 7c05 4400 8301  r-q$d.d...|.D...
-00002390: 7d06 7c00 6a07 7c06 8e00 0100 7124 6408  }.|.j.|.....q$d.
-000023a0: 5300 2909 7a39 6361 6c6c 2072 6564 7563  S.).z9call reduc
-000023b0: 655f 7665 7274 6578 206f 6e20 616c 6c20  e_vertex on all 
-000023c0: 7665 7274 6963 6573 2077 6974 6820 6964  vertices with id
-000023d0: 656e 7469 6361 6c20 7661 6c75 6573 2e63  entical values.c
-000023e0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000023f0: 0300 0000 5300 0000 f30c 0000 0074 007c  ....S........t.|
-00002400: 0064 0119 0083 0153 00a9 024e 7206 0000  .d.....S...Nr...
-00002410: 00a9 0172 2700 0000 a901 7282 0000 0072  ...r'.....r....r
-00002420: 1600 0000 7216 0000 0072 1700 0000 da08  ....r....r......
-00002430: 3c6c 616d 6264 613e 1701 0000 f302 0000  <lambda>........
-00002440: 000c 007a 2e42 6c6f 636b 4d65 7368 4469  ...z.BlockMeshDi
-00002450: 6374 2e6d 6572 6765 5f76 6572 7469 6365  ct.merge_vertice
-00002460: 732e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  s.<locals>.<lamb
-00002470: 6461 3e29 01da 036b 6579 6301 0000 0000  da>)...keyc.....
-00002480: 0000 0000 0000 0001 0000 0003 0000 0053  ...............S
-00002490: 0000 0072 8400 0000 7285 0000 0072 8600  ...r....r....r..
-000024a0: 0000 7287 0000 0072 1600 0000 7216 0000  ..r....r....r...
-000024b0: 0072 1700 0000 7288 0000 001a 0100 0072  .r....r........r
-000024c0: 8900 0000 7206 0000 0063 0100 0000 0000  ....r....c......
-000024d0: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-000024e0: 0000 7314 0000 0067 007c 005d 067d 017c  ..s....g.|.].}.|
-000024f0: 0164 0019 0091 0271 0253 0029 0172 0100  .d.....q.S.).r..
-00002500: 0000 7216 0000 0029 0272 3800 0000 7282  ..r....).r8...r.
-00002510: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00002520: 0000 725a 0000 001f 0100 0073 0200 0000  ..rZ.......s....
-00002530: 1400 7a30 426c 6f63 6b4d 6573 6844 6963  ..z0BlockMeshDic
-00002540: 742e 6d65 7267 655f 7665 7274 6963 6573  t.merge_vertices
-00002550: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00002560: 6f6d 703e 4e29 0872 1e00 0000 da04 6c69  omp>N).r......li
-00002570: 7374 723b 0000 00da 0569 7465 6d73 7202  str;.....itemsr.
-00002580: 0000 0072 6200 0000 721c 0000 0072 8300  ...rb...r....r..
-00002590: 0000 2907 7215 0000 005a 0f73 6f72 7465  ..).r....Z.sorte
-000025a0: 645f 7665 7274 6963 6573 da06 6772 6f75  d_vertices..grou
-000025b0: 7073 da01 6bda 0167 da05 6772 6f75 7072  ps..k..g..groupr
-000025c0: 8100 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
-000025d0: 0000 00da 0e6d 6572 6765 5f76 6572 7469  .....merge_verti
-000025e0: 6365 7312 0100 0073 1800 0000 0204 1201  ces....s........
-000025f0: 06ff 0403 1601 1001 0801 0c01 0201 0e01  ................
-00002600: 0c01 04fc 7a1c 426c 6f63 6b4d 6573 6844  ....z.BlockMeshD
-00002610: 6963 742e 6d65 7267 655f 7665 7274 6963  ict.merge_vertic
-00002620: 6573 7206 0000 0063 0500 0000 0000 0000  esr....c........
-00002630: 0000 0000 0600 0000 0500 0000 4300 0000  ............C...
-00002640: 731c 0000 0074 007c 017c 027c 037c 0483  s....t.|.|.|.|..
-00002650: 047d 057c 057c 006a 017c 033c 007c 0553  .}.|.|.j.|.<.|.S
-00002660: 0072 0e00 0000 2902 7243 0000 0072 6a00  .r....).rC...rj.
-00002670: 0000 2906 7215 0000 0072 3200 0000 7244  ..).r....r2...rD
-00002680: 0000 0072 1200 0000 7245 0000 0072 5000  ...r....rE...rP.
-00002690: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-000026a0: 00da 0c61 6464 5f68 6578 626c 6f63 6b22  ...add_hexblock"
-000026b0: 0100 00f3 0600 0000 0e01 0a01 0401 7a1a  ..............z.
-000026c0: 426c 6f63 6b4d 6573 6844 6963 742e 6164  BlockMeshDict.ad
-000026d0: 645f 6865 7862 6c6f 636b 6304 0000 0000  d_hexblockc.....
-000026e0: 0000 0000 0000 0005 0000 0004 0000 0043  ...............C
-000026f0: 0000 00f3 1a00 0000 7400 7c01 7c02 7c03  ........t.|.|.|.
-00002700: 8303 7d04 7c04 7c00 6a01 7c02 3c00 7c04  ..}.|.|.j.|.<.|.
-00002710: 5300 720e 0000 0029 0272 0700 0000 726b  S.r....).r....rk
-00002720: 0000 0029 0572 1500 0000 7232 0000 0072  ...).r....r2...r
-00002730: 1200 0000 5a0c 696e 7465 725f 7665 7274  ....Z.inter_vert
-00002740: 6578 7249 0000 0072 1600 0000 7216 0000  exrI...r....r...
-00002750: 0072 1700 0000 da0b 6164 645f 6172 6365  .r......add_arce
-00002760: 6467 6527 0100 00f3 0600 0000 0c01 0a01  dge'............
-00002770: 0401 7a19 426c 6f63 6b4d 6573 6844 6963  ..z.BlockMeshDic
-00002780: 742e 6164 645f 6172 6365 6467 6563 0400  t.add_arcedgec..
-00002790: 0000 0000 0000 0000 0000 0500 0000 0400  ................
-000027a0: 0000 4300 0000 7294 0000 0072 0e00 0000  ..C...r....r....
-000027b0: 2902 7208 0000 0072 6b00 0000 2905 7215  ).r....rk...).r.
-000027c0: 0000 0072 3200 0000 7212 0000 00da 0670  ...r2...r......p
-000027d0: 6f69 6e74 7372 4900 0000 7216 0000 0072  ointsrI...r....r
-000027e0: 1600 0000 7217 0000 00da 0e61 6464 5f73  ....r......add_s
-000027f0: 706c 696e 6565 6467 652c 0100 0072 9600  plineedge,...r..
-00002800: 0000 7a1c 426c 6f63 6b4d 6573 6844 6963  ..z.BlockMeshDic
-00002810: 742e 6164 645f 7370 6c69 6e65 6564 6765  t.add_splineedge
-00002820: 6305 0000 0000 0000 0000 0000 0006 0000  c...............
-00002830: 0005 0000 0043 0000 0073 1c00 0000 7400  .....C...s....t.
-00002840: 7c01 7c02 7c03 7c04 8304 7d05 7c05 7c00  |.|.|.|...}.|.|.
-00002850: 6a01 7c02 3c00 7c05 5300 720e 0000 0029  j.|.<.|.S.r....)
-00002860: 0272 5e00 0000 726c 0000 0029 0672 1500  .r^...rl...).r..
-00002870: 0000 725f 0000 0072 1200 0000 7260 0000  ..r_...r....r`..
-00002880: 0072 6100 0000 7250 0000 0072 1600 0000  .ra...rP...r....
-00002890: 7216 0000 0072 1700 0000 da0c 6164 645f  r....r......add_
-000028a0: 626f 756e 6461 7279 3101 0000 7293 0000  boundary1...r...
-000028b0: 007a 1a42 6c6f 636b 4d65 7368 4469 6374  .z.BlockMeshDict
-000028c0: 2e61 6464 5f62 6f75 6e64 6172 7963 0500  .add_boundaryc..
-000028d0: 0000 0000 0000 0000 0000 0700 0000 0600  ................
-000028e0: 0000 4300 0000 732c 0000 007c 006a 0064  ..C...s,...|.j.d
-000028f0: 017c 017c 037c 0264 028d 047d 057c 006a  .|.|.|.d...}.|.j
-00002900: 0064 017c 027c 047c 0164 028d 047d 067c  .d.|.|.|.d...}.|
-00002910: 057c 0666 0253 0029 034e da06 6379 636c  .|.f.S.).N..cycl
-00002920: 6963 2901 7261 0000 0029 0172 9900 0000  ic).ra...).r....
-00002930: 2907 7215 0000 005a 056e 616d 6530 7280  ).r....Z.name0r.
-00002940: 0000 005a 0666 6163 6573 305a 0666 6163  ...Z.faces0Z.fac
-00002950: 6573 31da 0262 30da 0262 3172 1600 0000  es1..b0..b1r....
-00002960: 7216 0000 0072 1700 0000 da15 6164 645f  r....r......add_
-00002970: 6379 636c 6963 5f62 6f75 6e64 6172 6965  cyclic_boundarie
-00002980: 7336 0100 0073 0600 0000 1201 1201 0801  s6...s..........
-00002990: 7a23 426c 6f63 6b4d 6573 6844 6963 742e  z#BlockMeshDict.
-000029a0: 6164 645f 6379 636c 6963 5f62 6f75 6e64  add_cyclic_bound
-000029b0: 6172 6965 7354 6302 0000 0000 0000 0000  ariesTc.........
-000029c0: 0000 0007 0000 0005 0000 0043 0000 0073  ...........C...s
-000029d0: 8200 0000 7400 8300 7d02 6700 7c00 5f01  ....t...}.g.|._.
-000029e0: 7c00 6a02 a003 a100 4400 5d1e 7d03 7c03  |.j.....D.].}.|.
-000029f0: 6a04 4400 5d18 7d04 7c00 6a05 7c04 1900  j.D.].}.|.j.|...
-00002a00: 7d05 7c05 6a06 7c02 7601 7228 7c02 a007  }.|.j.|.v.r(|...
-00002a10: 7c05 6a06 a101 0100 7c00 6a01 a008 7c05  |.j.....|.j...|.
-00002a20: a101 0100 7110 710b 7c01 7232 7409 7c00  ....q.q.|.r2t.|.
-00002a30: 6a01 8301 7c00 5f01 740a 7c00 6a01 8301  j...|._.t.|.j...
-00002a40: 4400 5d07 5c02 7d06 7d05 7c06 7c05 5f0b  D.].\.}.}.|.|._.
-00002a50: 7137 6401 5300 2902 7ae3 312e 2063 7265  q7d.S.).z.1. cre
-00002a60: 6174 6520 6c69 7374 206f 6620 5665 7274  ate list of Vert
-00002a70: 6578 2077 6869 6368 2061 7265 2072 6566  ex which are ref
-00002a80: 6572 7265 6420 6279 2062 6c6f 636b 7320  erred by blocks 
-00002a90: 6f6e 6c79 2e0a 2020 2020 2020 2020 322e  only..        2.
-00002aa0: 2073 6f72 7420 7665 7274 6578 2061 6363   sort vertex acc
-00002ab0: 6f72 6469 6e67 2074 6f20 2878 2c20 792c  ording to (x, y,
-00002ac0: 207a 290a 2020 2020 2020 2020 332e 2061   z).        3. a
-00002ad0: 7373 6967 6e20 7365 7175 656e 6365 206e  ssign sequence n
-00002ae0: 756d 6265 7220 666f 7220 6561 6368 2056  umber for each V
-00002af0: 6572 7465 780a 2020 2020 2020 2020 342e  ertex.        4.
-00002b00: 2073 6f72 7465 6420 6c69 7374 2069 7320   sorted list is 
-00002b10: 7361 7665 6420 6173 2073 656c 662e 5f76  saved as self._v
-00002b20: 6572 7469 6365 735f 696e 5f62 6c6f 636b  ertices_in_block
-00002b30: 6d65 7368 0a20 2020 2020 2020 204e 290c  mesh.        N).
-00002b40: da03 7365 7472 6d00 0000 726a 0000 00da  ..setrm...rj....
-00002b50: 0676 616c 7565 7372 3200 0000 723b 0000  .valuesr2...r;..
-00002b60: 0072 1200 0000 da03 6164 6472 6200 0000  .r......addrb...
-00002b70: 721e 0000 00da 0965 6e75 6d65 7261 7465  r......enumerate
-00002b80: 7214 0000 0029 0772 1500 0000 da04 736f  r....).r......so
-00002b90: 7274 5a0b 766e 616d 6573 5f6b 6570 7472  rtZ.vnames_keptr
-00002ba0: 5000 0000 724d 0000 0072 8200 0000 7259  P...rM...r....rY
-00002bb0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00002bc0: 0000 da0f 6173 7369 676e 5f76 6572 7465  ....assign_verte
-00002bd0: 7869 643b 0100 0073 1e00 0000 0607 0601  xid;...s........
-00002be0: 0e01 0a01 0a01 0a01 0c01 0c01 0280 02fc  ................
-00002bf0: 0405 0c01 1201 0801 04ff 7a1d 426c 6f63  ..........z.Bloc
-00002c00: 6b4d 6573 6844 6963 742e 6173 7369 676e  kMeshDict.assign
-00002c10: 5f76 6572 7465 7869 6463 0100 0000 0000  _vertexidc......
-00002c20: 0000 0000 0000 0300 0000 0600 0000 4300  ..............C.
-00002c30: 0000 7338 0000 0064 0167 017d 017c 006a  ..s8...d.g.}.|.j
-00002c40: 0044 005d 0b7d 027c 01a0 0164 027c 02a0  .D.].}.|...d.|..
-00002c50: 02a1 0017 00a1 0101 0071 067c 01a0 0164  .........q.|...d
-00002c60: 03a1 0101 0064 04a0 037c 01a1 0153 0029  .....d...|...S.)
-00002c70: 057a ec66 6f72 6d61 7420 7665 7274 6963  .z.format vertic
-00002c80: 6573 2073 6563 7469 6f6e 2e0a 2020 2020  es section..    
-00002c90: 2020 2020 6173 7369 676e 5f76 6572 7465      assign_verte
-00002ca0: 7869 6428 2920 7368 6f75 6c64 2062 6520  xid() should be 
-00002cb0: 6361 6c6c 6564 2062 6566 6f72 6520 7468  called before th
-00002cc0: 6973 206d 6574 686f 642c 2062 6563 6175  is method, becau
-00002cd0: 7365 0a20 2020 2020 2020 2073 656c 662e  se.        self.
-00002ce0: 5f76 6572 7469 6365 735f 696e 5f62 6c6f  _vertices_in_blo
-00002cf0: 636b 6d65 7368 2073 686f 756c 6420 6265  ckmesh should be
-00002d00: 2061 7661 696c 6162 6c65 2061 6e64 0a20   available and. 
-00002d10: 2020 2020 2020 206d 656d 6265 7273 206f         members o
-00002d20: 6620 7365 6c66 2e5f 7665 7274 6963 6573  f self._vertices
-00002d30: 5f69 6e5f 626c 6f63 6b6d 6573 6820 7368  _in_blockmesh sh
-00002d40: 6f75 6c64 2068 6176 6520 7661 6c69 6420  ould have valid 
-00002d50: 696e 6465 782e 0a20 2020 2020 2020 207a  index..        z
-00002d60: 0a76 6572 7469 6365 730a 28fa 0420 2020  .vertices.(..   
-00002d70: 20fa 0229 3b72 6400 0000 2904 726d 0000   ..);rd...).rm..
-00002d80: 0072 6200 0000 7220 0000 0072 1d00 0000  .rb...r ...r....
-00002d90: 2903 7215 0000 0072 6500 0000 7282 0000  ).r....re...r...
-00002da0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00002db0: da17 666f 726d 6174 5f76 6572 7469 6365  ..format_vertice
-00002dc0: 735f 7365 6374 696f 6e4f 0100 0073 0a00  s_sectionO...s..
-00002dd0: 0000 0606 0a01 1401 0a01 0a01 7a25 426c  ............z%Bl
-00002de0: 6f63 6b4d 6573 6844 6963 742e 666f 726d  ockMeshDict.form
-00002df0: 6174 5f76 6572 7469 6365 735f 7365 6374  at_vertices_sect
-00002e00: 696f 6e63 0100 0000 0000 0000 0000 0000  ionc............
-00002e10: 0300 0000 0700 0000 4300 0000 f340 0000  ........C....@..
-00002e20: 0064 0167 017d 017c 006a 00a0 01a1 0044  .d.g.}.|.j.....D
-00002e30: 005d 0d7d 027c 01a0 0264 027c 02a0 037c  .].}.|...d.|...|
-00002e40: 006a 04a1 0117 00a1 0101 0071 087c 01a0  .j.........q.|..
-00002e50: 0264 03a1 0101 0064 04a0 057c 01a1 0153  .d.....d...|...S
-00002e60: 0029 057a a266 6f72 6d61 7420 626c 6f63  .).z.format bloc
-00002e70: 6b73 2073 6563 7469 6f6e 2e0a 2020 2020  ks section..    
-00002e80: 2020 2020 6173 7369 676e 5f76 6572 7465      assign_verte
-00002e90: 7869 6428 2920 7368 6f75 6c64 2062 6520  xid() should be 
-00002ea0: 6361 6c6c 6564 2062 6566 6f72 6520 7468  called before th
-00002eb0: 6973 206d 6574 686f 642c 2062 6563 6175  is method, becau
-00002ec0: 7365 0a20 2020 2020 2020 2076 6572 7469  se.        verti
-00002ed0: 6365 7320 7265 6665 7265 6420 6279 2062  ces refered by b
-00002ee0: 6c6f 636b 7320 7368 6f75 6c64 2068 6176  locks should hav
-00002ef0: 6520 7661 6c69 6420 696e 6465 782e 0a20  e valid index.. 
-00002f00: 2020 2020 2020 207a 0862 6c6f 636b 730a         z.blocks.
-00002f10: 2872 a400 0000 72a5 0000 0072 6400 0000  (r....r....rd...
-00002f20: 2906 726a 0000 0072 9f00 0000 7262 0000  ).rj...r....rb..
-00002f30: 0072 2000 0000 723b 0000 0072 1d00 0000  .r ...r;...r....
-00002f40: 2903 7215 0000 0072 6500 0000 7250 0000  ).r....re...rP..
-00002f50: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00002f60: da15 666f 726d 6174 5f62 6c6f 636b 735f  ..format_blocks_
-00002f70: 7365 6374 696f 6e5b 0100 0073 0a00 0000  section[...s....
-00002f80: 0605 0e01 1801 0a01 0a01 7a23 426c 6f63  ..........z#Bloc
-00002f90: 6b4d 6573 6844 6963 742e 666f 726d 6174  kMeshDict.format
-00002fa0: 5f62 6c6f 636b 735f 7365 6374 696f 6e63  _blocks_sectionc
-00002fb0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00002fc0: 0700 0000 4300 0000 72a7 0000 0029 057a  ....C...r....).z
-00002fd0: a166 6f72 6d61 7420 6564 6765 7320 7365  .format edges se
-00002fe0: 6374 696f 6e2e 0a20 2020 2020 2020 2061  ction..        a
-00002ff0: 7373 6967 6e5f 7665 7274 6578 6964 2829  ssign_vertexid()
-00003000: 2073 686f 756c 6420 6265 2063 616c 6c65   should be calle
-00003010: 6420 6265 666f 7265 2074 6869 7320 6d65  d before this me
-00003020: 7468 6f64 2c20 6265 6361 7573 650a 2020  thod, because.  
-00003030: 2020 2020 2020 7665 7274 6963 6573 2072        vertices r
-00003040: 6566 6572 6564 2062 7920 626c 6f63 6b73  efered by blocks
-00003050: 2073 686f 756c 6420 6861 7665 2076 616c   should have val
-00003060: 6964 2069 6e64 6578 2e0a 2020 2020 2020  id index..      
-00003070: 2020 7a07 6564 6765 730a 2872 a400 0000    z.edges.(r....
-00003080: 72a5 0000 0072 6400 0000 2906 726b 0000  r....rd...).rk..
-00003090: 0072 9f00 0000 7262 0000 0072 2000 0000  .r....rb...r ...
-000030a0: 723b 0000 0072 1d00 0000 2903 7215 0000  r;...r....).r...
-000030b0: 0072 6500 0000 7249 0000 0072 1600 0000  .re...rI...r....
-000030c0: 7216 0000 0072 1700 0000 da14 666f 726d  r....r......form
-000030d0: 6174 5f65 6467 6573 5f73 6563 7469 6f6e  at_edges_section
-000030e0: 6601 0000 730a 0000 0006 060e 0118 010a  f...s...........
-000030f0: 010a 017a 2242 6c6f 636b 4d65 7368 4469  ...z"BlockMeshDi
-00003100: 6374 2e66 6f72 6d61 745f 6564 6765 735f  ct.format_edges_
-00003110: 7365 6374 696f 6e63 0100 0000 0000 0000  sectionc........
-00003120: 0000 0000 0500 0000 0600 0000 4300 0000  ............C...
-00003130: 7354 0000 0064 0167 017d 017c 006a 00a0  sT...d.g.}.|.j..
-00003140: 01a1 0044 005d 177d 0264 027d 037c 02a0  ...D.].}.d.}.|..
-00003150: 027c 006a 03a1 01a0 0464 0364 037c 0317  .|.j.....d.d.|..
-00003160: 00a1 027d 047c 01a0 057c 037c 0417 00a1  ...}.|...|.|....
-00003170: 0101 0071 087c 01a0 0564 04a1 0101 0064  ...q.|...d.....d
-00003180: 03a0 067c 01a1 0153 0029 057a a366 6f72  ...|...S.).z.for
-00003190: 6d61 7420 626f 756e 6461 7279 2073 6563  mat boundary sec
-000031a0: 7469 6f6e 2e0a 2020 2020 2020 2020 6173  tion..        as
-000031b0: 7369 676e 5f76 6572 7465 7869 6428 2920  sign_vertexid() 
-000031c0: 7368 6f75 6c64 2062 6520 6361 6c6c 6564  should be called
-000031d0: 2062 6566 6f72 6520 7468 6973 206d 6574   before this met
-000031e0: 686f 642c 2062 6563 6175 7365 0a20 2020  hod, because.   
-000031f0: 2020 2020 2076 6572 7469 6365 7320 7265       vertices re
-00003200: 6665 7265 6420 6279 2066 6163 6573 2073  fered by faces s
-00003210: 686f 756c 6420 6861 7665 2076 616c 6964  hould have valid
-00003220: 2069 6e64 6578 2e0a 2020 2020 2020 2020   index..        
-00003230: 7a0a 626f 756e 6461 7279 0a28 72a4 0000  z.boundary.(r...
-00003240: 0072 6400 0000 72a5 0000 0029 0772 6c00  .rd...r....).rl.
-00003250: 0000 729f 0000 0072 2000 0000 723b 0000  ..r....r ...r;..
-00003260: 00da 0772 6570 6c61 6365 7262 0000 0072  ...replacerb...r
-00003270: 1d00 0000 2905 7215 0000 0072 6500 0000  ....).r....re...
-00003280: 7250 0000 00da 0669 6e64 656e 7472 3f00  rP.....indentr?.
-00003290: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-000032a0: 00da 1766 6f72 6d61 745f 626f 756e 6461  ...format_bounda
-000032b0: 7279 5f73 6563 7469 6f6e 7201 0000 730e  ry_sectionr...s.
-000032c0: 0000 0006 060e 0104 0218 0110 010a 010a  ................
-000032d0: 017a 2542 6c6f 636b 4d65 7368 4469 6374  .z%BlockMeshDict
-000032e0: 2e66 6f72 6d61 745f 626f 756e 6461 7279  .format_boundary
-000032f0: 5f73 6563 7469 6f6e 6301 0000 0000 0000  _sectionc.......
-00003300: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00003310: 0073 0400 0000 6401 5300 2902 4e7a 146d  .s....d.S.).Nz.m
-00003320: 6572 6765 5061 7463 6850 6169 7273 0a28  ergePatchPairs.(
-00003330: 0a29 3b72 1600 0000 7228 0000 0072 1600  .);r....r(...r..
-00003340: 0000 7216 0000 0072 1700 0000 da1e 666f  ..r....r......fo
-00003350: 726d 6174 5f6d 6572 6765 7061 7463 6870  rmat_mergepatchp
-00003360: 6169 7273 5f73 6563 7469 6f6e 8101 0000  airs_section....
-00003370: 7302 0000 0004 017a 2c42 6c6f 636b 4d65  s......z,BlockMe
-00003380: 7368 4469 6374 2e66 6f72 6d61 745f 6d65  shDict.format_me
-00003390: 7267 6570 6174 6368 7061 6972 735f 7365  rgepatchpairs_se
-000033a0: 6374 696f 6e63 0300 0000 0000 0000 0000  ctionc..........
-000033b0: 0000 0400 0000 0900 0000 4300 0000 7346  ..........C...sF
-000033c0: 0000 007c 006a 007c 0264 018d 0101 0074  ...|.j.|.d.....t
-000033d0: 0164 0283 017d 037c 036a 027c 0174 037c  .d...}.|.j.|.t.|
-000033e0: 006a 0483 017c 00a0 05a1 007c 00a0 06a1  .j...|.....|....
-000033f0: 007c 00a0 07a1 007c 00a0 08a1 007c 00a0  .|.....|.....|..
-00003400: 09a1 0064 038d 0753 0029 044e 2901 72a2  ...d...S.).N).r.
-00003410: 0000 0061 6f01 0000 2468 6561 6465 720a  ...ao...$header.
-00003420: 466f 616d 4669 6c65 0a7b 0a20 2020 2076  FoamFile.{.    v
-00003430: 6572 7369 6f6e 2020 2020 2032 2e30 3b0a  ersion     2.0;.
-00003440: 2020 2020 666f 726d 6174 2020 2020 2020      format      
-00003450: 6173 6369 693b 0a20 2020 2063 6c61 7373  ascii;.    class
-00003460: 2020 2020 2020 2064 6963 7469 6f6e 6172         dictionar
-00003470: 793b 0a20 2020 206f 626a 6563 7420 2020  y;.    object   
-00003480: 2020 2062 6c6f 636b 4d65 7368 4469 6374     blockMeshDict
-00003490: 3b0a 7d0a 2f2f 202a 202a 202a 202a 202a  ;.}.// * * * * *
-000034a0: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
-000034b0: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
-000034c0: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
-000034d0: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
-000034e0: 202f 2f0a 0a73 6361 6c65 2020 2024 6d65   //..scale   $me
-000034f0: 7472 6963 636f 6e76 6572 743b 0a0a 2476  tricconvert;..$v
-00003500: 6572 7469 6365 730a 0a24 626c 6f63 6b73  ertices..$blocks
-00003510: 0a0a 2465 6467 6573 0a0a 2462 6f75 6e64  ..$edges..$bound
-00003520: 6172 790a 0a24 6d65 7267 6570 6174 6368  ary..$mergepatch
-00003530: 7061 6972 730a 0a2f 2f20 2a2a 2a2a 2a2a  pairs..// ******
-00003540: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00003550: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00003560: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00003570: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00003580: 2a2a 2a20 2f2f 0a29 07da 0668 6561 6465  *** //.)...heade
-00003590: 725a 0d6d 6574 7269 6363 6f6e 7665 7274  rZ.metricconvert
-000035a0: 723b 0000 0072 6b00 0000 726a 0000 00da  r;...rk...rj....
-000035b0: 0862 6f75 6e64 6172 795a 0f6d 6572 6765  .boundaryZ.merge
-000035c0: 7061 7463 6870 6169 7273 290a 72a3 0000  patchpairs).r...
-000035d0: 0072 0300 0000 da0a 7375 6273 7469 7475  .r......substitu
-000035e0: 7465 7236 0000 0072 6900 0000 72a6 0000  ter6...ri...r...
-000035f0: 0072 a900 0000 72a8 0000 0072 ac00 0000  .r....r....r....
-00003600: 72ad 0000 0029 0472 1500 0000 72ae 0000  r....).r....r...
-00003610: 005a 0d73 6f72 745f 766f 7274 6963 6573  .Z.sort_vortices
-00003620: da08 7465 6d70 6c61 7465 7216 0000 0072  ..templater....r
-00003630: 1600 0000 7217 0000 0072 2000 0000 8701  ....r....r .....
-00003640: 0000 731a 0000 000c 0102 0102 0104 ff04  ..s.............
-00003650: 1b02 0108 0106 0106 0106 0106 0106 0106  ................
-00003660: f97a 1442 6c6f 636b 4d65 7368 4469 6374  .z.BlockMeshDict
-00003670: 2e66 6f72 6d61 7429 034e 4e4e 7267 0000  .format).NNNrg..
-00003680: 0029 0154 2918 722a 0000 0072 2b00 0000  .).T).r*...r+...
-00003690: 722c 0000 0072 1800 0000 7277 0000 0072  r,...r....rw...r
-000036a0: 7900 0000 727d 0000 0072 7e00 0000 7283  y...r}...r~...r.
-000036b0: 0000 0072 9100 0000 720b 0000 0072 9200  ...r....r....r..
-000036c0: 0000 7295 0000 0072 9800 0000 7299 0000  ..r....r....r...
-000036d0: 0072 9d00 0000 72a3 0000 0072 a600 0000  .r....r....r....
-000036e0: 72a8 0000 0072 a900 0000 72ac 0000 0072  r....r....r....r
-000036f0: ad00 0000 7205 0000 0072 2000 0000 7216  ....r....r ...r.
-00003700: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00003710: 0000 7268 0000 00d3 0000 0073 2800 0000  ..rh.......s(...
-00003720: 0800 0801 0808 080e 0a03 0813 0804 080e  ................
-00003730: 1410 0805 0805 0a05 0805 0a05 0814 080c  ................
-00003740: 080b 080c 080f 1206 7268 0000 004e 2916  ........rh...N).
-00003750: da07 5f5f 646f 635f 5fda 0969 7465 7274  ..__doc__..itert
-00003760: 6f6f 6c73 7202 0000 00da 0673 7472 696e  oolsr......strin
-00003770: 6772 0300 0000 da00 7205 0000 0072 6b00  gr......r....rk.
-00003780: 0000 7207 0000 0072 0800 0000 7245 0000  ..r....r....rE..
-00003790: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
-000037a0: 720c 0000 00da 075f 5f61 6c6c 5f5f 720d  r......__all__r.
-000037b0: 0000 0072 2e00 0000 7231 0000 0072 4300  ...r....r1...rC.
-000037c0: 0000 725e 0000 0072 6800 0000 7216 0000  ..r^...rh...r...
-000037d0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-000037e0: da08 3c6d 6f64 756c 653e 0100 0000 731a  ..<module>....s.
-000037f0: 0000 0004 000c 0c0c 010c 0210 0118 0108  ................
-00003800: 020e 0a0e 1e0e 0a0e 110e 5412 28         ..........T.(
+000000e0: 6120 0100 0048 656c 7065 7220 746f 2063  a ...Helper to c
+000000f0: 7265 6174 6520 626c 6f63 6b4d 6573 6844  reate blockMeshD
+00000100: 6963 7420 6669 6c65 730a 0a54 616b 656e  ict files..Taken
+00000110: 2066 726f 6d20 6874 7470 733a 2f2f 6769   from https://gi
+00000120: 7468 7562 2e63 6f6d 2f74 616b 6161 6b69  thub.com/takaaki
+00000130: 616f 6b69 2f6f 6662 6c6f 636b 6d65 7368  aoki/ofblockmesh
+00000140: 6469 6374 6865 6c70 6572 2028 4769 7420  dicthelper (Git 
+00000150: 636f 6d6d 6974 0a35 3835 3839 6631 2920  commit.58589f1) 
+00000160: 616e 6420 6d6f 6469 6669 6564 2061 7320  and modified as 
+00000170: 666f 6c6c 6f77 3a0a 0a2d 2060 6070 7975  follow:..- ``pyu
+00000180: 7067 7261 6465 205f 5f69 6e69 745f 5f2e  pgrade __init__.
+00000190: 7079 202d 2d70 7933 392d 706c 7573 6060  py --py39-plus``
+000001a0: 0a2d 2074 6573 7465 6420 2831 3030 2520  .- tested (100% 
+000001b0: 636f 7665 7261 6765 2920 616e 6420 7265  coverage) and re
+000001c0: 7072 6f64 7563 6962 6c65 2028 7365 7473  producible (sets
+000001d0: 2073 6f72 7465 6429 0a2d 2072 6566 6163   sorted).- refac
+000001e0: 746f 720a 2d20 7375 7070 6f72 7420 666f  tor.- support fo
+000001f0: 7220 6379 636c 6963 2062 6f75 6e64 6172  r cyclic boundar
+00000200: 6965 730a 0ae9 0000 0000 2901 da07 6772  ies.......)...gr
+00000210: 6f75 7062 7929 01da 0854 656d 706c 6174  oupby)...Templat
+00000220: 65e9 0200 0000 2901 da0e 4445 4641 554c  e.....)...DEFAUL
+00000230: 545f 4845 4144 4552 e901 0000 0029 02da  T_HEADER.....)..
+00000240: 0741 7263 4564 6765 da0a 5370 6c69 6e65  .ArcEdge..Spline
+00000250: 4564 6765 2904 da0b 4564 6765 4772 6164  Edge)...EdgeGrad
+00000260: 696e 67da 0747 7261 6469 6e67 da0d 5369  ing..Grading..Si
+00000270: 6d70 6c65 4772 6164 696e 67da 1453 696d  mpleGrading..Sim
+00000280: 706c 6547 7261 6469 6e67 456c 656d 656e  pleGradingElemen
+00000290: 7429 0672 0a00 0000 720c 0000 0072 0b00  t).r....r....r..
+000002a0: 0000 7209 0000 0072 0700 0000 7208 0000  ..r....r....r...
+000002b0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000002c0: 0000 0300 0000 4000 0000 7336 0000 0065  ......@...s6...e
+000002d0: 005a 0164 005a 0264 0c64 0264 0384 015a  .Z.d.Z.d.d.d...Z
+000002e0: 0364 0464 0584 005a 0464 0664 0784 005a  .d.d...Z.d.d...Z
+000002f0: 0564 0864 0984 005a 0664 0a64 0b84 005a  .d.d...Z.d.d...Z
+00000300: 0764 0153 0029 0dda 0656 6572 7465 784e  .d.S.)...VertexN
+00000310: 6306 0000 0000 0000 0000 0000 0006 0000  c...............
+00000320: 0002 0000 0043 0000 0073 2a00 0000 7c01  .....C...s*...|.
+00000330: 7c00 5f00 7c02 7c00 5f01 7c03 7c00 5f02  |._.|.|._.|.|._.
+00000340: 7c04 7c00 5f03 7c04 6801 7c00 5f04 7c05  |.|._.|.h.|._.|.
+00000350: 7c00 5f05 6400 5300 a901 4e29 06da 0178  |._.d.S...N)...x
+00000360: da01 79da 017a da04 6e61 6d65 da05 616c  ..y..z..name..al
+00000370: 6961 73da 0569 6e64 6578 2906 da04 7365  ias..index)...se
+00000380: 6c66 720f 0000 0072 1000 0000 7211 0000  lfr....r....r...
+00000390: 0072 1200 0000 7214 0000 00a9 0072 1600  .r....r......r..
+000003a0: 0000 fa55 2f68 6f6d 652f 7069 6572 7265  ...U/home/pierre
+000003b0: 2f44 6576 2f66 6c75 6964 7369 6d66 6f61  /Dev/fluidsimfoa
+000003c0: 6d2f 7372 632f 666c 7569 6473 696d 666f  m/src/fluidsimfo
+000003d0: 616d 2f66 6f61 6d5f 696e 7075 745f 6669  am/foam_input_fi
+000003e0: 6c65 732f 626c 6f63 6b6d 6573 682f 5f5f  les/blockmesh/__
+000003f0: 696e 6974 5f5f 2e70 79da 085f 5f69 6e69  init__.py..__ini
+00000400: 745f 5f1f 0000 0073 0c00 0000 0601 0601  t__....s........
+00000410: 0601 0601 0801 0a04 7a0f 5665 7274 6578  ........z.Vertex
+00000420: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
+00000430: 0000 0000 0000 0200 0000 0800 0000 4300  ..............C.
+00000440: 0000 7360 0000 007c 006a 009b 0064 017c  ..s`...|.j...d.|
+00000450: 006a 019b 009d 037d 0174 027c 006a 0383  .j.....}.t.|.j..
+00000460: 0164 026b 0472 1c7c 0164 0364 01a0 0474  .d.k.r.|.d.d...t
+00000470: 057c 006a 0383 01a1 0117 0037 007d 0164  .|.j.......7.}.d
+00000480: 047c 006a 0664 059b 0464 017c 006a 0764  .|.j.d...d.|.j.d
+00000490: 059b 0464 017c 006a 0864 059b 0464 067c  ...d.|.j.d...d.|
+000004a0: 019b 009d 0853 0029 074e da01 2072 0600  .....S.).N.. r..
+000004b0: 0000 7a03 203a 20fa 0228 20fa 0631 382e  ..z. : ..( ..18.
+000004c0: 3135 677a 0720 2920 202f 2f20 2909 7214  15gz. )  // ).r.
+000004d0: 0000 0072 1200 0000 da03 6c65 6e72 1300  ...r......lenr..
+000004e0: 0000 da04 6a6f 696e da06 736f 7274 6564  ....join..sorted
+000004f0: 720f 0000 0072 1000 0000 7211 0000 0029  r....r....r....)
+00000500: 0272 1500 0000 da07 636f 6d6d 656e 7472  .r......commentr
+00000510: 1600 0000 7216 0000 0072 1700 0000 da06  ....r....r......
+00000520: 666f 726d 6174 2a00 0000 730a 0000 0012  format*...s.....
+00000530: 010e 0118 0126 0202 ff7a 0d56 6572 7465  .....&...z.Verte
+00000540: 782e 666f 726d 6174 6302 0000 0000 0000  x.formatc.......
+00000550: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+00000560: 0073 2000 0000 7c00 6a00 7c00 6a01 7c00  .s ...|.j.|.j.|.
+00000570: 6a02 6603 7c01 6a00 7c01 6a01 7c01 6a02  j.f.|.j.|.j.|.j.
+00000580: 6603 6b00 5300 720e 0000 00a9 0372 1100  f.k.S.r......r..
+00000590: 0000 7210 0000 0072 0f00 0000 a902 7215  ..r....r......r.
+000005a0: 0000 00da 0372 6873 7216 0000 0072 1600  .....rhsr....r..
+000005b0: 0000 7217 0000 00da 065f 5f6c 745f 5f32  ..r......__lt__2
+000005c0: 0000 00f3 0200 0000 2001 7a0d 5665 7274  ........ .z.Vert
+000005d0: 6578 2e5f 5f6c 745f 5f63 0200 0000 0000  ex.__lt__c......
+000005e0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
+000005f0: 0000 7320 0000 007c 006a 007c 006a 017c  ..s ...|.j.|.j.|
+00000600: 006a 0266 037c 016a 007c 016a 017c 016a  .j.f.|.j.|.j.|.j
+00000610: 0266 036b 0253 0072 0e00 0000 7221 0000  .f.k.S.r....r!..
+00000620: 0072 2200 0000 7216 0000 0072 1600 0000  .r"...r....r....
+00000630: 7217 0000 00da 065f 5f65 715f 5f35 0000  r......__eq__5..
+00000640: 0072 2500 0000 7a0d 5665 7274 6578 2e5f  .r%...z.Vertex._
+00000650: 5f65 715f 5f63 0100 0000 0000 0000 0000  _eq__c..........
+00000660: 0000 0100 0000 0400 0000 4300 0000 7314  ..........C...s.
+00000670: 0000 0074 007c 006a 017c 006a 027c 006a  ...t.|.j.|.j.|.j
+00000680: 0366 0383 0153 0072 0e00 0000 2904 da04  .f...S.r....)...
+00000690: 6861 7368 7211 0000 0072 1000 0000 720f  hashr....r....r.
+000006a0: 0000 00a9 0172 1500 0000 7216 0000 0072  .....r....r....r
+000006b0: 1600 0000 7217 0000 00da 085f 5f68 6173  ....r......__has
+000006c0: 685f 5f38 0000 0073 0200 0000 1401 7a0f  h__8...s......z.
+000006d0: 5665 7274 6578 2e5f 5f68 6173 685f 5f72  Vertex.__hash__r
+000006e0: 0e00 0000 2908 da08 5f5f 6e61 6d65 5f5f  ....)...__name__
+000006f0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000700: 7175 616c 6e61 6d65 5f5f 7218 0000 0072  qualname__r....r
+00000710: 2000 0000 7224 0000 0072 2600 0000 7229   ...r$...r&...r)
+00000720: 0000 0072 1600 0000 7216 0000 0072 1600  ...r....r....r..
+00000730: 0000 7217 0000 0072 0d00 0000 1e00 0000  ..r....r........
+00000740: 730c 0000 0008 000a 0108 0b08 0808 030c  s...............
+00000750: 0372 0d00 0000 6300 0000 0000 0000 0000  .r....c.........
+00000760: 0000 0000 0000 0002 0000 0040 0000 00f3  ...........@....
+00000770: 1c00 0000 6500 5a01 6400 5a02 6401 6402  ....e.Z.d.Z.d.d.
+00000780: 8400 5a03 6403 6404 8400 5a04 6405 5300  ..Z.d.d...Z.d.S.
+00000790: 2906 da05 506f 696e 7463 0400 0000 0000  )...Pointc......
+000007a0: 0000 0000 0000 0400 0000 0200 0000 4300  ..............C.
+000007b0: 0000 7316 0000 007c 017c 005f 007c 027c  ..s....|.|._.|.|
+000007c0: 005f 017c 037c 005f 0264 0053 0072 0e00  ._.|.|._.d.S.r..
+000007d0: 0000 a903 720f 0000 0072 1000 0000 7211  ....r....r....r.
+000007e0: 0000 0029 0472 1500 0000 720f 0000 0072  ...).r....r....r
+000007f0: 1000 0000 7211 0000 0072 1600 0000 7216  ....r....r....r.
+00000800: 0000 0072 1700 0000 7218 0000 003d 0000  ...r....r....=..
+00000810: 0073 0600 0000 0601 0601 0a01 7a0e 506f  .s..........z.Po
+00000820: 696e 742e 5f5f 696e 6974 5f5f 6301 0000  int.__init__c...
+00000830: 0000 0000 0000 0000 0001 0000 0007 0000  ................
+00000840: 0043 0000 0073 2400 0000 6401 7c00 6a00  .C...s$...d.|.j.
+00000850: 6402 9b04 6403 7c00 6a01 6402 9b04 6403  d...d.|.j.d...d.
+00000860: 7c00 6a02 6402 9b04 6404 9d07 5300 2905  |.j.d...d...S.).
+00000870: 4e72 1a00 0000 721b 0000 0072 1900 0000  Nr....r....r....
+00000880: 7a02 2029 722f 0000 0072 2800 0000 7216  z. )r/...r(...r.
+00000890: 0000 0072 1600 0000 7217 0000 0072 2000  ...r....r....r .
+000008a0: 0000 4200 0000 7302 0000 0024 017a 0c50  ..B...s....$.z.P
+000008b0: 6f69 6e74 2e66 6f72 6d61 744e a905 722a  oint.formatN..r*
+000008c0: 0000 0072 2b00 0000 722c 0000 0072 1800  ...r+...r,...r..
+000008d0: 0000 7220 0000 0072 1600 0000 7216 0000  ..r ...r....r...
+000008e0: 0072 1600 0000 7217 0000 0072 2e00 0000  .r....r....r....
+000008f0: 3c00 0000 7306 0000 0008 0008 010c 0572  <...s..........r
+00000900: 2e00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000910: 0000 0000 0002 0000 0040 0000 0072 2d00  .........@...r-.
+00000920: 0000 2906 da04 4661 6365 6303 0000 0000  ..)...Facec.....
+00000930: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
+00000940: 0000 0073 1000 0000 7c01 7c00 5f00 7c02  ...s....|.|._.|.
+00000950: 7c00 5f01 6401 5300 2902 7a38 0a20 2020  |._.d.S.).z8.   
+00000960: 2020 2020 2076 6e61 6d65 2069 7320 6c69       vname is li
+00000970: 7374 206f 7220 7475 706c 6520 6f66 2076  st or tuple of v
+00000980: 6572 7465 7820 6e61 6d65 730a 2020 2020  ertex names.    
+00000990: 2020 2020 4e29 02da 0676 6e61 6d65 7372      N)...vnamesr
+000009a0: 1200 0000 2903 7215 0000 0072 3200 0000  ....).r....r2...
+000009b0: 7212 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
+000009c0: 1700 0000 7218 0000 0047 0000 0073 0400  ....r....G...s..
+000009d0: 0000 0604 0a01 7a0d 4661 6365 2e5f 5f69  ......z.Face.__i
+000009e0: 6e69 745f 5f63 0200 0000 0000 0000 0000  nit__c..........
+000009f0: 0000 0400 0000 0700 0000 0300 0000 7346  ..............sF
+00000a00: 0000 0064 01a0 0087 0066 0164 0264 0384  ...d.....f.d.d..
+00000a10: 087c 006a 0144 0083 01a1 017d 0264 01a0  .|.j.D.....}.d..
+00000a20: 007c 006a 01a1 017d 0364 047c 0264 059b  .|.j...}.d.|.d..
+00000a30: 0464 067c 006a 0264 059b 0464 077c 0364  .d.|.j.d...d.|.d
+00000a40: 059b 0464 089d 0753 0029 09fa 4b46 6f72  ...d...S.)..KFor
+00000a50: 6d61 7420 696e 7374 616e 6365 2074 6f20  mat instance to 
+00000a60: 6475 6d70 0a20 2020 2020 2020 2076 6572  dump.        ver
+00000a70: 7469 6365 7320 6973 2064 6963 7420 6f66  tices is dict of
+00000a80: 206e 616d 6520 746f 2056 6572 7465 780a   name to Vertex.
+00000a90: 2020 2020 2020 2020 7219 0000 0063 0100          r....c..
+00000aa0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00000ab0: 0000 3300 0000 f31e 0000 0081 007c 005d  ..3..........|.]
+00000ac0: 0a7d 0174 0088 007c 0119 006a 0183 0156  .}.t...|...j...V
+00000ad0: 0001 0071 0264 0053 0072 0e00 0000 a902  ...q.d.S.r......
+00000ae0: da03 7374 7272 1400 0000 a902 da02 2e30  ..strr.........0
+00000af0: da02 766e a901 da08 7665 7274 6963 6573  ..vn....vertices
+00000b00: 7216 0000 0072 1700 0000 da09 3c67 656e  r....r......<gen
+00000b10: 6578 7072 3e52 0000 00f3 0400 0000 0280  expr>R..........
+00000b20: 1c00 7a1e 4661 6365 2e66 6f72 6d61 742e  ..z.Face.format.
+00000b30: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
+00000b40: 723e fa01 28da 0173 7a06 2920 202f 2f20  r>..(..sz.)  // 
+00000b50: fa02 2028 fa01 2929 0372 1d00 0000 7232  .. (..)).r....r2
+00000b60: 0000 0072 1200 0000 a904 7215 0000 0072  ...r......r....r
+00000b70: 3b00 0000 7214 0000 0072 1f00 0000 7216  ;...r....r....r.
+00000b80: 0000 0072 3a00 0000 7217 0000 0072 2000  ...r:...r....r .
+00000b90: 0000 4e00 0000 7306 0000 001a 040c 0120  ..N...s........ 
+00000ba0: 017a 0b46 6163 652e 666f 726d 6174 4e72  .z.Face.formatNr
+00000bb0: 3000 0000 7216 0000 0072 1600 0000 7216  0...r....r....r.
+00000bc0: 0000 0072 1700 0000 7231 0000 0046 0000  ...r....r1...F..
+00000bd0: 0073 0600 0000 0800 0801 0c07 7231 0000  .s..........r1..
+00000be0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000bf0: 0000 0400 0000 4000 0000 7332 0000 0065  ......@...s2...e
+00000c00: 005a 0164 005a 0265 0364 0164 0164 0183  .Z.d.Z.e.d.d.d..
+00000c10: 0366 0164 0264 0384 015a 0464 0464 0584  .f.d.d...Z.d.d..
+00000c20: 005a 0564 0964 0764 0884 015a 0664 0653  .Z.d.d.d...Z.d.S
+00000c30: 0029 0ada 0848 6578 426c 6f63 6b72 0600  .)...HexBlockr..
+00000c40: 0000 6305 0000 0000 0000 0000 0000 0005  ..c.............
+00000c50: 0000 0002 0000 0043 0000 0073 1c00 0000  .......C...s....
+00000c60: 7c01 7c00 5f00 7c02 7c00 5f01 7c03 7c00  |.|._.|.|._.|.|.
+00000c70: 5f02 7c04 7c00 5f03 6401 5300 2902 612e  _.|.|._.d.S.).a.
+00000c80: 0100 0049 6e69 7469 616c 697a 6520 4865  ...Initialize He
+00000c90: 7842 6c6f 636b 2069 6e73 7461 6e63 650a  xBlock instance.
+00000ca0: 2020 2020 2020 2020 766e 616d 6573 2069          vnames i
+00000cb0: 7320 7468 6520 7665 7274 6578 206e 616d  s the vertex nam
+00000cc0: 6573 2069 6e20 6f72 6465 7220 6465 7363  es in order desc
+00000cd0: 7269 7665 6420 696e 0a20 2020 2020 2020  rived in.       
+00000ce0: 2020 2020 2068 7474 703a 2f2f 7777 772e       http://www.
+00000cf0: 6f70 656e 666f 616d 2e6f 7267 2f64 6f63  openfoam.org/doc
+00000d00: 732f 7573 6572 2f6d 6573 682d 6465 7363  s/user/mesh-desc
+00000d10: 7269 7074 696f 6e2e 7068 700a 2020 2020  ription.php.    
+00000d20: 2020 2020 6365 6c6c 7320 6973 206e 756d      cells is num
+00000d30: 6265 7220 6f66 2063 656c 6c73 2064 6576  ber of cells dev
+00000d40: 6965 6420 696e 746f 2069 6e20 6561 6368  ied into in each
+00000d50: 2064 6972 6563 7469 6f6e 0a20 2020 2020   direction.     
+00000d60: 2020 206e 616d 6520 6973 2074 6865 2075     name is the u
+00000d70: 6e69 7120 6e61 6d65 206f 6620 7468 6520  niq name of the 
+00000d80: 626c 6f63 6b0a 2020 2020 2020 2020 6772  block.        gr
+00000d90: 6164 696e 6720 6973 2067 7261 6469 6e67  ading is grading
+00000da0: 206d 6574 686f 642e 0a20 2020 2020 2020   method..       
+00000db0: 204e 2904 7232 0000 00da 0563 656c 6c73   N).r2.....cells
+00000dc0: 7212 0000 00da 0767 7261 6469 6e67 2905  r......grading).
+00000dd0: 7215 0000 0072 3200 0000 7244 0000 0072  r....r2...rD...r
+00000de0: 1200 0000 7245 0000 0072 1600 0000 7216  ....rE...r....r.
+00000df0: 0000 0072 1700 0000 7218 0000 0058 0000  ...r....r....X..
+00000e00: 0073 0800 0000 0608 0601 0601 0a01 7a11  .s............z.
+00000e10: 4865 7842 6c6f 636b 2e5f 5f69 6e69 745f  HexBlock.__init_
+00000e20: 5f63 0200 0000 0000 0000 0000 0000 0400  _c..............
+00000e30: 0000 1100 0000 0300 0000 737e 0000 0064  ..........s~...d
+00000e40: 01a0 0087 0066 0164 0264 0384 087c 006a  .....f.d.d...|.j
+00000e50: 0144 0083 01a1 017d 0264 01a0 007c 006a  .D.....}.d...|.j
+00000e60: 01a1 017d 0364 047c 029b 0064 057c 006a  ...}.d.|...d.|.j
+00000e70: 029b 0064 067c 006a 0364 0719 0064 089b  ...d.|.j.d...d..
+00000e80: 0464 017c 006a 0364 0919 0064 089b 0464  .d.|.j.d...d...d
+00000e90: 017c 006a 0364 0a19 0064 089b 0464 057c  .|.j.d...d...d.|
+00000ea0: 006a 04a0 05a1 009b 0064 0b7c 006a 029b  .j.......d.|.j..
+00000eb0: 0064 067c 039b 0064 0c9d 1153 0029 0d72  .d.|...d...S.).r
+00000ec0: 3300 0000 7219 0000 0063 0100 0000 0000  3...r....c......
+00000ed0: 0000 0000 0000 0200 0000 0400 0000 3300  ..............3.
+00000ee0: 0000 7234 0000 0072 0e00 0000 7235 0000  ..r4...r....r5..
+00000ef0: 0072 3700 0000 723a 0000 0072 1600 0000  .r7...r:...r....
+00000f00: 7217 0000 0072 3c00 0000 6900 0000 723d  r....r<...i...r=
+00000f10: 0000 007a 2248 6578 426c 6f63 6b2e 666f  ...z"HexBlock.fo
+00000f20: 726d 6174 2e3c 6c6f 6361 6c73 3e2e 3c67  rmat.<locals>.<g
+00000f30: 656e 6578 7072 3e7a 0568 6578 2028 7a02  enexpr>z.hex (z.
+00000f40: 2920 7240 0000 0072 0100 0000 da01 6472  ) r@...r......dr
+00000f50: 0600 0000 7204 0000 007a 0520 202f 2f20  ....r....z.  // 
+00000f60: 7241 0000 0029 0672 1d00 0000 7232 0000  rA...).r....r2..
+00000f70: 0072 1200 0000 7244 0000 0072 4500 0000  .r....rD...rE...
+00000f80: 7220 0000 0072 4200 0000 7216 0000 0072  r ...rB...r....r
+00000f90: 3a00 0000 7217 0000 0072 2000 0000 6500  :...r....r ...e.
+00000fa0: 0000 7320 0000 001a 040c 0110 020a 0104  ..s ............
+00000fb0: ff0a 0104 ff0a 0104 ff08 0204 fe04 0204  ................
+00000fc0: fe02 0206 fe02 ff7a 0f48 6578 426c 6f63  .......z.HexBloc
+00000fd0: 6b2e 666f 726d 6174 4e63 0300 0000 0000  k.formatNc......
+00000fe0: 0000 0000 0000 0700 0000 0500 0000 0300  ................
+00000ff0: 0000 73d4 0000 0069 0064 0164 0293 0164  ..s....i.d.d...d
+00001000: 0364 0293 0164 0464 0293 0164 0564 0693  .d...d.d...d.d..
+00001010: 0164 0764 0693 0164 0864 0693 0164 0964  .d.d...d.d...d.d
+00001020: 0a93 0164 0b64 0a93 0164 0c64 0a93 0164  ...d.d...d.d...d
+00001030: 0d64 0e93 0164 0f64 0e93 0164 1064 0e93  .d...d.d...d.d..
+00001040: 0164 1164 1293 0164 1364 1293 0164 1464  .d.d...d.d...d.d
+00001050: 1293 0164 1564 1293 0164 1664 1793 0164  ...d.d...d.d...d
+00001060: 1764 1764 1764 189c 03a5 017d 0367 0064  .d.d.d.....}.g.d
+00001070: 19a2 017d 0467 0064 1aa2 017d 0574 007c  ...}.g.d...}.t.|
+00001080: 0174 0183 0272 4c7c 037c 0119 007d 0174  .t...rL|.|...}.t
+00001090: 0287 0066 0164 1b64 1c84 087c 047c 0119  ...f.d.d...|.|..
+000010a0: 0044 0083 0183 017d 067c 0264 1d75 0072  .D.....}.|.d.u.r
+000010b0: 657c 057c 0119 00a0 0388 006a 04a1 017d  e|.|.......j...}
+000010c0: 0274 057c 067c 0283 0253 0029 1e61 0c02  .t.|.|...S.).a..
+000010d0: 0000 4765 6e65 7261 7465 2046 6163 6520  ..Generate Face 
+000010e0: 6f62 6a65 6374 0a20 2020 2020 2020 2069  object.        i
+000010f0: 6e64 6578 2069 7320 6e75 6d62 6572 206f  ndex is number o
+00001100: 7220 6b65 7977 6f72 6420 746f 2069 6465  r keyword to ide
+00001110: 6e74 6966 7920 7468 6520 6661 6365 206f  ntify the face o
+00001120: 6620 4865 780a 2020 2020 2020 2020 2020  f Hex.          
+00001130: 2020 3020 3d20 2777 2720 3d20 2778 6d27    0 = 'w' = 'xm'
+00001140: 203d 2027 2d31 3030 2720 3d20 2830 2034   = '-100' = (0 4
+00001150: 2037 2033 290a 2020 2020 2020 2020 2020   7 3).          
+00001160: 2020 3120 3d20 2765 2720 3d20 2778 7027    1 = 'e' = 'xp'
+00001170: 203d 2027 3130 3027 203d 2028 3120 3220   = '100' = (1 2 
+00001180: 3520 3629 0a20 2020 2020 2020 2020 2020  5 6).           
+00001190: 2032 203d 2027 7327 203d 2027 796d 2720   2 = 's' = 'ym' 
+000011a0: 3d20 2730 2d31 3027 203d 2028 3020 3120  = '0-10' = (0 1 
+000011b0: 3520 3429 0a20 2020 2020 2020 2020 2020  5 4).           
+000011c0: 2033 203d 2027 6e27 203d 2027 7970 2720   3 = 'n' = 'yp' 
+000011d0: 3d20 2730 3130 2720 3d20 2832 2033 2037  = '010' = (2 3 7
+000011e0: 2036 290a 2020 2020 2020 2020 2020 2020   6).            
+000011f0: 3420 3d20 2762 2720 3d20 277a 6d27 203d  4 = 'b' = 'zm' =
+00001200: 2027 3030 2d31 2720 3d20 2830 2033 2032   '00-1' = (0 3 2
+00001210: 2031 2920 3d20 2262 6f74 746f 6d22 0a20   1) = "bottom". 
+00001220: 2020 2020 2020 2020 2020 2035 203d 2027             5 = '
+00001230: 7427 203d 2027 7a70 2720 3d20 2730 3031  t' = 'zp' = '001
+00001240: 2720 3d20 2834 2035 2036 2037 2920 3d20  ' = (4 5 6 7) = 
+00001250: 2274 6f70 220a 2020 2020 2020 2020 6e61  "top".        na
+00001260: 6d65 2069 7320 6769 7665 6e20 746f 2046  me is given to F
+00001270: 6163 6520 696e 7374 616e 6365 2e20 4966  ace instance. If
+00001280: 206f 6d69 7474 6564 2c20 6e61 6d65 2069   omitted, name i
+00001290: 7320 6175 746f 6d61 7469 6361 6c6c 790a  s automatically.
+000012a0: 2020 2020 2020 2020 2020 2020 6765 6e61              gena
+000012b0: 7261 7469 6564 206c 696b 6520 2827 662d  ratied like ('f-
+000012c0: 2720 2b20 7365 6c66 2e6e 616d 6520 2b20  ' + self.name + 
+000012d0: 272d 7727 290a 2020 2020 2020 2020 da01  '-w').        ..
+000012e0: 7772 0100 0000 da02 786d 7a04 2d31 3030  wr......xmz.-100
+000012f0: da01 6572 0600 0000 da02 7870 da03 3130  ..er......xp..10
+00001300: 3072 3f00 0000 7204 0000 00da 0279 6d7a  0r?...r......ymz
+00001310: 0430 2d31 30da 016e e903 0000 00da 0279  .0-10..n.......y
+00001320: 705a 0330 3130 da01 62e9 0400 0000 da06  pZ.010..b.......
+00001330: 626f 7474 6f6d da02 7a6d 7a04 3030 2d31  bottom..zmz.00-1
+00001340: da01 74e9 0500 0000 2903 da03 746f 70da  ..t.....)...top.
+00001350: 027a 705a 0330 3031 2906 2904 7201 0000  .zpZ.001).).r...
+00001360: 0072 5100 0000 e907 0000 0072 4e00 0000  .rQ........rN...
+00001370: 2904 7206 0000 0072 0400 0000 e906 0000  ).r....r........
+00001380: 0072 5500 0000 2904 7201 0000 0072 0600  .rU...).r....r..
+00001390: 0000 7255 0000 0072 5100 0000 2904 7204  ..rU...rQ...).r.
+000013a0: 0000 0072 4e00 0000 7258 0000 0072 5900  ...rN...rX...rY.
+000013b0: 0000 2904 7201 0000 0072 4e00 0000 7204  ..).r....rN...r.
+000013c0: 0000 0072 0600 0000 2904 7251 0000 0072  ...r....).rQ...r
+000013d0: 5500 0000 7259 0000 0072 5800 0000 2906  U...rY...rX...).
+000013e0: 7a06 662d 7b7d 2d77 fa06 662d 7b7d 2d6e  z.f-{}-w..f-{}-n
+000013f0: 7a06 662d 7b7d 2d73 725a 0000 007a 0666  z.f-{}-srZ...z.f
+00001400: 2d7b 7d2d 627a 0666 2d7b 7d2d 7463 0100  -{}-bz.f-{}-tc..
+00001410: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00001420: 0000 1300 0000 7316 0000 0067 007c 005d  ......s....g.|.]
+00001430: 077d 0188 006a 007c 0119 0091 0271 0253  .}...j.|.....q.S
+00001440: 0072 1600 0000 2901 7232 0000 0029 0272  .r....).r2...).r
+00001450: 3800 0000 da01 6972 2800 0000 7216 0000  8.....ir(...r...
+00001460: 0072 1700 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
+00001470: 703e a700 0000 7302 0000 0016 007a 2148  p>....s......z!H
+00001480: 6578 426c 6f63 6b2e 6661 6365 2e3c 6c6f  exBlock.face.<lo
+00001490: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+000014a0: 4e29 06da 0a69 7369 6e73 7461 6e63 6572  N)...isinstancer
+000014b0: 3600 0000 da05 7475 706c 6572 2000 0000  6.....tupler ...
+000014c0: 7212 0000 0072 3100 0000 2907 7215 0000  r....r1...).r...
+000014d0: 0072 1400 0000 7212 0000 005a 0b6b 775f  .r....r....Z.kw_
+000014e0: 746f 5f69 6e64 6578 5a0f 696e 6465 785f  to_indexZ.index_
+000014f0: 746f 5f76 6572 7465 785a 1669 6e64 6578  to_vertexZ.index
+00001500: 5f74 6f5f 6465 6661 756c 7473 7566 6669  _to_defaultsuffi
+00001510: 7872 3200 0000 7216 0000 0072 2800 0000  xr2...r....r(...
+00001520: 7217 0000 00da 0466 6163 6571 0000 0073  r......faceq...s
+00001530: 5e00 0000 020c 0401 02ff 0402 02fe 0403  ^...............
+00001540: 02fd 0404 02fc 0405 02fb 0406 02fa 0407  ................
+00001550: 02f9 0408 02f8 0409 02f7 040a 02f6 040b  ................
+00001560: 02f5 040c 02f4 040d 02f3 040e 02f2 040f  ................
+00001570: 02f1 0410 02f0 0411 02ef 0212 0201 0201  ................
+00001580: 08ec 0816 0808 0a09 0801 1a02 0801 1001  ................
+00001590: 0a01 7a0d 4865 7842 6c6f 636b 2e66 6163  ..z.HexBlock.fac
+000015a0: 6572 0e00 0000 2907 722a 0000 0072 2b00  er....).r*...r+.
+000015b0: 0000 722c 0000 0072 0b00 0000 7218 0000  ..r,...r....r...
+000015c0: 0072 2000 0000 725f 0000 0072 1600 0000  .r ...r_...r....
+000015d0: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+000015e0: 4300 0000 5700 0000 7308 0000 0008 0014  C...W...s.......
+000015f0: 0108 0d0e 0c72 4300 0000 6300 0000 0000  .....rC...c.....
+00001600: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00001610: 0000 0073 2600 0000 6500 5a01 6400 5a02  ...s&...e.Z.d.Z.
+00001620: 6408 6402 6403 8401 5a03 6404 6405 8400  d.d.d...Z.d.d...
+00001630: 5a04 6406 6407 8400 5a05 6401 5300 2909  Z.d.d...Z.d.S.).
+00001640: da08 426f 756e 6461 7279 4e63 0500 0000  ..BoundaryNc....
+00001650: 0000 0000 0000 0000 0500 0000 0300 0000  ................
+00001660: 4300 0000 733a 0000 007c 017c 005f 007c  C...s:...|.|._.|
+00001670: 027c 005f 017c 0364 0175 0072 0d67 007d  .|._.|.d.u.r.g.}
+00001680: 036e 0874 027c 0374 0383 0272 157c 0367  .n.t.|.t...r.|.g
+00001690: 017d 037c 037c 005f 047c 047c 005f 0564  .}.|.|._.|.|._.d
+000016a0: 0153 0029 027a c469 6e69 7469 616c 697a  .S.).z.initializ
+000016b0: 6520 626f 756e 6461 7279 0a20 2020 2020  e boundary.     
+000016c0: 2020 2074 7970 655f 2069 7320 7479 7065     type_ is type
+000016d0: 206b 6579 776f 7264 2028 7761 6c6c 2c20   keyword (wall, 
+000016e0: 7061 7463 682c 2065 6d70 7479 2c20 2e2e  patch, empty, ..
+000016f0: 290a 2020 2020 2020 2020 6e61 6d65 2069  ).        name i
+00001700: 7320 6e61 7665 206f 6620 626f 756e 6461  s nave of bounda
+00001710: 7279 2065 6d65 6c6d 656e 740a 2020 2020  ry emelment.    
+00001720: 2020 2020 6661 6365 7320 6973 2066 6163      faces is fac
+00001730: 6573 2077 6869 6368 2061 7265 2061 7070  es which are app
+00001740: 6c69 6564 2077 6974 6820 7468 6973 2062  lied with this b
+00001750: 6f75 6e64 6172 7920 636f 6e64 6974 696f  oundary conditio
+00001760: 6e73 0a20 2020 2020 2020 204e 2906 da05  ns.        N)...
+00001770: 7479 7065 5f72 1200 0000 725d 0000 0072  type_r....r]...r
+00001780: 3100 0000 da05 6661 6365 73da 096e 6569  1.....faces..nei
+00001790: 6768 626f 7572 2905 7215 0000 0072 6100  ghbour).r....ra.
+000017a0: 0000 7212 0000 0072 6200 0000 7263 0000  ..r....rb...rc..
+000017b0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+000017c0: 7218 0000 00ae 0000 0073 1000 0000 0606  r........s......
+000017d0: 0601 0801 0601 0a01 0601 0601 0a01 7a11  ..............z.
+000017e0: 426f 756e 6461 7279 2e5f 5f69 6e69 745f  Boundary.__init_
+000017f0: 5f63 0200 0000 0000 0000 0000 0000 0200  _c..............
+00001800: 0000 0300 0000 4300 0000 7310 0000 007c  ......C...s....|
+00001810: 006a 00a0 017c 01a1 0101 0064 0153 0029  .j...|.....d.S.)
+00001820: 027a 5161 6464 2066 6163 6520 696e 7374  .zQadd face inst
+00001830: 616e 6365 0a20 2020 2020 2020 2066 6163  ance.        fac
+00001840: 6520 6973 2061 2046 6163 6520 696e 7374  e is a Face inst
+00001850: 616e 6365 2028 6e6f 7420 6e61 6d65 2920  ance (not name) 
+00001860: 746f 2062 6520 6164 6465 640a 2020 2020  to be added.    
+00001870: 2020 2020 4e29 0272 6200 0000 da06 6170      N).rb.....ap
+00001880: 7065 6e64 2902 7215 0000 0072 5f00 0000  pend).r....r_...
+00001890: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+000018a0: 0861 6464 5f66 6163 65bd 0000 0073 0200  .add_face....s..
+000018b0: 0000 1004 7a11 426f 756e 6461 7279 2e61  ....z.Boundary.a
+000018c0: 6464 5f66 6163 6563 0200 0000 0000 0000  dd_facec........
+000018d0: 0000 0000 0400 0000 0800 0000 4300 0000  ............C...
+000018e0: 7382 0000 007c 006a 0067 017d 027c 006a  s....|.j.g.}.|.j
+000018f0: 0164 0175 0072 167c 02a0 0264 0264 037c  .d.u.r.|...d.d.|
+00001900: 006a 039b 0064 049d 0317 00a1 0101 006e  .j...d.........n
+00001910: 107c 02a0 0264 0264 037c 006a 039b 0064  .|...d.d.|.j...d
+00001920: 057c 006a 019b 0064 049d 0517 00a1 0101  .|.j...d........
+00001930: 007c 006a 0444 005d 0d7d 037c 02a0 0264  .|.j.D.].}.|...d
+00001940: 067c 03a0 057c 01a1 019b 009d 02a1 0101  .|...|..........
+00001950: 0071 297c 02a0 0264 07a1 0101 0064 08a0  .q)|...d.....d..
+00001960: 067c 02a1 0153 0029 0972 3300 0000 4e7a  .|...S.).r3...Nz
+00001970: 027b 0a7a 0920 2020 2074 7970 6520 7a11  .{.z.    type z.
+00001980: 3b0a 2020 2020 6661 6365 730a 2020 2020  ;.    faces.    
+00001990: 287a 163b 0a20 2020 206e 6569 6768 626f  (z.;.    neighbo
+000019a0: 7572 5061 7463 6820 207a 0820 2020 2020  urPatch  z.     
+000019b0: 2020 207a 0820 2020 2029 3b0a 7dda 010a     z.    );.}...
+000019c0: 2907 7212 0000 0072 6300 0000 7264 0000  ).r....rc...rd..
+000019d0: 0072 6100 0000 7262 0000 0072 2000 0000  .ra...rb...r ...
+000019e0: 721d 0000 0029 0472 1500 0000 723b 0000  r....).r....r;..
+000019f0: 00da 0374 6d70 da01 6672 1600 0000 7216  ...tmp..fr....r.
+00001a00: 0000 0072 1700 0000 7220 0000 00c3 0000  ...r....r ......
+00001a10: 0073 1800 0000 0804 0a01 1a01 0402 0201  .s..............
+00001a20: 1401 02ff 04ff 0a04 1801 0a01 0a01 7a0f  ..............z.
+00001a30: 426f 756e 6461 7279 2e66 6f72 6d61 74a9  Boundary.format.
+00001a40: 024e 4e29 0672 2a00 0000 722b 0000 0072  .NN).r*...r+...r
+00001a50: 2c00 0000 7218 0000 0072 6500 0000 7220  ,...r....re...r 
+00001a60: 0000 0072 1600 0000 7216 0000 0072 1600  ...r....r....r..
+00001a70: 0000 7217 0000 0072 6000 0000 ad00 0000  ..r....r`.......
+00001a80: 7308 0000 0008 000a 0108 0f0c 0672 6000  s............r`.
+00001a90: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00001aa0: 0000 0004 0000 0040 0000 0073 bc00 0000  .......@...s....
+00001ab0: 6500 5a01 6400 5a02 6401 6402 8400 5a03  e.Z.d.Z.d.d...Z.
+00001ac0: 6403 6404 8400 5a04 6405 6406 8400 5a05  d.d...Z.d.d...Z.
+00001ad0: 642a 6408 6409 8401 5a06 640a 640b 8400  d*d.d...Z.d.d...
+00001ae0: 5a07 640c 640d 8400 5a08 640e 640f 8400  Z.d.d...Z.d.d...
+00001af0: 5a09 650a 6410 6410 6410 8303 6601 6411  Z.e.d.d.d...f.d.
+00001b00: 6412 8401 5a0b 6413 6414 8400 5a0c 6415  d...Z.d.d...Z.d.
+00001b10: 6416 8400 5a0d 642b 6417 6418 8401 5a0e  d...Z.d+d.d...Z.
+00001b20: 6419 641a 8400 5a0f 642c 641c 641d 8401  d.d...Z.d,d.d...
+00001b30: 5a10 641e 641f 8400 5a11 6420 6421 8400  Z.d.d...Z.d d!..
+00001b40: 5a12 6422 6423 8400 5a13 6424 6425 8400  Z.d"d#..Z.d$d%..
+00001b50: 5a14 6426 6427 8400 5a15 6516 641b 6602  Z.d&d'..Z.e.d.f.
+00001b60: 6428 6429 8401 5a17 6407 5300 292d da0d  d(d)..Z.d.S.)-..
+00001b70: 426c 6f63 6b4d 6573 6844 6963 7463 0100  BlockMeshDictc..
+00001b80: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00001b90: 0000 4300 0000 7328 0000 0064 017c 005f  ..C...s(...d.|._
+00001ba0: 0069 007c 005f 0169 007c 005f 0269 007c  .i.|._.i.|._.i.|
+00001bb0: 005f 0369 007c 005f 0464 007c 005f 0564  ._.i.|._.d.|._.d
+00001bc0: 0053 0029 024e 6700 0000 0000 00f0 3f29  .S.).Ng.......?)
+00001bd0: 06da 1163 6f6e 7665 7274 5f74 6f5f 6d65  ...convert_to_me
+00001be0: 7465 7273 723b 0000 00da 0662 6c6f 636b  tersr;.....block
+00001bf0: 73da 0565 6467 6573 da0a 626f 756e 6461  s..edges..bounda
+00001c00: 7269 6573 da16 5f76 6572 7469 6365 735f  ries.._vertices_
+00001c10: 696e 5f62 6c6f 636b 6d65 7368 7228 0000  in_blockmeshr(..
+00001c20: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00001c30: 7218 0000 00d6 0000 0073 0c00 0000 0601  r........s......
+00001c40: 0601 0601 0601 0601 0a01 7a16 426c 6f63  ..........z.Bloc
+00001c50: 6b4d 6573 6844 6963 742e 5f5f 696e 6974  kMeshDict.__init
+00001c60: 5f5f 6302 0000 0000 0000 0000 0000 0003  __c.............
+00001c70: 0000 0009 0000 0043 0000 0073 2400 0000  .......C...s$...
+00001c80: 6401 6402 6403 6404 6405 6406 6407 6407  d.d.d.d.d.d.d.d.
+00001c90: 6408 9c08 7d02 7c02 7c01 1900 7c00 5f00  d...}.|.|...|._.
+00001ca0: 6409 5300 290a 7a22 7365 7420 7365 6c66  d.S.).z"set self
+00001cb0: 2e63 6f6d 7665 7274 5f74 6f5f 6d65 7465  .comvert_to_mete
+00001cc0: 7273 2062 7920 776f 7264 69e8 0300 0072  rs by wordi....r
+00001cd0: 0600 0000 677b 14ae 47e1 7a84 3f67 fca9  ....g{..G.z.?g..
+00001ce0: f1d2 4d62 503f 678d edb5 a0f7 c6b0 3e67  ..MbP?g.......>g
+00001cf0: 95d6 26e8 0b2e 113e 67bb bdd7 d9df 7cdb  ..&....>g.....|.
+00001d00: 3d29 08da 026b 6dda 016d da02 636d da02  =)...km..m..cm..
+00001d10: 6d6d da02 756d da02 6e6d da01 415a 0841  mm..um..nm..AZ.A
+00001d20: 6e67 7374 726f 6d4e a901 726b 0000 0029  ngstromN..rk...)
+00001d30: 0372 1500 0000 da06 6d65 7472 6963 5a17  .r......metricZ.
+00001d40: 6d65 7472 6963 7379 6d5f 746f 5f63 6f6e  metricsym_to_con
+00001d50: 7665 7273 696f 6e72 1600 0000 7216 0000  versionr....r...
+00001d60: 0072 1700 0000 da0a 7365 745f 6d65 7472  .r......set_metr
+00001d70: 6963 de00 0000 7314 0000 0002 0302 0102  ic....s.........
+00001d80: 0102 0102 0102 0102 0102 0106 f80e 0a7a  ...............z
+00001d90: 1842 6c6f 636b 4d65 7368 4469 6374 2e73  .BlockMeshDict.s
+00001da0: 6574 5f6d 6574 7269 6363 0200 0000 0000  et_metricc......
+00001db0: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
+00001dc0: 0000 730a 0000 007c 017c 005f 0064 0053  ..s....|.|._.d.S
+00001dd0: 0072 0e00 0000 7277 0000 0029 0272 1500  .r....rw...).r..
+00001de0: 0000 da05 7363 616c 6572 1600 0000 7216  ....scaler....r.
+00001df0: 0000 0072 1700 0000 da09 7365 745f 7363  ...r......set_sc
+00001e00: 616c 65ec 0000 0073 0200 0000 0a01 7a17  ale....s......z.
+00001e10: 426c 6f63 6b4d 6573 6844 6963 742e 7365  BlockMeshDict.se
+00001e20: 745f 7363 616c 654e 6305 0000 0000 0000  t_scaleNc.......
+00001e30: 0000 0000 0006 0000 0005 0000 0043 0000  .............C..
+00001e40: 0073 5800 0000 7400 7c01 7401 8302 721b  .sX...t.|.t...r.
+00001e50: 7402 6401 6402 8400 7c02 7c03 7c04 6603  t.d.d...|.|.|.f.
+00001e60: 4400 8301 8301 7215 7403 6403 8301 8201  D.....r.t.d.....
+00001e70: 7c01 7d05 7c05 6a04 7d04 6e07 7401 7c01  |.}.|.j.}.n.t.|.
+00001e80: 7c02 7c03 7c04 8304 7d05 7c05 7c00 6a05  |.|.|...}.|.|.j.
+00001e90: 7c04 3c00 7c00 6a05 7c04 1900 5300 2904  |.<.|.j.|...S.).
+00001ea0: 7ab2 6164 6420 7665 7274 6578 2062 7920  z.add vertex by 
+00001eb0: 636f 6f72 6469 6e61 7465 2061 6e64 2075  coordinate and u
+00001ec0: 6e69 7120 6e61 6d65 0a20 2020 2020 2020  niq name.       
+00001ed0: 2078 2079 207a 2069 7320 636f 6f72 6469   x y z is coordi
+00001ee0: 6e61 7465 7320 6f66 2076 6572 7465 780a  nates of vertex.
+00001ef0: 2020 2020 2020 2020 6e61 6d65 2069 7320          name is 
+00001f00: 756e 6971 206e 616d 6520 746f 2072 6566  uniq name to ref
+00001f10: 6572 2074 6865 2076 6572 7465 780a 2020  er the vertex.  
+00001f20: 2020 2020 2020 7265 7475 726e 7320 5665        returns Ve
+00001f30: 7274 6578 206f 626a 6563 7420 7768 6963  rtex object whic
+00001f40: 6920 6973 2061 6464 6564 2e0a 2020 2020  i is added..    
+00001f50: 2020 2020 6301 0000 0000 0000 0000 0000      c...........
+00001f60: 0002 0000 0003 0000 0073 0000 0073 1800  .........s...s..
+00001f70: 0000 8100 7c00 5d07 7d01 7c01 6400 7501  ....|.].}.|.d.u.
+00001f80: 5600 0100 7102 6400 5300 720e 0000 0072  V...q.d.S.r....r
+00001f90: 1600 0000 2902 7238 0000 00da 0361 7267  ....).r8.....arg
+00001fa0: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00001fb0: 3c00 0000 f600 0000 7304 0000 0002 8016  <.......s.......
+00001fc0: 007a 2b42 6c6f 636b 4d65 7368 4469 6374  .z+BlockMeshDict
+00001fd0: 2e61 6464 5f76 6572 7465 782e 3c6c 6f63  .add_vertex.<loc
+00001fe0: 616c 733e 2e3c 6765 6e65 7870 723e 7a40  als>.<genexpr>z@
+00001ff0: 7820 6973 2061 2056 6572 7465 7820 616e  x is a Vertex an
+00002000: 6420 6061 6e79 2861 7267 2069 7320 6e6f  d `any(arg is no
+00002010: 7420 4e6f 6e65 2066 6f72 2061 7267 2069  t None for arg i
+00002020: 6e20 2879 2c20 7a2c 206e 616d 6529 2960  n (y, z, name))`
+00002030: 2906 725d 0000 0072 0d00 0000 da03 616e  ).r]...r......an
+00002040: 79da 0a56 616c 7565 4572 726f 7272 1200  y..ValueErrorr..
+00002050: 0000 723b 0000 0029 0672 1500 0000 720f  ..r;...).r....r.
+00002060: 0000 0072 1000 0000 7211 0000 0072 1200  ...r....r....r..
+00002070: 0000 5a06 7665 7274 6578 7216 0000 0072  ..Z.vertexr....r
+00002080: 1600 0000 7217 0000 00da 0a61 6464 5f76  ....r......add_v
+00002090: 6572 7465 78ef 0000 0073 1400 0000 0a06  ertex....s......
+000020a0: 1801 0201 0201 04ff 0404 0801 0e02 0a01  ................
+000020b0: 0a01 7a18 426c 6f63 6b4d 6573 6844 6963  ..z.BlockMeshDic
+000020c0: 742e 6164 645f 7665 7274 6578 6302 0000  t.add_vertexc...
+000020d0: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+000020e0: 0043 0000 0073 0c00 0000 7c00 6a00 7c01  .C...s....|.j.|.
+000020f0: 3d00 6401 5300 2902 7a1f 6465 6c20 6e61  =.d.S.).z.del na
+00002100: 6d65 206b 6579 2066 726f 6d20 7365 6c66  me key from self
+00002110: 2e76 6572 7469 6365 734e 723a 0000 0029  .verticesNr:...)
+00002120: 0272 1500 0000 7212 0000 0072 1600 0000  .r....r....r....
+00002130: 7216 0000 0072 1700 0000 da0a 6465 6c5f  r....r......del_
+00002140: 7665 7274 6578 0201 0000 7302 0000 000c  vertex....s.....
+00002150: 027a 1842 6c6f 636b 4d65 7368 4469 6374  .z.BlockMeshDict
+00002160: 2e64 656c 5f76 6572 7465 7863 0200 0000  .del_vertexc....
+00002170: 0000 0000 0000 0000 0600 0000 0400 0000  ................
+00002180: 4700 0000 733a 0000 007c 006a 007c 0119  G...s:...|.j.|..
+00002190: 007d 037c 0244 005d 137d 047c 006a 007c  .}.|.D.].}.|.j.|
+000021a0: 0419 007d 057c 036a 01a0 027c 056a 01a1  ...}.|.j...|.j..
+000021b0: 0101 007c 037c 006a 007c 043c 0071 0764  ...|.|.j.|.<.q.d
+000021c0: 0153 0029 027a e274 7265 6174 206e 616d  .S.).z.treat nam
+000021d0: 6531 2c20 6e61 6d65 322c 202e 2e2e 2061  e1, name2, ... a
+000021e0: 7320 7361 6d65 2070 6f69 6e74 2e0a 0a20  s same point... 
+000021f0: 2020 2020 2020 206e 616d 6532 2e61 6c69         name2.ali
+00002200: 6173 2c20 6e61 6d65 332e 616c 6961 732c  as, name3.alias,
+00002210: 202e 2e2e 2061 7265 206d 6572 6765 6420   ... are merged 
+00002220: 7769 7468 206e 616d 6531 2e61 6c69 6173  with name1.alias
+00002230: 0a20 2020 2020 2020 2074 6865 206b 6579  .        the key
+00002240: 206e 616d 6532 2c20 6e61 6d65 332c 202e   name2, name3, .
+00002250: 2e2e 2069 6e20 7365 6c66 2e76 6572 7469  .. in self.verti
+00002260: 6365 7320 6172 6520 6b65 7074 2061 6e64  ces are kept and
+00002270: 206d 6170 7065 6420 746f 0a20 2020 2020   mapped to.     
+00002280: 2020 2073 616d 6520 5665 7274 6578 2069     same Vertex i
+00002290: 6e73 7461 6e63 6520 6173 206e 616d 6531  nstance as name1
+000022a0: 0a20 2020 2020 2020 204e 2903 723b 0000  .        N).r;..
+000022b0: 0072 1300 0000 da06 7570 6461 7465 2906  .r......update).
+000022c0: 7215 0000 00da 056e 616d 6531 da05 6e61  r......name1..na
+000022d0: 6d65 73da 0176 724d 0000 0072 4700 0000  mes..vrM...rG...
+000022e0: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+000022f0: 0d72 6564 7563 655f 7665 7274 6578 0601  .reduce_vertex..
+00002300: 0000 730c 0000 000a 0708 010a 010e 010c  ..s.............
+00002310: 0204 fc7a 1b42 6c6f 636b 4d65 7368 4469  ...z.BlockMeshDi
+00002320: 6374 2e72 6564 7563 655f 7665 7274 6578  ct.reduce_vertex
+00002330: 6301 0000 0000 0000 0000 0000 0007 0000  c...............
+00002340: 0005 0000 0043 0000 0073 7800 0000 7400  .....C...sx...t.
+00002350: 7401 7c00 6a02 a003 a100 8301 6401 6402  t.|.j.......d.d.
+00002360: 8400 6403 8d02 7d01 6700 7d02 7404 7c01  ..d...}.g.}.t.|.
+00002370: 6404 6402 8400 8302 4400 5d0b 5c02 7d03  d.d.....D.].\.}.
+00002380: 7d04 7c02 a005 7401 7c04 8301 a101 0100  }.|...t.|.......
+00002390: 7116 7c02 4400 5d15 7d05 7406 7c05 8301  q.|.D.].}.t.|...
+000023a0: 6405 6b02 722d 7124 6406 6407 8400 7c05  d.k.r-q$d.d...|.
+000023b0: 4400 8301 7d06 7c00 6a07 7c06 8e00 0100  D...}.|.j.|.....
+000023c0: 7124 6408 5300 2909 7a39 6361 6c6c 2072  q$d.S.).z9call r
+000023d0: 6564 7563 655f 7665 7274 6578 206f 6e20  educe_vertex on 
+000023e0: 616c 6c20 7665 7274 6963 6573 2077 6974  all vertices wit
+000023f0: 6820 6964 656e 7469 6361 6c20 7661 6c75  h identical valu
+00002400: 6573 2e63 0100 0000 0000 0000 0000 0000  es.c............
+00002410: 0100 0000 0300 0000 5300 0000 f30c 0000  ........S.......
+00002420: 0074 007c 0064 0119 0083 0153 00a9 024e  .t.|.d.....S...N
+00002430: 7206 0000 00a9 0172 2700 0000 a901 7284  r......r'.....r.
+00002440: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00002450: 0000 da08 3c6c 616d 6264 613e 1901 0000  ....<lambda>....
+00002460: f302 0000 000c 007a 2e42 6c6f 636b 4d65  .......z.BlockMe
+00002470: 7368 4469 6374 2e6d 6572 6765 5f76 6572  shDict.merge_ver
+00002480: 7469 6365 732e 3c6c 6f63 616c 733e 2e3c  tices.<locals>.<
+00002490: 6c61 6d62 6461 3e29 01da 036b 6579 6301  lambda>)...keyc.
+000024a0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+000024b0: 0000 0053 0000 0072 8600 0000 7287 0000  ...S...r....r...
+000024c0: 0072 8800 0000 7289 0000 0072 1600 0000  .r....r....r....
+000024d0: 7216 0000 0072 1700 0000 728a 0000 001c  r....r....r.....
+000024e0: 0100 0072 8b00 0000 7206 0000 0063 0100  ...r....r....c..
+000024f0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00002500: 0000 5300 0000 7314 0000 0067 007c 005d  ..S...s....g.|.]
+00002510: 067d 017c 0164 0019 0091 0271 0253 0029  .}.|.d.....q.S.)
+00002520: 0172 0100 0000 7216 0000 0029 0272 3800  .r....r....).r8.
+00002530: 0000 7284 0000 0072 1600 0000 7216 0000  ..r....r....r...
+00002540: 0072 1700 0000 725c 0000 0021 0100 0073  .r....r\...!...s
+00002550: 0200 0000 1400 7a30 426c 6f63 6b4d 6573  ......z0BlockMes
+00002560: 6844 6963 742e 6d65 7267 655f 7665 7274  hDict.merge_vert
+00002570: 6963 6573 2e3c 6c6f 6361 6c73 3e2e 3c6c  ices.<locals>.<l
+00002580: 6973 7463 6f6d 703e 4e29 0872 1e00 0000  istcomp>N).r....
+00002590: da04 6c69 7374 723b 0000 00da 0569 7465  ..listr;.....ite
+000025a0: 6d73 7202 0000 0072 6400 0000 721c 0000  msr....rd...r...
+000025b0: 0072 8500 0000 2907 7215 0000 005a 0f73  .r....).r....Z.s
+000025c0: 6f72 7465 645f 7665 7274 6963 6573 da06  orted_vertices..
+000025d0: 6772 6f75 7073 da01 6bda 0167 da05 6772  groups..k..g..gr
+000025e0: 6f75 7072 8300 0000 7216 0000 0072 1600  oupr....r....r..
+000025f0: 0000 7217 0000 00da 0e6d 6572 6765 5f76  ..r......merge_v
+00002600: 6572 7469 6365 7314 0100 0073 1800 0000  ertices....s....
+00002610: 0204 1201 06ff 0403 1601 1001 0801 0c01  ................
+00002620: 0201 0e01 0c01 04fc 7a1c 426c 6f63 6b4d  ........z.BlockM
+00002630: 6573 6844 6963 742e 6d65 7267 655f 7665  eshDict.merge_ve
+00002640: 7274 6963 6573 7206 0000 0063 0500 0000  rticesr....c....
+00002650: 0000 0000 0000 0000 0600 0000 0500 0000  ................
+00002660: 4300 0000 731c 0000 0074 007c 017c 027c  C...s....t.|.|.|
+00002670: 037c 0483 047d 057c 057c 006a 017c 033c  .|...}.|.|.j.|.<
+00002680: 007c 0553 0072 0e00 0000 2902 7243 0000  .|.S.r....).rC..
+00002690: 0072 6c00 0000 2906 7215 0000 0072 3200  .rl...).r....r2.
+000026a0: 0000 7244 0000 0072 1200 0000 7245 0000  ..rD...r....rE..
+000026b0: 0072 5000 0000 7216 0000 0072 1600 0000  .rP...r....r....
+000026c0: 7217 0000 00da 0c61 6464 5f68 6578 626c  r......add_hexbl
+000026d0: 6f63 6b24 0100 00f3 0600 0000 0e01 0a01  ock$............
+000026e0: 0401 7a1a 426c 6f63 6b4d 6573 6844 6963  ..z.BlockMeshDic
+000026f0: 742e 6164 645f 6865 7862 6c6f 636b 6304  t.add_hexblockc.
+00002700: 0000 0000 0000 0000 0000 0005 0000 0004  ................
+00002710: 0000 0043 0000 00f3 1a00 0000 7400 7c01  ...C........t.|.
+00002720: 7c02 7c03 8303 7d04 7c04 7c00 6a01 7c02  |.|...}.|.|.j.|.
+00002730: 3c00 7c04 5300 720e 0000 0029 0272 0700  <.|.S.r....).r..
+00002740: 0000 726d 0000 0029 0572 1500 0000 7232  ..rm...).r....r2
+00002750: 0000 0072 1200 0000 5a0c 696e 7465 725f  ...r....Z.inter_
+00002760: 7665 7274 6578 7249 0000 0072 1600 0000  vertexrI...r....
+00002770: 7216 0000 0072 1700 0000 da0b 6164 645f  r....r......add_
+00002780: 6172 6365 6467 6529 0100 00f3 0600 0000  arcedge)........
+00002790: 0c01 0a01 0401 7a19 426c 6f63 6b4d 6573  ......z.BlockMes
+000027a0: 6844 6963 742e 6164 645f 6172 6365 6467  hDict.add_arcedg
+000027b0: 6563 0400 0000 0000 0000 0000 0000 0500  ec..............
+000027c0: 0000 0400 0000 4300 0000 7296 0000 0072  ......C...r....r
+000027d0: 0e00 0000 2902 7208 0000 0072 6d00 0000  ....).r....rm...
+000027e0: 2905 7215 0000 0072 3200 0000 7212 0000  ).r....r2...r...
+000027f0: 00da 0670 6f69 6e74 7372 4900 0000 7216  ...pointsrI...r.
+00002800: 0000 0072 1600 0000 7217 0000 00da 0e61  ...r....r......a
+00002810: 6464 5f73 706c 696e 6565 6467 652e 0100  dd_splineedge...
+00002820: 0072 9800 0000 7a1c 426c 6f63 6b4d 6573  .r....z.BlockMes
+00002830: 6844 6963 742e 6164 645f 7370 6c69 6e65  hDict.add_spline
+00002840: 6564 6765 6305 0000 0000 0000 0000 0000  edgec...........
+00002850: 0006 0000 0005 0000 0043 0000 0073 1c00  .........C...s..
+00002860: 0000 7400 7c01 7c02 7c03 7c04 8304 7d05  ..t.|.|.|.|...}.
+00002870: 7c05 7c00 6a01 7c02 3c00 7c05 5300 720e  |.|.j.|.<.|.S.r.
+00002880: 0000 0029 0272 6000 0000 726e 0000 0029  ...).r`...rn...)
+00002890: 0672 1500 0000 7261 0000 0072 1200 0000  .r....ra...r....
+000028a0: 7262 0000 0072 6300 0000 7250 0000 0072  rb...rc...rP...r
+000028b0: 1600 0000 7216 0000 0072 1700 0000 da0c  ....r....r......
+000028c0: 6164 645f 626f 756e 6461 7279 3301 0000  add_boundary3...
+000028d0: 7295 0000 007a 1a42 6c6f 636b 4d65 7368  r....z.BlockMesh
+000028e0: 4469 6374 2e61 6464 5f62 6f75 6e64 6172  Dict.add_boundar
+000028f0: 7963 0500 0000 0000 0000 0000 0000 0700  yc..............
+00002900: 0000 0600 0000 4300 0000 732c 0000 007c  ......C...s,...|
+00002910: 006a 0064 017c 017c 037c 0264 028d 047d  .j.d.|.|.|.d...}
+00002920: 057c 006a 0064 017c 027c 047c 0164 028d  .|.j.d.|.|.|.d..
+00002930: 047d 067c 057c 0666 0253 0029 034e da06  .}.|.|.f.S.).N..
+00002940: 6379 636c 6963 2901 7263 0000 0029 0172  cyclic).rc...).r
+00002950: 9b00 0000 2907 7215 0000 005a 056e 616d  ....).r....Z.nam
+00002960: 6530 7282 0000 005a 0666 6163 6573 305a  e0r....Z.faces0Z
+00002970: 0666 6163 6573 31da 0262 30da 0262 3172  .faces1..b0..b1r
+00002980: 1600 0000 7216 0000 0072 1700 0000 da15  ....r....r......
+00002990: 6164 645f 6379 636c 6963 5f62 6f75 6e64  add_cyclic_bound
+000029a0: 6172 6965 7338 0100 0073 0600 0000 1201  aries8...s......
+000029b0: 1201 0801 7a23 426c 6f63 6b4d 6573 6844  ....z#BlockMeshD
+000029c0: 6963 742e 6164 645f 6379 636c 6963 5f62  ict.add_cyclic_b
+000029d0: 6f75 6e64 6172 6965 7354 6302 0000 0000  oundariesTc.....
+000029e0: 0000 0000 0000 0008 0000 0005 0000 0043  ...............C
+000029f0: 0000 0073 ba00 0000 7400 8300 7d02 6700  ...s....t...}.g.
+00002a00: 7c00 5f01 7c00 6a02 a003 a100 4400 5d1e  |._.|.j.....D.].
+00002a10: 7d03 7c03 6a04 4400 5d18 7d04 7c00 6a05  }.|.j.D.].}.|.j.
+00002a20: 7c04 1900 7d05 7c05 6a06 7c02 7601 7228  |...}.|.j.|.v.r(
+00002a30: 7c02 a007 7c05 6a06 a101 0100 7c00 6a01  |...|.j.....|.j.
+00002a40: a008 7c05 a101 0100 7110 710b 7c01 6401  ..|.....q.q.|.d.
+00002a50: 6b02 7246 6700 7c00 5f01 7c00 6a05 a009  k.rFg.|._.|.j...
+00002a60: a100 4400 5d0e 5c02 7d06 7d05 7c06 7c02  ..D.].\.}.}.|.|.
+00002a70: 7600 7244 7c00 6a01 a008 7c05 a101 0100  v.rD|.j...|.....
+00002a80: 7136 6e08 7c01 724e 740a 7c00 6a01 8301  q6n.|.rNt.|.j...
+00002a90: 7c00 5f01 740b 7c00 6a01 8301 4400 5d07  |._.t.|.j...D.].
+00002aa0: 5c02 7d07 7d05 7c07 7c05 5f0c 7153 6402  \.}.}.|.|._.qSd.
+00002ab0: 5300 2903 7ae3 312e 2063 7265 6174 6520  S.).z.1. create 
+00002ac0: 6c69 7374 206f 6620 5665 7274 6578 2077  list of Vertex w
+00002ad0: 6869 6368 2061 7265 2072 6566 6572 7265  hich are referre
+00002ae0: 6420 6279 2062 6c6f 636b 7320 6f6e 6c79  d by blocks only
+00002af0: 2e0a 2020 2020 2020 2020 322e 2073 6f72  ..        2. sor
+00002b00: 7420 7665 7274 6578 2061 6363 6f72 6469  t vertex accordi
+00002b10: 6e67 2074 6f20 2878 2c20 792c 207a 290a  ng to (x, y, z).
+00002b20: 2020 2020 2020 2020 332e 2061 7373 6967          3. assig
+00002b30: 6e20 7365 7175 656e 6365 206e 756d 6265  n sequence numbe
+00002b40: 7220 666f 7220 6561 6368 2056 6572 7465  r for each Verte
+00002b50: 780a 2020 2020 2020 2020 342e 2073 6f72  x.        4. sor
+00002b60: 7465 6420 6c69 7374 2069 7320 7361 7665  ted list is save
+00002b70: 6420 6173 2073 656c 662e 5f76 6572 7469  d as self._verti
+00002b80: 6365 735f 696e 5f62 6c6f 636b 6d65 7368  ces_in_blockmesh
+00002b90: 0a20 2020 2020 2020 205a 0861 735f 6164  .        Z.as_ad
+00002ba0: 6465 644e 290d da03 7365 7472 6f00 0000  dedN)...setro...
+00002bb0: 726c 0000 00da 0676 616c 7565 7372 3200  rl.....valuesr2.
+00002bc0: 0000 723b 0000 0072 1200 0000 da03 6164  ..r;...r......ad
+00002bd0: 6472 6400 0000 728e 0000 0072 1e00 0000  drd...r....r....
+00002be0: da09 656e 756d 6572 6174 6572 1400 0000  ..enumerater....
+00002bf0: 2908 7215 0000 00da 0473 6f72 745a 0b76  ).r......sortZ.v
+00002c00: 6e61 6d65 735f 6b65 7074 7250 0000 0072  names_keptrP...r
+00002c10: 4d00 0000 7284 0000 00da 0576 6e61 6d65  M...r......vname
+00002c20: 725b 0000 0072 1600 0000 7216 0000 0072  r[...r....r....r
+00002c30: 1700 0000 da0f 6173 7369 676e 5f76 6572  ......assign_ver
+00002c40: 7465 7869 643d 0100 0073 2c00 0000 0607  texid=...s,.....
+00002c50: 0601 0e01 0a01 0a01 0a01 0c01 0c01 0280  ................
+00002c60: 02fc 0805 0601 1201 0801 0c01 0280 02fe  ................
+00002c70: 0403 0c01 1201 0801 04ff 7a1d 426c 6f63  ..........z.Bloc
+00002c80: 6b4d 6573 6844 6963 742e 6173 7369 676e  kMeshDict.assign
+00002c90: 5f76 6572 7465 7869 6463 0100 0000 0000  _vertexidc......
+00002ca0: 0000 0000 0000 0300 0000 0600 0000 4300  ..............C.
+00002cb0: 0000 7338 0000 0064 0167 017d 017c 006a  ..s8...d.g.}.|.j
+00002cc0: 0044 005d 0b7d 027c 01a0 0164 027c 02a0  .D.].}.|...d.|..
+00002cd0: 02a1 0017 00a1 0101 0071 067c 01a0 0164  .........q.|...d
+00002ce0: 03a1 0101 0064 04a0 037c 01a1 0153 0029  .....d...|...S.)
+00002cf0: 057a ec66 6f72 6d61 7420 7665 7274 6963  .z.format vertic
+00002d00: 6573 2073 6563 7469 6f6e 2e0a 2020 2020  es section..    
+00002d10: 2020 2020 6173 7369 676e 5f76 6572 7465      assign_verte
+00002d20: 7869 6428 2920 7368 6f75 6c64 2062 6520  xid() should be 
+00002d30: 6361 6c6c 6564 2062 6566 6f72 6520 7468  called before th
+00002d40: 6973 206d 6574 686f 642c 2062 6563 6175  is method, becau
+00002d50: 7365 0a20 2020 2020 2020 2073 656c 662e  se.        self.
+00002d60: 5f76 6572 7469 6365 735f 696e 5f62 6c6f  _vertices_in_blo
+00002d70: 636b 6d65 7368 2073 686f 756c 6420 6265  ckmesh should be
+00002d80: 2061 7661 696c 6162 6c65 2061 6e64 0a20   available and. 
+00002d90: 2020 2020 2020 206d 656d 6265 7273 206f         members o
+00002da0: 6620 7365 6c66 2e5f 7665 7274 6963 6573  f self._vertices
+00002db0: 5f69 6e5f 626c 6f63 6b6d 6573 6820 7368  _in_blockmesh sh
+00002dc0: 6f75 6c64 2068 6176 6520 7661 6c69 6420  ould have valid 
+00002dd0: 696e 6465 782e 0a20 2020 2020 2020 207a  index..        z
+00002de0: 0a76 6572 7469 6365 730a 28fa 0420 2020  .vertices.(..   
+00002df0: 20fa 0229 3b72 6600 0000 2904 726f 0000   ..);rf...).ro..
+00002e00: 0072 6400 0000 7220 0000 0072 1d00 0000  .rd...r ...r....
+00002e10: 2903 7215 0000 0072 6700 0000 7284 0000  ).r....rg...r...
+00002e20: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00002e30: da17 666f 726d 6174 5f76 6572 7469 6365  ..format_vertice
+00002e40: 735f 7365 6374 696f 6e56 0100 0073 0a00  s_sectionV...s..
+00002e50: 0000 0606 0a01 1401 0a01 0a01 7a25 426c  ............z%Bl
+00002e60: 6f63 6b4d 6573 6844 6963 742e 666f 726d  ockMeshDict.form
+00002e70: 6174 5f76 6572 7469 6365 735f 7365 6374  at_vertices_sect
+00002e80: 696f 6e63 0100 0000 0000 0000 0000 0000  ionc............
+00002e90: 0300 0000 0700 0000 4300 0000 f340 0000  ........C....@..
+00002ea0: 0064 0167 017d 017c 006a 00a0 01a1 0044  .d.g.}.|.j.....D
+00002eb0: 005d 0d7d 027c 01a0 0264 027c 02a0 037c  .].}.|...d.|...|
+00002ec0: 006a 04a1 0117 00a1 0101 0071 087c 01a0  .j.........q.|..
+00002ed0: 0264 03a1 0101 0064 04a0 057c 01a1 0153  .d.....d...|...S
+00002ee0: 0029 057a a266 6f72 6d61 7420 626c 6f63  .).z.format bloc
+00002ef0: 6b73 2073 6563 7469 6f6e 2e0a 2020 2020  ks section..    
+00002f00: 2020 2020 6173 7369 676e 5f76 6572 7465      assign_verte
+00002f10: 7869 6428 2920 7368 6f75 6c64 2062 6520  xid() should be 
+00002f20: 6361 6c6c 6564 2062 6566 6f72 6520 7468  called before th
+00002f30: 6973 206d 6574 686f 642c 2062 6563 6175  is method, becau
+00002f40: 7365 0a20 2020 2020 2020 2076 6572 7469  se.        verti
+00002f50: 6365 7320 7265 6665 7265 6420 6279 2062  ces refered by b
+00002f60: 6c6f 636b 7320 7368 6f75 6c64 2068 6176  locks should hav
+00002f70: 6520 7661 6c69 6420 696e 6465 782e 0a20  e valid index.. 
+00002f80: 2020 2020 2020 207a 0862 6c6f 636b 730a         z.blocks.
+00002f90: 2872 a700 0000 72a8 0000 0072 6600 0000  (r....r....rf...
+00002fa0: 2906 726c 0000 0072 a100 0000 7264 0000  ).rl...r....rd..
+00002fb0: 0072 2000 0000 723b 0000 0072 1d00 0000  .r ...r;...r....
+00002fc0: 2903 7215 0000 0072 6700 0000 7250 0000  ).r....rg...rP..
+00002fd0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00002fe0: da15 666f 726d 6174 5f62 6c6f 636b 735f  ..format_blocks_
+00002ff0: 7365 6374 696f 6e62 0100 0073 0a00 0000  sectionb...s....
+00003000: 0605 0e01 1801 0a01 0a01 7a23 426c 6f63  ..........z#Bloc
+00003010: 6b4d 6573 6844 6963 742e 666f 726d 6174  kMeshDict.format
+00003020: 5f62 6c6f 636b 735f 7365 6374 696f 6e63  _blocks_sectionc
+00003030: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+00003040: 0700 0000 4300 0000 72aa 0000 0029 057a  ....C...r....).z
+00003050: a166 6f72 6d61 7420 6564 6765 7320 7365  .format edges se
+00003060: 6374 696f 6e2e 0a20 2020 2020 2020 2061  ction..        a
+00003070: 7373 6967 6e5f 7665 7274 6578 6964 2829  ssign_vertexid()
+00003080: 2073 686f 756c 6420 6265 2063 616c 6c65   should be calle
+00003090: 6420 6265 666f 7265 2074 6869 7320 6d65  d before this me
+000030a0: 7468 6f64 2c20 6265 6361 7573 650a 2020  thod, because.  
+000030b0: 2020 2020 2020 7665 7274 6963 6573 2072        vertices r
+000030c0: 6566 6572 6564 2062 7920 626c 6f63 6b73  efered by blocks
+000030d0: 2073 686f 756c 6420 6861 7665 2076 616c   should have val
+000030e0: 6964 2069 6e64 6578 2e0a 2020 2020 2020  id index..      
+000030f0: 2020 7a07 6564 6765 730a 2872 a700 0000    z.edges.(r....
+00003100: 72a8 0000 0072 6600 0000 2906 726d 0000  r....rf...).rm..
+00003110: 0072 a100 0000 7264 0000 0072 2000 0000  .r....rd...r ...
+00003120: 723b 0000 0072 1d00 0000 2903 7215 0000  r;...r....).r...
+00003130: 0072 6700 0000 7249 0000 0072 1600 0000  .rg...rI...r....
+00003140: 7216 0000 0072 1700 0000 da14 666f 726d  r....r......form
+00003150: 6174 5f65 6467 6573 5f73 6563 7469 6f6e  at_edges_section
+00003160: 6d01 0000 730a 0000 0006 060e 0118 010a  m...s...........
+00003170: 010a 017a 2242 6c6f 636b 4d65 7368 4469  ...z"BlockMeshDi
+00003180: 6374 2e66 6f72 6d61 745f 6564 6765 735f  ct.format_edges_
+00003190: 7365 6374 696f 6e63 0100 0000 0000 0000  sectionc........
+000031a0: 0000 0000 0500 0000 0600 0000 4300 0000  ............C...
+000031b0: 7354 0000 0064 0167 017d 017c 006a 00a0  sT...d.g.}.|.j..
+000031c0: 01a1 0044 005d 177d 0264 027d 037c 02a0  ...D.].}.d.}.|..
+000031d0: 027c 006a 03a1 01a0 0464 0364 037c 0317  .|.j.....d.d.|..
+000031e0: 00a1 027d 047c 01a0 057c 037c 0417 00a1  ...}.|...|.|....
+000031f0: 0101 0071 087c 01a0 0564 04a1 0101 0064  ...q.|...d.....d
+00003200: 03a0 067c 01a1 0153 0029 057a a366 6f72  ...|...S.).z.for
+00003210: 6d61 7420 626f 756e 6461 7279 2073 6563  mat boundary sec
+00003220: 7469 6f6e 2e0a 2020 2020 2020 2020 6173  tion..        as
+00003230: 7369 676e 5f76 6572 7465 7869 6428 2920  sign_vertexid() 
+00003240: 7368 6f75 6c64 2062 6520 6361 6c6c 6564  should be called
+00003250: 2062 6566 6f72 6520 7468 6973 206d 6574   before this met
+00003260: 686f 642c 2062 6563 6175 7365 0a20 2020  hod, because.   
+00003270: 2020 2020 2076 6572 7469 6365 7320 7265       vertices re
+00003280: 6665 7265 6420 6279 2066 6163 6573 2073  fered by faces s
+00003290: 686f 756c 6420 6861 7665 2076 616c 6964  hould have valid
+000032a0: 2069 6e64 6578 2e0a 2020 2020 2020 2020   index..        
+000032b0: 7a0a 626f 756e 6461 7279 0a28 72a7 0000  z.boundary.(r...
+000032c0: 0072 6600 0000 72a8 0000 0029 0772 6e00  .rf...r....).rn.
+000032d0: 0000 72a1 0000 0072 2000 0000 723b 0000  ..r....r ...r;..
+000032e0: 00da 0772 6570 6c61 6365 7264 0000 0072  ...replacerd...r
+000032f0: 1d00 0000 2905 7215 0000 0072 6700 0000  ....).r....rg...
+00003300: 7250 0000 00da 0669 6e64 656e 7472 3f00  rP.....indentr?.
+00003310: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00003320: 00da 1766 6f72 6d61 745f 626f 756e 6461  ...format_bounda
+00003330: 7279 5f73 6563 7469 6f6e 7901 0000 730e  ry_sectiony...s.
+00003340: 0000 0006 060e 0104 0218 0110 010a 010a  ................
+00003350: 017a 2542 6c6f 636b 4d65 7368 4469 6374  .z%BlockMeshDict
+00003360: 2e66 6f72 6d61 745f 626f 756e 6461 7279  .format_boundary
+00003370: 5f73 6563 7469 6f6e 6301 0000 0000 0000  _sectionc.......
+00003380: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+00003390: 0073 0400 0000 6401 5300 2902 4e7a 146d  .s....d.S.).Nz.m
+000033a0: 6572 6765 5061 7463 6850 6169 7273 0a28  ergePatchPairs.(
+000033b0: 0a29 3b72 1600 0000 7228 0000 0072 1600  .);r....r(...r..
+000033c0: 0000 7216 0000 0072 1700 0000 da1e 666f  ..r....r......fo
+000033d0: 726d 6174 5f6d 6572 6765 7061 7463 6870  rmat_mergepatchp
+000033e0: 6169 7273 5f73 6563 7469 6f6e 8801 0000  airs_section....
+000033f0: 7302 0000 0004 017a 2c42 6c6f 636b 4d65  s......z,BlockMe
+00003400: 7368 4469 6374 2e66 6f72 6d61 745f 6d65  shDict.format_me
+00003410: 7267 6570 6174 6368 7061 6972 735f 7365  rgepatchpairs_se
+00003420: 6374 696f 6e63 0300 0000 0000 0000 0000  ctionc..........
+00003430: 0000 0400 0000 0900 0000 4300 0000 7346  ..........C...sF
+00003440: 0000 007c 006a 007c 0264 018d 0101 0074  ...|.j.|.d.....t
+00003450: 0164 0283 017d 037c 036a 027c 0174 037c  .d...}.|.j.|.t.|
+00003460: 006a 0483 017c 00a0 05a1 007c 00a0 06a1  .j...|.....|....
+00003470: 007c 00a0 07a1 007c 00a0 08a1 007c 00a0  .|.....|.....|..
+00003480: 09a1 0064 038d 0753 0029 044e 2901 72a4  ...d...S.).N).r.
+00003490: 0000 0061 6f01 0000 2468 6561 6465 720a  ...ao...$header.
+000034a0: 466f 616d 4669 6c65 0a7b 0a20 2020 2076  FoamFile.{.    v
+000034b0: 6572 7369 6f6e 2020 2020 2032 2e30 3b0a  ersion     2.0;.
+000034c0: 2020 2020 666f 726d 6174 2020 2020 2020      format      
+000034d0: 6173 6369 693b 0a20 2020 2063 6c61 7373  ascii;.    class
+000034e0: 2020 2020 2020 2064 6963 7469 6f6e 6172         dictionar
+000034f0: 793b 0a20 2020 206f 626a 6563 7420 2020  y;.    object   
+00003500: 2020 2062 6c6f 636b 4d65 7368 4469 6374     blockMeshDict
+00003510: 3b0a 7d0a 2f2f 202a 202a 202a 202a 202a  ;.}.// * * * * *
+00003520: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
+00003530: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
+00003540: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
+00003550: 202a 202a 202a 202a 202a 202a 202a 202a   * * * * * * * *
+00003560: 202f 2f0a 0a73 6361 6c65 2020 2024 6d65   //..scale   $me
+00003570: 7472 6963 636f 6e76 6572 743b 0a0a 2476  tricconvert;..$v
+00003580: 6572 7469 6365 730a 0a24 626c 6f63 6b73  ertices..$blocks
+00003590: 0a0a 2465 6467 6573 0a0a 2462 6f75 6e64  ..$edges..$bound
+000035a0: 6172 790a 0a24 6d65 7267 6570 6174 6368  ary..$mergepatch
+000035b0: 7061 6972 730a 0a2f 2f20 2a2a 2a2a 2a2a  pairs..// ******
+000035c0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000035d0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000035e0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000035f0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00003600: 2a2a 2a20 2f2f 0a29 07da 0668 6561 6465  *** //.)...heade
+00003610: 725a 0d6d 6574 7269 6363 6f6e 7665 7274  rZ.metricconvert
+00003620: 723b 0000 0072 6d00 0000 726c 0000 00da  r;...rm...rl....
+00003630: 0862 6f75 6e64 6172 795a 0f6d 6572 6765  .boundaryZ.merge
+00003640: 7061 7463 6870 6169 7273 290a 72a6 0000  patchpairs).r...
+00003650: 0072 0300 0000 da0a 7375 6273 7469 7475  .r......substitu
+00003660: 7465 7236 0000 0072 6b00 0000 72a9 0000  ter6...rk...r...
+00003670: 0072 ac00 0000 72ab 0000 0072 af00 0000  .r....r....r....
+00003680: 72b0 0000 0029 0472 1500 0000 72b1 0000  r....).r....r...
+00003690: 005a 0d73 6f72 745f 766f 7274 6963 6573  .Z.sort_vortices
+000036a0: da08 7465 6d70 6c61 7465 7216 0000 0072  ..templater....r
+000036b0: 1600 0000 7217 0000 0072 2000 0000 8e01  ....r....r .....
+000036c0: 0000 731a 0000 000c 0102 0102 0104 ff04  ..s.............
+000036d0: 1b02 0108 0106 0106 0106 0106 0106 0106  ................
+000036e0: f97a 1442 6c6f 636b 4d65 7368 4469 6374  .z.BlockMeshDict
+000036f0: 2e66 6f72 6d61 7429 034e 4e4e 7269 0000  .format).NNNri..
+00003700: 0029 0154 2918 722a 0000 0072 2b00 0000  .).T).r*...r+...
+00003710: 722c 0000 0072 1800 0000 7279 0000 0072  r,...r....ry...r
+00003720: 7b00 0000 727f 0000 0072 8000 0000 7285  {...r....r....r.
+00003730: 0000 0072 9300 0000 720b 0000 0072 9400  ...r....r....r..
+00003740: 0000 7297 0000 0072 9a00 0000 729b 0000  ..r....r....r...
+00003750: 0072 9f00 0000 72a6 0000 0072 a900 0000  .r....r....r....
+00003760: 72ab 0000 0072 ac00 0000 72af 0000 0072  r....r....r....r
+00003770: b000 0000 7205 0000 0072 2000 0000 7216  ....r....r ...r.
+00003780: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00003790: 0000 726a 0000 00d5 0000 0073 2800 0000  ..rj.......s(...
+000037a0: 0800 0801 0808 080e 0a03 0813 0804 080e  ................
+000037b0: 1410 0805 0805 0a05 0805 0a05 0819 080c  ................
+000037c0: 080b 080c 080f 1206 726a 0000 004e 2916  ........rj...N).
+000037d0: da07 5f5f 646f 635f 5fda 0969 7465 7274  ..__doc__..itert
+000037e0: 6f6f 6c73 7202 0000 00da 0673 7472 696e  oolsr......strin
+000037f0: 6772 0300 0000 da00 7205 0000 0072 6d00  gr......r....rm.
+00003800: 0000 7207 0000 0072 0800 0000 7245 0000  ..r....r....rE..
+00003810: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00003820: 720c 0000 00da 075f 5f61 6c6c 5f5f 720d  r......__all__r.
+00003830: 0000 0072 2e00 0000 7231 0000 0072 4300  ...r....r1...rC.
+00003840: 0000 7260 0000 0072 6a00 0000 7216 0000  ..r`...rj...r...
+00003850: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00003860: da08 3c6d 6f64 756c 653e 0100 0000 731a  ..<module>....s.
+00003870: 0000 0004 000c 0c0c 010c 0210 0118 0108  ................
+00003880: 020e 0a0e 1e0e 0a0e 110e 5612 28         ..........V.(
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/__pycache__/edges.cpython-310.pyc` & `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/edges.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 24 21:00:31 2023 UTC, .py size: 1810 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -32,116 +32,116 @@
 000001f0: 6865 2062 6c6f 636b 0a20 2020 2020 2020  he block.       
 00000200: 2067 7261 6469 6e67 2069 7320 6772 6164   grading is grad
 00000210: 696e 6720 6d65 7468 6f64 2e0a 2020 2020  ing method..    
 00000220: 2020 2020 4e29 03da 0676 6e61 6d65 73da      N)...vnames.
 00000230: 046e 616d 65da 0c69 6e74 6572 5f76 6572  .name..inter_ver
 00000240: 7465 7829 04da 0473 656c 6672 0400 0000  tex)...selfr....
 00000250: 7205 0000 0072 0600 0000 a900 7208 0000  r....r......r...
-00000260: 00fa 582f 686f 6d65 2f70 6965 7272 652f  ..X/home/pierre/
+00000260: 00fa 522f 686f 6d65 2f70 6965 7272 652f  ..R/home/pierre/
 00000270: 4465 762f 666c 7569 6473 696d 666f 616d  Dev/fluidsimfoam
 00000280: 2f73 7263 2f66 6c75 6964 7369 6d66 6f61  /src/fluidsimfoa
 00000290: 6d2f 666f 616d 5f69 6e70 7574 5f66 696c  m/foam_input_fil
-000002a0: 6573 2f62 6c6f 636b 6d65 7368 6865 6c70  es/blockmeshhelp
-000002b0: 6572 2f65 6467 6573 2e70 79da 085f 5f69  er/edges.py..__i
-000002c0: 6e69 745f 5f02 0000 0073 0600 0000 0609  nit__....s......
-000002d0: 0601 0a01 7a10 4172 6345 6467 652e 5f5f  ....z.ArcEdge.__
-000002e0: 696e 6974 5f5f 6302 0000 0000 0000 0000  init__c.........
-000002f0: 0000 0005 0000 000d 0000 0003 0000 0073  ...............s
-00000300: 6400 0000 6401 a000 8700 6601 6402 6403  d...d.....f.d.d.
-00000310: 8408 7c00 6a01 4400 8301 a101 7d02 6401  ..|.j.D.....}.d.
-00000320: a000 7c00 6a01 a101 7d03 7c00 6a02 7d04  ..|.j...}.|.j.}.
-00000330: 6404 7c02 9b00 6405 7c04 6a03 6406 9b04  d.|...d.|.j.d...
-00000340: 6401 7c04 6a04 6406 9b04 6401 7c04 6a05  d.|.j.d...d.|.j.
-00000350: 6406 9b04 6407 7c00 6a06 9b00 6405 7c03  d...d.|.j...d.|.
-00000360: 9b00 6408 9d0d 5300 2909 fa4b 466f 726d  ..d...S.)..KForm
-00000370: 6174 2069 6e73 7461 6e63 6520 746f 2064  at instance to d
-00000380: 756d 700a 2020 2020 2020 2020 7665 7274  ump.        vert
-00000390: 6963 6573 2069 7320 6469 6374 206f 6620  ices is dict of 
-000003a0: 6e61 6d65 2074 6f20 5665 7274 6578 0a20  name to Vertex. 
-000003b0: 2020 2020 2020 20fa 0120 6301 0000 0000         .. c.....
-000003c0: 0000 0000 0000 0002 0000 0004 0000 0033  ...............3
-000003d0: 0000 00f3 1e00 0000 8100 7c00 5d0a 7d01  ..........|.].}.
-000003e0: 7400 8800 7c01 1900 6a01 8301 5600 0100  t...|...j...V...
-000003f0: 7102 6400 5300 a901 4ea9 02da 0373 7472  q.d.S...N....str
-00000400: da05 696e 6465 78a9 02da 022e 30da 0276  ..index.....0..v
-00000410: 6ea9 01da 0876 6572 7469 6365 7372 0800  n....verticesr..
-00000420: 0000 7209 0000 00da 093c 6765 6e65 7870  ..r......<genexp
-00000430: 723e 1300 0000 f304 0000 0002 801c 007a  r>.............z
-00000440: 2141 7263 4564 6765 2e66 6f72 6d61 742e  !ArcEdge.format.
-00000450: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
-00000460: 723e 7a04 6172 6320 fa02 2028 7a06 3138  r>z.arc .. (z.18
-00000470: 2e31 3567 7a05 2920 2f2f 20fa 0129 2907  .15gz.) // ..)).
-00000480: da04 6a6f 696e 7204 0000 0072 0600 0000  ..joinr....r....
-00000490: da01 78da 0179 da01 7a72 0500 0000 2905  ..x..y..zr....).
-000004a0: 7207 0000 0072 1600 0000 7211 0000 00da  r....r....r.....
-000004b0: 0763 6f6d 6d65 6e74 da01 7672 0800 0000  .comment..vr....
-000004c0: 7215 0000 0072 0900 0000 da06 666f 726d  r....r......form
-000004d0: 6174 0f00 0000 7312 0000 001a 040c 0106  at....s.........
-000004e0: 0126 0204 0104 ff02 0106 ff02 ff7a 0e41  .&...........z.A
-000004f0: 7263 4564 6765 2e66 6f72 6d61 744e a905  rcEdge.formatN..
-00000500: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000510: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000520: 6d65 5f5f 720a 0000 0072 2100 0000 7208  me__r....r!...r.
-00000530: 0000 0072 0800 0000 7208 0000 0072 0900  ...r....r....r..
-00000540: 0000 7202 0000 0001 0000 0073 0600 0000  ..r........s....
-00000550: 0800 0801 0c0d 7202 0000 0063 0000 0000  ......r....c....
-00000560: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-00000570: 4000 0000 7201 0000 0029 06da 0a53 706c  @...r....)...Spl
-00000580: 696e 6545 6467 6563 0400 0000 0000 0000  ineEdgec........
-00000590: 0000 0000 0400 0000 0200 0000 4300 0000  ............C...
-000005a0: 7203 0000 0029 027a cd49 6e69 7469 616c  r....).z.Initial
-000005b0: 697a 6520 5370 6c69 6e65 4564 6765 2069  ize SplineEdge i
-000005c0: 6e73 7461 6e63 650a 2020 2020 2020 2020  nstance.        
-000005d0: 766e 616d 6573 2069 7320 7468 6520 7665  vnames is the ve
-000005e0: 7274 6578 206e 616d 6573 2069 6e20 6f72  rtex names in or
-000005f0: 6465 7220 6465 7363 7269 7665 6420 696e  der descrived in
-00000600: 0a20 2020 2020 2020 2020 2068 7474 703a  .          http:
-00000610: 2f2f 7777 772e 6f70 656e 666f 616d 2e6f  //www.openfoam.o
-00000620: 7267 2f64 6f63 732f 7573 6572 2f6d 6573  rg/docs/user/mes
-00000630: 682d 6465 7363 7269 7074 696f 6e2e 7068  h-description.ph
-00000640: 700a 2020 2020 2020 2020 2320 7477 6f20  p.        # two 
-00000650: 7665 7274 6963 6573 2069 7320 6e65 6564  vertices is need
-00000660: 6564 2066 6f72 2053 706c 696e 650a 2020  ed for Spline.  
-00000670: 2020 2020 2020 4e29 0372 0400 0000 7205        N).r....r.
-00000680: 0000 00da 0670 6f69 6e74 7329 0472 0700  .....points).r..
-00000690: 0000 7204 0000 0072 0500 0000 7227 0000  ..r....r....r'..
-000006a0: 0072 0800 0000 7208 0000 0072 0900 0000  .r....r....r....
-000006b0: 720a 0000 001d 0000 0073 0600 0000 0606  r........s......
-000006c0: 0601 0a01 7a13 5370 6c69 6e65 4564 6765  ....z.SplineEdge
-000006d0: 2e5f 5f69 6e69 745f 5f63 0200 0000 0000  .__init__c......
-000006e0: 0000 0000 0000 0600 0000 0900 0000 0300  ................
-000006f0: 0000 7386 0000 0064 01a0 0087 0066 0164  ..s....d.....f.d
-00000700: 0264 0384 087c 006a 0144 0083 01a1 017d  .d...|.j.D.....}
-00000710: 0264 01a0 007c 006a 01a1 017d 0367 007d  .d...|.j...}.g.}
-00000720: 047c 04a0 0264 047c 029b 0064 057c 006a  .|...d.|...d.|.j
-00000730: 039b 0064 067c 039b 0064 079d 07a1 0101  ...d.|...d......
-00000740: 007c 04a0 0264 08a1 0101 007c 006a 0444  .|...d.....|.j.D
-00000750: 005d 0b7d 057c 04a0 0264 097c 05a0 05a1  .].}.|...d.|....
-00000760: 0017 00a1 0101 0071 2d7c 04a0 0264 07a1  .......q-|...d..
-00000770: 0101 0064 0aa0 007c 04a1 0153 0029 0b72  ...d...|...S.).r
-00000780: 0b00 0000 720c 0000 0063 0100 0000 0000  ....r....c......
-00000790: 0000 0000 0000 0200 0000 0400 0000 3300  ..............3.
-000007a0: 0000 720d 0000 0072 0e00 0000 720f 0000  ..r....r....r...
-000007b0: 0072 1200 0000 7215 0000 0072 0800 0000  .r....r....r....
-000007c0: 7209 0000 0072 1700 0000 2b00 0000 7218  r....r....+...r.
-000007d0: 0000 007a 2453 706c 696e 6545 6467 652e  ...z$SplineEdge.
-000007e0: 666f 726d 6174 2e3c 6c6f 6361 6c73 3e2e  format.<locals>.
-000007f0: 3c67 656e 6578 7072 3e7a 0773 706c 696e  <genexpr>z.splin
-00000800: 6520 7a19 2020 2020 2020 2020 2020 2020  e z.            
-00000810: 2020 2020 2020 2020 2020 2f2f 2072 1900            // r..
-00000820: 0000 721a 0000 007a 0520 2020 2028 7a09  ..r....z.    (z.
-00000830: 2020 2020 2020 2020 20da 010a 2906 721b           ...).r.
-00000840: 0000 0072 0400 0000 da06 6170 7065 6e64  ...r......append
-00000850: 7205 0000 0072 2700 0000 7221 0000 0029  r....r'...r!...)
-00000860: 0672 0700 0000 7216 0000 0072 1100 0000  .r....r....r....
-00000870: 721f 0000 00da 0374 6d70 da01 7072 0800  r......tmp..pr..
-00000880: 0000 7215 0000 0072 0900 0000 7221 0000  ..r....r....r!..
-00000890: 0027 0000 0073 1600 0000 1a04 0c01 0401  .'...s..........
-000008a0: 0401 1801 04ff 0a03 0a01 1401 0a01 0a01  ................
-000008b0: 7a11 5370 6c69 6e65 4564 6765 2e66 6f72  z.SplineEdge.for
-000008c0: 6d61 744e 7222 0000 0072 0800 0000 7208  matNr"...r....r.
-000008d0: 0000 0072 0800 0000 7209 0000 0072 2600  ...r....r....r&.
-000008e0: 0000 1c00 0000 7306 0000 0008 0008 010c  ......s.........
-000008f0: 0a72 2600 0000 4e29 0272 0200 0000 7226  .r&...N).r....r&
-00000900: 0000 0072 0800 0000 7208 0000 0072 0800  ...r....r....r..
-00000910: 0000 7209 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000920: 3e01 0000 0073 0400 0000 0e00 121b       >....s........
+000002a0: 6573 2f62 6c6f 636b 6d65 7368 2f65 6467  es/blockmesh/edg
+000002b0: 6573 2e70 79da 085f 5f69 6e69 745f 5f02  es.py..__init__.
+000002c0: 0000 0073 0600 0000 0609 0601 0a01 7a10  ...s..........z.
+000002d0: 4172 6345 6467 652e 5f5f 696e 6974 5f5f  ArcEdge.__init__
+000002e0: 6302 0000 0000 0000 0000 0000 0005 0000  c...............
+000002f0: 000d 0000 0003 0000 0073 6400 0000 6401  .........sd...d.
+00000300: a000 8700 6601 6402 6403 8408 7c00 6a01  ....f.d.d...|.j.
+00000310: 4400 8301 a101 7d02 6401 a000 7c00 6a01  D.....}.d...|.j.
+00000320: a101 7d03 7c00 6a02 7d04 6404 7c02 9b00  ..}.|.j.}.d.|...
+00000330: 6405 7c04 6a03 6406 9b04 6401 7c04 6a04  d.|.j.d...d.|.j.
+00000340: 6406 9b04 6401 7c04 6a05 6406 9b04 6407  d...d.|.j.d...d.
+00000350: 7c00 6a06 9b00 6405 7c03 9b00 6408 9d0d  |.j...d.|...d...
+00000360: 5300 2909 fa4b 466f 726d 6174 2069 6e73  S.)..KFormat ins
+00000370: 7461 6e63 6520 746f 2064 756d 700a 2020  tance to dump.  
+00000380: 2020 2020 2020 7665 7274 6963 6573 2069        vertices i
+00000390: 7320 6469 6374 206f 6620 6e61 6d65 2074  s dict of name t
+000003a0: 6f20 5665 7274 6578 0a20 2020 2020 2020  o Vertex.       
+000003b0: 20fa 0120 6301 0000 0000 0000 0000 0000   .. c...........
+000003c0: 0002 0000 0004 0000 0033 0000 00f3 1e00  .........3......
+000003d0: 0000 8100 7c00 5d0a 7d01 7400 8800 7c01  ....|.].}.t...|.
+000003e0: 1900 6a01 8301 5600 0100 7102 6400 5300  ..j...V...q.d.S.
+000003f0: a901 4ea9 02da 0373 7472 da05 696e 6465  ..N....str..inde
+00000400: 78a9 02da 022e 30da 0276 6ea9 01da 0876  x.....0..vn....v
+00000410: 6572 7469 6365 7372 0800 0000 7209 0000  erticesr....r...
+00000420: 00da 093c 6765 6e65 7870 723e 1300 0000  ...<genexpr>....
+00000430: f304 0000 0002 801c 007a 2141 7263 4564  .........z!ArcEd
+00000440: 6765 2e66 6f72 6d61 742e 3c6c 6f63 616c  ge.format.<local
+00000450: 733e 2e3c 6765 6e65 7870 723e 7a04 6172  s>.<genexpr>z.ar
+00000460: 6320 fa02 2028 7a06 3138 2e31 3567 7a05  c .. (z.18.15gz.
+00000470: 2920 2f2f 20fa 0129 2907 da04 6a6f 696e  ) // ..))...join
+00000480: 7204 0000 0072 0600 0000 da01 78da 0179  r....r......x..y
+00000490: da01 7a72 0500 0000 2905 7207 0000 0072  ..zr....).r....r
+000004a0: 1600 0000 7211 0000 00da 0763 6f6d 6d65  ....r......comme
+000004b0: 6e74 da01 7672 0800 0000 7215 0000 0072  nt..vr....r....r
+000004c0: 0900 0000 da06 666f 726d 6174 0f00 0000  ......format....
+000004d0: 7312 0000 001a 040c 0106 0126 0204 0104  s..........&....
+000004e0: ff02 0106 ff02 ff7a 0e41 7263 4564 6765  .......z.ArcEdge
+000004f0: 2e66 6f72 6d61 744e a905 da08 5f5f 6e61  .formatN....__na
+00000500: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000510: da0c 5f5f 7175 616c 6e61 6d65 5f5f 720a  ..__qualname__r.
+00000520: 0000 0072 2100 0000 7208 0000 0072 0800  ...r!...r....r..
+00000530: 0000 7208 0000 0072 0900 0000 7202 0000  ..r....r....r...
+00000540: 0001 0000 0073 0600 0000 0800 0801 0c0d  .....s..........
+00000550: 7202 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000560: 0000 0000 0000 0200 0000 4000 0000 7201  ..........@...r.
+00000570: 0000 0029 06da 0a53 706c 696e 6545 6467  ...)...SplineEdg
+00000580: 6563 0400 0000 0000 0000 0000 0000 0400  ec..............
+00000590: 0000 0200 0000 4300 0000 7203 0000 0029  ......C...r....)
+000005a0: 027a cd49 6e69 7469 616c 697a 6520 5370  .z.Initialize Sp
+000005b0: 6c69 6e65 4564 6765 2069 6e73 7461 6e63  lineEdge instanc
+000005c0: 650a 2020 2020 2020 2020 766e 616d 6573  e.        vnames
+000005d0: 2069 7320 7468 6520 7665 7274 6578 206e   is the vertex n
+000005e0: 616d 6573 2069 6e20 6f72 6465 7220 6465  ames in order de
+000005f0: 7363 7269 7665 6420 696e 0a20 2020 2020  scrived in.     
+00000600: 2020 2020 2068 7474 703a 2f2f 7777 772e       http://www.
+00000610: 6f70 656e 666f 616d 2e6f 7267 2f64 6f63  openfoam.org/doc
+00000620: 732f 7573 6572 2f6d 6573 682d 6465 7363  s/user/mesh-desc
+00000630: 7269 7074 696f 6e2e 7068 700a 2020 2020  ription.php.    
+00000640: 2020 2020 2320 7477 6f20 7665 7274 6963      # two vertic
+00000650: 6573 2069 7320 6e65 6564 6564 2066 6f72  es is needed for
+00000660: 2053 706c 696e 650a 2020 2020 2020 2020   Spline.        
+00000670: 4e29 0372 0400 0000 7205 0000 00da 0670  N).r....r......p
+00000680: 6f69 6e74 7329 0472 0700 0000 7204 0000  oints).r....r...
+00000690: 0072 0500 0000 7227 0000 0072 0800 0000  .r....r'...r....
+000006a0: 7208 0000 0072 0900 0000 720a 0000 001d  r....r....r.....
+000006b0: 0000 0073 0600 0000 0606 0601 0a01 7a13  ...s..........z.
+000006c0: 5370 6c69 6e65 4564 6765 2e5f 5f69 6e69  SplineEdge.__ini
+000006d0: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
+000006e0: 0600 0000 0900 0000 0300 0000 7386 0000  ............s...
+000006f0: 0064 01a0 0087 0066 0164 0264 0384 087c  .d.....f.d.d...|
+00000700: 006a 0144 0083 01a1 017d 0264 01a0 007c  .j.D.....}.d...|
+00000710: 006a 01a1 017d 0367 007d 047c 04a0 0264  .j...}.g.}.|...d
+00000720: 047c 029b 0064 057c 006a 039b 0064 067c  .|...d.|.j...d.|
+00000730: 039b 0064 079d 07a1 0101 007c 04a0 0264  ...d.......|...d
+00000740: 08a1 0101 007c 006a 0444 005d 0b7d 057c  .....|.j.D.].}.|
+00000750: 04a0 0264 097c 05a0 05a1 0017 00a1 0101  ...d.|..........
+00000760: 0071 2d7c 04a0 0264 07a1 0101 0064 0aa0  .q-|...d.....d..
+00000770: 007c 04a1 0153 0029 0b72 0b00 0000 720c  .|...S.).r....r.
+00000780: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000790: 0200 0000 0400 0000 3300 0000 720d 0000  ........3...r...
+000007a0: 0072 0e00 0000 720f 0000 0072 1200 0000  .r....r....r....
+000007b0: 7215 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
+000007c0: 1700 0000 2b00 0000 7218 0000 007a 2453  ....+...r....z$S
+000007d0: 706c 696e 6545 6467 652e 666f 726d 6174  plineEdge.format
+000007e0: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
+000007f0: 7072 3e7a 0773 706c 696e 6520 7a19 2020  pr>z.spline z.  
+00000800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000810: 2020 2020 2f2f 2072 1900 0000 721a 0000      // r....r...
+00000820: 007a 0520 2020 2028 7a09 2020 2020 2020  .z.    (z.      
+00000830: 2020 20da 010a 2906 721b 0000 0072 0400     ...).r....r..
+00000840: 0000 da06 6170 7065 6e64 7205 0000 0072  ....appendr....r
+00000850: 2700 0000 7221 0000 0029 0672 0700 0000  '...r!...).r....
+00000860: 7216 0000 0072 1100 0000 721f 0000 00da  r....r....r.....
+00000870: 0374 6d70 da01 7072 0800 0000 7215 0000  .tmp..pr....r...
+00000880: 0072 0900 0000 7221 0000 0027 0000 0073  .r....r!...'...s
+00000890: 1600 0000 1a04 0c01 0401 0401 1801 04ff  ................
+000008a0: 0a03 0a01 1401 0a01 0a01 7a11 5370 6c69  ..........z.Spli
+000008b0: 6e65 4564 6765 2e66 6f72 6d61 744e 7222  neEdge.formatNr"
+000008c0: 0000 0072 0800 0000 7208 0000 0072 0800  ...r....r....r..
+000008d0: 0000 7209 0000 0072 2600 0000 1c00 0000  ..r....r&.......
+000008e0: 7306 0000 0008 0008 010c 0a72 2600 0000  s..........r&...
+000008f0: 4e29 0272 0200 0000 7226 0000 0072 0800  N).r....r&...r..
+00000900: 0000 7208 0000 0072 0800 0000 7209 0000  ..r....r....r...
+00000910: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000920: 0400 0000 0e00 121b                      ........
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/__pycache__/grading.cpython-310.pyc` & `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/grading.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 24 20:58:16 2023 UTC, .py size: 3426 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -14,181 +14,180 @@
 000000d0: 5300 2903 da07 4772 6164 696e 677a 2862  S.)...Gradingz(b
 000000e0: 6173 6520 636c 6173 7320 666f 7220 5369  ase class for Si
 000000f0: 6d70 6c65 2d20 616e 6420 4564 6765 2d20  mple- and Edge- 
 00000100: 4772 6164 696e 674e 2904 da08 5f5f 6e61  GradingN)...__na
 00000110: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
 00000120: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
 00000130: 5f5f 646f 635f 5fa9 0072 0900 0000 7209  __doc__..r....r.
-00000140: 0000 00fa 5a2f 686f 6d65 2f70 6965 7272  ....Z/home/pierr
+00000140: 0000 00fa 542f 686f 6d65 2f70 6965 7272  ....T/home/pierr
 00000150: 652f 4465 762f 666c 7569 6473 696d 666f  e/Dev/fluidsimfo
 00000160: 616d 2f73 7263 2f66 6c75 6964 7369 6d66  am/src/fluidsimf
 00000170: 6f61 6d2f 666f 616d 5f69 6e70 7574 5f66  oam/foam_input_f
-00000180: 696c 6573 2f62 6c6f 636b 6d65 7368 6865  iles/blockmeshhe
-00000190: 6c70 6572 2f67 7261 6469 6e67 2e70 7972  lper/grading.pyr
-000001a0: 0400 0000 0500 0000 7304 0000 0008 0008  ........s.......
-000001b0: 0172 0400 0000 6300 0000 0000 0000 0000  .r....c.........
-000001c0: 0000 0000 0000 0002 0000 0040 0000 00f3  ...........@....
-000001d0: 2000 0000 6500 5a01 6400 5a02 6401 5a03   ...e.Z.d.Z.d.Z.
-000001e0: 6402 6403 8400 5a04 6404 6405 8400 5a05  d.d...Z.d.d...Z.
-000001f0: 6406 5300 2907 da14 5369 6d70 6c65 4772  d.S.)...SimpleGr
-00000200: 6164 696e 6745 6c65 6d65 6e74 7a3c 782c  adingElementz<x,
-00000210: 2079 206f 7220 7a20 456c 656d 656e 7420   y or z Element 
-00000220: 6f66 2073 696d 706c 6547 7261 6469 6e67  of simpleGrading
-00000230: 2e20 6164 6f70 7465 6420 746f 206d 756c  . adopted to mul
-00000240: 7469 2d67 7261 6469 6e67 6302 0000 0000  ti-gradingc.....
-00000250: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
-00000260: 0000 0073 0a00 0000 7c01 7c00 5f00 6401  ...s....|.|._.d.
-00000270: 5300 2902 7a9b 696e 6974 6961 6c69 7a61  S.).z.initializa
-00000280: 7469 6f6e 0a20 2020 2020 2020 2064 2069  tion.        d i
-00000290: 7320 7369 6e67 6c65 206e 756d 6265 7220  s single number 
-000002a0: 666f 7220 6578 7061 6e73 696f 6e20 7261  for expansion ra
-000002b0: 7469 6f0a 2020 2020 2020 2020 2020 6f72  tio.          or
-000002c0: 2069 7465 7261 7469 7665 206f 626a 6563   iterative objec
-000002d0: 7420 636f 6e73 6974 7320 2864 6972 6563  t consits (direc
-000002e0: 7469 6f6e 2072 6174 696f 2c20 6365 6c6c  tion ratio, cell
-000002f0: 2072 6174 696f 2c20 6578 7061 6e73 696f   ratio, expansio
-00000300: 6e20 7261 7469 6f29 0a20 2020 2020 2020  n ratio).       
-00000310: 204e 2901 da01 6429 02da 0473 656c 6672   N)...d)...selfr
-00000320: 0d00 0000 7209 0000 0072 0900 0000 720a  ....r....r....r.
-00000330: 0000 00da 085f 5f69 6e69 745f 5f0c 0000  .....__init__...
-00000340: 0073 0200 0000 0a05 7a1d 5369 6d70 6c65  .s......z.Simple
-00000350: 4772 6164 696e 6745 6c65 6d65 6e74 2e5f  GradingElement._
-00000360: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-00000370: 0000 0000 0100 0000 0500 0000 4300 0000  ............C...
-00000380: 7334 0000 0074 007c 006a 0174 0283 0272  s4...t.|.j.t...r
-00000390: 1564 0164 02a0 0364 0364 0484 007c 006a  .d.d...d.d...|.j
-000003a0: 0144 0083 01a1 0117 0064 0517 0053 0074  .D.......d...S.t
-000003b0: 047c 006a 0183 0153 0029 064e fa02 2820  .|.j...S.).N..( 
-000003c0: fa01 2063 0100 0000 0000 0000 0000 0000  .. c............
-000003d0: 0200 0000 0800 0000 7300 0000 733a 0000  ........s...s:..
-000003e0: 0081 007c 005d 187d 0164 007c 0164 0119  ...|.].}.d.|.d..
-000003f0: 0064 029b 0464 037c 0164 0419 0064 029b  .d...d.|.d...d..
-00000400: 0464 037c 0164 0519 0064 029b 0464 069d  .d.|.d...d...d..
-00000410: 0756 0001 0071 0264 0753 0029 0872 1000  .V...q.d.S.).r..
-00000420: 0000 7201 0000 00da 0167 7211 0000 00e9  ..r......gr.....
-00000430: 0100 0000 e902 0000 00fa 0220 294e 7209  ........... )Nr.
-00000440: 0000 0029 02da 022e 30da 0165 7209 0000  ...)....0..er...
-00000450: 0072 0900 0000 720a 0000 00da 093c 6765  .r....r......<ge
-00000460: 6e65 7870 723e 1700 0000 7304 0000 0002  nexpr>....s.....
-00000470: 8038 007a 2e53 696d 706c 6547 7261 6469  .8.z.SimpleGradi
-00000480: 6e67 456c 656d 656e 742e 666f 726d 6174  ngElement.format
-00000490: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
-000004a0: 7072 3e72 1500 0000 2905 da0a 6973 696e  pr>r....)...isin
-000004b0: 7374 616e 6365 720d 0000 0072 0200 0000  stancer....r....
-000004c0: da04 6a6f 696e da03 7374 72a9 0172 0e00  ..join..str..r..
-000004d0: 0000 7209 0000 0072 0900 0000 720a 0000  ..r....r....r...
-000004e0: 00da 0666 6f72 6d61 7413 0000 0073 1000  ...format....s..
-000004f0: 0000 0c01 0202 1401 02ff 0202 02fe 02ff  ................
-00000500: 0a06 7a1b 5369 6d70 6c65 4772 6164 696e  ..z.SimpleGradin
-00000510: 6745 6c65 6d65 6e74 2e66 6f72 6d61 744e  gElement.formatN
-00000520: a906 7205 0000 0072 0600 0000 7207 0000  ..r....r....r...
-00000530: 0072 0800 0000 720f 0000 0072 1d00 0000  .r....r....r....
-00000540: 7209 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
-00000550: 0a00 0000 720c 0000 0009 0000 0073 0800  ....r........s..
-00000560: 0000 0800 0401 0802 0c07 720c 0000 0063  ..........r....c
-00000570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000580: 0200 0000 4000 0000 720b 0000 0029 07da  ....@...r....)..
-00000590: 0d53 696d 706c 6547 7261 6469 6e67 7a21  .SimpleGradingz!
-000005a0: 636f 6e66 6967 7574 6174 696f 6e20 666f  configutation fo
-000005b0: 7220 2773 696d 706c 6547 7261 6469 6e67  r 'simpleGrading
-000005c0: 2763 0400 0000 0000 0000 0000 0000 0400  'c..............
-000005d0: 0000 0300 0000 4300 0000 735a 0000 0074  ......C...sZ...t
-000005e0: 007c 0174 0183 0273 0b74 017c 0183 017c  .|.t...s.t.|...|
-000005f0: 005f 026e 037c 017c 005f 0274 007c 0274  ._.n.|.|._.t.|.t
-00000600: 0183 0273 1974 017c 0283 017c 005f 036e  ...s.t.|...|._.n
-00000610: 037c 027c 005f 0374 007c 0374 0183 0273  .|.|._.t.|.t...s
-00000620: 2874 017c 0383 017c 005f 0464 0053 007c  (t.|...|._.d.S.|
-00000630: 037c 005f 0464 0053 00a9 014e 2905 7219  .|._.d.S...N).r.
-00000640: 0000 0072 0c00 0000 da01 78da 0179 da01  ...r......x..y..
-00000650: 7a29 0472 0e00 0000 7221 0000 0072 2200  z).r....r!...r".
-00000660: 0000 7223 0000 0072 0900 0000 7209 0000  ..r#...r....r...
-00000670: 0072 0a00 0000 720f 0000 0021 0000 0073  .r....r....!...s
-00000680: 1200 0000 0a01 0c01 0602 0a01 0c01 0602  ................
-00000690: 0a01 0e01 0a02 7a16 5369 6d70 6c65 4772  ......z.SimpleGr
-000006a0: 6164 696e 672e 5f5f 696e 6974 5f5f 6301  ading.__init__c.
-000006b0: 0000 0000 0000 0000 0000 0001 0000 0007  ................
-000006c0: 0000 0043 0000 0073 2a00 0000 6401 7c00  ...C...s*...d.|.
-000006d0: 6a00 a001 a100 9b00 6402 7c00 6a02 a001  j.......d.|.j...
-000006e0: a100 9b00 6402 7c00 6a03 a001 a100 9b00  ....d.|.j.......
-000006f0: 6403 9d07 5300 2904 4e7a 0f73 696d 706c  d...S.).Nz.simpl
-00000700: 6547 7261 6469 6e67 2028 7211 0000 00fa  eGrading (r.....
-00000710: 0129 2904 7221 0000 0072 1d00 0000 7222  .)).r!...r....r"
-00000720: 0000 0072 2300 0000 721c 0000 0072 0900  ...r#...r....r..
-00000730: 0000 7209 0000 0072 0a00 0000 721d 0000  ..r....r....r...
-00000740: 002f 0000 0073 1000 0000 0202 0801 04ff  ./...s..........
-00000750: 0801 04ff 0801 06ff 02ff 7a14 5369 6d70  ..........z.Simp
-00000760: 6c65 4772 6164 696e 672e 666f 726d 6174  leGrading.format
-00000770: 4e72 1e00 0000 7209 0000 0072 0900 0000  Nr....r....r....
-00000780: 7209 0000 0072 0a00 0000 721f 0000 001e  r....r....r.....
-00000790: 0000 0073 0800 0000 0800 0401 0802 0c0e  ...s............
-000007a0: 721f 0000 0063 0000 0000 0000 0000 0000  r....c..........
-000007b0: 0000 0000 0000 0200 0000 4000 0000 720b  ..........@...r.
-000007c0: 0000 0029 07da 0b45 6467 6547 7261 6469  ...)...EdgeGradi
-000007d0: 6e67 7a1f 636f 6e66 6967 7574 6174 696f  ngz.configutatio
-000007e0: 6e20 666f 7220 2765 6467 6547 7261 6469  n for 'edgeGradi
-000007f0: 6e67 2763 0d00 0000 0000 0000 0000 0000  ng'c............
-00000800: 0d00 0000 0300 0000 4300 0000 7356 0100  ........C...sV..
-00000810: 0074 007c 0174 0183 0273 0b74 017c 0183  .t.|.t...s.t.|..
-00000820: 017c 005f 026e 037c 017c 005f 0274 007c  .|._.n.|.|._.t.|
-00000830: 0274 0183 0273 1974 017c 0283 017c 005f  .t...s.t.|...|._
-00000840: 036e 037c 027c 005f 0374 007c 0374 0183  .n.|.|._.t.|.t..
-00000850: 0273 2774 017c 0383 017c 005f 046e 037c  .s't.|...|._.n.|
-00000860: 037c 005f 0474 007c 0474 0183 0273 3574  .|._.t.|.t...s5t
-00000870: 017c 0483 017c 005f 056e 037c 047c 005f  .|...|._.n.|.|._
-00000880: 0574 007c 0574 0183 0273 4374 017c 0583  .t.|.t...sCt.|..
-00000890: 017c 005f 066e 037c 057c 005f 0674 007c  .|._.n.|.|._.t.|
-000008a0: 0674 0183 0273 5174 017c 0683 017c 005f  .t...sQt.|...|._
-000008b0: 076e 037c 067c 005f 0774 007c 0774 0183  .n.|.|._.t.|.t..
-000008c0: 0273 5f74 017c 0783 017c 005f 086e 037c  .s_t.|...|._.n.|
-000008d0: 077c 005f 0874 007c 0874 0183 0273 6d74  .|._.t.|.t...smt
-000008e0: 017c 0883 017c 005f 096e 037c 087c 005f  .|...|._.n.|.|._
-000008f0: 0974 007c 0174 0183 0273 7b74 017c 0983  .t.|.t...s{t.|..
-00000900: 017c 005f 0a6e 037c 097c 005f 0a74 007c  .|._.n.|.|._.t.|
-00000910: 0a74 0183 0273 8974 017c 0a83 017c 005f  .t...s.t.|...|._
-00000920: 0b6e 037c 0a7c 005f 0b74 007c 0b74 0183  .n.|.|._.t.|.t..
-00000930: 0273 9774 017c 0b83 017c 005f 0c6e 037c  .s.t.|...|._.n.|
-00000940: 0b7c 005f 0c74 007c 0c74 0183 0273 a674  .|._.t.|.t...s.t
-00000950: 017c 0c83 017c 005f 0d64 0053 007c 0c7c  .|...|._.d.S.|.|
-00000960: 005f 0d64 0053 0072 2000 0000 290e 7219  ._.d.S.r ...).r.
-00000970: 0000 0072 0c00 0000 da02 7831 da02 7832  ...r......x1..x2
-00000980: da02 7833 da02 7834 da02 7931 da02 7932  ..x3..x4..y1..y2
-00000990: da02 7933 da02 7934 da02 7a31 da02 7a32  ..y3..y4..z1..z2
-000009a0: da02 7a33 da02 7a34 290d 720e 0000 0072  ..z3..z4).r....r
-000009b0: 2600 0000 7227 0000 0072 2800 0000 7229  &...r'...r(...r)
-000009c0: 0000 0072 2a00 0000 722b 0000 0072 2c00  ...r*...r+...r,.
-000009d0: 0000 722d 0000 0072 2e00 0000 722f 0000  ..r-...r....r/..
-000009e0: 0072 3000 0000 7231 0000 0072 0900 0000  .r0...r1...r....
-000009f0: 7209 0000 0072 0a00 0000 720f 0000 0039  r....r....r....9
-00000a00: 0000 0073 4800 0000 0a01 0c01 0602 0a01  ...sH...........
+00000180: 696c 6573 2f62 6c6f 636b 6d65 7368 2f67  iles/blockmesh/g
+00000190: 7261 6469 6e67 2e70 7972 0400 0000 0500  rading.pyr......
+000001a0: 0000 7304 0000 0008 0008 0172 0400 0000  ..s........r....
+000001b0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000001c0: 0002 0000 0040 0000 00f3 2000 0000 6500  .....@.... ...e.
+000001d0: 5a01 6400 5a02 6401 5a03 6402 6403 8400  Z.d.Z.d.Z.d.d...
+000001e0: 5a04 6404 6405 8400 5a05 6406 5300 2907  Z.d.d...Z.d.S.).
+000001f0: da14 5369 6d70 6c65 4772 6164 696e 6745  ..SimpleGradingE
+00000200: 6c65 6d65 6e74 7a3c 782c 2079 206f 7220  lementz<x, y or 
+00000210: 7a20 456c 656d 656e 7420 6f66 2073 696d  z Element of sim
+00000220: 706c 6547 7261 6469 6e67 2e20 6164 6f70  pleGrading. adop
+00000230: 7465 6420 746f 206d 756c 7469 2d67 7261  ted to multi-gra
+00000240: 6469 6e67 6302 0000 0000 0000 0000 0000  dingc...........
+00000250: 0002 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
+00000260: 0000 7c01 7c00 5f00 6401 5300 2902 7a9b  ..|.|._.d.S.).z.
+00000270: 696e 6974 6961 6c69 7a61 7469 6f6e 0a20  initialization. 
+00000280: 2020 2020 2020 2064 2069 7320 7369 6e67         d is sing
+00000290: 6c65 206e 756d 6265 7220 666f 7220 6578  le number for ex
+000002a0: 7061 6e73 696f 6e20 7261 7469 6f0a 2020  pansion ratio.  
+000002b0: 2020 2020 2020 2020 6f72 2069 7465 7261          or itera
+000002c0: 7469 7665 206f 626a 6563 7420 636f 6e73  tive object cons
+000002d0: 6974 7320 2864 6972 6563 7469 6f6e 2072  its (direction r
+000002e0: 6174 696f 2c20 6365 6c6c 2072 6174 696f  atio, cell ratio
+000002f0: 2c20 6578 7061 6e73 696f 6e20 7261 7469  , expansion rati
+00000300: 6f29 0a20 2020 2020 2020 204e 2901 da01  o).        N)...
+00000310: 6429 02da 0473 656c 6672 0d00 0000 7209  d)...selfr....r.
+00000320: 0000 0072 0900 0000 720a 0000 00da 085f  ...r....r......_
+00000330: 5f69 6e69 745f 5f0c 0000 0073 0200 0000  _init__....s....
+00000340: 0a05 7a1d 5369 6d70 6c65 4772 6164 696e  ..z.SimpleGradin
+00000350: 6745 6c65 6d65 6e74 2e5f 5f69 6e69 745f  gElement.__init_
+00000360: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+00000370: 0000 0500 0000 4300 0000 7334 0000 0074  ......C...s4...t
+00000380: 007c 006a 0174 0283 0272 1564 0164 02a0  .|.j.t...r.d.d..
+00000390: 0364 0364 0484 007c 006a 0144 0083 01a1  .d.d...|.j.D....
+000003a0: 0117 0064 0517 0053 0074 047c 006a 0183  ...d...S.t.|.j..
+000003b0: 0153 0029 064e fa02 2820 fa01 2063 0100  .S.).N..( .. c..
+000003c0: 0000 0000 0000 0000 0000 0200 0000 0800  ................
+000003d0: 0000 7300 0000 733a 0000 0081 007c 005d  ..s...s:.....|.]
+000003e0: 187d 0164 007c 0164 0119 0064 029b 0464  .}.d.|.d...d...d
+000003f0: 037c 0164 0419 0064 029b 0464 037c 0164  .|.d...d...d.|.d
+00000400: 0519 0064 029b 0464 069d 0756 0001 0071  ...d...d...V...q
+00000410: 0264 0753 0029 0872 1000 0000 7201 0000  .d.S.).r....r...
+00000420: 00da 0167 7211 0000 00e9 0100 0000 e902  ...gr...........
+00000430: 0000 00fa 0220 294e 7209 0000 0029 02da  ..... )Nr....)..
+00000440: 022e 30da 0165 7209 0000 0072 0900 0000  ..0..er....r....
+00000450: 720a 0000 00da 093c 6765 6e65 7870 723e  r......<genexpr>
+00000460: 1700 0000 7304 0000 0002 8038 007a 2e53  ....s......8.z.S
+00000470: 696d 706c 6547 7261 6469 6e67 456c 656d  impleGradingElem
+00000480: 656e 742e 666f 726d 6174 2e3c 6c6f 6361  ent.format.<loca
+00000490: 6c73 3e2e 3c67 656e 6578 7072 3e72 1500  ls>.<genexpr>r..
+000004a0: 0000 2905 da0a 6973 696e 7374 616e 6365  ..)...isinstance
+000004b0: 720d 0000 0072 0200 0000 da04 6a6f 696e  r....r......join
+000004c0: da03 7374 72a9 0172 0e00 0000 7209 0000  ..str..r....r...
+000004d0: 0072 0900 0000 720a 0000 00da 0666 6f72  .r....r......for
+000004e0: 6d61 7413 0000 0073 1000 0000 0c01 0202  mat....s........
+000004f0: 1401 02ff 0202 02fe 02ff 0a06 7a1b 5369  ............z.Si
+00000500: 6d70 6c65 4772 6164 696e 6745 6c65 6d65  mpleGradingEleme
+00000510: 6e74 2e66 6f72 6d61 744e a906 7205 0000  nt.formatN..r...
+00000520: 0072 0600 0000 7207 0000 0072 0800 0000  .r....r....r....
+00000530: 720f 0000 0072 1d00 0000 7209 0000 0072  r....r....r....r
+00000540: 0900 0000 7209 0000 0072 0a00 0000 720c  ....r....r....r.
+00000550: 0000 0009 0000 0073 0800 0000 0800 0401  .......s........
+00000560: 0802 0c07 720c 0000 0063 0000 0000 0000  ....r....c......
+00000570: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
+00000580: 0000 720b 0000 0029 07da 0d53 696d 706c  ..r....)...Simpl
+00000590: 6547 7261 6469 6e67 7a21 636f 6e66 6967  eGradingz!config
+000005a0: 7574 6174 696f 6e20 666f 7220 2773 696d  utation for 'sim
+000005b0: 706c 6547 7261 6469 6e67 2763 0400 0000  pleGrading'c....
+000005c0: 0000 0000 0000 0000 0400 0000 0300 0000  ................
+000005d0: 4300 0000 735a 0000 0074 007c 0174 0183  C...sZ...t.|.t..
+000005e0: 0273 0b74 017c 0183 017c 005f 026e 037c  .s.t.|...|._.n.|
+000005f0: 017c 005f 0274 007c 0274 0183 0273 1974  .|._.t.|.t...s.t
+00000600: 017c 0283 017c 005f 036e 037c 027c 005f  .|...|._.n.|.|._
+00000610: 0374 007c 0374 0183 0273 2874 017c 0383  .t.|.t...s(t.|..
+00000620: 017c 005f 0464 0053 007c 037c 005f 0464  .|._.d.S.|.|._.d
+00000630: 0053 00a9 014e 2905 7219 0000 0072 0c00  .S...N).r....r..
+00000640: 0000 da01 78da 0179 da01 7a29 0472 0e00  ....x..y..z).r..
+00000650: 0000 7221 0000 0072 2200 0000 7223 0000  ..r!...r"...r#..
+00000660: 0072 0900 0000 7209 0000 0072 0a00 0000  .r....r....r....
+00000670: 720f 0000 0021 0000 0073 1200 0000 0a01  r....!...s......
+00000680: 0c01 0602 0a01 0c01 0602 0a01 0e01 0a02  ................
+00000690: 7a16 5369 6d70 6c65 4772 6164 696e 672e  z.SimpleGrading.
+000006a0: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
+000006b0: 0000 0000 0001 0000 0007 0000 0043 0000  .............C..
+000006c0: 0073 2a00 0000 6401 7c00 6a00 a001 a100  .s*...d.|.j.....
+000006d0: 9b00 6402 7c00 6a02 a001 a100 9b00 6402  ..d.|.j.......d.
+000006e0: 7c00 6a03 a001 a100 9b00 6403 9d07 5300  |.j.......d...S.
+000006f0: 2904 4e7a 0f73 696d 706c 6547 7261 6469  ).Nz.simpleGradi
+00000700: 6e67 2028 7211 0000 00fa 0129 2904 7221  ng (r......)).r!
+00000710: 0000 0072 1d00 0000 7222 0000 0072 2300  ...r....r"...r#.
+00000720: 0000 721c 0000 0072 0900 0000 7209 0000  ..r....r....r...
+00000730: 0072 0a00 0000 721d 0000 002f 0000 0073  .r....r..../...s
+00000740: 1000 0000 0202 0801 04ff 0801 04ff 0801  ................
+00000750: 06ff 02ff 7a14 5369 6d70 6c65 4772 6164  ....z.SimpleGrad
+00000760: 696e 672e 666f 726d 6174 4e72 1e00 0000  ing.formatNr....
+00000770: 7209 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
+00000780: 0a00 0000 721f 0000 001e 0000 0073 0800  ....r........s..
+00000790: 0000 0800 0401 0802 0c0e 721f 0000 0063  ..........r....c
+000007a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000007b0: 0200 0000 4000 0000 720b 0000 0029 07da  ....@...r....)..
+000007c0: 0b45 6467 6547 7261 6469 6e67 7a1f 636f  .EdgeGradingz.co
+000007d0: 6e66 6967 7574 6174 696f 6e20 666f 7220  nfigutation for 
+000007e0: 2765 6467 6547 7261 6469 6e67 2763 0d00  'edgeGrading'c..
+000007f0: 0000 0000 0000 0000 0000 0d00 0000 0300  ................
+00000800: 0000 4300 0000 7356 0100 0074 007c 0174  ..C...sV...t.|.t
+00000810: 0183 0273 0b74 017c 0183 017c 005f 026e  ...s.t.|...|._.n
+00000820: 037c 017c 005f 0274 007c 0274 0183 0273  .|.|._.t.|.t...s
+00000830: 1974 017c 0283 017c 005f 036e 037c 027c  .t.|...|._.n.|.|
+00000840: 005f 0374 007c 0374 0183 0273 2774 017c  ._.t.|.t...s't.|
+00000850: 0383 017c 005f 046e 037c 037c 005f 0474  ...|._.n.|.|._.t
+00000860: 007c 0474 0183 0273 3574 017c 0483 017c  .|.t...s5t.|...|
+00000870: 005f 056e 037c 047c 005f 0574 007c 0574  ._.n.|.|._.t.|.t
+00000880: 0183 0273 4374 017c 0583 017c 005f 066e  ...sCt.|...|._.n
+00000890: 037c 057c 005f 0674 007c 0674 0183 0273  .|.|._.t.|.t...s
+000008a0: 5174 017c 0683 017c 005f 076e 037c 067c  Qt.|...|._.n.|.|
+000008b0: 005f 0774 007c 0774 0183 0273 5f74 017c  ._.t.|.t...s_t.|
+000008c0: 0783 017c 005f 086e 037c 077c 005f 0874  ...|._.n.|.|._.t
+000008d0: 007c 0874 0183 0273 6d74 017c 0883 017c  .|.t...smt.|...|
+000008e0: 005f 096e 037c 087c 005f 0974 007c 0174  ._.n.|.|._.t.|.t
+000008f0: 0183 0273 7b74 017c 0983 017c 005f 0a6e  ...s{t.|...|._.n
+00000900: 037c 097c 005f 0a74 007c 0a74 0183 0273  .|.|._.t.|.t...s
+00000910: 8974 017c 0a83 017c 005f 0b6e 037c 0a7c  .t.|...|._.n.|.|
+00000920: 005f 0b74 007c 0b74 0183 0273 9774 017c  ._.t.|.t...s.t.|
+00000930: 0b83 017c 005f 0c6e 037c 0b7c 005f 0c74  ...|._.n.|.|._.t
+00000940: 007c 0c74 0183 0273 a674 017c 0c83 017c  .|.t...s.t.|...|
+00000950: 005f 0d64 0053 007c 0c7c 005f 0d64 0053  ._.d.S.|.|._.d.S
+00000960: 0072 2000 0000 290e 7219 0000 0072 0c00  .r ...).r....r..
+00000970: 0000 da02 7831 da02 7832 da02 7833 da02  ....x1..x2..x3..
+00000980: 7834 da02 7931 da02 7932 da02 7933 da02  x4..y1..y2..y3..
+00000990: 7934 da02 7a31 da02 7a32 da02 7a33 da02  y4..z1..z2..z3..
+000009a0: 7a34 290d 720e 0000 0072 2600 0000 7227  z4).r....r&...r'
+000009b0: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
+000009c0: 0000 722b 0000 0072 2c00 0000 722d 0000  ..r+...r,...r-..
+000009d0: 0072 2e00 0000 722f 0000 0072 3000 0000  .r....r/...r0...
+000009e0: 7231 0000 0072 0900 0000 7209 0000 0072  r1...r....r....r
+000009f0: 0a00 0000 720f 0000 0039 0000 0073 4800  ....r....9...sH.
+00000a00: 0000 0a01 0c01 0602 0a01 0c01 0602 0a01  ................
 00000a10: 0c01 0602 0a01 0c01 0602 0a01 0c01 0602  ................
 00000a20: 0a01 0c01 0602 0a01 0c01 0602 0a01 0c01  ................
 00000a30: 0602 0a01 0c01 0602 0a01 0c01 0602 0a01  ................
-00000a40: 0c01 0602 0a01 0c01 0602 0a01 0e01 0a02  ................
-00000a50: 7a14 4564 6765 4772 6164 696e 672e 5f5f  z.EdgeGrading.__
-00000a60: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
-00000a70: 0000 0005 0000 0005 0000 0043 0000 0073  ...........C...s
-00000a80: 4600 0000 6700 7d01 7400 6401 6402 8302  F...g.}.t.d.d...
-00000a90: 4400 5d12 5c02 7d02 7d03 7401 7c00 7c02  D.].\.}.}.t.|.|.
-00000aa0: 7c03 1700 8302 7d04 7c01 a002 7c04 a003  |.....}.|...|...
-00000ab0: a100 a101 0100 7107 6403 6404 a004 7c01  ......q.d.d...|.
-00000ac0: a101 1700 6405 1700 5300 2906 4e5a 0378  ....d...S.).NZ.x
-00000ad0: 797a da04 3132 3334 7a0d 6564 6765 4772  yz..1234z.edgeGr
-00000ae0: 6164 696e 6720 2872 1100 0000 7224 0000  ading (r....r$..
-00000af0: 0029 0572 0300 0000 da07 6765 7461 7474  .).r......getatt
-00000b00: 72da 0661 7070 656e 6472 1d00 0000 721a  r..appendr....r.
-00000b10: 0000 0029 0572 0e00 0000 da03 746d 70da  ...).r......tmp.
-00000b20: 066c 6574 7465 72da 0569 6e64 6578 da03  .letter..index..
-00000b30: 7661 7272 0900 0000 7209 0000 0072 0a00  varr....r....r..
-00000b40: 0000 721d 0000 006b 0000 0073 0a00 0000  ..r....k...s....
-00000b50: 0401 1201 0e01 1001 1201 7a12 4564 6765  ..........z.Edge
-00000b60: 4772 6164 696e 672e 666f 726d 6174 4e72  Grading.formatNr
-00000b70: 1e00 0000 7209 0000 0072 0900 0000 7209  ....r....r....r.
-00000b80: 0000 0072 0a00 0000 7225 0000 0036 0000  ...r....r%...6..
-00000b90: 0073 0800 0000 0800 0401 0802 0c32 7225  .s...........2r%
-00000ba0: 0000 004e 2908 da0f 636f 6c6c 6563 7469  ...N)...collecti
-00000bb0: 6f6e 732e 6162 6372 0200 0000 da09 6974  ons.abcr......it
-00000bc0: 6572 746f 6f6c 7372 0300 0000 7204 0000  ertoolsr....r...
-00000bd0: 0072 0c00 0000 721f 0000 0072 2500 0000  .r....r....r%...
-00000be0: 7209 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
-00000bf0: 0a00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000c00: 0000 730c 0000 000c 000c 010e 030e 0410  ..s.............
-00000c10: 1514 18                                  ...
+00000a40: 0c01 0602 0a01 0e01 0a02 7a14 4564 6765  ..........z.Edge
+00000a50: 4772 6164 696e 672e 5f5f 696e 6974 5f5f  Grading.__init__
+00000a60: 6301 0000 0000 0000 0000 0000 0005 0000  c...............
+00000a70: 0005 0000 0043 0000 0073 4600 0000 6700  .....C...sF...g.
+00000a80: 7d01 7400 6401 6402 8302 4400 5d12 5c02  }.t.d.d...D.].\.
+00000a90: 7d02 7d03 7401 7c00 7c02 7c03 1700 8302  }.}.t.|.|.|.....
+00000aa0: 7d04 7c01 a002 7c04 a003 a100 a101 0100  }.|...|.........
+00000ab0: 7107 6403 6404 a004 7c01 a101 1700 6405  q.d.d...|.....d.
+00000ac0: 1700 5300 2906 4e5a 0378 797a da04 3132  ..S.).NZ.xyz..12
+00000ad0: 3334 7a0d 6564 6765 4772 6164 696e 6720  34z.edgeGrading 
+00000ae0: 2872 1100 0000 7224 0000 0029 0572 0300  (r....r$...).r..
+00000af0: 0000 da07 6765 7461 7474 72da 0661 7070  ....getattr..app
+00000b00: 656e 6472 1d00 0000 721a 0000 0029 0572  endr....r....).r
+00000b10: 0e00 0000 da03 746d 70da 066c 6574 7465  ......tmp..lette
+00000b20: 72da 0569 6e64 6578 da03 7661 7272 0900  r..index..varr..
+00000b30: 0000 7209 0000 0072 0a00 0000 721d 0000  ..r....r....r...
+00000b40: 006b 0000 0073 0a00 0000 0401 1201 0e01  .k...s..........
+00000b50: 1001 1201 7a12 4564 6765 4772 6164 696e  ....z.EdgeGradin
+00000b60: 672e 666f 726d 6174 4e72 1e00 0000 7209  g.formatNr....r.
+00000b70: 0000 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
+00000b80: 0000 7225 0000 0036 0000 0073 0800 0000  ..r%...6...s....
+00000b90: 0800 0401 0802 0c32 7225 0000 004e 2908  .......2r%...N).
+00000ba0: da0f 636f 6c6c 6563 7469 6f6e 732e 6162  ..collections.ab
+00000bb0: 6372 0200 0000 da09 6974 6572 746f 6f6c  cr......itertool
+00000bc0: 7372 0300 0000 7204 0000 0072 0c00 0000  sr....r....r....
+00000bd0: 721f 0000 0072 2500 0000 7209 0000 0072  r....r%...r....r
+00000be0: 0900 0000 7209 0000 0072 0a00 0000 da08  ....r....r......
+00000bf0: 3c6d 6f64 756c 653e 0100 0000 730c 0000  <module>....s...
+00000c00: 000c 000c 010e 030e 0410 1514 18         .............
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/edges.py` & `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/edges.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/grading.py` & `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/blockmesh/grading.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/generators.py` & `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/generators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+"""Internal machinery to generate the OpenFOAM input files"""
+
 from abc import ABC, abstractmethod
 from inspect import getmodule
 from pathlib import Path
 
 import jinja2
 from inflection import camelize, underscore
 
 from fluiddyn.util import import_class
+from fluidsimfoam.foam_input_files import FileHelper, parse, read_field_file
 
 
 class InputFiles:
     """Container of the generator objects"""
 
     def __init__(self, output):
         self.output = output
@@ -34,89 +37,127 @@
 
 
 class FileGeneratorABC(ABC):
     rel_path: str
 
     def __init__(self, output):
         self.output = output
+        self.input_files = output.input_files
 
-    def generate_file(self):
+    def generate_file(self, params=None):
         """Generate the file"""
+        if params is None:
+            params = self.output.sim.params
         with open(self.output.path_run / self.rel_path, "w") as file:
-            file.write(self.generate_code())
+            file.write(self.generate_code(params))
 
     @abstractmethod
     def generate_code(self):
         """Generate the code of the file"""
 
+    def read(self):
+        path = self.output.path_run / self.rel_path
+        if any(
+            self.rel_path.startswith(start) for start in ["system", "constant"]
+        ):
+            tree = parse(path.read_text())
+            tree.path = path
+            return tree
+        else:
+            return read_field_file(path)
+
+    def overwrite(self, dumpable):
+        with open(self.output.path_run / self.rel_path, "w") as file:
+            file.write(dumpable.dump())
+
 
 class FileGenerator(FileGeneratorABC):
     template_name: str
 
     def __init__(self, output):
         super().__init__(output)
-        self._name = underscore(Path(self.rel_path).name)
 
-    def generate_code(self):
+    def generate_code(self, params=None):
         """Generate the code of the file from ...
 
         - a method named like `sim.output.make_code_block_mesh_dict`,
         - or a Jinja template.
         """
+        if params is None:
+            params = self.output.sim.params
+
         try:
-            method = getattr(self.output, "make_code_" + self._name)
-            if method is None:
-                raise AttributeError
+            make_code = getattr(self.output, "make_code_" + self._name)
         except AttributeError:
+            make_code = None
+
+        if make_code is None:
             try:
                 make_tree = getattr(self.output, "make_tree_" + self._name)
-                if make_tree is None:
-                    raise AttributeError
             except AttributeError:
-                template = self.output.input_files.get_template(
-                    self.template_name
-                )
-                return template.render(params=self.output.sim.params)
-            else:
+                make_tree = None
 
-                def method(params):
-                    return make_tree(params).dump()
+            if make_tree is None:
+                try:
+                    helper = getattr(self.output, "helper_" + self._name)
+                except AttributeError:
+                    pass
+                else:
+                    if isinstance(helper, FileHelper):
+                        make_tree = helper.make_tree
+
+            if make_tree is not None:
+
+                def make_code(params_):
+                    return make_tree(params_).dump()
+
+        if make_code is None:
+            template = self.input_files.get_template(self.template_name)
+            return template.render(params=params)
 
-        if (self.output.input_files.templates_dir / self.template_name).exists():
+        if (self.input_files.templates_dir / self.template_name).exists():
             raise RuntimeError(
                 "Fluidsimfoam solver issue: "
                 f"2 concurrent methods to produce {self.rel_path}:\n"
-                f"- template in {self.output.input_files.templates_dir},\n"
+                f"- template in {self.input_files.templates_dir},\n"
                 f"- function output.make_code_{self._name}.\n"
                 "Remove the file or the function (or make it equal to None)."
             )
 
-        return method(self.output.sim.params)
+        return make_code(params)
 
     @classmethod
     def _complete_params_with_default(cls, params, info_solver):
         output_cls = import_class(
             info_solver.classes.Output.module_name,
             info_solver.classes.Output.class_name,
         )
-
         try:
-            method = getattr(output_cls, "_complete_params_" + cls._name)
-            if method is None:
-                raise AttributeError
+            complete_params = getattr(output_cls, "_complete_params_" + cls._name)
         except AttributeError:
-            pass
-        else:
-            method(params)
+            complete_params = None
+
+        if complete_params is None:
+            try:
+                helper = getattr(output_cls, "helper_" + cls._name)
+            except AttributeError:
+                pass
+            else:
+                if isinstance(helper, FileHelper):
+                    complete_params = helper.complete_params
+
+        if complete_params is not None:
+            complete_params(params)
 
 
 def new_file_generator_class(file_name, dir_name="0"):
     cls_name = f"FileGenerator{camelize(file_name)}"
     return type(
         cls_name,
         (FileGenerator,),
         {
+            "dir_name": dir_name,
             "rel_path": f"{dir_name}/{file_name}",
             "template_name": f"{file_name}.jinja",
-            "_name": underscore(file_name),
+            "_name": underscore(file_name.replace(".", "_")),
         },
     )
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/grammar.lark` & `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/grammar.lark`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/grammar_advanced.lark` & `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/grammar_advanced.lark`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/parser.py` & `fluidsimfoam-0.0.3/src/fluidsimfoam/foam_input_files/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Parser for OpenFOAM input files"""
+
 from dataclasses import dataclass
 from pathlib import Path
 
 from lark import Lark, Token, Transformer
 from lark.exceptions import LarkError
 
 from .ast import (
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/info.py` & `fluidsimfoam-0.0.3/src/fluidsimfoam/info.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+"""Base class for ``Simul.InfoSolver``"""
+
 from fluidsim_core.info import InfoSolverCore
 
 
 class InfoSolver(InfoSolverCore):
+    """Contains the information on which classes are used in a solver"""
     def _init_root(self):
         super()._init_root()
 
         self.classes._set_child(
             "Output",
             attribs={
                 "module_name": "fluidsimfoam.output",
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/log.py` & `fluidsimfoam-0.0.3/src/fluidsimfoam/log.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""Logging
-==========
-A logger instance (variable :code:`logger`).
+"""Fluidsimfoam logging
+
+Define a logger instance (variable :code:`logger`).
 
 """
 
 import logging
 import os
 
 logger = logging.getLogger(__name__)
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/next_fluidsim_core.py` & `fluidsimfoam-0.0.3/src/fluidsimfoam/next_fluidsim_core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Code that should be part of the next ``fluidsim_core`` release"""
+
 from pathlib import Path
 from textwrap import dedent
 
 from fluiddyn.io import FLUIDSIM_PATH
 
 from .log import logger
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/output/__pycache__/base.cpython-310.pyc` & `fluidsimfoam-0.0.3/src/fluidsimfoam/output/__pycache__/base.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Apr 26 13:42:06 2023 UTC, .py size: 10986 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,566 +1,477 @@
-00000000: 6f0d 0d0a 0000 0000 2e2a 4964 ea2a 0000  o........*Id.*..
+00000000: 6f0d 0d0a 0000 0000 8712 5a64 f623 0000  o.........Zd.#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 6400 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000080: 0100 6400 6407 6c0d 6d0e 5a0e 0100 6400  ..d.d.l.m.Z...d.
 00000090: 6408 6c0f 6d10 5a10 6d11 5a11 6d12 5a12  d.l.m.Z.m.Z.m.Z.
-000000a0: 0100 6400 6409 6c13 6d14 5a14 6d15 5a15  ..d.d.l.m.Z.m.Z.
+000000a0: 6d13 5a13 0100 6400 6409 6c14 6d15 5a15  m.Z...d.d.l.m.Z.
 000000b0: 6d16 5a16 0100 6400 640a 6c17 6d18 5a18  m.Z...d.d.l.m.Z.
 000000c0: 0100 6400 640b 6c19 6d1a 5a1a 0100 4700  ..d.d.l.m.Z...G.
 000000d0: 640c 640d 8400 640d 650c 8303 5a1b 6401  d.d...d.e...Z.d.
 000000e0: 5300 290e e900 0000 004e 2901 da04 5061  S.)......N)...Pa
 000000f0: 7468 a901 da0a 756e 6465 7273 636f 7265  th....underscore
 00000100: 2901 da11 7374 646f 7574 5f72 6564 6972  )...stdout_redir
 00000110: 6563 7465 6429 01da 036d 7069 2901 da0a  ected)...mpi)...
 00000120: 4f75 7470 7574 436f 7265 2901 da14 6974  OutputCore)...it
 00000130: 6572 5f63 6f6d 706c 6574 655f 7061 7261  er_complete_para
-00000140: 6d73 2903 da14 4445 4641 554c 545f 434f  ms)...DEFAULT_CO
+00000140: 6d73 2904 da14 4445 4641 554c 545f 434f  ms)...DEFAULT_CO
 00000150: 4e54 524f 4c5f 4449 4354 da0e 4445 4641  NTROL_DICT..DEFA
-00000160: 554c 545f 4845 4144 4552 da0d 466f 616d  ULT_HEADER..Foam
-00000170: 496e 7075 7446 696c 6529 03da 1046 696c  InputFile)...Fil
-00000180: 6547 656e 6572 6174 6f72 4142 43da 0a49  eGeneratorABC..I
-00000190: 6e70 7574 4669 6c65 73da 186e 6577 5f66  nputFiles..new_f
-000001a0: 696c 655f 6765 6e65 7261 746f 725f 636c  ile_generator_cl
-000001b0: 6173 7329 01da 066c 6f67 6765 7229 01da  ass)...logger)..
-000001c0: 1267 6574 5f73 6f6c 7665 725f 7061 636b  .get_solver_pack
-000001d0: 6167 6563 0000 0000 0000 0000 0000 0000  agec............
-000001e0: 0000 0000 0400 0000 0000 0000 73da 0000  ............s...
-000001f0: 0065 005a 0164 005a 0264 0164 0267 025a  .e.Z.d.Z.d.d.g.Z
-00000200: 0364 0364 0467 025a 0467 0064 05a2 015a  .d.d.g.Z.g.d...Z
-00000210: 0565 0664 0664 0784 0083 015a 0765 0664  .e.d.d.....Z.e.d
-00000220: 0864 0984 0083 015a 0865 0664 0a64 0b84  .d.....Z.e.d.d..
-00000230: 0083 015a 0965 0664 0c64 0d84 0083 015a  ...Z.e.d.d.....Z
-00000240: 0a64 2787 0066 0164 0f64 1084 095a 0b65  .d'..f.d.d...Z.e
-00000250: 0664 1164 1284 0083 015a 0c87 0066 0164  .d.d.....Z...f.d
-00000260: 1364 1484 085a 0d64 1564 1684 005a 0e65  .d...Z.d.d...Z.e
-00000270: 0664 1764 1884 0083 015a 0f64 1964 1a84  .d.d.....Z.d.d..
-00000280: 005a 1064 1b64 1c84 005a 1165 0664 1d64  .Z.d.d...Z.e.d.d
-00000290: 1e84 0083 015a 1264 1f64 2084 005a 1365  .....Z.d.d ..Z.e
-000002a0: 0664 2164 2284 0083 015a 1465 0664 2364  .d!d"....Z.e.d#d
-000002b0: 2484 0083 015a 1565 0664 2564 2684 0083  $....Z.e.d%d&...
-000002c0: 015a 1687 0004 005a 1753 0029 28da 064f  .Z.....Z.S.)(..O
-000002d0: 7574 7075 74da 0170 da01 55da 1374 7261  utput..p..U..tra
-000002e0: 6e73 706f 7274 5072 6f70 6572 7469 6573  nsportProperties
-000002f0: da14 7475 7262 756c 656e 6365 5072 6f70  ..turbulenceProp
-00000300: 6572 7469 6573 2903 da0b 636f 6e74 726f  erties)...contro
-00000310: 6c44 6963 74da 0966 7653 6368 656d 6573  lDict..fvSchemes
-00000320: da0a 6676 536f 6c75 7469 6f6e 6302 0000  ..fvSolutionc...
-00000330: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-00000340: 0043 0000 0073 2800 0000 7c01 6a00 6a01  .C...s(...|.j.j.
-00000350: a002 6401 a101 7d02 7c00 a003 7c02 a101  ..d...}.|...|...
-00000360: 0100 7c01 6a00 6a01 a004 a100 0100 6402  ..|.j.j.......d.
-00000370: 5300 2903 7a66 436f 6d70 6c65 7465 2074  S.).zfComplete t
-00000380: 6865 2069 6e66 6f5f 736f 6c76 6572 2069  he info_solver i
-00000390: 6e73 7461 6e63 6520 7769 7468 2063 6869  nstance with chi
-000003a0: 6c64 2063 6c61 7373 2064 6574 6169 6c73  ld class details
-000003b0: 2028 6d6f 6475 6c65 0a20 2020 2020 2020   (module.       
-000003c0: 2061 6e64 2063 6c61 7373 206e 616d 6573   and class names
-000003d0: 292e 0a0a 2020 2020 2020 2020 da07 636c  )...        ..cl
-000003e0: 6173 7365 734e 2905 7219 0000 0072 1100  assesN).r....r..
-000003f0: 0000 da0a 5f73 6574 5f63 6869 6c64 da18  ...._set_child..
-00000400: 5f73 6574 5f69 6e66 6f5f 736f 6c76 6572  _set_info_solver
-00000410: 5f63 6c61 7373 6573 da15 636f 6d70 6c65  _classes..comple
-00000420: 7465 5f77 6974 685f 636c 6173 7365 7329  te_with_classes)
-00000430: 03da 0363 6c73 da0b 696e 666f 5f73 6f6c  ...cls..info_sol
-00000440: 7665 7272 1900 0000 a900 721f 0000 00fa  verr......r.....
-00000450: 3d2f 686f 6d65 2f70 6965 7272 652f 4465  =/home/pierre/De
-00000460: 762f 666c 7569 6473 696d 666f 616d 2f73  v/fluidsimfoam/s
-00000470: 7263 2f66 6c75 6964 7369 6d66 6f61 6d2f  rc/fluidsimfoam/
-00000480: 6f75 7470 7574 2f62 6173 652e 7079 da15  output/base.py..
-00000490: 5f63 6f6d 706c 6574 655f 696e 666f 5f73  _complete_info_s
-000004a0: 6f6c 7665 721f 0000 0073 0600 0000 0e06  olver....s......
-000004b0: 0a01 1002 7a1c 4f75 7470 7574 2e5f 636f  ....z.Output._co
-000004c0: 6d70 6c65 7465 5f69 6e66 6f5f 736f 6c76  mplete_info_solv
-000004d0: 6572 6302 0000 0000 0000 0000 0000 0002  erc.............
-000004e0: 0000 0001 0000 0043 0000 0073 0400 0000  .......C...s....
-000004f0: 6401 5300 2902 7a2e 5365 7420 7468 6520  d.S.).z.Set the 
-00000500: 636c 6173 7365 7320 666f 7220 696e 666f  classes for info
-00000510: 5f73 6f6c 7665 722e 636c 6173 7365 732e  _solver.classes.
-00000520: 4f75 7470 7574 4e72 1f00 0000 2902 721d  OutputNr....).r.
-00000530: 0000 0072 1900 0000 721f 0000 0072 1f00  ...r....r....r..
-00000540: 0000 7220 0000 0072 1b00 0000 2a00 0000  ..r ...r....*...
-00000550: 7302 0000 0004 007a 1f4f 7574 7075 742e  s......z.Output.
-00000560: 5f73 6574 5f69 6e66 6f5f 736f 6c76 6572  _set_info_solver
-00000570: 5f63 6c61 7373 6573 6301 0000 0000 0000  _classesc.......
-00000580: 0000 0000 0004 0000 0004 0000 0043 0000  .............C..
-00000590: 0073 5a00 0000 6900 0400 7d01 7c00 5f00  .sZ...i...}.|._.
-000005a0: 7c00 6a01 4400 5d08 7d02 7402 7c02 8301  |.j.D.].}.t.|...
-000005b0: 7c01 7c02 3c00 7108 7c00 6a03 4400 5d09  |.|.<.q.|.j.D.].
-000005c0: 7d03 7402 7c03 6401 8302 7c01 7c03 3c00  }.t.|.d...|.|.<.
-000005d0: 7114 7c00 6a04 4400 5d09 7d03 7402 7c03  q.|.j.D.].}.t.|.
-000005e0: 6402 8302 7c01 7c03 3c00 7121 6400 5300  d...|.|.<.q!d.S.
-000005f0: 2903 4eda 0863 6f6e 7374 616e 74da 0673  ).N..constant..s
-00000600: 7973 7465 6d29 05da 185f 6669 6c65 5f67  ystem)..._file_g
-00000610: 656e 6572 6174 6f72 735f 636c 6173 7365  enerators_classe
-00000620: 73da 0e76 6172 6961 626c 655f 6e61 6d65  s..variable_name
-00000630: 7372 0e00 0000 da14 636f 6e73 7461 6e74  sr......constant
-00000640: 5f66 696c 6573 5f6e 616d 6573 da12 7379  _files_names..sy
-00000650: 7374 656d 5f66 696c 6573 5f6e 616d 6573  stem_files_names
-00000660: 2904 721d 0000 0072 1900 0000 5a0d 7661  ).r....r....Z.va
-00000670: 7269 6162 6c65 5f6e 616d 65da 0966 696c  riable_name..fil
-00000680: 655f 6e61 6d65 721f 0000 0072 1f00 0000  e_namer....r....
-00000690: 7220 0000 00da 1e5f 7365 7475 705f 6669  r ....._setup_fi
-000006a0: 6c65 5f67 656e 6572 6174 6f72 735f 636c  le_generators_cl
-000006b0: 6173 7365 732e 0000 0073 1000 0000 0a02  asses....s......
-000006c0: 0a01 0e01 0a02 1001 0a02 1001 04ff 7a25  ..............z%
-000006d0: 4f75 7470 7574 2e5f 7365 7475 705f 6669  Output._setup_fi
-000006e0: 6c65 5f67 656e 6572 6174 6f72 735f 636c  le_generators_cl
-000006f0: 6173 7365 7363 0300 0000 0000 0000 0000  assesc..........
-00000700: 0000 0400 0000 0600 0000 4300 0000 7372  ..........C...sr
-00000710: 0000 007c 00a0 00a1 0001 0074 017c 017c  ...|.......t.|.|
-00000720: 027c 006a 02a0 03a1 0083 0301 007c 01a0  .|.j.........|..
-00000730: 0474 0564 0164 0264 038d 02a1 0101 007c  .t.d.d.d.......|
-00000740: 016a 0664 0464 0164 0564 069c 0264 078d  .j.d.d.d.d...d..
-00000750: 0201 007c 016a 07a0 0874 09a0 0a64 08a1  ...|.j...t...d..
-00000760: 01a1 0101 007c 026a 0b6a 0ca0 0da1 007d  .....|.j.j.....}
-00000770: 0374 017c 017c 027c 03a0 03a1 0083 0301  .t.|.|.|........
-00000780: 0064 0953 0029 0a7a 3e54 6869 7320 7374  .d.S.).z>This st
-00000790: 6174 6963 206d 6574 686f 6420 6973 2075  atic method is u
-000007a0: 7365 6420 746f 2063 6f6d 706c 6574 6520  sed to complete 
-000007b0: 7468 6520 2a70 6172 616d 732a 2063 6f6e  the *params* con
-000007c0: 7461 696e 6572 2e54 da03 7275 6e29 02da  tainer.T..run)..
-000007d0: 0f4e 4557 5f44 4952 5f52 4553 554c 5453  .NEW_DIR_RESULTS
-000007e0: 5a13 7368 6f72 745f 6e61 6d65 5f74 7970  Z.short_name_typ
-000007f0: 655f 7275 6eda 066f 7574 7075 74da 0029  e_run..output..)
-00000800: 02da 0b48 4153 5f54 4f5f 5341 5645 da0d  ...HAS_TO_SAVE..
-00000810: 7375 625f 6469 7265 6374 6f72 79a9 01da  sub_directory...
-00000820: 0761 7474 7269 6273 612e 0100 000a 2020  .attribsa.....  
-00000830: 2020 2d20 6060 4841 535f 544f 5f53 4156    - ``HAS_TO_SAV
-00000840: 4560 603a 2062 6f6f 6c20 2864 6566 6175  E``: bool (defau
-00000850: 6c74 3a20 5472 7565 2920 4966 2046 616c  lt: True) If Fal
-00000860: 7365 2c20 6e6f 7468 696e 6720 6e65 7720  se, nothing new 
-00000870: 6973 2073 6176 6564 2069 6e0a 2020 2020  is saved in.    
-00000880: 2020 7468 6520 6469 7265 6374 6f72 7920    the directory 
-00000890: 6f66 2074 6865 2073 696d 756c 6174 696f  of the simulatio
-000008a0: 6e2e 0a20 2020 202d 2060 6073 7562 5f64  n..    - ``sub_d
-000008b0: 6972 6563 746f 7279 6060 3a20 7374 7220  irectory``: str 
-000008c0: 2864 6566 6175 6c74 3a20 2222 2920 4120  (default: "") A 
-000008d0: 6e61 6d65 206f 6620 6120 7375 622d 6469  name of a sub-di
-000008e0: 7265 6374 6f72 7920 2872 656c 6174 6976  rectory (relativ
-000008f0: 650a 2020 2020 2020 746f 2024 464c 5549  e.      to $FLUI
-00000900: 4444 594e 5f50 4154 485f 5343 5241 5443  DDYN_PATH_SCRATC
-00000910: 4829 2077 6865 7265 696e 2074 6865 2064  H) wherein the d
-00000920: 6972 6563 746f 7279 206f 6620 7468 6520  irectory of the 
-00000930: 7369 6d75 6c61 7469 6f6e 0a20 2020 2020  simulation.     
-00000940: 2028 6060 7061 7468 5f72 756e 6060 2920   (``path_run``) 
-00000950: 6973 2073 6176 6564 2e0a 0a4e 290e 7229  is saved...N).r)
-00000960: 0000 0072 0800 0000 7224 0000 00da 0676  ...r....r$.....v
-00000970: 616c 7565 73da 0c5f 7365 745f 6174 7472  alues.._set_attr
-00000980: 6962 73da 0464 6963 7472 1a00 0000 722c  ibs..dictr....r,
-00000990: 0000 00da 085f 7365 745f 646f 63da 0874  ....._set_doc..t
-000009a0: 6578 7477 7261 70da 0664 6564 656e 7472  extwrap..dedentr
-000009b0: 1900 0000 7211 0000 00da 0e69 6d70 6f72  ....r......impor
-000009c0: 745f 636c 6173 7365 7329 0472 1d00 0000  t_classes).r....
-000009d0: da06 7061 7261 6d73 721e 0000 00da 0c64  ..paramsr......d
-000009e0: 6963 745f 636c 6173 7365 7372 1f00 0000  ict_classesr....
-000009f0: 721f 0000 0072 2000 0000 da1d 5f63 6f6d  r....r ....._com
-00000a00: 706c 6574 655f 7061 7261 6d73 5f77 6974  plete_params_wit
-00000a10: 685f 6465 6661 756c 743a 0000 0073 1e00  h_default:...s..
-00000a20: 0000 0804 0201 0c01 04ff 1205 0401 0a01  ................
-00000a30: 06ff 0603 0401 0201 02ff 04ff 0c0d 1401  ................
-00000a40: 7a24 4f75 7470 7574 2e5f 636f 6d70 6c65  z$Output._comple
-00000a50: 7465 5f70 6172 616d 735f 7769 7468 5f64  te_params_with_d
-00000a60: 6566 6175 6c74 4e63 0300 0000 0000 0000  efaultNc........
-00000a70: 0000 0000 0a00 0000 0800 0000 0300 0000  ................
-00000a80: 73e0 0100 007c 017c 005f 007a 087c 016a  s....|.|._.z.|.j
-00000a90: 016a 026a 037c 005f 0457 006e 0904 0074  .j.j.|._.W.n...t
-00000aa0: 0579 1401 0001 0001 0059 006e 0777 0074  .y.......Y.n.w.t
-00000ab0: 067c 006a 0483 017c 005f 077c 00a0 08a1  .|.j...|._.|....
-00000ac0: 007c 005f 097c 0172 2e7c 016a 0a6a 0b7c  .|._.|.r.|.j.j.|
-00000ad0: 005f 0a74 0c83 00a0 0d7c 01a1 0101 006e  ._.t.....|.....n
-00000ae0: 0f7c 0272 357c 026a 0b7c 005f 0a6e 0864  .|.r5|.j.|._.n.d
-00000af0: 007c 005f 0a74 0ea0 0f64 01a1 0101 007c  .|._.t...d.....|
-00000b00: 0173 4164 0053 0074 107c 006a 1183 017c  .sAd.S.t.|.j...|
-00000b10: 005f 1174 127c 0083 017c 005f 137c 016a  ._.t.|...|._.|.j
-00000b20: 016a 026a 146a 15a0 16a1 007d 0374 177c  .j.j.j.....}.t.|
-00000b30: 0064 0283 0273 5d7c 00a0 18a1 0001 007c  .d...s]|.......|
-00000b40: 03a0 197c 006a 1aa1 0101 0067 007d 047c  ...|.j.....g.}.|
-00000b50: 03a0 1ba1 0044 005d 365c 027d 057d 0674  .....D.]6\.}.}.t
-00000b60: 1c7c 007c 0683 0272 7371 6974 1d7c 0583  .|.|...rsqit.|..
-00000b70: 017d 0774 1e7c 0674 1f83 0272 857c 006a  .}.t.|.t...r.|.j
-00000b80: 137d 087c 04a0 207c 05a1 0101 006e 127c  .}.|.. |.....n.|
-00000b90: 007d 087c 006a 0004 006a 2164 03a0 2264  .}.|.j...j!d.."d
-00000ba0: 047c 079b 0064 059d 037c 06a1 0237 0002  .|...d...|...7..
-00000bb0: 005f 2174 237c 087c 077c 067c 0083 0183  ._!t#|.|.|.|....
-00000bc0: 0301 0071 697c 0472 b37c 006a 0004 006a  ...qi|.r.|.j...j
-00000bd0: 2164 0664 079b 0464 08a0 247c 04a1 019b  !d.d...d..$|....
-00000be0: 0064 099d 0337 0002 005f 2174 256a 2664  .d...7..._!t%j&d
-00000bf0: 0a6b 0272 c07c 006a 2772 c07c 006a 006a  .k.r.|.j'r.|.j.j
-00000c00: 0a6a 2873 c264 0053 007c 006a 1164 0b1b  .j(s.d.S.|.j.d..
-00000c10: 00a0 29a1 0001 007c 006a 1164 0c1b 00a0  ..)....|.j.d....
-00000c20: 29a1 0001 007c 006a 1164 0d1b 00a0 29a1  )....|.j.d....).
-00000c30: 0001 007a 0874 2a7c 006a 1364 0e83 027d  ...z.t*|.j.d...}
-00000c40: 0957 006e 0a04 0074 0579 e901 0001 0001  .W.n...t.y......
-00000c50: 0059 0064 0053 0077 007c 09a0 2ba1 0001  .Y.d.S.w.|..+...
-00000c60: 0064 0053 0029 0f4e 7a45 496e 6974 6961  .d.S.).NzEInitia
-00000c70: 6c69 7a69 6e67 204f 7574 7075 7420 636c  lizing Output cl
-00000c80: 6173 7320 7769 7468 6f75 7420 7369 6d20  ass without sim 
-00000c90: 6f72 2070 6172 616d 7320 6d69 6768 7420  or params might 
-00000ca0: 6c65 6164 2074 6f20 6572 726f 7273 2e72  lead to errors.r
-00000cb0: 2400 0000 7a09 7b3a 3238 737d 7b7d 0a7a  $...z.{:28s}{}.z
-00000cc0: 0b73 696d 2e6f 7574 7075 742e 7a02 3a20  .sim.output.z.: 
-00000cd0: 7a0c 696e 7075 7420 6669 6c65 733a 5a03  z.input files:Z.
-00000ce0: 3238 73fa 0120 da01 0a72 0100 0000 7223  28s.. ...r....r#
-00000cf0: 0000 00da 0130 7222 0000 00da 0f62 6c6f  .....0r".....blo
-00000d00: 636b 5f6d 6573 685f 6469 6374 292c da03  ck_mesh_dict),..
-00000d10: 7369 6dda 0469 6e66 6fda 0673 6f6c 7665  sim..info..solve
-00000d20: 72da 0a73 686f 7274 5f6e 616d 65da 0b6e  r..short_name..n
-00000d30: 616d 655f 736f 6c76 6572 da0e 4174 7472  ame_solver..Attr
-00000d40: 6962 7574 6545 7272 6f72 7210 0000 00da  ibuteErrorr.....
-00000d50: 0770 6163 6b61 6765 da17 6765 745f 7061  .package..get_pa
-00000d60: 7468 5f73 6f6c 7665 725f 7061 636b 6167  th_solver_packag
-00000d70: 655a 1370 6174 685f 736f 6c76 6572 5f70  eZ.path_solver_p
-00000d80: 6163 6b61 6765 7239 0000 0072 2c00 0000  ackager9...r,...
-00000d90: da05 7375 7065 72da 085f 5f69 6e69 745f  ..super..__init_
-00000da0: 5f72 0f00 0000 da07 7761 726e 696e 6772  _r......warningr
-00000db0: 0200 0000 da08 7061 7468 5f72 756e 720d  ......path_runr.
-00000dc0: 0000 00da 0b69 6e70 7574 5f66 696c 6573  .....input_files
-00000dd0: 7219 0000 0072 1100 0000 7238 0000 00da  r....r....r8....
-00000de0: 0768 6173 6174 7472 7229 0000 00da 0675  .hasattrr).....u
-00000df0: 7064 6174 6572 2400 0000 da05 6974 656d  pdater$.....item
-00000e00: 73da 0a69 7369 6e73 7461 6e63 6572 0400  s..isinstancer..
-00000e10: 0000 da0a 6973 7375 6263 6c61 7373 720c  ....issubclassr.
-00000e20: 0000 00da 0661 7070 656e 64da 115f 6f62  .....append.._ob
-00000e30: 6a65 6374 735f 746f 5f70 7269 6e74 da06  jects_to_print..
-00000e40: 666f 726d 6174 da07 7365 7461 7474 72da  format..setattr.
-00000e50: 046a 6f69 6e72 0600 0000 da04 7261 6e6b  .joinr......rank
-00000e60: da0c 5f68 6173 5f74 6f5f 7361 7665 722b  .._has_to_saver+
-00000e70: 0000 00da 056d 6b64 6972 da07 6765 7461  .....mkdir..geta
-00000e80: 7474 72da 0d67 656e 6572 6174 655f 6669  ttr..generate_fi
-00000e90: 6c65 290a da04 7365 6c66 7240 0000 0072  le)...selfr@...r
-00000ea0: 3900 0000 723a 0000 005a 1366 6f72 5f73  9...r:...Z.for_s
-00000eb0: 7472 5f69 6e70 7574 5f66 696c 6573 da08  tr_input_files..
-00000ec0: 636c 735f 6e61 6d65 da05 436c 6173 73da  cls_name..Class.
-00000ed0: 086f 626a 5f6e 616d 655a 0e6f 626a 5f63  .obj_nameZ.obj_c
-00000ee0: 6f6e 7461 696e 696e 67da 0e66 696c 655f  ontaining..file_
-00000ef0: 6765 6e65 7261 746f 72a9 01da 095f 5f63  generator....__c
-00000f00: 6c61 7373 5f5f 721f 0000 0072 2000 0000  lass__r....r ...
-00000f10: 7249 0000 0058 0000 0073 7400 0000 0601  rI...X...st.....
-00000f20: 0201 1001 0c01 0401 02ff 0c03 0a02 0402  ................
-00000f30: 0a02 0e01 0401 0a02 0602 0401 0201 04ff  ................
-00000f40: 0404 0401 0c02 0a02 1002 0a02 0801 0c01  ................
-00000f50: 0402 1001 0a01 0201 0801 0a02 0601 0c01  ................
-00000f60: 0402 0c01 0c01 08ff 1204 0402 0801 1401  ................
-00000f70: 06ff 0805 02ff 0402 02fe 0803 02fd 0405  ................
-00000f80: 0e02 0e01 0e01 0202 1001 0c01 0601 02ff  ................
-00000f90: 0c03 7a0f 4f75 7470 7574 2e5f 5f69 6e69  ..z.Output.__ini
-00000fa0: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
-00000fb0: 0100 0000 0400 0000 4300 0000 7312 0000  ........C...s...
-00000fc0: 0074 0074 01a0 027c 00a1 016a 0383 016a  .t.t...|...j...j
-00000fd0: 0453 0029 017a 2847 6574 2074 6865 2070  .S.).z(Get the p
-00000fe0: 6174 6820 746f 7761 7264 7320 7468 6520  ath towards the 
-00000ff0: 736f 6c76 6572 2070 6163 6b61 6765 2e29  solver package.)
-00001000: 0572 0200 0000 da07 696e 7370 6563 74da  .r......inspect.
-00001010: 0967 6574 6d6f 6475 6c65 da08 5f5f 6669  .getmodule..__fi
-00001020: 6c65 5f5f da06 7061 7265 6e74 2901 721d  le__..parent).r.
-00001030: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
-00001040: 0000 7247 0000 00a5 0000 0073 0200 0000  ..rG.......s....
-00001050: 1203 7a1e 4f75 7470 7574 2e67 6574 5f70  ..z.Output.get_p
-00001060: 6174 685f 736f 6c76 6572 5f70 6163 6b61  ath_solver_packa
-00001070: 6765 6301 0000 0000 0000 0000 0000 0005  gec.............
-00001080: 0000 0008 0000 0003 0000 0073 c800 0000  ...........s....
-00001090: 7400 6a01 6401 6b02 720d 7402 6402 7c00  t.j.d.k.r.t.d.|.
-000010a0: 6a03 9b00 9d02 8301 0100 7404 8300 8f0d  j.........t.....
-000010b0: 0100 7405 8300 a006 a100 0100 5700 6403  ..t.........W.d.
-000010c0: 0400 0400 8303 0100 6e08 3100 7320 7701  ........n.1.s w.
-000010d0: 0100 0100 0100 5900 0100 7407 a008 7c00  ......Y...t...|.
-000010e0: 6a09 6a0a a101 0100 7400 6a01 6401 6b02  j.j.....t.j.d.k.
-000010f0: 723d 7c00 6a0b 723d 7c00 6a09 6a0c 6a0d  r=|.j.r=|.j.j.j.
-00001100: 723d 7c00 a00e a100 0100 740f 7c00 6a03  r=|.......t.|.j.
-00001110: 8301 7d01 7c01 6404 1b00 7d02 7c02 6a10  ..}.|.d...}.|.j.
-00001120: 6405 6406 8d01 0100 6407 4400 5d13 7d03  d.d.....d.D.].}.
-00001130: 7c02 7c03 1b00 7d04 7c04 a011 a100 7259  |.|...}.|.....rY
-00001140: 714e 7412 a013 7c01 7c03 1b00 7c04 a102  qNt...|.|...|...
-00001150: 0100 714e 6403 5300 2908 7a21 4c6f 6773  ..qNd.S.).z!Logs
-00001160: 2069 6e66 6f20 6f6e 2069 6e73 7461 6e74   info on instant
-00001170: 6961 7465 6420 636c 6173 7365 7372 0100  iated classesr..
-00001180: 0000 7a0a 7061 7468 5f72 756e 3a20 4e7a  ..z.path_run: Nz
-00001190: 0e2e 6461 7461 5f66 6c75 6964 7369 6d54  ..data_fluidsimT
-000011a0: 2901 da08 6578 6973 745f 6f6b 2902 7a0f  )...exist_ok).z.
-000011b0: 696e 666f 5f73 6f6c 7665 722e 786d 6c7a  info_solver.xmlz
-000011c0: 1070 6172 616d 735f 7369 6d75 6c2e 786d  .params_simul.xm
-000011d0: 6c29 1472 0600 0000 7257 0000 00da 0570  l).r....rW.....p
-000011e0: 7269 6e74 724b 0000 0072 0500 0000 7248  rintrK...r....rH
-000011f0: 0000 00da 0970 6f73 745f 696e 6974 720f  .....post_initr.
-00001200: 0000 0072 4100 0000 7240 0000 0072 5300  ...rA...r@...rS.
-00001210: 0000 7258 0000 0072 3900 0000 722b 0000  ..rX...r9...r+..
-00001220: 00da 2870 6f73 745f 696e 6974 5f63 7265  ..(post_init_cre
-00001230: 6174 655f 6164 6469 7469 6f6e 616c 5f73  ate_additional_s
-00001240: 6f75 7263 655f 6669 6c65 7372 0200 0000  ource_filesr....
-00001250: 7259 0000 00da 0665 7869 7374 73da 0673  rY.....exists..s
-00001260: 6875 7469 6cda 0463 6f70 7929 0572 5c00  hutil..copy).r\.
-00001270: 0000 724b 0000 005a 1270 6174 685f 696e  ..rK...Z.path_in
-00001280: 666f 5f66 6c75 6964 7369 6d72 2800 0000  fo_fluidsimr(...
-00001290: 5a08 7061 7468 5f6e 6577 7261 0000 0072  Z.path_newra...r
-000012a0: 1f00 0000 7220 0000 0072 6900 0000 aa00  ....r ...ri.....
-000012b0: 0000 732c 0000 000a 0310 0108 030c 011c  ..s,............
-000012c0: ff0e 0308 0402 ff04 0202 fe08 0302 fd08  ................
-000012d0: 050a 0308 010c 0108 0108 0108 0102 0112  ................
-000012e0: 0104 fc7a 104f 7574 7075 742e 706f 7374  ...z.Output.post
-000012f0: 5f69 6e69 7463 0100 0000 0000 0000 0000  _initc..........
-00001300: 0000 0400 0000 0400 0000 4300 0000 736e  ..........C...sn
-00001310: 0000 0074 007c 006a 0183 01a0 02a1 0044  ...t.|.j.......D
-00001320: 005d 125c 027d 017d 027c 0164 016b 0272  .].\.}.}.|.d.k.r
-00001330: 1071 0774 037c 0264 0283 0272 197c 02a0  .q.t.|.d...r.|..
-00001340: 04a1 0001 0071 077c 006a 016a 0564 031b  .....q.|.j.j.d..
-00001350: 007d 037c 03a0 06a1 0073 2d74 0764 047c  .}.|.....s-t.d.|
-00001360: 006a 016a 059b 009d 0283 0182 0174 08a0  .j.j.........t..
-00001370: 097c 037c 006a 0a6a 0ba1 0201 0064 0553  .|.|.j.j.....d.S
-00001380: 0029 067a 2443 7265 6174 6520 7468 6520  .).z$Create the 
-00001390: 6669 6c65 7320 6672 6f6d 2074 6865 6972  files from their
-000013a0: 2074 656d 706c 6174 6572 3f00 0000 725b   templater?...r[
-000013b0: 0000 007a 0874 6173 6b73 2e70 797a 2974  ...z.tasks.pyz)t
-000013c0: 6173 6b73 2e70 7920 6d69 7373 696e 6720  asks.py missing 
-000013d0: 696e 2073 6f6c 7665 7220 7465 6d70 6c61  in solver templa
-000013e0: 7465 735f 6469 7220 4e29 0cda 0476 6172  tes_dir N)...var
-000013f0: 7372 4c00 0000 724f 0000 0072 4d00 0000  srL...rO...rM...
-00001400: 725b 0000 005a 0d74 656d 706c 6174 6573  r[...Z.templates
-00001410: 5f64 6972 726b 0000 00da 0c52 756e 7469  _dirrk.....Runti
-00001420: 6d65 4572 726f 7272 6c00 0000 726d 0000  meErrorrl...rm..
-00001430: 0072 4000 0000 724b 0000 0029 0472 5c00  .r@...rK...).r\.
-00001440: 0000 da04 6e61 6d65 7260 0000 005a 0d70  ....namer`...Z.p
-00001450: 6174 685f 7461 736b 735f 7079 721f 0000  ath_tasks_pyr...
-00001460: 0072 1f00 0000 7220 0000 0072 6a00 0000  .r....r ...rj...
-00001470: c800 0000 731c 0000 0016 0208 0102 020a  ....s...........
-00001480: 0108 0102 800c 0208 0102 0102 0106 0104  ................
-00001490: ff04 ff14 047a 2f4f 7574 7075 742e 706f  .....z/Output.po
-000014a0: 7374 5f69 6e69 745f 6372 6561 7465 5f61  st_init_create_a
-000014b0: 6464 6974 696f 6e61 6c5f 736f 7572 6365  dditional_source
-000014c0: 5f66 696c 6573 6302 0000 0000 0000 0000  _filesc.........
-000014d0: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
-000014e0: 2600 0000 6401 6402 8400 7400 a001 a100  &...d.d...t.....
-000014f0: 4400 8301 7d02 7c01 6a02 6403 7c02 6404  D...}.|.j.d.|.d.
-00001500: 6405 8d03 0100 6400 5300 2906 4e63 0100  d.....d.S.).Nc..
-00001510: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00001520: 0000 5300 0000 731a 0000 0069 007c 005d  ..S...s....i.|.]
-00001530: 095c 027d 017d 0274 007c 0183 017c 0293  .\.}.}.t.|...|..
-00001540: 0271 0253 0072 1f00 0000 7203 0000 0029  .q.S.r....r....)
-00001550: 03da 022e 30da 036b 6579 da05 7661 6c75  ....0..key..valu
-00001560: 6572 1f00 0000 721f 0000 0072 2000 0000  er....r....r ...
-00001570: da0a 3c64 6963 7463 6f6d 703e db00 0000  ..<dictcomp>....
-00001580: 7306 0000 0006 000e 0106 ff7a 384f 7574  s..........z8Out
-00001590: 7075 742e 5f63 6f6d 706c 6574 655f 7061  put._complete_pa
-000015a0: 7261 6d73 5f63 6f6e 7472 6f6c 5f64 6963  rams_control_dic
-000015b0: 742e 3c6c 6f63 616c 733e 2e3c 6469 6374  t.<locals>.<dict
-000015c0: 636f 6d70 3eda 0c63 6f6e 7472 6f6c 5f64  comp>..control_d
-000015d0: 6963 747a 3d53 6565 2068 7474 7073 3a2f  ictz=See https:/
-000015e0: 2f64 6f63 2e63 6664 2e64 6972 6563 742f  /doc.cfd.direct/
-000015f0: 6f70 656e 666f 616d 2f75 7365 722d 6775  openfoam/user-gu
-00001600: 6964 652d 7636 2f63 6f6e 7472 6f6c 6469  ide-v6/controldi
-00001610: 6374 a902 7231 0000 00da 0364 6f63 2903  ct..r1.....doc).
-00001620: 7209 0000 0072 4f00 0000 721a 0000 0029  r....rO...r....)
-00001630: 0372 1d00 0000 7239 0000 0072 3100 0000  .r....r9...r1...
-00001640: 721f 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
-00001650: 1d5f 636f 6d70 6c65 7465 5f70 6172 616d  ._complete_param
-00001660: 735f 636f 6e74 726f 6c5f 6469 6374 d900  s_control_dict..
-00001670: 0000 7310 0000 0006 0206 0106 ff04 0402  ..s.............
-00001680: 0102 0102 010a fd7a 244f 7574 7075 742e  .......z$Output.
-00001690: 5f63 6f6d 706c 6574 655f 7061 7261 6d73  _complete_params
-000016a0: 5f63 6f6e 7472 6f6c 5f64 6963 7463 0200  _control_dictc..
-000016b0: 0000 0000 0000 0000 0000 0400 0000 0700  ................
-000016c0: 0000 0300 0000 7334 0000 0087 0066 0164  ......s4.....f.d
-000016d0: 0164 0284 0874 00a0 01a1 0044 0083 017d  .d...t.....D...}
-000016e0: 0274 0264 0364 0464 0564 0664 0764 089c  .t.d.d.d.d.d.d..
-000016f0: 057c 0274 0364 098d 037d 037c 0353 0029  .|.t.d...}.|.S.)
-00001700: 0a4e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
-00001710: 0000 0006 0000 0013 0000 0073 1c00 0000  ...........s....
-00001720: 6900 7c00 5d0a 7d01 7c01 8800 6a00 7401  i.|.].}.|...j.t.
-00001730: 7c01 8301 1900 9302 7102 5300 721f 0000  |.......q.S.r...
-00001740: 0029 0272 7500 0000 7204 0000 0029 0272  .).ru...r....).r
-00001750: 7100 0000 7272 0000 00a9 0172 3900 0000  q...rr.....r9...
-00001760: 721f 0000 0072 2000 0000 7274 0000 00e6  r....r ...rt....
-00001770: 0000 0073 0800 0000 0600 0202 0eff 06ff  ...s............
-00001780: 7a31 4f75 7470 7574 2e6d 616b 655f 7472  z1Output.make_tr
-00001790: 6565 5f63 6f6e 7472 6f6c 5f64 6963 742e  ee_control_dict.
-000017a0: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
-000017b0: 6d70 3efa 0332 2e30 da05 6173 6369 69da  mp>..2.0..ascii.
-000017c0: 0a64 6963 7469 6f6e 6172 797a 0822 7379  .dictionaryz."sy
-000017d0: 7374 656d 2272 1600 0000 2905 da07 7665  stem"r....)...ve
-000017e0: 7273 696f 6e72 5400 0000 da05 636c 6173  rsionrT.....clas
-000017f0: 73da 086c 6f63 6174 696f 6eda 066f 626a  s..location..obj
-00001800: 6563 74a9 0372 4100 0000 da08 6368 696c  ect..rA.....chil
-00001810: 6472 656e da06 6865 6164 6572 2904 7209  dren..header).r.
-00001820: 0000 00da 046b 6579 7372 0b00 0000 720a  .....keysr....r.
-00001830: 0000 0029 0472 5c00 0000 7239 0000 0072  ...).r\...r9...r
-00001840: 8200 0000 da04 7472 6565 721f 0000 0072  ......treer....r
-00001850: 7900 0000 7220 0000 00da 166d 616b 655f  y...r .....make_
-00001860: 7472 6565 5f63 6f6e 7472 6f6c 5f64 6963  tree_control_dic
-00001870: 74e5 0000 0073 1c00 0000 0a01 0602 06fe  t....s..........
-00001880: 0205 0202 0201 0201 0201 0201 04fb 0207  ................
-00001890: 0201 06f7 040b 7a1d 4f75 7470 7574 2e6d  ......z.Output.m
-000018a0: 616b 655f 7472 6565 5f63 6f6e 7472 6f6c  ake_tree_control
-000018b0: 5f64 6963 7463 0200 0000 0000 0000 0000  _dictc..........
-000018c0: 0000 0300 0000 0300 0000 4300 0000 7312  ..........C...s.
-000018d0: 0000 007c 00a0 007c 01a1 017d 027c 02a0  ...|...|...}.|..
-000018e0: 01a1 0053 0029 014e 2902 7286 0000 00da  ...S.).N).r.....
-000018f0: 0464 756d 7029 0372 5c00 0000 7239 0000  .dump).r\...r9..
-00001900: 0072 8500 0000 721f 0000 0072 1f00 0000  .r....r....r....
-00001910: 7220 0000 00da 166d 616b 655f 636f 6465  r .....make_code
-00001920: 5f63 6f6e 7472 6f6c 5f64 6963 74f8 0000  _control_dict...
-00001930: 0073 0400 0000 0a01 0801 7a1d 4f75 7470  .s........z.Outp
-00001940: 7574 2e6d 616b 655f 636f 6465 5f63 6f6e  ut.make_code_con
-00001950: 7472 6f6c 5f64 6963 7463 0200 0000 0000  trol_dictc......
-00001960: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
-00001970: 0000 7318 0000 007c 016a 0064 0164 0264  ..s....|.j.d.d.d
-00001980: 0369 0164 0464 058d 0301 0064 0053 0029  .i.d.d.....d.S.)
-00001990: 064e da15 7475 7262 756c 656e 6365 5f70  .N..turbulence_p
-000019a0: 726f 7065 7274 6965 73da 0f73 696d 756c  roperties..simul
-000019b0: 6174 696f 6e5f 7479 7065 5a07 6c61 6d69  ation_typeZ.lami
-000019c0: 6e61 72da 0454 4f44 4f72 7600 0000 a901  nar..TODOrv.....
-000019d0: 721a 0000 0029 0272 1d00 0000 7239 0000  r....).r....r9..
-000019e0: 0072 1f00 0000 721f 0000 0072 2000 0000  .r....r....r ...
-000019f0: da26 5f63 6f6d 706c 6574 655f 7061 7261  .&_complete_para
-00001a00: 6d73 5f74 7572 6275 6c65 6e63 655f 7072  ms_turbulence_pr
-00001a10: 6f70 6572 7469 6573 fc00 0000 730a 0000  operties....s...
-00001a20: 0004 0202 0106 0102 010a fd7a 2d4f 7574  ...........z-Out
-00001a30: 7075 742e 5f63 6f6d 706c 6574 655f 7061  put._complete_pa
-00001a40: 7261 6d73 5f74 7572 6275 6c65 6e63 655f  rams_turbulence_
-00001a50: 7072 6f70 6572 7469 6573 6302 0000 0000  propertiesc.....
-00001a60: 0000 0000 0000 0002 0000 0006 0000 0043  ...............C
-00001a70: 0000 0073 2000 0000 7400 6401 6402 6403  ...s ...t.d.d.d.
-00001a80: 6404 6405 9c04 6406 7c01 6a01 6a02 6901  d.d...d.|.j.j.i.
-00001a90: 7403 6407 8d03 5300 2908 4e72 7a00 0000  t.d...S.).Nrz...
-00001aa0: 727b 0000 0072 7c00 0000 7215 0000 0029  r{...r|...r....)
-00001ab0: 0472 7d00 0000 7254 0000 0072 7e00 0000  .r}...rT...r~...
-00001ac0: 7280 0000 005a 0e73 696d 756c 6174 696f  r....Z.simulatio
-00001ad0: 6e54 7970 6572 8100 0000 2904 720b 0000  nTyper....).r...
-00001ae0: 0072 8900 0000 728a 0000 0072 0a00 0000  .r....r....r....
-00001af0: 2902 725c 0000 0072 3900 0000 721f 0000  ).r\...r9...r...
-00001b00: 0072 1f00 0000 7220 0000 00da 1f6d 616b  .r....r .....mak
-00001b10: 655f 7472 6565 5f74 7572 6275 6c65 6e63  e_tree_turbulenc
-00001b20: 655f 7072 6f70 6572 7469 6573 0401 0000  e_properties....
-00001b30: 7314 0000 0002 0102 0202 0102 0102 0104  s...............
-00001b40: fc08 0702 ff02 0306 f67a 264f 7574 7075  .........z&Outpu
-00001b50: 742e 6d61 6b65 5f74 7265 655f 7475 7262  t.make_tree_turb
-00001b60: 756c 656e 6365 5f70 726f 7065 7274 6965  ulence_propertie
-00001b70: 7363 0200 0000 0000 0000 0000 0000 0400  sc..............
-00001b80: 0000 0700 0000 4300 0000 7386 0000 007c  ......C...s....|
-00001b90: 016a 0064 0164 0264 038d 0201 007c 016a  .j.d.d.d.....|.j
-00001ba0: 016a 0064 0464 0264 038d 027d 0264 0564  .j.d.d.d...}.d.d
-00001bb0: 0664 0764 0864 099c 047d 037c 026a 0064  .d.d.d...}.|.j.d
-00001bc0: 0a7c 0364 0b8d 0201 007c 026a 0064 0c7c  .|.d.....|.j.d.|
-00001bd0: 0364 0b8d 0201 0064 0d7c 026a 025f 037c  .d.....d.|.j._.|
-00001be0: 026a 0064 0e64 0f64 1064 1164 0d64 099c  .j.d.d.d.d.d.d..
-00001bf0: 0464 0b8d 0201 007c 016a 016a 0064 1264  .d.....|.j.j.d.d
-00001c00: 1364 1464 1564 0d64 169c 0464 0b8d 0201  .d.d.d.d...d....
-00001c10: 0064 0053 0029 174e da0b 6676 5f73 6f6c  .d.S.).N..fv_sol
-00001c20: 7574 696f 6e72 8b00 0000 a901 7277 0000  utionr......rw..
-00001c30: 00da 0773 6f6c 7665 7273 da03 5043 475a  ...solvers..PCGZ
-00001c40: 0344 4943 678d edb5 a0f7 c6b0 3e67 7b14  .DICg.......>g{.
-00001c50: ae47 e17a 843f 2904 7242 0000 005a 0e70  .G.z.?).rB...Z.p
-00001c60: 7265 636f 6e64 6974 696f 6e65 72da 0974  reconditioner..t
-00001c70: 6f6c 6572 616e 6365 da06 7265 6c54 6f6c  olerance..relTol
-00001c80: 7212 0000 0072 3000 0000 da06 7046 696e  r....r0.....pFin
-00001c90: 616c 7201 0000 0072 1300 0000 5a09 5042  alr....r....Z.PB
-00001ca0: 6943 4753 7461 625a 0444 494c 5567 3a8c  iCGStabZ.DILUg:.
-00001cb0: 30e2 8e79 453e 5a04 7069 736f e902 0000  0..yE>Z.piso....
-00001cc0: 00e9 0100 0000 7a07 2830 2030 2030 2929  ......z.(0 0 0))
-00001cd0: 045a 0b6e 436f 7272 6563 746f 7273 5a18  .Z.nCorrectorsZ.
-00001ce0: 6e4e 6f6e 4f72 7468 6f67 6f6e 616c 436f  nNonOrthogonalCo
-00001cf0: 7272 6563 746f 7273 da09 7052 6566 506f  rrectors..pRefPo
-00001d00: 696e 745a 0970 5265 6656 616c 7565 2904  intZ.pRefValue).
-00001d10: 721a 0000 0072 8f00 0000 7295 0000 0072  r....r....r....r
-00001d20: 9400 0000 2904 721d 0000 0072 3900 0000  ....).r....r9...
-00001d30: 7291 0000 0072 3100 0000 721f 0000 0072  r....r1...r....r
-00001d40: 1f00 0000 7220 0000 00da 1c5f 636f 6d70  ....r ....._comp
-00001d50: 6c65 7465 5f70 6172 616d 735f 6676 5f73  lete_params_fv_s
-00001d60: 6f6c 7574 696f 6e12 0100 0073 3400 0000  olution....s4...
-00001d70: 0e02 1001 0202 0201 0201 0201 06fc 0e07  ................
-00001d80: 0e01 0801 0401 0201 0202 0201 0201 0201  ................
-00001d90: 04fc 06fe 060a 0201 0202 0201 0201 0201  ................
-00001da0: 04fc 0afe 7a23 4f75 7470 7574 2e5f 636f  ....z#Output._co
-00001db0: 6d70 6c65 7465 5f70 6172 616d 735f 6676  mplete_params_fv
-00001dc0: 5f73 6f6c 7574 696f 6e63 0200 0000 0000  _solutionc......
-00001dd0: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
-00001de0: 0000 737e 0000 007c 016a 0064 0164 0264  ..s~...|.j.d.d.d
-00001df0: 038d 027d 027c 026a 0064 0464 0564 0669  ...}.|.j.d.d.d.i
-00001e00: 0164 078d 0201 007c 026a 0064 0864 0564  .d.....|.j.d.d.d
-00001e10: 0969 0164 078d 0201 007c 026a 0064 0a64  .i.d.....|.j.d.d
-00001e20: 0564 0b69 0164 078d 0201 007c 026a 0064  .d.i.d.....|.j.d
-00001e30: 0c64 0564 0d69 0164 078d 0201 007c 026a  .d.d.i.d.....|.j
-00001e40: 0064 0e64 0564 0f69 0164 078d 0201 007c  .d.d.d.i.d.....|
-00001e50: 026a 0064 1064 0564 1169 0164 078d 0201  .j.d.d.d.i.d....
-00001e60: 0064 0053 0029 124e da0a 6676 5f73 6368  .d.S.).N..fv_sch
-00001e70: 656d 6573 728b 0000 0072 9000 0000 5a0a  emesr....r....Z.
-00001e80: 6464 7453 6368 656d 6573 da07 6465 6661  ddtSchemes..defa
-00001e90: 756c 74da 0862 6163 6b77 6172 6472 3000  ult..backwardr0.
-00001ea0: 0000 5a0b 6772 6164 5363 6865 6d65 735a  ..Z.gradSchemesZ
-00001eb0: 0c6c 6561 7374 5371 7561 7265 735a 0a64  .leastSquaresZ.d
-00001ec0: 6976 5363 6865 6d65 73da 046e 6f6e 655a  ivSchemes..noneZ
-00001ed0: 106c 6170 6c61 6369 616e 5363 6865 6d65  .laplacianScheme
-00001ee0: 737a 1647 6175 7373 206c 696e 6561 7220  sz.Gauss linear 
-00001ef0: 636f 7272 6563 7465 645a 1469 6e74 6572  correctedZ.inter
-00001f00: 706f 6c61 7469 6f6e 5363 6865 6d65 73da  polationSchemes.
-00001f10: 066c 696e 6561 725a 0d73 6e47 7261 6453  .linearZ.snGradS
-00001f20: 6368 656d 6573 5a09 636f 7272 6563 7465  chemesZ.correcte
-00001f30: 6472 8c00 0000 2903 721d 0000 0072 3900  dr....).r....r9.
-00001f40: 0000 729a 0000 0072 1f00 0000 721f 0000  ..r....r....r...
-00001f50: 0072 2000 0000 da1b 5f63 6f6d 706c 6574  .r ....._complet
-00001f60: 655f 7061 7261 6d73 5f66 765f 7363 6865  e_params_fv_sche
-00001f70: 6d65 7334 0100 0073 1600 0000 0e02 1201  mes4...s........
-00001f80: 1201 1201 0401 0801 06ff 0403 0801 06ff  ................
-00001f90: 1603 7a22 4f75 7470 7574 2e5f 636f 6d70  ..z"Output._comp
-00001fa0: 6c65 7465 5f70 6172 616d 735f 6676 5f73  lete_params_fv_s
-00001fb0: 6368 656d 6573 6302 0000 0000 0000 0000  chemesc.........
-00001fc0: 0000 0003 0000 0009 0000 0043 0000 0073  ...........C...s
-00001fd0: 2a00 0000 6401 6401 6401 6402 6402 6402  *...d.d.d.d.d.d.
-00001fe0: 6403 6400 6404 9c08 7d02 7c01 6a00 6405  d.d.d...}.|.j.d.
-00001ff0: 7c02 6406 6407 8d03 0100 6400 5300 2908  |.d.d.....d.S.).
-00002000: 4ee9 2800 0000 6700 0000 0000 00f0 3fda  N.(...g.......?.
-00002010: 016d 2908 da02 6e78 da02 6e79 da02 6e7a  .m)...nx..ny..nz
-00002020: da02 6c78 da02 6c79 da02 6c7a da06 6d65  ..lx..ly..lz..me
-00002030: 7472 6963 da05 7363 616c 6572 3f00 0000  tric..scaler?...
-00002040: 728b 0000 0072 7600 0000 728c 0000 0029  r....rv...r....)
-00002050: 0372 1d00 0000 7239 0000 0072 9b00 0000  .r....r9...r....
-00002060: 721f 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
-00002070: 205f 636f 6d70 6c65 7465 5f70 6172 616d   _complete_param
-00002080: 735f 626c 6f63 6b5f 6d65 7368 5f64 6963  s_block_mesh_dic
-00002090: 7442 0100 0073 1c00 0000 0203 0201 0201  tB...s..........
-000020a0: 0201 0201 0201 0201 0201 06f8 040b 0201  ................
-000020b0: 0201 0201 0afd 7a27 4f75 7470 7574 2e5f  ......z'Output._
-000020c0: 636f 6d70 6c65 7465 5f70 6172 616d 735f  complete_params_
-000020d0: 626c 6f63 6b5f 6d65 7368 5f64 6963 7429  block_mesh_dict)
-000020e0: 024e 4e29 18da 085f 5f6e 616d 655f 5fda  .NN)...__name__.
-000020f0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00002100: 7561 6c6e 616d 655f 5f72 2500 0000 7226  ualname__r%...r&
-00002110: 0000 0072 2700 0000 da0b 636c 6173 736d  ...r'.....classm
-00002120: 6574 686f 6472 2100 0000 721b 0000 0072  ethodr!...r....r
-00002130: 2900 0000 723b 0000 0072 4900 0000 7247  )...r;...rI...rG
-00002140: 0000 0072 6900 0000 726a 0000 0072 7800  ...ri...rj...rx.
-00002150: 0000 7286 0000 0072 8800 0000 728d 0000  ..r....r....r...
-00002160: 0072 8e00 0000 7299 0000 0072 9f00 0000  .r....r....r....
-00002170: 72aa 0000 00da 0d5f 5f63 6c61 7373 6365  r......__classce
-00002180: 6c6c 5f5f 721f 0000 0072 1f00 0000 7261  ll__r....r....ra
-00002190: 0000 0072 2000 0000 7211 0000 001a 0000  ...r ...r.......
-000021a0: 0073 3c00 0000 0800 0801 0801 0801 0202  .s<.............
-000021b0: 0a01 020a 0a01 0203 0a01 020b 0a01 0e1d  ................
-000021c0: 024d 0a01 0c04 081e 0211 0a01 080b 0813  .M..............
-000021d0: 0204 0a01 0807 020e 0a01 0221 0a01 020d  ...........!....
-000021e0: 1201 7211 0000 0029 1c72 6300 0000 726c  ..r....).rc...rl
-000021f0: 0000 0072 3600 0000 da07 7061 7468 6c69  ...r6.....pathli
-00002200: 6272 0200 0000 da0a 696e 666c 6563 7469  br......inflecti
-00002210: 6f6e 7204 0000 005a 0b66 6c75 6964 6479  onr....Z.fluiddy
-00002220: 6e2e 696f 7205 0000 005a 0d66 6c75 6964  n.ior....Z.fluid
-00002230: 6479 6e2e 7574 696c 7206 0000 005a 1466  dyn.utilr....Z.f
-00002240: 6c75 6964 7369 6d5f 636f 7265 2e6f 7574  luidsim_core.out
-00002250: 7075 7472 0700 0000 da14 666c 7569 6473  putr......fluids
-00002260: 696d 5f63 6f72 652e 7061 7261 6d73 7208  im_core.paramsr.
-00002270: 0000 00da 1d66 6c75 6964 7369 6d66 6f61  .....fluidsimfoa
-00002280: 6d2e 666f 616d 5f69 6e70 7574 5f66 696c  m.foam_input_fil
-00002290: 6573 7209 0000 0072 0a00 0000 720b 0000  esr....r....r...
-000022a0: 005a 2866 6c75 6964 7369 6d66 6f61 6d2e  .Z(fluidsimfoam.
-000022b0: 666f 616d 5f69 6e70 7574 5f66 696c 6573  foam_input_files
-000022c0: 2e67 656e 6572 6174 6f72 7372 0c00 0000  .generatorsr....
-000022d0: 720d 0000 0072 0e00 0000 5a10 666c 7569  r....r....Z.flui
-000022e0: 6473 696d 666f 616d 2e6c 6f67 720f 0000  dsimfoam.logr...
-000022f0: 00da 1466 6c75 6964 7369 6d66 6f61 6d2e  ...fluidsimfoam.
-00002300: 736f 6c76 6572 7372 1000 0000 7211 0000  solversr....r...
-00002310: 0072 1f00 0000 721f 0000 0072 1f00 0000  .r....r....r....
-00002320: 7220 0000 00da 083c 6d6f 6475 6c65 3e01  r .....<module>.
-00002330: 0000 0073 1c00 0000 0800 0801 0801 0c01  ...s............
-00002340: 0c02 0c02 0c01 0c01 0c01 1401 1405 0c05  ................
-00002350: 0c01 1403                                ....
+00000160: 554c 545f 4845 4144 4552 da12 436f 6e73  ULT_HEADER..Cons
+00000170: 7461 6e74 4669 6c65 4865 6c70 6572 da0d  tantFileHelper..
+00000180: 466f 616d 496e 7075 7446 696c 6529 02da  FoamInputFile)..
+00000190: 0a49 6e70 7574 4669 6c65 73da 186e 6577  .InputFiles..new
+000001a0: 5f66 696c 655f 6765 6e65 7261 746f 725f  _file_generator_
+000001b0: 636c 6173 7329 01da 066c 6f67 6765 7229  class)...logger)
+000001c0: 01da 1267 6574 5f73 6f6c 7665 725f 7061  ...get_solver_pa
+000001d0: 636b 6167 6563 0000 0000 0000 0000 0000  ckagec..........
+000001e0: 0000 0000 0000 0400 0000 0000 0000 73c0  ..............s.
+000001f0: 0000 0065 005a 0164 005a 0264 0164 0267  ...e.Z.d.Z.d.d.g
+00000200: 025a 0364 0364 0467 025a 0467 0064 05a2  .Z.d.d.g.Z.g.d..
+00000210: 015a 0565 065a 0765 0864 0464 0664 0769  .Z.e.Z.e.d.d.d.i
+00000220: 0183 025a 0965 0a64 0864 0984 0083 015a  ...Z.e.d.d.....Z
+00000230: 0b65 0a64 0a64 0b84 0083 015a 0c65 0a64  .e.d.d.....Z.e.d
+00000240: 0c64 0d84 0083 015a 0d65 0a64 0e64 0f84  .d.....Z.e.d.d..
+00000250: 0083 015a 0e64 2187 0066 0164 1164 1284  ...Z.d!..f.d.d..
+00000260: 095a 0f65 0a64 1364 1484 0083 015a 1087  .Z.e.d.d.....Z..
+00000270: 0066 0164 1564 1684 085a 1164 1764 1884  .f.d.d...Z.d.d..
+00000280: 005a 1265 0a64 1964 1a84 0083 015a 1364  .Z.e.d.d.....Z.d
+00000290: 1b64 1c84 005a 1464 1d64 1e84 005a 1565  .d...Z.d.d...Z.e
+000002a0: 0a64 1f64 2084 0083 015a 1687 0004 005a  .d.d ....Z.....Z
+000002b0: 1753 0029 22da 064f 7574 7075 74da 0170  .S.)"..Output..p
+000002c0: da01 55da 1374 7261 6e73 706f 7274 5072  ..U..transportPr
+000002d0: 6f70 6572 7469 6573 da14 7475 7262 756c  operties..turbul
+000002e0: 656e 6365 5072 6f70 6572 7469 6573 2903  enceProperties).
+000002f0: da0b 636f 6e74 726f 6c44 6963 74da 0966  ..controlDict..f
+00000300: 7653 6368 656d 6573 5a0a 6676 536f 6c75  vSchemesZ.fvSolu
+00000310: 7469 6f6e da0e 7369 6d75 6c61 7469 6f6e  tion..simulation
+00000320: 5479 7065 da07 6c61 6d69 6e61 7263 0200  Type..laminarc..
+00000330: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+00000340: 0000 4300 0000 7328 0000 007c 016a 006a  ..C...s(...|.j.j
+00000350: 01a0 0264 01a1 017d 027c 00a0 037c 02a1  ...d...}.|...|..
+00000360: 0101 007c 016a 006a 01a0 04a1 0001 0064  ...|.j.j.......d
+00000370: 0253 0029 037a 6643 6f6d 706c 6574 6520  .S.).zfComplete 
+00000380: 7468 6520 696e 666f 5f73 6f6c 7665 7220  the info_solver 
+00000390: 696e 7374 616e 6365 2077 6974 6820 6368  instance with ch
+000003a0: 696c 6420 636c 6173 7320 6465 7461 696c  ild class detail
+000003b0: 7320 286d 6f64 756c 650a 2020 2020 2020  s (module.      
+000003c0: 2020 616e 6420 636c 6173 7320 6e61 6d65    and class name
+000003d0: 7329 2e0a 0a20 2020 2020 2020 20da 0763  s)...        ..c
+000003e0: 6c61 7373 6573 4e29 0572 1a00 0000 7211  lassesN).r....r.
+000003f0: 0000 00da 0a5f 7365 745f 6368 696c 64da  ....._set_child.
+00000400: 185f 7365 745f 696e 666f 5f73 6f6c 7665  ._set_info_solve
+00000410: 725f 636c 6173 7365 73da 1563 6f6d 706c  r_classes..compl
+00000420: 6574 655f 7769 7468 5f63 6c61 7373 6573  ete_with_classes
+00000430: 2903 da03 636c 73da 0b69 6e66 6f5f 736f  )...cls..info_so
+00000440: 6c76 6572 721a 0000 00a9 0072 2000 0000  lverr......r ...
+00000450: fa3d 2f68 6f6d 652f 7069 6572 7265 2f44  .=/home/pierre/D
+00000460: 6576 2f66 6c75 6964 7369 6d66 6f61 6d2f  ev/fluidsimfoam/
+00000470: 7372 632f 666c 7569 6473 696d 666f 616d  src/fluidsimfoam
+00000480: 2f6f 7574 7075 742f 6261 7365 2e70 79da  /output/base.py.
+00000490: 155f 636f 6d70 6c65 7465 5f69 6e66 6f5f  ._complete_info_
+000004a0: 736f 6c76 6572 2400 0000 7306 0000 000e  solver$...s.....
+000004b0: 060a 0110 027a 1c4f 7574 7075 742e 5f63  .....z.Output._c
+000004c0: 6f6d 706c 6574 655f 696e 666f 5f73 6f6c  omplete_info_sol
+000004d0: 7665 7263 0200 0000 0000 0000 0000 0000  verc............
+000004e0: 0200 0000 0100 0000 4300 0000 7304 0000  ........C...s...
+000004f0: 0064 0153 0029 027a 2e53 6574 2074 6865  .d.S.).z.Set the
+00000500: 2063 6c61 7373 6573 2066 6f72 2069 6e66   classes for inf
+00000510: 6f5f 736f 6c76 6572 2e63 6c61 7373 6573  o_solver.classes
+00000520: 2e4f 7574 7075 744e 7220 0000 0029 0272  .OutputNr ...).r
+00000530: 1e00 0000 721a 0000 0072 2000 0000 7220  ....r....r ...r 
+00000540: 0000 0072 2100 0000 721c 0000 002f 0000  ...r!...r..../..
+00000550: 0073 0200 0000 0400 7a1f 4f75 7470 7574  .s......z.Output
+00000560: 2e5f 7365 745f 696e 666f 5f73 6f6c 7665  ._set_info_solve
+00000570: 725f 636c 6173 7365 7363 0100 0000 0000  r_classesc......
+00000580: 0000 0000 0000 0400 0000 0700 0000 4300  ..............C.
+00000590: 0000 7362 0000 0069 0004 007d 017c 005f  ..sb...i...}.|._
+000005a0: 007c 006a 0144 005d 0c7d 0274 027c 0283  .|.j.D.].}.t.|..
+000005b0: 017c 017c 02a0 0364 0164 02a1 023c 0071  .|.|...d.d...<.q
+000005c0: 087c 006a 0444 005d 097d 0374 027c 0364  .|.j.D.].}.t.|.d
+000005d0: 0383 027c 017c 033c 0071 187c 006a 0544  ...|.|.<.q.|.j.D
+000005e0: 005d 097d 0374 027c 0364 0483 027c 017c  .].}.t.|.d...|.|
+000005f0: 033c 0071 2564 0053 0029 054e da01 2eda  .<.q%d.S.).N....
+00000600: 015f da08 636f 6e73 7461 6e74 da06 7379  ._..constant..sy
+00000610: 7374 656d 2906 da18 5f66 696c 655f 6765  stem)..._file_ge
+00000620: 6e65 7261 746f 7273 5f63 6c61 7373 6573  nerators_classes
+00000630: da0e 7661 7269 6162 6c65 5f6e 616d 6573  ..variable_names
+00000640: 720e 0000 00da 0772 6570 6c61 6365 da14  r......replace..
+00000650: 636f 6e73 7461 6e74 5f66 696c 6573 5f6e  constant_files_n
+00000660: 616d 6573 da12 7379 7374 656d 5f66 696c  ames..system_fil
+00000670: 6573 5f6e 616d 6573 2904 721e 0000 0072  es_names).r....r
+00000680: 1a00 0000 5a0d 7661 7269 6162 6c65 5f6e  ....Z.variable_n
+00000690: 616d 65da 0966 696c 655f 6e61 6d65 7220  ame..file_namer 
+000006a0: 0000 0072 2000 0000 7221 0000 00da 1e5f  ...r ...r!....._
+000006b0: 7365 7475 705f 6669 6c65 5f67 656e 6572  setup_file_gener
+000006c0: 6174 6f72 735f 636c 6173 7365 7333 0000  ators_classes3..
+000006d0: 0073 1400 0000 0a02 0a01 0201 0201 12ff  .s..............
+000006e0: 0a04 1001 0a02 1001 04ff 7a25 4f75 7470  ..........z%Outp
+000006f0: 7574 2e5f 7365 7475 705f 6669 6c65 5f67  ut._setup_file_g
+00000700: 656e 6572 6174 6f72 735f 636c 6173 7365  enerators_classe
+00000710: 7363 0300 0000 0000 0000 0000 0000 0400  sc..............
+00000720: 0000 0600 0000 4300 0000 7372 0000 007c  ......C...sr...|
+00000730: 00a0 00a1 0001 0074 017c 017c 027c 006a  .......t.|.|.|.j
+00000740: 02a0 03a1 0083 0301 007c 01a0 0474 0564  .........|...t.d
+00000750: 0164 0264 038d 02a1 0101 007c 016a 0664  .d.d.......|.j.d
+00000760: 0464 0164 0564 069c 0264 078d 0201 007c  .d.d.d...d.....|
+00000770: 016a 07a0 0874 09a0 0a64 08a1 01a1 0101  .j...t...d......
+00000780: 007c 026a 0b6a 0ca0 0da1 007d 0374 017c  .|.j.j.....}.t.|
+00000790: 017c 027c 03a0 03a1 0083 0301 0064 0953  .|.|.........d.S
+000007a0: 0029 0a7a 3e54 6869 7320 7374 6174 6963  .).z>This static
+000007b0: 206d 6574 686f 6420 6973 2075 7365 6420   method is used 
+000007c0: 746f 2063 6f6d 706c 6574 6520 7468 6520  to complete the 
+000007d0: 2a70 6172 616d 732a 2063 6f6e 7461 696e  *params* contain
+000007e0: 6572 2e54 da03 7275 6e29 02da 0f4e 4557  er.T..run)...NEW
+000007f0: 5f44 4952 5f52 4553 554c 5453 5a13 7368  _DIR_RESULTSZ.sh
+00000800: 6f72 745f 6e61 6d65 5f74 7970 655f 7275  ort_name_type_ru
+00000810: 6eda 066f 7574 7075 74da 0029 02da 0b48  n..output..)...H
+00000820: 4153 5f54 4f5f 5341 5645 da0d 7375 625f  AS_TO_SAVE..sub_
+00000830: 6469 7265 6374 6f72 7929 01da 0761 7474  directory)...att
+00000840: 7269 6273 612e 0100 000a 2020 2020 2d20  ribsa.....    - 
+00000850: 6060 4841 535f 544f 5f53 4156 4560 603a  ``HAS_TO_SAVE``:
+00000860: 2062 6f6f 6c20 2864 6566 6175 6c74 3a20   bool (default: 
+00000870: 5472 7565 2920 4966 2046 616c 7365 2c20  True) If False, 
+00000880: 6e6f 7468 696e 6720 6e65 7720 6973 2073  nothing new is s
+00000890: 6176 6564 2069 6e0a 2020 2020 2020 7468  aved in.      th
+000008a0: 6520 6469 7265 6374 6f72 7920 6f66 2074  e directory of t
+000008b0: 6865 2073 696d 756c 6174 696f 6e2e 0a20  he simulation.. 
+000008c0: 2020 202d 2060 6073 7562 5f64 6972 6563     - ``sub_direc
+000008d0: 746f 7279 6060 3a20 7374 7220 2864 6566  tory``: str (def
+000008e0: 6175 6c74 3a20 2222 2920 4120 6e61 6d65  ault: "") A name
+000008f0: 206f 6620 6120 7375 622d 6469 7265 6374   of a sub-direct
+00000900: 6f72 7920 2872 656c 6174 6976 650a 2020  ory (relative.  
+00000910: 2020 2020 746f 2024 464c 5549 4444 594e      to $FLUIDDYN
+00000920: 5f50 4154 485f 5343 5241 5443 4829 2077  _PATH_SCRATCH) w
+00000930: 6865 7265 696e 2074 6865 2064 6972 6563  herein the direc
+00000940: 746f 7279 206f 6620 7468 6520 7369 6d75  tory of the simu
+00000950: 6c61 7469 6f6e 0a20 2020 2020 2028 6060  lation.      (``
+00000960: 7061 7468 5f72 756e 6060 2920 6973 2073  path_run``) is s
+00000970: 6176 6564 2e0a 0a4e 290e 722d 0000 0072  aved...N).r-...r
+00000980: 0800 0000 7227 0000 00da 0676 616c 7565  ....r'.....value
+00000990: 73da 0c5f 7365 745f 6174 7472 6962 73da  s.._set_attribs.
+000009a0: 0464 6963 7472 1b00 0000 7230 0000 00da  .dictr....r0....
+000009b0: 085f 7365 745f 646f 63da 0874 6578 7477  ._set_doc..textw
+000009c0: 7261 70da 0664 6564 656e 7472 1a00 0000  rap..dedentr....
+000009d0: 7211 0000 00da 0e69 6d70 6f72 745f 636c  r......import_cl
+000009e0: 6173 7365 7329 0472 1e00 0000 da06 7061  asses).r......pa
+000009f0: 7261 6d73 721f 0000 00da 0c64 6963 745f  ramsr......dict_
+00000a00: 636c 6173 7365 7372 2000 0000 7220 0000  classesr ...r ..
+00000a10: 0072 2100 0000 da1d 5f63 6f6d 706c 6574  .r!....._complet
+00000a20: 655f 7061 7261 6d73 5f77 6974 685f 6465  e_params_with_de
+00000a30: 6661 756c 7441 0000 0073 1e00 0000 0804  faultA...s......
+00000a40: 0201 0c01 04ff 1205 0401 0a01 06ff 0603  ................
+00000a50: 0401 0201 02ff 04ff 0c0d 1401 7a24 4f75  ............z$Ou
+00000a60: 7470 7574 2e5f 636f 6d70 6c65 7465 5f70  tput._complete_p
+00000a70: 6172 616d 735f 7769 7468 5f64 6566 6175  arams_with_defau
+00000a80: 6c74 4e63 0300 0000 0000 0000 0000 0000  ltNc............
+00000a90: 0b00 0000 0800 0000 0300 0000 733c 0200  ............s<..
+00000aa0: 007c 017c 005f 007a 087c 016a 016a 026a  .|.|._.z.|.j.j.j
+00000ab0: 037c 005f 0457 006e 0904 0074 0579 1401  .|._.W.n...t.y..
+00000ac0: 0001 0001 0059 006e 0777 0074 067c 006a  .....Y.n.w.t.|.j
+00000ad0: 0483 017c 005f 077c 00a0 08a1 007c 005f  ...|._.|.....|._
+00000ae0: 097c 0172 2e7c 016a 0a6a 0b7c 005f 0a74  .|.r.|.j.j.|._.t
+00000af0: 0c83 00a0 0d7c 01a1 0101 006e 0f7c 0272  .....|.....n.|.r
+00000b00: 357c 026a 0b7c 005f 0a6e 0864 007c 005f  5|.j.|._.n.d.|._
+00000b10: 0a74 0ea0 0f64 01a1 0101 007c 0173 4164  .t...d.....|.sAd
+00000b20: 0053 0074 107c 006a 1183 017c 005f 1174  .S.t.|.j...|._.t
+00000b30: 127c 0083 017c 005f 137c 016a 016a 026a  .|...|._.|.j.j.j
+00000b40: 146a 15a0 16a1 007d 037c 03a0 17a1 0044  .j.....}.|.....D
+00000b50: 005d 265c 027d 047d 0574 187c 007c 0583  .]&\.}.}.t.|.|..
+00000b60: 0272 6271 5874 197c 0483 017d 067c 006a  .rbqXt.|...}.|.j
+00000b70: 0004 006a 1a64 02a0 1b64 037c 069b 0064  ...j.d...d.|...d
+00000b80: 049d 037c 05a1 0237 0002 005f 1a74 1c7c  ...|...7..._.t.|
+00000b90: 007c 067c 057c 0083 0183 0301 0071 5874  .|.|.|.......qXt
+00000ba0: 1d7c 0064 0583 0273 887c 00a0 1ea1 0001  .|.d...s.|......
+00000bb0: 0069 007d 077c 006a 1fa0 17a1 0044 005d  .i.}.|.j.....D.]
+00000bc0: 255c 027d 047d 0574 197c 0483 017d 067c  %\.}.}.t.|...}.|
+00000bd0: 056a 207c 0776 0172 a37c 0467 017c 077c  .j |.v.r.|.g.|.|
+00000be0: 056a 203c 006e 087c 077c 056a 2019 00a0  .j <.n.|.|.j ...
+00000bf0: 217c 04a1 0101 0074 1c7c 006a 137c 067c  !|.....t.|.j.|.|
+00000c00: 057c 0083 0183 0301 0071 8f7c 0772 dc7c  .|.......q.|.r.|
+00000c10: 006a 0004 006a 1a64 0637 0002 005f 1a7c  .j...j.d.7..._.|
+00000c20: 07a0 17a1 0044 005d 185c 027d 087d 097c  .....D.].\.}.}.|
+00000c30: 006a 0004 006a 1a64 077c 0864 0817 0064  .j...j.d.|.d...d
+00000c40: 099b 0464 0aa0 227c 09a1 019b 0064 0b9d  ...d.."|.....d..
+00000c50: 0437 0002 005f 1a71 c374 236a 2464 0c6b  .7..._.q.t#j$d.k
+00000c60: 0272 e97c 006a 2572 e97c 006a 006a 0a6a  .r.|.j%r.|.j.j.j
+00000c70: 2673 eb64 0053 007c 006a 1164 0d1b 00a0  &s.d.S.|.j.d....
+00000c80: 27a1 0001 007c 006a 1164 0e1b 00a0 27a1  '....|.j.d....'.
+00000c90: 0001 007c 006a 1164 0f1b 00a0 27a1 0001  ...|.j.d....'...
+00000ca0: 0074 287c 006a 1383 01a0 29a1 0044 005d  .t(|.j....)..D.]
+00000cb0: 147d 0a74 1d7c 0a64 1083 0290 0172 1a7c  .}.t.|.d.....r.|
+00000cc0: 0a6a 2aa0 2b64 0da1 0190 0172 1a7c 0aa0  .j*.+d.....r.|..
+00000cd0: 2ca1 0001 0090 0171 0764 0053 0029 114e  ,......q.d.S.).N
+00000ce0: 7a45 496e 6974 6961 6c69 7a69 6e67 204f  zEInitializing O
+00000cf0: 7574 7075 7420 636c 6173 7320 7769 7468  utput class with
+00000d00: 6f75 7420 7369 6d20 6f72 2070 6172 616d  out sim or param
+00000d10: 7320 6d69 6768 7420 6c65 6164 2074 6f20  s might lead to 
+00000d20: 6572 726f 7273 2e7a 097b 3a32 3873 7d7b  errors.z.{:28s}{
+00000d30: 7d0a 7a0b 7369 6d2e 6f75 7470 7574 2e7a  }.z.sim.output.z
+00000d40: 023a 2072 2700 0000 7a0d 696e 7075 745f  .: r'...z.input_
+00000d50: 6669 6c65 733a 0a7a 0720 202d 2069 6e20  files:.z.  - in 
+00000d60: fa01 3a5a 0331 3273 da01 20da 010a 7201  ..:Z.12s.. ...r.
+00000d70: 0000 0072 2600 0000 da01 3072 2500 0000  ...r&.....0r%...
+00000d80: da0d 6765 6e65 7261 7465 5f66 696c 6529  ..generate_file)
+00000d90: 2dda 0373 696d da04 696e 666f da06 736f  -..sim..info..so
+00000da0: 6c76 6572 da0a 7368 6f72 745f 6e61 6d65  lver..short_name
+00000db0: da0b 6e61 6d65 5f73 6f6c 7665 72da 0e41  ..name_solver..A
+00000dc0: 7474 7269 6275 7465 4572 726f 7272 1000  ttributeErrorr..
+00000dd0: 0000 da07 7061 636b 6167 65da 1767 6574  ....package..get
+00000de0: 5f70 6174 685f 736f 6c76 6572 5f70 6163  _path_solver_pac
+00000df0: 6b61 6765 5a13 7061 7468 5f73 6f6c 7665  kageZ.path_solve
+00000e00: 725f 7061 636b 6167 6572 3c00 0000 7230  r_packager<...r0
+00000e10: 0000 00da 0573 7570 6572 da08 5f5f 696e  .....super..__in
+00000e20: 6974 5f5f 720f 0000 00da 0777 6172 6e69  it__r......warni
+00000e30: 6e67 7202 0000 00da 0870 6174 685f 7275  ngr......path_ru
+00000e40: 6e72 0d00 0000 da0b 696e 7075 745f 6669  nr......input_fi
+00000e50: 6c65 7372 1a00 0000 7211 0000 0072 3b00  lesr....r....r;.
+00000e60: 0000 da05 6974 656d 73da 0a69 7369 6e73  ....items..isins
+00000e70: 7461 6e63 6572 0400 0000 da11 5f6f 626a  tancer......_obj
+00000e80: 6563 7473 5f74 6f5f 7072 696e 74da 0666  ects_to_print..f
+00000e90: 6f72 6d61 74da 0773 6574 6174 7472 da07  ormat..setattr..
+00000ea0: 6861 7361 7474 7272 2d00 0000 7227 0000  hasattrr-...r'..
+00000eb0: 00da 0864 6972 5f6e 616d 65da 0661 7070  ...dir_name..app
+00000ec0: 656e 64da 046a 6f69 6e72 0600 0000 da04  end..joinr......
+00000ed0: 7261 6e6b da0c 5f68 6173 5f74 6f5f 7361  rank.._has_to_sa
+00000ee0: 7665 722f 0000 00da 056d 6b64 6972 da04  ver/.....mkdir..
+00000ef0: 7661 7273 7235 0000 00da 0872 656c 5f70  varsr5.....rel_p
+00000f00: 6174 68da 0a73 7461 7274 7377 6974 6872  ath..startswithr
+00000f10: 4300 0000 290b da04 7365 6c66 7244 0000  C...)...selfrD..
+00000f20: 0072 3c00 0000 723d 0000 00da 0863 6c73  .r<...r=.....cls
+00000f30: 5f6e 616d 65da 0543 6c61 7373 da08 6f62  _name..Class..ob
+00000f40: 6a5f 6e61 6d65 5a13 666f 725f 7374 725f  j_nameZ.for_str_
+00000f50: 696e 7075 745f 6669 6c65 7372 5700 0000  input_filesrW...
+00000f60: 7250 0000 00da 0e66 696c 655f 6765 6e65  rP.....file_gene
+00000f70: 7261 746f 72a9 01da 095f 5f63 6c61 7373  rator....__class
+00000f80: 5f5f 7220 0000 0072 2100 0000 724d 0000  __r ...r!...rM..
+00000f90: 005f 0000 0073 8000 0000 0601 0201 1001  ._...s..........
+00000fa0: 0c01 0401 02ff 0c03 0a02 0402 0a02 0e01  ................
+00000fb0: 0401 0a02 0602 0401 0201 04ff 0404 0401  ................
+00000fc0: 0c02 0a02 1002 1001 0a01 0201 0801 0c01  ................
+00000fd0: 0c01 08ff 1203 0a02 0801 0401 1201 0801  ................
+00000fe0: 0a02 0e01 1002 1401 0402 1001 1001 0801  ................
+00000ff0: 1a01 08ff 0805 02ff 0402 02fe 0803 02fd  ................
+00001000: 0405 0e02 0e01 0e01 1202 0201 0401 06ff  ................
+00001010: 0a02 04fe 0803 0480 04fc 7a0f 4f75 7470  ..........z.Outp
+00001020: 7574 2e5f 5f69 6e69 745f 5f63 0100 0000  ut.__init__c....
+00001030: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00001040: 4300 0000 7312 0000 0074 0074 01a0 027c  C...s....t.t...|
+00001050: 00a1 016a 0383 016a 0453 0029 017a 2847  ...j...j.S.).z(G
+00001060: 6574 2074 6865 2070 6174 6820 746f 7761  et the path towa
+00001070: 7264 7320 7468 6520 736f 6c76 6572 2070  rds the solver p
+00001080: 6163 6b61 6765 2e29 0572 0200 0000 da07  ackage.).r......
+00001090: 696e 7370 6563 74da 0967 6574 6d6f 6475  inspect..getmodu
+000010a0: 6c65 da08 5f5f 6669 6c65 5f5f da06 7061  le..__file__..pa
+000010b0: 7265 6e74 2901 721e 0000 0072 2000 0000  rent).r....r ...
+000010c0: 7220 0000 0072 2100 0000 724b 0000 00ac  r ...r!...rK....
+000010d0: 0000 0073 0200 0000 1203 7a1e 4f75 7470  ...s......z.Outp
+000010e0: 7574 2e67 6574 5f70 6174 685f 736f 6c76  ut.get_path_solv
+000010f0: 6572 5f70 6163 6b61 6765 6301 0000 0000  er_packagec.....
+00001100: 0000 0000 0000 0005 0000 0008 0000 0003  ................
+00001110: 0000 0073 c800 0000 7400 6a01 6401 6b02  ...s....t.j.d.k.
+00001120: 720d 7402 6402 7c00 6a03 9b00 9d02 8301  r.t.d.|.j.......
+00001130: 0100 7404 8300 8f0d 0100 7405 8300 a006  ..t.......t.....
+00001140: a100 0100 5700 6403 0400 0400 8303 0100  ....W.d.........
+00001150: 6e08 3100 7320 7701 0100 0100 0100 5900  n.1.s w.......Y.
+00001160: 0100 7407 a008 7c00 6a09 6a0a a101 0100  ..t...|.j.j.....
+00001170: 7400 6a01 6401 6b02 723d 7c00 6a0b 723d  t.j.d.k.r=|.j.r=
+00001180: 7c00 6a09 6a0c 6a0d 723d 7c00 a00e a100  |.j.j.j.r=|.....
+00001190: 0100 740f 7c00 6a03 8301 7d01 7c01 6404  ..t.|.j...}.|.d.
+000011a0: 1b00 7d02 7c02 6a10 6405 6406 8d01 0100  ..}.|.j.d.d.....
+000011b0: 6407 4400 5d13 7d03 7c02 7c03 1b00 7d04  d.D.].}.|.|...}.
+000011c0: 7c04 a011 a100 7259 714e 7412 a013 7c01  |.....rYqNt...|.
+000011d0: 7c03 1b00 7c04 a102 0100 714e 6403 5300  |...|.....qNd.S.
+000011e0: 2908 7a21 4c6f 6773 2069 6e66 6f20 6f6e  ).z!Logs info on
+000011f0: 2069 6e73 7461 6e74 6961 7465 6420 636c   instantiated cl
+00001200: 6173 7365 7372 0100 0000 7a0a 7061 7468  assesr....z.path
+00001210: 5f72 756e 3a20 4e7a 0e2e 6461 7461 5f66  _run: Nz..data_f
+00001220: 6c75 6964 7369 6d54 2901 da08 6578 6973  luidsimT)...exis
+00001230: 745f 6f6b 2902 7a0f 696e 666f 5f73 6f6c  t_ok).z.info_sol
+00001240: 7665 722e 786d 6c7a 1070 6172 616d 735f  ver.xmlz.params_
+00001250: 7369 6d75 6c2e 786d 6c29 1472 0600 0000  simul.xml).r....
+00001260: 725a 0000 00da 0570 7269 6e74 724f 0000  rZ.....printrO..
+00001270: 0072 0500 0000 724c 0000 00da 0970 6f73  .r....rL.....pos
+00001280: 745f 696e 6974 720f 0000 0072 4500 0000  t_initr....rE...
+00001290: 7244 0000 0072 5300 0000 725b 0000 0072  rD...rS...r[...r
+000012a0: 3c00 0000 722f 0000 00da 2870 6f73 745f  <...r/....(post_
+000012b0: 696e 6974 5f63 7265 6174 655f 6164 6469  init_create_addi
+000012c0: 7469 6f6e 616c 5f73 6f75 7263 655f 6669  tional_source_fi
+000012d0: 6c65 7372 0200 0000 725c 0000 00da 0665  lesr....r\.....e
+000012e0: 7869 7374 73da 0673 6875 7469 6cda 0463  xists..shutil..c
+000012f0: 6f70 7929 0572 6000 0000 724f 0000 005a  opy).r`...rO...Z
+00001300: 1270 6174 685f 696e 666f 5f66 6c75 6964  .path_info_fluid
+00001310: 7369 6d72 2c00 0000 5a08 7061 7468 5f6e  simr,...Z.path_n
+00001320: 6577 7265 0000 0072 2000 0000 7221 0000  ewre...r ...r!..
+00001330: 0072 6d00 0000 b100 0000 732c 0000 000a  .rm.......s,....
+00001340: 0310 0108 030c 011c ff0e 0308 0402 ff04  ................
+00001350: 0202 fe08 0302 fd08 050a 0308 010c 0108  ................
+00001360: 0108 0108 0102 0112 0104 fc7a 104f 7574  ...........z.Out
+00001370: 7075 742e 706f 7374 5f69 6e69 7463 0100  put.post_initc..
+00001380: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00001390: 0000 4300 0000 736c 0000 007c 006a 006a  ..C...sl...|.j.j
+000013a0: 0164 011b 007d 017c 01a0 02a1 0073 1374  .d...}.|.....s.t
+000013b0: 0364 027c 006a 006a 019b 009d 0283 0182  .d.|.j.j........
+000013c0: 0174 04a0 057c 017c 006a 066a 07a1 0201  .t...|.|.j.j....
+000013d0: 0074 087c 006a 0083 01a0 09a1 0044 005d  .t.|.j.......D.]
+000013e0: 117d 0274 0a7c 0264 0383 0272 337c 026a  .}.t.|.d...r3|.j
+000013f0: 0ba0 0c64 04a1 0173 337c 02a0 0da1 0001  ...d...s3|......
+00001400: 0071 2264 0553 0029 067a 2443 7265 6174  .q"d.S.).z$Creat
+00001410: 6520 7468 6520 6669 6c65 7320 6672 6f6d  e the files from
+00001420: 2074 6865 6972 2074 656d 706c 6174 657a   their templatez
+00001430: 0874 6173 6b73 2e70 797a 2974 6173 6b73  .tasks.pyz)tasks
+00001440: 2e70 7920 6d69 7373 696e 6720 696e 2073  .py missing in s
+00001450: 6f6c 7665 7220 7465 6d70 6c61 7465 735f  olver templates_
+00001460: 6469 7220 7243 0000 0072 2600 0000 4e29  dir rC...r&...N)
+00001470: 0e72 5000 0000 5a0d 7465 6d70 6c61 7465  .rP...Z.template
+00001480: 735f 6469 7272 6f00 0000 da0c 5275 6e74  s_dirro.....Runt
+00001490: 696d 6545 7272 6f72 7270 0000 0072 7100  imeErrorrp...rq.
+000014a0: 0000 7244 0000 0072 4f00 0000 725d 0000  ..rD...rO...r]..
+000014b0: 0072 3500 0000 7256 0000 0072 5e00 0000  .r5...rV...r^...
+000014c0: 725f 0000 0072 4300 0000 2903 7260 0000  r_...rC...).r`..
+000014d0: 005a 0d70 6174 685f 7461 736b 735f 7079  .Z.path_tasks_py
+000014e0: 7264 0000 0072 2000 0000 7220 0000 0072  rd...r ...r ...r
+000014f0: 2100 0000 726e 0000 00cf 0000 0073 2200  !...rn.......s".
+00001500: 0000 0c02 0801 0201 0201 0601 04ff 04ff  ................
+00001510: 1004 1202 0201 0401 04ff 0a02 02fe 0804  ................
+00001520: 0280 04fb 7a2f 4f75 7470 7574 2e70 6f73  ....z/Output.pos
+00001530: 745f 696e 6974 5f63 7265 6174 655f 6164  t_init_create_ad
+00001540: 6469 7469 6f6e 616c 5f73 6f75 7263 655f  ditional_source_
+00001550: 6669 6c65 7363 0200 0000 0000 0000 0000  filesc..........
+00001560: 0000 0300 0000 0500 0000 4300 0000 7328  ..........C...s(
+00001570: 0000 0064 0164 0284 007c 006a 00a0 01a1  ...d.d...|.j....
+00001580: 0044 0083 017d 027c 016a 0264 037c 0264  .D...}.|.j.d.|.d
+00001590: 0464 058d 0301 0064 0053 0029 064e 6301  .d.....d.S.).Nc.
+000015a0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+000015b0: 0000 0053 0000 0073 1a00 0000 6900 7c00  ...S...s....i.|.
+000015c0: 5d09 5c02 7d01 7d02 7400 7c01 8301 7c02  ].\.}.}.t.|...|.
+000015d0: 9302 7102 5300 7220 0000 0072 0300 0000  ..q.S.r ...r....
+000015e0: 2903 da02 2e30 da03 6b65 79da 0576 616c  )....0..key..val
+000015f0: 7565 7220 0000 0072 2000 0000 7221 0000  uer ...r ...r!..
+00001600: 00da 0a3c 6469 6374 636f 6d70 3ee2 0000  ...<dictcomp>...
+00001610: 0073 0800 0000 0600 0602 08ff 06ff 7a38  .s............z8
+00001620: 4f75 7470 7574 2e5f 636f 6d70 6c65 7465  Output._complete
+00001630: 5f70 6172 616d 735f 636f 6e74 726f 6c5f  _params_control_
+00001640: 6469 6374 2e3c 6c6f 6361 6c73 3e2e 3c64  dict.<locals>.<d
+00001650: 6963 7463 6f6d 703e da0c 636f 6e74 726f  ictcomp>..contro
+00001660: 6c5f 6469 6374 7a3d 5365 6520 6874 7470  l_dictz=See http
+00001670: 733a 2f2f 646f 632e 6366 642e 6469 7265  s://doc.cfd.dire
+00001680: 6374 2f6f 7065 6e66 6f61 6d2f 7573 6572  ct/openfoam/user
+00001690: 2d67 7569 6465 2d76 362f 636f 6e74 726f  -guide-v6/contro
+000016a0: 6c64 6963 74a9 0272 3400 0000 da03 646f  ldict..r4.....do
+000016b0: 6329 03da 1b64 6566 6175 6c74 5f63 6f6e  c)...default_con
+000016c0: 7472 6f6c 5f64 6963 745f 7061 7261 6d73  trol_dict_params
+000016d0: 7251 0000 0072 1b00 0000 2903 721e 0000  rQ...r....).r...
+000016e0: 0072 3c00 0000 7234 0000 0072 2000 0000  .r<...r4...r ...
+000016f0: 7220 0000 0072 2100 0000 da1d 5f63 6f6d  r ...r!....._com
+00001700: 706c 6574 655f 7061 7261 6d73 5f63 6f6e  plete_params_con
+00001710: 7472 6f6c 5f64 6963 74e0 0000 0073 1000  trol_dict....s..
+00001720: 0000 0602 0802 06fe 0405 0201 0201 0201  ................
+00001730: 0afd 7a24 4f75 7470 7574 2e5f 636f 6d70  ..z$Output._comp
+00001740: 6c65 7465 5f70 6172 616d 735f 636f 6e74  lete_params_cont
+00001750: 726f 6c5f 6469 6374 6302 0000 0000 0000  rol_dictc.......
+00001760: 0000 0000 0004 0000 0007 0000 0003 0000  ................
+00001770: 0073 3600 0000 8700 6601 6401 6402 8408  .s6.....f.d.d...
+00001780: 7c00 6a00 a001 a100 4400 8301 7d02 7402  |.j.....D...}.t.
+00001790: 6403 6404 6405 6406 6407 6408 9c05 7c02  d.d.d.d.d.d...|.
+000017a0: 7403 6409 8d03 7d03 7c03 5300 290a 4e63  t.d...}.|.S.).Nc
+000017b0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000017c0: 0600 0000 1300 0000 731c 0000 0069 007c  ........s....i.|
+000017d0: 005d 0a7d 017c 0188 006a 0074 017c 0183  .].}.|...j.t.|..
+000017e0: 0119 0093 0271 0253 0072 2000 0000 2902  .....q.S.r ...).
+000017f0: 7277 0000 0072 0400 0000 2902 7273 0000  rw...r....).rs..
+00001800: 0072 7400 0000 a901 723c 0000 0072 2000  .rt.....r<...r .
+00001810: 0000 7221 0000 0072 7600 0000 ee00 0000  ..r!...rv.......
+00001820: 7308 0000 0006 0002 020e ff06 ff7a 314f  s............z1O
+00001830: 7574 7075 742e 6d61 6b65 5f74 7265 655f  utput.make_tree_
+00001840: 636f 6e74 726f 6c5f 6469 6374 2e3c 6c6f  control_dict.<lo
+00001850: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
+00001860: 7a03 322e 30da 0561 7363 6969 da0a 6469  z.2.0..ascii..di
+00001870: 6374 696f 6e61 7279 7a08 2273 7973 7465  ctionaryz."syste
+00001880: 6d22 7216 0000 0029 05da 0776 6572 7369  m"r....)...versi
+00001890: 6f6e 7254 0000 00da 0563 6c61 7373 da08  onrT.....class..
+000018a0: 6c6f 6361 7469 6f6e da06 6f62 6a65 6374  location..object
+000018b0: 2903 7245 0000 00da 0863 6869 6c64 7265  ).rE.....childre
+000018c0: 6eda 0668 6561 6465 7229 0472 7a00 0000  n..header).rz...
+000018d0: da04 6b65 7973 720c 0000 0072 0a00 0000  ..keysr....r....
+000018e0: 2904 7260 0000 0072 3c00 0000 7283 0000  ).r`...r<...r...
+000018f0: 00da 0474 7265 6572 2000 0000 727c 0000  ...treer ...r|..
+00001900: 0072 2100 0000 da16 6d61 6b65 5f74 7265  .r!.....make_tre
+00001910: 655f 636f 6e74 726f 6c5f 6469 6374 ed00  e_control_dict..
+00001920: 0000 731c 0000 000a 0108 0206 fe02 0502  ..s.............
+00001930: 0202 0102 0102 0102 0104 fb02 0702 0106  ................
+00001940: f704 0b7a 1d4f 7574 7075 742e 6d61 6b65  ...z.Output.make
+00001950: 5f74 7265 655f 636f 6e74 726f 6c5f 6469  _tree_control_di
+00001960: 6374 6302 0000 0000 0000 0000 0000 0003  ctc.............
+00001970: 0000 0003 0000 0043 0000 0073 1200 0000  .......C...s....
+00001980: 7c00 a000 7c01 a101 7d02 7c02 a001 a100  |...|...}.|.....
+00001990: 5300 2901 4e29 0272 8700 0000 da04 6475  S.).N).r......du
+000019a0: 6d70 2903 7260 0000 0072 3c00 0000 7286  mp).r`...r<...r.
+000019b0: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
+000019c0: 0000 da16 6d61 6b65 5f63 6f64 655f 636f  ....make_code_co
+000019d0: 6e74 726f 6c5f 6469 6374 0001 0000 7304  ntrol_dict....s.
+000019e0: 0000 000a 0108 017a 1d4f 7574 7075 742e  .......z.Output.
+000019f0: 6d61 6b65 5f63 6f64 655f 636f 6e74 726f  make_code_contro
+00001a00: 6c5f 6469 6374 6302 0000 0000 0000 0000  l_dictc.........
+00001a10: 0000 0003 0000 0009 0000 0043 0000 0073  ...........C...s
+00001a20: 2a00 0000 6401 6401 6401 6402 6402 6402  *...d.d.d.d.d.d.
+00001a30: 6403 6400 6404 9c08 7d02 7c01 6a00 6405  d.d.d...}.|.j.d.
+00001a40: 7c02 6406 6407 8d03 0100 6400 5300 2908  |.d.d.....d.S.).
+00001a50: 4ee9 2800 0000 6700 0000 0000 00f0 3fda  N.(...g.......?.
+00001a60: 016d 2908 da02 6e78 da02 6e79 da02 6e7a  .m)...nx..ny..nz
+00001a70: da02 6c78 da02 6c79 da02 6c7a da06 6d65  ..lx..ly..lz..me
+00001a80: 7472 6963 da05 7363 616c 65da 0f62 6c6f  tric..scale..blo
+00001a90: 636b 5f6d 6573 685f 6469 6374 da04 544f  ck_mesh_dict..TO
+00001aa0: 444f 7278 0000 0029 0172 1b00 0000 2903  DOrx...).r....).
+00001ab0: 721e 0000 0072 3c00 0000 da07 6465 6661  r....r<.....defa
+00001ac0: 756c 7472 2000 0000 7220 0000 0072 2100  ultr ...r ...r!.
+00001ad0: 0000 da20 5f63 6f6d 706c 6574 655f 7061  ... _complete_pa
+00001ae0: 7261 6d73 5f62 6c6f 636b 5f6d 6573 685f  rams_block_mesh_
+00001af0: 6469 6374 0401 0000 731c 0000 0002 0302  dict....s.......
+00001b00: 0102 0102 0102 0102 0102 0102 0106 f804  ................
+00001b10: 0b02 0102 0102 010a fd7a 274f 7574 7075  .........z'Outpu
+00001b20: 742e 5f63 6f6d 706c 6574 655f 7061 7261  t._complete_para
+00001b30: 6d73 5f62 6c6f 636b 5f6d 6573 685f 6469  ms_block_mesh_di
+00001b40: 6374 2902 4e4e 2918 da08 5f5f 6e61 6d65  ct).NN)...__name
+00001b50: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00001b60: 5f5f 7175 616c 6e61 6d65 5f5f 7228 0000  __qualname__r(..
+00001b70: 0072 2a00 0000 722b 0000 0072 0900 0000  .r*...r+...r....
+00001b80: 727a 0000 0072 0b00 0000 da1c 6865 6c70  rz...r......help
+00001b90: 6572 5f74 7572 6275 6c65 6e63 655f 7072  er_turbulence_pr
+00001ba0: 6f70 6572 7469 6573 da0b 636c 6173 736d  operties..classm
+00001bb0: 6574 686f 6472 2200 0000 721c 0000 0072  ethodr"...r....r
+00001bc0: 2d00 0000 723e 0000 0072 4d00 0000 724b  -...r>...rM...rK
+00001bd0: 0000 0072 6d00 0000 726e 0000 0072 7b00  ...rm...rn...r{.
+00001be0: 0000 7287 0000 0072 8900 0000 7297 0000  ..r....r....r...
+00001bf0: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
+00001c00: 7220 0000 0072 2000 0000 7265 0000 0072  r ...r ...re...r
+00001c10: 2100 0000 7211 0000 001a 0000 0073 3600  !...r........s6.
+00001c20: 0000 0800 0801 0801 0801 0401 0202 0801  ................
+00001c30: 04ff 0204 0a01 020a 0a01 0203 0a01 020d  ................
+00001c40: 0a01 0e1d 024d 0a01 0c04 081e 0211 0a01  .....M..........
+00001c50: 080c 0813 0204 1201 7211 0000 0029 1c72  ........r....).r
+00001c60: 6700 0000 7270 0000 0072 3900 0000 da07  g...rp...r9.....
+00001c70: 7061 7468 6c69 6272 0200 0000 da0a 696e  pathlibr......in
+00001c80: 666c 6563 7469 6f6e 7204 0000 005a 0b66  flectionr....Z.f
+00001c90: 6c75 6964 6479 6e2e 696f 7205 0000 005a  luiddyn.ior....Z
+00001ca0: 0d66 6c75 6964 6479 6e2e 7574 696c 7206  .fluiddyn.utilr.
+00001cb0: 0000 005a 1466 6c75 6964 7369 6d5f 636f  ...Z.fluidsim_co
+00001cc0: 7265 2e6f 7574 7075 7472 0700 0000 da14  re.outputr......
+00001cd0: 666c 7569 6473 696d 5f63 6f72 652e 7061  fluidsim_core.pa
+00001ce0: 7261 6d73 7208 0000 00da 1d66 6c75 6964  ramsr......fluid
+00001cf0: 7369 6d66 6f61 6d2e 666f 616d 5f69 6e70  simfoam.foam_inp
+00001d00: 7574 5f66 696c 6573 7209 0000 0072 0a00  ut_filesr....r..
+00001d10: 0000 720b 0000 0072 0c00 0000 5a28 666c  ..r....r....Z(fl
+00001d20: 7569 6473 696d 666f 616d 2e66 6f61 6d5f  uidsimfoam.foam_
+00001d30: 696e 7075 745f 6669 6c65 732e 6765 6e65  input_files.gene
+00001d40: 7261 746f 7273 720d 0000 0072 0e00 0000  ratorsr....r....
+00001d50: 5a10 666c 7569 6473 696d 666f 616d 2e6c  Z.fluidsimfoam.l
+00001d60: 6f67 720f 0000 00da 1466 6c75 6964 7369  ogr......fluidsi
+00001d70: 6d66 6f61 6d2e 736f 6c76 6572 7372 1000  mfoam.solversr..
+00001d80: 0000 7211 0000 0072 2000 0000 7220 0000  ..r....r ...r ..
+00001d90: 0072 2000 0000 7221 0000 00da 083c 6d6f  .r ...r!.....<mo
+00001da0: 6475 6c65 3e01 0000 0073 1c00 0000 0800  dule>....s......
+00001db0: 0801 0801 0c01 0c02 0c02 0c01 0c01 0c01  ................
+00001dc0: 1801 1006 0c04 0c01 1403                 ..........
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/output/base.py` & `fluidsimfoam-0.0.3/src/fluidsimfoam/output/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,29 +8,34 @@
 from fluiddyn.io import stdout_redirected
 from fluiddyn.util import mpi
 from fluidsim_core.output import OutputCore
 from fluidsim_core.params import iter_complete_params
 from fluidsimfoam.foam_input_files import (
     DEFAULT_CONTROL_DICT,
     DEFAULT_HEADER,
+    ConstantFileHelper,
     FoamInputFile,
 )
 from fluidsimfoam.foam_input_files.generators import (
-    FileGeneratorABC,
     InputFiles,
     new_file_generator_class,
 )
 from fluidsimfoam.log import logger
 from fluidsimfoam.solvers import get_solver_package
 
 
 class Output(OutputCore):
     variable_names = ["p", "U"]
     constant_files_names = ["transportProperties", "turbulenceProperties"]
     system_files_names = ["controlDict", "fvSchemes", "fvSolution"]
+    default_control_dict_params = DEFAULT_CONTROL_DICT
+
+    helper_turbulence_properties = ConstantFileHelper(
+        "turbulenceProperties", {"simulationType": "laminar"}
+    )
 
     @classmethod
     def _complete_info_solver(cls, info_solver):
         """Complete the info_solver instance with child class details (module
         and class names).
 
         """
@@ -43,15 +48,17 @@
     def _set_info_solver_classes(cls, classes):
         """Set the classes for info_solver.classes.Output"""
 
     @classmethod
     def _setup_file_generators_classes(cls):
         classes = cls._file_generators_classes = {}
         for variable_name in cls.variable_names:
-            classes[variable_name] = new_file_generator_class(variable_name)
+            classes[variable_name.replace(".", "_")] = new_file_generator_class(
+                variable_name
+            )
 
         for file_name in cls.constant_files_names:
             classes[file_name] = new_file_generator_class(file_name, "constant")
 
         for file_name in cls.system_files_names:
             classes[file_name] = new_file_generator_class(file_name, "system")
 
@@ -113,58 +120,58 @@
             return
 
         self.path_run = Path(self.path_run)
 
         self.input_files = InputFiles(self)
         # initialize objects
         dict_classes = sim.info.solver.classes.Output.import_classes()
-
-        if not hasattr(self, "_file_generators_classes"):
-            self._setup_file_generators_classes()
-        dict_classes.update(self._file_generators_classes)
-
-        for_str_input_files = []
         for cls_name, Class in dict_classes.items():
             if isinstance(self, Class):
                 continue
             obj_name = underscore(cls_name)
+            self.sim._objects_to_print += "{:28s}{}\n".format(
+                f"sim.output.{obj_name}: ", Class
+            )
+            setattr(self, obj_name, Class(self))
 
-            if issubclass(Class, FileGeneratorABC):
-                obj_containing = self.input_files
-                for_str_input_files.append(cls_name)
-            else:
-                obj_containing = self
-                self.sim._objects_to_print += "{:28s}{}\n".format(
-                    f"sim.output.{obj_name}: ", Class
-                )
+        if not hasattr(self, "_file_generators_classes"):
+            self._setup_file_generators_classes()
+        for_str_input_files = {}
+        for cls_name, Class in self._file_generators_classes.items():
+            obj_name = underscore(cls_name)
 
-            setattr(obj_containing, obj_name, Class(self))
+            if Class.dir_name not in for_str_input_files:
+                for_str_input_files[Class.dir_name] = [cls_name]
+            else:
+                for_str_input_files[Class.dir_name].append(cls_name)
+            setattr(self.input_files, obj_name, Class(self))
 
         if for_str_input_files:
-            self.sim._objects_to_print += (
-                f"{'input files:':28s}{' '.join(for_str_input_files)}\n"
-            )
+            self.sim._objects_to_print += "input_files:\n"
+            for dir_name, input_files in for_str_input_files.items():
+                self.sim._objects_to_print += (
+                    f"  - in {dir_name + ':':12s}{' '.join(input_files)}\n"
+                )
 
         if not (
             mpi.rank == 0
             and self._has_to_save
             and self.sim.params.NEW_DIR_RESULTS
         ):
             return
 
         (self.path_run / "system").mkdir()
         (self.path_run / "0").mkdir()
         (self.path_run / "constant").mkdir()
 
-        try:
-            file_generator = getattr(self.input_files, "block_mesh_dict")
-        except AttributeError:
-            pass
-        else:
-            file_generator.generate_file()
+        for file_generator in vars(self.input_files).values():
+            if hasattr(
+                file_generator, "generate_file"
+            ) and file_generator.rel_path.startswith("system"):
+                file_generator.generate_file()
 
     @classmethod
     def get_path_solver_package(cls):
         """Get the path towards the solver package."""
         return Path(inspect.getmodule(cls).__file__).parent
 
     def post_init(self):
@@ -195,45 +202,46 @@
             path_new = path_info_fluidsim / file_name
             if path_new.exists():
                 continue
             shutil.copy(path_run / file_name, path_new)
 
     def post_init_create_additional_source_files(self):
         """Create the files from their template"""
-        for name, file_generator in vars(self.input_files).items():
-            if name == "block_mesh_dict":
-                # already produced during __init__
-                continue
-            if hasattr(file_generator, "generate_file"):
-                file_generator.generate_file()
-
         path_tasks_py = self.input_files.templates_dir / "tasks.py"
         if not path_tasks_py.exists():
             raise RuntimeError(
                 "tasks.py missing in solver templates_dir "
                 f"{self.input_files.templates_dir}"
             )
         shutil.copy(path_tasks_py, self.sim.path_run)
 
+        for file_generator in vars(self.input_files).values():
+            if hasattr(
+                file_generator, "generate_file"
+            ) and not file_generator.rel_path.startswith("system"):
+                # system files are already generated
+                file_generator.generate_file()
+
     @classmethod
     def _complete_params_control_dict(cls, params):
         attribs = {
-            underscore(key): value for key, value in DEFAULT_CONTROL_DICT.items()
+            underscore(key): value
+            for key, value in cls.default_control_dict_params.items()
         }
 
         params._set_child(
             "control_dict",
             attribs=attribs,
             doc="""See https://doc.cfd.direct/openfoam/user-guide-v6/controldict""",
         )
 
     def make_tree_control_dict(self, params):
         children = {
             key: params.control_dict[underscore(key)]
-            for key in DEFAULT_CONTROL_DICT.keys()
+            for key in self.default_control_dict_params.keys()
         }
 
         tree = FoamInputFile(
             info={
                 "version": "2.0",
                 "format": "ascii",
                 "class": "dictionary",
@@ -246,84 +254,14 @@
         return tree
 
     def make_code_control_dict(self, params):
         tree = self.make_tree_control_dict(params)
         return tree.dump()
 
     @classmethod
-    def _complete_params_turbulence_properties(cls, params):
-        params._set_child(
-            "turbulence_properties",
-            attribs={"simulation_type": "laminar"},
-            doc="""TODO""",
-        )
-
-    def make_tree_turbulence_properties(self, params):
-        return FoamInputFile(
-            info={
-                "version": "2.0",
-                "format": "ascii",
-                "class": "dictionary",
-                "object": "turbulenceProperties",
-            },
-            children={
-                "simulationType": params.turbulence_properties.simulation_type
-            },
-            header=DEFAULT_HEADER,
-        )
-
-    @classmethod
-    def _complete_params_fv_solution(cls, params):
-        params._set_child("fv_solution", doc="""TODO""")
-        solvers = params.fv_solution._set_child("solvers", doc="""TODO""")
-        attribs = {
-            "solver": "PCG",
-            "preconditioner": "DIC",
-            "tolerance": 1e-06,
-            "relTol": 0.01,
-        }
-
-        solvers._set_child("p", attribs=attribs)
-        solvers._set_child("pFinal", attribs=attribs)
-        solvers.pFinal.relTol = 0
-        solvers._set_child(
-            "U",
-            attribs={
-                "solver": "PBiCGStab",
-                "preconditioner": "DILU",
-                "tolerance": 1e-08,
-                "relTol": 0,
-            },
-        )
-
-        params.fv_solution._set_child(
-            "piso",
-            attribs={
-                "nCorrectors": 2,
-                "nNonOrthogonalCorrectors": 1,
-                "pRefPoint": "(0 0 0)",
-                "pRefValue": 0,
-            },
-        )
-
-    @classmethod
-    def _complete_params_fv_schemes(cls, params):
-        fv_schemes = params._set_child("fv_schemes", doc="""TODO""")
-        fv_schemes._set_child("ddtSchemes", attribs={"default": "backward"})
-        fv_schemes._set_child("gradSchemes", attribs={"default": "leastSquares"})
-        fv_schemes._set_child("divSchemes", attribs={"default": "none"})
-        fv_schemes._set_child(
-            "laplacianSchemes", attribs={"default": "Gauss linear corrected"}
-        )
-        fv_schemes._set_child(
-            "interpolationSchemes", attribs={"default": "linear"}
-        )
-        fv_schemes._set_child("snGradSchemes", attribs={"default": "corrected"})
-
-    @classmethod
     def _complete_params_block_mesh_dict(cls, params):
         default = {
             "nx": 40,
             "ny": 40,
             "nz": 40,
             "lx": 1.0,
             "ly": 1.0,
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/solvers/__init__.py` & `fluidsimfoam-0.0.3/src/fluidsimfoam/solvers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Solver framework
+Define and use solvers
 
 .. autosummary::
    :toctree:
 
    base
 
 """
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc` & `fluidsimfoam-0.0.3/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Apr 26 14:14:21 2023 UTC, .py size: 2759 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-00000000: 6f0d 0d0a 0000 0000 bd31 4964 c70a 0000  o........1Id....
+00000000: 6f0d 0d0a 0000 0000 f444 5a64 cd0a 0000  o........DZd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6401 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6408 6409 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000080: 0100 6503 6509 6a0e 640a 640b 8d02 5a0e  ..e.e.j.d.d...Z.
 00000090: 640c 650e 5f00 6503 6509 6a0f 640a 640b  d.e._.e.e.j.d.d.
 000000a0: 8d02 5a0f 640d 650f 5f00 640e 640f 8400  ..Z.d.e._.d.d...
 000000b0: 5a10 6410 6411 8400 5a11 6412 6413 8400  Z.d.d...Z.d.d...
-000000c0: 5a12 6402 5300 2914 7a3b 0a53 6f6c 7665  Z.d.S.).z;.Solve
-000000d0: 7220 6672 616d 6577 6f72 6b0a 0a2e 2e20  r framework.... 
-000000e0: 6175 746f 7375 6d6d 6172 793a 3a0a 2020  autosummary::.  
-000000f0: 203a 746f 6374 7265 653a 0a0a 2020 2062   :toctree:..   b
-00000100: 6173 650a 0ae9 0000 0000 4e29 01da 0770  ase.......N)...p
-00000110: 6172 7469 616c 2901 da0a 4d6f 6475 6c65  artial)...Module
-00000120: 496e 666f 2901 da0a 4d6f 6475 6c65 5479  Info)...ModuleTy
-00000130: 7065 2901 da06 6c6f 6164 6572 2901 da0e  pe)...loader)...
-00000140: 496e 666f 536f 6c76 6572 436f 7265 e902  InfoSolverCore..
-00000150: 0000 0029 01da 066c 6f67 6765 727a 1466  ...)...loggerz.f
-00000160: 6c75 6964 7369 6d66 6f61 6d2e 736f 6c76  luidsimfoam.solv
-00000170: 6572 7329 015a 0e65 6e74 7279 706f 696e  ers).Z.entrypoin
-00000180: 745f 6772 707a 4c52 6574 7572 6e73 2061  t_grpzLReturns a
-00000190: 2064 6963 7469 6f6e 6172 7920 6f66 2061   dictionary of a
-000001a0: 6c6c 2072 6567 6973 7465 7265 6420 736f  ll registered so
-000001b0: 6c76 6572 7320 7265 6769 7374 6572 6564  lvers registered
-000001c0: 2061 7320 616e 2065 6e74 7279 706f 696e   as an entrypoin
-000001d0: 742e 0a7a 2349 6d70 6f72 7420 7468 6520  t..z#Import the 
-000001e0: 5369 6d75 6c20 636c 6173 7320 6f66 2061  Simul class of a
-000001f0: 2073 6f6c 7665 722e 6301 0000 0000 0000   solver.c.......
-00000200: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-00000210: 0073 5600 0000 7400 7c00 7401 8302 720c  .sV...t.|.t...r.
-00000220: 7402 6a03 a004 7c00 a101 7d01 6e1a 7400  t.j...|...}.n.t.
-00000230: 7c00 7405 8302 7215 7c00 6a06 7d01 6e11  |.t...r.|.j.}.n.
-00000240: 7400 7c00 7407 8302 721d 7c00 6a08 5300  t.|.t...r.|.j.S.
-00000250: 7409 6401 740a 7c00 8301 9b00 9d02 8301  t.d.t.|.........
-00000260: 8201 7c01 6a0b 6402 7501 5300 2903 7527  ..|.j.d.u.S.).u'
-00000270: 0100 0043 6865 636b 7320 6966 2061 206d  ...Checks if a m
-00000280: 6f64 756c 6520 6973 2061 2070 6163 6b61  odule is a packa
-00000290: 6765 206f 7220 6e6f 742e 2041 7320 6f66  ge or not. As of
-000002a0: 2050 4550 2034 3531 2074 6869 7320 696e   PEP 451 this in
-000002b0: 666f 726d 6174 696f 6e0a 2020 2020 6973  formation.    is
-000002c0: 2061 6c73 6f20 6176 6169 6c61 626c 6520   also available 
-000002d0: 6f6e 2074 6865 206d 6f64 756c 65e2 8099  on the module...
-000002e0: 7320 5f5f 7370 6563 5f5f 2e73 7562 6d6f  s __spec__.submo
-000002f0: 6475 6c65 5f73 6561 7263 685f 6c6f 6361  dule_search_loca
-00000300: 7469 6f6e 730a 2020 2020 6174 7472 6962  tions.    attrib
-00000310: 7574 652c 2077 6869 6368 2077 696c 6c20  ute, which will 
-00000320: 6e6f 7420 6265 204e 6f6e 6520 666f 7220  not be None for 
-00000330: 7061 636b 6167 6573 2e0a 0a20 2020 2050  packages...    P
-00000340: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-00000350: 2d2d 2d2d 2d2d 2d2d 0a20 2020 206d 6f64  --------.    mod
-00000360: 756c 653a 2073 7472 206f 7220 6d6f 6475  ule: str or modu
-00000370: 6c65 0a0a 2020 2020 5265 7475 726e 730a  le..    Returns.
-00000380: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00000390: 626f 6f6c 0a0a 2020 2020 7a0f 4361 6e6e  bool..    z.Cann
-000003a0: 6f74 2070 726f 6365 7373 204e 290c da0a  ot process N)...
-000003b0: 6973 696e 7374 616e 6365 da03 7374 72da  isinstance..str.
-000003c0: 0969 6d70 6f72 746c 6962 da04 7574 696c  .importlib..util
-000003d0: da09 6669 6e64 5f73 7065 6372 0400 0000  ..find_specr....
-000003e0: da08 5f5f 7370 6563 5f5f 7203 0000 00da  ..__spec__r.....
-000003f0: 0569 7370 6b67 da0a 5661 6c75 6545 7272  .ispkg..ValueErr
-00000400: 6f72 da04 7479 7065 da1a 7375 626d 6f64  or..type..submod
-00000410: 756c 655f 7365 6172 6368 5f6c 6f63 6174  ule_search_locat
-00000420: 696f 6e73 2902 da06 6d6f 6475 6c65 da04  ions)...module..
-00000430: 7370 6563 a900 7215 0000 00fa 422f 686f  spec..r.....B/ho
-00000440: 6d65 2f70 6965 7272 652f 4465 762f 666c  me/pierre/Dev/fl
-00000450: 7569 6473 696d 666f 616d 2f73 7263 2f66  uidsimfoam/src/f
-00000460: 6c75 6964 7369 6d66 6f61 6d2f 736f 6c76  luidsimfoam/solv
-00000470: 6572 732f 5f5f 696e 6974 5f5f 2e70 79da  ers/__init__.py.
-00000480: 0a69 735f 7061 636b 6167 6522 0000 0073  .is_package"...s
-00000490: 1000 0000 0a0e 0e01 0a01 0801 0a01 0601  ................
-000004a0: 1202 0a02 7217 0000 0063 0100 0000 0000  ....r....c......
-000004b0: 0000 0000 0000 0300 0000 0800 0000 4300  ..............C.
-000004c0: 0000 7348 0000 0074 0083 007c 0019 007d  ..sH...t...|...}
-000004d0: 017a 057c 016a 017d 0257 006e 0c04 0074  .z.|.j.}.W.n...t
-000004e0: 0279 1601 0001 0001 007c 016a 037d 0259  .y.......|.j.}.Y
-000004f0: 006e 0177 0074 047c 0283 0172 1d7c 0253  .n.w.t.|...r.|.S
-00000500: 007c 02a0 0564 01a1 0164 0219 0053 0029  .|...d...d...S.)
-00000510: 037a d852 6574 7572 6e20 6e61 6d65 206f  .z.Return name o
-00000520: 6620 7468 6520 736f 6c76 6572 2070 6163  f the solver pac
-00000530: 6b61 6765 2062 7920 6368 6563 6b69 6e67  kage by checking
-00000540: 2074 6865 2060 6073 6e65 6b35 3030 302e   the ``snek5000.
-00000550: 736f 6c76 6572 7360 600a 2020 2020 656e  solvers``.    en
-00000560: 7472 7970 6f69 6e74 2067 726f 7570 2e0a  trypoint group..
-00000570: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-00000580: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00000590: 2020 206e 616d 655f 736f 6c76 6572 3a20     name_solver: 
-000005a0: 7374 720a 2020 2020 2020 2020 5368 6f72  str.        Shor
-000005b0: 7420 6e61 6d65 206f 6620 7468 6520 736f  t name of the so
-000005c0: 6c76 6572 0a0a 2020 2020 5265 7475 726e  lver..    Return
-000005d0: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
-000005e0: 2020 7374 720a 0a20 2020 20da 012e 7201    str..    ...r.
-000005f0: 0000 0029 06da 1161 7661 696c 6162 6c65  ...)...available
-00000600: 5f73 6f6c 7665 7273 7213 0000 00da 0e41  _solversr......A
-00000610: 7474 7269 6275 7465 4572 726f 72da 0b6d  ttributeError..m
-00000620: 6f64 756c 655f 6e61 6d65 7217 0000 00da  odule_namer.....
-00000630: 0a72 7061 7274 6974 696f 6e29 03da 0b6e  .rpartition)...n
-00000640: 616d 655f 736f 6c76 6572 da0a 656e 7472  ame_solver..entr
-00000650: 7970 6f69 6e74 7213 0000 0072 1500 0000  ypointr....r....
-00000660: 7215 0000 0072 1600 0000 da12 6765 745f  r....r......get_
-00000670: 736f 6c76 6572 5f70 6163 6b61 6765 3c00  solver_package<.
-00000680: 0000 7312 0000 000a 0e02 010a 020c 010a  ..s.............
-00000690: 0102 ff08 0204 010e 0272 1f00 0000 6301  .........r....c.
-000006a0: 0000 0000 0000 0000 0000 0004 0000 0005  ................
-000006b0: 0000 0043 0000 0073 5e00 0000 7c00 6401  ...C...s^...|.d.
-000006c0: 1b00 7d01 7c01 a000 a100 730c 7c00 6402  ..}.|.....s.|.d.
-000006d0: 1b00 7d01 7c01 a000 a100 721a 7401 7c01  ..}.|.....r.t.|.
-000006e0: 6403 8d01 7d02 7c02 6a02 7d03 7c03 5300  d...}.|.j.}.|.S.
-000006f0: 7403 a004 6404 7c01 9b00 6405 9d03 a101  t...d.|...d.....
-00000700: 0100 7c00 a005 a100 6a06 a007 6406 a101  ..|.....j...d...
-00000710: 6407 1900 7d03 7c03 5300 2908 7ae6 4465  d...}.|.S.).z.De
-00000720: 7465 6374 7320 7368 6f72 7420 6e61 6d65  tects short name
-00000730: 206f 6620 7468 6520 736f 6c76 6572 2066   of the solver f
-00000740: 726f 6d20 6060 696e 666f 5f73 6f6c 7665  rom ``info_solve
-00000750: 722e 786d 6c60 6020 6966 2070 7265 7365  r.xml`` if prese
-00000760: 6e74 206f 720a 2020 2020 7468 6520 7061  nt or.    the pa
-00000770: 7468 2e0a 0a20 2020 2050 6172 616d 6574  th...    Paramet
-00000780: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-00000790: 2d2d 0a20 2020 2070 6174 685f 6469 723a  --.    path_dir:
-000007a0: 2070 6174 682d 6c69 6b65 0a20 2020 2020   path-like.     
-000007b0: 2020 2050 6174 6820 746f 2061 2073 696d     Path to a sim
-000007c0: 756c 6174 696f 6e20 6469 7265 6374 6f72  ulation director
-000007d0: 790a 0a20 2020 2052 6574 7572 6e73 0a20  y..    Returns. 
-000007e0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2073     -------.    s
-000007f0: 686f 7274 5f6e 616d 653a 2073 7472 0a0a  hort_name: str..
-00000800: 2020 2020 7a0f 696e 666f 5f73 6f6c 7665      z.info_solve
-00000810: 722e 786d 6c7a 1e2e 6461 7461 5f66 6c75  r.xmlz..data_flu
-00000820: 6964 7369 6d2f 696e 666f 5f73 6f6c 7665  idsim/info_solve
-00000830: 722e 786d 6c29 01da 0970 6174 685f 6669  r.xml)...path_fi
-00000840: 6c65 7a04 5468 6520 7a45 2066 696c 6520  lez.The zE file 
-00000850: 6973 206d 6973 7369 6e67 2120 4174 7465  is missing! Atte
-00000860: 6d70 7469 6e67 2074 6f20 6775 6573 7320  mpting to guess 
-00000870: 736f 6c76 6572 2066 726f 6d20 7468 6520  solver from the 
-00000880: 6469 7265 6374 6f72 7920 6e61 6d65 2eda  directory name..
-00000890: 015f 7201 0000 0029 08da 0665 7869 7374  ._r....)...exist
-000008a0: 7372 0600 0000 da0a 7368 6f72 745f 6e61  sr......short_na
-000008b0: 6d65 7208 0000 00da 0777 6172 6e69 6e67  mer......warning
-000008c0: da08 6162 736f 6c75 7465 da04 6e61 6d65  ..absolute..name
-000008d0: da05 7370 6c69 7429 04da 0870 6174 685f  ..split)...path_
-000008e0: 6469 725a 0f69 6e66 6f5f 736f 6c76 6572  dirZ.info_solver
-000008f0: 5f78 6d6c da0b 696e 666f 5f73 6f6c 7665  _xml..info_solve
-00000900: 7272 2300 0000 7215 0000 0072 1500 0000  rr#...r....r....
-00000910: 7216 0000 00da 1567 6574 5f73 6f6c 7665  r......get_solve
-00000920: 725f 7368 6f72 745f 6e61 6d65 5600 0000  r_short_nameV...
-00000930: 7318 0000 0008 0e08 0108 0108 020a 0106  s...............
-00000940: 0104 0804 fa0a 0104 ff14 0404 0272 2a00  .............r*.
-00000950: 0000 2913 da07 5f5f 646f 635f 5f72 0b00  ..)...__doc__r..
-00000960: 0000 da09 6675 6e63 746f 6f6c 7372 0200  ....functoolsr..
-00000970: 0000 da07 706b 6775 7469 6c72 0300 0000  ....pkgutilr....
-00000980: da05 7479 7065 7372 0400 0000 5a0d 666c  ..typesr....Z.fl
-00000990: 7569 6473 696d 5f63 6f72 6572 0500 0000  uidsim_corer....
-000009a0: 5a12 666c 7569 6473 696d 5f63 6f72 652e  Z.fluidsim_core.
-000009b0: 696e 666f 7206 0000 00da 036c 6f67 7208  infor......logr.
-000009c0: 0000 0072 1900 0000 da10 696d 706f 7274  ...r......import
-000009d0: 5f63 6c73 5f73 696d 756c 7217 0000 0072  _cls_simulr....r
-000009e0: 1f00 0000 722a 0000 0072 1500 0000 7215  ....r*...r....r.
-000009f0: 0000 0072 1500 0000 7216 0000 00da 083c  ...r....r......<
-00000a00: 6d6f 6475 6c65 3e01 0000 0073 2600 0000  module>....s&...
-00000a10: 0400 080a 0c01 0c01 0c01 0c02 0c01 0c02  ................
-00000a20: 0202 0601 06ff 0603 0204 0601 06ff 0603  ................
-00000a30: 0803 081a 0c1a                           ......
+000000c0: 5a12 6402 5300 2914 7a41 0a44 6566 696e  Z.d.S.).zA.Defin
+000000d0: 6520 616e 6420 7573 6520 736f 6c76 6572  e and use solver
+000000e0: 730a 0a2e 2e20 6175 746f 7375 6d6d 6172  s.... autosummar
+000000f0: 793a 3a0a 2020 203a 746f 6374 7265 653a  y::.   :toctree:
+00000100: 0a0a 2020 2062 6173 650a 0ae9 0000 0000  ..   base.......
+00000110: 4e29 01da 0770 6172 7469 616c 2901 da0a  N)...partial)...
+00000120: 4d6f 6475 6c65 496e 666f 2901 da0a 4d6f  ModuleInfo)...Mo
+00000130: 6475 6c65 5479 7065 2901 da06 6c6f 6164  duleType)...load
+00000140: 6572 2901 da0e 496e 666f 536f 6c76 6572  er)...InfoSolver
+00000150: 436f 7265 e902 0000 0029 01da 066c 6f67  Core.....)...log
+00000160: 6765 727a 1466 6c75 6964 7369 6d66 6f61  gerz.fluidsimfoa
+00000170: 6d2e 736f 6c76 6572 7329 015a 0e65 6e74  m.solvers).Z.ent
+00000180: 7279 706f 696e 745f 6772 707a 4c52 6574  rypoint_grpzLRet
+00000190: 7572 6e73 2061 2064 6963 7469 6f6e 6172  urns a dictionar
+000001a0: 7920 6f66 2061 6c6c 2072 6567 6973 7465  y of all registe
+000001b0: 7265 6420 736f 6c76 6572 7320 7265 6769  red solvers regi
+000001c0: 7374 6572 6564 2061 7320 616e 2065 6e74  stered as an ent
+000001d0: 7279 706f 696e 742e 0a7a 2349 6d70 6f72  rypoint..z#Impor
+000001e0: 7420 7468 6520 5369 6d75 6c20 636c 6173  t the Simul clas
+000001f0: 7320 6f66 2061 2073 6f6c 7665 722e 6301  s of a solver.c.
+00000200: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000210: 0000 0043 0000 0073 5600 0000 7400 7c00  ...C...sV...t.|.
+00000220: 7401 8302 720c 7402 6a03 a004 7c00 a101  t...r.t.j...|...
+00000230: 7d01 6e1a 7400 7c00 7405 8302 7215 7c00  }.n.t.|.t...r.|.
+00000240: 6a06 7d01 6e11 7400 7c00 7407 8302 721d  j.}.n.t.|.t...r.
+00000250: 7c00 6a08 5300 7409 6401 740a 7c00 8301  |.j.S.t.d.t.|...
+00000260: 9b00 9d02 8301 8201 7c01 6a0b 6402 7501  ........|.j.d.u.
+00000270: 5300 2903 7527 0100 0043 6865 636b 7320  S.).u'...Checks 
+00000280: 6966 2061 206d 6f64 756c 6520 6973 2061  if a module is a
+00000290: 2070 6163 6b61 6765 206f 7220 6e6f 742e   package or not.
+000002a0: 2041 7320 6f66 2050 4550 2034 3531 2074   As of PEP 451 t
+000002b0: 6869 7320 696e 666f 726d 6174 696f 6e0a  his information.
+000002c0: 2020 2020 6973 2061 6c73 6f20 6176 6169      is also avai
+000002d0: 6c61 626c 6520 6f6e 2074 6865 206d 6f64  lable on the mod
+000002e0: 756c 65e2 8099 7320 5f5f 7370 6563 5f5f  ule...s __spec__
+000002f0: 2e73 7562 6d6f 6475 6c65 5f73 6561 7263  .submodule_searc
+00000300: 685f 6c6f 6361 7469 6f6e 730a 2020 2020  h_locations.    
+00000310: 6174 7472 6962 7574 652c 2077 6869 6368  attribute, which
+00000320: 2077 696c 6c20 6e6f 7420 6265 204e 6f6e   will not be Non
+00000330: 6520 666f 7220 7061 636b 6167 6573 2e0a  e for packages..
+00000340: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+00000350: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00000360: 2020 206d 6f64 756c 653a 2073 7472 206f     module: str o
+00000370: 7220 6d6f 6475 6c65 0a0a 2020 2020 5265  r module..    Re
+00000380: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+00000390: 2d0a 2020 2020 626f 6f6c 0a0a 2020 2020  -.    bool..    
+000003a0: 7a0f 4361 6e6e 6f74 2070 726f 6365 7373  z.Cannot process
+000003b0: 204e 290c da0a 6973 696e 7374 616e 6365   N)...isinstance
+000003c0: da03 7374 72da 0969 6d70 6f72 746c 6962  ..str..importlib
+000003d0: da04 7574 696c da09 6669 6e64 5f73 7065  ..util..find_spe
+000003e0: 6372 0400 0000 da08 5f5f 7370 6563 5f5f  cr......__spec__
+000003f0: 7203 0000 00da 0569 7370 6b67 da0a 5661  r......ispkg..Va
+00000400: 6c75 6545 7272 6f72 da04 7479 7065 da1a  lueError..type..
+00000410: 7375 626d 6f64 756c 655f 7365 6172 6368  submodule_search
+00000420: 5f6c 6f63 6174 696f 6e73 2902 da06 6d6f  _locations)...mo
+00000430: 6475 6c65 da04 7370 6563 a900 7215 0000  dule..spec..r...
+00000440: 00fa 422f 686f 6d65 2f70 6965 7272 652f  ..B/home/pierre/
+00000450: 4465 762f 666c 7569 6473 696d 666f 616d  Dev/fluidsimfoam
+00000460: 2f73 7263 2f66 6c75 6964 7369 6d66 6f61  /src/fluidsimfoa
+00000470: 6d2f 736f 6c76 6572 732f 5f5f 696e 6974  m/solvers/__init
+00000480: 5f5f 2e70 79da 0a69 735f 7061 636b 6167  __.py..is_packag
+00000490: 6522 0000 0073 1000 0000 0a0e 0e01 0a01  e"...s..........
+000004a0: 0801 0a01 0601 1202 0a02 7217 0000 0063  ..........r....c
+000004b0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+000004c0: 0800 0000 4300 0000 7348 0000 0074 0083  ....C...sH...t..
+000004d0: 007c 0019 007d 017a 057c 016a 017d 0257  .|...}.z.|.j.}.W
+000004e0: 006e 0c04 0074 0279 1601 0001 0001 007c  .n...t.y.......|
+000004f0: 016a 037d 0259 006e 0177 0074 047c 0283  .j.}.Y.n.w.t.|..
+00000500: 0172 1d7c 0253 007c 02a0 0564 01a1 0164  .r.|.S.|...d...d
+00000510: 0219 0053 0029 037a d852 6574 7572 6e20  ...S.).z.Return 
+00000520: 6e61 6d65 206f 6620 7468 6520 736f 6c76  name of the solv
+00000530: 6572 2070 6163 6b61 6765 2062 7920 6368  er package by ch
+00000540: 6563 6b69 6e67 2074 6865 2060 6073 6e65  ecking the ``sne
+00000550: 6b35 3030 302e 736f 6c76 6572 7360 600a  k5000.solvers``.
+00000560: 2020 2020 656e 7472 7970 6f69 6e74 2067      entrypoint g
+00000570: 726f 7570 2e0a 0a20 2020 2050 6172 616d  roup...    Param
+00000580: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+00000590: 2d2d 2d2d 0a20 2020 206e 616d 655f 736f  ----.    name_so
+000005a0: 6c76 6572 3a20 7374 720a 2020 2020 2020  lver: str.      
+000005b0: 2020 5368 6f72 7420 6e61 6d65 206f 6620    Short name of 
+000005c0: 7468 6520 736f 6c76 6572 0a0a 2020 2020  the solver..    
+000005d0: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+000005e0: 2d2d 2d0a 2020 2020 7374 720a 0a20 2020  ---.    str..   
+000005f0: 20da 012e 7201 0000 0029 06da 1161 7661   ...r....)...ava
+00000600: 696c 6162 6c65 5f73 6f6c 7665 7273 7213  ilable_solversr.
+00000610: 0000 00da 0e41 7474 7269 6275 7465 4572  .....AttributeEr
+00000620: 726f 72da 0b6d 6f64 756c 655f 6e61 6d65  ror..module_name
+00000630: 7217 0000 00da 0a72 7061 7274 6974 696f  r......rpartitio
+00000640: 6e29 03da 0b6e 616d 655f 736f 6c76 6572  n)...name_solver
+00000650: da0a 656e 7472 7970 6f69 6e74 7213 0000  ..entrypointr...
+00000660: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
+00000670: da12 6765 745f 736f 6c76 6572 5f70 6163  ..get_solver_pac
+00000680: 6b61 6765 3c00 0000 7312 0000 000a 0e02  kage<...s.......
+00000690: 010a 020c 010a 0102 ff08 0204 010e 0272  ...............r
+000006a0: 1f00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+000006b0: 0004 0000 0005 0000 0043 0000 0073 5e00  .........C...s^.
+000006c0: 0000 7c00 6401 1b00 7d01 7c01 a000 a100  ..|.d...}.|.....
+000006d0: 730c 7c00 6402 1b00 7d01 7c01 a000 a100  s.|.d...}.|.....
+000006e0: 721a 7401 7c01 6403 8d01 7d02 7c02 6a02  r.t.|.d...}.|.j.
+000006f0: 7d03 7c03 5300 7403 a004 6404 7c01 9b00  }.|.S.t...d.|...
+00000700: 6405 9d03 a101 0100 7c00 a005 a100 6a06  d.......|.....j.
+00000710: a007 6406 a101 6407 1900 7d03 7c03 5300  ..d...d...}.|.S.
+00000720: 2908 7ae6 4465 7465 6374 7320 7368 6f72  ).z.Detects shor
+00000730: 7420 6e61 6d65 206f 6620 7468 6520 736f  t name of the so
+00000740: 6c76 6572 2066 726f 6d20 6060 696e 666f  lver from ``info
+00000750: 5f73 6f6c 7665 722e 786d 6c60 6020 6966  _solver.xml`` if
+00000760: 2070 7265 7365 6e74 206f 720a 2020 2020   present or.    
+00000770: 7468 6520 7061 7468 2e0a 0a20 2020 2050  the path...    P
+00000780: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+00000790: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2070 6174  --------.    pat
+000007a0: 685f 6469 723a 2070 6174 682d 6c69 6b65  h_dir: path-like
+000007b0: 0a20 2020 2020 2020 2050 6174 6820 746f  .        Path to
+000007c0: 2061 2073 696d 756c 6174 696f 6e20 6469   a simulation di
+000007d0: 7265 6374 6f72 790a 0a20 2020 2052 6574  rectory..    Ret
+000007e0: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
+000007f0: 0a20 2020 2073 686f 7274 5f6e 616d 653a  .    short_name:
+00000800: 2073 7472 0a0a 2020 2020 7a0f 696e 666f   str..    z.info
+00000810: 5f73 6f6c 7665 722e 786d 6c7a 1e2e 6461  _solver.xmlz..da
+00000820: 7461 5f66 6c75 6964 7369 6d2f 696e 666f  ta_fluidsim/info
+00000830: 5f73 6f6c 7665 722e 786d 6c29 01da 0970  _solver.xml)...p
+00000840: 6174 685f 6669 6c65 7a04 5468 6520 7a45  ath_filez.The zE
+00000850: 2066 696c 6520 6973 206d 6973 7369 6e67   file is missing
+00000860: 2120 4174 7465 6d70 7469 6e67 2074 6f20  ! Attempting to 
+00000870: 6775 6573 7320 736f 6c76 6572 2066 726f  guess solver fro
+00000880: 6d20 7468 6520 6469 7265 6374 6f72 7920  m the directory 
+00000890: 6e61 6d65 2eda 015f 7201 0000 0029 08da  name..._r....)..
+000008a0: 0665 7869 7374 7372 0600 0000 da0a 7368  .existsr......sh
+000008b0: 6f72 745f 6e61 6d65 7208 0000 00da 0777  ort_namer......w
+000008c0: 6172 6e69 6e67 da08 6162 736f 6c75 7465  arning..absolute
+000008d0: da04 6e61 6d65 da05 7370 6c69 7429 04da  ..name..split)..
+000008e0: 0870 6174 685f 6469 725a 0f69 6e66 6f5f  .path_dirZ.info_
+000008f0: 736f 6c76 6572 5f78 6d6c da0b 696e 666f  solver_xml..info
+00000900: 5f73 6f6c 7665 7272 2300 0000 7215 0000  _solverr#...r...
+00000910: 0072 1500 0000 7216 0000 00da 1567 6574  .r....r......get
+00000920: 5f73 6f6c 7665 725f 7368 6f72 745f 6e61  _solver_short_na
+00000930: 6d65 5600 0000 7318 0000 0008 0e08 0108  meV...s.........
+00000940: 0108 020a 0106 0104 0804 fa0a 0104 ff14  ................
+00000950: 0404 0272 2a00 0000 2913 da07 5f5f 646f  ...r*...)...__do
+00000960: 635f 5f72 0b00 0000 da09 6675 6e63 746f  c__r......functo
+00000970: 6f6c 7372 0200 0000 da07 706b 6775 7469  olsr......pkguti
+00000980: 6c72 0300 0000 da05 7479 7065 7372 0400  lr......typesr..
+00000990: 0000 5a0d 666c 7569 6473 696d 5f63 6f72  ..Z.fluidsim_cor
+000009a0: 6572 0500 0000 5a12 666c 7569 6473 696d  er....Z.fluidsim
+000009b0: 5f63 6f72 652e 696e 666f 7206 0000 00da  _core.infor.....
+000009c0: 036c 6f67 7208 0000 0072 1900 0000 da10  .logr....r......
+000009d0: 696d 706f 7274 5f63 6c73 5f73 696d 756c  import_cls_simul
+000009e0: 7217 0000 0072 1f00 0000 722a 0000 0072  r....r....r*...r
+000009f0: 1500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+00000a00: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000a10: 0073 2600 0000 0400 080a 0c01 0c01 0c01  .s&.............
+00000a20: 0c02 0c01 0c02 0202 0601 06ff 0603 0204  ................
+00000a30: 0601 06ff 0603 0803 081a 0c1a            ............
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/solvers/__pycache__/base.cpython-310.pyc` & `fluidsimfoam-0.0.3/src/fluidsimfoam/solvers/__pycache__/base.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 21 01:35:47 2023 UTC, .py size: 1683 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,103 +1,112 @@
-00000000: 6f0d 0d0a 0000 0000 73e8 4164 9306 0000  o.......s.Ad....
+00000000: 6f0d 0d0a 0000 0000 6541 5a64 4107 0000  o.......eAZdA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c08 6d09 5a09 0100 4700 6406 6407  d.l.m.Z...G.d.d.
-00000070: 8400 6407 6507 8303 5a0a 6408 5300 2909  ..d.e...Z.d.S.).
-00000080: e900 0000 0029 01da 0450 6174 6829 01da  .....)...Path)..
-00000090: 0a75 6e64 6572 7363 6f72 6529 01da 036d  .underscore)...m
-000000a0: 7069 2901 da09 5369 6d75 6c43 6f72 6529  pi)...SimulCore)
-000000b0: 01da 066c 6f67 6765 7263 0000 0000 0000  ...loggerc......
-000000c0: 0000 0000 0000 0000 0000 0400 0000 0000  ................
-000000d0: 0000 733c 0000 0065 005a 0164 005a 0264  ..s<...e.Z.d.Z.d
-000000e0: 015a 0365 0464 0264 0384 0083 015a 0565  .Z.e.d.d.....Z.e
-000000f0: 0487 0066 0164 0464 0584 0883 015a 0687  ...f.d.d.....Z..
-00000100: 0066 0164 0664 0784 085a 0787 0004 005a  .f.d.d...Z.....Z
-00000110: 0853 0029 08da 0953 696d 756c 466f 616d  .S.)...SimulFoam
-00000120: 7a15 4261 7365 204f 7065 6e46 4f41 4d20  z.Base OpenFOAM 
-00000130: 736f 6c76 6572 2e63 0200 0000 0000 0000  solver.c........
-00000140: 0000 0000 0200 0000 0100 0000 4300 0000  ............C...
-00000150: 7304 0000 0064 0053 00a9 014e a900 a902  s....d.S...N....
-00000160: da03 636c 73da 0670 6172 616d 7372 0900  ..cls..paramsr..
-00000170: 0000 7209 0000 00fa 3e2f 686f 6d65 2f70  ..r.....>/home/p
-00000180: 6965 7272 652f 4465 762f 666c 7569 6473  ierre/Dev/fluids
-00000190: 696d 666f 616d 2f73 7263 2f66 6c75 6964  imfoam/src/fluid
-000001a0: 7369 6d66 6f61 6d2f 736f 6c76 6572 732f  simfoam/solvers/
-000001b0: 6261 7365 2e70 79da 1d5f 636f 6d70 6c65  base.py.._comple
-000001c0: 7465 5f70 6172 616d 735f 7769 7468 5f64  te_params_with_d
-000001d0: 6566 6175 6c74 0d00 0000 7302 0000 0004  efault....s.....
-000001e0: 027a 2753 696d 756c 466f 616d 2e5f 636f  .z'SimulFoam._co
-000001f0: 6d70 6c65 7465 5f70 6172 616d 735f 7769  mplete_params_wi
-00000200: 7468 5f64 6566 6175 6c74 6301 0000 0000  th_defaultc.....
-00000210: 0000 0000 0000 0002 0000 0002 0000 0003  ................
-00000220: 0000 0073 0e00 0000 7400 8300 a001 a100  ...s....t.......
-00000230: 7d01 7c01 5300 7208 0000 0029 02da 0573  }.|.S.r....)...s
-00000240: 7570 6572 da15 6372 6561 7465 5f64 6566  uper..create_def
-00000250: 6175 6c74 5f70 6172 616d 7372 0a00 0000  ault_paramsr....
-00000260: a901 da09 5f5f 636c 6173 735f 5f72 0900  ....__class__r..
-00000270: 0000 720d 0000 0072 1000 0000 1100 0000  ..r....r........
-00000280: 7304 0000 000a 0304 017a 1f53 696d 756c  s........z.Simul
-00000290: 466f 616d 2e63 7265 6174 655f 6465 6661  Foam.create_defa
-000002a0: 756c 745f 7061 7261 6d73 6302 0000 0000  ult_paramsc.....
-000002b0: 0000 0000 0000 0006 0000 0008 0000 0003  ................
-000002c0: 0000 0073 de00 0000 7400 8300 a001 7c01  ...s....t.....|.
-000002d0: a101 0100 6401 a002 6402 7403 7c00 8301  ....d...d.t.|...
-000002e0: a102 7c00 5f04 7c00 6a05 a006 a100 7d02  ..|._.|.j.....}.
-000002f0: 7c02 a007 a100 4400 5d25 5c02 7d03 7d04  |.....D.]%\.}.}.
-00000300: 7408 7c00 7c04 8302 7222 7118 7409 7c03  t.|.|...r"q.t.|.
-00000310: 8301 7d05 740a 7c00 7c05 7c04 7c00 8301  ..}.t.|.|.|.|...
-00000320: 8303 0100 7c00 0400 6a04 6401 a002 6403  ....|...j.d...d.
-00000330: 7c05 9b00 6404 9d03 7c04 a102 3700 0200  |...d...|...7...
-00000340: 5f04 7118 6405 7c02 7600 725e 7c01 6a0b  _.q.d.|.v.r^|.j.
-00000350: 7350 740c 7c01 6a0d 8301 0400 7c00 5f0d  sPt.|.j.....|._.
-00000360: 7c00 6a0e 5f0d 6e07 740c 7c00 6a0e 6a0d  |.j._.n.t.|.j.j.
-00000370: 8301 7c00 5f0d 7c00 6a0e a00f a100 0100  ..|._.|.j.......
-00000380: 6400 5300 6400 7c00 5f0d 7410 6a11 6406  d.S.d.|._.t.j.d.
-00000390: 6b02 726d 7412 a013 6407 a101 0100 6400  k.rmt...d.....d.
-000003a0: 5300 6400 5300 2908 4e7a 097b 3a32 3873  S.d.S.).Nz.{:28s
-000003b0: 7d7b 7d0a 7a05 7369 6d3a 207a 0473 696d  }{}.z.sim: z.sim
-000003c0: 2e7a 023a 20da 064f 7574 7075 7472 0100  .z.: ..Outputr..
-000003d0: 0000 7a1c 4e6f 206f 7574 7075 7420 636c  ..z.No output cl
-000003e0: 6173 7320 696e 6974 6961 6c69 7a65 6421  ass initialized!
-000003f0: 2914 720f 0000 00da 085f 5f69 6e69 745f  ).r......__init_
-00000400: 5fda 0666 6f72 6d61 74da 0474 7970 655a  _..format..typeZ
-00000410: 115f 6f62 6a65 6374 735f 746f 5f70 7269  ._objects_to_pri
-00000420: 6e74 da0b 696e 666f 5f73 6f6c 7665 72da  nt..info_solver.
-00000430: 0e69 6d70 6f72 745f 636c 6173 7365 73da  .import_classes.
-00000440: 0569 7465 6d73 da0a 6973 696e 7374 616e  .items..isinstan
-00000450: 6365 7203 0000 00da 0773 6574 6174 7472  cer......setattr
-00000460: da0f 4e45 575f 4449 525f 5245 5355 4c54  ..NEW_DIR_RESULT
-00000470: 5372 0200 0000 da08 7061 7468 5f72 756e  Sr......path_run
-00000480: da06 6f75 7470 7574 da09 706f 7374 5f69  ..output..post_i
-00000490: 6e69 7472 0400 0000 da04 7261 6e6b 7206  nitr......rankr.
-000004a0: 0000 00da 0777 6172 6e69 6e67 2906 da04  .....warning)...
-000004b0: 7365 6c66 720c 0000 00da 0c64 6963 745f  selfr......dict_
-000004c0: 636c 6173 7365 73da 0863 6c73 5f6e 616d  classes..cls_nam
-000004d0: 65da 0543 6c61 7373 da08 6f62 6a5f 6e61  e..Class..obj_na
-000004e0: 6d65 7211 0000 0072 0900 0000 720d 0000  mer....r....r...
-000004f0: 0072 1400 0000 1700 0000 7328 0000 000c  .r........s(....
-00000500: 0112 020a 0110 030a 0202 0108 0210 010a  ................
-00000510: 010c 010a ff08 0406 0116 010e 040e 0206  ................
-00000520: 020a 010e 0104 ff7a 1253 696d 756c 466f  .......z.SimulFo
-00000530: 616d 2e5f 5f69 6e69 745f 5f29 09da 085f  am.__init__)..._
-00000540: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000550: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000560: 5fda 075f 5f64 6f63 5f5f da0b 636c 6173  _..__doc__..clas
-00000570: 736d 6574 686f 6472 0e00 0000 7210 0000  smethodr....r...
-00000580: 0072 1400 0000 da0d 5f5f 636c 6173 7363  .r......__classc
-00000590: 656c 6c5f 5f72 0900 0000 7209 0000 0072  ell__r....r....r
-000005a0: 1100 0000 720d 0000 0072 0700 0000 0a00  ....r....r......
-000005b0: 0000 730e 0000 0008 0004 0102 020a 0102  ..s.............
-000005c0: 030e 0114 0572 0700 0000 4e29 0bda 0770  .....r....N)...p
-000005d0: 6174 686c 6962 7202 0000 005a 0a69 6e66  athlibr....Z.inf
-000005e0: 6c65 6374 696f 6e72 0300 0000 5a0d 666c  lectionr....Z.fl
-000005f0: 7569 6464 796e 2e75 7469 6c72 0400 0000  uiddyn.utilr....
-00000600: 5a14 666c 7569 6473 696d 5f63 6f72 652e  Z.fluidsim_core.
-00000610: 736f 6c76 6572 7205 0000 005a 1066 6c75  solverr....Z.flu
-00000620: 6964 7369 6d66 6f61 6d2e 6c6f 6772 0600  idsimfoam.logr..
-00000630: 0000 7207 0000 0072 0900 0000 7209 0000  ..r....r....r...
-00000640: 0072 0900 0000 720d 0000 00da 083c 6d6f  .r....r......<mo
-00000650: 6475 6c65 3e01 0000 0073 0c00 0000 0c00  dule>....s......
-00000660: 0c02 0c02 0c01 0c01 1403                 ..........
+00000020: 0004 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
+00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
+00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
+00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
+00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
+00000070: 6407 6c0b 6d0c 5a0c 0100 4700 6408 6409  d.l.m.Z...G.d.d.
+00000080: 8400 6409 6508 8303 5a0d 640a 5300 290b  ..d.e...Z.d.S.).
+00000090: 7a21 4261 7365 2063 6c61 7373 2066 6f72  z!Base class for
+000000a0: 2074 6865 2060 6073 696d 6060 206f 626a   the ``sim`` obj
+000000b0: 6563 74e9 0000 0000 2901 da04 5061 7468  ect.....)...Path
+000000c0: 2901 da0a 756e 6465 7273 636f 7265 2901  )...underscore).
+000000d0: da03 6d70 6929 01da 0953 696d 756c 436f  ..mpi)...SimulCo
+000000e0: 7265 2901 da06 6c6f 6767 6572 2901 da0a  re)...logger)...
+000000f0: 5061 7261 6d65 7465 7273 6300 0000 0000  Parametersc.....
+00000100: 0000 0000 0000 0000 0000 0004 0000 0000  ................
+00000110: 0000 0073 4000 0000 6500 5a01 6400 5a02  ...s@...e.Z.d.Z.
+00000120: 6401 5a03 6504 5a04 6505 6402 6403 8400  d.Z.e.Z.e.d.d...
+00000130: 8301 5a06 6505 8700 6601 6404 6405 8408  ..Z.e...f.d.d...
+00000140: 8301 5a07 8700 6601 6406 6407 8408 5a08  ..Z...f.d.d...Z.
+00000150: 8700 0400 5a09 5300 2908 da09 5369 6d75  ....Z.S.)...Simu
+00000160: 6c46 6f61 6d7a 1e42 6173 6520 4f70 656e  lFoamz.Base Open
+00000170: 464f 414d 2046 6c75 6964 7369 6d20 736f  FOAM Fluidsim so
+00000180: 6c76 6572 2e63 0200 0000 0000 0000 0000  lver.c..........
+00000190: 0000 0200 0000 0100 0000 4300 0000 7304  ..........C...s.
+000001a0: 0000 0064 0053 00a9 014e a900 a902 da03  ...d.S...N......
+000001b0: 636c 73da 0670 6172 616d 7372 0a00 0000  cls..paramsr....
+000001c0: 720a 0000 00fa 3e2f 686f 6d65 2f70 6965  r.....>/home/pie
+000001d0: 7272 652f 4465 762f 666c 7569 6473 696d  rre/Dev/fluidsim
+000001e0: 666f 616d 2f73 7263 2f66 6c75 6964 7369  foam/src/fluidsi
+000001f0: 6d66 6f61 6d2f 736f 6c76 6572 732f 6261  mfoam/solvers/ba
+00000200: 7365 2e70 79da 1d5f 636f 6d70 6c65 7465  se.py.._complete
+00000210: 5f70 6172 616d 735f 7769 7468 5f64 6566  _params_with_def
+00000220: 6175 6c74 1200 0000 7302 0000 0004 027a  ault....s......z
+00000230: 2753 696d 756c 466f 616d 2e5f 636f 6d70  'SimulFoam._comp
+00000240: 6c65 7465 5f70 6172 616d 735f 7769 7468  lete_params_with
+00000250: 5f64 6566 6175 6c74 6301 0000 0000 0000  _defaultc.......
+00000260: 0000 0000 0002 0000 0002 0000 0003 0000  ................
+00000270: 0073 0e00 0000 7400 8300 a001 a100 7d01  .s....t.......}.
+00000280: 7c01 5300 7209 0000 0029 02da 0573 7570  |.S.r....)...sup
+00000290: 6572 da15 6372 6561 7465 5f64 6566 6175  er..create_defau
+000002a0: 6c74 5f70 6172 616d 7372 0b00 0000 a901  lt_paramsr......
+000002b0: da09 5f5f 636c 6173 735f 5f72 0a00 0000  ..__class__r....
+000002c0: 720e 0000 0072 1100 0000 1600 0000 7304  r....r........s.
+000002d0: 0000 000a 0304 017a 1f53 696d 756c 466f  .......z.SimulFo
+000002e0: 616d 2e63 7265 6174 655f 6465 6661 756c  am.create_defaul
+000002f0: 745f 7061 7261 6d73 6302 0000 0000 0000  t_paramsc.......
+00000300: 0000 0000 0006 0000 0008 0000 0003 0000  ................
+00000310: 0073 e200 0000 7400 8300 a001 7c01 a101  .s....t.....|...
+00000320: 0100 6401 a002 6402 7403 7c00 8301 a102  ..d...d.t.|.....
+00000330: 7c00 5f04 7c00 6a05 a006 a100 7d02 7c02  |._.|.j.....}.|.
+00000340: a007 a100 4400 5d25 5c02 7d03 7d04 7408  ....D.]%\.}.}.t.
+00000350: 7c00 7c04 8302 7222 7118 7409 7c03 8301  |.|...r"q.t.|...
+00000360: 7d05 740a 7c00 7c05 7c04 7c00 8301 8303  }.t.|.|.|.|.....
+00000370: 0100 7c00 0400 6a04 6401 a002 6403 7c05  ..|...j.d...d.|.
+00000380: 9b00 6404 9d03 7c04 a102 3700 0200 5f04  ..d...|...7..._.
+00000390: 7118 6405 7c02 7600 725d 7c01 6a0b 7350  q.d.|.v.r]|.j.sP
+000003a0: 740c 7c01 6a0d 8301 0400 7c00 5f0d 7c00  t.|.j.....|._.|.
+000003b0: 6a0e 5f0d 6e07 740c 7c00 6a0e 6a0d 8301  j._.n.t.|.j.j...
+000003c0: 7c00 5f0d 7c00 6a0e a00f a100 0100 6e0d  |._.|.j.......n.
+000003d0: 6400 7c00 5f0d 7410 6a11 6406 6b02 726a  d.|._.t.j.d.k.rj
+000003e0: 7412 a013 6407 a101 0100 7c00 6a0e 6a14  t...d.....|.j.j.
+000003f0: 7c00 5f14 6400 5300 2908 4e7a 097b 3a32  |._.d.S.).Nz.{:2
+00000400: 3873 7d7b 7d0a 7a05 7369 6d3a 207a 0473  8s}{}.z.sim: z.s
+00000410: 696d 2e7a 023a 20da 064f 7574 7075 7472  im.z.: ..Outputr
+00000420: 0100 0000 7a1c 4e6f 206f 7574 7075 7420  ....z.No output 
+00000430: 636c 6173 7320 696e 6974 6961 6c69 7a65  class initialize
+00000440: 6421 2915 7210 0000 00da 085f 5f69 6e69  d!).r......__ini
+00000450: 745f 5fda 0666 6f72 6d61 74da 0474 7970  t__..format..typ
+00000460: 655a 115f 6f62 6a65 6374 735f 746f 5f70  eZ._objects_to_p
+00000470: 7269 6e74 da0b 696e 666f 5f73 6f6c 7665  rint..info_solve
+00000480: 72da 0e69 6d70 6f72 745f 636c 6173 7365  r..import_classe
+00000490: 73da 0569 7465 6d73 da0a 6973 696e 7374  s..items..isinst
+000004a0: 616e 6365 7203 0000 00da 0773 6574 6174  ancer......setat
+000004b0: 7472 da0f 4e45 575f 4449 525f 5245 5355  tr..NEW_DIR_RESU
+000004c0: 4c54 5372 0200 0000 da08 7061 7468 5f72  LTSr......path_r
+000004d0: 756e da06 6f75 7470 7574 da09 706f 7374  un..output..post
+000004e0: 5f69 6e69 7472 0400 0000 da04 7261 6e6b  _initr......rank
+000004f0: 7206 0000 00da 0777 6172 6e69 6e67 5a0b  r......warningZ.
+00000500: 696e 7075 745f 6669 6c65 7329 06da 0473  input_files)...s
+00000510: 656c 6672 0d00 0000 da0c 6469 6374 5f63  elfr......dict_c
+00000520: 6c61 7373 6573 da08 636c 735f 6e61 6d65  lasses..cls_name
+00000530: da05 436c 6173 73da 086f 626a 5f6e 616d  ..Class..obj_nam
+00000540: 6572 1200 0000 720a 0000 0072 0e00 0000  er....r....r....
+00000550: 7215 0000 001c 0000 0073 2800 0000 0c01  r........s(.....
+00000560: 1202 0a01 1003 0a02 0201 0802 1001 0a01  ................
+00000570: 0c01 0aff 0804 0601 1601 0e04 0c02 0602  ................
+00000580: 0a01 0a01 0e02 7a12 5369 6d75 6c46 6f61  ......z.SimulFoa
+00000590: 6d2e 5f5f 696e 6974 5f5f 290a da08 5f5f  m.__init__)...__
+000005a0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+000005b0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+000005c0: da07 5f5f 646f 635f 5f72 0700 0000 da0b  ..__doc__r......
+000005d0: 636c 6173 736d 6574 686f 6472 0f00 0000  classmethodr....
+000005e0: 7211 0000 0072 1500 0000 da0d 5f5f 636c  r....r......__cl
+000005f0: 6173 7363 656c 6c5f 5f72 0a00 0000 720a  asscell__r....r.
+00000600: 0000 0072 1200 0000 720e 0000 0072 0800  ...r....r....r..
+00000610: 0000 0d00 0000 7310 0000 0008 0004 0104  ......s.........
+00000620: 0202 020a 0102 030e 0114 0572 0800 0000  ...........r....
+00000630: 4e29 0e72 2b00 0000 da07 7061 7468 6c69  N).r+.....pathli
+00000640: 6272 0200 0000 da0a 696e 666c 6563 7469  br......inflecti
+00000650: 6f6e 7203 0000 005a 0d66 6c75 6964 6479  onr....Z.fluiddy
+00000660: 6e2e 7574 696c 7204 0000 005a 1466 6c75  n.utilr....Z.flu
+00000670: 6964 7369 6d5f 636f 7265 2e73 6f6c 7665  idsim_core.solve
+00000680: 7272 0500 0000 5a10 666c 7569 6473 696d  rr....Z.fluidsim
+00000690: 666f 616d 2e6c 6f67 7206 0000 00da 1366  foam.logr......f
+000006a0: 6c75 6964 7369 6d66 6f61 6d2e 7061 7261  luidsimfoam.para
+000006b0: 6d73 7207 0000 0072 0800 0000 720a 0000  msr....r....r...
+000006c0: 0072 0a00 0000 720a 0000 0072 0e00 0000  .r....r....r....
+000006d0: da08 3c6d 6f64 756c 653e 0100 0000 7310  ..<module>....s.
+000006e0: 0000 0004 000c 020c 020c 020c 010c 010c  ................
+000006f0: 0114 03                                  ...
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/solvers/base.py` & `fluidsimfoam-0.0.3/src/fluidsimfoam/solvers/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,23 @@
+"""Base class for the ``sim`` object"""
+
 from pathlib import Path
 
 from inflection import underscore
 
 from fluiddyn.util import mpi  # noqa: F401
 from fluidsim_core.solver import SimulCore
 from fluidsimfoam.log import logger
+from fluidsimfoam.params import Parameters
 
 
 class SimulFoam(SimulCore):
-    """Base OpenFOAM solver."""
+    """Base OpenFOAM Fluidsim solver."""
+
+    Parameters = Parameters
 
     @classmethod
     def _complete_params_with_default(cls, params):
         pass
 
     @classmethod
     def create_default_params(cls):
@@ -47,7 +52,9 @@
                 self.path_run = Path(self.output.path_run)
 
             self.output.post_init()
         else:
             self.path_run = None
             if mpi.rank == 0:
                 logger.warning("No output class initialized!")
+
+        self.input_files = self.output.input_files
```

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/util/__pycache__/console.cpython-310.pyc` & `fluidsimfoam-0.0.3/src/fluidsimfoam/util/__pycache__/console.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.2/src/fluidsimfoam/util/console.py` & `fluidsimfoam-0.0.3/src/fluidsimfoam/util/console.py`

 * *Files identical despite different names*

