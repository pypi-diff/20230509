# Comparing `tmp/sans-0.0.1b7.tar.gz` & `tmp/sans-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sans-0.0.1b7.tar", last modified: Fri Jan  3 20:04:06 2020, max compression
+gzip compressed data, was "sans-1.0.0a1.tar", last modified: Tue May  9 02:57:07 2023, max compression
```

## Comparing `sans-0.0.1b7.tar` & `sans-1.0.0a1.tar`

### file list

```diff
@@ -1,22 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-03 20:04:06.980843 sans-0.0.1b7/
--rw-r--r--   0 runner    (1001) docker     (115)     4520 2020-01-03 20:04:06.980843 sans-0.0.1b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     2751 2020-01-03 20:03:58.000000 sans-0.0.1b7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-03 20:04:06.980843 sans-0.0.1b7/sans/
--rw-r--r--   0 runner    (1001) docker     (115)      188 2020-01-03 20:03:58.000000 sans-0.0.1b7/sans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     2696 2020-01-03 20:03:58.000000 sans-0.0.1b7/sans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (115)     1869 2020-01-03 20:03:58.000000 sans-0.0.1b7/sans/_lock.py
--rw-r--r--   0 runner    (1001) docker     (115)    19133 2020-01-03 20:03:58.000000 sans-0.0.1b7/sans/api.py
--rw-r--r--   0 runner    (1001) docker     (115)     2463 2020-01-03 20:03:58.000000 sans-0.0.1b7/sans/errors.py
--rw-r--r--   0 runner    (1001) docker     (115)      345 2020-01-03 20:03:58.000000 sans-0.0.1b7/sans/info.py
--rw-r--r--   0 runner    (1001) docker     (115)     4305 2020-01-03 20:03:58.000000 sans-0.0.1b7/sans/objects.py
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-01-03 20:03:58.000000 sans-0.0.1b7/sans/server.py
--rw-r--r--   0 runner    (1001) docker     (115)     1582 2020-01-03 20:03:58.000000 sans-0.0.1b7/sans/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-03 20:04:06.980843 sans-0.0.1b7/sans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)     4520 2020-01-03 20:04:06.000000 sans-0.0.1b7/sans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)      332 2020-01-03 20:04:06.000000 sans-0.0.1b7/sans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-01-03 20:04:06.000000 sans-0.0.1b7/sans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)       45 2020-01-03 20:04:06.000000 sans-0.0.1b7/sans.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (115)       57 2020-01-03 20:04:06.000000 sans-0.0.1b7/sans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)        5 2020-01-03 20:04:06.000000 sans-0.0.1b7/sans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (115)     1026 2020-01-03 20:04:06.980843 sans-0.0.1b7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)       70 2020-01-03 20:03:58.000000 sans-0.0.1b7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:57:07.457871 sans-1.0.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:57:07.453871 sans-1.0.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:57:07.453871 sans-1.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-09 02:56:56.000000 sans-1.0.0a1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-09 02:56:56.000000 sans-1.0.0a1/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-09 02:56:56.000000 sans-1.0.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-09 02:56:56.000000 sans-1.0.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-09 02:56:56.000000 sans-1.0.0a1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-09 02:56:56.000000 sans-1.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-09 02:56:56.000000 sans-1.0.0a1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-09 02:57:07.457871 sans-1.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-09 02:56:56.000000 sans-1.0.0a1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:57:07.453871 sans-1.0.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-09 02:56:56.000000 sans-1.0.0a1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-09 02:56:56.000000 sans-1.0.0a1/docs/__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-09 02:56:56.000000 sans-1.0.0a1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-05-09 02:56:56.000000 sans-1.0.0a1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 02:56:56.000000 sans-1.0.0a1/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-09 02:56:56.000000 sans-1.0.0a1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-09 02:56:56.000000 sans-1.0.0a1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-09 02:56:56.000000 sans-1.0.0a1/docs/objects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-09 02:56:56.000000 sans-1.0.0a1/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-09 02:56:56.000000 sans-1.0.0a1/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-09 02:56:56.000000 sans-1.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-09 02:56:56.000000 sans-1.0.0a1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:57:07.457871 sans-1.0.0a1/sans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23022 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:57:07.457871 sans-1.0.0a1/sans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-09 02:57:07.000000 sans-1.0.0a1/sans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-09 02:57:07.000000 sans-1.0.0a1/sans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 02:57:07.000000 sans-1.0.0a1/sans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-09 02:57:07.000000 sans-1.0.0a1/sans.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-09 02:57:07.000000 sans-1.0.0a1/sans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 02:57:07.000000 sans-1.0.0a1/sans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 02:57:07.457871 sans-1.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-09 02:56:56.000000 sans-1.0.0a1/setup.py
```

### Comparing `sans-0.0.1b7/README.rst` & `sans-1.0.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `sans-0.0.1b7/sans/__main__.py` & `sans-1.0.0a1/sans/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,30 @@
+#!/usr/bin/python3
+
+from __future__ import annotations
+
 import argparse
-import logging
 import shlex
 import sys
+import traceback
+from typing import Any
+from xml.etree import ElementTree as etree
 
 import sans
-from sans.api import Api
-from sans.errors import HTTPException
-from sans.utils import pretty_string
 
+try:
+    from rich import print  # type: ignore
+    from rich.syntax import Syntax  # type: ignore
+except ImportError:
 
-logger = logging.getLogger(__name__)
+    def Syntax(arg: Any, *_: Any, **__: Any) -> Any:
+        return arg
 
 
-def main():
+def main() -> None:
     parser = argparse.ArgumentParser(
         allow_abbrev=False,
         description="SANS Console Entry",
         prog="sans",
         epilog="Any unknown args will be used to build the API request.",
     )
     parser.add_argument(
@@ -28,58 +36,68 @@
         action="store_true",
         help="quit the console program loop after this run",
     )
     parser.usage = parser.format_usage() + " ..."
     known, unknown = parser.parse_known_args()
     if not any(vars(known).values()):
         parser.print_help(sys.stderr)
-    sans.run_in_thread()
     if known.quit and not unknown:
-        return print("Okay I'll just leave I guess...", file=sys.stderr)
-    Api.agent = known.agent or input("User agent: ")
-    args = ()
-    while True:
-        print()
-        if not args and unknown:
-            args = (known, unknown)
-        else:
-            args = parser.parse_known_args(shlex.split(input(parser.prog + " ")))
-            if args[0].agent:
-                print(
-                    "You can't change the agent in the middle of the script.",
-                    file=sys.stderr,
-                )
-        known, unknown = args
-        if not unknown:
-            if known.quit:
-                return print("No query provided. Exiting...", file=sys.stderr)
-            print("No query provided.", file=sys.stderr)
-            parser.print_usage(sys.stderr)
-            continue
-        request = {}
-        key = "q"
-        for arg in unknown:
-            if arg.startswith("--"):
-                if key != "q":
-                    print("No value provided for key {!r}".format(key), file=sys.stderr)
-                    continue
-                key = arg[2:]
+        print("Okay, I'll just leave I guess...", file=sys.stderr)
+        return
+    sans.set_agent(known.agent or input("User agent: "))
+    args: tuple[argparse.Namespace, list[str]] | tuple[()] = ()
+    with sans.Client() as client:
+        while True:
+            print()
+            if not args and unknown:
+                args = (known, unknown)
             else:
-                request.setdefault(key, []).append(arg)
-                key = "q"
-        if key != "q":
-            print("No value provided for key {!r}".format(key), file=sys.stderr)
-            continue
-        request = Api(request)
-        try:
-            for element in request.threadsafe:
-                print(pretty_string(element), end="")
-        except HTTPException as e:
-            print(e, file=sys.stderr)
-        except Exception as e:
-            logging.exception(e)
-        if known.quit:
-            return print("Exiting...", file=sys.stderr)
+                args = parser.parse_known_args(shlex.split(input(parser.prog + " ")))
+                if args[0].agent:
+                    print(
+                        "You can't change the agent in the middle of the script.",
+                        file=sys.stderr,
+                    )
+            known, unknown = args
+            if not unknown:
+                if known.quit:
+                    print("No query provided. Exiting...", file=sys.stderr)
+                    return
+                print("No query provided.", file=sys.stderr)
+                parser.print_usage(sys.stderr)
+                continue
+            parameters: dict[str, list[str]] = {}
+            key = "q"
+            for arg in unknown:
+                if arg.startswith("--"):
+                    if key != "q":
+                        print(
+                            "No value provided for key {!r}".format(key),
+                            file=sys.stderr,
+                        )
+                        continue
+                    key = arg[2:]
+                else:
+                    parameters.setdefault(key, []).append(arg)
+                    key = "q"
+            if key != "q":
+                print("No value provided for key {!r}".format(key), file=sys.stderr)
+                continue
+            try:
+                with client.stream("GET", sans.API_URL, params=parameters) as response:
+                    print(response.url, end="\n\n")
+                    for element in response.iter_xml():
+                        pretty_print(element)
+            except Exception:
+                traceback.print_exc()
+            if known.quit:
+                print("Exiting...", file=sys.stderr)
+                return
+
+
+def pretty_print(element: etree.Element) -> None:
+    sans.indent(element)
+    print(Syntax(etree.tostring(element, encoding="unicode").strip(), "xml"))
 
 
 if __name__ == "__main__":
     main()
```

