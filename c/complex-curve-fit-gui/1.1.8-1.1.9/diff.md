# Comparing `tmp/complex_curve_fit_gui-1.1.8.tar.gz` & `tmp/complex_curve_fit_gui-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "complex_curve_fit_gui-1.1.8.tar", last modified: Mon May  8 22:00:36 2023, max compression
+gzip compressed data, was "complex_curve_fit_gui-1.1.9.tar", last modified: Mon May  8 22:24:02 2023, max compression
```

## Comparing `complex_curve_fit_gui-1.1.8.tar` & `complex_curve_fit_gui-1.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 22:00:36.775564 complex_curve_fit_gui-1.1.8/
--rw-r--r--   0 kojo       (501) staff       (20)       44 2023-04-24 04:46:49.000000 complex_curve_fit_gui-1.1.8/MANIFEST.in
--rw-r--r--   0 kojo       (501) staff       (20)    10116 2023-05-08 22:00:36.775651 complex_curve_fit_gui-1.1.8/PKG-INFO
--rw-r--r--   0 kojo       (501) staff       (20)     9657 2023-05-08 00:07:44.000000 complex_curve_fit_gui-1.1.8/README.md
--rw-rw-rw-   0 kojo       (501) staff       (20)       79 2023-05-08 22:00:36.775973 complex_curve_fit_gui-1.1.8/setup.cfg
--rw-rw-rw-   0 kojo       (501) staff       (20)     1309 2023-05-08 21:59:59.000000 complex_curve_fit_gui-1.1.8/setup.py
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 22:00:36.771594 complex_curve_fit_gui-1.1.8/src/
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 22:00:36.774563 complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui/
--rw-rw-rw-   0 kojo       (501) staff       (20)      181 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui/__init__.py
--rw-rw-rw-   0 kojo       (501) staff       (20)     7155 2023-04-27 04:39:20.000000 complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui/_curvefitgui.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    15968 2023-05-07 23:59:53.000000 complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui/_gui.py
--rw-rw-rw-   0 kojo       (501) staff       (20)     1529 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui/_settings.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    16715 2023-05-07 23:22:42.000000 complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui/_tools.py
--rw-rw-rw-   0 kojo       (501) staff       (20)       22 2023-05-08 22:00:21.000000 complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui/_version.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    32342 2023-04-28 06:02:55.000000 complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui/_widgets.py
--rw-rw-rw-   0 kojo       (501) staff       (20)      879 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui/config.txt
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 22:00:36.775323 complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui.egg-info/
--rw-r--r--   0 kojo       (501) staff       (20)    10116 2023-05-08 22:00:36.000000 complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui.egg-info/PKG-INFO
--rw-r--r--   0 kojo       (501) staff       (20)      582 2023-05-08 22:00:36.000000 complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui.egg-info/SOURCES.txt
--rw-r--r--   0 kojo       (501) staff       (20)        1 2023-05-08 22:00:36.000000 complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui.egg-info/dependency_links.txt
--rw-r--r--   0 kojo       (501) staff       (20)       22 2023-05-08 22:00:36.000000 complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui.egg-info/top_level.txt
--rw-r--r--   0 kojo       (501) staff       (20)        1 2023-04-24 04:57:58.000000 complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui.egg-info/zip-safe
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 22:24:02.655381 complex_curve_fit_gui-1.1.9/
+-rw-r--r--   0 kojo       (501) staff       (20)       44 2023-04-24 04:46:49.000000 complex_curve_fit_gui-1.1.9/MANIFEST.in
+-rw-r--r--   0 kojo       (501) staff       (20)    10116 2023-05-08 22:24:02.655478 complex_curve_fit_gui-1.1.9/PKG-INFO
+-rw-r--r--   0 kojo       (501) staff       (20)     9657 2023-05-08 00:07:44.000000 complex_curve_fit_gui-1.1.9/README.md
+-rw-rw-rw-   0 kojo       (501) staff       (20)       79 2023-05-08 22:24:02.655824 complex_curve_fit_gui-1.1.9/setup.cfg
+-rw-rw-rw-   0 kojo       (501) staff       (20)     1309 2023-05-08 21:59:59.000000 complex_curve_fit_gui-1.1.9/setup.py
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 22:24:02.651157 complex_curve_fit_gui-1.1.9/src/
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 22:24:02.654280 complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui/
+-rw-rw-rw-   0 kojo       (501) staff       (20)      181 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui/__init__.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)     7155 2023-04-27 04:39:20.000000 complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui/_curvefitgui.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    15968 2023-05-07 23:59:53.000000 complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui/_gui.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)     1539 2023-05-08 22:23:30.000000 complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui/_settings.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    16715 2023-05-07 23:22:42.000000 complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui/_tools.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)       22 2023-05-08 22:23:59.000000 complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui/_version.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    32342 2023-04-28 06:02:55.000000 complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui/_widgets.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)      879 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui/config.txt
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 22:24:02.655130 complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui.egg-info/
+-rw-r--r--   0 kojo       (501) staff       (20)    10116 2023-05-08 22:24:02.000000 complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui.egg-info/PKG-INFO
+-rw-r--r--   0 kojo       (501) staff       (20)      582 2023-05-08 22:24:02.000000 complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 kojo       (501) staff       (20)        1 2023-05-08 22:24:02.000000 complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 kojo       (501) staff       (20)       22 2023-05-08 22:24:02.000000 complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui.egg-info/top_level.txt
+-rw-r--r--   0 kojo       (501) staff       (20)        1 2023-04-24 04:57:58.000000 complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui.egg-info/zip-safe
```

### Comparing `complex_curve_fit_gui-1.1.8/PKG-INFO` & `complex_curve_fit_gui-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: complex_curve_fit_gui
-Version: 1.1.8
+Version: 1.1.9
 Summary: GUI for lmfit using matplotlib
 Home-page: https://github.com/boakyeni/data-visualization-and-curve-fitting
 Author: Kojo Nimako
 Author-email: boakyeni@usc.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `complex_curve_fit_gui-1.1.8/README.md` & `complex_curve_fit_gui-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.8/setup.py` & `complex_curve_fit_gui-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui/_curvefitgui.py` & `complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui/_curvefitgui.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui/_gui.py` & `complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui/_gui.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui/_settings.py` & `complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui/_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from importlib import resources as _resources
 import configparser
 
 
 _config = configparser.ConfigParser()
-with _resources.path("curvefitgui", "config.txt") as _path:
+with _resources.path("complex_curve_fit_gui", "config.txt") as _path:
     _config.read(str(_path))
 
 settings = {}
 
 # general
 settings['MODEL_NUMPOINTS'] = int(_config['general']['numpoints'])
 settings['SIGNIFICANT_DIGITS'] = int(_config['general']['significant_digits'])
```

### Comparing `complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui/_tools.py` & `complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui/_tools.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui/_widgets.py` & `complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui/_widgets.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui/config.txt` & `complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui/config.txt`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui.egg-info/PKG-INFO` & `complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: complex-curve-fit-gui
-Version: 1.1.8
+Version: 1.1.9
 Summary: GUI for lmfit using matplotlib
 Home-page: https://github.com/boakyeni/data-visualization-and-curve-fitting
 Author: Kojo Nimako
 Author-email: boakyeni@usc.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `complex_curve_fit_gui-1.1.8/src/complex_curve_fit_gui.egg-info/SOURCES.txt` & `complex_curve_fit_gui-1.1.9/src/complex_curve_fit_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

