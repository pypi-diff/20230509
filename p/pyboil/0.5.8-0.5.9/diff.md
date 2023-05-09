# Comparing `tmp/pyboil-0.5.8.tar.gz` & `tmp/pyboil-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyboil-0.5.8.tar", last modified: Tue May  9 16:59:12 2023, max compression
+gzip compressed data, was "pyboil-0.5.9.tar", last modified: Tue May  9 17:01:02 2023, max compression
```

## Comparing `pyboil-0.5.8.tar` & `pyboil-0.5.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:59:12.043786 pyboil-0.5.8/
--rw-r--r--   0 reed      (1000) reed      (1000)    35149 2023-05-09 15:34:10.000000 pyboil-0.5.8/LICENSE
--rw-r--r--   0 reed      (1000) reed      (1000)      338 2023-05-09 16:59:12.043786 pyboil-0.5.8/PKG-INFO
--rw-r--r--   0 reed      (1000) reed      (1000)       58 2023-05-09 16:24:15.000000 pyboil-0.5.8/README.md
-drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:59:12.043786 pyboil-0.5.8/pyboil/
--rw-r--r--   0 reed      (1000) reed      (1000)        0 2023-05-09 15:38:29.000000 pyboil-0.5.8/pyboil/__init__.py
--rw-r--r--   0 reed      (1000) reed      (1000)     1089 2023-05-09 16:24:39.000000 pyboil-0.5.8/pyboil/parser.py
--rw-r--r--   0 reed      (1000) reed      (1000)      622 2023-05-09 16:57:58.000000 pyboil-0.5.8/pyboil/pyboil.py
-drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:59:12.043786 pyboil-0.5.8/pyboil.egg-info/
--rw-r--r--   0 reed      (1000) reed      (1000)      338 2023-05-09 16:59:12.000000 pyboil-0.5.8/pyboil.egg-info/PKG-INFO
--rw-r--r--   0 reed      (1000) reed      (1000)      247 2023-05-09 16:59:12.000000 pyboil-0.5.8/pyboil.egg-info/SOURCES.txt
--rw-r--r--   0 reed      (1000) reed      (1000)        1 2023-05-09 16:59:12.000000 pyboil-0.5.8/pyboil.egg-info/dependency_links.txt
--rw-r--r--   0 reed      (1000) reed      (1000)       48 2023-05-09 16:59:12.000000 pyboil-0.5.8/pyboil.egg-info/entry_points.txt
--rw-r--r--   0 reed      (1000) reed      (1000)        7 2023-05-09 16:59:12.000000 pyboil-0.5.8/pyboil.egg-info/top_level.txt
--rw-r--r--   0 reed      (1000) reed      (1000)       80 2023-05-09 15:35:33.000000 pyboil-0.5.8/pyproject.toml
--rw-r--r--   0 reed      (1000) reed      (1000)       38 2023-05-09 16:59:12.043786 pyboil-0.5.8/setup.cfg
--rw-r--r--   0 reed      (1000) reed      (1000)      865 2023-05-09 16:58:37.000000 pyboil-0.5.8/setup.py
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 17:01:02.643786 pyboil-0.5.9/
+-rw-r--r--   0 reed      (1000) reed      (1000)    35149 2023-05-09 15:34:10.000000 pyboil-0.5.9/LICENSE
+-rw-r--r--   0 reed      (1000) reed      (1000)      338 2023-05-09 17:01:02.633786 pyboil-0.5.9/PKG-INFO
+-rw-r--r--   0 reed      (1000) reed      (1000)       58 2023-05-09 16:24:15.000000 pyboil-0.5.9/README.md
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 17:01:02.633786 pyboil-0.5.9/pyboil/
+-rw-r--r--   0 reed      (1000) reed      (1000)        0 2023-05-09 15:38:29.000000 pyboil-0.5.9/pyboil/__init__.py
+-rw-r--r--   0 reed      (1000) reed      (1000)     1089 2023-05-09 16:24:39.000000 pyboil-0.5.9/pyboil/parser.py
+-rw-r--r--   0 reed      (1000) reed      (1000)      621 2023-05-09 17:00:45.000000 pyboil-0.5.9/pyboil/pyboil.py
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 17:01:02.633786 pyboil-0.5.9/pyboil.egg-info/
+-rw-r--r--   0 reed      (1000) reed      (1000)      338 2023-05-09 17:01:02.000000 pyboil-0.5.9/pyboil.egg-info/PKG-INFO
+-rw-r--r--   0 reed      (1000) reed      (1000)      247 2023-05-09 17:01:02.000000 pyboil-0.5.9/pyboil.egg-info/SOURCES.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)        1 2023-05-09 17:01:02.000000 pyboil-0.5.9/pyboil.egg-info/dependency_links.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)       48 2023-05-09 17:01:02.000000 pyboil-0.5.9/pyboil.egg-info/entry_points.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)        7 2023-05-09 17:01:02.000000 pyboil-0.5.9/pyboil.egg-info/top_level.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)       80 2023-05-09 15:35:33.000000 pyboil-0.5.9/pyproject.toml
+-rw-r--r--   0 reed      (1000) reed      (1000)       38 2023-05-09 17:01:02.643786 pyboil-0.5.9/setup.cfg
+-rw-r--r--   0 reed      (1000) reed      (1000)      865 2023-05-09 17:00:52.000000 pyboil-0.5.9/setup.py
```

### Comparing `pyboil-0.5.8/LICENSE` & `pyboil-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyboil-0.5.8/pyboil/parser.py` & `pyboil-0.5.9/pyboil/parser.py`

 * *Files identical despite different names*

### Comparing `pyboil-0.5.8/pyboil/pyboil.py` & `pyboil-0.5.9/pyboil/pyboil.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pyboil.parser import parser
 import shutil, os, sys
 
 def launch():
     args = parser.parse_args()
 
-    final_path = (os.pardir / "template")
+    final_path = f"{os.pardir}/template"
     shutil.copytree(final_path, '.')
 
     with open('./setup.py') as f:
         setup = f.read()
 
     setup.replace('{NAME}', args['NAME'])
     setup.replace('{VERSION}', args['VERSION'])
```

### Comparing `pyboil-0.5.8/setup.py` & `pyboil-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_dir = Path(__file__).parent
 long_description = (this_dir / "README.md").read_text()
 
 setup_info = dict(
     name='pyboil',
     python_requires=">=3.10",
-    version='0.5.8',
+    version='0.5.9',
     description='CLI script to initialize python packages',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Reed Schick",
     author_email='rns350@nyu.edu',
     url='https://github.com/rns350/pyinit',
     packages=find_packages(
```

