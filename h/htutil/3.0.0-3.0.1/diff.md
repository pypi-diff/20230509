# Comparing `tmp/htutil-3.0.0.tar.gz` & `tmp/htutil-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/htutil/htutil/dist/.tmp-wctbzqvj/htutil-3.0.0.tar", last modified: Fri Apr 14 02:07:07 2023, max compression
+gzip compressed data, was "/home/runner/work/htutil/htutil/dist/.tmp-viilr2b8/htutil-3.0.1.tar", last modified: Tue May  9 07:16:38 2023, max compression
```

## Comparing `htutil-3.0.0.tar` & `htutil-3.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 02:07:07.000000 htutil-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-04-14 02:06:57.000000 htutil-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-14 02:07:07.000000 htutil-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-14 02:06:57.000000 htutil-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 02:07:07.000000 htutil-3.0.0/htutil/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 02:06:57.000000 htutil-3.0.0/htutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-14 02:06:57.000000 htutil-3.0.0/htutil/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-14 02:06:57.000000 htutil-3.0.0/htutil/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-14 02:06:57.000000 htutil-3.0.0/htutil/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 02:07:07.000000 htutil-3.0.0/htutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-14 02:07:07.000000 htutil-3.0.0/htutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-14 02:07:07.000000 htutil-3.0.0/htutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 02:07:07.000000 htutil-3.0.0/htutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 02:07:07.000000 htutil-3.0.0/htutil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 02:07:07.000000 htutil-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-14 02:06:57.000000 htutil-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:16:38.000000 htutil-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-09 07:16:26.000000 htutil-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-09 07:16:38.000000 htutil-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-09 07:16:26.000000 htutil-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:16:38.000000 htutil-3.0.1/htutil/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:16:26.000000 htutil-3.0.1/htutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-09 07:16:26.000000 htutil-3.0.1/htutil/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-09 07:16:26.000000 htutil-3.0.1/htutil/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-09 07:16:26.000000 htutil-3.0.1/htutil/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:16:38.000000 htutil-3.0.1/htutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-09 07:16:38.000000 htutil-3.0.1/htutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-09 07:16:38.000000 htutil-3.0.1/htutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:16:38.000000 htutil-3.0.1/htutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 07:16:38.000000 htutil-3.0.1/htutil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 07:16:38.000000 htutil-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-09 07:16:26.000000 htutil-3.0.1/setup.py
```

### Comparing `htutil-3.0.0/LICENSE` & `htutil-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `htutil-3.0.0/PKG-INFO` & `htutil-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htutil
-Version: 3.0.0
+Version: 3.0.1
 Summary: HaoTian's Python Util
 Home-page: https://github.com/117503445/htutil
 Author: 117503445
 Author-email: t117503445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `htutil-3.0.0/README.md` & `htutil-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `htutil-3.0.0/htutil/cache.py` & `htutil-3.0.1/htutil/cache.py`

 * *Files identical despite different names*

### Comparing `htutil-3.0.0/htutil/file.py` & `htutil-3.0.1/htutil/file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,106 +1,107 @@
 import os
 import pickle as pkl
+from pathlib import Path
 import json
 
 
-def read_text(path: str) -> str:
+def read_text(path: str| Path) -> str:
     with open(path, 'r', encoding='utf-8', errors='ignore') as f:
         lines = f.readlines()
         text = ''.join(lines)
         return text
 
 
-def read_lines(path: str) -> list[str]:
+def read_lines(path: str| Path) -> list[str]:
     with open(path, 'r', encoding='utf-8', errors='ignore') as f:
         lines = f.readlines()
         for i in range(len(lines)):
             lines[i] = lines[i].replace('\n', '')
             lines[i] = lines[i].replace('\r', '')
         return lines
 
 
-def write_text(path: str, content: str) -> None:
+def write_text(path: str| Path, content: str) -> None:
     content = str(content)
     create_dir_if_not_exist(os.path.dirname(path))
     with open(path, 'w', encoding='utf-8', errors='ignore') as f:
         f.write(content)
 
 
-def write_lines(path: str, content: list) -> None:
+def write_lines(path: str| Path, content: list) -> None:
     if not isinstance(content, list):
         raise TypeError('content is not list')
     create_dir_if_not_exist(os.path.dirname(path))
     text = '\n'.join(content)
     with open(path, 'w', encoding='utf-8', errors='ignore') as f:
         f.write(text)
 
 
-def append_text(path: str, content: str, newline=True) -> None:
+def append_text(path: str| Path, content: str, newline=True) -> None:
     if not os.path.exists(path):
         write_text(path, '')
     content = str(content)
     if newline:
         content += '\n'
     with open(path, 'a', encoding='utf-8', errors='ignore') as f:
         f.write(content)
 
 
-def append_lines(path: str, content: list) -> None:
+def append_lines(path: str| Path, content: list) -> None:
     if not isinstance(content, list):
         raise TypeError('content is not list')
     if not os.path.exists(path):
         write_text(path, '')
     with open(path, 'a', encoding='utf-8', errors='ignore') as f:
         text = '\n'.join(content)
         f.write(text)
 
 
-def create_dir_if_not_exist(path: str) -> None:
+def create_dir_if_not_exist(path: str| Path) -> None:
     if path == '':
         return
     if not os.path.exists(path):
         os.makedirs(path)
 
 
-def read_csv(path: str) -> None:
+def read_csv(path: str| Path) -> list[list[str]]:
     lines = read_lines(path)
-    rows = []
+    rows:list[list[str]] = []
     for line in lines:
         rows.append(line.split(','))
     return rows
 
 
-def write_csv(path: str, rows: list) -> None:
+def write_csv(path: str| Path, rows: list) -> None:
     lines = []
     for row in rows:
         for i in range(len(row)):
             row[i] = str(row[i])
         line = ','.join(row)
         lines.append(line)
     write_lines(path, lines)
 
 
-def write_pkl(path: str, content) -> None:
+def write_pkl(path: str| Path, content) -> None:
     create_dir_if_not_exist(os.path.dirname(path))
     with open(path, 'wb') as f:
         pkl.dump(content, f)
 
 
-def read_pkl(path: str):
+def read_pkl(path: str| Path):
     with open(path, 'rb') as f:
         result = pkl.load(f)
     return result
 
 
-def write_json(path: str, content, indent=4) -> None:
+def write_json(path: str| Path, content, indent=4) -> None:
     write_text(path, json.dumps(content, indent=indent, ensure_ascii=False))
 
 
-def read_json(path: str):
+def read_json(path: str| Path):
     return json.loads(read_text(path))
 
 
 def main():
     s = 'hello'
     write_text('1.txt', s)
     # hello in 1.txt
```

### Comparing `htutil-3.0.0/htutil.egg-info/PKG-INFO` & `htutil-3.0.1/htutil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htutil
-Version: 3.0.0
+Version: 3.0.1
 Summary: HaoTian's Python Util
 Home-page: https://github.com/117503445/htutil
 Author: 117503445
 Author-email: t117503445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `htutil-3.0.0/setup.py` & `htutil-3.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="htutil",
-    version="3.0.0",
+    version="3.0.1",
     author="117503445",
     author_email="t117503445@gmail.com",
     description="HaoTian's Python Util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/117503445/htutil",
     packages=setuptools.find_packages(),
```

