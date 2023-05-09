# Comparing `tmp/GuiMPLpretest-0.0.8.tar.gz` & `tmp/GuiMPLpretest-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GuiMPLpretest-0.0.8.tar", last modified: Tue May  9 21:09:25 2023, max compression
+gzip compressed data, was "GuiMPLpretest-0.0.9.tar", last modified: Tue May  9 21:33:59 2023, max compression
```

## Comparing `GuiMPLpretest-0.0.8.tar` & `GuiMPLpretest-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 21:09:25.759206 GuiMPLpretest-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-05-09 21:09:25.719305 GuiMPLpretest-0.0.8/GuiMPLpretest/
--rw-rw-rw-   0        0        0      123 2023-05-09 19:47:11.000000 GuiMPLpretest-0.0.8/GuiMPLpretest/__init__.py
--rw-rw-rw-   0        0        0      502 2023-05-09 19:38:14.000000 GuiMPLpretest-0.0.8/GuiMPLpretest/app.py
--rw-rw-rw-   0        0        0     6099 2023-05-09 19:43:18.000000 GuiMPLpretest-0.0.8/GuiMPLpretest/controller.py
-drwxrwxrwx   0        0        0        0 2023-05-09 21:09:25.744711 GuiMPLpretest-0.0.8/GuiMPLpretest/custom_widgets/
--rw-rw-rw-   0        0        0        0 2023-05-09 21:08:34.000000 GuiMPLpretest-0.0.8/GuiMPLpretest/custom_widgets/__init__.py
--rw-rw-rw-   0        0        0      705 2023-05-08 10:41:55.000000 GuiMPLpretest-0.0.8/GuiMPLpretest/custom_widgets/color_chooser.py
--rw-rw-rw-   0        0        0     1294 2023-05-09 14:16:24.000000 GuiMPLpretest-0.0.8/GuiMPLpretest/custom_widgets/double_spinbox.py
--rw-rw-rw-   0        0        0     2098 2023-05-07 18:07:31.000000 GuiMPLpretest-0.0.8/GuiMPLpretest/dico_params.py
--rw-rw-rw-   0        0        0     3024 2023-05-09 14:32:19.000000 GuiMPLpretest-0.0.8/GuiMPLpretest/model.py
-drwxrwxrwx   0        0        0        0 2023-05-09 21:09:25.752042 GuiMPLpretest-0.0.8/GuiMPLpretest/row_pygubu/
--rw-rw-rw-   0        0        0        0 2023-05-09 21:08:24.000000 GuiMPLpretest-0.0.8/GuiMPLpretest/row_pygubu/__init__.py
--rw-rw-rw-   0        0        0      474 2023-05-07 18:59:33.000000 GuiMPLpretest-0.0.8/GuiMPLpretest/row_pygubu/autowidgets_base_frame.py
--rw-rw-rw-   0        0        0     1217 2023-05-07 19:19:14.000000 GuiMPLpretest-0.0.8/GuiMPLpretest/row_pygubu/axeschoosewidgetsframe.py
--rw-rw-rw-   0        0        0     1059 2023-05-01 14:44:47.000000 GuiMPLpretest-0.0.8/GuiMPLpretest/row_pygubu/axewidgetsbaseframe.py
--rw-rw-rw-   0        0        0     1648 2023-05-09 19:26:53.000000 GuiMPLpretest-0.0.8/GuiMPLpretest/row_pygubu/row_pygubu_main.py
-drwxrwxrwx   0        0        0        0 2023-05-09 21:09:25.755191 GuiMPLpretest-0.0.8/GuiMPLpretest/surcouches_pygubu/
--rw-rw-rw-   0        0        0        0 2023-05-09 21:08:15.000000 GuiMPLpretest-0.0.8/GuiMPLpretest/surcouches_pygubu/__init__.py
--rw-rw-rw-   0        0        0     4524 2023-05-09 19:39:07.000000 GuiMPLpretest-0.0.8/GuiMPLpretest/surcouches_pygubu/autowidgetsframe.py
--rw-rw-rw-   0        0        0     1322 2023-05-09 19:39:12.000000 GuiMPLpretest-0.0.8/GuiMPLpretest/surcouches_pygubu/mainaxewidgetsframewidget.py
--rw-rw-rw-   0        0        0    16009 2023-05-09 20:48:22.000000 GuiMPLpretest-0.0.8/GuiMPLpretest/view.py
-drwxrwxrwx   0        0        0        0 2023-05-09 21:09:25.739554 GuiMPLpretest-0.0.8/GuiMPLpretest.egg-info/
--rw-rw-rw-   0        0        0      615 2023-05-09 21:09:25.000000 GuiMPLpretest-0.0.8/GuiMPLpretest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      863 2023-05-09 21:09:25.000000 GuiMPLpretest-0.0.8/GuiMPLpretest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 21:09:25.000000 GuiMPLpretest-0.0.8/GuiMPLpretest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-09 21:09:25.000000 GuiMPLpretest-0.0.8/GuiMPLpretest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-09 21:09:25.000000 GuiMPLpretest-0.0.8/GuiMPLpretest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      615 2023-05-09 21:09:25.756222 GuiMPLpretest-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-09 21:09:25.760211 GuiMPLpretest-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      922 2023-05-09 21:09:14.000000 GuiMPLpretest-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 21:33:59.114381 GuiMPLpretest-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-05-09 21:33:59.086750 GuiMPLpretest-0.0.9/GuiMPLpretest/
+-rw-rw-rw-   0        0        0      102 2023-05-09 21:31:56.000000 GuiMPLpretest-0.0.9/GuiMPLpretest/__init__.py
+-rw-rw-rw-   0        0        0      495 2023-05-09 21:31:57.000000 GuiMPLpretest-0.0.9/GuiMPLpretest/app.py
+-rw-rw-rw-   0        0        0     6078 2023-05-09 21:32:52.000000 GuiMPLpretest-0.0.9/GuiMPLpretest/controller.py
+drwxrwxrwx   0        0        0        0 2023-05-09 21:33:59.106370 GuiMPLpretest-0.0.9/GuiMPLpretest/custom_widgets/
+-rw-rw-rw-   0        0        0        0 2023-05-09 21:08:34.000000 GuiMPLpretest-0.0.9/GuiMPLpretest/custom_widgets/__init__.py
+-rw-rw-rw-   0        0        0      705 2023-05-08 10:41:55.000000 GuiMPLpretest-0.0.9/GuiMPLpretest/custom_widgets/color_chooser.py
+-rw-rw-rw-   0        0        0     1294 2023-05-09 14:16:24.000000 GuiMPLpretest-0.0.9/GuiMPLpretest/custom_widgets/double_spinbox.py
+-rw-rw-rw-   0        0        0     2098 2023-05-07 18:07:31.000000 GuiMPLpretest-0.0.9/GuiMPLpretest/dico_params.py
+-rw-rw-rw-   0        0        0     3024 2023-05-09 14:32:19.000000 GuiMPLpretest-0.0.9/GuiMPLpretest/model.py
+drwxrwxrwx   0        0        0        0 2023-05-09 21:33:59.111393 GuiMPLpretest-0.0.9/GuiMPLpretest/row_pygubu/
+-rw-rw-rw-   0        0        0        0 2023-05-09 21:08:24.000000 GuiMPLpretest-0.0.9/GuiMPLpretest/row_pygubu/__init__.py
+-rw-rw-rw-   0        0        0      474 2023-05-07 18:59:33.000000 GuiMPLpretest-0.0.9/GuiMPLpretest/row_pygubu/autowidgets_base_frame.py
+-rw-rw-rw-   0        0        0     1217 2023-05-07 19:19:14.000000 GuiMPLpretest-0.0.9/GuiMPLpretest/row_pygubu/axeschoosewidgetsframe.py
+-rw-rw-rw-   0        0        0     1059 2023-05-01 14:44:47.000000 GuiMPLpretest-0.0.9/GuiMPLpretest/row_pygubu/axewidgetsbaseframe.py
+-rw-rw-rw-   0        0        0     1648 2023-05-09 21:17:50.000000 GuiMPLpretest-0.0.9/GuiMPLpretest/row_pygubu/row_pygubu_main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 21:33:59.113385 GuiMPLpretest-0.0.9/GuiMPLpretest/surcouches_pygubu/
+-rw-rw-rw-   0        0        0        0 2023-05-09 21:08:15.000000 GuiMPLpretest-0.0.9/GuiMPLpretest/surcouches_pygubu/__init__.py
+-rw-rw-rw-   0        0        0     4503 2023-05-09 21:31:52.000000 GuiMPLpretest-0.0.9/GuiMPLpretest/surcouches_pygubu/autowidgetsframe.py
+-rw-rw-rw-   0        0        0     1315 2023-05-09 21:31:50.000000 GuiMPLpretest-0.0.9/GuiMPLpretest/surcouches_pygubu/mainaxewidgetsframewidget.py
+-rw-rw-rw-   0        0        0    16045 2023-05-09 21:33:45.000000 GuiMPLpretest-0.0.9/GuiMPLpretest/view.py
+drwxrwxrwx   0        0        0        0 2023-05-09 21:33:59.103389 GuiMPLpretest-0.0.9/GuiMPLpretest.egg-info/
+-rw-rw-rw-   0        0        0      615 2023-05-09 21:33:58.000000 GuiMPLpretest-0.0.9/GuiMPLpretest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2023-05-09 21:33:59.000000 GuiMPLpretest-0.0.9/GuiMPLpretest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 21:33:58.000000 GuiMPLpretest-0.0.9/GuiMPLpretest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-09 21:33:58.000000 GuiMPLpretest-0.0.9/GuiMPLpretest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-09 21:33:59.000000 GuiMPLpretest-0.0.9/GuiMPLpretest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      615 2023-05-09 21:33:59.114381 GuiMPLpretest-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-09 21:33:59.115383 GuiMPLpretest-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      922 2023-05-09 21:33:06.000000 GuiMPLpretest-0.0.9/setup.py
```

### Comparing `GuiMPLpretest-0.0.8/GuiMPLpretest/controller.py` & `GuiMPLpretest-0.0.9/GuiMPLpretest/controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from tkinter import filedialog
 import os
 import pickle
 from matplotlib.figure import Figure
 
-from GuiMPLpretest.view import View
-from GuiMPLpretest.model import Model
-from GuiMPLpretest.dico_params import dico_param_figure, dico_param_axe, dico_param_line
+from guimpl.view import View
+from guimpl.model import Model
+from guimpl.dico_params import dico_param_figure, dico_param_axe, dico_param_line
 
 
 class Controller:
     def __init__(self, fig: Figure = None, fig_file_name: str = None):
         self.model = Model()
         self.view = View(self)
         self.data_set_list = []
```

### Comparing `GuiMPLpretest-0.0.8/GuiMPLpretest/custom_widgets/color_chooser.py` & `GuiMPLpretest-0.0.9/GuiMPLpretest/custom_widgets/color_chooser.py`

 * *Files identical despite different names*

### Comparing `GuiMPLpretest-0.0.8/GuiMPLpretest/custom_widgets/double_spinbox.py` & `GuiMPLpretest-0.0.9/GuiMPLpretest/custom_widgets/double_spinbox.py`

 * *Files identical despite different names*

### Comparing `GuiMPLpretest-0.0.8/GuiMPLpretest/dico_params.py` & `GuiMPLpretest-0.0.9/GuiMPLpretest/dico_params.py`

 * *Files identical despite different names*

### Comparing `GuiMPLpretest-0.0.8/GuiMPLpretest/model.py` & `GuiMPLpretest-0.0.9/GuiMPLpretest/model.py`

 * *Files identical despite different names*

### Comparing `GuiMPLpretest-0.0.8/GuiMPLpretest/row_pygubu/axeschoosewidgetsframe.py` & `GuiMPLpretest-0.0.9/GuiMPLpretest/row_pygubu/axeschoosewidgetsframe.py`

 * *Files identical despite different names*

### Comparing `GuiMPLpretest-0.0.8/GuiMPLpretest/row_pygubu/axewidgetsbaseframe.py` & `GuiMPLpretest-0.0.9/GuiMPLpretest/row_pygubu/axewidgetsbaseframe.py`

 * *Files identical despite different names*

### Comparing `GuiMPLpretest-0.0.8/GuiMPLpretest/row_pygubu/row_pygubu_main.py` & `GuiMPLpretest-0.0.9/GuiMPLpretest/row_pygubu/row_pygubu_main.py`

 * *Files identical despite different names*

### Comparing `GuiMPLpretest-0.0.8/GuiMPLpretest/surcouches_pygubu/autowidgetsframe.py` & `GuiMPLpretest-0.0.9/GuiMPLpretest/surcouches_pygubu/autowidgetsframe.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import tkinter as tk
 import tkinter.ttk as ttk
 
-from GuiMPLpretest.row_pygubu.autowidgets_base_frame import AutowidgetsBaseFrameWidget
-from GuiMPLpretest.custom_widgets.color_chooser import ColorChooser
-from GuiMPLpretest.custom_widgets.double_spinbox import DoubleSpinbox
+from guimpl.row_pygubu.autowidgets_base_frame import AutowidgetsBaseFrameWidget
+from guimpl.custom_widgets.color_chooser import ColorChooser
+from guimpl.custom_widgets.double_spinbox import DoubleSpinbox
 
 
 class AutoWidgetsFrame(AutowidgetsBaseFrameWidget):
     def __init__(self, master=None, **kw):
         super().__init__(master, **kw)
         self.next_widget_row = 0
         self.widgets_dico = {}
```

### Comparing `GuiMPLpretest-0.0.8/GuiMPLpretest/surcouches_pygubu/mainaxewidgetsframewidget.py` & `GuiMPLpretest-0.0.9/GuiMPLpretest/surcouches_pygubu/mainaxewidgetsframewidget.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tkinter as tk
 import tkinter.ttk as ttk
 
-from GuiMPLpretest.row_pygubu.axewidgetsbaseframe import AxeWidgetsBaseFrameWidget
+from guimpl.row_pygubu.axewidgetsbaseframe import AxeWidgetsBaseFrameWidget
 
 
 class MainAxeWidgetsFrameWidget(ttk.Frame):
     def __init__(self, master=None, **kw):
         super(MainAxeWidgetsFrameWidget, self).__init__(master, **kw)
         self.canvas = tk.Canvas(self)
         self.canvas.configure(height=800, width=320)
```

### Comparing `GuiMPLpretest-0.0.8/GuiMPLpretest/view.py` & `GuiMPLpretest-0.0.9/GuiMPLpretest/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python3
 import matplotlib
 import tkinter as tk
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 
-# from sys import platform as sys_pf
+from sys import platform as sys_pf
 
 from GuiMPLpretest.row_pygubu.row_pygubu_main import RowPygubuUiApp
 from GuiMPLpretest.row_pygubu.axeschoosewidgetsframe import AxesChooseWidgetsFrameWidget
 
 from GuiMPLpretest.surcouches_pygubu.autowidgetsframe import AutoWidgetsFrame
 from GuiMPLpretest.surcouches_pygubu.mainaxewidgetsframewidget import (
     MainAxeWidgetsFrameWidget,
@@ -17,14 +17,15 @@
 
 
 class View(RowPygubuUiApp):
     # Initialisation
 
     def __init__(self, controller, master=None):
         super().__init__(master)
+        self.mainwindow.title("GuiMPL")
         self.controller = controller
         self.rinit()
         self.menu_initiator()
 
     def rinit(self):
         self.widgets_dico = {}
 
@@ -370,13 +371,13 @@
             self.line_widgets_list[axe_row][axe_col][line_index].grid_remove()
         self.line_widgets_list[axe_row][axe_col][line_choice].grid(column=0, row=0)
 
     def run(self):
         self.main_frame.mainloop()
 
 
-# if sys_pf == "darwin":
-#    matplotlib.use("TkAgg")
+if sys_pf == "darwin":
+    matplotlib.use("TkAgg")
 
 if __name__ == "__main__":
     app = View("fake_contro")
     app.run()
```

### Comparing `GuiMPLpretest-0.0.8/GuiMPLpretest.egg-info/PKG-INFO` & `GuiMPLpretest-0.0.9/GuiMPLpretest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GuiMPLpretest
-Version: 0.0.8
+Version: 0.0.9
 Summary: Application pour modifier l'esthétique d'un graphique matplotlib
 Author: Groupe Figure MPCI
 Keywords: matplotlib,graphique,interface graphique,python,figures
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `GuiMPLpretest-0.0.8/GuiMPLpretest.egg-info/SOURCES.txt` & `GuiMPLpretest-0.0.9/GuiMPLpretest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GuiMPLpretest-0.0.8/PKG-INFO` & `GuiMPLpretest-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GuiMPLpretest
-Version: 0.0.8
+Version: 0.0.9
 Summary: Application pour modifier l'esthétique d'un graphique matplotlib
 Author: Groupe Figure MPCI
 Keywords: matplotlib,graphique,interface graphique,python,figures
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `GuiMPLpretest-0.0.8/setup.py` & `GuiMPLpretest-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 DESCRIPTION = "Application pour modifier l'esthétique d'un graphique matplotlib"
 LONG_DESCRIPTION = "Projet Figure S2 MPCI ayant pour but le développement d'une interface graphique permettant d'intéragir ergonomiquement avec des figures matplotlib"
 
 # Setting up
 setup(
     name="GuiMPLpretest",
     version=VERSION,
```

