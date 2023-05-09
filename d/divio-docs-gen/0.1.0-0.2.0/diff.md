# Comparing `tmp/divio_docs_gen-0.1.0.tar.gz` & `tmp/divio_docs_gen-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "divio_docs_gen-0.1.0.tar", last modified: Thu May  4 13:13:11 2023, max compression
+gzip compressed data, was "divio_docs_gen-0.2.0.tar", last modified: Tue May  9 06:34:28 2023, max compression
```

## Comparing `divio_docs_gen-0.1.0.tar` & `divio_docs_gen-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 13:13:11.668909 divio_docs_gen-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6045 2023-05-04 13:13:11.664909 divio_docs_gen-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5251 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)      907 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 13:13:11.668909 divio_docs_gen-0.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 13:13:11.664909 divio_docs_gen-0.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 13:13:11.664909 divio_docs_gen-0.1.0/src/divio_docs_gen/
--rw-r--r--   0 root         (0) root         (0)     7564 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/Args.py
--rw-r--r--   0 root         (0) root         (0)     3892 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/DivioDocsEntry.py
--rw-r--r--   0 root         (0) root         (0)     2951 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/Repo.py
--rw-r--r--   0 root         (0) root         (0)     5417 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/Section.py
--rw-r--r--   0 root         (0) root         (0)      191 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/__init__.py
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/index.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 13:13:11.664909 divio_docs_gen-0.1.0/src/divio_docs_gen/write_to_disk/
--rw-r--r--   0 root         (0) root         (0)     1732 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/write_to_disk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3312 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/write_to_disk/nav.py
--rw-r--r--   0 root         (0) root         (0)      611 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/write_to_disk/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 13:13:11.664909 divio_docs_gen-0.1.0/src/divio_docs_gen.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6045 2023-05-04 13:13:11.000000 divio_docs_gen-0.1.0/src/divio_docs_gen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      583 2023-05-04 13:13:11.000000 divio_docs_gen-0.1.0/src/divio_docs_gen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 13:13:11.000000 divio_docs_gen-0.1.0/src/divio_docs_gen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-04 13:13:11.000000 divio_docs_gen-0.1.0/src/divio_docs_gen.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-04 13:13:11.000000 divio_docs_gen-0.1.0/src/divio_docs_gen.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:34:28.737783 divio_docs_gen-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6045 2023-05-09 06:34:28.737783 divio_docs_gen-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5251 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      907 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 06:34:28.737783 divio_docs_gen-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:34:28.733783 divio_docs_gen-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:34:28.737783 divio_docs_gen-0.2.0/src/divio_docs_gen/
+-rw-r--r--   0 root         (0) root         (0)     7676 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/Args.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:34:28.737783 divio_docs_gen-0.2.0/src/divio_docs_gen/Repo/
+-rw-r--r--   0 root         (0) root         (0)     3135 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/Repo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1754 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/Repo/files.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/Repo/sections.py
+-rw-r--r--   0 root         (0) root         (0)     5417 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/Section.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/index.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/markdown_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:34:28.737783 divio_docs_gen-0.2.0/src/divio_docs_gen/write_to_disk/
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/write_to_disk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/write_to_disk/nav.py
+-rw-r--r--   0 root         (0) root         (0)      611 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/write_to_disk/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:34:28.737783 divio_docs_gen-0.2.0/src/divio_docs_gen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6045 2023-05-09 06:34:28.000000 divio_docs_gen-0.2.0/src/divio_docs_gen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      662 2023-05-09 06:34:28.000000 divio_docs_gen-0.2.0/src/divio_docs_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 06:34:28.000000 divio_docs_gen-0.2.0/src/divio_docs_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-09 06:34:28.000000 divio_docs_gen-0.2.0/src/divio_docs_gen.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-09 06:34:28.000000 divio_docs_gen-0.2.0/src/divio_docs_gen.egg-info/top_level.txt
```

### Comparing `divio_docs_gen-0.1.0/LICENSE` & `divio_docs_gen-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.1.0/PKG-INFO` & `divio_docs_gen-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: divio_docs_gen
-Version: 0.1.0
+Version: 0.2.0
 Summary: Turn all the markdown files in your repos into one big, divio structrured documentation
 Author-email: Denperidge <denperidge@gmail.com>
 Project-URL: Homepage, https://github.com/Denperidge-Redpencil/divio-docs-gen
 Project-URL: Bug Tracker, https://github.com/Denperidge-Redpencil/divio-docs-gen/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
```

### Comparing `divio_docs_gen-0.1.0/README.md` & `divio_docs_gen-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.1.0/pyproject.toml` & `divio_docs_gen-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "divio_docs_gen"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     { name="Denperidge", email="denperidge@gmail.com" },
 ]
 description = "Turn all the markdown files in your repos into one big, divio structrured documentation"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `divio_docs_gen-0.1.0/src/divio_docs_gen/Args.py` & `divio_docs_gen-0.2.0/src/divio_docs_gen/Args.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Native imports
 from configparser import ConfigParser
 from os import getcwd, path
 from argparse import ArgumentParser
 
-from .Repo import Repo
-
 """Code to handle configuration, through docs.conf or args"""
 
 section_keys = ["tutorials", "howtos", "explanations", "references"]
 class Args:
     def __init__(self) -> None:
         # store_true default is False, which means save_conf's output will be too verbose. Use None instead
         self.save_conf = None  
@@ -168,42 +166,44 @@
         args.explanations = value
     elif i == 3:
         args.references = value
 
 
 if get_cli_arg_value("repos"):
     for repo_arg in get_cli_arg_value("repos"):
-        repo = Repo(repo_arg[0])
+        repo_config = dict()
+        repo_config.url = repo_arg[0]
         for arg in repo_arg[1:]:
             key, value = arg.split("=", 1)
             key = key.lower()
             if "ignore" in key:
-                repo.files_to_ignore += value.split("//")
+                repo_config["files_to_ignore"] = value.split("//")
             elif "move" in key:
-                repo.files_to_move += value.split("//") 
+                repo_config["files_to_move"] = value.split("//") 
 
-        args.repos.append(repo)
-        conf[repo["url"]] = repo
+        args.repos.append(repo_config)
+        conf[repo_config["url"]] = repo_config
     
 if use_conf:
     all_conf_sections = conf.sections()
     for conf_section_id in all_conf_sections:
         if conf_section_id in conf_sections.values(): continue
 
         conf_section = conf[conf_section_id]
-        repo_data = dict(conf_section)
-        repo = Repo(repo_data["url"])
+        raw_data = dict(conf_section)
+        repo_config = dict()
+        repo_config["url"] = raw_data["url"]
         
-        if "ignore" in repo_data:
-            repo.files_to_ignore += repo_data["ignore"].split("//")
-        if "move" in repo_data:
-            repo.files_to_move += repo_data["move"].split("//")
+        if "ignore" in raw_data:
+            repo_config["files_to_ignore"] = raw_data["ignore"].split("//")
+        if "move" in raw_data:
+            repo_config["files_to_move"] = raw_data["move"].split("//")
 
-        if repo not in args.repos:
-            args.repos.append(repo)
+        if repo_config not in args.repos:
+            args.repos.append(repo_config)
         
 
 if args.save_conf:
     with open("docs.conf", mode="w", encoding="UTF-8") as configfile:
         conf.write(configfile)
 
 print(args)
```

### Comparing `divio_docs_gen-0.1.0/src/divio_docs_gen/Section.py` & `divio_docs_gen-0.2.0/src/divio_docs_gen/Section.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.1.0/src/divio_docs_gen/index.py` & `divio_docs_gen-0.2.0/src/divio_docs_gen/index.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,51 @@
 # Native imports
 from typing import List
 # Local imports
 from .Repo import Repo
-from .DivioDocsEntry import _get_repo_docs
 from .write_to_disk import clear_docs, generate_nav_as_needed
 from .Args import args
 
 """Entrypoint for the application"""
 
 def _docs_from_configured_repos():
-    """Generate docs from configured repos"""
+    """Generate docs from repos configured in Args"""
     for repoconfig in args.repos:
-         _get_repo_docs(repoconfig, write_to_disk=args.write_to_disk)
+         files_to_move = repoconfig["files_to_move"] if "files_to_move" in repoconfig else []
+         files_to_ignore = repoconfig["files_to_ignore"] if "files_to_ignore" in repoconfig else []
+         Repo(repoconfig["url"], parse_docs_on_init=True, write_to_disk_on_init=args.write_to_disk, files_to_move=files_to_move, files_to_ignore=files_to_ignore)
     
     generate_nav_as_needed()
 
 
-def docs_from_repo(git_url: str, write_to_disk=args.write_to_disk):
-    """Generate documentation from the passed git url. This function does NOT automatically create nav files; make sure to run generate_nav_if_needed if desired"""
-    repo = Repo(git_url)
-    return _get_repo_docs(repo, write_to_disk=write_to_disk)
+def docs_from_repo(git_url: str) -> Repo:
+    """
+    Generate documentation from the passed git url, optionally writing to disk.
 
+    Returns a Repo object
+    
+    NOTE: This function does NOT automatically create nav files; make sure to run generate_nav_if_needed if desired
+    """
+    repo = Repo(git_url, parse_docs_on_init=True)
+    return repo
+
+
+def docs_from_repos(git_urls: List[str], write_to_disk=args.write_to_disk) -> List[Repo]:
+    """
+    Generate documentation from passed git urls, optionally writing to disk.
+    Iterative wrapper for docs_from_repo
 
-def docs_from_repos(git_urls: List[str]):
-    """Generate documentation from passed git urls. This function DOES automatically create nav files, if enabled in docs.conf or the passed args"""
+    Returns a Repo object
+    
+    NOTE: This function DOES automatically create nav files, if enabled in docs.conf or the passed args
+    """
+    repos = []
     for url in git_urls:
-        docs_from_repo(url)
+        repos.append(docs_from_repo(url, write_to_disk))
+
     generate_nav_as_needed()
     
 def main():
     """When this package is run directly, clear any existing docs and generate new ones based on args"""
     clear_docs()
     _docs_from_configured_repos()
```

### Comparing `divio_docs_gen-0.1.0/src/divio_docs_gen/write_to_disk/__init__.py` & `divio_docs_gen-0.2.0/src/divio_docs_gen/write_to_disk/__init__.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.1.0/src/divio_docs_gen/write_to_disk/nav.py` & `divio_docs_gen-0.2.0/src/divio_docs_gen/write_to_disk/nav.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.1.0/src/divio_docs_gen/write_to_disk/utils.py` & `divio_docs_gen-0.2.0/src/divio_docs_gen/write_to_disk/utils.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.1.0/src/divio_docs_gen.egg-info/PKG-INFO` & `divio_docs_gen-0.2.0/src/divio_docs_gen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: divio-docs-gen
-Version: 0.1.0
+Version: 0.2.0
 Summary: Turn all the markdown files in your repos into one big, divio structrured documentation
 Author-email: Denperidge <denperidge@gmail.com>
 Project-URL: Homepage, https://github.com/Denperidge-Redpencil/divio-docs-gen
 Project-URL: Bug Tracker, https://github.com/Denperidge-Redpencil/divio-docs-gen/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
```

### Comparing `divio_docs_gen-0.1.0/src/divio_docs_gen.egg-info/SOURCES.txt` & `divio_docs_gen-0.2.0/src/divio_docs_gen.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
 src/divio_docs_gen/Args.py
-src/divio_docs_gen/DivioDocsEntry.py
-src/divio_docs_gen/Repo.py
 src/divio_docs_gen/Section.py
 src/divio_docs_gen/__init__.py
 src/divio_docs_gen/__main__.py
 src/divio_docs_gen/index.py
+src/divio_docs_gen/markdown_parser.py
 src/divio_docs_gen.egg-info/PKG-INFO
 src/divio_docs_gen.egg-info/SOURCES.txt
 src/divio_docs_gen.egg-info/dependency_links.txt
 src/divio_docs_gen.egg-info/entry_points.txt
 src/divio_docs_gen.egg-info/top_level.txt
+src/divio_docs_gen/Repo/__init__.py
+src/divio_docs_gen/Repo/files.py
+src/divio_docs_gen/Repo/sections.py
 src/divio_docs_gen/write_to_disk/__init__.py
 src/divio_docs_gen/write_to_disk/nav.py
 src/divio_docs_gen/write_to_disk/utils.py
```

