# Comparing `tmp/rmpy-0.1.3.tar.gz` & `tmp/rmpy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmpy-0.1.3.tar", last modified: Tue May  9 12:01:10 2023, max compression
+gzip compressed data, was "rmpy-1.1.1.tar", last modified: Tue May  9 12:22:11 2023, max compression
```

## Comparing `rmpy-0.1.3.tar` & `rmpy-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 12:01:10.732087 rmpy-0.1.3/
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 12:01:10.731422 rmpy-0.1.3/PKG-INFO
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56370 2023-05-08 13:29:14.000000 rmpy-0.1.3/README.md
-drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 12:01:10.727652 rmpy-0.1.3/rmpy/
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    97066 2023-05-08 12:10:58.000000 rmpy-0.1.3/rmpy/NpVaR.py
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    90889 2023-05-08 12:11:00.000000 rmpy-0.1.3/rmpy/PaVaR.py
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)     1140 2023-05-08 07:53:26.000000 rmpy-0.1.3/rmpy/__init__.py
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    33445 2023-05-09 11:54:33.000000 rmpy-0.1.3/rmpy/inputs_handler.py
-drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 12:01:10.730535 rmpy-0.1.3/rmpy.egg-info/
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 12:01:10.000000 rmpy-0.1.3/rmpy.egg-info/PKG-INFO
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)      225 2023-05-09 12:01:10.000000 rmpy-0.1.3/rmpy.egg-info/SOURCES.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)        1 2023-05-09 12:01:10.000000 rmpy-0.1.3/rmpy.egg-info/dependency_links.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)       28 2023-05-09 12:01:10.000000 rmpy-0.1.3/rmpy.egg-info/requires.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)        5 2023-05-09 12:01:10.000000 rmpy-0.1.3/rmpy.egg-info/top_level.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)       38 2023-05-09 12:01:10.732307 rmpy-0.1.3/setup.cfg
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)      861 2023-05-09 12:00:51.000000 rmpy-0.1.3/setup.py
+drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 12:22:11.053128 rmpy-1.1.1/
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 12:22:11.052410 rmpy-1.1.1/PKG-INFO
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56370 2023-05-08 13:29:14.000000 rmpy-1.1.1/README.md
+drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 12:22:11.048516 rmpy-1.1.1/rmpy/
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    97066 2023-05-08 12:10:58.000000 rmpy-1.1.1/rmpy/NpVaR.py
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    90889 2023-05-08 12:11:00.000000 rmpy-1.1.1/rmpy/PaVaR.py
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)     1140 2023-05-08 07:53:26.000000 rmpy-1.1.1/rmpy/__init__.py
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    33422 2023-05-09 12:21:10.000000 rmpy-1.1.1/rmpy/inputs_handler.py
+drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 12:22:11.051445 rmpy-1.1.1/rmpy.egg-info/
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 12:22:10.000000 rmpy-1.1.1/rmpy.egg-info/PKG-INFO
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)      225 2023-05-09 12:22:10.000000 rmpy-1.1.1/rmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)        1 2023-05-09 12:22:10.000000 rmpy-1.1.1/rmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)       28 2023-05-09 12:22:10.000000 rmpy-1.1.1/rmpy.egg-info/requires.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)        5 2023-05-09 12:22:10.000000 rmpy-1.1.1/rmpy.egg-info/top_level.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)       38 2023-05-09 12:22:11.053358 rmpy-1.1.1/setup.cfg
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)      861 2023-05-09 12:21:50.000000 rmpy-1.1.1/setup.py
```

### Comparing `rmpy-0.1.3/PKG-INFO` & `rmpy-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmpy
-Version: 0.1.3
+Version: 1.1.1
 Summary: This Python package provides a comprehensive set of tools for calculating and analyzing Non-Parametric and Parametric Value-at-Risk (NpVaR and pVaR).
 Home-page: https://github.com/GianMarcoOddo/rmpy
 Author: Gian Marco Oddo, Mattia Aprea, Sofia Compagnoni
 Author-email: gian.marco.oddo@usi.ch, mattia.aprea@usi.ch, sofia.compagnoni@usi.ch
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `rmpy-0.1.3/README.md` & `rmpy-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rmpy-0.1.3/rmpy/NpVaR.py` & `rmpy-1.1.1/rmpy/NpVaR.py`

 * *Files identical despite different names*

### Comparing `rmpy-0.1.3/rmpy/PaVaR.py` & `rmpy-1.1.1/rmpy/PaVaR.py`

 * *Files identical despite different names*

### Comparing `rmpy-0.1.3/rmpy/__init__.py` & `rmpy-1.1.1/rmpy/__init__.py`

 * *Files identical despite different names*

### Comparing `rmpy-0.1.3/rmpy/inputs_handler.py` & `rmpy-1.1.1/rmpy/inputs_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -669,15 +669,15 @@
             raise Exception("The array/list with the confidence_level parameter should contain only one value")
         dim = np.ndim(confidence_level)
         if dim > 1:
             raise Exception("The confidence_level array/list should be one-dimensional")
         confidence_level = confidence_level[0]
 
     # Handle if confidence_level is a number
-    if not isinstance(confidence_level, (float, np.int32, np.int64 , np.uint64, np.float16, np.float32, np.float64)):
+    if not isinstance(confidence_level, (float, np.int32, np.int64, np.float16, np.float32, np.float64)):
         raise TypeError("The confidence_level parameter must be a float number between 0 and 1")
 
     # Ensure the value of confidence_level is between 0 and 1
     if confidence_level > 1 or confidence_level < 0:
         raise Exception("Please, insert a correct value for confidence_level parameter! Between 0 and 1 (i.e for 95% insert 0.95)")
 
     return confidence_level
@@ -725,15 +725,15 @@
             raise Exception("The interval array/list should be one-dimensional")
         if len(interval) > 1:
             raise Exception("More than one interva provided")
         interval = interval[0]
         
 
     # Handle if interval is a number
-    if not isinstance(interval, (int, np.int32, np.int64 , np.uint64)):
+    if not isinstance(interval, (int, np.int32, np.int64 )):
         raise TypeError("The interval parameter must be an integer ")
 
     # Ensure the value of interval higher than one
     if interval < 1:
         raise Exception("Please, insert a correct value for interval parameter! > 1)")
 
     return interval
```

### Comparing `rmpy-0.1.3/rmpy.egg-info/PKG-INFO` & `rmpy-1.1.1/rmpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmpy
-Version: 0.1.3
+Version: 1.1.1
 Summary: This Python package provides a comprehensive set of tools for calculating and analyzing Non-Parametric and Parametric Value-at-Risk (NpVaR and pVaR).
 Home-page: https://github.com/GianMarcoOddo/rmpy
 Author: Gian Marco Oddo, Mattia Aprea, Sofia Compagnoni
 Author-email: gian.marco.oddo@usi.ch, mattia.aprea@usi.ch, sofia.compagnoni@usi.ch
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `rmpy-0.1.3/setup.py` & `rmpy-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Reading the content of the README.md file
 here = pathlib.Path(__file__).parent
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="rmpy",
-    version="0.1.3",
+    version="1.1.1",
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'yfinance',
         'scipy'],
     author="Gian Marco Oddo, Mattia Aprea, Sofia Compagnoni",
```

