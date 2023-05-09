# Comparing `tmp/flams-0.0.3.tar.gz` & `tmp/flams-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flams-0.0.3.tar", last modified: Wed May  3 08:25:54 2023, max compression
+gzip compressed data, was "flams-0.0.4.tar", last modified: Tue May  9 13:13:30 2023, max compression
```

## Comparing `flams-0.0.3.tar` & `flams-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-03 08:25:54.940258 flams-0.0.3/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     1223 2023-05-02 14:42:26.000000 flams-0.0.3/LICENSE
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     5783 2023-05-03 08:25:54.940258 flams-0.0.3/PKG-INFO
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     5523 2023-05-02 06:30:11.000000 flams-0.0.3/README.md
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-03 08:25:54.936258 flams-0.0.3/flams/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-04-07 09:12:53.000000 flams-0.0.3/flams/__init__.py
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-03 08:25:54.940258 flams-0.0.3/flams/databases/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-04-07 09:12:53.000000 flams-0.0.3/flams/databases/__init__.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     2825 2023-04-07 09:12:53.000000 flams-0.0.3/flams/databases/cplmv4.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     8911 2023-05-02 11:49:48.000000 flams-0.0.3/flams/databases/setup.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     3491 2023-05-02 06:30:11.000000 flams-0.0.3/flams/display.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     2449 2023-05-02 12:00:55.000000 flams-0.0.3/flams/flams.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)    12083 2023-05-02 14:35:57.000000 flams-0.0.3/flams/input.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)    12408 2023-05-02 11:49:04.000000 flams-0.0.3/flams/run_blast.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      768 2023-04-07 09:12:53.000000 flams-0.0.3/flams/utils.py
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-03 08:25:54.940258 flams-0.0.3/flams.egg-info/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     5783 2023-05-03 08:25:54.000000 flams-0.0.3/flams.egg-info/PKG-INFO
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      403 2023-05-03 08:25:54.000000 flams-0.0.3/flams.egg-info/SOURCES.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        1 2023-05-03 08:25:54.000000 flams-0.0.3/flams.egg-info/dependency_links.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)       43 2023-05-03 08:25:54.000000 flams-0.0.3/flams.egg-info/entry_points.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      316 2023-05-03 08:25:54.000000 flams-0.0.3/flams.egg-info/requires.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        6 2023-05-03 08:25:54.000000 flams-0.0.3/flams.egg-info/top_level.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      454 2023-05-03 08:25:49.000000 flams-0.0.3/pyproject.toml
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      315 2023-04-07 09:12:53.000000 flams-0.0.3/requirements.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)       38 2023-05-03 08:25:54.940258 flams-0.0.3/setup.cfg
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 13:13:30.587750 flams-0.0.4/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     1223 2023-05-09 12:23:21.000000 flams-0.0.4/LICENSE
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     5783 2023-05-09 13:13:30.587750 flams-0.0.4/PKG-INFO
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     5523 2023-05-09 12:23:21.000000 flams-0.0.4/README.md
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 13:13:30.583750 flams-0.0.4/flams/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 12:23:21.000000 flams-0.0.4/flams/__init__.py
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 13:13:30.587750 flams-0.0.4/flams/databases/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 12:23:21.000000 flams-0.0.4/flams/databases/__init__.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     2825 2023-05-09 12:23:21.000000 flams-0.0.4/flams/databases/cplmv4.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     8911 2023-05-09 12:23:21.000000 flams-0.0.4/flams/databases/setup.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     3491 2023-05-09 12:23:21.000000 flams-0.0.4/flams/display.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     2449 2023-05-09 12:23:21.000000 flams-0.0.4/flams/flams.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)    12083 2023-05-09 12:23:21.000000 flams-0.0.4/flams/input.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)    12408 2023-05-09 12:23:21.000000 flams-0.0.4/flams/run_blast.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      960 2023-05-09 12:59:47.000000 flams-0.0.4/flams/utils.py
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 13:13:30.587750 flams-0.0.4/flams.egg-info/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     5783 2023-05-09 13:13:30.000000 flams-0.0.4/flams.egg-info/PKG-INFO
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      403 2023-05-09 13:13:30.000000 flams-0.0.4/flams.egg-info/SOURCES.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        1 2023-05-09 13:13:30.000000 flams-0.0.4/flams.egg-info/dependency_links.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)       43 2023-05-09 13:13:30.000000 flams-0.0.4/flams.egg-info/entry_points.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      316 2023-05-09 13:13:30.000000 flams-0.0.4/flams.egg-info/requires.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        6 2023-05-09 13:13:30.000000 flams-0.0.4/flams.egg-info/top_level.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      454 2023-05-09 13:13:22.000000 flams-0.0.4/pyproject.toml
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      315 2023-05-09 12:23:21.000000 flams-0.0.4/requirements.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)       38 2023-05-09 13:13:30.587750 flams-0.0.4/setup.cfg
```

### Comparing `flams-0.0.3/LICENSE` & `flams-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flams-0.0.3/PKG-INFO` & `flams-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flams
-Version: 0.0.3
+Version: 0.0.4
 Summary: Find Lysine Acylation & other Modification Sites
 Project-URL: repository, https://github.com/hannelorelongin/FLAMS
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FLAMS: Find Lysine Acylation & other Modification Sites
```

### Comparing `flams-0.0.3/README.md` & `flams-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `flams-0.0.3/flams/databases/cplmv4.py` & `flams-0.0.4/flams/databases/cplmv4.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.3/flams/databases/setup.py` & `flams-0.0.4/flams/databases/setup.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.3/flams/display.py` & `flams-0.0.4/flams/display.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.3/flams/flams.py` & `flams-0.0.4/flams/flams.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.3/flams/input.py` & `flams-0.0.4/flams/input.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.3/flams/run_blast.py` & `flams-0.0.4/flams/run_blast.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.3/flams/utils.py` & `flams-0.0.4/flams/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,10 +21,14 @@
     Parameters
     ----------
     app_name: str
     Name of application, i.e., flams
 
     """
     # Ensure data dir exists and return.
-    data_dir = appdirs.user_data_dir(app_name)
-    Path(data_dir).mkdir(parents=True, exist_ok=True)
+    try:
+        data_dir = appdirs.user_data_dir(app_name)
+        Path(data_dir).mkdir(parents=True, exist_ok=True)
+    except PermissionError: # This should only apply for deployment of web-app
+        data_dir = "/app/flams_data/"
+        Path(data_dir).mkdir(parents=True, exist_ok=True)
     return data_dir
```

### Comparing `flams-0.0.3/flams.egg-info/PKG-INFO` & `flams-0.0.4/flams.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flams
-Version: 0.0.3
+Version: 0.0.4
 Summary: Find Lysine Acylation & other Modification Sites
 Project-URL: repository, https://github.com/hannelorelongin/FLAMS
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FLAMS: Find Lysine Acylation & other Modification Sites
```

