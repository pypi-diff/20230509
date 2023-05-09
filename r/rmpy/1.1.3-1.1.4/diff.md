# Comparing `tmp/rmpy-1.1.3.tar.gz` & `tmp/rmpy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmpy-1.1.3.tar", last modified: Tue May  9 12:44:49 2023, max compression
+gzip compressed data, was "rmpy-1.1.4.tar", last modified: Tue May  9 13:29:25 2023, max compression
```

## Comparing `rmpy-1.1.3.tar` & `rmpy-1.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 12:44:49.720558 rmpy-1.1.3/
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 12:44:49.719881 rmpy-1.1.3/PKG-INFO
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56370 2023-05-08 13:29:14.000000 rmpy-1.1.3/README.md
-drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 12:44:49.714122 rmpy-1.1.3/rmpy/
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    97066 2023-05-08 12:10:58.000000 rmpy-1.1.3/rmpy/NpVaR.py
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    90889 2023-05-08 12:11:00.000000 rmpy-1.1.3/rmpy/PaVaR.py
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)     1140 2023-05-08 07:53:26.000000 rmpy-1.1.3/rmpy/__init__.py
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    33422 2023-05-09 12:21:10.000000 rmpy-1.1.3/rmpy/inputs_handler.py
-drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 12:44:49.718989 rmpy-1.1.3/rmpy.egg-info/
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 12:44:49.000000 rmpy-1.1.3/rmpy.egg-info/PKG-INFO
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)      225 2023-05-09 12:44:49.000000 rmpy-1.1.3/rmpy.egg-info/SOURCES.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)        1 2023-05-09 12:44:49.000000 rmpy-1.1.3/rmpy.egg-info/dependency_links.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)       28 2023-05-09 12:44:49.000000 rmpy-1.1.3/rmpy.egg-info/requires.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)        5 2023-05-09 12:44:49.000000 rmpy-1.1.3/rmpy.egg-info/top_level.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)       38 2023-05-09 12:44:49.720851 rmpy-1.1.3/setup.cfg
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)      861 2023-05-09 12:43:04.000000 rmpy-1.1.3/setup.py
+drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 13:29:25.424654 rmpy-1.1.4/
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 13:29:25.423952 rmpy-1.1.4/PKG-INFO
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56370 2023-05-08 13:29:14.000000 rmpy-1.1.4/README.md
+drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 13:29:25.420196 rmpy-1.1.4/rmpy/
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    97066 2023-05-09 13:27:47.000000 rmpy-1.1.4/rmpy/NpVaR.py
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    90889 2023-05-08 12:11:00.000000 rmpy-1.1.4/rmpy/PaVaR.py
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)     1140 2023-05-08 07:53:26.000000 rmpy-1.1.4/rmpy/__init__.py
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    33422 2023-05-09 12:56:32.000000 rmpy-1.1.4/rmpy/inputs_handler.py
+drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 13:29:25.423085 rmpy-1.1.4/rmpy.egg-info/
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 13:29:25.000000 rmpy-1.1.4/rmpy.egg-info/PKG-INFO
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)      225 2023-05-09 13:29:25.000000 rmpy-1.1.4/rmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)        1 2023-05-09 13:29:25.000000 rmpy-1.1.4/rmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)       28 2023-05-09 13:29:25.000000 rmpy-1.1.4/rmpy.egg-info/requires.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)        5 2023-05-09 13:29:25.000000 rmpy-1.1.4/rmpy.egg-info/top_level.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)       38 2023-05-09 13:29:25.424875 rmpy-1.1.4/setup.cfg
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)      861 2023-05-09 13:29:11.000000 rmpy-1.1.4/setup.py
```

### Comparing `rmpy-1.1.3/PKG-INFO` & `rmpy-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmpy
-Version: 1.1.3
+Version: 1.1.4
 Summary: This Python package provides a comprehensive set of tools for calculating and analyzing Non-Parametric and Parametric Value-at-Risk (NpVaR and pVaR).
 Home-page: https://github.com/GianMarcoOddo/rmpy
 Author: Gian Marco Oddo, Mattia Aprea, Sofia Compagnoni
 Author-email: gian.marco.oddo@usi.ch, mattia.aprea@usi.ch, sofia.compagnoni@usi.ch
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `rmpy-1.1.3/README.md` & `rmpy-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `rmpy-1.1.3/rmpy/NpVaR.py` & `rmpy-1.1.4/rmpy/NpVaR.py`

 * *Files identical despite different names*

### Comparing `rmpy-1.1.3/rmpy/PaVaR.py` & `rmpy-1.1.4/rmpy/PaVaR.py`

 * *Files identical despite different names*

### Comparing `rmpy-1.1.3/rmpy/__init__.py` & `rmpy-1.1.4/rmpy/__init__.py`

 * *Files identical despite different names*

### Comparing `rmpy-1.1.3/rmpy/inputs_handler.py` & `rmpy-1.1.4/rmpy/inputs_handler.py`

 * *Files identical despite different names*

### Comparing `rmpy-1.1.3/rmpy.egg-info/PKG-INFO` & `rmpy-1.1.4/rmpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmpy
-Version: 1.1.3
+Version: 1.1.4
 Summary: This Python package provides a comprehensive set of tools for calculating and analyzing Non-Parametric and Parametric Value-at-Risk (NpVaR and pVaR).
 Home-page: https://github.com/GianMarcoOddo/rmpy
 Author: Gian Marco Oddo, Mattia Aprea, Sofia Compagnoni
 Author-email: gian.marco.oddo@usi.ch, mattia.aprea@usi.ch, sofia.compagnoni@usi.ch
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `rmpy-1.1.3/setup.py` & `rmpy-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Reading the content of the README.md file
 here = pathlib.Path(__file__).parent
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="rmpy",
-    version="1.1.3",
+    version="1.1.4",
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'yfinance',
         'scipy'],
     author="Gian Marco Oddo, Mattia Aprea, Sofia Compagnoni",
```

