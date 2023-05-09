# Comparing `tmp/pyboil-0.5.2.tar.gz` & `tmp/pyboil-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyboil-0.5.2.tar", last modified: Tue May  9 16:29:15 2023, max compression
+gzip compressed data, was "pyboil-0.5.4.tar", last modified: Tue May  9 16:44:32 2023, max compression
```

## Comparing `pyboil-0.5.2.tar` & `pyboil-0.5.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:29:15.733786 pyboil-0.5.2/
--rw-r--r--   0 reed      (1000) reed      (1000)    35149 2023-05-09 15:34:10.000000 pyboil-0.5.2/LICENSE
--rw-r--r--   0 reed      (1000) reed      (1000)      338 2023-05-09 16:29:15.733786 pyboil-0.5.2/PKG-INFO
--rw-r--r--   0 reed      (1000) reed      (1000)       58 2023-05-09 16:24:15.000000 pyboil-0.5.2/README.md
-drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:29:15.723786 pyboil-0.5.2/pyboil/
--rw-r--r--   0 reed      (1000) reed      (1000)        0 2023-05-09 15:38:29.000000 pyboil-0.5.2/pyboil/__init__.py
--rw-r--r--   0 reed      (1000) reed      (1000)     1089 2023-05-09 16:24:39.000000 pyboil-0.5.2/pyboil/parser.py
--rw-r--r--   0 reed      (1000) reed      (1000)      530 2023-05-09 16:28:55.000000 pyboil-0.5.2/pyboil/pyboil.py
-drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:29:15.733786 pyboil-0.5.2/pyboil.egg-info/
--rw-r--r--   0 reed      (1000) reed      (1000)      338 2023-05-09 16:29:15.000000 pyboil-0.5.2/pyboil.egg-info/PKG-INFO
--rw-r--r--   0 reed      (1000) reed      (1000)      247 2023-05-09 16:29:15.000000 pyboil-0.5.2/pyboil.egg-info/SOURCES.txt
--rw-r--r--   0 reed      (1000) reed      (1000)        1 2023-05-09 16:29:15.000000 pyboil-0.5.2/pyboil.egg-info/dependency_links.txt
--rw-r--r--   0 reed      (1000) reed      (1000)       41 2023-05-09 16:29:15.000000 pyboil-0.5.2/pyboil.egg-info/entry_points.txt
--rw-r--r--   0 reed      (1000) reed      (1000)        7 2023-05-09 16:29:15.000000 pyboil-0.5.2/pyboil.egg-info/top_level.txt
--rw-r--r--   0 reed      (1000) reed      (1000)       80 2023-05-09 15:35:33.000000 pyboil-0.5.2/pyproject.toml
--rw-r--r--   0 reed      (1000) reed      (1000)       38 2023-05-09 16:29:15.733786 pyboil-0.5.2/setup.cfg
--rw-r--r--   0 reed      (1000) reed      (1000)      858 2023-05-09 16:29:06.000000 pyboil-0.5.2/setup.py
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:44:32.813786 pyboil-0.5.4/
+-rw-r--r--   0 reed      (1000) reed      (1000)    35149 2023-05-09 15:34:10.000000 pyboil-0.5.4/LICENSE
+-rw-r--r--   0 reed      (1000) reed      (1000)      338 2023-05-09 16:44:32.803786 pyboil-0.5.4/PKG-INFO
+-rw-r--r--   0 reed      (1000) reed      (1000)       58 2023-05-09 16:24:15.000000 pyboil-0.5.4/README.md
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:44:32.803786 pyboil-0.5.4/pyboil/
+-rw-r--r--   0 reed      (1000) reed      (1000)        0 2023-05-09 15:38:29.000000 pyboil-0.5.4/pyboil/__init__.py
+-rw-r--r--   0 reed      (1000) reed      (1000)     1089 2023-05-09 16:24:39.000000 pyboil-0.5.4/pyboil/parser.py
+-rw-r--r--   0 reed      (1000) reed      (1000)      571 2023-05-09 16:41:45.000000 pyboil-0.5.4/pyboil/pyboil.py
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-09 16:44:32.803786 pyboil-0.5.4/pyboil.egg-info/
+-rw-r--r--   0 reed      (1000) reed      (1000)      338 2023-05-09 16:44:32.000000 pyboil-0.5.4/pyboil.egg-info/PKG-INFO
+-rw-r--r--   0 reed      (1000) reed      (1000)      247 2023-05-09 16:44:32.000000 pyboil-0.5.4/pyboil.egg-info/SOURCES.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)        1 2023-05-09 16:44:32.000000 pyboil-0.5.4/pyboil.egg-info/dependency_links.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)       41 2023-05-09 16:44:32.000000 pyboil-0.5.4/pyboil.egg-info/entry_points.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)        7 2023-05-09 16:44:32.000000 pyboil-0.5.4/pyboil.egg-info/top_level.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)       80 2023-05-09 15:35:33.000000 pyboil-0.5.4/pyproject.toml
+-rw-r--r--   0 reed      (1000) reed      (1000)       38 2023-05-09 16:44:32.813786 pyboil-0.5.4/setup.cfg
+-rw-r--r--   0 reed      (1000) reed      (1000)      858 2023-05-09 16:44:23.000000 pyboil-0.5.4/setup.py
```

### Comparing `pyboil-0.5.2/LICENSE` & `pyboil-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyboil-0.5.2/pyboil/parser.py` & `pyboil-0.5.4/pyboil/parser.py`

 * *Files identical despite different names*

### Comparing `pyboil-0.5.2/pyboil/pyboil.py` & `pyboil-0.5.4/pyboil/pyboil.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,8 +13,11 @@
     setup.replace('{VERSION}', args['VERSION'])
     setup.replace('{DESCRIPTION}', args['DESCRIPTION'])
     setup.replace('{AUTHOR}', args['AUTHOR'])
     setup.replace('{EMAIL}', args['EMAIL'])
     setup.replace('{URL}', args['URL'])
 
     with open('./setup.py', 'w') as f:
-        f.write(setup)
+        f.write(setup)
+
+if __name__ == "__main__":
+    launch()
```

### Comparing `pyboil-0.5.2/setup.py` & `pyboil-0.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_dir = Path(__file__).parent
 long_description = (this_dir / "README.md").read_text()
 
 setup_info = dict(
     name='pyboil',
     python_requires=">=3.10",
-    version='0.5.2',
+    version='0.5.4',
     description='CLI script to initialize python packages',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Reed Schick",
     author_email='rns350@nyu.edu',
     url='https://github.com/rns350/pyinit',
     packages=find_packages(
```

