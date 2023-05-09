# Comparing `tmp/GuiMPLpretest-0.0.2.tar.gz` & `tmp/GuiMPLpretest-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GuiMPLpretest-0.0.2.tar", last modified: Tue May  9 19:40:55 2023, max compression
+gzip compressed data, was "GuiMPLpretest-0.0.3.tar", last modified: Tue May  9 19:44:36 2023, max compression
```

## Comparing `GuiMPLpretest-0.0.2.tar` & `GuiMPLpretest-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 19:40:55.071757 GuiMPLpretest-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-05-09 19:40:55.042382 GuiMPLpretest-0.0.2/GuiMPLpretest/
--rw-rw-rw-   0        0        0      147 2023-05-09 17:12:05.000000 GuiMPLpretest-0.0.2/GuiMPLpretest/__init__.py
--rw-rw-rw-   0        0        0      502 2023-05-09 19:38:14.000000 GuiMPLpretest-0.0.2/GuiMPLpretest/app.py
--rw-rw-rw-   0        0        0     6071 2023-05-09 19:38:12.000000 GuiMPLpretest-0.0.2/GuiMPLpretest/controller.py
--rw-rw-rw-   0        0        0     2098 2023-05-07 18:07:31.000000 GuiMPLpretest-0.0.2/GuiMPLpretest/dico_params.py
--rw-rw-rw-   0        0        0     3024 2023-05-09 14:32:19.000000 GuiMPLpretest-0.0.2/GuiMPLpretest/model.py
--rw-rw-rw-   0        0        0    15997 2023-05-09 19:38:42.000000 GuiMPLpretest-0.0.2/GuiMPLpretest/view.py
-drwxrwxrwx   0        0        0        0 2023-05-09 19:40:55.066770 GuiMPLpretest-0.0.2/GuiMPLpretest.egg-info/
--rw-rw-rw-   0        0        0      615 2023-05-09 19:40:54.000000 GuiMPLpretest-0.0.2/GuiMPLpretest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-05-09 19:40:54.000000 GuiMPLpretest-0.0.2/GuiMPLpretest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 19:40:54.000000 GuiMPLpretest-0.0.2/GuiMPLpretest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-09 19:40:54.000000 GuiMPLpretest-0.0.2/GuiMPLpretest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-09 19:40:54.000000 GuiMPLpretest-0.0.2/GuiMPLpretest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      615 2023-05-09 19:40:55.070753 GuiMPLpretest-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-09 19:40:55.072754 GuiMPLpretest-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      922 2023-05-09 19:40:30.000000 GuiMPLpretest-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:44:36.351820 GuiMPLpretest-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-05-09 19:44:36.327887 GuiMPLpretest-0.0.3/GuiMPLpretest/
+-rw-rw-rw-   0        0        0      147 2023-05-09 17:12:05.000000 GuiMPLpretest-0.0.3/GuiMPLpretest/__init__.py
+-rw-rw-rw-   0        0        0      502 2023-05-09 19:38:14.000000 GuiMPLpretest-0.0.3/GuiMPLpretest/app.py
+-rw-rw-rw-   0        0        0     6099 2023-05-09 19:43:18.000000 GuiMPLpretest-0.0.3/GuiMPLpretest/controller.py
+-rw-rw-rw-   0        0        0     2098 2023-05-07 18:07:31.000000 GuiMPLpretest-0.0.3/GuiMPLpretest/dico_params.py
+-rw-rw-rw-   0        0        0     3024 2023-05-09 14:32:19.000000 GuiMPLpretest-0.0.3/GuiMPLpretest/model.py
+-rw-rw-rw-   0        0        0    15997 2023-05-09 19:38:42.000000 GuiMPLpretest-0.0.3/GuiMPLpretest/view.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:44:36.349866 GuiMPLpretest-0.0.3/GuiMPLpretest.egg-info/
+-rw-rw-rw-   0        0        0      615 2023-05-09 19:44:36.000000 GuiMPLpretest-0.0.3/GuiMPLpretest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-05-09 19:44:36.000000 GuiMPLpretest-0.0.3/GuiMPLpretest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 19:44:36.000000 GuiMPLpretest-0.0.3/GuiMPLpretest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-09 19:44:36.000000 GuiMPLpretest-0.0.3/GuiMPLpretest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-09 19:44:36.000000 GuiMPLpretest-0.0.3/GuiMPLpretest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      615 2023-05-09 19:44:36.350821 GuiMPLpretest-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-09 19:44:36.351820 GuiMPLpretest-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      922 2023-05-09 19:44:28.000000 GuiMPLpretest-0.0.3/setup.py
```

### Comparing `GuiMPLpretest-0.0.2/GuiMPLpretest/controller.py` & `GuiMPLpretest-0.0.3/GuiMPLpretest/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from view import View
-from model import Model
 from tkinter import filedialog
 import os
 import pickle
 from matplotlib.figure import Figure
 
+from GuiMPLpretest.view import View
+from GuiMPLpretest.model import Model
 from GuiMPLpretest.dico_params import dico_param_figure, dico_param_axe, dico_param_line
 
 
 class Controller:
     def __init__(self, fig: Figure = None, fig_file_name: str = None):
         self.model = Model()
         self.view = View(self)
```

### Comparing `GuiMPLpretest-0.0.2/GuiMPLpretest/dico_params.py` & `GuiMPLpretest-0.0.3/GuiMPLpretest/dico_params.py`

 * *Files identical despite different names*

### Comparing `GuiMPLpretest-0.0.2/GuiMPLpretest/model.py` & `GuiMPLpretest-0.0.3/GuiMPLpretest/model.py`

 * *Files identical despite different names*

### Comparing `GuiMPLpretest-0.0.2/GuiMPLpretest/view.py` & `GuiMPLpretest-0.0.3/GuiMPLpretest/view.py`

 * *Files identical despite different names*

### Comparing `GuiMPLpretest-0.0.2/GuiMPLpretest.egg-info/PKG-INFO` & `GuiMPLpretest-0.0.3/GuiMPLpretest.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GuiMPLpretest
-Version: 0.0.2
+Version: 0.0.3
 Summary: Application pour modifier l'esthétique d'un graphique matplotlib
 Author: Groupe Figure MPCI
 Keywords: matplotlib,graphique,interface graphique,python,figures
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `GuiMPLpretest-0.0.2/PKG-INFO` & `GuiMPLpretest-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GuiMPLpretest
-Version: 0.0.2
+Version: 0.0.3
 Summary: Application pour modifier l'esthétique d'un graphique matplotlib
 Author: Groupe Figure MPCI
 Keywords: matplotlib,graphique,interface graphique,python,figures
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `GuiMPLpretest-0.0.2/setup.py` & `GuiMPLpretest-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = "Application pour modifier l'esthétique d'un graphique matplotlib"
 LONG_DESCRIPTION = "Projet Figure S2 MPCI ayant pour but le développement d'une interface graphique permettant d'intéragir ergonomiquement avec des figures matplotlib"
 
 # Setting up
 setup(
     name="GuiMPLpretest",
     version=VERSION,
```

