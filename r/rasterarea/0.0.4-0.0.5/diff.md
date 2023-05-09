# Comparing `tmp/rasterarea-0.0.4.tar.gz` & `tmp/rasterarea-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasterarea-0.0.4.tar", last modified: Sat Apr 22 03:44:13 2023, max compression
+gzip compressed data, was "rasterarea-0.0.5.tar", last modified: Tue May  9 18:56:47 2023, max compression
```

## Comparing `rasterarea-0.0.4.tar` & `rasterarea-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:44:13.895546 rasterarea-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-22 03:43:57.000000 rasterarea-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-22 03:43:57.000000 rasterarea-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-22 03:44:13.895546 rasterarea-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-22 03:43:57.000000 rasterarea-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:44:13.895546 rasterarea-0.0.4/rasterarea/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-22 03:43:57.000000 rasterarea-0.0.4/rasterarea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-22 03:43:57.000000 rasterarea-0.0.4/rasterarea/foliummap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-04-22 03:43:57.000000 rasterarea-0.0.4/rasterarea/ipyleafletmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-04-22 03:43:57.000000 rasterarea-0.0.4/rasterarea/rasterarea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:44:13.895546 rasterarea-0.0.4/rasterarea.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-22 03:44:13.000000 rasterarea-0.0.4/rasterarea.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-22 03:44:13.000000 rasterarea-0.0.4/rasterarea.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-22 03:44:13.000000 rasterarea-0.0.4/rasterarea.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 03:44:13.000000 rasterarea-0.0.4/rasterarea.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-22 03:44:13.000000 rasterarea-0.0.4/rasterarea.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 03:44:13.000000 rasterarea-0.0.4/rasterarea.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-22 03:43:57.000000 rasterarea-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-22 03:44:13.895546 rasterarea-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-22 03:43:57.000000 rasterarea-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:56:47.834867 rasterarea-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 18:56:37.000000 rasterarea-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-09 18:56:37.000000 rasterarea-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-09 18:56:47.834867 rasterarea-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-09 18:56:37.000000 rasterarea-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:56:47.834867 rasterarea-0.0.5/rasterarea/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-09 18:56:37.000000 rasterarea-0.0.5/rasterarea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-09 18:56:37.000000 rasterarea-0.0.5/rasterarea/foliummap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-05-09 18:56:37.000000 rasterarea-0.0.5/rasterarea/ipyleafletmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-05-09 18:56:37.000000 rasterarea-0.0.5/rasterarea/rasterarea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:56:47.834867 rasterarea-0.0.5/rasterarea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-09 18:56:47.000000 rasterarea-0.0.5/rasterarea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-09 18:56:47.000000 rasterarea-0.0.5/rasterarea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-09 18:56:47.000000 rasterarea-0.0.5/rasterarea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 18:56:47.000000 rasterarea-0.0.5/rasterarea.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-09 18:56:47.000000 rasterarea-0.0.5/rasterarea.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 18:56:47.000000 rasterarea-0.0.5/rasterarea.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-09 18:56:37.000000 rasterarea-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-09 18:56:47.838867 rasterarea-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-09 18:56:37.000000 rasterarea-0.0.5/setup.py
```

### Comparing `rasterarea-0.0.4/LICENSE` & `rasterarea-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rasterarea-0.0.4/PKG-INFO` & `rasterarea-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasterarea
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package provides a more accurate way to claculate the area of rasters.
 Home-page: https://github.com/Feng96/rasterarea
 Author: Yinan Feng
 Author-email: 1041267458@qq.com
 License: MIT license
 Keywords: rasterarea
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `rasterarea-0.0.4/README.md` & `rasterarea-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rasterarea-0.0.4/rasterarea/foliummap.py` & `rasterarea-0.0.5/rasterarea/foliummap.py`

 * *Files identical despite different names*

### Comparing `rasterarea-0.0.4/rasterarea/ipyleafletmap.py` & `rasterarea-0.0.5/rasterarea/ipyleafletmap.py`

 * *Files 24% similar despite different names*

```diff
@@ -210,8 +210,116 @@
             url (str): The URL of the image.
             width (int): The width of the image.
             height (int): The height of the image.
             position (str, optional): The position of the image. Defaults to 'bottomright'.
         """
         widget = widgets.HTML(value = f'<img src="{url}" width="{width}" height="{height}">')
         control = WidgetControl(widget=widget, position=position)
-        self.add(control)
+        self.add(control)
+
+    
+    def add_toolbar(self, position='topright', **kwargs):
+        """Adds a toolbar to the map.
+
+        Args:
+            toolbar (str, optional): The toolbar to add. Defaults to 'draw'.
+            position (str, optional): The position of the toolbar. Defaults to 'topright'.
+        """
+        widget_width = "250px"
+        padding = "0px 0px 0px 5px"  # upper, right, bottom, left
+
+        toolbar_button = widgets.ToggleButton(
+            value=False,
+            tooltip="Toolbar",
+            icon="wrench",
+            layout=widgets.Layout(width="28px", height="28px", padding=padding),
+        )
+
+        close_button = widgets.ToggleButton(
+            value=False,
+            tooltip="Close the tool",
+            icon="times",
+            button_style="primary",
+            layout=widgets.Layout(height="28px", width="28px", padding=padding),
+        )
+        toolbar = widgets.HBox([toolbar_button])
+
+        def toolbar_click(change):
+            if change["new"]:
+                toolbar.children = [toolbar_button, close_button]
+            else:
+                toolbar.children = [toolbar_button]
+        
+        toolbar_button.observe(toolbar_click, "value")
+
+        def close_click(change):
+            if change["new"]:
+                toolbar_button.close()
+                close_button.close()
+                toolbar.close()
+        
+        close_button.observe(close_click, "value")
+        rows = 2
+        cols = 2
+        grid = widgets.GridspecLayout(rows, cols, grid_gap="0px", layout=widgets.Layout(width="65px"))
+        icons = ["folder-open", "map", "info", "question"]
+
+        for i in range(rows):
+            for j in range(cols):
+                grid[i, j] = widgets.Button(description="", button_style="primary", icon=icons[i*rows+j], 
+                                            layout=widgets.Layout(width="28px", padding="0px"))
+        toolbar = widgets.VBox([toolbar_button])
+        def toolbar_click(change):
+            if change["new"]:
+                toolbar.children = [widgets.HBox([close_button, toolbar_button]), grid]
+            else:
+                toolbar.children = [toolbar_button]
+        
+        toolbar_button.observe(toolbar_click, "value")
+
+        toolbar_ctrl = WidgetControl(widget=toolbar, position=position)
+
+        output = widgets.Output()
+        output_ctrl = WidgetControl(widget=output, position="bottomright")
+        def tool_click(b):    
+            with output:
+                output.clear_output()
+                print(f"You clicked the {b.icon} button")
+
+        for i in range(rows):
+            for j in range(cols):
+                tool = grid[i, j]
+                tool.on_click(tool_click)
+
+        with output:
+            output.clear_output()
+            print("Click on a button to see the output")
+
+        basemap = widgets.Dropdown(
+            options=["roadmap", "satellite"],
+            value=None,
+            description="Basemap:",
+            style={"description_width": "initial"},
+            layout=widgets.Layout(width="200px"),
+        )
+        basemap_ctrl = WidgetControl(widget=basemap, position="topright")
+
+        def tool_click(b):    
+            with output:
+                output.clear_output()
+                print(f"You clicked the {b.icon} button")
+
+                if b.icon == "map":
+                    self.add_control(basemap_ctrl)
+
+        for i in range(rows):
+            for j in range(cols):
+                tool = grid[i, j]
+                tool.on_click(tool_click)
+
+        def change_basemap(change):
+            if change["new"]:
+                self.add_basemap(basemap.value)
+
+        basemap.observe(change_basemap, names='value')
+        self.add_control(toolbar_ctrl)
+
```

### Comparing `rasterarea-0.0.4/rasterarea.egg-info/PKG-INFO` & `rasterarea-0.0.5/rasterarea.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasterarea
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package provides a more accurate way to claculate the area of rasters.
 Home-page: https://github.com/Feng96/rasterarea
 Author: Yinan Feng
 Author-email: 1041267458@qq.com
 License: MIT license
 Keywords: rasterarea
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `rasterarea-0.0.4/setup.py` & `rasterarea-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='rasterarea',
     name='rasterarea',
     packages=find_packages(include=['rasterarea', 'rasterarea.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Feng96/rasterarea',
-    version='0.0.4',
+    version='0.0.5',
     zip_safe=False,
 )
```

