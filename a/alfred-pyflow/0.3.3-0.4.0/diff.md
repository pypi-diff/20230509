# Comparing `tmp/alfred-pyflow-0.3.3.tar.gz` & `tmp/alfred_pyflow-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred-pyflow-0.3.3.tar", last modified: Wed Dec 21 16:23:49 2022, max compression
+gzip compressed data, was "alfred_pyflow-0.4.0.tar", max compression
```

## Comparing `alfred-pyflow-0.3.3.tar` & `alfred_pyflow-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       15 2022-12-21 16:23:20.679521 alfred-pyflow-0.3.3/README.md
--rw-r--r--   0        0        0       31 2022-12-21 16:23:20.679521 alfred-pyflow-0.3.3/pyflow/__init__.py
--rw-r--r--   0        0        0      541 2022-12-21 16:23:20.679521 alfred-pyflow-0.3.3/pyflow/cache.py
--rw-r--r--   0        0        0     6609 2022-12-21 16:23:20.679521 alfred-pyflow-0.3.3/pyflow/icon.py
--rw-r--r--   0        0        0     2629 2022-12-21 16:23:20.679521 alfred-pyflow-0.3.3/pyflow/item.py
--rw-r--r--   0        0        0     2312 2022-12-21 16:23:20.679521 alfred-pyflow-0.3.3/pyflow/workflow.py
--rw-r--r--   0        0        0      919 2022-12-21 16:23:20.679521 alfred-pyflow-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      705 2022-12-21 16:23:49.857039 alfred-pyflow-0.3.3/setup.py
--rw-r--r--   0        0        0      792 2022-12-21 16:23:49.857300 alfred-pyflow-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       15 2023-05-09 07:14:52.171790 alfred_pyflow-0.4.0/README.md
+-rw-r--r--   0        0        0       31 2023-05-09 07:14:52.171790 alfred_pyflow-0.4.0/pyflow/__init__.py
+-rw-r--r--   0        0        0      542 2023-05-09 07:14:52.171790 alfred_pyflow-0.4.0/pyflow/cache.py
+-rw-r--r--   0        0        0     6609 2023-05-09 07:14:52.171790 alfred_pyflow-0.4.0/pyflow/icon.py
+-rw-r--r--   0        0        0     2629 2023-05-09 07:14:52.171790 alfred_pyflow-0.4.0/pyflow/item.py
+-rw-r--r--   0        0        0     1303 2023-05-09 07:14:52.171790 alfred_pyflow-0.4.0/pyflow/testing.py
+-rw-r--r--   0        0        0     2344 2023-05-09 07:14:52.171790 alfred_pyflow-0.4.0/pyflow/workflow.py
+-rw-r--r--   0        0        0      963 2023-05-09 07:14:52.171790 alfred_pyflow-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 alfred_pyflow-0.4.0/setup.py
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 alfred_pyflow-0.4.0/PKG-INFO
```

### Comparing `alfred-pyflow-0.3.3/pyflow/cache.py` & `alfred_pyflow-0.4.0/pyflow/cache.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+
 import requests
 
 
 class Cache:
     def __init__(self, cachedir: str):
         if not os.path.exists(cachedir):
             os.makedirs(cachedir)
```

### Comparing `alfred-pyflow-0.3.3/pyflow/icon.py` & `alfred_pyflow-0.4.0/pyflow/icon.py`

 * *Files identical despite different names*

### Comparing `alfred-pyflow-0.3.3/pyflow/item.py` & `alfred_pyflow-0.4.0/pyflow/item.py`

 * *Files identical despite different names*

### Comparing `alfred-pyflow-0.3.3/pyflow/workflow.py` & `alfred_pyflow-0.4.0/pyflow/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import os
 import json
-import sys
-from typing import Dict, List
 import logging
+import os
+import sys
 from logging import Logger, INFO, DEBUG
+from typing import Dict, List
 
 from .cache import Cache
-from .item import Item
 from .icon import Icon
+from .item import Item
 
 
 class Workflow:
     def __init__(self):
         self._cache: Cache = None
         self._env: Dict[str, str] = None
         self._items: List[dict] = []
@@ -77,16 +77,16 @@
             self.new_item(
                 title=str(e),
                 subtitle=f"Error while running workflow '{self.name}:v{self.version}'",
             ).set_icon_builtin(
                 icon=Icon.ALERT_STOP,
             )
 
-    def send_feedback(self):
-        json.dump(self.serialized, sys.stdout)
+    def send_feedback(self, indent: int = 2):
+        json.dump(self.serialized, sys.stdout, indent=indent)
         sys.stdout.flush()
 
     @property
     def serialized(self) -> dict:
         return {
             "items": list(
                 map(
```

### Comparing `alfred-pyflow-0.3.3/pyproject.toml` & `alfred_pyflow-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 [tool.poetry]
 name = "alfred-pyflow"
 description = "Minimal library for the development of Alfred Workflows."
 documentation = "https://github.com/fedecalendino/alfred-pyflow/blob/main/README.md"
 homepage = "https://github.com/fedecalendino/alfred-pyflow"
 license = "MIT"
 readme = "README.md"
-version = "0.3.3"
+version = "0.4.0"
 
 authors = [
   "Fede Calendino <fede@calendino.com>",
 ]
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
 ]
 keywords = [
   "alfred",
   "workflow",
 ]
 packages = [
   { include = "pyflow" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requests = "^2.28.1"
+requests = "^2.30.0"
 
 [tool.poetry.dev-dependencies]
-black = "^22.6.0"
-ddt = "^1.5.0"
-coverage = "^6.4.2"
+black = "^23.3.0"
+ddt = "^1.6.0"
+coverage = "^7.2.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `alfred-pyflow-0.3.3/setup.py` & `alfred_pyflow-0.4.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 packages = \
 ['pyflow']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['requests>=2.28.1,<3.0.0']
+['requests>=2.30.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'alfred-pyflow',
-    'version': '0.3.3',
+    'version': '0.4.0',
     'description': 'Minimal library for the development of Alfred Workflows.',
     'long_description': '# alfred-pyflow',
     'author': 'Fede Calendino',
     'author_email': 'fede@calendino.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/fedecalendino/alfred-pyflow',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

