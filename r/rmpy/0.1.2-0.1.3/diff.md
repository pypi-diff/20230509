# Comparing `tmp/rmpy-0.1.2.tar.gz` & `tmp/rmpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmpy-0.1.2.tar", last modified: Tue May  9 11:55:49 2023, max compression
+gzip compressed data, was "rmpy-0.1.3.tar", last modified: Tue May  9 12:01:10 2023, max compression
```

## Comparing `rmpy-0.1.2.tar` & `rmpy-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 11:55:49.308261 rmpy-0.1.2/
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 11:55:49.307622 rmpy-0.1.2/PKG-INFO
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56370 2023-05-08 13:29:14.000000 rmpy-0.1.2/README.md
-drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 11:55:49.303532 rmpy-0.1.2/rmpy/
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    97066 2023-05-08 12:10:58.000000 rmpy-0.1.2/rmpy/NpVaR.py
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    90889 2023-05-08 12:11:00.000000 rmpy-0.1.2/rmpy/PaVaR.py
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)     1140 2023-05-08 07:53:26.000000 rmpy-0.1.2/rmpy/__init__.py
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    33445 2023-05-09 11:54:33.000000 rmpy-0.1.2/rmpy/inputs_handler.py
-drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 11:55:49.306740 rmpy-0.1.2/rmpy.egg-info/
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 11:55:49.000000 rmpy-0.1.2/rmpy.egg-info/PKG-INFO
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)      225 2023-05-09 11:55:49.000000 rmpy-0.1.2/rmpy.egg-info/SOURCES.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)        1 2023-05-09 11:55:49.000000 rmpy-0.1.2/rmpy.egg-info/dependency_links.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)       28 2023-05-09 11:55:49.000000 rmpy-0.1.2/rmpy.egg-info/requires.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)        5 2023-05-09 11:55:49.000000 rmpy-0.1.2/rmpy.egg-info/top_level.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)       38 2023-05-09 11:55:49.308432 rmpy-0.1.2/setup.cfg
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)      861 2023-05-09 11:55:15.000000 rmpy-0.1.2/setup.py
+drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 12:01:10.732087 rmpy-0.1.3/
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 12:01:10.731422 rmpy-0.1.3/PKG-INFO
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56370 2023-05-08 13:29:14.000000 rmpy-0.1.3/README.md
+drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 12:01:10.727652 rmpy-0.1.3/rmpy/
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    97066 2023-05-08 12:10:58.000000 rmpy-0.1.3/rmpy/NpVaR.py
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    90889 2023-05-08 12:11:00.000000 rmpy-0.1.3/rmpy/PaVaR.py
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)     1140 2023-05-08 07:53:26.000000 rmpy-0.1.3/rmpy/__init__.py
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    33445 2023-05-09 11:54:33.000000 rmpy-0.1.3/rmpy/inputs_handler.py
+drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 12:01:10.730535 rmpy-0.1.3/rmpy.egg-info/
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 12:01:10.000000 rmpy-0.1.3/rmpy.egg-info/PKG-INFO
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)      225 2023-05-09 12:01:10.000000 rmpy-0.1.3/rmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)        1 2023-05-09 12:01:10.000000 rmpy-0.1.3/rmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)       28 2023-05-09 12:01:10.000000 rmpy-0.1.3/rmpy.egg-info/requires.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)        5 2023-05-09 12:01:10.000000 rmpy-0.1.3/rmpy.egg-info/top_level.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)       38 2023-05-09 12:01:10.732307 rmpy-0.1.3/setup.cfg
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)      861 2023-05-09 12:00:51.000000 rmpy-0.1.3/setup.py
```

### Comparing `rmpy-0.1.2/PKG-INFO` & `rmpy-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: This Python package provides a comprehensive set of tools for calculating and analyzing Non-Parametric and Parametric Value-at-Risk (NpVaR and pVaR).
 Home-page: https://github.com/GianMarcoOddo/rmpy
 Author: Gian Marco Oddo, Mattia Aprea, Sofia Compagnoni
 Author-email: gian.marco.oddo@usi.ch, mattia.aprea@usi.ch, sofia.compagnoni@usi.ch
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `rmpy-0.1.2/README.md` & `rmpy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `rmpy-0.1.2/rmpy/NpVaR.py` & `rmpy-0.1.3/rmpy/NpVaR.py`

 * *Files identical despite different names*

### Comparing `rmpy-0.1.2/rmpy/PaVaR.py` & `rmpy-0.1.3/rmpy/PaVaR.py`

 * *Files identical despite different names*

### Comparing `rmpy-0.1.2/rmpy/__init__.py` & `rmpy-0.1.3/rmpy/__init__.py`

 * *Files identical despite different names*

### Comparing `rmpy-0.1.2/rmpy/inputs_handler.py` & `rmpy-0.1.3/rmpy/inputs_handler.py`

 * *Files identical despite different names*

### Comparing `rmpy-0.1.2/rmpy.egg-info/PKG-INFO` & `rmpy-0.1.3/rmpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: This Python package provides a comprehensive set of tools for calculating and analyzing Non-Parametric and Parametric Value-at-Risk (NpVaR and pVaR).
 Home-page: https://github.com/GianMarcoOddo/rmpy
 Author: Gian Marco Oddo, Mattia Aprea, Sofia Compagnoni
 Author-email: gian.marco.oddo@usi.ch, mattia.aprea@usi.ch, sofia.compagnoni@usi.ch
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `rmpy-0.1.2/setup.py` & `rmpy-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Reading the content of the README.md file
 here = pathlib.Path(__file__).parent
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="rmpy",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'yfinance',
         'scipy'],
     author="Gian Marco Oddo, Mattia Aprea, Sofia Compagnoni",
```

