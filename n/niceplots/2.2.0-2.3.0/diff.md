# Comparing `tmp/niceplots-2.2.0-py3-none-any.whl.zip` & `tmp/niceplots-2.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 16773 bytes, number of entries: 11
--rw-r--r--  2.0 unx       66 b- defN 23-Apr-19 23:28 niceplots/__init__.py
--rw-r--r--  2.0 unx     3452 b- defN 23-Apr-19 23:28 niceplots/parula.py
--rw-r--r--  2.0 unx    33254 b- defN 23-Apr-19 23:28 niceplots/utils.py
--rw-r--r--  2.0 unx     1146 b- defN 23-Apr-19 23:28 niceplots/styles/doumont-dark.mplstyle
--rw-r--r--  2.0 unx     1112 b- defN 23-Apr-19 23:28 niceplots/styles/doumont-light.mplstyle
--rw-r--r--  2.0 unx      909 b- defN 23-Apr-19 23:28 niceplots/styles/james-dark.mplstyle
--rw-r--r--  2.0 unx      904 b- defN 23-Apr-19 23:28 niceplots/styles/james-light.mplstyle
--rw-r--r--  2.0 unx     4485 b- defN 23-Apr-19 23:28 niceplots-2.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 23:28 niceplots-2.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-19 23:28 niceplots-2.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      910 b- defN 23-Apr-19 23:28 niceplots-2.2.0.dist-info/RECORD
-11 files, 46340 bytes uncompressed, 15227 bytes compressed:  67.1%
+Zip file size: 16859 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       66 b- defN 23-May-09 17:32 niceplots/__init__.py
+-rw-r--r--  2.0 unx     3452 b- defN 23-May-09 17:32 niceplots/parula.py
+-rw-r--r--  2.0 unx    34658 b- defN 23-May-09 17:32 niceplots/utils.py
+-rw-r--r--  2.0 unx     1146 b- defN 23-May-09 17:32 niceplots/styles/doumont-dark.mplstyle
+-rw-r--r--  2.0 unx     1112 b- defN 23-May-09 17:32 niceplots/styles/doumont-light.mplstyle
+-rw-r--r--  2.0 unx      909 b- defN 23-May-09 17:32 niceplots/styles/james-dark.mplstyle
+-rw-r--r--  2.0 unx      904 b- defN 23-May-09 17:32 niceplots/styles/james-light.mplstyle
+-rw-r--r--  2.0 unx     4485 b- defN 23-May-09 17:32 niceplots-2.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-09 17:32 niceplots-2.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-May-09 17:32 niceplots-2.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      910 b- defN 23-May-09 17:32 niceplots-2.3.0.dist-info/RECORD
+11 files, 47744 bytes uncompressed, 15313 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: niceplots/styles/james-dark.mplstyle
 Comment: 
 
 Filename: niceplots/styles/james-light.mplstyle
 Comment: 
 
-Filename: niceplots-2.2.0.dist-info/METADATA
+Filename: niceplots-2.3.0.dist-info/METADATA
 Comment: 
 
-Filename: niceplots-2.2.0.dist-info/WHEEL
+Filename: niceplots-2.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: niceplots-2.2.0.dist-info/top_level.txt
+Filename: niceplots-2.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: niceplots-2.2.0.dist-info/RECORD
+Filename: niceplots-2.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## niceplots/__init__.py

```diff
@@ -1,4 +1,4 @@
-__version__ = "2.2.0"
+__version__ = "2.3.0"
 
 from .utils import *
 from .parula import *
```

## niceplots/utils.py

```diff
@@ -49,61 +49,93 @@
         curDir = os.path.dirname(os.path.abspath(__file__))
         return os.path.join(curDir, "styles", styleName + ".mplstyle")
 
     # Otherwise assume it's a matplotlib style and just return the style name
     return styleName
 
 
-def get_colors():
+def get_colors(styleName=None):
     """
     Get a dictionary with the colors for the current style. This function
     only works when niceplots styles are used (not built-in matplotlib ones).
 
+    Parameters
+    ----------
+    styleName : str, optional
+        Name of desired style. By default gets the colors for the current style. Avaiable styles are:
+
+            - doumont-light: the niceplots style you know and love
+            - doumont-dark: the dark version of the niceplots style you know and love
+            - james-dark: a really cool alternative to classic niceplots
+            - james-light: a version of james with a light background, naturally
+
     Returns
     -------
     dict
         Dictionary of the colors for the requested style. The keys
         are human-readable names and the keys are the hex codes. It
         also adds color names from the rcParams that are generally useful:
 
             - "Axis": axis spine color
             - "Background" axis background color
             - "Text": default text color
             - "Label": axis label color
     """
-    # Get the color codes and their names from the (hopefully) "special" parameter
-    color_codes = get_colors_list()
-    color_names = plt.rcParams["keymap.help"]
-
-    # Ensure that the amount of color names matches the amount of colors
-    if len(color_codes) != len(color_names):
-        raise ValueError(
-            "The colors are not properly named in the stylesheet, please open an issue on GitHub with the details!"
-        )
-
-    colors = OrderedDict(zip(color_names, color_codes))
-    colors["Axis"] = plt.rcParams["axes.edgecolor"]
-    colors["Background"] = plt.rcParams["axes.facecolor"]
-    colors["Text"] = plt.rcParams["text.color"]
-    colors["Label"] = plt.rcParams["axes.labelcolor"]
 
-    return colors
+    def get_colors_from_current_style():
+        # Get the color codes and their names from the (hopefully) "special" parameter
+        color_codes = get_colors_list()
+        color_names = plt.rcParams["keymap.help"]
+
+        # Ensure that the amount of color names matches the amount of colors
+        if len(color_codes) != len(color_names):
+            raise ValueError(
+                "The colors are not properly named in the stylesheet, please open an issue on GitHub with the details!"
+            )
+
+        colors = OrderedDict(zip(color_names, color_codes))
+        colors["Axis"] = plt.rcParams["axes.edgecolor"]
+        colors["Background"] = plt.rcParams["axes.facecolor"]
+        colors["Text"] = plt.rcParams["text.color"]
+        colors["Label"] = plt.rcParams["axes.labelcolor"]
+
+        return colors
+
+    if styleName:
+        with plt.style.context(get_style(styleName)):
+            return get_colors_from_current_style()
+    else:
+        return get_colors_from_current_style()
 
 
-def get_colors_list():
+def get_colors_list(styleName=None):
     """
     Get a list with the colors for the current style. This function
     works with all matplotlib styles.
 
+    Parameters
+    ----------
+    styleName : str, optional
+        Name of desired style. By default gets the colors for the current style. Avaiable styles are:
+
+            - doumont-light: the niceplots style you know and love
+            - doumont-dark: the dark version of the niceplots style you know and love
+            - james-dark: a really cool alternative to classic niceplots
+            - james-light: a version of james with a light background, naturally
+
     Returns
     -------
     list
         List of the colors for the requested style.
     """
-    return plt.rcParams["axes.prop_cycle"].by_key()["color"]
+    if styleName:
+        with plt.style.context(get_style(styleName)):
+            return plt.rcParams["axes.prop_cycle"].by_key()["color"]
+    else:
+        return plt.rcParams["axes.prop_cycle"].by_key()["color"]
 
 
 def get_available_styles():
     """
     Get a list of the names of styles available.
 
     Returns
```

## Comparing `niceplots-2.2.0.dist-info/METADATA` & `niceplots-2.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niceplots
-Version: 2.2.0
+Version: 2.3.0
 Summary: Plotting utilities for matplotlib in python
 Home-page: https://github.com/mdolab/niceplots
 Author: 
 Author-email: 
 License: Apache License, Version 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

