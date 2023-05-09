# Comparing `tmp/raspunzel-0.2.0.tar.gz` & `tmp/raspunzel-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspunzel-0.2.0.tar", last modified: Thu Sep 15 08:21:15 2022, max compression
+gzip compressed data, was "raspunzel-0.3.0.tar", last modified: Tue May  9 16:28:26 2023, max compression
```

## Comparing `raspunzel-0.2.0.tar` & `raspunzel-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,11 @@
--rw-r--r--   0        0        0       12 2022-08-18 16:01:08.081282 raspunzel-0.2.0/.gitignore
--rw-r--r--   0        0        0      275 2022-09-15 08:16:51.264816 raspunzel-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2022-08-18 14:54:15.489192 raspunzel-0.2.0/LICENSE
--rw-r--r--   0        0        0      801 2022-09-15 08:21:06.515881 raspunzel-0.2.0/README.md
--rw-r--r--   0        0        0     1231 2022-09-14 13:01:56.341783 raspunzel-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3146 2022-09-15 08:17:04.816767 raspunzel-0.2.0/raspunzel/__init__.py
--rw-r--r--   0        0        0     1044 2022-09-04 16:09:51.095609 raspunzel-0.2.0/raspunzel/build.py
--rw-r--r--   0        0        0     3287 2022-08-28 17:13:51.325450 raspunzel-0.2.0/raspunzel/run.py
--rw-r--r--   0        0        0     1984 2022-08-19 16:01:25.736057 raspunzel-0.2.0/raspunzel/spdlog.py
--rw-r--r--   0        0        0     1606 2022-08-28 17:26:14.663218 raspunzel-0.2.0/raspunzel/sync.py
--rw-r--r--   0        0        0     1711 2022-08-28 17:07:34.228672 raspunzel-0.2.0/raspunzel/utils.py
--rw-r--r--   0        0        0     2109 2022-08-28 17:16:45.289572 raspunzel-0.2.0/raspunzel/workspace.py
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 raspunzel-0.2.0/setup.py
--rw-r--r--   0        0        0     1916 1970-01-01 00:00:00.000000 raspunzel-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-04-11 14:24:26.535838 raspunzel-0.3.0/.gitignore
+-rw-r--r--   0        0        0      411 2023-05-09 16:27:17.569713 raspunzel-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-04-11 14:24:26.535838 raspunzel-0.3.0/LICENSE
+-rw-r--r--   0        0        0      671 2023-05-09 16:25:42.374916 raspunzel-0.3.0/README.md
+-rw-r--r--   0        0        0     1632 2023-05-09 16:28:09.913051 raspunzel-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2120 2023-05-09 16:27:24.713622 raspunzel-0.3.0/raspunzel/__init__.py
+-rw-r--r--   0        0        0     3301 2023-05-09 16:25:04.419395 raspunzel-0.3.0/raspunzel/run.py
+-rw-r--r--   0        0        0     1497 2023-05-09 16:25:04.419395 raspunzel-0.3.0/raspunzel/utils.py
+-rw-r--r--   0        0        0     2175 2023-05-09 16:25:04.423395 raspunzel-0.3.0/raspunzel/workspace.py
+-rwxr-xr-x   0        0        0     6978 2023-05-09 16:25:04.423395 raspunzel-0.3.0/standalone/raspunzel
+-rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 raspunzel-0.3.0/PKG-INFO
```

### Comparing `raspunzel-0.2.0/LICENSE` & `raspunzel-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `raspunzel-0.2.0/pyproject.toml` & `raspunzel-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -10,34 +10,56 @@
 ]
 maintainers = [
     {name = "Stéphane Caron", email = "stephane.caron@normalesup.org"},
 ]
 dynamic = ['version', 'description']
 requires-python = ">=3.7"
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 dependencies = [
 ]
+keywords = ["raspberry pi", "bazel", "cross-compilation", "deploy"]
 
 [project.optional-dependencies]
 doc = ["sphinx"]
 
 [project.scripts]
 raspunzel = "raspunzel:main"
 
 [project.urls]
 Source = "https://github.com/tasts-robots/raspunzel"
 Tracker = "https://github.com/tasts-robots/raspunzel/issues"
 Changelog = "https://github.com/tasts-robots/raspunzel/blob/master/CHANGELOG.md"
 
 [tool.black]
 line-length = 79
+
+[tool.ruff]
+line-length = 79
+select = [
+    # pyflakes
+    "F",
+    # pycodestyle
+    "E",
+    "W",
+    # isort
+    "I001",
+    # pydocstyle
+    "D"
+]
+ignore = [
+    "D401",  # good for methods but not for class docstrings
+    "D405",  # British-style section names are also "proper"!
+]
+
+[tool.ruff.pydocstyle]
+convention = "google"
```

### Comparing `raspunzel-0.2.0/raspunzel/__init__.py` & `raspunzel-0.3.0/raspunzel/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,32 +11,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Deploy and run Bazel targets on a Raspberry Pi.
-"""
+"""Deploy and run Bazel targets on a Raspberry Pi."""
 
 import argparse
+import logging
 import os
 import sys
 
-from .build import build
 from .run import run
-from .spdlog import logging
-from .sync import sync
 from .workspace import Workspace
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 
 def get_argument_parser() -> argparse.ArgumentParser:
+    """Get command-line argument parser."""
     parser = argparse.ArgumentParser(description=__doc__)
     parser.add_argument(
         "-s",
         "--sudo",
         default=False,
         action="store_true",
         help="run as administrator (sudo -E)",
@@ -44,65 +41,31 @@
     parser.add_argument(
         "-v",
         "--verbose",
         default=False,
         action="store_true",
         help="verbose mode",
     )
-    subparsers = parser.add_subparsers(title="subcommands", dest="subcmd")
-
-    # build -------------------------------------------------------------------
-    parser_build = subparsers.add_parser(
-        "build",
-        help="build Bazel targets listed in a project file",
-    )
-    parser_build.add_argument("target", help="Bazel target")
-    parser_build.add_argument(
-        "subargs",
-        nargs=argparse.REMAINDER,
-        help="arguments forwarded to the target",
-    )
-
-    # run ---------------------------------------------------------------------
-    parser_run = subparsers.add_parser(
-        "run",
-        help="run a Bazel target",
-    )
-    parser_run.add_argument("target", help="Bazel target")
-    parser_run.add_argument(
+    parser.add_argument("command", help="Bazel command")
+    parser.add_argument("target", help="Bazel target")
+    parser.add_argument(
         "subargs",
         nargs=argparse.REMAINDER,
         help="arguments forwarded to the target",
     )
-
-    # sync --------------------------------------------------------------------
-    parser_sync = subparsers.add_parser(
-        "sync",
-        help="sync Bazel workspace with the remote host",
-    )
-    parser_sync.add_argument(
-        "destination",
-        help="destination in rsync+ssh format [user@]host:path",
-    )
-
     return parser
 
 
 def main(argv=None):
+    """Entry point for the command-line tool."""
     parser = get_argument_parser()
     args = parser.parse_args(argv)
-    if args.subcmd is None:
-        parser.print_help()
-        sys.exit(-1)
     if args.verbose:
         logger = logging.getLogger()
         logger.setLevel(logging.INFO)
     if args.sudo and os.geteuid() != 0:
         args = ["sudo", "-E", sys.executable] + sys.argv + [os.environ]
         os.execlpe("sudo", *args)
-
-    if args.subcmd == "build":
-        build(args.target, args.subargs)
-    elif args.subcmd == "run":
+    if args.command == "run":
         run(Workspace(), args.target, args.subargs)
-    elif args.subcmd == "sync":
-        sync(Workspace(), args.destination)
+    else:  # unknown command
+        logging.error(f'Command "{args.command}" not available with raspunzel')
```

### Comparing `raspunzel-0.2.0/raspunzel/run.py` & `raspunzel-0.3.0/raspunzel/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,39 +11,37 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Deploy and run Bazel targets on the Raspberry Pi.
-"""
+"""Deploy and run Bazel targets on the Raspberry Pi."""
 
+import logging
 import os
 from os import path
 from typing import List
 
-from .spdlog import logging
 from .workspace import Workspace
 
 
 def read_arch(bazel_bin, target, name):
+    """Read system architecture."""
     suffix = "-2.params"
     if path.exists(f"{bazel_bin}/{target}/{name}_spine-2.params"):
         suffix = "_spine-2.params"  # for C++ agents
     with open(f"{bazel_bin}/{target}/{name}{suffix}", "r") as params:
         for line in params:
             if line.startswith("bazel-out"):
                 return line.split("/")[1]
 
 
 def log_run(target_name: str, arch: str) -> None:
-    """
-    Log target name and build configuration.
+    """Log target name and build configuration.
 
     Args:
         target_name: Name of the Bazel target.
         arch: Build configuration found.
     """
     RED: str = "\033[31m"
     GREEN: str = "\033[32m"
@@ -60,16 +58,15 @@
     elif "unknown" in arch:
         color = RED
     target_message += color + arch + RESET
     logging.info(target_message)
 
 
 def run(workspace: Workspace, target: str, subargs: List[str]) -> None:
-    """
-    Run target from a Bazel workspace.
+    """Run target from a Bazel workspace.
 
     Args:
         workspace: Bazel workspace information.
         target: Label of the Bazel target to run.
         subargs: Command-line arguments for the target.
     """
     try:
@@ -86,15 +83,15 @@
     if target_dir[0] == "@":
         external_name, target_dir = target_dir[1:].split("//")
         target_dir = f"external/{external_name}/{target_dir}"
 
     try:
         arch = read_arch(workspace.bazel_bin, target_dir, target_name)
     except FileNotFoundError:
-        logging.warn(
+        logging.warning(
             "Couldn't read arch from "
             f"'{workspace.bazel_bin}/{target_dir}/{target_name}-2.params', "
             "maybe the target is not a Python script?"
         )
         arch = "unknown"
 
     log_run(target_name, arch)
```

### Comparing `raspunzel-0.2.0/raspunzel/utils.py` & `raspunzel-0.3.0/raspunzel/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,30 +11,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Utility functions.
-"""
+"""Utility functions."""
 
 import os
 from os import path
 from typing import Optional
 
-import subprocess
-
-from .spdlog import logging
-
 
 def find_file(name: str, required: bool) -> Optional[str]:
-    """
-    Search for a file or directory in the script's parent folders.
+    """Search for a file or directory in the script's parent folders.
 
     Args:
         name: Name of the file or directory to search.
         required: If True, raise an exception if the file is not found.
 
     Returns:
         File path, if found, None otherwise.
@@ -50,15 +43,7 @@
         old_path = cur_path
         cur_path = path.dirname(cur_path)
         if cur_path == old_path:
             break
     if required:
         raise FileNotFoundError(f"Cannot find {name} in parent folders")
     return None
-
-
-def sh(*args, **kwargs):
-    """
-    Run a shell command.
-    """
-    logging.info("run: " + args[0])
-    subprocess.check_call(*args, shell=True, **kwargs)
```

### Comparing `raspunzel-0.2.0/raspunzel/workspace.py` & `raspunzel-0.3.0/raspunzel/workspace.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""Bazel workspace information."""
+
+import logging
 from os import path
 
-from .spdlog import logging
 from .utils import find_file
 
 
 def get_workspace_name(workspace_file: str) -> str:
-    """
-    Read workspace name from WORKSPACE file.
+    """Read workspace name from WORKSPACE file.
 
     Args:
         workspace_file: Path to WORKSPACE file.
 
     Returns:
         Workspace name, if found.
 
@@ -42,31 +43,30 @@
         "Could not find name in WORKSPACE. "
         "Note that we don't parse Starlark beyond "
         '``workspace(name = "something")``.'
     )
 
 
 class Workspace:
-
-    """
-    Bazel workspace information.
+    """Bazel workspace information.
 
     Attributes:
         bazel_bin: Path to bazel-bin directory.
         name: Name of the workspace, defined in WORKSPACE file.
         root: Path to the workspace root directory.
     """
 
     bazel_bin: str
     name: str
     root: str
 
     def __init__(self):
+        """Initialize Bazel workspace information."""
         bazel_bin = find_file("bazel-bin", required=True)
         workspace_file = find_file("WORKSPACE", required=True)
         name = get_workspace_name(workspace_file)
         logging.info(f"Found bazel-bin at {bazel_bin}")
         logging.info(f"Found workspace file at {workspace_file}")
-        logging.info(f"Read workspace name as '{name}'")
+        logging.info(f'Read workspace name as "{name}"')
         self.bazel_bin = bazel_bin
         self.name = name
         self.root = path.dirname(workspace_file)
```

### Comparing `raspunzel-0.2.0/PKG-INFO` & `raspunzel-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: raspunzel
-Version: 0.2.0
+Version: 0.3.0
 Summary: Deploy and run Bazel targets on a Raspberry Pi.
+Keywords: raspberry pi,bazel,cross-compilation,deploy
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,39 +21,27 @@
 Project-URL: Changelog, https://github.com/tasts-robots/raspunzel/blob/master/CHANGELOG.md
 Project-URL: Source, https://github.com/tasts-robots/raspunzel
 Project-URL: Tracker, https://github.com/tasts-robots/raspunzel/issues
 Provides-Extra: doc
 
 # raspunzel
 
-Command-line tool to deploy and run cross-compiled Bazel targets on a Raspberry Pi.
-
-## Installation
-
-```console
-pip install raspunzel
-```
-
-## Usage
-
-The basic usage for ``raspunzel`` goes in three steps. First, build all cross-compiled targets locally:
+Command-line tool to run Bazel targets on systems where Bazel is not installed. For instance, we can run cross-compiled Bazel targets on a Raspberry Pi:
 
 ```console
-bazel build --config=my_cross_compilation_stack //my/target
+pi@raspi:~/my_bazel_dir$ raspunzel run //my/target -- --foo --bar
 ```
 
-Then, sync the repository to the robot host:
+Raspunzel's syntax is the same as Bazel, but it only supports the ``run`` command.
 
-```console
-raspunzel sync my_robot_host:some/path
-```
+## Installation
 
-Finally, go to ``some/path`` on the robot host and run your target using the regular Bazel syntax:
+### PyPI
 
 ```console
-raspunzel run //my/target -- --foo --bar
+$ pip install raspunzel
 ```
 
-## Tips
+### Standalone script
 
-* If you have a 64-bit Raspberry Pi cross-compilation stack configured in ``.bazelrc``, name it ``"pi64"`` and use ``raspunzel build``, which is shorthand for ``bazel build --config=pi64``.
+Raspunzel is easy to ship in your own project as a [standalone script](https://github.com/tasts-robots/raspunzel/tree/main/standalone). Check out how it is done for instance in [upkie\_locomotion](https://github.com/tasts-robots/upkie_locomotion).
```

