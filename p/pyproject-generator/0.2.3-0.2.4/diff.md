# Comparing `tmp/pyproject-generator-0.2.3.tar.gz` & `tmp/pyproject-generator-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-generator-0.2.3.tar", last modified: Sun May  7 22:37:15 2023, max compression
+gzip compressed data, was "pyproject-generator-0.2.4.tar", last modified: Tue May  9 15:02:25 2023, max compression
```

## Comparing `pyproject-generator-0.2.3.tar` & `pyproject-generator-0.2.4.tar`

### file list

```diff
@@ -1,40 +1,45 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-07 22:37:15.403766 pyproject-generator-0.2.3/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1078 2023-05-04 01:48:13.000000 pyproject-generator-0.2.3/LICENSE
--rw-r--r--   0 cangyuanli   (501) staff       (20)     4200 2023-05-07 22:37:15.404135 pyproject-generator-0.2.3/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3659 2023-05-06 14:06:08.000000 pyproject-generator-0.2.3/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      264 2023-05-05 02:42:29.000000 pyproject-generator-0.2.3/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-05-07 22:37:15.405511 pyproject-generator-0.2.3/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-07 22:37:15.370496 pyproject-generator-0.2.3/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-07 22:37:15.379989 pyproject-generator-0.2.3/src/pyproject/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       51 2023-05-05 02:42:30.000000 pyproject-generator-0.2.3/src/pyproject/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-05-07 22:37:10.000000 pyproject-generator-0.2.3/src/pyproject/__version__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     4070 2023-05-06 12:36:27.000000 pyproject-generator-0.2.3/src/pyproject/cli.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-07 22:37:15.382112 pyproject-generator-0.2.3/src/pyproject/config/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      337 2023-05-05 15:13:27.000000 pyproject-generator-0.2.3/src/pyproject/config/default_config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1029 2023-05-05 02:42:30.000000 pyproject-generator-0.2.3/src/pyproject/licenses.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1727 2023-05-05 12:40:42.000000 pyproject-generator-0.2.3/src/pyproject/logger.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)    16834 2023-05-07 22:02:11.000000 pyproject-generator-0.2.3/src/pyproject/project_builder.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2851 2023-05-06 22:21:55.000000 pyproject-generator-0.2.3/src/pyproject/spinner.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-07 22:37:15.397328 pyproject-generator-0.2.3/src/pyproject/templates/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1498 2023-05-03 19:23:49.000000 pyproject-generator-0.2.3/src/pyproject/templates/gitignore.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.2.3/src/pyproject/templates/license_apache.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1457 2023-05-04 13:35:45.000000 pyproject-generator-0.2.3/src/pyproject/templates/license_bsd3.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:11:38.000000 pyproject-generator-0.2.3/src/pyproject/templates/license_gpl_v3.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.2.3/src/pyproject/templates/license_mit.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      905 2023-05-03 23:48:11.000000 pyproject-generator-0.2.3/src/pyproject/templates/pre_commit_config.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      263 2023-05-04 02:15:39.000000 pyproject-generator-0.2.3/src/pyproject/templates/pyproject.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1040 2023-05-04 20:10:03.000000 pyproject-generator-0.2.3/src/pyproject/templates/readme.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      603 2023-05-05 12:52:13.000000 pyproject-generator-0.2.3/src/pyproject/templates/setup.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.2.3/src/pyproject/templates/tests.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.2.3/src/pyproject/templates/tox.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      189 2023-05-05 20:21:04.000000 pyproject-generator-0.2.3/src/pyproject/utils.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-07 22:37:15.400538 pyproject-generator-0.2.3/src/pyproject_generator.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     4200 2023-05-07 22:37:15.000000 pyproject-generator-0.2.3/src/pyproject_generator.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1095 2023-05-07 22:37:15.000000 pyproject-generator-0.2.3/src/pyproject_generator.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-05-07 22:37:15.000000 pyproject-generator-0.2.3/src/pyproject_generator.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-05-07 22:37:15.000000 pyproject-generator-0.2.3/src/pyproject_generator.egg-info/entry_points.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-05-07 22:37:15.000000 pyproject-generator-0.2.3/src/pyproject_generator.egg-info/requires.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-05-07 22:37:15.000000 pyproject-generator-0.2.3/src/pyproject_generator.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-07 22:37:15.402686 pyproject-generator-0.2.3/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      303 2023-05-06 12:39:33.000000 pyproject-generator-0.2.3/tests/test_cli.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1802 2023-05-06 12:35:08.000000 pyproject-generator-0.2.3/tests/test_pyproject.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-09 15:02:25.026131 pyproject-generator-0.2.4/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1078 2023-05-04 01:48:13.000000 pyproject-generator-0.2.4/LICENSE
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     4200 2023-05-09 15:02:25.026440 pyproject-generator-0.2.4/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3659 2023-05-09 02:31:28.000000 pyproject-generator-0.2.4/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      264 2023-05-08 15:13:51.000000 pyproject-generator-0.2.4/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      874 2023-05-09 15:02:25.027523 pyproject-generator-0.2.4/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-09 15:02:24.974986 pyproject-generator-0.2.4/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-09 15:02:24.988418 pyproject-generator-0.2.4/src/pyproject/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       51 2023-05-05 02:42:30.000000 pyproject-generator-0.2.4/src/pyproject/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-05-09 15:02:16.000000 pyproject-generator-0.2.4/src/pyproject/__version__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     4706 2023-05-08 19:41:06.000000 pyproject-generator-0.2.4/src/pyproject/cli.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-09 15:02:24.989662 pyproject-generator-0.2.4/src/pyproject/config/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      337 2023-05-05 15:13:27.000000 pyproject-generator-0.2.4/src/pyproject/config/default_config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2246 2023-05-09 13:28:26.000000 pyproject-generator-0.2.4/src/pyproject/licenses.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1727 2023-05-05 12:40:42.000000 pyproject-generator-0.2.4/src/pyproject/logger.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    16184 2023-05-08 19:41:53.000000 pyproject-generator-0.2.4/src/pyproject/project_builder.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2905 2023-05-08 19:42:00.000000 pyproject-generator-0.2.4/src/pyproject/spinner.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-09 15:02:25.016996 pyproject-generator-0.2.4/src/pyproject/templates/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1498 2023-05-03 19:23:49.000000 pyproject-generator-0.2.4/src/pyproject/templates/gitignore.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    34503 2023-05-09 13:30:26.000000 pyproject-generator-0.2.4/src/pyproject/templates/license_agpl_v3.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      549 2023-05-09 02:32:18.000000 pyproject-generator-0.2.4/src/pyproject/templates/license_apache_v2.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1292 2023-05-09 00:48:28.000000 pyproject-generator-0.2.4/src/pyproject/templates/license_bsd2.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1457 2023-05-04 13:35:45.000000 pyproject-generator-0.2.4/src/pyproject/templates/license_bsd3.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    18092 2023-05-09 00:34:37.000000 pyproject-generator-0.2.4/src/pyproject/templates/license_gpl_v2.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    35149 2023-05-09 00:33:45.000000 pyproject-generator-0.2.4/src/pyproject/templates/license_gpl_v3.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     7633 2023-05-09 13:30:26.000000 pyproject-generator-0.2.4/src/pyproject/templates/license_lgpl_v3.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.2.4/src/pyproject/templates/license_mit.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    16726 2023-05-09 00:40:15.000000 pyproject-generator-0.2.4/src/pyproject/templates/license_mozilla_v2.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      905 2023-05-03 23:48:11.000000 pyproject-generator-0.2.4/src/pyproject/templates/pre_commit_config.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      263 2023-05-04 02:15:39.000000 pyproject-generator-0.2.4/src/pyproject/templates/pyproject.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1040 2023-05-04 20:10:03.000000 pyproject-generator-0.2.4/src/pyproject/templates/readme.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      603 2023-05-05 12:52:13.000000 pyproject-generator-0.2.4/src/pyproject/templates/setup.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.2.4/src/pyproject/templates/tests.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.2.4/src/pyproject/templates/tox.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      220 2023-05-07 23:06:58.000000 pyproject-generator-0.2.4/src/pyproject/utils.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-09 15:02:25.022922 pyproject-generator-0.2.4/src/pyproject_generator.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     4200 2023-05-09 15:02:24.000000 pyproject-generator-0.2.4/src/pyproject_generator.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1342 2023-05-09 15:02:24.000000 pyproject-generator-0.2.4/src/pyproject_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-05-09 15:02:24.000000 pyproject-generator-0.2.4/src/pyproject_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-05-09 15:02:24.000000 pyproject-generator-0.2.4/src/pyproject_generator.egg-info/entry_points.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       18 2023-05-09 15:02:24.000000 pyproject-generator-0.2.4/src/pyproject_generator.egg-info/requires.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-05-09 15:02:24.000000 pyproject-generator-0.2.4/src/pyproject_generator.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-09 15:02:25.025166 pyproject-generator-0.2.4/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1001 2023-05-09 02:01:59.000000 pyproject-generator-0.2.4/tests/test_cli.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1808 2023-05-09 06:04:34.000000 pyproject-generator-0.2.4/tests/test_pyproject.py
```

### Comparing `pyproject-generator-0.2.3/LICENSE` & `pyproject-generator-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.3/PKG-INFO` & `pyproject-generator-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.2.3
+Version: 0.2.4
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.2.3/README.md` & `pyproject-generator-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.3/setup.cfg` & `pyproject-generator-0.2.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	platformdirs
+	rich
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 pyproject = 
 	py.typed
```

### Comparing `pyproject-generator-0.2.3/src/pyproject/cli.py` & `pyproject-generator-0.2.4/src/pyproject/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 import argparse
+import re
 import typing
 from typing import Optional
 
 from .__version__ import __version__
 from .licenses import LICENSES
 from .logger import Level, Logger
 from .project_builder import Action, ProjectBuilder
 
 ACTIONS = typing.get_args(Action)
 ALLOWED_LICENSES = tuple(LICENSES.keys())
 
 
+def _validate_project_name(project_name: str) -> None:
+    # https://packaging.python.org/en/latest/specifications/name-normalization/
+    regex = "^([A-Z0-9]|[A-Z0-9][A-Z0-9._-]*[A-Z0-9])$"
+    if not bool(re.match(regex, project_name, re.IGNORECASE)):
+        raise ValueError(
+            "A valid project name may only contain ASCII letters, numbers, ., -,"
+            " and/or _, and they must begin and end with a letter or number."
+        )
+
+
 def _parse_arg_to_set(string: Optional[str], sep: str = ",") -> set[str]:
     """Expects a delimited string of arguments, e.g. `a,b,c,d`. Transforms string
     into a set.
 
     Args:
         string (Optional[str]): `a,b,c,d`
         sep (str): What to split on
@@ -84,16 +95,22 @@
     return parser
 
 
 def _validate_input(args, logger: Logger):
     if args.action not in ACTIONS:
         logger.error(f"Invalid choice `{args.action}`, choose from {ACTIONS}")
 
-    if args.action == "init" and args.project_name is None:
-        logger.error("Action `init` requires project name")
+    if args.action == "init":
+        if args.project_name is None:
+            logger.error("Action `init` requires project name")
+        else:
+            try:
+                _validate_project_name(args.project_name)
+            except ValueError as e:
+                logger.error(str(e))
 
     if args.license not in LICENSES and args.license is not None:
         logger.error(f"Invalid choice `{args.license}`, choose from {ALLOWED_LICENSES}")
 
 
 def main():
     parser = get_parser()
```

### Comparing `pyproject-generator-0.2.3/src/pyproject/logger.py` & `pyproject-generator-0.2.4/src/pyproject/logger.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.3/src/pyproject/project_builder.py` & `pyproject-generator-0.2.4/src/pyproject/project_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from __future__ import annotations
 
 import dataclasses
 import datetime
 import json
 import os
-import re
 import shutil
 import string
 import subprocess
 import venv
 from pathlib import Path
 from types import SimpleNamespace
 from typing import Literal, Optional, Union
@@ -153,24 +152,14 @@
         self._template_path = Path(template_path)
         self._logger = logger
 
         self._user_config_dir = Path(user_config_dir)
         self._create_config_dir()
         self._config = self._set_config(config)
 
-    @staticmethod
-    def _validate_project_name(project_name: str) -> None:
-        # https://packaging.python.org/en/latest/specifications/name-normalization/
-        regex = "^([A-Z0-9]|[A-Z0-9][A-Z0-9._-]*[A-Z0-9])$"
-        if not bool(re.match(regex, project_name, re.IGNORECASE)):
-            raise ValueError(
-                "A valid project name may only contain ASCII letters, numbers, ., -,"
-                " and/or _, and they must begin and end with a letter or number."
-            )
-
     def _create_config_dir(self) -> None:
         """Create the user config directory if it does not exist. Since the default
         configuration may add keys, merge the two, preferring the
         existing config so we don't overwrite user changes.
         """
         self._user_config_dir.mkdir(exist_ok=True)
         config_file = self._user_config_dir / "config.json"
@@ -275,19 +264,14 @@
         """Called when user specifies `action = init`.
 
         Args:
             project_name (str): User-supplied name of project
         """
 
         # Create the project directory
-        try:
-            self._validate_project_name(project_name)
-        except ValueError as e:
-            self._logger.error(str(e))
-
         proj_path = self.proj_path / project_name
 
         try:
             proj_path.mkdir()
         except FileExistsError:
             self._logger.error(f"{proj_path} already exists")
```

### Comparing `pyproject-generator-0.2.3/src/pyproject/spinner.py` & `pyproject-generator-0.2.4/src/pyproject/spinner.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import threading
 import time
 from typing import Optional
 
 from rich.console import Console
 
 BACKSPACE = "\b"
-CLEAR_LINE = "\033[K"
+CLEAR_LINE = "\033[K"  # https://tldp.org/HOWTO/Bash-Prompt-HOWTO/x361.html
 CHECKMARK = "[green]\u2713[/green]"
 XMARK = "[red]\u2717[/red]"
 
 
 class Spinner:
     def __init__(
         self,
```

### Comparing `pyproject-generator-0.2.3/src/pyproject/templates/gitignore.template` & `pyproject-generator-0.2.4/src/pyproject/templates/gitignore.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.3/src/pyproject/templates/license_apache.template` & `pyproject-generator-0.2.4/src/pyproject/templates/license_apache_v2.template`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
-limitations under the License.
+limitations under the License.
```

### Comparing `pyproject-generator-0.2.3/src/pyproject/templates/license_bsd3.template` & `pyproject-generator-0.2.4/src/pyproject/templates/license_bsd3.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.3/src/pyproject/templates/license_mit.template` & `pyproject-generator-0.2.4/src/pyproject/templates/license_mit.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.3/src/pyproject/templates/pre_commit_config.template` & `pyproject-generator-0.2.4/src/pyproject/templates/pre_commit_config.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.3/src/pyproject/templates/readme.template` & `pyproject-generator-0.2.4/src/pyproject/templates/readme.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.3/src/pyproject/templates/setup.template` & `pyproject-generator-0.2.4/src/pyproject/templates/setup.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.3/src/pyproject/templates/tests.template` & `pyproject-generator-0.2.4/src/pyproject/templates/tests.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.3/src/pyproject_generator.egg-info/PKG-INFO` & `pyproject-generator-0.2.4/src/pyproject_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.2.3
+Version: 0.2.4
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.2.3/src/pyproject_generator.egg-info/SOURCES.txt` & `pyproject-generator-0.2.4/src/pyproject_generator.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,23 @@
 src/pyproject/licenses.py
 src/pyproject/logger.py
 src/pyproject/project_builder.py
 src/pyproject/spinner.py
 src/pyproject/utils.py
 src/pyproject/config/default_config.json
 src/pyproject/templates/gitignore.template
-src/pyproject/templates/license_apache.template
+src/pyproject/templates/license_agpl_v3.template
+src/pyproject/templates/license_apache_v2.template
+src/pyproject/templates/license_bsd2.template
 src/pyproject/templates/license_bsd3.template
+src/pyproject/templates/license_gpl_v2.template
 src/pyproject/templates/license_gpl_v3.template
+src/pyproject/templates/license_lgpl_v3.template
 src/pyproject/templates/license_mit.template
+src/pyproject/templates/license_mozilla_v2.template
 src/pyproject/templates/pre_commit_config.template
 src/pyproject/templates/pyproject.template
 src/pyproject/templates/readme.template
 src/pyproject/templates/setup.template
 src/pyproject/templates/tests.template
 src/pyproject/templates/tox.template
 src/pyproject_generator.egg-info/PKG-INFO
```

### Comparing `pyproject-generator-0.2.3/tests/test_pyproject.py` & `pyproject-generator-0.2.4/tests/test_pyproject.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 CONFIG2: dict = {
     "pypi_username": "username",
     "pypi_password": "password",
     "github_url": "url",
     "author": "author",
     "email": "email",
-    "license": "apache",
+    "license": "apache_v2",
     "set_dependencies": {"black", "ruff", "pytest"},
     "add_dependencies": {"white"},
     "remove_dependencies": {"black"},
     "reset_config": False,
     "show": False,
 }
 
@@ -63,10 +63,10 @@
     builder = pb.ProjectBuilder(config=CONFIG2, options={}, logger=logger.Level.INFO)
     assert builder._config == pb.Config(
         pypi_username="username",
         pypi_password="password",
         github_url="url",
         author="author",
         email="email",
-        license="apache",
+        license="apache_v2",
         dependencies={"white", "ruff", "pytest"},
     )
```

