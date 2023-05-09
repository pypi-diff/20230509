# Comparing `tmp/alfred_pyflow-0.4.3.tar.gz` & `tmp/alfred_pyflow-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred_pyflow-0.4.3.tar", max compression
+gzip compressed data, was "alfred_pyflow-0.4.4.tar", max compression
```

## Comparing `alfred_pyflow-0.4.3.tar` & `alfred_pyflow-0.4.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       15 2023-05-09 08:08:04.789940 alfred_pyflow-0.4.3/README.md
--rw-r--r--   0        0        0       31 2023-05-09 08:08:04.789940 alfred_pyflow-0.4.3/pyflow/__init__.py
--rw-r--r--   0        0        0      542 2023-05-09 08:08:04.789940 alfred_pyflow-0.4.3/pyflow/cache.py
--rw-r--r--   0        0        0     6609 2023-05-09 08:08:04.789940 alfred_pyflow-0.4.3/pyflow/icon.py
--rw-r--r--   0        0        0     2629 2023-05-09 08:08:04.789940 alfred_pyflow-0.4.3/pyflow/item.py
--rw-r--r--   0        0        0     1592 2023-05-09 08:08:04.789940 alfred_pyflow-0.4.3/pyflow/testing.py
--rw-r--r--   0        0        0     2344 2023-05-09 08:08:04.789940 alfred_pyflow-0.4.3/pyflow/workflow.py
--rw-r--r--   0        0        0      981 2023-05-09 08:08:04.789940 alfred_pyflow-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 alfred_pyflow-0.4.3/setup.py
--rw-r--r--   0        0        0     1078 1970-01-01 00:00:00.000000 alfred_pyflow-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0       15 2023-05-09 08:32:00.165791 alfred_pyflow-0.4.4/README.md
+-rw-r--r--   0        0        0       31 2023-05-09 08:32:00.165791 alfred_pyflow-0.4.4/pyflow/__init__.py
+-rw-r--r--   0        0        0      542 2023-05-09 08:32:00.165791 alfred_pyflow-0.4.4/pyflow/cache.py
+-rw-r--r--   0        0        0     6609 2023-05-09 08:32:00.165791 alfred_pyflow-0.4.4/pyflow/icon.py
+-rw-r--r--   0        0        0     2629 2023-05-09 08:32:00.165791 alfred_pyflow-0.4.4/pyflow/item.py
+-rw-r--r--   0        0        0     1578 2023-05-09 08:32:00.165791 alfred_pyflow-0.4.4/pyflow/testing.py
+-rw-r--r--   0        0        0     2344 2023-05-09 08:32:00.165791 alfred_pyflow-0.4.4/pyflow/workflow.py
+-rw-r--r--   0        0        0      981 2023-05-09 08:32:00.165791 alfred_pyflow-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 alfred_pyflow-0.4.4/setup.py
+-rw-r--r--   0        0        0     1078 1970-01-01 00:00:00.000000 alfred_pyflow-0.4.4/PKG-INFO
```

### Comparing `alfred_pyflow-0.4.3/pyflow/cache.py` & `alfred_pyflow-0.4.4/pyflow/cache.py`

 * *Files identical despite different names*

### Comparing `alfred_pyflow-0.4.3/pyflow/icon.py` & `alfred_pyflow-0.4.4/pyflow/icon.py`

 * *Files identical despite different names*

### Comparing `alfred_pyflow-0.4.3/pyflow/item.py` & `alfred_pyflow-0.4.4/pyflow/item.py`

 * *Files identical despite different names*

### Comparing `alfred_pyflow-0.4.3/pyflow/testing.py` & `alfred_pyflow-0.4.4/pyflow/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,25 +27,24 @@
     def alfred_workflow_version(self) -> str:
         return self.cmd("poetry version --short")
 
     @property
     def alfred_workflow_cache(self) -> str:
         return f"/tmp/{self.alfred_workflow_name}"
 
-    @property
-    def workflow(self) -> Workflow:
+    def workflow(self, **envs) -> Workflow:
         os.environ.setdefault("alfred_debug", self.alfred_debug)
         os.environ.setdefault("alfred_workflow_bundleid", self.alfred_workflow_bundleid)
         os.environ.setdefault("alfred_workflow_name", self.alfred_workflow_name)
         os.environ.setdefault("alfred_workflow_version", self.alfred_workflow_version)
         os.environ.setdefault("alfred_workflow_cache", self.alfred_workflow_cache)
 
-        return Workflow()
-
-    def run_workflow(self, workflow: Workflow, target: callable, *args, **envs) -> dict:
         for key, value in envs.items():
             os.environ.setdefault(key, value)
 
-        sys.argv = [""] + list(args)
+        return Workflow()
 
+    def run_workflow(self, workflow: Workflow, target: callable, *args) -> dict:
+        sys.argv = [""] + list(args)
         workflow.run(target)
+
         return workflow.serialized
```

### Comparing `alfred_pyflow-0.4.3/pyflow/workflow.py` & `alfred_pyflow-0.4.4/pyflow/workflow.py`

 * *Files identical despite different names*

### Comparing `alfred_pyflow-0.4.3/pyproject.toml` & `alfred_pyflow-0.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "alfred-pyflow"
 description = "Minimal library for the development of Alfred Workflows."
 documentation = "https://github.com/fedecalendino/alfred-pyflow/blob/main/README.md"
 homepage = "https://github.com/fedecalendino/alfred-pyflow"
 license = "MIT"
 readme = "README.md"
-version = "0.4.3"
+version = "0.4.4"
 
 authors = [
   "Fede Calendino <fede@calendino.com>",
 ]
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
```

### Comparing `alfred_pyflow-0.4.3/setup.py` & `alfred_pyflow-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.30.0,<3.0.0', 'urllib3==2.0.2']
 
 setup_kwargs = {
     'name': 'alfred-pyflow',
-    'version': '0.4.3',
+    'version': '0.4.4',
     'description': 'Minimal library for the development of Alfred Workflows.',
     'long_description': '# alfred-pyflow',
     'author': 'Fede Calendino',
     'author_email': 'fede@calendino.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fedecalendino/alfred-pyflow',
```

### Comparing `alfred_pyflow-0.4.3/PKG-INFO` & `alfred_pyflow-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred-pyflow
-Version: 0.4.3
+Version: 0.4.4
 Summary: Minimal library for the development of Alfred Workflows.
 Home-page: https://github.com/fedecalendino/alfred-pyflow
 License: MIT
 Keywords: alfred,workflow
 Author: Fede Calendino
 Author-email: fede@calendino.com
 Requires-Python: >=3.8,<4.0
```

