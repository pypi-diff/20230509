# Comparing `tmp/rmpy-1.1.4.tar.gz` & `tmp/rmpy-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmpy-1.1.4.tar", last modified: Tue May  9 13:29:25 2023, max compression
+gzip compressed data, was "rmpy-1.1.5.tar", last modified: Tue May  9 13:33:56 2023, max compression
```

## Comparing `rmpy-1.1.4.tar` & `rmpy-1.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 13:29:25.424654 rmpy-1.1.4/
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 13:29:25.423952 rmpy-1.1.4/PKG-INFO
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56370 2023-05-08 13:29:14.000000 rmpy-1.1.4/README.md
-drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 13:29:25.420196 rmpy-1.1.4/rmpy/
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    97066 2023-05-09 13:27:47.000000 rmpy-1.1.4/rmpy/NpVaR.py
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    90889 2023-05-08 12:11:00.000000 rmpy-1.1.4/rmpy/PaVaR.py
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)     1140 2023-05-08 07:53:26.000000 rmpy-1.1.4/rmpy/__init__.py
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    33422 2023-05-09 12:56:32.000000 rmpy-1.1.4/rmpy/inputs_handler.py
-drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 13:29:25.423085 rmpy-1.1.4/rmpy.egg-info/
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 13:29:25.000000 rmpy-1.1.4/rmpy.egg-info/PKG-INFO
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)      225 2023-05-09 13:29:25.000000 rmpy-1.1.4/rmpy.egg-info/SOURCES.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)        1 2023-05-09 13:29:25.000000 rmpy-1.1.4/rmpy.egg-info/dependency_links.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)       28 2023-05-09 13:29:25.000000 rmpy-1.1.4/rmpy.egg-info/requires.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)        5 2023-05-09 13:29:25.000000 rmpy-1.1.4/rmpy.egg-info/top_level.txt
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)       38 2023-05-09 13:29:25.424875 rmpy-1.1.4/setup.cfg
--rw-r--r--   0 gianmarcooddo   (501) staff       (20)      861 2023-05-09 13:29:11.000000 rmpy-1.1.4/setup.py
+drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 13:33:56.861061 rmpy-1.1.5/
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 13:33:56.860378 rmpy-1.1.5/PKG-INFO
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56370 2023-05-08 13:29:14.000000 rmpy-1.1.5/README.md
+drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 13:33:56.856519 rmpy-1.1.5/rmpy/
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    97066 2023-05-09 13:27:47.000000 rmpy-1.1.5/rmpy/NpVaR.py
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    90889 2023-05-08 12:11:00.000000 rmpy-1.1.5/rmpy/PaVaR.py
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)     1140 2023-05-08 07:53:26.000000 rmpy-1.1.5/rmpy/__init__.py
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    33579 2023-05-09 13:33:24.000000 rmpy-1.1.5/rmpy/inputs_handler.py
+drwxr-xr-x   0 gianmarcooddo   (501) staff       (20)        0 2023-05-09 13:33:56.859413 rmpy-1.1.5/rmpy.egg-info/
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)    56819 2023-05-09 13:33:56.000000 rmpy-1.1.5/rmpy.egg-info/PKG-INFO
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)      225 2023-05-09 13:33:56.000000 rmpy-1.1.5/rmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)        1 2023-05-09 13:33:56.000000 rmpy-1.1.5/rmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)       28 2023-05-09 13:33:56.000000 rmpy-1.1.5/rmpy.egg-info/requires.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)        5 2023-05-09 13:33:56.000000 rmpy-1.1.5/rmpy.egg-info/top_level.txt
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)       38 2023-05-09 13:33:56.861206 rmpy-1.1.5/setup.cfg
+-rw-r--r--   0 gianmarcooddo   (501) staff       (20)      861 2023-05-09 13:33:50.000000 rmpy-1.1.5/setup.py
```

### Comparing `rmpy-1.1.4/PKG-INFO` & `rmpy-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmpy
-Version: 1.1.4
+Version: 1.1.5
 Summary: This Python package provides a comprehensive set of tools for calculating and analyzing Non-Parametric and Parametric Value-at-Risk (NpVaR and pVaR).
 Home-page: https://github.com/GianMarcoOddo/rmpy
 Author: Gian Marco Oddo, Mattia Aprea, Sofia Compagnoni
 Author-email: gian.marco.oddo@usi.ch, mattia.aprea@usi.ch, sofia.compagnoni@usi.ch
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `rmpy-1.1.4/README.md` & `rmpy-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `rmpy-1.1.4/rmpy/NpVaR.py` & `rmpy-1.1.5/rmpy/NpVaR.py`

 * *Files identical despite different names*

### Comparing `rmpy-1.1.4/rmpy/PaVaR.py` & `rmpy-1.1.5/rmpy/PaVaR.py`

 * *Files identical despite different names*

### Comparing `rmpy-1.1.4/rmpy/__init__.py` & `rmpy-1.1.5/rmpy/__init__.py`

 * *Files identical despite different names*

### Comparing `rmpy-1.1.4/rmpy/inputs_handler.py` & `rmpy-1.1.5/rmpy/inputs_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,14 +342,17 @@
     """
 
     # Convert to upper case
     tickers = [x.upper() for x in tickers]
 
     import pandas as pd ; import numpy as np
 
+    if isinstance(tickers, str):
+        raise TypeError("Tickers should be provided in the following object: [ np.ndarray, pd.core.series.Series, list ]")
+
     if isinstance(tickers, pd.DataFrame):
         raise TypeError("Tickers should be provided in the following object: [ np.ndarray, pd.core.series.Series, list ]")
     
     if isinstance(tickers, pd.Series):
 
         tickers = tickers.tolist()
```

### Comparing `rmpy-1.1.4/rmpy.egg-info/PKG-INFO` & `rmpy-1.1.5/rmpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmpy
-Version: 1.1.4
+Version: 1.1.5
 Summary: This Python package provides a comprehensive set of tools for calculating and analyzing Non-Parametric and Parametric Value-at-Risk (NpVaR and pVaR).
 Home-page: https://github.com/GianMarcoOddo/rmpy
 Author: Gian Marco Oddo, Mattia Aprea, Sofia Compagnoni
 Author-email: gian.marco.oddo@usi.ch, mattia.aprea@usi.ch, sofia.compagnoni@usi.ch
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `rmpy-1.1.4/setup.py` & `rmpy-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Reading the content of the README.md file
 here = pathlib.Path(__file__).parent
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="rmpy",
-    version="1.1.4",
+    version="1.1.5",
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'yfinance',
         'scipy'],
     author="Gian Marco Oddo, Mattia Aprea, Sofia Compagnoni",
```

