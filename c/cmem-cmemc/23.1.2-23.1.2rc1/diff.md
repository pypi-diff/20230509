# Comparing `tmp/cmem_cmemc-23.1.2.tar.gz` & `tmp/cmem_cmemc-23.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_cmemc-23.1.2.tar", max compression
+gzip compressed data, was "cmem_cmemc-23.1.2rc1.tar", max compression
```

## Comparing `cmem_cmemc-23.1.2.tar` & `cmem_cmemc-23.1.2rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    11357 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/LICENSE
--rw-r--r--   0        0        0      808 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/README-public.md
--rw-r--r--   0        0        0      109 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/__init__.py
--rw-r--r--   0        0        0       28 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/__init__.py
--rw-r--r--   0        0        0     5571 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/__init__.py
--rw-r--r--   0        0        0     3311 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/__init__.py
--rw-r--r--   0        0        0     6709 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/admin.py
--rw-r--r--   0        0        0     5562 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/config.py
--rw-r--r--   0        0        0    27505 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/dataset.py
--rw-r--r--   0        0        0    27110 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/graph.py
--rw-r--r--   0        0        0     7808 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/metrics.py
--rw-r--r--   0        0        0    17612 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/project.py
--rw-r--r--   0        0        0     6948 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/python.py
--rw-r--r--   0        0        0    27725 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/query.py
--rw-r--r--   0        0        0     7556 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/resource.py
--rw-r--r--   0        0        0     8192 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/scheduler.py
--rw-r--r--   0        0        0     6961 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/store.py
--rw-r--r--   0        0        0    10654 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/user.py
--rw-r--r--   0        0        0    16218 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/vocabulary.py
--rw-r--r--   0        0        0    21832 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/workflow.py
--rw-r--r--   0        0        0     4761 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/workspace.py
--rw-r--r--   0        0        0    38221 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/completion.py
--rw-r--r--   0        0        0    15648 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/context.py
--rw-r--r--   0        0        0      139 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/exceptions.py
--rw-r--r--   0        0        0       43 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/manual_helper/__init__.py
--rw-r--r--   0        0        0     3261 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/manual_helper/graph.py
--rw-r--r--   0        0        0    11127 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/manual_helper/multi_page.py
--rw-r--r--   0        0        0     1303 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/manual_helper/single_page.py
--rw-r--r--   0        0        0     8086 2023-05-09 08:11:21.787894 cmem_cmemc-23.1.2/cmem/cmemc/cli/utils.py
--rw-r--r--   0        0        0     2381 2023-05-09 08:11:39.955778 cmem_cmemc-23.1.2/pyproject.toml
--rw-r--r--   0        0        0     2542 1970-01-01 00:00:00.000000 cmem_cmemc-23.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-18 07:15:37.943836 cmem_cmemc-23.1.2rc1/LICENSE
+-rw-r--r--   0        0        0      808 2023-01-18 07:15:37.943900 cmem_cmemc-23.1.2rc1/README-public.md
+-rw-r--r--   0        0        0      109 2023-01-18 07:15:37.944108 cmem_cmemc-23.1.2rc1/cmem/__init__.py
+-rw-r--r--   0        0        0       28 2023-01-18 07:15:37.944190 cmem_cmemc-23.1.2rc1/cmem/cmemc/__init__.py
+-rw-r--r--   0        0        0     5571 2023-04-28 12:54:24.692339 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/__init__.py
+-rw-r--r--   0        0        0     3311 2023-02-14 08:17:24.862278 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/__init__.py
+-rw-r--r--   0        0        0     6709 2023-04-21 12:08:15.190979 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/admin.py
+-rw-r--r--   0        0        0     5562 2023-03-15 16:42:29.626951 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/config.py
+-rw-r--r--   0        0        0    27505 2023-04-21 06:37:45.132177 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/dataset.py
+-rw-r--r--   0        0        0    27110 2023-03-15 16:42:29.627797 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/graph.py
+-rw-r--r--   0        0        0     7808 2023-03-15 16:42:29.628159 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/metrics.py
+-rw-r--r--   0        0        0    17612 2023-03-15 16:42:29.628389 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/project.py
+-rw-r--r--   0        0        0     6948 2023-03-15 16:42:29.628590 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/python.py
+-rw-r--r--   0        0        0    27725 2023-03-15 16:42:29.628916 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/query.py
+-rw-r--r--   0        0        0     7556 2023-03-15 16:42:29.629062 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/resource.py
+-rw-r--r--   0        0        0     8192 2023-03-15 16:42:29.629342 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/scheduler.py
+-rw-r--r--   0        0        0     6961 2023-03-15 16:42:29.629976 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/store.py
+-rw-r--r--   0        0        0    10654 2023-02-15 15:36:55.698463 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/user.py
+-rw-r--r--   0        0        0    16218 2023-03-15 16:42:29.630243 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/vocabulary.py
+-rw-r--r--   0        0        0    21832 2023-03-15 16:42:29.630535 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/workflow.py
+-rw-r--r--   0        0        0     4761 2023-03-15 16:42:29.630851 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/workspace.py
+-rw-r--r--   0        0        0    38221 2023-04-21 06:37:45.133132 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/completion.py
+-rw-r--r--   0        0        0    15648 2023-04-24 20:44:46.137043 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/context.py
+-rw-r--r--   0        0        0      139 2023-01-18 07:15:37.946025 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/exceptions.py
+-rw-r--r--   0        0        0       43 2023-01-18 07:15:37.946113 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/manual_helper/__init__.py
+-rw-r--r--   0        0        0     3261 2023-01-18 07:15:37.946179 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/manual_helper/graph.py
+-rw-r--r--   0        0        0    11127 2023-04-28 12:54:24.692606 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/manual_helper/multi_page.py
+-rw-r--r--   0        0        0     1303 2023-01-18 07:15:37.946315 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/manual_helper/single_page.py
+-rw-r--r--   0        0        0     8086 2023-04-24 20:44:46.137197 cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/utils.py
+-rw-r--r--   0        0        0     2384 2023-05-05 14:31:45.416295 cmem_cmemc-23.1.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     2545 1970-01-01 00:00:00.000000 cmem_cmemc-23.1.2rc1/PKG-INFO
```

### Comparing `cmem_cmemc-23.1.2/LICENSE` & `cmem_cmemc-23.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/README-public.md` & `cmem_cmemc-23.1.2rc1/README-public.md`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/__init__.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/__init__.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/admin.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/admin.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/config.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/dataset.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/dataset.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/graph.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/graph.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/metrics.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/project.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/project.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/python.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/python.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/query.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/query.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/resource.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/resource.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/scheduler.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/scheduler.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/store.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/store.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/user.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/user.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/vocabulary.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/vocabulary.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/workflow.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/workflow.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/commands/workspace.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/commands/workspace.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/completion.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/completion.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/context.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/context.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/manual_helper/graph.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/manual_helper/graph.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/manual_helper/multi_page.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/manual_helper/multi_page.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/manual_helper/single_page.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/manual_helper/single_page.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/cmem/cmemc/cli/utils.py` & `cmem_cmemc-23.1.2rc1/cmem/cmemc/cli/utils.py`

 * *Files identical despite different names*

### Comparing `cmem_cmemc-23.1.2/pyproject.toml` & `cmem_cmemc-23.1.2rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-cmemc"
-version = "23.1.2"
+version = "23.1.2rc1"
 description = "Command line client for eccenca Corporate Memory"
 license = "Apache 2.0"
 classifiers = ["Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "Intended Audience :: Science/Research", "Intended Audience :: System Administrators", "License :: OSI Approved :: Apache Software License", "Programming Language :: Python :: 3.9", "Topic :: Software Development :: Testing", "Topic :: Database", "Topic :: Utilities"]
 homepage = "https://eccenca.com/go/cmemc"
 authors = ["eccenca <cmempy-developer@eccenca.com>", "Sebastian Tramp <sebastian.tramp@eccenca.com>"]
 readme = "README-public.md"
 packages = [
```

### Comparing `cmem_cmemc-23.1.2/PKG-INFO` & `cmem_cmemc-23.1.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmem-cmemc
-Version: 23.1.2
+Version: 23.1.2rc1
 Summary: Command line client for eccenca Corporate Memory
 Home-page: https://eccenca.com/go/cmemc
 License: Apache 2.0
 Author: eccenca
 Author-email: cmempy-developer@eccenca.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

