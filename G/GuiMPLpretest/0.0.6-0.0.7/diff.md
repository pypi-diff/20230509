# Comparing `tmp/GuiMPLpretest-0.0.6.tar.gz` & `tmp/GuiMPLpretest-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GuiMPLpretest-0.0.6.tar", last modified: Tue May  9 20:52:32 2023, max compression
+gzip compressed data, was "GuiMPLpretest-0.0.7.tar", last modified: Tue May  9 20:56:48 2023, max compression
```

## Comparing `GuiMPLpretest-0.0.6.tar` & `GuiMPLpretest-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 20:52:32.722411 GuiMPLpretest-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-05-09 20:52:32.696800 GuiMPLpretest-0.0.6/GuiMPLpretest/
--rw-rw-rw-   0        0        0      123 2023-05-09 19:47:11.000000 GuiMPLpretest-0.0.6/GuiMPLpretest/__init__.py
--rw-rw-rw-   0        0        0      502 2023-05-09 19:38:14.000000 GuiMPLpretest-0.0.6/GuiMPLpretest/app.py
--rw-rw-rw-   0        0        0     6099 2023-05-09 19:43:18.000000 GuiMPLpretest-0.0.6/GuiMPLpretest/controller.py
--rw-rw-rw-   0        0        0     2098 2023-05-07 18:07:31.000000 GuiMPLpretest-0.0.6/GuiMPLpretest/dico_params.py
--rw-rw-rw-   0        0        0     3024 2023-05-09 14:32:19.000000 GuiMPLpretest-0.0.6/GuiMPLpretest/model.py
--rw-rw-rw-   0        0        0    16009 2023-05-09 20:48:22.000000 GuiMPLpretest-0.0.6/GuiMPLpretest/view.py
-drwxrwxrwx   0        0        0        0 2023-05-09 20:52:32.715965 GuiMPLpretest-0.0.6/GuiMPLpretest.egg-info/
--rw-rw-rw-   0        0        0      615 2023-05-09 20:52:32.000000 GuiMPLpretest-0.0.6/GuiMPLpretest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-05-09 20:52:32.000000 GuiMPLpretest-0.0.6/GuiMPLpretest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 20:52:32.000000 GuiMPLpretest-0.0.6/GuiMPLpretest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-09 20:52:32.000000 GuiMPLpretest-0.0.6/GuiMPLpretest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-09 20:52:32.000000 GuiMPLpretest-0.0.6/GuiMPLpretest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      615 2023-05-09 20:52:32.717954 GuiMPLpretest-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-09 20:52:32.722411 GuiMPLpretest-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1062 2023-05-09 20:52:29.000000 GuiMPLpretest-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 20:56:48.959137 GuiMPLpretest-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-05-09 20:56:48.936271 GuiMPLpretest-0.0.7/GuiMPLpretest/
+-rw-rw-rw-   0        0        0      123 2023-05-09 19:47:11.000000 GuiMPLpretest-0.0.7/GuiMPLpretest/__init__.py
+-rw-rw-rw-   0        0        0      502 2023-05-09 19:38:14.000000 GuiMPLpretest-0.0.7/GuiMPLpretest/app.py
+-rw-rw-rw-   0        0        0     6099 2023-05-09 19:43:18.000000 GuiMPLpretest-0.0.7/GuiMPLpretest/controller.py
+-rw-rw-rw-   0        0        0     2098 2023-05-07 18:07:31.000000 GuiMPLpretest-0.0.7/GuiMPLpretest/dico_params.py
+-rw-rw-rw-   0        0        0     3024 2023-05-09 14:32:19.000000 GuiMPLpretest-0.0.7/GuiMPLpretest/model.py
+-rw-rw-rw-   0        0        0    16009 2023-05-09 20:48:22.000000 GuiMPLpretest-0.0.7/GuiMPLpretest/view.py
+drwxrwxrwx   0        0        0        0 2023-05-09 20:56:48.957126 GuiMPLpretest-0.0.7/GuiMPLpretest.egg-info/
+-rw-rw-rw-   0        0        0      615 2023-05-09 20:56:48.000000 GuiMPLpretest-0.0.7/GuiMPLpretest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-05-09 20:56:48.000000 GuiMPLpretest-0.0.7/GuiMPLpretest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 20:56:48.000000 GuiMPLpretest-0.0.7/GuiMPLpretest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-09 20:56:48.000000 GuiMPLpretest-0.0.7/GuiMPLpretest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-09 20:56:48.000000 GuiMPLpretest-0.0.7/GuiMPLpretest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      615 2023-05-09 20:56:48.959137 GuiMPLpretest-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-09 20:56:48.960520 GuiMPLpretest-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1104 2023-05-09 20:56:33.000000 GuiMPLpretest-0.0.7/setup.py
```

### Comparing `GuiMPLpretest-0.0.6/GuiMPLpretest/controller.py` & `GuiMPLpretest-0.0.7/GuiMPLpretest/controller.py`

 * *Files identical despite different names*

### Comparing `GuiMPLpretest-0.0.6/GuiMPLpretest/dico_params.py` & `GuiMPLpretest-0.0.7/GuiMPLpretest/dico_params.py`

 * *Files identical despite different names*

### Comparing `GuiMPLpretest-0.0.6/GuiMPLpretest/model.py` & `GuiMPLpretest-0.0.7/GuiMPLpretest/model.py`

 * *Files identical despite different names*

### Comparing `GuiMPLpretest-0.0.6/GuiMPLpretest/view.py` & `GuiMPLpretest-0.0.7/GuiMPLpretest/view.py`

 * *Files identical despite different names*

### Comparing `GuiMPLpretest-0.0.6/GuiMPLpretest.egg-info/PKG-INFO` & `GuiMPLpretest-0.0.7/GuiMPLpretest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GuiMPLpretest
-Version: 0.0.6
+Version: 0.0.7
 Summary: Application pour modifier l'esthétique d'un graphique matplotlib
 Author: Groupe Figure MPCI
 Keywords: matplotlib,graphique,interface graphique,python,figures
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `GuiMPLpretest-0.0.6/PKG-INFO` & `GuiMPLpretest-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GuiMPLpretest
-Version: 0.0.6
+Version: 0.0.7
 Summary: Application pour modifier l'esthétique d'un graphique matplotlib
 Author: Groupe Figure MPCI
 Keywords: matplotlib,graphique,interface graphique,python,figures
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `GuiMPLpretest-0.0.6/setup.py` & `GuiMPLpretest-0.0.7/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 DESCRIPTION = "Application pour modifier l'esthétique d'un graphique matplotlib"
 LONG_DESCRIPTION = "Projet Figure S2 MPCI ayant pour but le développement d'une interface graphique permettant d'intéragir ergonomiquement avec des figures matplotlib"
 
 # Setting up
 setup(
     name="GuiMPLpretest",
     version=VERSION,
     author="Groupe Figure MPCI",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages()
-    + find_packages(where="./row_pygubu")
-    + find_packages(where="./surcouches_pygubu")
-    + find_packages(where="./custom_widgets"),
+    + find_packages(where="./GuiMPLpretest/row_pygubu")
+    + find_packages(where="./GuiMPLpretest/surcouches_pygubu")
+    + find_packages(where="./GuiMPLpretest/custom_widgets"),
     install_requires=["matplotlib"],
     keywords=["matplotlib", "graphique", "interface graphique", "python", "figures"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

