# Comparing `tmp/bioplotz-0.1.0.dev5.tar.gz` & `tmp/bioplotz-0.1.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioplotz-0.1.0.dev5.tar", last modified: Mon May  8 07:23:09 2023, max compression
+gzip compressed data, was "bioplotz-0.1.0.dev6.tar", last modified: Tue May  9 09:43:05 2023, max compression
```

## Comparing `bioplotz-0.1.0.dev5.tar` & `bioplotz-0.1.0.dev6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-08 07:23:09.505732 bioplotz-0.1.0.dev5/
--rw-r--r--   0 zsc       (1000) users      (100)     1305 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev5/LICENSE
--rw-r--r--   0 zsc       (1000) users      (100)       67 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev5/MANIFEST.in
--rw-r--r--   0 zsc       (1000) users      (100)    13845 2023-05-08 07:23:09.505732 bioplotz-0.1.0.dev5/PKG-INFO
--rw-r--r--   0 zsc       (1000) users      (100)    13548 2023-05-05 02:18:26.000000 bioplotz-0.1.0.dev5/README.md
-drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-08 07:23:09.501732 bioplotz-0.1.0.dev5/bioplotz/
--rw-r--r--   0 zsc       (1000) users      (100)      225 2023-05-08 07:21:48.000000 bioplotz-0.1.0.dev5/bioplotz/__init__.py
--rw-r--r--   0 zsc       (1000) users      (100)    10185 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev5/bioplotz/chromosome.py
--rw-r--r--   0 zsc       (1000) users      (100)     2477 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev5/bioplotz/genecluster.py
--rwxr-xr-x   0 zsc       (1000) users      (100)     6110 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev5/bioplotz/manhattan.py
--rw-r--r--   0 zsc       (1000) users      (100)     4706 2023-05-08 07:20:31.000000 bioplotz-0.1.0.dev5/bioplotz/mulitalign.py
-drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-08 07:23:09.505732 bioplotz-0.1.0.dev5/bioplotz.egg-info/
--rw-r--r--   0 zsc       (1000) users      (100)    13845 2023-05-08 07:23:09.000000 bioplotz-0.1.0.dev5/bioplotz.egg-info/PKG-INFO
--rw-r--r--   0 zsc       (1000) users      (100)      310 2023-05-08 07:23:09.000000 bioplotz-0.1.0.dev5/bioplotz.egg-info/SOURCES.txt
--rw-r--r--   0 zsc       (1000) users      (100)        1 2023-05-08 07:23:09.000000 bioplotz-0.1.0.dev5/bioplotz.egg-info/dependency_links.txt
--rw-r--r--   0 zsc       (1000) users      (100)       24 2023-05-08 07:23:09.000000 bioplotz-0.1.0.dev5/bioplotz.egg-info/requires.txt
--rw-r--r--   0 zsc       (1000) users      (100)        9 2023-05-08 07:23:09.000000 bioplotz-0.1.0.dev5/bioplotz.egg-info/top_level.txt
--rw-r--r--   0 zsc       (1000) users      (100)       38 2023-05-08 07:23:09.505732 bioplotz-0.1.0.dev5/setup.cfg
--rw-r--r--   0 zsc       (1000) users      (100)      643 2023-05-08 07:21:45.000000 bioplotz-0.1.0.dev5/setup.py
+drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-09 09:43:05.280982 bioplotz-0.1.0.dev6/
+-rw-r--r--   0 zsc       (1000) users      (100)     1305 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev6/LICENSE
+-rw-r--r--   0 zsc       (1000) users      (100)       67 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev6/MANIFEST.in
+-rw-r--r--   0 zsc       (1000) users      (100)    13845 2023-05-09 09:43:05.280982 bioplotz-0.1.0.dev6/PKG-INFO
+-rw-r--r--   0 zsc       (1000) users      (100)    13548 2023-05-05 02:18:26.000000 bioplotz-0.1.0.dev6/README.md
+drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-09 09:43:05.276982 bioplotz-0.1.0.dev6/bioplotz/
+-rw-r--r--   0 zsc       (1000) users      (100)      225 2023-05-09 09:42:11.000000 bioplotz-0.1.0.dev6/bioplotz/__init__.py
+-rw-r--r--   0 zsc       (1000) users      (100)    10185 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev6/bioplotz/chromosome.py
+-rw-r--r--   0 zsc       (1000) users      (100)     2477 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev6/bioplotz/genecluster.py
+-rwxr-xr-x   0 zsc       (1000) users      (100)     6110 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev6/bioplotz/manhattan.py
+-rw-r--r--   0 zsc       (1000) users      (100)     4706 2023-05-08 07:20:31.000000 bioplotz-0.1.0.dev6/bioplotz/multialign.py
+drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-09 09:43:05.280982 bioplotz-0.1.0.dev6/bioplotz.egg-info/
+-rw-r--r--   0 zsc       (1000) users      (100)    13845 2023-05-09 09:43:05.000000 bioplotz-0.1.0.dev6/bioplotz.egg-info/PKG-INFO
+-rw-r--r--   0 zsc       (1000) users      (100)      310 2023-05-09 09:43:05.000000 bioplotz-0.1.0.dev6/bioplotz.egg-info/SOURCES.txt
+-rw-r--r--   0 zsc       (1000) users      (100)        1 2023-05-09 09:43:05.000000 bioplotz-0.1.0.dev6/bioplotz.egg-info/dependency_links.txt
+-rw-r--r--   0 zsc       (1000) users      (100)       24 2023-05-09 09:43:05.000000 bioplotz-0.1.0.dev6/bioplotz.egg-info/requires.txt
+-rw-r--r--   0 zsc       (1000) users      (100)        9 2023-05-09 09:43:05.000000 bioplotz-0.1.0.dev6/bioplotz.egg-info/top_level.txt
+-rw-r--r--   0 zsc       (1000) users      (100)       38 2023-05-09 09:43:05.280982 bioplotz-0.1.0.dev6/setup.cfg
+-rw-r--r--   0 zsc       (1000) users      (100)      643 2023-05-09 09:42:35.000000 bioplotz-0.1.0.dev6/setup.py
```

### Comparing `bioplotz-0.1.0.dev5/LICENSE` & `bioplotz-0.1.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev5/PKG-INFO` & `bioplotz-0.1.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioplotz
-Version: 0.1.0.dev5
+Version: 0.1.0.dev6
 Summary: A python package for drawing some bioinformatic pictures.
 Home-page: https://github.com/sc-zhang/bioplotz
 Author: Shengcheng Zhang
 Author-email: zsc-zhang@foxmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bioplotz-0.1.0.dev5/README.md` & `bioplotz-0.1.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev5/bioplotz/chromosome.py` & `bioplotz-0.1.0.dev6/bioplotz/chromosome.py`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev5/bioplotz/genecluster.py` & `bioplotz-0.1.0.dev6/bioplotz/genecluster.py`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev5/bioplotz/manhattan.py` & `bioplotz-0.1.0.dev6/bioplotz/manhattan.py`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev5/bioplotz/mulitalign.py` & `bioplotz-0.1.0.dev6/bioplotz/multialign.py`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev5/bioplotz.egg-info/PKG-INFO` & `bioplotz-0.1.0.dev6/bioplotz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioplotz
-Version: 0.1.0.dev5
+Version: 0.1.0.dev6
 Summary: A python package for drawing some bioinformatic pictures.
 Home-page: https://github.com/sc-zhang/bioplotz
 Author: Shengcheng Zhang
 Author-email: zsc-zhang@foxmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bioplotz-0.1.0.dev5/setup.py` & `bioplotz-0.1.0.dev6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='bioplotz',
-    version='0.1.0.dev5',
+    version='0.1.0.dev6',
     packages=['bioplotz'],
     url='https://github.com/sc-zhang/bioplotz',
     license='',
     author='Shengcheng Zhang',
     author_email='zsc-zhang@foxmail.com',
     description='A python package for drawing some bioinformatic pictures.',
     long_description=long_description,
```

