# Comparing `tmp/pyboil-0.5.5.tar.gz` & `tmp/pyboil-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyboil-0.5.5.tar", last modified: Tue May  9 16:48:37 2023, max compression
+gzip compressed data, was "pyboil-0.5.6.tar", last modified: Tue May  9 16:51:06 2023, max compression
```

## Comparing `pyboil-0.5.5.tar` & `pyboil-0.5.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:48:37.273786 pyboil-0.5.5/
--rw-r--r--   0 reed      (1000) reed      (1000)    35149 2023-05-09 15:34:10.000000 pyboil-0.5.5/LICENSE
--rw-r--r--   0 reed      (1000) reed      (1000)      338 2023-05-09 16:48:37.273786 pyboil-0.5.5/PKG-INFO
--rw-r--r--   0 reed      (1000) reed      (1000)       58 2023-05-09 16:24:15.000000 pyboil-0.5.5/README.md
-drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:48:37.273786 pyboil-0.5.5/pyboil/
--rw-r--r--   0 reed      (1000) reed      (1000)        0 2023-05-09 15:38:29.000000 pyboil-0.5.5/pyboil/__init__.py
--rw-r--r--   0 reed      (1000) reed      (1000)      571 2023-05-09 16:48:05.000000 pyboil-0.5.5/pyboil/main.py
--rw-r--r--   0 reed      (1000) reed      (1000)     1089 2023-05-09 16:24:39.000000 pyboil-0.5.5/pyboil/parser.py
-drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:48:37.273786 pyboil-0.5.5/pyboil.egg-info/
--rw-r--r--   0 reed      (1000) reed      (1000)      338 2023-05-09 16:48:37.000000 pyboil-0.5.5/pyboil.egg-info/PKG-INFO
--rw-r--r--   0 reed      (1000) reed      (1000)      245 2023-05-09 16:48:37.000000 pyboil-0.5.5/pyboil.egg-info/SOURCES.txt
--rw-r--r--   0 reed      (1000) reed      (1000)        1 2023-05-09 16:48:37.000000 pyboil-0.5.5/pyboil.egg-info/dependency_links.txt
--rw-r--r--   0 reed      (1000) reed      (1000)       39 2023-05-09 16:48:37.000000 pyboil-0.5.5/pyboil.egg-info/entry_points.txt
--rw-r--r--   0 reed      (1000) reed      (1000)        7 2023-05-09 16:48:37.000000 pyboil-0.5.5/pyboil.egg-info/top_level.txt
--rw-r--r--   0 reed      (1000) reed      (1000)       80 2023-05-09 15:35:33.000000 pyboil-0.5.5/pyproject.toml
--rw-r--r--   0 reed      (1000) reed      (1000)       38 2023-05-09 16:48:37.273786 pyboil-0.5.5/setup.cfg
--rw-r--r--   0 reed      (1000) reed      (1000)      856 2023-05-09 16:48:17.000000 pyboil-0.5.5/setup.py
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:51:06.743786 pyboil-0.5.6/
+-rw-r--r--   0 reed      (1000) reed      (1000)    35149 2023-05-09 15:34:10.000000 pyboil-0.5.6/LICENSE
+-rw-r--r--   0 reed      (1000) reed      (1000)      338 2023-05-09 16:51:06.743786 pyboil-0.5.6/PKG-INFO
+-rw-r--r--   0 reed      (1000) reed      (1000)       58 2023-05-09 16:24:15.000000 pyboil-0.5.6/README.md
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:51:06.743786 pyboil-0.5.6/pyboil/
+-rw-r--r--   0 reed      (1000) reed      (1000)        0 2023-05-09 15:38:29.000000 pyboil-0.5.6/pyboil/__init__.py
+-rw-r--r--   0 reed      (1000) reed      (1000)     1089 2023-05-09 16:24:39.000000 pyboil-0.5.6/pyboil/parser.py
+-rw-r--r--   0 reed      (1000) reed      (1000)      571 2023-05-09 16:48:05.000000 pyboil-0.5.6/pyboil/pyboil.py
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:51:06.743786 pyboil-0.5.6/pyboil.egg-info/
+-rw-r--r--   0 reed      (1000) reed      (1000)      338 2023-05-09 16:51:06.000000 pyboil-0.5.6/pyboil.egg-info/PKG-INFO
+-rw-r--r--   0 reed      (1000) reed      (1000)      247 2023-05-09 16:51:06.000000 pyboil-0.5.6/pyboil.egg-info/SOURCES.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)        1 2023-05-09 16:51:06.000000 pyboil-0.5.6/pyboil.egg-info/dependency_links.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)       48 2023-05-09 16:51:06.000000 pyboil-0.5.6/pyboil.egg-info/entry_points.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)        7 2023-05-09 16:51:06.000000 pyboil-0.5.6/pyboil.egg-info/top_level.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)       80 2023-05-09 15:35:33.000000 pyboil-0.5.6/pyproject.toml
+-rw-r--r--   0 reed      (1000) reed      (1000)       38 2023-05-09 16:51:06.743786 pyboil-0.5.6/setup.cfg
+-rw-r--r--   0 reed      (1000) reed      (1000)      865 2023-05-09 16:50:56.000000 pyboil-0.5.6/setup.py
```

### Comparing `pyboil-0.5.5/LICENSE` & `pyboil-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyboil-0.5.5/pyboil/main.py` & `pyboil-0.5.6/pyboil/pyboil.py`

 * *Files identical despite different names*

### Comparing `pyboil-0.5.5/pyboil/parser.py` & `pyboil-0.5.6/pyboil/parser.py`

 * *Files identical despite different names*

### Comparing `pyboil-0.5.5/setup.py` & `pyboil-0.5.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 
 this_dir = Path(__file__).parent
 long_description = (this_dir / "README.md").read_text()
 
 setup_info = dict(
     name='pyboil',
     python_requires=">=3.10",
-    version='0.5.5',
+    version='0.5.6',
     description='CLI script to initialize python packages',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Reed Schick",
     author_email='rns350@nyu.edu',
     url='https://github.com/rns350/pyinit',
     packages=find_packages(
         where='.', 
         include=['pyboil*']
     ),
     include_package_data=True,
     entry_points={
             'console_scripts': [
-                'pyboil = main:launch',
+                'pyboil = pyboil.pyboil:launch',
             ]
         },
     install_requires=[],
     setup_requires=[],
     tests_require=['pytest']
 )
```

