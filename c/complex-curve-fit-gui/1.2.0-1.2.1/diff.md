# Comparing `tmp/complex_curve_fit_gui-1.2.0.tar.gz` & `tmp/complex_curve_fit_gui-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "complex_curve_fit_gui-1.2.0.tar", last modified: Mon May  8 22:33:38 2023, max compression
+gzip compressed data, was "complex_curve_fit_gui-1.2.1.tar", last modified: Mon May  8 23:55:17 2023, max compression
```

## Comparing `complex_curve_fit_gui-1.2.0.tar` & `complex_curve_fit_gui-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 22:33:38.846874 complex_curve_fit_gui-1.2.0/
--rw-r--r--   0 kojo       (501) staff       (20)       44 2023-04-24 04:46:49.000000 complex_curve_fit_gui-1.2.0/MANIFEST.in
--rw-r--r--   0 kojo       (501) staff       (20)    10116 2023-05-08 22:33:38.846971 complex_curve_fit_gui-1.2.0/PKG-INFO
--rw-r--r--   0 kojo       (501) staff       (20)     9657 2023-05-08 00:07:44.000000 complex_curve_fit_gui-1.2.0/README.md
--rw-rw-rw-   0 kojo       (501) staff       (20)       79 2023-05-08 22:33:38.847326 complex_curve_fit_gui-1.2.0/setup.cfg
--rw-rw-rw-   0 kojo       (501) staff       (20)     1231 2023-05-08 22:31:05.000000 complex_curve_fit_gui-1.2.0/setup.py
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 22:33:38.842882 complex_curve_fit_gui-1.2.0/src/
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 22:33:38.845746 complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui/
--rw-rw-rw-   0 kojo       (501) staff       (20)      181 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui/__init__.py
--rw-rw-rw-   0 kojo       (501) staff       (20)     7155 2023-04-27 04:39:20.000000 complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui/_curvefitgui.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    15968 2023-05-07 23:59:53.000000 complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui/_gui.py
--rw-rw-rw-   0 kojo       (501) staff       (20)     1539 2023-05-08 22:23:30.000000 complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui/_settings.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    16715 2023-05-07 23:22:42.000000 complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui/_tools.py
--rw-rw-rw-   0 kojo       (501) staff       (20)       22 2023-05-08 22:33:29.000000 complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui/_version.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    32342 2023-04-28 06:02:55.000000 complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui/_widgets.py
--rw-rw-rw-   0 kojo       (501) staff       (20)      879 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui/config.txt
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 22:33:38.846612 complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui.egg-info/
--rw-r--r--   0 kojo       (501) staff       (20)    10116 2023-05-08 22:33:38.000000 complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui.egg-info/PKG-INFO
--rw-r--r--   0 kojo       (501) staff       (20)      582 2023-05-08 22:33:38.000000 complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui.egg-info/SOURCES.txt
--rw-r--r--   0 kojo       (501) staff       (20)        1 2023-05-08 22:33:38.000000 complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui.egg-info/dependency_links.txt
--rw-r--r--   0 kojo       (501) staff       (20)       22 2023-05-08 22:33:38.000000 complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui.egg-info/top_level.txt
--rw-r--r--   0 kojo       (501) staff       (20)        1 2023-04-24 04:57:58.000000 complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui.egg-info/zip-safe
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 23:55:17.071100 complex_curve_fit_gui-1.2.1/
+-rw-r--r--   0 kojo       (501) staff       (20)       44 2023-04-24 04:46:49.000000 complex_curve_fit_gui-1.2.1/MANIFEST.in
+-rw-r--r--   0 kojo       (501) staff       (20)    10122 2023-05-08 23:55:17.071202 complex_curve_fit_gui-1.2.1/PKG-INFO
+-rw-r--r--   0 kojo       (501) staff       (20)     9663 2023-05-08 23:03:28.000000 complex_curve_fit_gui-1.2.1/README.md
+-rw-rw-rw-   0 kojo       (501) staff       (20)       79 2023-05-08 23:55:17.071526 complex_curve_fit_gui-1.2.1/setup.cfg
+-rw-rw-rw-   0 kojo       (501) staff       (20)     1231 2023-05-08 22:31:05.000000 complex_curve_fit_gui-1.2.1/setup.py
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 23:55:17.066967 complex_curve_fit_gui-1.2.1/src/
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 23:55:17.069963 complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui/
+-rw-rw-rw-   0 kojo       (501) staff       (20)      181 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui/__init__.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)     7155 2023-04-27 04:39:20.000000 complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui/_curvefitgui.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    15968 2023-05-07 23:59:53.000000 complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui/_gui.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)     1539 2023-05-08 22:23:30.000000 complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui/_settings.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    16715 2023-05-07 23:22:42.000000 complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui/_tools.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)       22 2023-05-08 23:55:12.000000 complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui/_version.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    32788 2023-05-08 23:48:33.000000 complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui/_widgets.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)      879 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui/config.txt
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 23:55:17.070855 complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui.egg-info/
+-rw-r--r--   0 kojo       (501) staff       (20)    10122 2023-05-08 23:55:17.000000 complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui.egg-info/PKG-INFO
+-rw-r--r--   0 kojo       (501) staff       (20)      582 2023-05-08 23:55:17.000000 complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 kojo       (501) staff       (20)        1 2023-05-08 23:55:17.000000 complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 kojo       (501) staff       (20)       22 2023-05-08 23:55:17.000000 complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui.egg-info/top_level.txt
+-rw-r--r--   0 kojo       (501) staff       (20)        1 2023-04-24 04:57:58.000000 complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui.egg-info/zip-safe
```

### Comparing `complex_curve_fit_gui-1.2.0/PKG-INFO` & `complex_curve_fit_gui-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: complex_curve_fit_gui
-Version: 1.2.0
+Version: 1.2.1
 Summary: GUI for lmfit using matplotlib
 Home-page: https://github.com/boakyeni/data-visualization-and-curve-fitting
 Author: Kojo Nimako
 Author-email: boakyeni@usc.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
 
 - Using `pip`:
 
       pip install numpy scipy matplotlib PyQt5 lmfit sympy
 
 - Using `conda` (required for M1 Mac):    
 
-      conda install numpy scipy matplotlib qtpy pyqt && conda install -c conda-forge lmfit
+      conda install numpy scipy matplotlib sympy qtpy pyqt && conda install -c conda-forge lmfit
 
 ### Getting Started
 1. If on MacOS M1 a conda environment will be needed
 2. import the gui:
        `from complex_curve_fit_gui import curve_fit_gui`
 3. define x and y data as 1 dimensional numpy arrays of equal length
        `xdata = np.array([1, 2, 3, 4, 5])`
```

### Comparing `complex_curve_fit_gui-1.2.0/README.md` & `complex_curve_fit_gui-1.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 - Using `pip`:
 
       pip install numpy scipy matplotlib PyQt5 lmfit sympy
 
 - Using `conda` (required for M1 Mac):    
 
-      conda install numpy scipy matplotlib qtpy pyqt && conda install -c conda-forge lmfit
+      conda install numpy scipy matplotlib sympy qtpy pyqt && conda install -c conda-forge lmfit
 
 ### Getting Started
 1. If on MacOS M1 a conda environment will be needed
 2. import the gui:
        `from complex_curve_fit_gui import curve_fit_gui`
 3. define x and y data as 1 dimensional numpy arrays of equal length
        `xdata = np.array([1, 2, 3, 4, 5])`
```

### Comparing `complex_curve_fit_gui-1.2.0/setup.py` & `complex_curve_fit_gui-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui/_curvefitgui.py` & `complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui/_curvefitgui.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui/_gui.py` & `complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui/_gui.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui/_settings.py` & `complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui/_settings.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui/_tools.py` & `complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui/_tools.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui/_widgets.py` & `complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui/_widgets.py`

 * *Files 3% similar despite different names*

```diff
@@ -686,56 +686,70 @@
                 # sort data if required
                 if settings["SORT_RESIDUALS"]:
                     order = np.argsort(self.fitter.data.y.real)
                 else:
                     order = np.arange(0, len(self.fitter.data.y.real))
 
                 data_copy = np.array([])
+                order_copy = []
                 for i in range(len(self.fitter.data.y)):
                     if self.fitter.data.mask[i] == True:
                         data_copy = np.append(
                             data_copy, [self.fitter.data.y.real[i]]
                         )
+                for i in range(len(self.fitter.data.y)):
+                    if self.fitter.data.mask[i] == True:
+                        order_copy.append(order[i])
+
                 self.residual_line.set_data(
-                    data_copy[order[: len(self.residuals)]],
-                    self.residuals.real[order[: len(self.residuals)]],
+                    self.fitter.data.y.real[order_copy[:]],
+                    self.residuals.real[order_copy[:]],
                 )
             self.ax1.legend()
         else:
             if self.residuals is not None:
                 # if the zero residual line is not yet created, do so
                 if self.zero_res is None:
                     self.ax2.axhline(y=0, linestyle="--", color="black")
 
                 # sort data if required
                 if settings["SORT_RESIDUALS"]:
                     order = np.argsort(self.fitter.data.x)
                 else:
                     order = np.arange(0, len(self.fitter.data.x))
+                # print("order", order)
                 # print("self.data.x", self.data.x, type(self.data.x))
                 # print("self.residuals", self.residuals, type(self.residuals))
                 # print("order slice", order[: len(self.residuals)], type(order))
                 # print("len of mask", len(self.data.mask), type(self.data.mask))
                 # print("self mask", self.data.mask)
 
                 """
                 Make a copy of data.x
                 iterate thru mask
                 if data.mask[i] is false then delete data.x[i] in the copy
                 use that copy in the residual line set data.
                 """
                 data_copy = np.array([])
+                # for range selection
+                order_copy = []
+
                 for i in range(len(self.fitter.data.x)):
                     if self.fitter.data.mask[i] == True:
                         data_copy = np.append(
                             data_copy, [self.fitter.data.x[i]]
                         )
+
+                for i in range(len(self.fitter.data.x)):
+                    if self.fitter.data.mask[i] == True:
+                        order_copy.append(order[i])
+
                 self.residual_line.set_data(
-                    data_copy[order[: len(self.residuals)]],
-                    self.residuals[order[: len(self.residuals)]],
+                    data_copy[order_copy[:]],
+                    self.residuals[order_copy[:]],
                 )
 
                 # self.residual_line.set_data(
                 #     self.data.x[order],
                 #     self.residuals[order[: len(self.residuals)]],
                 # )
```

### Comparing `complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui/config.txt` & `complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui/config.txt`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui.egg-info/PKG-INFO` & `complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: complex-curve-fit-gui
-Version: 1.2.0
+Version: 1.2.1
 Summary: GUI for lmfit using matplotlib
 Home-page: https://github.com/boakyeni/data-visualization-and-curve-fitting
 Author: Kojo Nimako
 Author-email: boakyeni@usc.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
 
 - Using `pip`:
 
       pip install numpy scipy matplotlib PyQt5 lmfit sympy
 
 - Using `conda` (required for M1 Mac):    
 
-      conda install numpy scipy matplotlib qtpy pyqt && conda install -c conda-forge lmfit
+      conda install numpy scipy matplotlib sympy qtpy pyqt && conda install -c conda-forge lmfit
 
 ### Getting Started
 1. If on MacOS M1 a conda environment will be needed
 2. import the gui:
        `from complex_curve_fit_gui import curve_fit_gui`
 3. define x and y data as 1 dimensional numpy arrays of equal length
        `xdata = np.array([1, 2, 3, 4, 5])`
```

### Comparing `complex_curve_fit_gui-1.2.0/src/complex_curve_fit_gui.egg-info/SOURCES.txt` & `complex_curve_fit_gui-1.2.1/src/complex_curve_fit_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

