# Comparing `tmp/gscipy-0.1.3.tar.gz` & `tmp/gscipy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gscipy-0.1.3.tar", last modified: Fri May  5 11:10:58 2023, max compression
+gzip compressed data, was "gscipy-0.1.4.tar", last modified: Tue May  9 12:17:03 2023, max compression
```

## Comparing `gscipy-0.1.3.tar` & `gscipy-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 11:10:58.886693 gscipy-0.1.3/
--rw-rw-rw-   0        0        0    17095 2022-12-14 10:37:12.000000 gscipy-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0    20525 2023-05-05 11:10:58.886191 gscipy-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       55 2022-11-03 15:15:37.000000 gscipy-0.1.3/README.md
--rw-rw-rw-   0        0        0     1710 2023-05-05 11:09:10.000000 gscipy-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 11:10:58.887194 gscipy-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-05 11:10:58.748727 gscipy-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-05 11:10:58.855614 gscipy-0.1.3/src/gscipy/
--rw-rw-rw-   0        0        0        2 2023-01-05 22:19:22.000000 gscipy-0.1.3/src/gscipy/__init__.py
--rw-rw-rw-   0        0        0      421 2023-04-06 13:52:32.000000 gscipy-0.1.3/src/gscipy/config.py
--rw-rw-rw-   0        0        0     5682 2023-01-11 15:19:15.000000 gscipy-0.1.3/src/gscipy/csv_io.py
--rw-rw-rw-   0        0        0      775 2023-01-11 09:29:40.000000 gscipy-0.1.3/src/gscipy/decorators.py
--rw-rw-rw-   0        0        0     2312 2023-04-04 14:48:36.000000 gscipy-0.1.3/src/gscipy/general.py
--rw-rw-rw-   0        0        0     6969 2023-04-15 22:24:08.000000 gscipy-0.1.3/src/gscipy/json_io.py
--rw-rw-rw-   0        0        0     9000 2023-04-15 22:25:56.000000 gscipy-0.1.3/src/gscipy/operators.py
--rw-rw-rw-   0        0        0    28233 2023-04-15 22:19:10.000000 gscipy-0.1.3/src/gscipy/signals.py
--rw-rw-rw-   0        0        0    13336 2023-04-15 22:25:16.000000 gscipy-0.1.3/src/gscipy/time.py
--rw-rw-rw-   0        0        0    20689 2023-04-15 22:23:18.000000 gscipy-0.1.3/src/gscipy/trajectories.py
--rw-rw-rw-   0        0        0     3585 2023-04-15 14:24:09.000000 gscipy-0.1.3/src/gscipy/utils.py
--rw-rw-rw-   0        0        0    17978 2023-04-15 22:27:23.000000 gscipy-0.1.3/src/gscipy/vectors.py
--rw-rw-rw-   0        0        0     5158 2023-04-06 13:52:11.000000 gscipy-0.1.3/src/gscipy/visualization.py
-drwxrwxrwx   0        0        0        0 2023-05-05 11:10:58.877863 gscipy-0.1.3/src/gscipy.egg-info/
--rw-rw-rw-   0        0        0    20525 2023-05-05 11:10:58.000000 gscipy-0.1.3/src/gscipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      523 2023-05-05 11:10:58.000000 gscipy-0.1.3/src/gscipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 11:10:58.000000 gscipy-0.1.3/src/gscipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-05-05 11:10:58.000000 gscipy-0.1.3/src/gscipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 11:10:58.000000 gscipy-0.1.3/src/gscipy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 11:10:58.884166 gscipy-0.1.3/tests/
--rw-rw-rw-   0        0        0       34 2022-11-14 14:39:43.000000 gscipy-0.1.3/tests/test_data_io.py
+drwxrwxrwx   0        0        0        0 2023-05-09 12:17:03.458390 gscipy-0.1.4/
+-rw-rw-rw-   0        0        0    17095 2022-12-14 10:37:12.000000 gscipy-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0    20525 2023-05-09 12:17:03.457866 gscipy-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2022-11-03 15:15:37.000000 gscipy-0.1.4/README.md
+-rw-rw-rw-   0        0        0     1710 2023-05-09 12:16:27.000000 gscipy-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 12:17:03.458390 gscipy-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 12:17:03.424695 gscipy-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 12:17:03.442366 gscipy-0.1.4/src/gscipy/
+-rw-rw-rw-   0        0        0        2 2023-01-05 22:19:22.000000 gscipy-0.1.4/src/gscipy/__init__.py
+-rw-rw-rw-   0        0        0      421 2023-04-06 13:52:32.000000 gscipy-0.1.4/src/gscipy/config.py
+-rw-rw-rw-   0        0        0     5682 2023-01-11 15:19:15.000000 gscipy-0.1.4/src/gscipy/csv_io.py
+-rw-rw-rw-   0        0        0      775 2023-01-11 09:29:40.000000 gscipy-0.1.4/src/gscipy/decorators.py
+-rw-rw-rw-   0        0        0     2312 2023-04-04 14:48:36.000000 gscipy-0.1.4/src/gscipy/general.py
+-rw-rw-rw-   0        0        0     6969 2023-04-15 22:24:08.000000 gscipy-0.1.4/src/gscipy/json_io.py
+-rw-rw-rw-   0        0        0     9000 2023-04-15 22:25:56.000000 gscipy-0.1.4/src/gscipy/operators.py
+-rw-rw-rw-   0        0        0    28233 2023-04-15 22:19:10.000000 gscipy-0.1.4/src/gscipy/signals.py
+-rw-rw-rw-   0        0        0    13336 2023-04-15 22:25:16.000000 gscipy-0.1.4/src/gscipy/time.py
+-rw-rw-rw-   0        0        0    20689 2023-04-15 22:23:18.000000 gscipy-0.1.4/src/gscipy/trajectories.py
+-rw-rw-rw-   0        0        0     6002 2023-05-09 12:13:24.000000 gscipy-0.1.4/src/gscipy/utils.py
+-rw-rw-rw-   0        0        0    17978 2023-04-15 22:27:23.000000 gscipy-0.1.4/src/gscipy/vectors.py
+-rw-rw-rw-   0        0        0     5158 2023-04-06 13:52:11.000000 gscipy-0.1.4/src/gscipy/visualization.py
+drwxrwxrwx   0        0        0        0 2023-05-09 12:17:03.455425 gscipy-0.1.4/src/gscipy.egg-info/
+-rw-rw-rw-   0        0        0    20525 2023-05-09 12:17:03.000000 gscipy-0.1.4/src/gscipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      523 2023-05-09 12:17:03.000000 gscipy-0.1.4/src/gscipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 12:17:03.000000 gscipy-0.1.4/src/gscipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-05-09 12:17:03.000000 gscipy-0.1.4/src/gscipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-09 12:17:03.000000 gscipy-0.1.4/src/gscipy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 12:17:03.456427 gscipy-0.1.4/tests/
+-rw-rw-rw-   0        0        0       34 2022-11-14 14:39:43.000000 gscipy-0.1.4/tests/test_data_io.py
```

### Comparing `gscipy-0.1.3/LICENSE.txt` & `gscipy-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gscipy-0.1.3/PKG-INFO` & `gscipy-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gscipy
-Version: 0.1.3
+Version: 0.1.4
 Summary: Gabba Scientific utilities
 Author: Matteo Gabba
 Author-email: m.gabba083@gmail.com
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
```

### Comparing `gscipy-0.1.3/pyproject.toml` & `gscipy-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 where = ["src"]  # ["."] by default
 # include = ["mypackage*"]  # ["*"] by default
 # exclude = ["mypackage.tests*"]  # empty by default
 # namespaces = false  # true by default
 
 [project]
 name = "gscipy"
-version = "0.1.3"
+version = "0.1.4"
 description = "Gabba Scientific utilities"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
 keywords = ["gabba scientific", ]
 authors  =[
     {name = "Matteo Gabba"},
```

### Comparing `gscipy-0.1.3/src/gscipy/csv_io.py` & `gscipy-0.1.4/src/gscipy/csv_io.py`

 * *Files identical despite different names*

### Comparing `gscipy-0.1.3/src/gscipy/decorators.py` & `gscipy-0.1.4/src/gscipy/decorators.py`

 * *Files identical despite different names*

### Comparing `gscipy-0.1.3/src/gscipy/general.py` & `gscipy-0.1.4/src/gscipy/general.py`

 * *Files identical despite different names*

### Comparing `gscipy-0.1.3/src/gscipy/json_io.py` & `gscipy-0.1.4/src/gscipy/json_io.py`

 * *Files identical despite different names*

### Comparing `gscipy-0.1.3/src/gscipy/operators.py` & `gscipy-0.1.4/src/gscipy/operators.py`

 * *Files identical despite different names*

### Comparing `gscipy-0.1.3/src/gscipy/signals.py` & `gscipy-0.1.4/src/gscipy/signals.py`

 * *Files identical despite different names*

### Comparing `gscipy-0.1.3/src/gscipy/time.py` & `gscipy-0.1.4/src/gscipy/time.py`

 * *Files identical despite different names*

### Comparing `gscipy-0.1.3/src/gscipy/trajectories.py` & `gscipy-0.1.4/src/gscipy/trajectories.py`

 * *Files identical despite different names*

### Comparing `gscipy-0.1.3/src/gscipy/vectors.py` & `gscipy-0.1.4/src/gscipy/vectors.py`

 * *Files identical despite different names*

### Comparing `gscipy-0.1.3/src/gscipy/visualization.py` & `gscipy-0.1.4/src/gscipy/visualization.py`

 * *Files identical despite different names*

### Comparing `gscipy-0.1.3/src/gscipy.egg-info/PKG-INFO` & `gscipy-0.1.4/src/gscipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gscipy
-Version: 0.1.3
+Version: 0.1.4
 Summary: Gabba Scientific utilities
 Author: Matteo Gabba
 Author-email: m.gabba083@gmail.com
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
```

### Comparing `gscipy-0.1.3/src/gscipy.egg-info/SOURCES.txt` & `gscipy-0.1.4/src/gscipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

