# Comparing `tmp/assignment-manager-0.1.5.tar.gz` & `tmp/assignment-manager-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assignment-manager-0.1.5.tar", last modified: Fri Apr 28 16:05:10 2023, max compression
+gzip compressed data, was "assignment-manager-0.1.6.tar", last modified: Tue May  9 06:25:04 2023, max compression
```

## Comparing `assignment-manager-0.1.5.tar` & `assignment-manager-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-28 16:05:10.749641 assignment-manager-0.1.5/
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     1074 2023-04-23 16:17:44.000000 assignment-manager-0.1.5/LICENSE
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-04-28 16:05:10.749641 assignment-manager-0.1.5/PKG-INFO
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       21 2023-04-23 16:24:52.000000 assignment-manager-0.1.5/README.md
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      129 2023-04-26 20:40:07.000000 assignment-manager-0.1.5/pyproject.toml
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       74 2023-04-28 16:05:10.749641 assignment-manager-0.1.5/setup.cfg
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     2136 2023-04-28 16:04:47.000000 assignment-manager-0.1.5/setup.py
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-28 16:05:10.745641 assignment-manager-0.1.5/src/
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-28 16:05:10.745641 assignment-manager-0.1.5/src/assignment_manager/
--rw-rw-r--   0 rancic    (1000) rancic    (1000)        0 2023-04-23 16:35:05.000000 assignment-manager-0.1.5/src/assignment_manager/__init__.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     5177 2023-04-28 16:03:33.000000 assignment-manager-0.1.5/src/assignment_manager/assignments.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     1817 2023-04-28 15:55:50.000000 assignment-manager-0.1.5/src/assignment_manager/data.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     2461 2023-04-28 09:11:02.000000 assignment-manager-0.1.5/src/assignment_manager/io.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     1013 2023-04-28 09:09:32.000000 assignment-manager-0.1.5/src/assignment_manager/main.py
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-28 16:05:10.745641 assignment-manager-0.1.5/src/assignment_manager.egg-info/
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-04-28 16:05:10.000000 assignment-manager-0.1.5/src/assignment_manager.egg-info/PKG-INFO
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      493 2023-04-28 16:05:10.000000 assignment-manager-0.1.5/src/assignment_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)        1 2023-04-28 16:05:10.000000 assignment-manager-0.1.5/src/assignment_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      106 2023-04-28 16:05:10.000000 assignment-manager-0.1.5/src/assignment_manager.egg-info/entry_points.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       20 2023-04-28 16:05:10.000000 assignment-manager-0.1.5/src/assignment_manager.egg-info/requires.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       19 2023-04-28 16:05:10.000000 assignment-manager-0.1.5/src/assignment_manager.egg-info/top_level.txt
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-05-09 06:25:04.318008 assignment-manager-0.1.6/
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     1074 2023-04-23 16:17:44.000000 assignment-manager-0.1.6/LICENSE
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-05-09 06:25:04.318008 assignment-manager-0.1.6/PKG-INFO
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       21 2023-04-23 16:24:52.000000 assignment-manager-0.1.6/README.md
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      129 2023-04-26 20:40:07.000000 assignment-manager-0.1.6/pyproject.toml
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       74 2023-05-09 06:25:04.318008 assignment-manager-0.1.6/setup.cfg
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     2136 2023-05-09 06:24:46.000000 assignment-manager-0.1.6/setup.py
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-05-09 06:25:04.314008 assignment-manager-0.1.6/src/
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-05-09 06:25:04.314008 assignment-manager-0.1.6/src/assignment_manager/
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)        0 2023-04-23 16:35:05.000000 assignment-manager-0.1.6/src/assignment_manager/__init__.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     5193 2023-05-09 06:24:19.000000 assignment-manager-0.1.6/src/assignment_manager/assignments.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     1817 2023-04-28 15:55:50.000000 assignment-manager-0.1.6/src/assignment_manager/data.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     2461 2023-04-28 09:11:02.000000 assignment-manager-0.1.6/src/assignment_manager/io.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     1013 2023-04-28 09:09:32.000000 assignment-manager-0.1.6/src/assignment_manager/main.py
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-05-09 06:25:04.318008 assignment-manager-0.1.6/src/assignment_manager.egg-info/
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-05-09 06:25:04.000000 assignment-manager-0.1.6/src/assignment_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      493 2023-05-09 06:25:04.000000 assignment-manager-0.1.6/src/assignment_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)        1 2023-05-09 06:25:04.000000 assignment-manager-0.1.6/src/assignment_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      106 2023-05-09 06:25:04.000000 assignment-manager-0.1.6/src/assignment_manager.egg-info/entry_points.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       20 2023-05-09 06:25:04.000000 assignment-manager-0.1.6/src/assignment_manager.egg-info/requires.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       19 2023-05-09 06:25:04.000000 assignment-manager-0.1.6/src/assignment_manager.egg-info/top_level.txt
```

### Comparing `assignment-manager-0.1.5/LICENSE` & `assignment-manager-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `assignment-manager-0.1.5/PKG-INFO` & `assignment-manager-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assignment-manager
-Version: 0.1.5
+Version: 0.1.6
 Summary: Manage reoccuring assignments and tasks.
 Home-page: https://github.com/PraxTube/assignment-manager
 Author: Prax
 Project-URL: Bug Reports, https://github.com/PraxTube/assignment-manager/issues
 Project-URL: Source, https://github.com/PraxTube/assignment-manager
 Keywords: manager,task,assignment,task-manager,assignment-manager
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `assignment-manager-0.1.5/setup.py` & `assignment-manager-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="assignment-manager",
-    version="0.1.5",
+    version="0.1.6",
     description=("Manage reoccuring assignments and tasks."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PraxTube/assignment-manager",
     author="Prax",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `assignment-manager-0.1.5/src/assignment_manager/assignments.py` & `assignment-manager-0.1.6/src/assignment_manager/assignments.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 )
 from assignment_manager import io
 
 
 def _find_next_deadline(assignment_data):
     current_date = datetime.today()
     for i, d in enumerate(assignment_data):
-        if datetime.strptime(d[1], "%d.%m.%Y") >= current_date:
+        if (datetime.strptime(d[1], "%d.%m.%Y") - current_date).days >= -1:
             return i
     return len(assignment_data) - 1
 
 
 def sort_data(row_data, sort_index, ascending=True):
     if sort_index < 0 or sort_index >= len(row_data):
         raise ValueError(
@@ -35,15 +35,15 @@
     data = load_data()
     table_rows = []
     for key in data:
         cycle = _find_next_deadline(data[key])
         remaing_days = (
             datetime.strptime(data[key][cycle][1], "%d.%m.%Y")
             - datetime.today()
-        ).days
+        ).days + 1
         table_rows.append(
             [
                 key,
                 datetime.strptime(data[key][cycle][0], "%d.%m.%Y"),
                 datetime.strptime(data[key][cycle][1], "%d.%m.%Y"),
                 Progress(data[key][cycle][2]),
                 remaing_days,
```

### Comparing `assignment-manager-0.1.5/src/assignment_manager/data.py` & `assignment-manager-0.1.6/src/assignment_manager/data.py`

 * *Files identical despite different names*

### Comparing `assignment-manager-0.1.5/src/assignment_manager/io.py` & `assignment-manager-0.1.6/src/assignment_manager/io.py`

 * *Files identical despite different names*

### Comparing `assignment-manager-0.1.5/src/assignment_manager/main.py` & `assignment-manager-0.1.6/src/assignment_manager/main.py`

 * *Files identical despite different names*

### Comparing `assignment-manager-0.1.5/src/assignment_manager.egg-info/PKG-INFO` & `assignment-manager-0.1.6/src/assignment_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assignment-manager
-Version: 0.1.5
+Version: 0.1.6
 Summary: Manage reoccuring assignments and tasks.
 Home-page: https://github.com/PraxTube/assignment-manager
 Author: Prax
 Project-URL: Bug Reports, https://github.com/PraxTube/assignment-manager/issues
 Project-URL: Source, https://github.com/PraxTube/assignment-manager
 Keywords: manager,task,assignment,task-manager,assignment-manager
 Classifier: Development Status :: 3 - Alpha
```

