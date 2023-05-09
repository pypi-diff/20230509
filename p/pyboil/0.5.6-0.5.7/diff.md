# Comparing `tmp/pyboil-0.5.6.tar.gz` & `tmp/pyboil-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyboil-0.5.6.tar", last modified: Tue May  9 16:51:06 2023, max compression
+gzip compressed data, was "pyboil-0.5.7.tar", last modified: Tue May  9 16:56:28 2023, max compression
```

## Comparing `pyboil-0.5.6.tar` & `pyboil-0.5.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:51:06.743786 pyboil-0.5.6/
--rw-r--r--   0 reed      (1000) reed      (1000)    35149 2023-05-09 15:34:10.000000 pyboil-0.5.6/LICENSE
--rw-r--r--   0 reed      (1000) reed      (1000)      338 2023-05-09 16:51:06.743786 pyboil-0.5.6/PKG-INFO
--rw-r--r--   0 reed      (1000) reed      (1000)       58 2023-05-09 16:24:15.000000 pyboil-0.5.6/README.md
-drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:51:06.743786 pyboil-0.5.6/pyboil/
--rw-r--r--   0 reed      (1000) reed      (1000)        0 2023-05-09 15:38:29.000000 pyboil-0.5.6/pyboil/__init__.py
--rw-r--r--   0 reed      (1000) reed      (1000)     1089 2023-05-09 16:24:39.000000 pyboil-0.5.6/pyboil/parser.py
--rw-r--r--   0 reed      (1000) reed      (1000)      571 2023-05-09 16:48:05.000000 pyboil-0.5.6/pyboil/pyboil.py
-drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:51:06.743786 pyboil-0.5.6/pyboil.egg-info/
--rw-r--r--   0 reed      (1000) reed      (1000)      338 2023-05-09 16:51:06.000000 pyboil-0.5.6/pyboil.egg-info/PKG-INFO
--rw-r--r--   0 reed      (1000) reed      (1000)      247 2023-05-09 16:51:06.000000 pyboil-0.5.6/pyboil.egg-info/SOURCES.txt
--rw-r--r--   0 reed      (1000) reed      (1000)        1 2023-05-09 16:51:06.000000 pyboil-0.5.6/pyboil.egg-info/dependency_links.txt
--rw-r--r--   0 reed      (1000) reed      (1000)       48 2023-05-09 16:51:06.000000 pyboil-0.5.6/pyboil.egg-info/entry_points.txt
--rw-r--r--   0 reed      (1000) reed      (1000)        7 2023-05-09 16:51:06.000000 pyboil-0.5.6/pyboil.egg-info/top_level.txt
--rw-r--r--   0 reed      (1000) reed      (1000)       80 2023-05-09 15:35:33.000000 pyboil-0.5.6/pyproject.toml
--rw-r--r--   0 reed      (1000) reed      (1000)       38 2023-05-09 16:51:06.743786 pyboil-0.5.6/setup.cfg
--rw-r--r--   0 reed      (1000) reed      (1000)      865 2023-05-09 16:50:56.000000 pyboil-0.5.6/setup.py
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:56:28.443786 pyboil-0.5.7/
+-rw-r--r--   0 reed      (1000) reed      (1000)    35149 2023-05-09 15:34:10.000000 pyboil-0.5.7/LICENSE
+-rw-r--r--   0 reed      (1000) reed      (1000)      338 2023-05-09 16:56:28.443786 pyboil-0.5.7/PKG-INFO
+-rw-r--r--   0 reed      (1000) reed      (1000)       58 2023-05-09 16:24:15.000000 pyboil-0.5.7/README.md
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:56:28.433786 pyboil-0.5.7/pyboil/
+-rw-r--r--   0 reed      (1000) reed      (1000)        0 2023-05-09 15:38:29.000000 pyboil-0.5.7/pyboil/__init__.py
+-rw-r--r--   0 reed      (1000) reed      (1000)     1089 2023-05-09 16:24:39.000000 pyboil-0.5.7/pyboil/parser.py
+-rw-r--r--   0 reed      (1000) reed      (1000)      667 2023-05-09 16:55:54.000000 pyboil-0.5.7/pyboil/pyboil.py
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:56:28.443786 pyboil-0.5.7/pyboil.egg-info/
+-rw-r--r--   0 reed      (1000) reed      (1000)      338 2023-05-09 16:56:28.000000 pyboil-0.5.7/pyboil.egg-info/PKG-INFO
+-rw-r--r--   0 reed      (1000) reed      (1000)      247 2023-05-09 16:56:28.000000 pyboil-0.5.7/pyboil.egg-info/SOURCES.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)        1 2023-05-09 16:56:28.000000 pyboil-0.5.7/pyboil.egg-info/dependency_links.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)       48 2023-05-09 16:56:28.000000 pyboil-0.5.7/pyboil.egg-info/entry_points.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)        7 2023-05-09 16:56:28.000000 pyboil-0.5.7/pyboil.egg-info/top_level.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)       80 2023-05-09 15:35:33.000000 pyboil-0.5.7/pyproject.toml
+-rw-r--r--   0 reed      (1000) reed      (1000)       38 2023-05-09 16:56:28.443786 pyboil-0.5.7/setup.cfg
+-rw-r--r--   0 reed      (1000) reed      (1000)      865 2023-05-09 16:55:58.000000 pyboil-0.5.7/setup.py
```

### Comparing `pyboil-0.5.6/LICENSE` & `pyboil-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyboil-0.5.6/pyboil/parser.py` & `pyboil-0.5.7/pyboil/parser.py`

 * *Files identical despite different names*

### Comparing `pyboil-0.5.6/pyboil/pyboil.py` & `pyboil-0.5.7/pyboil/pyboil.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from pyboil.parser import parser
-import shutil
+import shutil, os, sys
 
 def launch():
     args = parser.parse_args()
 
-    shutil.copytree("template", '.')
+    current_dir = os.path.pardir(__file__)
+    final_path = (current_dir / "template")
+    shutil.copytree(final_path, '.')
 
     with open('./setup.py') as f:
         setup = f.read()
 
     setup.replace('{NAME}', args['NAME'])
     setup.replace('{VERSION}', args['VERSION'])
     setup.replace('{DESCRIPTION}', args['DESCRIPTION'])
```

### Comparing `pyboil-0.5.6/setup.py` & `pyboil-0.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_dir = Path(__file__).parent
 long_description = (this_dir / "README.md").read_text()
 
 setup_info = dict(
     name='pyboil',
     python_requires=">=3.10",
-    version='0.5.6',
+    version='0.5.7',
     description='CLI script to initialize python packages',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Reed Schick",
     author_email='rns350@nyu.edu',
     url='https://github.com/rns350/pyinit',
     packages=find_packages(
```

