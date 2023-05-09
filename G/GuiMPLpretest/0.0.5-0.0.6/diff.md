# Comparing `tmp/GuiMPLpretest-0.0.5.tar.gz` & `tmp/GuiMPLpretest-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GuiMPLpretest-0.0.5.tar", last modified: Tue May  9 19:57:19 2023, max compression
+gzip compressed data, was "GuiMPLpretest-0.0.6.tar", last modified: Tue May  9 20:52:32 2023, max compression
```

## Comparing `GuiMPLpretest-0.0.5.tar` & `GuiMPLpretest-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 19:57:19.513163 GuiMPLpretest-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-05-09 19:57:19.489308 GuiMPLpretest-0.0.5/GuiMPLpretest/
--rw-rw-rw-   0        0        0      123 2023-05-09 19:47:11.000000 GuiMPLpretest-0.0.5/GuiMPLpretest/__init__.py
--rw-rw-rw-   0        0        0      502 2023-05-09 19:38:14.000000 GuiMPLpretest-0.0.5/GuiMPLpretest/app.py
--rw-rw-rw-   0        0        0     6099 2023-05-09 19:43:18.000000 GuiMPLpretest-0.0.5/GuiMPLpretest/controller.py
--rw-rw-rw-   0        0        0     2098 2023-05-07 18:07:31.000000 GuiMPLpretest-0.0.5/GuiMPLpretest/dico_params.py
--rw-rw-rw-   0        0        0     3024 2023-05-09 14:32:19.000000 GuiMPLpretest-0.0.5/GuiMPLpretest/model.py
--rw-rw-rw-   0        0        0    15946 2023-05-09 19:56:39.000000 GuiMPLpretest-0.0.5/GuiMPLpretest/view.py
-drwxrwxrwx   0        0        0        0 2023-05-09 19:57:19.509168 GuiMPLpretest-0.0.5/GuiMPLpretest.egg-info/
--rw-rw-rw-   0        0        0      615 2023-05-09 19:57:19.000000 GuiMPLpretest-0.0.5/GuiMPLpretest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-05-09 19:57:19.000000 GuiMPLpretest-0.0.5/GuiMPLpretest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 19:57:19.000000 GuiMPLpretest-0.0.5/GuiMPLpretest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-09 19:57:19.000000 GuiMPLpretest-0.0.5/GuiMPLpretest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-09 19:57:19.000000 GuiMPLpretest-0.0.5/GuiMPLpretest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      615 2023-05-09 19:57:19.510165 GuiMPLpretest-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-09 19:57:19.513163 GuiMPLpretest-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      922 2023-05-09 19:56:51.000000 GuiMPLpretest-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 20:52:32.722411 GuiMPLpretest-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-05-09 20:52:32.696800 GuiMPLpretest-0.0.6/GuiMPLpretest/
+-rw-rw-rw-   0        0        0      123 2023-05-09 19:47:11.000000 GuiMPLpretest-0.0.6/GuiMPLpretest/__init__.py
+-rw-rw-rw-   0        0        0      502 2023-05-09 19:38:14.000000 GuiMPLpretest-0.0.6/GuiMPLpretest/app.py
+-rw-rw-rw-   0        0        0     6099 2023-05-09 19:43:18.000000 GuiMPLpretest-0.0.6/GuiMPLpretest/controller.py
+-rw-rw-rw-   0        0        0     2098 2023-05-07 18:07:31.000000 GuiMPLpretest-0.0.6/GuiMPLpretest/dico_params.py
+-rw-rw-rw-   0        0        0     3024 2023-05-09 14:32:19.000000 GuiMPLpretest-0.0.6/GuiMPLpretest/model.py
+-rw-rw-rw-   0        0        0    16009 2023-05-09 20:48:22.000000 GuiMPLpretest-0.0.6/GuiMPLpretest/view.py
+drwxrwxrwx   0        0        0        0 2023-05-09 20:52:32.715965 GuiMPLpretest-0.0.6/GuiMPLpretest.egg-info/
+-rw-rw-rw-   0        0        0      615 2023-05-09 20:52:32.000000 GuiMPLpretest-0.0.6/GuiMPLpretest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-05-09 20:52:32.000000 GuiMPLpretest-0.0.6/GuiMPLpretest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 20:52:32.000000 GuiMPLpretest-0.0.6/GuiMPLpretest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-09 20:52:32.000000 GuiMPLpretest-0.0.6/GuiMPLpretest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-09 20:52:32.000000 GuiMPLpretest-0.0.6/GuiMPLpretest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      615 2023-05-09 20:52:32.717954 GuiMPLpretest-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-09 20:52:32.722411 GuiMPLpretest-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1062 2023-05-09 20:52:29.000000 GuiMPLpretest-0.0.6/setup.py
```

### Comparing `GuiMPLpretest-0.0.5/GuiMPLpretest/controller.py` & `GuiMPLpretest-0.0.6/GuiMPLpretest/controller.py`

 * *Files identical despite different names*

### Comparing `GuiMPLpretest-0.0.5/GuiMPLpretest/dico_params.py` & `GuiMPLpretest-0.0.6/GuiMPLpretest/dico_params.py`

 * *Files identical despite different names*

### Comparing `GuiMPLpretest-0.0.5/GuiMPLpretest/model.py` & `GuiMPLpretest-0.0.6/GuiMPLpretest/model.py`

 * *Files identical despite different names*

### Comparing `GuiMPLpretest-0.0.5/GuiMPLpretest/view.py` & `GuiMPLpretest-0.0.6/GuiMPLpretest/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/python3
 import matplotlib
 import tkinter as tk
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
-from sys import platform as sys_pf
 
-from row_pygubu.row_pygubu_main import RowPygubuUiApp
-from row_pygubu.axeschoosewidgetsframe import AxesChooseWidgetsFrameWidget
+# from sys import platform as sys_pf
 
-from surcouches_pygubu.autowidgetsframe import AutoWidgetsFrame
-from surcouches_pygubu.mainaxewidgetsframewidget import (
+from GuiMPLpretest.row_pygubu.row_pygubu_main import RowPygubuUiApp
+from GuiMPLpretest.row_pygubu.axeschoosewidgetsframe import AxesChooseWidgetsFrameWidget
+
+from GuiMPLpretest.surcouches_pygubu.autowidgetsframe import AutoWidgetsFrame
+from GuiMPLpretest.surcouches_pygubu.mainaxewidgetsframewidget import (
     MainAxeWidgetsFrameWidget,
 )
 
 from GuiMPLpretest.dico_params import dico_param_figure, dico_param_axe, dico_param_line
 
 
 class View(RowPygubuUiApp):
@@ -369,13 +370,13 @@
             self.line_widgets_list[axe_row][axe_col][line_index].grid_remove()
         self.line_widgets_list[axe_row][axe_col][line_choice].grid(column=0, row=0)
 
     def run(self):
         self.main_frame.mainloop()
 
 
-if sys_pf == "darwin":
-    matplotlib.use("TkAgg")
+# if sys_pf == "darwin":
+#    matplotlib.use("TkAgg")
 
 if __name__ == "__main__":
     app = View("fake_contro")
     app.run()
```

### Comparing `GuiMPLpretest-0.0.5/GuiMPLpretest.egg-info/PKG-INFO` & `GuiMPLpretest-0.0.6/GuiMPLpretest.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GuiMPLpretest
-Version: 0.0.5
+Version: 0.0.6
 Summary: Application pour modifier l'esthétique d'un graphique matplotlib
 Author: Groupe Figure MPCI
 Keywords: matplotlib,graphique,interface graphique,python,figures
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `GuiMPLpretest-0.0.5/PKG-INFO` & `GuiMPLpretest-0.0.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GuiMPLpretest
-Version: 0.0.5
+Version: 0.0.6
 Summary: Application pour modifier l'esthétique d'un graphique matplotlib
 Author: Groupe Figure MPCI
 Keywords: matplotlib,graphique,interface graphique,python,figures
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

