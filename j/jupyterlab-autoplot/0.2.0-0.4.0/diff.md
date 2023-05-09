# Comparing `tmp/jupyterlab-autoplot-0.2.0.tar.gz` & `tmp/jupyterlab-autoplot-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab-autoplot-0.2.0.tar", last modified: Wed May 12 08:37:10 2021, max compression
+gzip compressed data, was "jupyterlab-autoplot-0.4.0.tar", last modified: Tue May  9 19:51:26 2023, max compression
```

## Comparing `jupyterlab-autoplot-0.2.0.tar` & `jupyterlab-autoplot-0.4.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-05-12 08:37:10.843504 jupyterlab-autoplot-0.2.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5631 2021-05-12 08:37:10.843504 jupyterlab-autoplot-0.2.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4596 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-05-12 08:37:10.839504 jupyterlab-autoplot-0.2.0/autoplot/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8823 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/autoplot/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-05-12 08:37:10.839504 jupyterlab-autoplot-0.2.0/autoplot/dtaler/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8909 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/autoplot/dtaler/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-05-12 08:37:10.839504 jupyterlab-autoplot-0.2.0/autoplot/extensions/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       77 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/autoplot/extensions/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1271 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/autoplot/extensions/autoplot_display.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4934 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/autoplot/extensions/toast.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-05-12 08:37:10.839504 jupyterlab-autoplot-0.2.0/autoplot/plotter/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26246 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/autoplot/plotter/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2612 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/autoplot/plotter/range_selector_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9645 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/autoplot/plotter/trace.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-05-12 08:37:10.839504 jupyterlab-autoplot-0.2.0/autoplot/plugins/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      836 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/autoplot/plugins/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-05-12 08:37:10.839504 jupyterlab-autoplot-0.2.0/autoplot/plugins/bundles/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5860 2021-05-12 08:36:55.000000 jupyterlab-autoplot-0.2.0/autoplot/plugins/bundles/interactiveLegend.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5885 2021-05-12 08:36:55.000000 jupyterlab-autoplot-0.2.0/autoplot/plugins/bundles/rangeSelectorButtons.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7707 2021-05-12 08:36:55.000000 jupyterlab-autoplot-0.2.0/autoplot/plugins/bundles/saveImageButtons.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11503 2021-05-12 08:36:55.000000 jupyterlab-autoplot-0.2.0/autoplot/plugins/bundles/timeSeriesTooltip.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2913 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/autoplot/plugins/interactive_legend.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1009 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/autoplot/plugins/line_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3767 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/autoplot/plugins/range_selector_buttons.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1819 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/autoplot/plugins/save_image_buttons.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2238 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/autoplot/plugins/time_series_tooltip.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-05-12 08:37:10.839504 jupyterlab-autoplot-0.2.0/autoplot/utils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      231 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/autoplot/utils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      878 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/autoplot/utils/constants.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-05-12 08:37:10.839504 jupyterlab-autoplot-0.2.0/autoplot/view_manager/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12387 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/autoplot/view_manager/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1325 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/autoplot/view_manager/variable_utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-05-12 08:37:10.843504 jupyterlab-autoplot-0.2.0/jupyterlab_autoplot.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5631 2021-05-12 08:37:10.000000 jupyterlab-autoplot-0.2.0/jupyterlab_autoplot.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1041 2021-05-12 08:37:10.000000 jupyterlab-autoplot-0.2.0/jupyterlab_autoplot.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-05-12 08:37:10.000000 jupyterlab-autoplot-0.2.0/jupyterlab_autoplot.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       69 2021-05-12 08:37:10.000000 jupyterlab-autoplot-0.2.0/jupyterlab_autoplot.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2021-05-12 08:37:10.000000 jupyterlab-autoplot-0.2.0/jupyterlab_autoplot.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2021-05-12 08:37:10.843504 jupyterlab-autoplot-0.2.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1120 2021-05-12 08:34:42.000000 jupyterlab-autoplot-0.2.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.570782 jupyterlab-autoplot-0.4.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5136 2023-05-09 19:51:26.570782 jupyterlab-autoplot-0.4.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4596 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.566782 jupyterlab-autoplot-0.4.0/autoplot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8823 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.566782 jupyterlab-autoplot-0.4.0/autoplot/dtaler/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9125 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/dtaler/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.566782 jupyterlab-autoplot-0.4.0/autoplot/extensions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/extensions/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1272 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/extensions/autoplot_display.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4934 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/extensions/toast.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.566782 jupyterlab-autoplot-0.4.0/autoplot/plotter/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26256 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/plotter/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2612 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/plotter/range_selector_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9665 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/plotter/trace.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.566782 jupyterlab-autoplot-0.4.0/autoplot/plugins/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      836 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.566782 jupyterlab-autoplot-0.4.0/autoplot/plugins/bundles/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5860 2023-05-09 19:51:09.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/bundles/interactiveLegend.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5885 2023-05-09 19:51:09.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/bundles/rangeSelectorButtons.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7707 2023-05-09 19:51:09.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/bundles/saveImageButtons.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11503 2023-05-09 19:51:09.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/bundles/timeSeriesTooltip.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2913 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/interactive_legend.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/line_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3932 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/range_selector_buttons.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1819 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/save_image_buttons.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2238 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/time_series_tooltip.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.566782 jupyterlab-autoplot-0.4.0/autoplot/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      231 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      878 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/utils/constants.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.570782 jupyterlab-autoplot-0.4.0/autoplot/view_manager/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12387 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/view_manager/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1325 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/view_manager/variable_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.570782 jupyterlab-autoplot-0.4.0/jupyterlab_autoplot.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5136 2023-05-09 19:51:26.000000 jupyterlab-autoplot-0.4.0/jupyterlab_autoplot.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1041 2023-05-09 19:51:26.000000 jupyterlab-autoplot-0.4.0/jupyterlab_autoplot.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-09 19:51:26.000000 jupyterlab-autoplot-0.4.0/jupyterlab_autoplot.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-05-09 19:51:26.000000 jupyterlab-autoplot-0.4.0/jupyterlab_autoplot.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-05-09 19:51:26.000000 jupyterlab-autoplot-0.4.0/jupyterlab_autoplot.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-09 19:51:26.570782 jupyterlab-autoplot-0.4.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1114 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/setup.py
```

### Comparing `jupyterlab-autoplot-0.2.0/PKG-INFO` & `jupyterlab-autoplot-0.4.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,58 @@
-Metadata-Version: 1.2
-Name: jupyterlab-autoplot
-Version: 0.2.0
-Summary: The IPython component for the Autoplot JupyterLab extension.
-Home-page: https://github.com/man-group/jupyterlab-autoplot
-Author: Man Alpha Technology
-Author-email: ManAlphaTech@man.com
-License: BSD 3-Clause
-Description: # JupyterLab Autoplot - IPython Component
-        
-        This IPython extension is one of the three components that make up the [JupyterLab Autoplot extension](../README.md).
-        
-        ## Development
-        
-        First you should follow the instructions [here](../autoplot-display#development) to install the JupyterLab extension component. Then, to apply the changes you have made to the IPython component:
-        
-        ```sh
-        cd ipython-extension/
-        python -m pip install -e .
-        ```
-        
-        You can then reload the extension in your JupyterLab instance with `%reload_ext autoplot` (you may need to restart the kernel first).
-        
-        ### Description of classes
-        
-        Each of the following classes will be initialised **once** in the `load_ipython_extension()` function, and, where necessary, these instances will be accessible to each other. A diagram showing how these classes interact can be found at the bottom of this section.
-        
-        #### `ViewManager`
-        
-        This class is the interface between the ipython interactions and the underlying models. The `redraw` method is expected to be called in the `post_run_cell` IPython hook. All the other methods implement one of the magic commands in autoplot.
-        
-        This class is a proxy for the actual models, which implement the `View` interface and will perform the actual work needed to integrate with dtale or mpd3.
-        
-        When `redraw` is called, the class instance will scan the variables in the notebook's namespace, and look for pandas variables. The active view's `update_variables` is called with the filtered variables. Then, the `draw` method is called. Currently, only the active view's `update_variables` is called; however, it may be argued that syncing the `--freeze` and `--ignore` commands regardless of the current view is more natural. In that case, it will be useful to call `update_variables` in all views, rather than just the active one. We need to get more user feedback to decide which is the best approach.
-        
-        #### `_make_magic` (`AutoplotMagic`)
-        
-        The function `_make_magic` is a factory for instances of `AutoplotMagic`, in fact, it builds the class itself so that it can easily define the list of possible views in the `-v` argument.
-        
-        AutoplotMagic extends [`IPython.core.magic.Magics`](https://ipython.readthedocs.io/en/stable/api/generated/IPython.core.magic.html#IPython.core.magic.Magics), and defines the magic commands described [here](../README.md#modifying-the-plot--traces). This class translates the user input into calls to the `ViewManager`.
-        
-        #### `AutoplotDisplay`
-        
-        This class extends [`ipywidgets.Output`](https://ipywidgets.readthedocs.io/en/latest/examples/Output%20Widget.html), and defines the output area in which the graph is plotted. By matching the attributes `_model_name`, `_model_module_version` etc. with the equivalents in the JupyterLab extension class `AutoplotDisplayModel`, the two become linked and the output captured by the IPython component will be displayed wherever the JupyterLab component is rendered.
-        
-        This class also defines the `data_id` property, which is used by dtale to find out which instance (dataframe) is currently active.
-        
-        #### `Toast`
-        
-        This class defines some methods to dispatch DOM events that trigger toast notifications in the JupyterLab extension. These toasts change colour depending on their type, which can be one of 'error', 'warning', 'success' or 'info'.
-        
-        #### Backends
-        
-        ##### `Dtaler`
-        
-        This is the class that implements the View interface for the dtale integration. It's responsible to keep track of the changed variables and dtale instances.
-        
-        ##### `PlotterModel` and `Plotter`
-        
-        `PlotterModel` is the class that implements the View interface. It defines a dictionary of series names to their values, and one of dataframe names to the set of series names that were created from its columns. The `draw` method calls `plotter.plot()`, which initialises a matplotlib figure and axes, adds the defined traces to it and styles the figure.
-        
-        When a series is added, modified or deleted, the dictionaries will be updated and the appropriate calls will be made to the `Plotter` instance.
-        
-        The `Plotter` class manages the collection of `Trace` class instances and handles the graph plotting. It has a number of public methods like `update_trace_series()`, `update_trace_colour()` etc. which are used by the `PlotterModel` class to modify the plot and/or traces.
-        
-        The `Trace` class stores a matplotlib `Line2D` instance and some details about how it should be displayed. Like the `Plotter` class, it defines a number of public methods to allow it to be easily updated, like `update_series()` or `update_colour()`. It also handles the downsampling of long series.
-        
-Keywords: jupyter,jupyterlab,matplotlib,mpld3,time series
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: Jupyter
-Requires-Python: >=3.6
+# JupyterLab Autoplot - IPython Component
+
+This IPython extension is one of the three components that make up the [JupyterLab Autoplot extension](../README.md).
+
+## Development
+
+First you should follow the instructions [here](../autoplot-display#development) to install the JupyterLab extension component. Then, to apply the changes you have made to the IPython component:
+
+```sh
+cd ipython-extension/
+python -m pip install -e .
+```
+
+You can then reload the extension in your JupyterLab instance with `%reload_ext autoplot` (you may need to restart the kernel first).
+
+### Description of classes
+
+Each of the following classes will be initialised **once** in the `load_ipython_extension()` function, and, where necessary, these instances will be accessible to each other. A diagram showing how these classes interact can be found at the bottom of this section.
+
+#### `ViewManager`
+
+This class is the interface between the ipython interactions and the underlying models. The `redraw` method is expected to be called in the `post_run_cell` IPython hook. All the other methods implement one of the magic commands in autoplot.
+
+This class is a proxy for the actual models, which implement the `View` interface and will perform the actual work needed to integrate with dtale or mpd3.
+
+When `redraw` is called, the class instance will scan the variables in the notebook's namespace, and look for pandas variables. The active view's `update_variables` is called with the filtered variables. Then, the `draw` method is called. Currently, only the active view's `update_variables` is called; however, it may be argued that syncing the `--freeze` and `--ignore` commands regardless of the current view is more natural. In that case, it will be useful to call `update_variables` in all views, rather than just the active one. We need to get more user feedback to decide which is the best approach.
+
+#### `_make_magic` (`AutoplotMagic`)
+
+The function `_make_magic` is a factory for instances of `AutoplotMagic`, in fact, it builds the class itself so that it can easily define the list of possible views in the `-v` argument.
+
+AutoplotMagic extends [`IPython.core.magic.Magics`](https://ipython.readthedocs.io/en/stable/api/generated/IPython.core.magic.html#IPython.core.magic.Magics), and defines the magic commands described [here](../README.md#modifying-the-plot--traces). This class translates the user input into calls to the `ViewManager`.
+
+#### `AutoplotDisplay`
+
+This class extends [`ipywidgets.Output`](https://ipywidgets.readthedocs.io/en/latest/examples/Output%20Widget.html), and defines the output area in which the graph is plotted. By matching the attributes `_model_name`, `_model_module_version` etc. with the equivalents in the JupyterLab extension class `AutoplotDisplayModel`, the two become linked and the output captured by the IPython component will be displayed wherever the JupyterLab component is rendered.
+
+This class also defines the `data_id` property, which is used by dtale to find out which instance (dataframe) is currently active.
+
+#### `Toast`
+
+This class defines some methods to dispatch DOM events that trigger toast notifications in the JupyterLab extension. These toasts change colour depending on their type, which can be one of 'error', 'warning', 'success' or 'info'.
+
+#### Backends
+
+##### `Dtaler`
+
+This is the class that implements the View interface for the dtale integration. It's responsible to keep track of the changed variables and dtale instances.
+
+##### `PlotterModel` and `Plotter`
+
+`PlotterModel` is the class that implements the View interface. It defines a dictionary of series names to their values, and one of dataframe names to the set of series names that were created from its columns. The `draw` method calls `plotter.plot()`, which initialises a matplotlib figure and axes, adds the defined traces to it and styles the figure.
+
+When a series is added, modified or deleted, the dictionaries will be updated and the appropriate calls will be made to the `Plotter` instance.
+
+The `Plotter` class manages the collection of `Trace` class instances and handles the graph plotting. It has a number of public methods like `update_trace_series()`, `update_trace_colour()` etc. which are used by the `PlotterModel` class to modify the plot and/or traces.
+
+The `Trace` class stores a matplotlib `Line2D` instance and some details about how it should be displayed. Like the `Plotter` class, it defines a number of public methods to allow it to be easily updated, like `update_series()` or `update_colour()`. It also handles the downsampling of long series.
```

### Comparing `jupyterlab-autoplot-0.2.0/README.md` & `jupyterlab-autoplot-0.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: jupyterlab-autoplot
+Version: 0.4.0
+Summary: The IPython component for the Autoplot JupyterLab extension.
+Home-page: https://github.com/man-group/jupyterlab-autoplot
+Author: Man Alpha Technology
+Author-email: ManAlphaTech@man.com
+License: BSD 3-Clause
+Keywords: jupyter,jupyterlab,matplotlib,mpld3,time series
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: Jupyter
+Requires-Python: >=3.6
+
 # JupyterLab Autoplot - IPython Component
 
 This IPython extension is one of the three components that make up the [JupyterLab Autoplot extension](../README.md).
 
 ## Development
 
 First you should follow the instructions [here](../autoplot-display#development) to install the JupyterLab extension component. Then, to apply the changes you have made to the IPython component:
```

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/__init__.py` & `jupyterlab-autoplot-0.4.0/autoplot/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/dtaler/__init__.py` & `jupyterlab-autoplot-0.4.0/autoplot/dtaler/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     Implements the dtale backend for this project. This class will call
     dtale.show for each new dataframe, given dtale's implementation that means
     we will have a single dtale server per kernel. This class uses the data_id
     field in AutoplotDisplay, which is populated from the frontend. That tells
     it which table is being shown to the user.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         # This is the current state of the variables we track. The tracked dict are the active variables, ignored and
         # forced_shown are variables the user wants to either ignore or stop ignoring
         self._tracked: Dict[str, VarData] = {}
         self._ignored: Set[str] = set()
         self._frozen = False
 
         # These variables are set using magic commands and informs us of the user's intentions before update_variables
@@ -101,15 +101,15 @@
         # 5. Update tracked variables which have changed
         updated_variables = _filter_updated(pandas_vars.items(), self._tracked.copy())
         for name, var in updated_variables.items():
             self._update_tracked_var(name, var)
 
     def draw(self, force: bool, output: AutoplotDisplay) -> None:
         refresh = False
-        current = dtale.get_instance(output.data_id)
+        current = dtale.get_instance(int(output.data_id))
         if current is None:
             current = Image(data=resource_filename(__name__, "assets/imgs/dtale.png"))
         # The conditionals below encode precedence. Whatever the user wants to show takes is the preferred value to
         # display, followed by new values and so on.
         if set(self._force_show) & set(self._tracked.keys()):
             for key in reversed(self._force_show):
                 if key in self._tracked:
@@ -169,32 +169,37 @@
         return result
 
     def _remove_tracked_var(self, var_name: str):
         vardata = self._tracked.pop(var_name, None)
         if vardata:
             data_id = vardata.dd._data_id
             dtale.global_state.cleanup(data_id)
-            self._deleted.append(vardata.dd._data_id)
+            try:
+                # this will be fixed in newer version of D-Tale
+                del dtale.global_state._default_store._data_names[var_name]
+            except KeyError:
+                pass
+            self._deleted.append(str(vardata.dd._data_id))
 
     def _add_tracked_var(self, name, var):
-        dd = self._dtale_show(var, ignore_duplicate=True, reaper_on=False, name=name, hide_shutdown=True)
+        dd = self._dtale_show(data=var, ignore_duplicate=True, reaper_on=False, name=name, hide_shutdown=True)
         self._tracked[name] = VarData(pdf=var, dd=dd)
         self._new.append(name)
 
     def _update_tracked_var(self, name, var):
         vardata = self._tracked[name]
         vardata.dd.data = var
         self._tracked[name] = VarData(pdf=var, dd=vardata.dd)
-        self._updated.append(vardata.dd._data_id)
+        self._updated.append(str(vardata.dd._data_id))
 
 
 def _removed_in_dtale(tracked: Iterable) -> Set[str]:
     removed: Set[str] = set()
     for name, vardata in tracked:
-        if dtale.global_state.find_data_id(vardata.dd._data_id) is None:
+        if dtale.get_instance(int(vardata.dd._data_id)) is None:
             removed.add(name)
     return removed
 
 
 def _filter_updated(pandas_vars: Iterable, tracked: Dict[str, VarData]) -> Dict[str, Union[pd.Series, pd.DataFrame]]:
     result: Dict[str, Union[pd.Series, pd.DataFrame]] = {}
 
@@ -203,12 +208,12 @@
         if vardata is not None and vardata.pdf is not var:
             result[name] = var
 
     return result
 
 
 def _next_dtale_data():
-    data_id = next(iter(dtale.global_state.get_data().keys()), None)
+    data_id = next(iter(dtale.global_state.keys()), None)
     if data_id is not None:
         return dtale.get_instance(data_id)
     else:
         return Image(data=resource_filename(__name__, "assets/imgs/dtale.png"))
```

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/extensions/autoplot_display.py` & `jupyterlab-autoplot-0.4.0/autoplot/extensions/autoplot_display.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import uuid
 
 from ipywidgets import Output
 from traitlets import Unicode
 
 # these values must mach those in autoplot-display/version.ts
 EXTENSION_TITLE = "Autoplot Display"
-EXTENSION_VERSION = "0.2.0"
+EXTENSION_VERSION = "0.4.0"
 MODULE_NAME = "@jupyter-widgets/autoplot-display"
 
 MODEL_NAME = "AutoplotDisplayModel"
 VIEW_NAME = "AutoplotDisplayView"
 
 
 class AutoplotDisplay(Output):
@@ -35,8 +35,8 @@
     _view_name = Unicode(VIEW_NAME).tag(sync=True)
     _view_module = Unicode(MODULE_NAME).tag(sync=True)
     _view_module_version = Unicode(EXTENSION_VERSION).tag(sync=True)
 
     # custom attributes
     title = Unicode(EXTENSION_TITLE).tag(sync=True)
     uuid = Unicode(uuid.uuid4().hex).tag(sync=True)
-    data_id = Unicode("").tag(sync=True)
+    data_id = Unicode("1").tag(sync=True)
```

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/extensions/toast.py` & `jupyterlab-autoplot-0.4.0/autoplot/extensions/toast.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/plotter/__init__.py` & `jupyterlab-autoplot-0.4.0/autoplot/plotter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -509,15 +509,15 @@
         else:
             raise TypeError(f"Can only set values of type 'set' or 'pd.Series', not '{type(value)}'")
 
     def get_plotted_dfs(self) -> Dict[str, Set[str]]:
         """Return the dictionary of series names associated with each dataframe."""
         return self._plotted_dfs
 
-    def _update_trace_if_changed(self, name: str, series: pd.Series, df_name: str = None):
+    def _update_trace_if_changed(self, name: str, series: pd.Series, df_name: Optional[str] = None):
         """Update the named trace with the given series.
 
         This function does nothing if the variable is not new and the series has
         not been modified.
 
         Parameters
         ----------
```

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/plotter/range_selector_utils.py` & `jupyterlab-autoplot-0.4.0/autoplot/plotter/range_selector_utils.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/plotter/trace.py` & `jupyterlab-autoplot-0.4.0/autoplot/plotter/trace.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 -------
 Trace
     Class to store a `Line2D` instance, and manage how it is displayed and updated.
 """
 
 import copy
 import datetime
-from typing import Tuple
+from typing import Optional, Tuple
 
 import matplotlib.lines as mpl_lines
 import numpy as np
 import pandas as pd
 from matplotlib.colors import is_color_like
 
 from autoplot.extensions.toast import Toast
@@ -59,15 +59,15 @@
         toast: Toast,
         name: str,
         series: pd.Series,
         index: int,
         max_length: int,
         *,
         visible: bool = True,
-        df_name: str = None,
+        df_name: Optional[str] = None,
     ):
         """Initialise a `Trace` instance.
 
         Parameters
         ----------
         toast: Toast
             The `Toast` class instance.
```

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/plugins/__init__.py` & `jupyterlab-autoplot-0.4.0/autoplot/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/plugins/bundles/interactiveLegend.js` & `jupyterlab-autoplot-0.4.0/autoplot/plugins/bundles/interactiveLegend.js`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/plugins/bundles/rangeSelectorButtons.js` & `jupyterlab-autoplot-0.4.0/autoplot/plugins/bundles/rangeSelectorButtons.js`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/plugins/bundles/saveImageButtons.js` & `jupyterlab-autoplot-0.4.0/autoplot/plugins/bundles/saveImageButtons.js`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/plugins/bundles/timeSeriesTooltip.js` & `jupyterlab-autoplot-0.4.0/autoplot/plugins/bundles/timeSeriesTooltip.js`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/plugins/interactive_legend.py` & `jupyterlab-autoplot-0.4.0/autoplot/plugins/interactive_legend.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/plugins/line_utils.py` & `jupyterlab-autoplot-0.4.0/autoplot/plugins/line_utils.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/plugins/range_selector_buttons.py` & `jupyterlab-autoplot-0.4.0/autoplot/plugins/range_selector_buttons.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Classes
 -------
 RangeSelectorButtons
     Class defining an mpld3 plugin to create range selector buttons.
 """
 
-from typing import List
+from typing import List, Optional
 
 import matplotlib.lines as mpl_lines
 import mpld3
 from pkg_resources import resource_filename
 
 from autoplot.plugins.line_utils import get_line_ids
 
@@ -19,54 +19,58 @@
 with open(_js_file_path, "r") as f:
     _js = f.read()
 
 
 class RangeSelectorButtons(mpld3.plugins.PluginBase):
     """Class defining an mpld3 plugin to create range selector buttons.
 
-    It extends `mpld3.plugins.PluginBase`, and can be connected to an mpld3 figure
-    using `mpld3.plugins.connect(fig, <instance>)`.
+        It extends `mpld3.plugins.PluginBase`, and can be connected to an mpld3 figure
+        using `mpld3.plugins.connect(fig, <instance>)`.
 
-    Properties
-    ----------
-    JAVASCRIPT: str
-        A string containing the necessary JavaScript code for the plugin.
-
-    css_: str
-        A string containing the necessary style definitions for the plugin.
-
-    Examples
-    --------
-    >>> import matplotlib.pyplot as plt
-import mpld3
-import numpy as np
-import pandas as pd
-%matplotlib inline
-    >>> mpld3.enable_notebook()
-    >>> fig, ax = plt.subplots(figsize=(10, 4))
-    >>> x = pd.date_range("2020-01-01", "2021-06-01")
-    >>> y = np.random.randn(len(x))
-    >>> lines = [ax.plot(x, y)]
-    >>> button_labels = ["fit", "reset", "5d", "14d", "1m", "6m", "ytd", "1y"]
-    >>> ax.autoscale(enable=True, axis="x", tight=True)
-    >>> mpld3.plugins.connect(fig, RangeSelectorButtons(button_labels, lines))
-    >>> plt.show()
-
-    Notes
-    -----
-    This plugin communicates with the `InteractiveLegend` plugin via the mpld3 Line
-    property `.isHidden`.
+        Properties
+        ----------
+        JAVASCRIPT: str
+            A string containing the necessary JavaScript code for the plugin.
+
+        css_: str
+            A string containing the necessary style definitions for the plugin.
+
+        Examples
+        --------
+        >>> import matplotlib.pyplot as plt
+    import mpld3
+    import numpy as np
+    import pandas as pd
+    %matplotlib inline
+        >>> mpld3.enable_notebook()
+        >>> fig, ax = plt.subplots(figsize=(10, 4))
+        >>> x = pd.date_range("2020-01-01", "2021-06-01")
+        >>> y = np.random.randn(len(x))
+        >>> lines = [ax.plot(x, y)]
+        >>> button_labels = ["fit", "reset", "5d", "14d", "1m", "6m", "ytd", "1y"]
+        >>> ax.autoscale(enable=True, axis="x", tight=True)
+        >>> mpld3.plugins.connect(fig, RangeSelectorButtons(button_labels, lines))
+        >>> plt.show()
+
+        Notes
+        -----
+        This plugin communicates with the `InteractiveLegend` plugin via the mpld3 Line
+        property `.isHidden`.
     """
 
     JAVASCRIPT = _js
     css_ = """.mpld3-range-selector-button-rect { cursor: pointer; }
               .mpld3-range-selector-button-text { cursor: pointer; }"""
 
     def __init__(
-        self, button_labels: List[str], lines: List[mpl_lines.Line2D] = None, margin_right: int = 0, fontsize: int = 13
+        self,
+        button_labels: List[str],
+        lines: Optional[List[mpl_lines.Line2D]] = None,
+        margin_right: int = 0,
+        fontsize: int = 13,
     ):
         """Initialise a `RangeSelectorButtons` instance.
 
         Parameters
         ----------
         button_labels: List[str]
             List of button labels. Each label must either be of the form
```

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/plugins/save_image_buttons.py` & `jupyterlab-autoplot-0.4.0/autoplot/plugins/save_image_buttons.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/plugins/time_series_tooltip.py` & `jupyterlab-autoplot-0.4.0/autoplot/plugins/time_series_tooltip.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/utils/constants.py` & `jupyterlab-autoplot-0.4.0/autoplot/utils/constants.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/view_manager/__init__.py` & `jupyterlab-autoplot-0.4.0/autoplot/view_manager/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     def active_view(self) -> View:
         return self._views[self._active]
 
     @property
     def view_names(self) -> List[str]:
         return list(self._views.keys())
 
-    def redraw(self):
+    def redraw(self) -> None:
         pandas_vars: Dict[str, Union[pd.Series, pd.DataFrame]] = {}
         for name, var in self._shell.user_ns.items():
             if not name.startswith("_") and name not in self._reserved and self._is_pandas(var):
                 pandas_vars[name] = var
 
         self.active_view.update_variables(pandas_vars)
         self.active_view.draw(self._changed, self._output)
@@ -271,24 +271,24 @@
             return self.active_view.update_max_series_length(toast, sample)
         except NotImplementedError:
             toast.show(f"{self._active} does not implement max series length", ToastType.warning)
 
     def set_ylabel(self, toast: Toast, ylabel: str) -> None:
         """Set the y axis label.
 
-         If the new label is different, set `self._changed` to True.
+        If the new label is different, set `self._changed` to True.
 
-         Parameters
-         ----------
-         toast: Toast
-             The `Toast` class instance.
-
-         ylabel: str
-             New label for the y axis. If it is an empty string, no label will be used.
-         """
+        Parameters
+        ----------
+        toast: Toast
+            The `Toast` class instance.
+
+        ylabel: str
+            New label for the y axis. If it is an empty string, no label will be used.
+        """
         try:
             return self.active_view.set_ylabel(toast, ylabel)
         except NotImplementedError:
             toast.show(f"{self._active} does not implement changing ylabel", ToastType.warning)
 
     def set_plot_height(self, toast: Toast, height: int) -> None:
         """Validate and set the height of the figure.
```

### Comparing `jupyterlab-autoplot-0.2.0/autoplot/view_manager/variable_utils.py` & `jupyterlab-autoplot-0.4.0/autoplot/view_manager/variable_utils.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.2.0/jupyterlab_autoplot.egg-info/PKG-INFO` & `jupyterlab-autoplot-0.4.0/jupyterlab_autoplot.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,73 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: jupyterlab-autoplot
-Version: 0.2.0
+Version: 0.4.0
 Summary: The IPython component for the Autoplot JupyterLab extension.
 Home-page: https://github.com/man-group/jupyterlab-autoplot
 Author: Man Alpha Technology
 Author-email: ManAlphaTech@man.com
 License: BSD 3-Clause
-Description: # JupyterLab Autoplot - IPython Component
-        
-        This IPython extension is one of the three components that make up the [JupyterLab Autoplot extension](../README.md).
-        
-        ## Development
-        
-        First you should follow the instructions [here](../autoplot-display#development) to install the JupyterLab extension component. Then, to apply the changes you have made to the IPython component:
-        
-        ```sh
-        cd ipython-extension/
-        python -m pip install -e .
-        ```
-        
-        You can then reload the extension in your JupyterLab instance with `%reload_ext autoplot` (you may need to restart the kernel first).
-        
-        ### Description of classes
-        
-        Each of the following classes will be initialised **once** in the `load_ipython_extension()` function, and, where necessary, these instances will be accessible to each other. A diagram showing how these classes interact can be found at the bottom of this section.
-        
-        #### `ViewManager`
-        
-        This class is the interface between the ipython interactions and the underlying models. The `redraw` method is expected to be called in the `post_run_cell` IPython hook. All the other methods implement one of the magic commands in autoplot.
-        
-        This class is a proxy for the actual models, which implement the `View` interface and will perform the actual work needed to integrate with dtale or mpd3.
-        
-        When `redraw` is called, the class instance will scan the variables in the notebook's namespace, and look for pandas variables. The active view's `update_variables` is called with the filtered variables. Then, the `draw` method is called. Currently, only the active view's `update_variables` is called; however, it may be argued that syncing the `--freeze` and `--ignore` commands regardless of the current view is more natural. In that case, it will be useful to call `update_variables` in all views, rather than just the active one. We need to get more user feedback to decide which is the best approach.
-        
-        #### `_make_magic` (`AutoplotMagic`)
-        
-        The function `_make_magic` is a factory for instances of `AutoplotMagic`, in fact, it builds the class itself so that it can easily define the list of possible views in the `-v` argument.
-        
-        AutoplotMagic extends [`IPython.core.magic.Magics`](https://ipython.readthedocs.io/en/stable/api/generated/IPython.core.magic.html#IPython.core.magic.Magics), and defines the magic commands described [here](../README.md#modifying-the-plot--traces). This class translates the user input into calls to the `ViewManager`.
-        
-        #### `AutoplotDisplay`
-        
-        This class extends [`ipywidgets.Output`](https://ipywidgets.readthedocs.io/en/latest/examples/Output%20Widget.html), and defines the output area in which the graph is plotted. By matching the attributes `_model_name`, `_model_module_version` etc. with the equivalents in the JupyterLab extension class `AutoplotDisplayModel`, the two become linked and the output captured by the IPython component will be displayed wherever the JupyterLab component is rendered.
-        
-        This class also defines the `data_id` property, which is used by dtale to find out which instance (dataframe) is currently active.
-        
-        #### `Toast`
-        
-        This class defines some methods to dispatch DOM events that trigger toast notifications in the JupyterLab extension. These toasts change colour depending on their type, which can be one of 'error', 'warning', 'success' or 'info'.
-        
-        #### Backends
-        
-        ##### `Dtaler`
-        
-        This is the class that implements the View interface for the dtale integration. It's responsible to keep track of the changed variables and dtale instances.
-        
-        ##### `PlotterModel` and `Plotter`
-        
-        `PlotterModel` is the class that implements the View interface. It defines a dictionary of series names to their values, and one of dataframe names to the set of series names that were created from its columns. The `draw` method calls `plotter.plot()`, which initialises a matplotlib figure and axes, adds the defined traces to it and styles the figure.
-        
-        When a series is added, modified or deleted, the dictionaries will be updated and the appropriate calls will be made to the `Plotter` instance.
-        
-        The `Plotter` class manages the collection of `Trace` class instances and handles the graph plotting. It has a number of public methods like `update_trace_series()`, `update_trace_colour()` etc. which are used by the `PlotterModel` class to modify the plot and/or traces.
-        
-        The `Trace` class stores a matplotlib `Line2D` instance and some details about how it should be displayed. Like the `Plotter` class, it defines a number of public methods to allow it to be easily updated, like `update_series()` or `update_colour()`. It also handles the downsampling of long series.
-        
 Keywords: jupyter,jupyterlab,matplotlib,mpld3,time series
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Jupyter
 Requires-Python: >=3.6
+
+# JupyterLab Autoplot - IPython Component
+
+This IPython extension is one of the three components that make up the [JupyterLab Autoplot extension](../README.md).
+
+## Development
+
+First you should follow the instructions [here](../autoplot-display#development) to install the JupyterLab extension component. Then, to apply the changes you have made to the IPython component:
+
+```sh
+cd ipython-extension/
+python -m pip install -e .
+```
+
+You can then reload the extension in your JupyterLab instance with `%reload_ext autoplot` (you may need to restart the kernel first).
+
+### Description of classes
+
+Each of the following classes will be initialised **once** in the `load_ipython_extension()` function, and, where necessary, these instances will be accessible to each other. A diagram showing how these classes interact can be found at the bottom of this section.
+
+#### `ViewManager`
+
+This class is the interface between the ipython interactions and the underlying models. The `redraw` method is expected to be called in the `post_run_cell` IPython hook. All the other methods implement one of the magic commands in autoplot.
+
+This class is a proxy for the actual models, which implement the `View` interface and will perform the actual work needed to integrate with dtale or mpd3.
+
+When `redraw` is called, the class instance will scan the variables in the notebook's namespace, and look for pandas variables. The active view's `update_variables` is called with the filtered variables. Then, the `draw` method is called. Currently, only the active view's `update_variables` is called; however, it may be argued that syncing the `--freeze` and `--ignore` commands regardless of the current view is more natural. In that case, it will be useful to call `update_variables` in all views, rather than just the active one. We need to get more user feedback to decide which is the best approach.
+
+#### `_make_magic` (`AutoplotMagic`)
+
+The function `_make_magic` is a factory for instances of `AutoplotMagic`, in fact, it builds the class itself so that it can easily define the list of possible views in the `-v` argument.
+
+AutoplotMagic extends [`IPython.core.magic.Magics`](https://ipython.readthedocs.io/en/stable/api/generated/IPython.core.magic.html#IPython.core.magic.Magics), and defines the magic commands described [here](../README.md#modifying-the-plot--traces). This class translates the user input into calls to the `ViewManager`.
+
+#### `AutoplotDisplay`
+
+This class extends [`ipywidgets.Output`](https://ipywidgets.readthedocs.io/en/latest/examples/Output%20Widget.html), and defines the output area in which the graph is plotted. By matching the attributes `_model_name`, `_model_module_version` etc. with the equivalents in the JupyterLab extension class `AutoplotDisplayModel`, the two become linked and the output captured by the IPython component will be displayed wherever the JupyterLab component is rendered.
+
+This class also defines the `data_id` property, which is used by dtale to find out which instance (dataframe) is currently active.
+
+#### `Toast`
+
+This class defines some methods to dispatch DOM events that trigger toast notifications in the JupyterLab extension. These toasts change colour depending on their type, which can be one of 'error', 'warning', 'success' or 'info'.
+
+#### Backends
+
+##### `Dtaler`
+
+This is the class that implements the View interface for the dtale integration. It's responsible to keep track of the changed variables and dtale instances.
+
+##### `PlotterModel` and `Plotter`
+
+`PlotterModel` is the class that implements the View interface. It defines a dictionary of series names to their values, and one of dataframe names to the set of series names that were created from its columns. The `draw` method calls `plotter.plot()`, which initialises a matplotlib figure and axes, adds the defined traces to it and styles the figure.
+
+When a series is added, modified or deleted, the dictionaries will be updated and the appropriate calls will be made to the `Plotter` instance.
+
+The `Plotter` class manages the collection of `Trace` class instances and handles the graph plotting. It has a number of public methods like `update_trace_series()`, `update_trace_colour()` etc. which are used by the `PlotterModel` class to modify the plot and/or traces.
+
+The `Trace` class stores a matplotlib `Line2D` instance and some details about how it should be displayed. Like the `Plotter` class, it defines a number of public methods to allow it to be easily updated, like `update_series()` or `update_colour()`. It also handles the downsampling of long series.
```

### Comparing `jupyterlab-autoplot-0.2.0/jupyterlab_autoplot.egg-info/SOURCES.txt` & `jupyterlab-autoplot-0.4.0/jupyterlab_autoplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.2.0/setup.py` & `jupyterlab-autoplot-0.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,25 +5,25 @@
     with open("README.md", "r", encoding="utf-8") as f:
         desc = f.read()
     return desc
 
 
 setup(
     name="jupyterlab-autoplot",
-    version="0.2.0",
+    version="0.4.0",
     author="Man Alpha Technology",
     author_email="ManAlphaTech@man.com",
     license="BSD 3-Clause",
     description="The IPython component for the Autoplot JupyterLab extension.",
     long_description=get_long_description(),
     url="https://github.com/man-group/jupyterlab-autoplot",
     keywords=["jupyter", "jupyterlab", "matplotlib", "mpld3", "time series"],
     packages=find_packages(include=["autoplot", "autoplot.*"], exclude=["tests", "tests.*"]),
     include_package_data=True,
-    install_requires=["ipywidgets", "ipython", "numpy", "pandas", "matplotlib", "mpld3", "dtale>=1.16.0,<1.36"],
+    install_requires=["ipywidgets", "ipython", "numpy", "pandas", "matplotlib", "mpld3", "dtale>=2.15.2"],
     tests_require=["pytest", "pytest-cov", "mock"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Framework :: Jupyter",
     ],
```

