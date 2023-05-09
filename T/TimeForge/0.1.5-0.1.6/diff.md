# Comparing `tmp/TimeForge-0.1.5.tar.gz` & `tmp/TimeForge-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TimeForge-0.1.5.tar", last modified: Tue May  2 12:38:00 2023, max compression
+gzip compressed data, was "TimeForge-0.1.6.tar", last modified: Tue May  9 20:24:27 2023, max compression
```

## Comparing `TimeForge-0.1.5.tar` & `TimeForge-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 12:38:00.283803 TimeForge-0.1.5/
--rw-r--r--   0 michael   (1000) michael   (1000)    34916 2023-04-04 11:47:23.000000 TimeForge-0.1.5/LICENSE.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-05-02 12:38:00.283803 TimeForge-0.1.5/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-04-05 15:25:59.000000 TimeForge-0.1.5/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)      935 2023-05-02 12:37:47.000000 TimeForge-0.1.5/pyproject.toml
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-05-02 12:38:00.283803 TimeForge-0.1.5/setup.cfg
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 12:38:00.283803 TimeForge-0.1.5/src/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 12:38:00.283803 TimeForge-0.1.5/src/TimeForge.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-05-02 12:38:00.000000 TimeForge-0.1.5/src/TimeForge.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      271 2023-05-02 12:38:00.000000 TimeForge-0.1.5/src/TimeForge.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-02 12:38:00.000000 TimeForge-0.1.5/src/TimeForge.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-05-02 12:38:00.000000 TimeForge-0.1.5/src/TimeForge.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       10 2023-05-02 12:38:00.000000 TimeForge-0.1.5/src/TimeForge.egg-info/top_level.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 12:38:00.283803 TimeForge-0.1.5/src/timeforge/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-24 11:15:53.000000 TimeForge-0.1.5/src/timeforge/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6834 2023-05-02 12:37:03.000000 TimeForge-0.1.5/src/timeforge/__main__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 20:24:27.025466 TimeForge-0.1.6/
+-rw-r--r--   0 michael   (1000) michael   (1000)    34916 2023-04-04 11:47:23.000000 TimeForge-0.1.6/LICENSE.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1232 2023-05-09 20:24:27.025466 TimeForge-0.1.6/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      559 2023-05-08 08:20:49.000000 TimeForge-0.1.6/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      935 2023-05-09 20:24:18.000000 TimeForge-0.1.6/pyproject.toml
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-05-09 20:24:27.025466 TimeForge-0.1.6/setup.cfg
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 20:24:27.022133 TimeForge-0.1.6/src/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 20:24:27.022133 TimeForge-0.1.6/src/TimeForge.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1232 2023-05-09 20:24:27.000000 TimeForge-0.1.6/src/TimeForge.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      271 2023-05-09 20:24:27.000000 TimeForge-0.1.6/src/TimeForge.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-09 20:24:27.000000 TimeForge-0.1.6/src/TimeForge.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-05-09 20:24:27.000000 TimeForge-0.1.6/src/TimeForge.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       10 2023-05-09 20:24:27.000000 TimeForge-0.1.6/src/TimeForge.egg-info/top_level.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 20:24:27.025466 TimeForge-0.1.6/src/timeforge/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-24 11:15:53.000000 TimeForge-0.1.6/src/timeforge/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6817 2023-05-09 20:24:02.000000 TimeForge-0.1.6/src/timeforge/__main__.py
```

### Comparing `TimeForge-0.1.5/LICENSE.md` & `TimeForge-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TimeForge-0.1.5/PKG-INFO` & `TimeForge-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeForge
-Version: 0.1.5
+Version: 0.1.6
 Summary: Create realistic looking but fake time documentation for your student job at KIT
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Scheduling
@@ -13,14 +13,18 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # TimeForge
 Create realistic looking but fake time documentation for your student job at KIT
 
+## Call for participation
+
+This is only a prototype with a lot of features that can be added. Unfortunately I do not have a lot of time to care for my project alone. If anyone wants to submit pull requests: Feel free to do so. 
+
 ## Installation
 
 Installation via pip:
 
 ``` bash
 $ pip install timeforge
 ```
```

### Comparing `TimeForge-0.1.5/pyproject.toml` & `TimeForge-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TimeForge"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
 	{ name="Michael Hohenstein", email="michael@hohenste.in" },
 ]
 description = "Create realistic looking but fake time documentation for your student job at KIT"
 readme = "README.md"
 requires-python= ">=3.7"
 classifiers = [
```

### Comparing `TimeForge-0.1.5/src/TimeForge.egg-info/PKG-INFO` & `TimeForge-0.1.6/src/TimeForge.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeForge
-Version: 0.1.5
+Version: 0.1.6
 Summary: Create realistic looking but fake time documentation for your student job at KIT
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Scheduling
@@ -13,14 +13,18 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # TimeForge
 Create realistic looking but fake time documentation for your student job at KIT
 
+## Call for participation
+
+This is only a prototype with a lot of features that can be added. Unfortunately I do not have a lot of time to care for my project alone. If anyone wants to submit pull requests: Feel free to do so. 
+
 ## Installation
 
 Installation via pip:
 
 ``` bash
 $ pip install timeforge
 ```
```

### Comparing `TimeForge-0.1.5/src/timeforge/__main__.py` & `TimeForge-0.1.6/src/timeforge/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 parser.add_argument('-s','--salary', type=float, required=True,
                     help="the salary (per hour) in euros")
 
 parser.add_argument('-O', '--organisation', type=str, required=True,
                     help='Name of the KIT organisational unit')
 
 parser.add_argument('-g', '--low-income', action='store_true',
-                    help='the \'geringfügig beschäftigt\' (GF) field in the form, default: False')
+                    help='the Großforschungsbereich (GF) field in the form, default: False')
 
 parser.add_argument('-u', action='store_true',
-                    help='the UB field in the form, default: False') # figure out what EB stands for
+                    help='the Universitätsbereich (UB) field in the form, default: True')
 
 parser.add_argument('-v', '--verbose', action='store_true',
                     help='more detailed information printing for debugging purpose')
 
 parser.add_argument('-i', '--input', type=str, required=True,
                     help='the location of the input file (The MiLoG-Arbeitszeitdokumentation.pdf from the PSE website)')
```

