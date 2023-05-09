# Comparing `tmp/carchive-0.0.57.tar.gz` & `tmp/carchive-0.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carchive-0.0.57.tar", last modified: Tue May  9 02:57:15 2023, max compression
+gzip compressed data, was "carchive-0.0.58.tar", last modified: Tue May  9 03:16:52 2023, max compression
```

## Comparing `carchive-0.0.57.tar` & `carchive-0.0.58.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:57:15.199807 carchive-0.0.57/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-09 02:57:10.000000 carchive-0.0.57/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-09 02:57:15.199807 carchive-0.0.57/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 02:57:10.000000 carchive-0.0.57/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:57:15.199807 carchive-0.0.57/carchive/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10242 2023-05-09 02:57:10.000000 carchive-0.0.57/carchive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:57:15.199807 carchive-0.0.57/carchive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-09 02:57:15.000000 carchive-0.0.57/carchive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-09 02:57:15.000000 carchive-0.0.57/carchive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 02:57:15.000000 carchive-0.0.57/carchive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-09 02:57:15.000000 carchive-0.0.57/carchive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 02:57:15.000000 carchive-0.0.57/carchive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 02:57:15.199807 carchive-0.0.57/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-05-09 02:57:10.000000 carchive-0.0.57/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:16:52.044066 carchive-0.0.58/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-09 03:16:45.000000 carchive-0.0.58/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-09 03:16:52.044066 carchive-0.0.58/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 03:16:45.000000 carchive-0.0.58/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:16:52.040065 carchive-0.0.58/carchive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10290 2023-05-09 03:16:45.000000 carchive-0.0.58/carchive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 03:16:52.044066 carchive-0.0.58/carchive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-09 03:16:52.000000 carchive-0.0.58/carchive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-09 03:16:52.000000 carchive-0.0.58/carchive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 03:16:52.000000 carchive-0.0.58/carchive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-09 03:16:52.000000 carchive-0.0.58/carchive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 03:16:52.000000 carchive-0.0.58/carchive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 03:16:52.044066 carchive-0.0.58/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-05-09 03:16:45.000000 carchive-0.0.58/setup.py
```

### Comparing `carchive-0.0.57/LICENSE` & `carchive-0.0.58/LICENSE`

 * *Files identical despite different names*

### Comparing `carchive-0.0.57/carchive/__init__.py` & `carchive-0.0.58/carchive/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, requests, datetime, time, queue, threading
+import os, requests, datetime, time, queue, threading, asyncio
 from copy import deepcopy as dc
 from threading import Lock
 from typing import Dict, List, Callable, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 import mystring,splittr
 import pause
@@ -215,14 +215,15 @@
 
 		def appr(string: mystring.string):
 			with open("mapping_file_{0}.csv".format(string.tobase64()), "a+") as writer:
 				writer.write(string)
 		self.appr = appr
 		self.api_watch = niceghapi()
 		self.delete_paths = delete_paths
+		asyncio.run(self.handle_git())
 	
 	@property
 	def timing(self):
 		self.api_watch.timing
 
 		extra_rate_limiting = self.g.get_rate_limit()
 		if hasattr(extra_rate_limiting, "search"):
@@ -239,15 +240,15 @@
 
 	def __call__(self, search_string:str):
 		self.timing
 		search_string = mystring.string(search_string)
 
 		def process_prep(repo_itr:int, repo:Repository, search_string:str, appr:Callable, fin_queue:queue.Queue):
 			def process():
-				name = mystring.string("ITR:{0}_URL:{1}_STR:{2}\n".format(
+				name = mystring.string("ITR>{0}_URL>{1}_STR>{2}\n".format(
 					repo_itr, repo.url, search_string
 				))
 				repo_dir = "repo_" + str(name.tobase64())
 				results_dir = "results_" + str(name.tobase64())
 
 				self.repair(repo_dir, create=False)
 				self.repair(results_dir)
@@ -294,15 +295,15 @@
 		except:
 			pass
 
 	@property
 	def complete(self):
 		return self.total_repo_len == self.current_repo_itr and self.processor.complete
 
-	def handle_git(self):
+	async def handle_git(self):
 		while not self.complete:
 			# Get up to 5 strings from the queue
 			paths,num_waiting = [], 5
 			while len(paths) < num_waiting:
 				try:
 					path = self.processed_paths.get()
 					paths.append(path)
```

### Comparing `carchive-0.0.57/setup.py` & `carchive-0.0.58/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.57"
+VERSION = "0.0.58"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

