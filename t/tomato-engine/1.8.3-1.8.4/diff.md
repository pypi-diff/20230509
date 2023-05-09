# Comparing `tmp/tomato-engine-1.8.3.tar.gz` & `tmp/tomato-engine-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomato-engine-1.8.3.tar", last modified: Thu May  4 22:52:20 2023, max compression
+gzip compressed data, was "tomato-engine-1.8.4.tar", last modified: Tue May  9 12:32:31 2023, max compression
```

## Comparing `tomato-engine-1.8.3.tar` & `tomato-engine-1.8.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-04 22:52:20.330214 tomato-engine-1.8.3/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)    35149 2022-05-23 23:00:31.000000 tomato-engine-1.8.3/LICENSE
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3049 2023-05-04 22:52:20.330214 tomato-engine-1.8.3/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2417 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/README.md
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       61 2022-05-23 23:00:31.000000 tomato-engine-1.8.3/pyproject.toml
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      836 2023-05-04 22:52:20.334214 tomato-engine-1.8.3/setup.cfg
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1009 2023-05-04 22:50:25.000000 tomato-engine-1.8.3/setup.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-04 22:52:20.326214 tomato-engine-1.8.3/src/
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-04 22:52:20.326214 tomato-engine-1.8.3/src/tomato/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       48 2022-05-23 23:00:31.000000 tomato-engine-1.8.3/src/tomato/__init__.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-04 22:52:20.326214 tomato-engine-1.8.3/src/tomato/classes/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       25 2022-05-23 23:00:31.000000 tomato-engine-1.8.3/src/tomato/classes/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)    10952 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/src/tomato/classes/board.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)    13921 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/src/tomato/classes/cell.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4569 2023-05-03 22:45:39.000000 tomato-engine-1.8.3/src/tomato/classes/cellmatrix.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3621 2023-05-04 17:41:57.000000 tomato-engine-1.8.3/src/tomato/classes/window.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-04 22:52:20.330214 tomato-engine-1.8.3/src/tomato/functions/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2022-05-23 23:00:31.000000 tomato-engine-1.8.3/src/tomato/functions/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      842 2022-06-20 19:13:20.000000 tomato-engine-1.8.3/src/tomato/functions/display.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4192 2022-07-06 18:41:02.000000 tomato-engine-1.8.3/src/tomato/functions/file_io.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4163 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/src/tomato/functions/utils.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-04 22:52:20.330214 tomato-engine-1.8.3/src/tomato/rules/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2022-05-23 23:00:31.000000 tomato-engine-1.8.3/src/tomato/rules/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      660 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/src/tomato/rules/colorful.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      273 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/src/tomato/rules/colorful_demo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      912 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/src/tomato/rules/cyclic.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      316 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/src/tomato/rules/cyclic_demo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      872 2023-05-04 22:48:21.000000 tomato-engine-1.8.3/src/tomato/rules/game_of_life.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      274 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/src/tomato/rules/game_of_life_demo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      759 2022-10-20 06:23:30.000000 tomato-engine-1.8.3/src/tomato/rules/toothpick_fractal.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      297 2023-04-27 23:43:06.000000 tomato-engine-1.8.3/src/tomato/rules/toothpick_fractal_demo.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-04 22:52:20.330214 tomato-engine-1.8.3/src/tomato_engine.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3049 2023-05-04 22:52:20.000000 tomato-engine-1.8.3/src/tomato_engine.egg-info/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      856 2023-05-04 22:52:20.000000 tomato-engine-1.8.3/src/tomato_engine.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-04 22:52:20.000000 tomato-engine-1.8.3/src/tomato_engine.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       53 2023-05-04 22:52:20.000000 tomato-engine-1.8.3/src/tomato_engine.egg-info/requires.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        7 2023-05-04 22:52:20.000000 tomato-engine-1.8.3/src/tomato_engine.egg-info/top_level.txt
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 12:32:31.950858 tomato-engine-1.8.4/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)    35149 2022-05-23 23:00:31.000000 tomato-engine-1.8.4/LICENSE
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3049 2023-05-09 12:32:31.950858 tomato-engine-1.8.4/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2417 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/README.md
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       61 2022-05-23 23:00:31.000000 tomato-engine-1.8.4/pyproject.toml
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      836 2023-05-09 12:32:31.950858 tomato-engine-1.8.4/setup.cfg
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1009 2023-05-04 22:54:50.000000 tomato-engine-1.8.4/setup.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 12:32:31.942858 tomato-engine-1.8.4/src/
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 12:32:31.942858 tomato-engine-1.8.4/src/tomato/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      116 2023-05-08 19:51:10.000000 tomato-engine-1.8.4/src/tomato/__init__.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 12:32:31.946858 tomato-engine-1.8.4/src/tomato/classes/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       93 2023-05-08 19:52:06.000000 tomato-engine-1.8.4/src/tomato/classes/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)    10952 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/src/tomato/classes/board.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)    13921 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/src/tomato/classes/cell.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4569 2023-05-03 22:45:39.000000 tomato-engine-1.8.4/src/tomato/classes/cellmatrix.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3621 2023-05-08 19:51:41.000000 tomato-engine-1.8.4/src/tomato/classes/window.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 12:32:31.946858 tomato-engine-1.8.4/src/tomato/functions/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2022-05-23 23:00:31.000000 tomato-engine-1.8.4/src/tomato/functions/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      842 2022-06-20 19:13:20.000000 tomato-engine-1.8.4/src/tomato/functions/display.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4192 2022-07-06 18:41:02.000000 tomato-engine-1.8.4/src/tomato/functions/file_io.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4163 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/src/tomato/functions/utils.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 12:32:31.950858 tomato-engine-1.8.4/src/tomato/rules/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2022-05-23 23:00:31.000000 tomato-engine-1.8.4/src/tomato/rules/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      660 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/src/tomato/rules/colorful.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      273 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/src/tomato/rules/colorful_demo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      912 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/src/tomato/rules/cyclic.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      316 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/src/tomato/rules/cyclic_demo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      872 2023-05-04 22:48:21.000000 tomato-engine-1.8.4/src/tomato/rules/game_of_life.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      274 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/src/tomato/rules/game_of_life_demo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      759 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/src/tomato/rules/toothpick_fractal.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      297 2023-04-27 23:43:06.000000 tomato-engine-1.8.4/src/tomato/rules/toothpick_fractal_demo.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 12:32:31.950858 tomato-engine-1.8.4/src/tomato_engine.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3049 2023-05-09 12:32:31.000000 tomato-engine-1.8.4/src/tomato_engine.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      856 2023-05-09 12:32:31.000000 tomato-engine-1.8.4/src/tomato_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-09 12:32:31.000000 tomato-engine-1.8.4/src/tomato_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       53 2023-05-09 12:32:31.000000 tomato-engine-1.8.4/src/tomato_engine.egg-info/requires.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        7 2023-05-09 12:32:31.000000 tomato-engine-1.8.4/src/tomato_engine.egg-info/top_level.txt
```

### Comparing `tomato-engine-1.8.3/LICENSE` & `tomato-engine-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.3/PKG-INFO` & `tomato-engine-1.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomato-engine
-Version: 1.8.3
+Version: 1.8.4
 Summary: Engine for prototyping and playing with cellular automata
 Home-page: https://codeberg.org/eduardotogpi/tomato-engine
 Author: Eduardo Lopes Dias, Murilo Melhem
 Author-email: eduardosprp@usp.br
 Project-URL: Bug Tracker, https://codeberg.org/eduardotogpi/tomato-engine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `tomato-engine-1.8.3/README.md` & `tomato-engine-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.3/setup.cfg` & `tomato-engine-1.8.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tomato-engine
-version = 1.8.3
+version = 1.8.4
 author = Eduardo Lopes Dias, Murilo Melhem
 author_email = eduardotogpi@usp.br
 description = Engine for prototyping and playing with cellular automata.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://codeberg.org/eduardotogpi/tomato-engine
 project_urls =
```

### Comparing `tomato-engine-1.8.3/setup.py` & `tomato-engine-1.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tomato-engine",
-    version="1.8.3",
+    version="1.8.4",
     author="Eduardo Lopes Dias, Murilo Melhem",
     author_email="eduardosprp@usp.br",
     description="Engine for prototyping and playing with cellular automata",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://codeberg.org/eduardotogpi/tomato-engine",
     project_urls={
```

### Comparing `tomato-engine-1.8.3/src/tomato/classes/board.py` & `tomato-engine-1.8.4/src/tomato/classes/board.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.3/src/tomato/classes/cell.py` & `tomato-engine-1.8.4/src/tomato/classes/cell.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.3/src/tomato/classes/cellmatrix.py` & `tomato-engine-1.8.4/src/tomato/classes/cellmatrix.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.3/src/tomato/classes/window.py` & `tomato-engine-1.8.4/src/tomato/classes/window.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ..functions import display
-import pygame
 from time import time
 from numpy import mean, std
 
 from os import environ
 environ['PYGAME_HIDE_SUPPORT_PROMPT'] = '1'
+import pygame
 
 class Window:
 
     """
     Uma classe para ser a representação da janelinha da simulação
     no projeto. Sim, porque não temos overhead suficiente.
```

### Comparing `tomato-engine-1.8.3/src/tomato/functions/display.py` & `tomato-engine-1.8.4/src/tomato/functions/display.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.3/src/tomato/functions/file_io.py` & `tomato-engine-1.8.4/src/tomato/functions/file_io.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.3/src/tomato/functions/utils.py` & `tomato-engine-1.8.4/src/tomato/functions/utils.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.3/src/tomato/rules/colorful.py` & `tomato-engine-1.8.4/src/tomato/rules/colorful.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.3/src/tomato/rules/cyclic.py` & `tomato-engine-1.8.4/src/tomato/rules/cyclic.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.3/src/tomato/rules/game_of_life.py` & `tomato-engine-1.8.4/src/tomato/rules/game_of_life.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.3/src/tomato/rules/toothpick_fractal.py` & `tomato-engine-1.8.4/src/tomato/rules/toothpick_fractal.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.3/src/tomato_engine.egg-info/PKG-INFO` & `tomato-engine-1.8.4/src/tomato_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomato-engine
-Version: 1.8.3
+Version: 1.8.4
 Summary: Engine for prototyping and playing with cellular automata
 Home-page: https://codeberg.org/eduardotogpi/tomato-engine
 Author: Eduardo Lopes Dias, Murilo Melhem
 Author-email: eduardosprp@usp.br
 Project-URL: Bug Tracker, https://codeberg.org/eduardotogpi/tomato-engine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `tomato-engine-1.8.3/src/tomato_engine.egg-info/SOURCES.txt` & `tomato-engine-1.8.4/src/tomato_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

