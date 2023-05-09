# Comparing `tmp/pysmithplot_fork-0.2.0.tar.gz` & `tmp/pysmithplot_fork-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysmithplot_fork-0.2.0.tar", last modified: Wed Jul 24 16:06:24 2019, max compression
+gzip compressed data, was "pysmithplot_fork-0.2.1.tar", last modified: Tue May  9 12:13:46 2023, max compression
```

## Comparing `pysmithplot_fork-0.2.0.tar` & `pysmithplot_fork-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2019-07-24 16:06:24.000000 pysmithplot_fork-0.2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4933 2019-07-24 16:06:24.000000 pysmithplot_fork-0.2.0/PKG-INFO
--rwxr-xr-x   0 sergey    (1000) sergey    (1000)     4026 2019-07-24 15:56:36.000000 pysmithplot_fork-0.2.0/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2019-07-24 16:06:24.000000 pysmithplot_fork-0.2.0/pysmithplot_fork.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4933 2019-07-24 16:06:24.000000 pysmithplot_fork-0.2.0/pysmithplot_fork.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      287 2019-07-24 16:06:24.000000 pysmithplot_fork-0.2.0/pysmithplot_fork.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2019-07-24 16:06:24.000000 pysmithplot_fork-0.2.0/pysmithplot_fork.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       30 2019-07-24 16:06:24.000000 pysmithplot_fork-0.2.0/pysmithplot_fork.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       10 2019-07-24 16:06:24.000000 pysmithplot_fork-0.2.0/pysmithplot_fork.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2019-07-24 16:06:24.000000 pysmithplot_fork-0.2.0/setup.cfg
--rwxr-xr-x   0 sergey    (1000) sergey    (1000)      593 2019-07-24 16:05:55.000000 pysmithplot_fork-0.2.0/setup.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2019-07-24 16:06:24.000000 pysmithplot_fork-0.2.0/smithplot/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      365 2019-07-24 15:56:36.000000 pysmithplot_fork-0.2.0/smithplot/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    61284 2019-07-24 15:56:36.000000 pysmithplot_fork-0.2.0/smithplot/smithaxes.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1403 2019-07-24 15:56:36.000000 pysmithplot_fork-0.2.0/smithplot/smithhelper.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 12:13:46.886782 pysmithplot_fork-0.2.1/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4318 2023-05-09 12:13:46.886782 pysmithplot_fork-0.2.1/PKG-INFO
+-rwxr-xr-x   0 sergey    (1000) sergey    (1000)     4026 2019-07-24 15:56:36.000000 pysmithplot_fork-0.2.1/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 12:13:46.886782 pysmithplot_fork-0.2.1/pysmithplot_fork.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4318 2023-05-09 12:13:46.000000 pysmithplot_fork-0.2.1/pysmithplot_fork.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      287 2023-05-09 12:13:46.000000 pysmithplot_fork-0.2.1/pysmithplot_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-05-09 12:13:46.000000 pysmithplot_fork-0.2.1/pysmithplot_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       30 2023-05-09 12:13:46.000000 pysmithplot_fork-0.2.1/pysmithplot_fork.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       10 2023-05-09 12:13:46.000000 pysmithplot_fork-0.2.1/pysmithplot_fork.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2023-05-09 12:13:46.886782 pysmithplot_fork-0.2.1/setup.cfg
+-rwxr-xr-x   0 sergey    (1000) sergey    (1000)      593 2023-05-09 12:13:20.000000 pysmithplot_fork-0.2.1/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-09 12:13:46.886782 pysmithplot_fork-0.2.1/smithplot/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      365 2019-07-24 15:56:36.000000 pysmithplot_fork-0.2.1/smithplot/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    61365 2023-05-09 12:12:58.000000 pysmithplot_fork-0.2.1/smithplot/smithaxes.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1476 2023-05-09 12:12:58.000000 pysmithplot_fork-0.2.1/smithplot/smithhelper.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pysmithplot_fork-0.2.0/PKG-INFO` & `pysmithplot_fork-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,82 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: pysmithplot_fork
-Version: 0.2.0
+Version: 0.2.1
 Summary: An extension for Matplotlib providing a projection class to generate high quality Smith Chart plots.
 Home-page: https://github.com/vMeijin/pySmithPlot
 Author: Paul Staerke
 Author-email: paul.staerke@gmail.com
 License: BSD
-Description: pySmithPlot
-        ===========
-        
-        ## New Release of Version 0.2
-        
-        After 2 years of getting dusty **pySmithPlot** now got some new features and bug fixes. Here is a short changelog:
-        
-        - **Support for Python 3**
-        - improved grid generation algorithm
-        - plot() now also handles also single numbers and purely real data
-        - plot() can now interpolate lines between points or generate an equidistant spacing
-        - changed handling of input data and renormalization; now the actual datatype (S,Z,Y-Parameter) can be specified when calling plot()
-        - changed behaviour for normalization and placement of the label
-        - added some parameter checks 
-        - removed default `matplotlib` settings
-        - renamed some parameters to improve consistency 
-        - fixed issues with Unicode symbols
-        - fixed issues with grid generation
-        - fixed issues with axis label display and placement
-        
-        There are still some plans for the future and they hopefully don't take another two years:
-        
-        - [ ] support for Admittance Charts
-        - [ ] support for `contour()` plots
-        - [ ] zoom and 'cut out' function
-        - [ ] special handling of other `matplotlib.patch` objects like arrows
-        - [ ] ...
-        
-        ## Features
-        
-        **pySmithPlot** is a matplotlib extension providing a projection class for creating high quality Smith Charts with Python. The generated plots blend seamless into matplotlib's style and support almost the full range of customization options. 
-        
-        This Library allows the fully automatic generation of Smith Charts with various customizable parameters and well selected default values. It also provides the following modifications and extensions:
-        
-        - circle shaped drawing area with labels placed around 
-        - plot() accepts real and complex numbers as well as numpy.ndarray's
-        - lines can be automatically interpolated to improve the optical appearance 
-        - data ranges can be interpolated to an equidistant spacing
-        - start/end markers of lines can be modified and rotate tangential
-        - gridlines are 3-point arcs to improve space efficiency of exported plots
-        - 'fancy' option for adaptive grid generation
-        - own tick locators for nice axis labels
-        
-        For making a Smith Chart plot, it is sufficient to `import smithplot` and create a new subplot with projection set to 'smith'. (Requires matplotlib version 1.2)
-        
-        A short example can be found in the `testbenches` directory and started with:
-        
-            python3 smith_short_test.py
-            
-        For more details and documentation, take a look into `smithplot/smithaxes.py`. 
-        
-        `testbenches/smith_full_test.py` runs various testbenches and gives a comparison for almost all parameters. These are the generated sample plots: 
-        
-        ![Grid Styles](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_grid_styles.png)
-        [Grid Styles - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_grid_styles.pdf)
-        
-        ![Fancy Threshold](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_fancy_grid.png)
-        [Fancy Threshold - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_fancy_grid.pdf)
-        
-        ![Grid Locators](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_grid_locators.png)
-        [Grid Locators - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_grid_locators.pdf)
-        
-        ![Marker Modification](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_markers.png)
-        [Marker Modification - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_markers.pdf)
-        
-        ![Interpolation](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_interpolation.png)
-        [Interpolation - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_interpolation.pdf)
-        
-        ![Normalize](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_normalize.png)
-        [Normalize - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_normalize.pdf)
-        
-        ![Miscellaneous](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_miscellaneous.png)
-        [Miscellaneous - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_miscellaneous.pdf)
-        
-Platform: UNKNOWN
+
+pySmithPlot
+===========
+
+## New Release of Version 0.2
+
+After 2 years of getting dusty **pySmithPlot** now got some new features and bug fixes. Here is a short changelog:
+
+- **Support for Python 3**
+- improved grid generation algorithm
+- plot() now also handles also single numbers and purely real data
+- plot() can now interpolate lines between points or generate an equidistant spacing
+- changed handling of input data and renormalization; now the actual datatype (S,Z,Y-Parameter) can be specified when calling plot()
+- changed behaviour for normalization and placement of the label
+- added some parameter checks 
+- removed default `matplotlib` settings
+- renamed some parameters to improve consistency 
+- fixed issues with Unicode symbols
+- fixed issues with grid generation
+- fixed issues with axis label display and placement
+
+There are still some plans for the future and they hopefully don't take another two years:
+
+- [ ] support for Admittance Charts
+- [ ] support for `contour()` plots
+- [ ] zoom and 'cut out' function
+- [ ] special handling of other `matplotlib.patch` objects like arrows
+- [ ] ...
+
+## Features
+
+**pySmithPlot** is a matplotlib extension providing a projection class for creating high quality Smith Charts with Python. The generated plots blend seamless into matplotlib's style and support almost the full range of customization options. 
+
+This Library allows the fully automatic generation of Smith Charts with various customizable parameters and well selected default values. It also provides the following modifications and extensions:
+
+- circle shaped drawing area with labels placed around 
+- plot() accepts real and complex numbers as well as numpy.ndarray's
+- lines can be automatically interpolated to improve the optical appearance 
+- data ranges can be interpolated to an equidistant spacing
+- start/end markers of lines can be modified and rotate tangential
+- gridlines are 3-point arcs to improve space efficiency of exported plots
+- 'fancy' option for adaptive grid generation
+- own tick locators for nice axis labels
+
+For making a Smith Chart plot, it is sufficient to `import smithplot` and create a new subplot with projection set to 'smith'. (Requires matplotlib version 1.2)
+
+A short example can be found in the `testbenches` directory and started with:
+
+    python3 smith_short_test.py
+    
+For more details and documentation, take a look into `smithplot/smithaxes.py`. 
+
+`testbenches/smith_full_test.py` runs various testbenches and gives a comparison for almost all parameters. These are the generated sample plots: 
+
+![Grid Styles](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_grid_styles.png)
+[Grid Styles - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_grid_styles.pdf)
+
+![Fancy Threshold](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_fancy_grid.png)
+[Fancy Threshold - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_fancy_grid.pdf)
+
+![Grid Locators](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_grid_locators.png)
+[Grid Locators - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_grid_locators.pdf)
+
+![Marker Modification](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_markers.png)
+[Marker Modification - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_markers.pdf)
+
+![Interpolation](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_interpolation.png)
+[Interpolation - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_interpolation.pdf)
+
+![Normalize](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_normalize.png)
+[Normalize - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_normalize.pdf)
+
+![Miscellaneous](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_miscellaneous.png)
+[Miscellaneous - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_miscellaneous.pdf)
```

### Comparing `pysmithplot_fork-0.2.0/README.md` & `pysmithplot_fork-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pysmithplot_fork-0.2.0/pysmithplot_fork.egg-info/PKG-INFO` & `pysmithplot_fork-0.2.1/pysmithplot_fork.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,82 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: pysmithplot-fork
-Version: 0.2.0
+Version: 0.2.1
 Summary: An extension for Matplotlib providing a projection class to generate high quality Smith Chart plots.
 Home-page: https://github.com/vMeijin/pySmithPlot
 Author: Paul Staerke
 Author-email: paul.staerke@gmail.com
 License: BSD
-Description: pySmithPlot
-        ===========
-        
-        ## New Release of Version 0.2
-        
-        After 2 years of getting dusty **pySmithPlot** now got some new features and bug fixes. Here is a short changelog:
-        
-        - **Support for Python 3**
-        - improved grid generation algorithm
-        - plot() now also handles also single numbers and purely real data
-        - plot() can now interpolate lines between points or generate an equidistant spacing
-        - changed handling of input data and renormalization; now the actual datatype (S,Z,Y-Parameter) can be specified when calling plot()
-        - changed behaviour for normalization and placement of the label
-        - added some parameter checks 
-        - removed default `matplotlib` settings
-        - renamed some parameters to improve consistency 
-        - fixed issues with Unicode symbols
-        - fixed issues with grid generation
-        - fixed issues with axis label display and placement
-        
-        There are still some plans for the future and they hopefully don't take another two years:
-        
-        - [ ] support for Admittance Charts
-        - [ ] support for `contour()` plots
-        - [ ] zoom and 'cut out' function
-        - [ ] special handling of other `matplotlib.patch` objects like arrows
-        - [ ] ...
-        
-        ## Features
-        
-        **pySmithPlot** is a matplotlib extension providing a projection class for creating high quality Smith Charts with Python. The generated plots blend seamless into matplotlib's style and support almost the full range of customization options. 
-        
-        This Library allows the fully automatic generation of Smith Charts with various customizable parameters and well selected default values. It also provides the following modifications and extensions:
-        
-        - circle shaped drawing area with labels placed around 
-        - plot() accepts real and complex numbers as well as numpy.ndarray's
-        - lines can be automatically interpolated to improve the optical appearance 
-        - data ranges can be interpolated to an equidistant spacing
-        - start/end markers of lines can be modified and rotate tangential
-        - gridlines are 3-point arcs to improve space efficiency of exported plots
-        - 'fancy' option for adaptive grid generation
-        - own tick locators for nice axis labels
-        
-        For making a Smith Chart plot, it is sufficient to `import smithplot` and create a new subplot with projection set to 'smith'. (Requires matplotlib version 1.2)
-        
-        A short example can be found in the `testbenches` directory and started with:
-        
-            python3 smith_short_test.py
-            
-        For more details and documentation, take a look into `smithplot/smithaxes.py`. 
-        
-        `testbenches/smith_full_test.py` runs various testbenches and gives a comparison for almost all parameters. These are the generated sample plots: 
-        
-        ![Grid Styles](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_grid_styles.png)
-        [Grid Styles - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_grid_styles.pdf)
-        
-        ![Fancy Threshold](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_fancy_grid.png)
-        [Fancy Threshold - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_fancy_grid.pdf)
-        
-        ![Grid Locators](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_grid_locators.png)
-        [Grid Locators - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_grid_locators.pdf)
-        
-        ![Marker Modification](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_markers.png)
-        [Marker Modification - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_markers.pdf)
-        
-        ![Interpolation](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_interpolation.png)
-        [Interpolation - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_interpolation.pdf)
-        
-        ![Normalize](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_normalize.png)
-        [Normalize - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_normalize.pdf)
-        
-        ![Miscellaneous](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_miscellaneous.png)
-        [Miscellaneous - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_miscellaneous.pdf)
-        
-Platform: UNKNOWN
+
+pySmithPlot
+===========
+
+## New Release of Version 0.2
+
+After 2 years of getting dusty **pySmithPlot** now got some new features and bug fixes. Here is a short changelog:
+
+- **Support for Python 3**
+- improved grid generation algorithm
+- plot() now also handles also single numbers and purely real data
+- plot() can now interpolate lines between points or generate an equidistant spacing
+- changed handling of input data and renormalization; now the actual datatype (S,Z,Y-Parameter) can be specified when calling plot()
+- changed behaviour for normalization and placement of the label
+- added some parameter checks 
+- removed default `matplotlib` settings
+- renamed some parameters to improve consistency 
+- fixed issues with Unicode symbols
+- fixed issues with grid generation
+- fixed issues with axis label display and placement
+
+There are still some plans for the future and they hopefully don't take another two years:
+
+- [ ] support for Admittance Charts
+- [ ] support for `contour()` plots
+- [ ] zoom and 'cut out' function
+- [ ] special handling of other `matplotlib.patch` objects like arrows
+- [ ] ...
+
+## Features
+
+**pySmithPlot** is a matplotlib extension providing a projection class for creating high quality Smith Charts with Python. The generated plots blend seamless into matplotlib's style and support almost the full range of customization options. 
+
+This Library allows the fully automatic generation of Smith Charts with various customizable parameters and well selected default values. It also provides the following modifications and extensions:
+
+- circle shaped drawing area with labels placed around 
+- plot() accepts real and complex numbers as well as numpy.ndarray's
+- lines can be automatically interpolated to improve the optical appearance 
+- data ranges can be interpolated to an equidistant spacing
+- start/end markers of lines can be modified and rotate tangential
+- gridlines are 3-point arcs to improve space efficiency of exported plots
+- 'fancy' option for adaptive grid generation
+- own tick locators for nice axis labels
+
+For making a Smith Chart plot, it is sufficient to `import smithplot` and create a new subplot with projection set to 'smith'. (Requires matplotlib version 1.2)
+
+A short example can be found in the `testbenches` directory and started with:
+
+    python3 smith_short_test.py
+    
+For more details and documentation, take a look into `smithplot/smithaxes.py`. 
+
+`testbenches/smith_full_test.py` runs various testbenches and gives a comparison for almost all parameters. These are the generated sample plots: 
+
+![Grid Styles](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_grid_styles.png)
+[Grid Styles - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_grid_styles.pdf)
+
+![Fancy Threshold](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_fancy_grid.png)
+[Fancy Threshold - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_fancy_grid.pdf)
+
+![Grid Locators](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_grid_locators.png)
+[Grid Locators - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_grid_locators.pdf)
+
+![Marker Modification](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_markers.png)
+[Marker Modification - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_markers.pdf)
+
+![Interpolation](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_interpolation.png)
+[Interpolation - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_interpolation.pdf)
+
+![Normalize](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_normalize.png)
+[Normalize - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_normalize.pdf)
+
+![Miscellaneous](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_miscellaneous.png)
+[Miscellaneous - PDF](https://github.com/vMeijin/pySmithPlot/wiki/images/examples/sample_miscellaneous.pdf)
```

### Comparing `pysmithplot_fork-0.2.0/setup.py` & `pysmithplot_fork-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(name="pysmithplot_fork",
-      version="0.2.0",
+      version="0.2.1",
       packages=["smithplot"],
       description="An extension for Matplotlib providing a projection class to generate high quality Smith Chart plots.",
       long_description=read('README.md'),
       author="Paul Staerke",
       author_email="paul.staerke@gmail.com",
       license="BSD",
       url="https://github.com/vMeijin/pySmithPlot",
```

### Comparing `pysmithplot_fork-0.2.0/smithplot/smithaxes.py` & `pysmithplot_fork-0.2.1/smithplot/smithaxes.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,16 +31,18 @@
     pp.show()
     
 Note: Supplying parameters to :meth:`subplot` may not always work as
 expected, because subplot uses an index for the axes with a key created
 of all given parameters. This does not work always, especially if the
 parameters are array-like types (e.g. numpy.ndarray).
 '''
-
-from collections import Iterable
+try:
+    from collections import Iterable
+except ImportError:
+    from collections.abc import Iterable
 from numbers import Number
 from types import MethodType, FunctionType
 
 import matplotlib as mp
 import numpy as np
 from matplotlib.axes import Axes
 from matplotlib.axis import XAxis
@@ -1057,19 +1059,19 @@
                         x0, x1 = xticks[i:i + 2]
 
                         for k in range(len_y):
                             y0, y1 = yticks[k:k + 2]
 
                             x_div, y_div = d_mat[i, k]
 
-                            for xs in np.linspace(x0, x1, x_div + 1)[1:]:
+                            for xs in np.linspace(x0, x1, int(x_div) + 1)[1:]:
                                 x_lines.append([xs, y0, y1])
                                 x_lines.append([xs, -y1, -y0])
 
-                            for ys in np.linspace(y0, y1, y_div + 1)[1:]:
+                            for ys in np.linspace(y0, y1, int(y_div) + 1)[1:]:
                                 y_lines.append([ys, x0, x1])
                                 y_lines.append([-ys, x0, x1])
 
                     # round values to prevent float inaccuarcy
                     x_lines = np.round(np.array(x_lines), 7)
                     y_lines = np.round(np.array(y_lines), 7)
```

### Comparing `pysmithplot_fork-0.2.0/smithplot/smithhelper.py` & `pysmithplot_fork-0.2.1/smithplot/smithhelper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # -*- coding: utf-8 -*-
 # last edit: 11.04.2018
 
-from collections import Iterable
+try:
+    from collections import Iterable
+except ImportError:
+    from collections.abc import Iterable
 
 import numpy as np
 
 INF = 1e9
 EPSILON = 1e-7
 TWO_PI = 2 * np.pi
```

