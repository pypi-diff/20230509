# Comparing `tmp/duckdb_kernel-0.3.0.tar.gz` & `tmp/duckdb_kernel-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/duckdb_kernel-0.3.0.tar", last modified: Tue May  9 13:22:19 2023, max compression
+gzip compressed data, was "dist/duckdb_kernel-0.4.0.tar", last modified: Tue May  9 13:26:33 2023, max compression
```

## Comparing `duckdb_kernel-0.3.0.tar` & `duckdb_kernel-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 suyin      (501) staff       (20)        0 2023-05-09 13:22:19.494103 duckdb_kernel-0.3.0/
--rw-r--r--   0 suyin      (501) staff       (20)     1065 2023-05-08 13:30:23.000000 duckdb_kernel-0.3.0/LICENSE.txt
--rw-r--r--   0 suyin      (501) staff       (20)      137 2023-05-08 12:21:33.000000 duckdb_kernel-0.3.0/MANIFEST.in
--rw-r--r--   0 suyin      (501) staff       (20)     1918 2023-05-09 13:22:19.494437 duckdb_kernel-0.3.0/PKG-INFO
--rw-r--r--   0 suyin      (501) staff       (20)      820 2023-05-08 15:26:37.000000 duckdb_kernel-0.3.0/README.md
-drwxr-xr-x   0 suyin      (501) staff       (20)        0 2023-05-09 13:22:19.488965 duckdb_kernel-0.3.0/duckdb_kernel/
--rw-r--r--   0 suyin      (501) staff       (20)       21 2023-05-09 13:21:57.000000 duckdb_kernel-0.3.0/duckdb_kernel/__init__.py
--rw-r--r--   0 suyin      (501) staff       (20)      132 2023-05-05 01:42:53.000000 duckdb_kernel-0.3.0/duckdb_kernel/__main__.py
--rw-r--r--   0 suyin      (501) staff       (20)     2495 2023-05-09 11:27:30.000000 duckdb_kernel-0.3.0/duckdb_kernel/kernel.py
--rw-r--r--   0 suyin      (501) staff       (20)      142 2023-05-08 13:01:54.000000 duckdb_kernel-0.3.0/duckdb_kernel/kernel_template.json
-drwxr-xr-x   0 suyin      (501) staff       (20)        0 2023-05-09 13:22:19.493304 duckdb_kernel-0.3.0/duckdb_kernel.egg-info/
--rw-r--r--   0 suyin      (501) staff       (20)     1918 2023-05-09 13:22:19.000000 duckdb_kernel-0.3.0/duckdb_kernel.egg-info/PKG-INFO
--rw-r--r--   0 suyin      (501) staff       (20)      347 2023-05-09 13:22:19.000000 duckdb_kernel-0.3.0/duckdb_kernel.egg-info/SOURCES.txt
--rw-r--r--   0 suyin      (501) staff       (20)        1 2023-05-09 13:22:19.000000 duckdb_kernel-0.3.0/duckdb_kernel.egg-info/dependency_links.txt
--rw-r--r--   0 suyin      (501) staff       (20)       24 2023-05-09 13:22:19.000000 duckdb_kernel-0.3.0/duckdb_kernel.egg-info/requires.txt
--rw-r--r--   0 suyin      (501) staff       (20)       14 2023-05-09 13:22:19.000000 duckdb_kernel-0.3.0/duckdb_kernel.egg-info/top_level.txt
--rw-r--r--   0 suyin      (501) staff       (20)      258 2023-05-09 13:22:19.495991 duckdb_kernel-0.3.0/setup.cfg
--rw-r--r--   0 suyin      (501) staff       (20)     3198 2023-05-09 13:21:44.000000 duckdb_kernel-0.3.0/setup.py
+drwxr-xr-x   0 suyin      (501) staff       (20)        0 2023-05-09 13:26:33.062764 duckdb_kernel-0.4.0/
+-rw-r--r--   0 suyin      (501) staff       (20)     1065 2023-05-08 13:30:23.000000 duckdb_kernel-0.4.0/LICENSE.txt
+-rw-r--r--   0 suyin      (501) staff       (20)      137 2023-05-08 12:21:33.000000 duckdb_kernel-0.4.0/MANIFEST.in
+-rw-r--r--   0 suyin      (501) staff       (20)     1918 2023-05-09 13:26:33.063115 duckdb_kernel-0.4.0/PKG-INFO
+-rw-r--r--   0 suyin      (501) staff       (20)      820 2023-05-08 15:26:37.000000 duckdb_kernel-0.4.0/README.md
+drwxr-xr-x   0 suyin      (501) staff       (20)        0 2023-05-09 13:26:33.056887 duckdb_kernel-0.4.0/duckdb_kernel/
+-rw-r--r--   0 suyin      (501) staff       (20)       21 2023-05-09 13:25:56.000000 duckdb_kernel-0.4.0/duckdb_kernel/__init__.py
+-rw-r--r--   0 suyin      (501) staff       (20)      132 2023-05-05 01:42:53.000000 duckdb_kernel-0.4.0/duckdb_kernel/__main__.py
+-rw-r--r--   0 suyin      (501) staff       (20)     2495 2023-05-09 11:27:30.000000 duckdb_kernel-0.4.0/duckdb_kernel/kernel.py
+-rw-r--r--   0 suyin      (501) staff       (20)      142 2023-05-08 13:01:54.000000 duckdb_kernel-0.4.0/duckdb_kernel/kernel_template.json
+drwxr-xr-x   0 suyin      (501) staff       (20)        0 2023-05-09 13:26:33.061950 duckdb_kernel-0.4.0/duckdb_kernel.egg-info/
+-rw-r--r--   0 suyin      (501) staff       (20)     1918 2023-05-09 13:26:33.000000 duckdb_kernel-0.4.0/duckdb_kernel.egg-info/PKG-INFO
+-rw-r--r--   0 suyin      (501) staff       (20)      347 2023-05-09 13:26:33.000000 duckdb_kernel-0.4.0/duckdb_kernel.egg-info/SOURCES.txt
+-rw-r--r--   0 suyin      (501) staff       (20)        1 2023-05-09 13:26:33.000000 duckdb_kernel-0.4.0/duckdb_kernel.egg-info/dependency_links.txt
+-rw-r--r--   0 suyin      (501) staff       (20)       24 2023-05-09 13:26:33.000000 duckdb_kernel-0.4.0/duckdb_kernel.egg-info/requires.txt
+-rw-r--r--   0 suyin      (501) staff       (20)       14 2023-05-09 13:26:33.000000 duckdb_kernel-0.4.0/duckdb_kernel.egg-info/top_level.txt
+-rw-r--r--   0 suyin      (501) staff       (20)      258 2023-05-09 13:26:33.064381 duckdb_kernel-0.4.0/setup.cfg
+-rw-r--r--   0 suyin      (501) staff       (20)     3180 2023-05-09 13:25:45.000000 duckdb_kernel-0.4.0/setup.py
```

### Comparing `duckdb_kernel-0.3.0/LICENSE.txt` & `duckdb_kernel-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `duckdb_kernel-0.3.0/PKG-INFO` & `duckdb_kernel-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckdb_kernel
-Version: 0.3.0
+Version: 0.4.0
 Summary: UNKNOWN
 Home-page: https://github.com/suyin1203/duckdb_kernel
 Author: suyin
 License: MIT
 Description: 
         A duckdb kernel for Jupyter. Using SQL for data analysis in  Jupyter with DuckDB.  
         在Jupyter中使用SQL和duckdb进行数据分析。
```

### Comparing `duckdb_kernel-0.3.0/README.md` & `duckdb_kernel-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `duckdb_kernel-0.3.0/duckdb_kernel/kernel.py` & `duckdb_kernel-0.4.0/duckdb_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `duckdb_kernel-0.3.0/duckdb_kernel.egg-info/PKG-INFO` & `duckdb_kernel-0.4.0/duckdb_kernel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckdb-kernel
-Version: 0.3.0
+Version: 0.4.0
 Summary: UNKNOWN
 Home-page: https://github.com/suyin1203/duckdb_kernel
 Author: suyin
 License: MIT
 Description: 
         A duckdb kernel for Jupyter. Using SQL for data analysis in  Jupyter with DuckDB.  
         在Jupyter中使用SQL和duckdb进行数据分析。
```

### Comparing `duckdb_kernel-0.3.0/setup.py` & `duckdb_kernel-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,25 +26,25 @@
 os.makedirs(os.path.join(DISTNAME, 'duckdb'), exist_ok=True)
 with open(os.path.join(DISTNAME, 'kernel_template.json'), 'r') as fp:
     duckdb_json = json.load(fp)
 duckdb_json['argv'][0] = PY_EXECUTABLE
 with open(os.path.join(DISTNAME, 'duckdb','kernel.json'), 'w') as fp:
     json.dump(duckdb_json, fp)
 
-# os.makedirs(os.path.join(DISTNAME, 'duckdb_connect'), exist_ok=True)
-# with open(os.path.join(DISTNAME, 'kernel_template.json'), 'r') as fp:
-#     duckdb_json = json.load(fp)
+os.makedirs(os.path.join(DISTNAME, 'duckdb_connect'), exist_ok=True)
+with open(os.path.join(DISTNAME, 'kernel_template.json'), 'r') as fp:
+    duckdb_json = json.load(fp)
 
-# duckdb_json['argv'][0] = PY_EXECUTABLE
-# duckdb_json['display_name'] = 'duckdb (Connection)'
-# duckdb_json['name'] = "duckdb_connect"
+duckdb_json['argv'][0] = PY_EXECUTABLE
+duckdb_json['display_name'] = 'duckdb (Connection)'
+duckdb_json['name'] = "duckdb_connect"
 
-# duckdb_json['env'] = {'connect-to-existing-kernel': '1'}
-# with open(os.path.join(DISTNAME, 'duckdb_connect','kernel.json'), 'w') as fp:
-#     json.dump(duckdb_json, fp)
+duckdb_json['env'] = {'connect-to-existing-kernel': '1'}
+with open(os.path.join(DISTNAME, 'duckdb_connect','kernel.json'), 'w') as fp:
+    json.dump(duckdb_json, fp)
 
 PACKAGE_DATA = {
     DISTNAME: ['*.m'] + glob.glob('%s/**/*.*' % DISTNAME)
 }
 
 # DATA_FILES = [
 #     ('Jupyter/kernels/duckdb', [
```

