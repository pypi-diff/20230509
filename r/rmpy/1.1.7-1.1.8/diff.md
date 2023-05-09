# Comparing `tmp/rmpy-1.1.7.tar.gz` & `tmp/rmpy-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmpy-1.1.7.tar", last modified: Tue May  9 14:44:08 2023, max compression
+gzip compressed data, was "rmpy-1.1.8.tar", last modified: Tue May  9 14:49:03 2023, max compression
```

## Comparing `rmpy-1.1.7.tar` & `rmpy-1.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 14:44:08.965677 rmpy-1.1.7/
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 14:44:08.965051 rmpy-1.1.7/PKG-INFO
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56370 2023-05-08 13:29:14.000000 rmpy-1.1.7/README.md
-drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 14:44:08.960543 rmpy-1.1.7/rmpy/
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    97066 2023-05-09 13:27:47.000000 rmpy-1.1.7/rmpy/NpVaR.py
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    90889 2023-05-08 12:11:00.000000 rmpy-1.1.7/rmpy/PaVaR.py
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)     1140 2023-05-09 14:39:31.000000 rmpy-1.1.7/rmpy/__init__.py
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    33335 2023-05-09 14:38:44.000000 rmpy-1.1.7/rmpy/inputs_handler.py
-drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 14:44:08.964310 rmpy-1.1.7/rmpy.egg-info/
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 14:44:08.000000 rmpy-1.1.7/rmpy.egg-info/PKG-INFO
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)      225 2023-05-09 14:44:08.000000 rmpy-1.1.7/rmpy.egg-info/SOURCES.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)        1 2023-05-09 14:44:08.000000 rmpy-1.1.7/rmpy.egg-info/dependency_links.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)       28 2023-05-09 14:44:08.000000 rmpy-1.1.7/rmpy.egg-info/requires.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)        5 2023-05-09 14:44:08.000000 rmpy-1.1.7/rmpy.egg-info/top_level.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)       38 2023-05-09 14:44:08.965890 rmpy-1.1.7/setup.cfg
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)      861 2023-05-09 14:43:43.000000 rmpy-1.1.7/setup.py
+drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 14:49:03.797381 rmpy-1.1.8/
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 14:49:03.796905 rmpy-1.1.8/PKG-INFO
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56370 2023-05-08 13:29:14.000000 rmpy-1.1.8/README.md
+drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 14:49:03.793138 rmpy-1.1.8/rmpy/
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    97066 2023-05-09 13:27:47.000000 rmpy-1.1.8/rmpy/NpVaR.py
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    90889 2023-05-08 12:11:00.000000 rmpy-1.1.8/rmpy/PaVaR.py
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)     1140 2023-05-09 14:39:31.000000 rmpy-1.1.8/rmpy/__init__.py
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    33335 2023-05-09 14:48:25.000000 rmpy-1.1.8/rmpy/inputs_handler.py
+drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 14:49:03.796276 rmpy-1.1.8/rmpy.egg-info/
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 14:49:03.000000 rmpy-1.1.8/rmpy.egg-info/PKG-INFO
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)      225 2023-05-09 14:49:03.000000 rmpy-1.1.8/rmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)        1 2023-05-09 14:49:03.000000 rmpy-1.1.8/rmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)       28 2023-05-09 14:49:03.000000 rmpy-1.1.8/rmpy.egg-info/requires.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)        5 2023-05-09 14:49:03.000000 rmpy-1.1.8/rmpy.egg-info/top_level.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)       38 2023-05-09 14:49:03.797559 rmpy-1.1.8/setup.cfg
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)      861 2023-05-09 14:48:35.000000 rmpy-1.1.8/setup.py
```

### Comparing `rmpy-1.1.7/PKG-INFO` & `rmpy-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmpy
-Version: 1.1.7
+Version: 1.1.8
 Summary: This Python package provides a comprehensive set of tools for calculating and analyzing Non-Parametric and Parametric Value-at-Risk (NpVaR and pVaR).
 Home-page: https://github.com/GianMarcoOddo/rmpy
 Author: Gian Marco Oddo, Mattia Aprea, Sofia Compagnoni
 Author-email: gian.marco.oddo@usi.ch, mattia.aprea@usi.ch, sofia.compagnoni@usi.ch
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `rmpy-1.1.7/README.md` & `rmpy-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `rmpy-1.1.7/rmpy/NpVaR.py` & `rmpy-1.1.8/rmpy/NpVaR.py`

 * *Files identical despite different names*

### Comparing `rmpy-1.1.7/rmpy/PaVaR.py` & `rmpy-1.1.8/rmpy/PaVaR.py`

 * *Files identical despite different names*

### Comparing `rmpy-1.1.7/rmpy/__init__.py` & `rmpy-1.1.8/rmpy/__init__.py`

 * *Files identical despite different names*

### Comparing `rmpy-1.1.7/rmpy/inputs_handler.py` & `rmpy-1.1.8/rmpy/inputs_handler.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -337,22 +337,22 @@
     TypeError: If the tickers are provided in a pandas dataframe.
     Exception: If the tickers are an empty list, array, or series.
     Exception: If the tickers array or list is multidimensional.
     Exception: If only one ticker or a non-string type is provided.
     ValueError: If there are duplicate tickers in the list or array.
     """
 
+    import pandas as pd ; import numpy as np
+
     if not isinstance(tickers, (list, np.ndarray, pd.Series)):
         raise TypeError("Tickers should be provided in the following object: [ np.ndarray, pd.core.series.Series, list ]")
 
     # Convert to upper case
     tickers = [x.upper() for x in tickers]
 
-    import pandas as pd ; import numpy as np
-
     if isinstance(tickers, pd.Series):
         tickers = list(tickers)
         if len(tickers) == 0:
             raise Exception("The Series with the tickers is empty")
 
     if isinstance(tickers, np.ndarray):
         if len(tickers) == 0:
```

### Comparing `rmpy-1.1.7/rmpy.egg-info/PKG-INFO` & `rmpy-1.1.8/rmpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmpy
-Version: 1.1.7
+Version: 1.1.8
 Summary: This Python package provides a comprehensive set of tools for calculating and analyzing Non-Parametric and Parametric Value-at-Risk (NpVaR and pVaR).
 Home-page: https://github.com/GianMarcoOddo/rmpy
 Author: Gian Marco Oddo, Mattia Aprea, Sofia Compagnoni
 Author-email: gian.marco.oddo@usi.ch, mattia.aprea@usi.ch, sofia.compagnoni@usi.ch
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `rmpy-1.1.7/setup.py` & `rmpy-1.1.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Reading the content of the README.md file
 here = pathlib.Path(__file__).parent
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="rmpy",
-    version="1.1.7",
+    version="1.1.8",
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'yfinance',
         'scipy'],
     author="Gian Marco Oddo, Mattia Aprea, Sofia Compagnoni",
```

