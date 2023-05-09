# Comparing `tmp/magic-class-0.6.9.tar.gz` & `tmp/magic_class-0.7.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magic-class-0.6.9.tar", last modified: Tue Aug 30 14:08:40 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `magic-class-0.6.9.tar` & `magic_class-0.7.0rc0.tar`

### file list

```diff
@@ -1,137 +1,132 @@
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:40.155543 magic-class-0.6.9/
--rw-rw-rw-   0        0        0     1546 2021-10-20 15:41:30.000000 magic-class-0.6.9/LICENSE
--rw-rw-rw-   0        0        0     4525 2022-08-30 14:08:40.151543 magic-class-0.6.9/PKG-INFO
--rw-rw-rw-   0        0        0     4177 2022-08-02 09:42:39.000000 magic-class-0.6.9/README.md
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:37.933486 magic-class-0.6.9/magic_class.egg-info/
--rw-rw-rw-   0        0        0     4525 2022-08-30 14:08:31.000000 magic-class-0.6.9/magic_class.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3396 2022-08-30 14:08:33.000000 magic-class-0.6.9/magic_class.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-30 14:08:31.000000 magic-class-0.6.9/magic_class.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2022-08-30 14:08:31.000000 magic-class-0.6.9/magic_class.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-08-30 14:08:31.000000 magic-class-0.6.9/magic_class.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:38.101776 magic-class-0.6.9/magicclass/
--rw-rw-rw-   0        0        0     1968 2022-08-30 14:03:05.000000 magic-class-0.6.9/magicclass/__init__.py
--rw-rw-rw-   0        0        0     1285 2022-07-20 12:55:15.000000 magic-class-0.6.9/magicclass/_app.py
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:38.209035 magic-class-0.6.9/magicclass/_gui/
--rw-rw-rw-   0        0        0      169 2022-05-07 05:53:09.000000 magic-class-0.6.9/magicclass/_gui/__init__.py
--rw-rw-rw-   0        0        0    49425 2022-08-30 07:01:55.000000 magic-class-0.6.9/magicclass/_gui/_base.py
--rw-rw-rw-   0        0        0     1412 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/_gui/_dock_widget.py
--rw-rw-rw-   0        0        0     5449 2022-08-30 13:39:04.000000 magic-class-0.6.9/magicclass/_gui/_function_gui.py
--rw-rw-rw-   0        0        0     6986 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/_gui/_icon.py
--rw-rw-rw-   0        0        0    11488 2022-05-07 05:53:09.000000 magic-class-0.6.9/magicclass/_gui/_macro.py
--rw-rw-rw-   0        0        0    10632 2022-08-30 13:58:24.000000 magic-class-0.6.9/magicclass/_gui/_message_box.py
--rw-rw-rw-   0        0        0      725 2022-05-07 05:53:09.000000 magic-class-0.6.9/magicclass/_gui/_napari_type.py
--rw-rw-rw-   0        0        0    25292 2022-08-30 14:03:53.000000 magic-class-0.6.9/magicclass/_gui/class_gui.py
--rw-rw-rw-   0        0        0     5100 2022-08-30 07:44:16.000000 magic-class-0.6.9/magicclass/_gui/keybinding.py
--rw-rw-rw-   0        0        0    10819 2022-08-30 07:04:53.000000 magic-class-0.6.9/magicclass/_gui/menu_gui.py
--rw-rw-rw-   0        0        0    12786 2022-08-30 14:00:57.000000 magic-class-0.6.9/magicclass/_gui/mgui_ext.py
--rw-rw-rw-   0        0        0    11442 2022-08-28 07:45:24.000000 magic-class-0.6.9/magicclass/_gui/toolbar.py
--rw-rw-rw-   0        0        0     3444 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/_gui/utils.py
--rw-rw-rw-   0        0        0     1426 2022-08-30 13:56:29.000000 magic-class-0.6.9/magicclass/_register_types.py
--rw-rw-rw-   0        0        0    21222 2022-08-30 07:05:07.000000 magic-class-0.6.9/magicclass/core.py
--rw-rw-rw-   0        0        0     4308 2022-08-01 13:19:47.000000 magic-class-0.6.9/magicclass/core.pyi
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:38.230645 magic-class-0.6.9/magicclass/ext/
--rw-rw-rw-   0        0        0       51 2022-02-14 08:22:00.000000 magic-class-0.6.9/magicclass/ext/__init__.py
--rw-rw-rw-   0        0        0     1788 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/ext/_doc.py
--rw-rw-rw-   0        0        0      270 2022-04-05 10:25:52.000000 magic-class-0.6.9/magicclass/ext/_shared_utils.py
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:38.254848 magic-class-0.6.9/magicclass/ext/dask/
--rw-rw-rw-   0        0        0      107 2022-05-07 05:53:08.000000 magic-class-0.6.9/magicclass/ext/dask/__init__.py
--rw-rw-rw-   0        0        0     5973 2022-08-12 09:12:56.000000 magic-class-0.6.9/magicclass/ext/dask/progress.py
--rw-rw-rw-   0        0        0     3411 2022-05-07 05:53:08.000000 magic-class-0.6.9/magicclass/ext/dask/resource.py
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:38.297493 magic-class-0.6.9/magicclass/ext/napari/
--rw-rw-rw-   0        0        0      257 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/ext/napari/__init__.py
--rw-rw-rw-   0        0        0     4714 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/ext/napari/_magicgui.py
--rw-rw-rw-   0        0        0     1610 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/ext/napari/types.py
--rw-rw-rw-   0        0        0     2921 2022-05-07 05:53:08.000000 magic-class-0.6.9/magicclass/ext/napari/utils.py
--rw-rw-rw-   0        0        0     2947 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/ext/napari/viewer.py
--rw-rw-rw-   0        0        0     1728 2022-06-27 02:42:26.000000 magic-class-0.6.9/magicclass/ext/napari/widgets.py
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:38.341205 magic-class-0.6.9/magicclass/ext/pandas/
--rw-rw-rw-   0        0        0      230 2022-06-19 06:38:34.000000 magic-class-0.6.9/magicclass/ext/pandas/__init__.py
--rw-rw-rw-   0        0        0     3599 2022-06-19 06:38:34.000000 magic-class-0.6.9/magicclass/ext/pandas/_dataframe.py
--rw-rw-rw-   0        0        0      418 2022-06-19 06:38:34.000000 magic-class-0.6.9/magicclass/ext/pandas/io.py
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:38.541986 magic-class-0.6.9/magicclass/ext/pyqtgraph/
--rw-rw-rw-   0        0        0     2167 2022-02-14 08:22:05.000000 magic-class-0.6.9/magicclass/ext/pyqtgraph/__init__.py
--rw-rw-rw-   0        0        0      250 2022-02-14 08:22:05.000000 magic-class-0.6.9/magicclass/ext/pyqtgraph/_const.py
--rw-rw-rw-   0        0        0     6120 2022-04-05 10:26:20.000000 magic-class-0.6.9/magicclass/ext/pyqtgraph/components.py
--rw-rw-rw-   0        0        0    21293 2022-08-20 05:20:38.000000 magic-class-0.6.9/magicclass/ext/pyqtgraph/graph_items.py
--rw-rw-rw-   0        0        0     1734 2022-02-14 08:22:05.000000 magic-class-0.6.9/magicclass/ext/pyqtgraph/mouse_event.py
--rw-rw-rw-   0        0        0     3220 2022-08-03 07:20:16.000000 magic-class-0.6.9/magicclass/ext/pyqtgraph/plot_api.py
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:38.629376 magic-class-0.6.9/magicclass/ext/pyqtgraph/tests/
--rw-rw-rw-   0        0        0        0 2021-12-30 11:05:01.000000 magic-class-0.6.9/magicclass/ext/pyqtgraph/tests/__init__.py
--rw-rw-rw-   0        0        0     3368 2022-07-04 16:04:30.000000 magic-class-0.6.9/magicclass/ext/pyqtgraph/tests/test_qtgraph.py
--rw-rw-rw-   0        0        0    30852 2022-08-30 13:33:00.000000 magic-class-0.6.9/magicclass/ext/pyqtgraph/widgets.py
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:38.850620 magic-class-0.6.9/magicclass/ext/qtconsole/
--rw-rw-rw-   0        0        0      766 2022-02-14 08:22:01.000000 magic-class-0.6.9/magicclass/ext/qtconsole/__init__.py
--rw-rw-rw-   0        0        0     3243 2022-02-14 08:22:05.000000 magic-class-0.6.9/magicclass/ext/qtconsole/_qt.py
--rw-rw-rw-   0        0        0     1519 2022-04-07 01:52:54.000000 magic-class-0.6.9/magicclass/ext/qtconsole/widgets.py
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:39.092211 magic-class-0.6.9/magicclass/ext/vispy/
--rw-rw-rw-   0        0        0      362 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/ext/vispy/__init__.py
--rw-rw-rw-   0        0        0     3980 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/ext/vispy/_base.py
--rw-rw-rw-   0        0        0     6034 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/ext/vispy/layer2d.py
--rw-rw-rw-   0        0        0    11715 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/ext/vispy/layer3d.py
--rw-rw-rw-   0        0        0      698 2022-07-06 01:24:26.000000 magic-class-0.6.9/magicclass/ext/vispy/layerlist.py
--rw-rw-rw-   0        0        0     3256 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/ext/vispy/plot_api.py
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:39.109397 magic-class-0.6.9/magicclass/ext/vispy/tests/
--rw-rw-rw-   0        0        0        0 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/ext/vispy/tests/__init__.py
--rw-rw-rw-   0        0        0     1134 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/ext/vispy/tests/test_vispy2d.py
--rw-rw-rw-   0        0        0    11197 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/ext/vispy/widgets2d.py
--rw-rw-rw-   0        0        0     3969 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/ext/vispy/widgets3d.py
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:39.146952 magic-class-0.6.9/magicclass/ext/vtk/
--rw-rw-rw-   0        0        0      237 2022-04-04 15:47:42.000000 magic-class-0.6.9/magicclass/ext/vtk/__init__.py
--rw-rw-rw-   0        0        0     5200 2022-06-19 06:38:34.000000 magic-class-0.6.9/magicclass/ext/vtk/components.py
--rw-rw-rw-   0        0        0     1055 2022-06-19 06:38:34.000000 magic-class-0.6.9/magicclass/ext/vtk/const.py
--rw-rw-rw-   0        0        0     5089 2022-06-19 06:38:34.000000 magic-class-0.6.9/magicclass/ext/vtk/volume.py
--rw-rw-rw-   0        0        0     4391 2022-04-04 15:47:42.000000 magic-class-0.6.9/magicclass/ext/vtk/widgets.py
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:39.170043 magic-class-0.6.9/magicclass/fields/
--rw-rw-rw-   0        0        0      194 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/fields/__init__.py
--rw-rw-rw-   0        0        0    26960 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/fields/_fields.py
--rw-rw-rw-   0        0        0    14215 2022-08-30 06:58:39.000000 magic-class-0.6.9/magicclass/fields/_group.py
--rw-rw-rw-   0        0        0    10773 2022-06-19 06:38:34.000000 magic-class-0.6.9/magicclass/help.py
--rw-rw-rw-   0        0        0     5880 2022-03-07 03:29:51.000000 magic-class-0.6.9/magicclass/signature.py
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:39.176045 magic-class-0.6.9/magicclass/stylesheets/
--rw-rw-rw-   0        0        0     1268 2022-02-14 08:22:06.000000 magic-class-0.6.9/magicclass/stylesheets/__init__.py
--rw-rw-rw-   0        0        0      802 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/testing.py
--rw-rw-rw-   0        0        0    11621 2022-08-30 06:34:40.000000 magic-class-0.6.9/magicclass/types.py
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:39.312070 magic-class-0.6.9/magicclass/utils/
--rw-rw-rw-   0        0        0      503 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/utils/__init__.py
--rw-rw-rw-   0        0        0     3189 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/utils/_click.py
--rw-rw-rw-   0        0        0     6670 2022-07-20 12:53:20.000000 magic-class-0.6.9/magicclass/utils/_functions.py
--rw-rw-rw-   0        0        0     3441 2022-08-30 07:28:01.000000 magic-class-0.6.9/magicclass/utils/qt.py
--rw-rw-rw-   0        0        0    25661 2022-08-12 09:02:42.000000 magic-class-0.6.9/magicclass/utils/qthreading.py
--rw-rw-rw-   0        0        0      351 2022-05-07 05:53:09.000000 magic-class-0.6.9/magicclass/utils/qtsignal.py
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:39.561332 magic-class-0.6.9/magicclass/widgets/
--rw-rw-rw-   0        0        0     1674 2022-07-20 12:55:15.000000 magic-class-0.6.9/magicclass/widgets/__init__.py
--rw-rw-rw-   0        0        0     8380 2022-06-20 01:23:20.000000 magic-class-0.6.9/magicclass/widgets/_mpl_canvas.py
--rw-rw-rw-   0        0        0    10365 2022-02-14 08:22:06.000000 magic-class-0.6.9/magicclass/widgets/color.py
--rw-rw-rw-   0        0        0    21144 2022-07-07 12:24:19.000000 magic-class-0.6.9/magicclass/widgets/containers.py
--rw-rw-rw-   0        0        0    13673 2022-08-04 12:31:45.000000 magic-class-0.6.9/magicclass/widgets/logger.py
--rw-rw-rw-   0        0        0    14495 2022-07-20 12:55:15.000000 magic-class-0.6.9/magicclass/widgets/misc.py
--rw-rw-rw-   0        0        0    15020 2022-06-20 01:23:20.000000 magic-class-0.6.9/magicclass/widgets/plot.py
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:39.682684 magic-class-0.6.9/magicclass/widgets/pywidgets/
--rw-rw-rw-   0        0        0     1997 2022-02-14 08:22:01.000000 magic-class-0.6.9/magicclass/widgets/pywidgets/__init__.py
--rw-rw-rw-   0        0        0     4979 2022-02-14 08:22:06.000000 magic-class-0.6.9/magicclass/widgets/pywidgets/dict.py
--rw-rw-rw-   0        0        0     5187 2022-02-14 08:22:06.000000 magic-class-0.6.9/magicclass/widgets/pywidgets/list.py
--rw-rw-rw-   0        0        0     3858 2022-06-19 06:38:34.000000 magic-class-0.6.9/magicclass/widgets/pywidgets/object.py
--rw-rw-rw-   0        0        0     4476 2022-02-14 08:22:06.000000 magic-class-0.6.9/magicclass/widgets/pywidgets/tree.py
--rw-rw-rw-   0        0        0     2619 2022-06-19 06:38:34.000000 magic-class-0.6.9/magicclass/widgets/separator.py
--rw-rw-rw-   0        0        0    11901 2022-03-14 01:12:30.000000 magic-class-0.6.9/magicclass/widgets/sequence.py
--rw-rw-rw-   0        0        0     2696 2022-07-20 12:55:15.000000 magic-class-0.6.9/magicclass/widgets/utils.py
--rw-rw-rw-   0        0        0    12150 2022-08-30 07:01:43.000000 magic-class-0.6.9/magicclass/wrappers.py
--rw-rw-rw-   0        0        0       42 2022-08-30 14:08:40.156545 magic-class-0.6.9/setup.cfg
--rw-rw-rw-   0        0        0     1097 2022-08-28 07:11:55.000000 magic-class-0.6.9/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-30 14:08:40.144550 magic-class-0.6.9/tests/
--rw-rw-rw-   0        0        0       68 2022-03-06 12:44:36.000000 magic-class-0.6.9/tests/__init__.py
--rw-rw-rw-   0        0        0     5136 2022-06-19 06:38:34.000000 magic-class-0.6.9/tests/test_bind.py
--rw-rw-rw-   0        0        0     4232 2022-06-19 06:38:34.000000 magic-class-0.6.9/tests/test_callbacks.py
--rw-rw-rw-   0        0        0     7391 2022-07-20 12:53:20.000000 magic-class-0.6.9/tests/test_construction.py
--rw-rw-rw-   0        0        0     1001 2022-02-14 08:22:01.000000 magic-class-0.6.9/tests/test_custom_widgets.py
--rw-rw-rw-   0        0        0    14792 2022-08-28 07:24:55.000000 magic-class-0.6.9/tests/test_fields.py
--rw-rw-rw-   0        0        0     2457 2022-02-14 08:22:51.000000 magic-class-0.6.9/tests/test_inheritance.py
--rw-rw-rw-   0        0        0     2234 2022-04-05 12:27:42.000000 magic-class-0.6.9/tests/test_keybindings.py
--rw-rw-rw-   0        0        0     3704 2022-08-02 07:56:49.000000 magic-class-0.6.9/tests/test_macro.py
--rw-rw-rw-   0        0        0     2566 2022-06-19 06:38:34.000000 magic-class-0.6.9/tests/test_magicgui.py
--rw-rw-rw-   0        0        0     1454 2022-03-06 12:44:36.000000 magic-class-0.6.9/tests/test_methods.py
--rw-rw-rw-   0        0        0     2398 2022-07-20 12:53:20.000000 magic-class-0.6.9/tests/test_popups.py
--rw-rw-rw-   0        0        0      887 2022-02-14 08:22:01.000000 magic-class-0.6.9/tests/test_running.py
--rw-rw-rw-   0        0        0      945 2022-08-30 07:30:57.000000 magic-class-0.6.9/tests/test_widget_types.py
--rw-rw-rw-   0        0        0     8133 2022-07-20 12:53:20.000000 magic-class-0.6.9/tests/test_wrappers.py
--rw-rw-rw-   0        0        0     2434 2022-03-07 05:12:59.000000 magic-class-0.6.9/tests/test_wraps.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/__init__.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_app.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_register_types.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/command_palette.py
+-rw-r--r--   0        0        0    23018 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/core.py
+-rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/core.pyi
+-rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/help.py
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/plot_api.py
+-rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/signature.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/testing.py
+-rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/undo.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/__init__.py
+-rw-r--r--   0        0        0    46951 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/_base.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/_dock_widget.py
+-rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/_function_gui.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/_gui_modes.py
+-rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/_icon.py
+-rw-r--r--   0        0        0    21659 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/_macro.py
+-rw-r--r--   0        0        0    13059 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/_macro_utils.py
+-rw-r--r--   0        0        0    10935 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/_message_box.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/_napari_type.py
+-rw-r--r--   0        0        0    26462 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/class_gui.py
+-rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/keybinding.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/menu_gui.py
+-rw-r--r--   0        0        0    13434 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/mgui_ext.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/runner.py
+-rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/toolbar.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/_gui/utils.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/__init__.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/_doc.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/_shared_utils.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/dask/__init__.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/dask/progress.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/dask/resource.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/napari/__init__.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/napari/_magicgui.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/napari/types.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/napari/utils.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/napari/viewer.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/napari/widgets.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pandas/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pandas/_viewer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pandas/tests/__init__.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pandas/tests/test_viewer.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/polars/__init__.py
+-rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/polars/_viewer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/polars/tests/__init__.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/polars/tests/test_viewer.py
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/_const.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/components.py
+-rw-r--r--   0        0        0    22882 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/graph_items.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/mouse_event.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/plot_api.py
+-rw-r--r--   0        0        0    32686 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/widgets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/tests/__init__.py
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/tests/test_qtgraph.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/qtconsole/__init__.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/qtconsole/_qt.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/qtconsole/widgets.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/__init__.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/_base.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/camera.py
+-rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/layer2d.py
+-rw-r--r--   0        0        0    20691 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/layer3d.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/layerlist.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/plot_api.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/widgets2d.py
+-rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/widgets3d.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/tests/__init__.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vispy/tests/test_vispy2d.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vtk/__init__.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vtk/components.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vtk/const.py
+-rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vtk/volume.py
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/ext/vtk/widgets.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/fields/__init__.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/fields/_define.py
+-rw-r--r--   0        0        0    29294 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/fields/_fields.py
+-rw-r--r--   0        0        0    14681 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/fields/_group.py
+-rw-r--r--   0        0        0    10491 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/fields/_property.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/functools/__init__.py
+-rw-r--r--   0        0        0     8480 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/functools/_dispatch.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/functools/_partial.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/functools/_wraps.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/logging/__init__.py
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/logging/core.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/stylesheets/__init__.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/types/__init__.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/types/_bound.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/types/_choices.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/types/_const.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/types/_expr.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/types/_optional.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/types/_path.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/types/_union.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/utils/__init__.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/utils/_click.py
+-rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/utils/_functions.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/utils/_recent.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/utils/qt.py
+-rw-r--r--   0        0        0    31513 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/utils/qthreading.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/utils/qtsignal.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/__init__.py
+-rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/_mpl_canvas.py
+-rw-r--r--   0        0        0    25094 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/codeedit.py
+-rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/color.py
+-rw-r--r--   0        0        0    23314 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/containers.py
+-rw-r--r--   0        0        0    11197 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/eval.py
+-rw-r--r--   0        0        0    15200 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/logger.py
+-rw-r--r--   0        0        0    18103 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/misc.py
+-rw-r--r--   0        0        0    15329 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/plot.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/separator.py
+-rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/toggle_switch.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/utils.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/pywidgets/__init__.py
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/pywidgets/dict.py
+-rw-r--r--   0        0        0     5187 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/pywidgets/list.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/pywidgets/object.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/pywidgets/tree.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/tests/__init__.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/widgets/tests/test_eval.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/wrappers/__init__.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/wrappers/_abstractapi.py
+-rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/wrappers/_confirm.py
+-rw-r--r--   0        0        0     8771 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/wrappers/_misc.py
+-rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/magicclass/wrappers/_preview.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/.gitignore
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/LICENSE
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/README.md
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     7383 2020-02-02 00:00:00.000000 magic_class-0.7.0rc0/PKG-INFO
```

### Comparing `magic-class-0.6.9/LICENSE` & `magic_class-0.7.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `magic-class-0.6.9/PKG-INFO` & `magic_class-0.7.0rc0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,18 @@
-Metadata-Version: 2.1
-Name: magic-class
-Version: 0.6.9
-Summary: Generate multifunctional GUIs from classes
-Download-URL: https://github.com/hanjinliu/magic-class
-Author: Hanjin Liu
-Author-email: liuhanjin-sc@g.ecc.u-tokyo.ac.jp
-License: BSD 3-Clause
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![License BSD-3](https://img.shields.io/pypi/l/magic-class.svg?color=green)](https://github.com/hanjinliu/magic-class/raw/main/LICENSE)
-[![Downloads](https://pepy.tech/badge/magic-class/month)](https://pepy.tech/project/magic-class)
+[![Python package index download statistics](https://img.shields.io/pypi/dm/magic-class.svg)](https://pypistats.org/packages/magic-class)
 [![PyPI version](https://badge.fury.io/py/magic-class.svg)](https://badge.fury.io/py/magic-class)
 [![Conda version](https://anaconda.org/conda-forge/magic-class/badges/version.svg)](https://anaconda.org/conda-forge/magic-class/badges/version.svg)
 
 
 # magic-class
 
 ![](https://github.com/hanjinliu/magic-class/blob/main/Figs/Example.gif)
 
-`magic-class` makes GUI development as easy as daily coding by converting well-typed Python class directly into GUI. It is powered by [magicgui](https://github.com/napari/magicgui) and has smooth interface with [napari](https://github.com/napari/napari). `magic-class` is also implemented with useful widgets such as `matplotlib` figure canvas, logger widget and color edit.
+`magic-class` makes GUI development as easy as daily coding by converting well-typed Python class directly into GUI. It is powered by [magicgui](https://github.com/pyapp-kit/magicgui) and has a smooth interface with [napari](https://github.com/napari/napari). `magic-class` is also implemented with useful widgets such as `matplotlib` figure canvas, logger widget and color edit.
 
 #### Target users
 
 - Researchers who already have their Python functions and classes and are planing to take a step forward to improve the interface using GUI, with minimum effort.
 - Non-professional programmers who don't want to spend time on debugging and maintaining GUI.
 - Users who are not satisfied with the low reproducibility of the most of the GUI.
 - People who are familiar with `magicgui` and interested in more sophisticated GUI using typing.
@@ -43,15 +31,15 @@
 
 ## Installation
 
 
 - use pip
 
 ```
-pip install magic-class
+pip install magic-class -U
 ```
 
 - get latest version
 
 ```
 pip install git+https://github.com/hanjinliu/magic-class.git
 ```
@@ -76,17 +64,15 @@
         ----------
         path : Path
             File path
         """
         self.data = np.loadtxt(str(path))
 
     def plot(self):
-        """
-        Plot data.
-        """
+        """Plot data."""
         plt.plot(self.data)
         plt.show()
 ```
 
 Classes decorated with `@magicclass` are converted to `magicgui`'s `Container` widgets. GUI starts with `show` method.
 
 ```python
```

### Comparing `magic-class-0.6.9/magicclass/__init__.py` & `magic_class-0.7.0rc0/magicclass/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,83 @@
-__version__ = "0.6.9"
+__version__ = "0.7.0rc0"
 
 from .core import (
     magicclass,
     magicmenu,
     magiccontext,
     magictoolbar,
     Parameters,
     build_help,
+    get_button,
     get_function_gui,
     repeat,
     update_widget_state,
 )
 
 from .wrappers import (
     set_options,
     set_design,
     do_not_record,
     bind_key,
     confirm,
     nogui,
     mark_preview,
+    impl_preview,
+    setup_function_gui,
+    mark_on_calling,
+    mark_on_called,
+    abstractapi,
 )
 
-from .fields import field, vfield, widget_property, FieldGroup, HasFields, dataclass_gui
-from ._gui._base import wraps, defaults, MagicTemplate, PopUpMode
+from .fields import (
+    field,
+    vfield,
+    widget_property,
+    magicproperty,
+    FieldGroup,
+    HasFields,
+    dataclass_gui,
+)
+from ._gui._base import defaults, MagicTemplate, PopUpMode
 from ._gui.keybinding import Key
 from ._gui._icon import Icon
-from . import widgets, utils, types
+from . import widgets, utils, types, functools, logging
 
 from magicgui import *
 
 __all__ = [
     "magicclass",
     "magicmenu",
     "magiccontext",
     "magictoolbar",
     "Parameters",
     "build_help",
+    "get_button",
     "get_function_gui",
     "repeat",
     "update_widget_state",
     "set_options",
     "set_design",
     "do_not_record",
     "bind_key",
     "confirm",
     "nogui",
     "mark_preview",
+    "impl_preview",
+    "setup_function_gui",
+    "mark_on_calling",
+    "mark_on_called",
+    "abstractapi",
     "field",
     "vfield",
     "widget_property",
+    "magicproperty",
     "FieldGroup",
     "HasFields",
     "dataclass_gui",
-    "wraps",
     "defaults",
     "MagicTemplate",
     "PopUpMode",
     "Key",
     "Icon",
 ]
 
@@ -71,19 +91,31 @@
             "magicclass namespace. Please 'from magicclass.utils import click'.",
             DeprecationWarning,
             stacklevel=2,
         )
         from .utils import click
 
         return click
+
     elif key == "redo":
         warnings.warn(
             "Function `redo` is deprecated because its name is confusing. Please "
             "use `repeat` instead.",
             DeprecationWarning,
             stacklevel=2,
         )
         from .core import repeat
 
         return repeat
 
+    elif key == "wraps":
+        warnings.warn(
+            "Function `wraps` is moved to magicclass.functools. Please use "
+            "`from magicclass.functools import wraps` instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        from magicclass.functools import wraps
+
+        return wraps
+
     raise AttributeError(f"module {__name__!r} has no attribute {key!r}")
```

### Comparing `magic-class-0.6.9/magicclass/_app.py` & `magic_class-0.7.0rc0/magicclass/_app.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from qtpy.QtWidgets import QApplication
-from qtpy import PYQT5
-from qtpy.QtCore import Qt
 
-APPLICATION = None
+APPLICATION: QApplication = None
 
 
 def gui_qt():
     """Call "%gui qt" magic."""
     try:
         from IPython import get_ipython
     except ImportError:
```

### Comparing `magic-class-0.6.9/magicclass/_gui/_base.py` & `magic_class-0.7.0rc0/magicclass/_gui/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from functools import wraps as functools_wraps
+import functools
 from typing import (
     Any,
     Callable,
     TYPE_CHECKING,
     Iterable,
     Iterator,
     TypeVar,
@@ -11,159 +11,99 @@
     MutableSequence,
 )
 from types import MethodType
 from abc import ABCMeta
 from typing_extensions import _AnnotatedAlias, Literal
 import inspect
 import warnings
-from enum import Enum
-import warnings
-from docstring_parser import parse, compose
 from qtpy.QtWidgets import QWidget, QDockWidget
-from qtpy.QtGui import QIcon
 
 from psygnal import Signal
-from magicgui.signature import MagicParameter, split_annotated_type
+from magicgui.signature import MagicParameter
 from magicgui.widgets import (
     FunctionGui,
     FileEdit,
     EmptyWidget,
     Widget,
     Container,
     Image,
     Table,
     Label,
     MainWindow,
 )
 from magicgui.application import use_app
-from magicgui.widgets._bases.widget import Widget
-from magicgui.widgets._bases import ButtonWidget, ValueWidget
-from macrokit import Expr, Head, Symbol, symbol
+from magicgui.types import Undefined
+from magicgui.widgets.bases import (
+    ButtonWidget,
+    ValueWidget,
+)
+from macrokit import Symbol
 
 from .keybinding import as_shortcut
 from .mgui_ext import (
     AbstractAction,
     Action,
     FunctionGuiPlus,
     PushButtonPlus,
     _LabeledWidgetAction,
     mguiLike,
 )
-from .utils import copy_class, get_parameters, callable_to_classes
-from ._macro import GuiMacro
+from .utils import copy_class, callable_to_classes, show_dialog_from_mgui
+from ._macro import GuiMacro, DummyMacro
+from ._macro_utils import inject_recorder, inject_silencer, value_widget_callback
 from ._icon import get_icon
+from ._gui_modes import PopUpMode, ErrorMode
 
-from ..utils import (
+from magicclass.utils import (
     get_signature,
-    iter_members,
     Tooltips,
     move_to_screen_center,
     argcount,
     is_instance_method,
     method_as_getter,
     eval_attribute,
-    thread_worker,
 )
-from ..widgets import Separator, FreeWidget
-from ..fields import MagicField
-from ..signature import MagicMethodSignature, get_additional_option
-from ..wrappers import upgrade_signature
+from magicclass.widgets import Separator, FreeWidget
+from magicclass.fields import MagicField, MagicValueField, field, vfield
+from magicclass.signature import (
+    MagicMethodSignature,
+    get_additional_option,
+    split_annotated_type,
+    upgrade_signature,
+)
+from magicclass.wrappers import abstractapi
+from magicclass.types import BoundLiteral, MGUI_SIMPLE_TYPES
+from magicclass.functools import wraps
 
 if TYPE_CHECKING:
     import numpy as np
     import napari
-    from types import TracebackType
-
-
-class PopUpMode(Enum):
-    """Define how to popup FunctionGui."""
-
-    popup = "popup"
-    first = "first"
-    last = "last"
-    above = "above"
-    below = "below"
-    dock = "dock"
-    dialog = "dialog"
-    parentlast = "parentlast"
-    parentsub = "parentsub"
-
-
-def _msgbox_raising(e, parent):
-    from ._message_box import QtErrorMessageBox
-
-    return QtErrorMessageBox.raise_(e, parent=parent.native)
-
-
-def _stderr_raising(e, parent):
-    pass
-
-
-def _stdout_raising(e, parent):
-    print(f"{e.__class__.__name__}: {e}")
-
-
-def _napari_notification_raising(e, parent):
-    from napari.utils.notifications import show_error
-
-    show_error(str(e))
-
-
-class ErrorMode(Enum):
-    msgbox = "msgbox"
-    stderr = "stderr"
-    stdout = "stdout"
-    napari = "napari"
-
-    def get_handler(self):
-        """Get error handler."""
-        return ErrorModeHandlers[self]
-
-    def wrap_handler(self, func: Callable, parent):
-        """Wrap function with the error handler."""
-        handler = self.get_handler()
-
-        @functools_wraps(func)
-        def wrapped_func(*args, **kwargs):
-            try:
-                out = func(*args, **kwargs)
-            except Exception as e:
-                e.__traceback__ = _cleanup_tb(e.__traceback__)
-                handler(e, parent=parent)
-                out = e
-            return out
-
-        return wrapped_func
-
-
-ErrorModeHandlers = {
-    ErrorMode.msgbox: _msgbox_raising,
-    ErrorMode.stderr: _stderr_raising,
-    ErrorMode.stdout: _stdout_raising,
-    ErrorMode.napari: _napari_notification_raising,
-}
+    from typing_extensions import Self
 
+    _X = TypeVar("_X", bound=MGUI_SIMPLE_TYPES)
+    _M = TypeVar("_M", bound="MagicTemplate")
 
 defaults = {
     "popup_mode": PopUpMode.popup,
     "error_mode": ErrorMode.msgbox,
     "close_on_run": True,
-    "macro-max-history": 1000,
+    "macro-max-history": 100000,
+    "macro-highlight": False,
+    "undo-max-history": 100,
 }
 
 _RESERVED = frozenset(
     {
         "__magicclass_parent__",
         "__magicclass_children__",
         "_close_on_run",
         "_error_mode",
         "_popup_mode",
         "_my_symbol",
         "_macro_instance",
-        "macro",
         "annotation",
         "enabled",
         "find_ancestor",
         "gui_only",
         "height",
         "label_changed",
         "label",
@@ -209,14 +149,16 @@
     collision = subclass_members & _RESERVED
     if collision:
         raise AttributeError(
             f"Cannot override magic class reserved attributes: {collision}"
         )
 
 
+_ANCESTORS: dict[tuple[int, int], MagicTemplate] = {}
+
 _T = TypeVar("_T", bound="MagicTemplate")
 _F = TypeVar("_F", bound=Callable)
 
 
 class _MagicTemplateMeta(ABCMeta):
     """This metaclass enables type checking of nested magicclasses."""
 
@@ -228,20 +170,23 @@
     def __get__(self: type[_T], obj: Literal[None], objtype=None) -> type[_T]:
         ...
 
     def __get__(self, obj, objtype=None):
         return self
 
 
-class MagicTemplate(metaclass=_MagicTemplateMeta):
+_W = TypeVar("_W", bound=Widget)
+
+
+class MagicTemplate(MutableSequence[Widget], metaclass=_MagicTemplateMeta):
     __doc__ = ""
     __magicclass_parent__: None | MagicTemplate
     __magicclass_children__: list[MagicTemplate]
     _close_on_run: bool
-    _component_class: type[Action | Widget]
+    _component_class: type[Action | PushButtonPlus]
     _error_mode: ErrorMode
     _list: list[Action | Widget]
     _macro_instance: GuiMacro
     _my_symbol: Symbol
     _popup_mode: PopUpMode
     annotation: Any
     changed: Signal
@@ -258,56 +203,58 @@
     max_width: int
     min_height: int
     min_width: int
     name: str
     native: QWidget
     options: dict
     param_kind: inspect._ParameterKind
-    parent: Widget
+    parent: Widget | None
     parent_changed: Signal
     tooltip: str
     visible: bool
     widget_type: str
     width: int
 
     __init_subclass__ = check_override
 
-    def show(self, run: bool) -> None:
+    def show(self, run: bool = True) -> None:
         raise NotImplementedError()
 
     def hide(self) -> None:
         raise NotImplementedError()
 
     def close(self) -> None:
         raise NotImplementedError()
 
     @overload
     def __getitem__(self, key: int | str) -> Widget:
         ...
 
     @overload
-    def __getitem__(self, key: slice) -> MutableSequence[Widget]:
+    def __getitem__(self, key: slice) -> Self[Widget]:
         ...
 
     def __getitem__(self, key):
         raise NotImplementedError()
 
-    def index(self, value: Any, start: int, stop: int) -> int:
-        raise NotImplementedError()
+    if TYPE_CHECKING:
 
-    def remove(self, value: Widget | str):
-        raise NotImplementedError()
+        def __iter__(self) -> Iterator[Widget]:
+            raise NotImplementedError()
 
-    def append(self, widget: Widget) -> None:
-        return self.insert(len(self, widget))
+        def index(self, value: Any, start: int, stop: int) -> int:
+            raise NotImplementedError()
 
-    def _fast_insert(self, key: int, widget: Widget) -> None:
+        def remove(self, value: Widget | str):
+            raise NotImplementedError()
+
+    def _fast_insert(self, key: int, widget: Widget | Callable) -> None:
         raise NotImplementedError()
 
-    def insert(self, key: int, widget: Widget) -> None:
+    def insert(self, key: int, widget: Widget | Callable) -> None:
         self._fast_insert(key, widget)
         self._unify_label_widths()
 
     def render(self) -> np.ndarray:
         raise NotImplementedError()
 
     def _unify_label_widths(self):
@@ -324,22 +271,17 @@
         else:
             return self.__magicclass_parent__.macro
 
     @property
     def parent_viewer(self) -> napari.Viewer | None:
         """Return napari.Viewer if magic class is a dock widget of a viewer."""
         parent_self = self._search_parent_magicclass()
-        if parent_self.native.parent() is None:
-            return None
-        try:
-            from napari.utils._magicgui import find_viewer_ancestor
-        except ImportError:
+        if not isinstance(parent_self.native.parent(), QDockWidget):
             return None
-        viewer = find_viewer_ancestor(parent_self.native)
-        return viewer
+        return _find_viewer_ancestor(parent_self.native)
 
     @property
     def parent_dock_widget(self) -> QDockWidget | None:
         """
         Return dock widget object if magic class is a dock widget of a main
         window widget, such as a napari Viewer.
         """
@@ -349,44 +291,53 @@
             if not isinstance(dock, QDockWidget):
                 dock = None
         except AttributeError:
             dock = None
 
         return dock
 
-    def find_ancestor(self, ancestor: type[_T]) -> _T:
+    def find_ancestor(self, ancestor: type[_T], cache: bool = False) -> _T:
         """
         Find magic class ancestor whose type matches the input.
+
         This method is useful when a child widget class is defined outside a magic
         class while it needs access to its parent.
 
         Parameters
         ----------
         ancestor : type of MagicTemplate
             Type of ancestor to search for.
+        cache : bool, default is False
+            If true, the result will be cached. Caching is not safe if the widget is
+            going to be used as a child of other widgets.
 
         Returns
         -------
         MagicTemplate
             Magic class object if found.
         """
+        if cache and (anc := _ANCESTORS.get((id(self), id(ancestor)), None)):
+            return anc
+
         if not isinstance(ancestor, type):
             raise TypeError(
                 "The first argument of 'find_ancestor' must be a type but got "
                 f"{type(ancestor)}"
             )
 
         current_self = self
         while type(current_self) is not ancestor:
             current_self = current_self.__magicclass_parent__
             if current_self is None:
                 raise RuntimeError(
                     f"Magic class {ancestor.__name__} not found. {ancestor.__name__} "
                     f"is not an ancestor of {self.__class__.__name__}"
                 )
+        if cache:
+            _ANCESTORS[(id(self), id(ancestor))] = current_self
         return current_self
 
     def objectName(self) -> str:
         """
         Return object name of the QWidget.
 
         This function makes the object name discoverable by napari's
@@ -469,28 +420,32 @@
                     sig: inspect.Signature = predefined.__signature__
                     predefined.__signature__ = sig.replace(
                         parameters=parent_sig.parameters.values(),
                         return_annotation=parent_sig.return_annotation,
                     )
                 upgrade_signature(predefined, additional_options={"copyto": []})
 
+                # if abstractapi, mark as resolved
+                if isinstance(predefined, abstractapi):
+                    predefined.resolve()
+
             if copy:
                 copyto_list = get_additional_option(func, "copyto", [])
                 copyto_list.append(cls.__name__)
                 upgrade_signature(func, additional_options={"copyto": copyto_list})
             else:
                 upgrade_signature(func, additional_options={"into": cls.__name__})
             return method
 
         return wrapper if method is None else wrapper(method)
 
     def _unwrap_method(
         self,
         method_name: str,
-        widget: FunctionGui | PushButtonPlus | Action,
+        widget: FunctionGui | PushButtonPlus | AbstractAction,
         moveto: str,
         copyto: list[str],
     ):
         """
         This private method converts class methods that are wrapped by its child widget class
         into widget in child widget. Practically same widget is shared between parent and child,
         but only visible in the child side.
@@ -513,67 +468,198 @@
         if moveto is not None:
             matcher = copyto + [moveto]
         else:
             matcher = copyto
 
         _found = 0
         _n_match = len(matcher)
-
         for child_instance in self._iter_child_magicclasses():
             _name = child_instance.__class__.__name__
             if _name in matcher:
+                n_children = len(child_instance)
+
                 # get the position of predefined child widget
                 try:
                     index = _get_index(child_instance, method_name)
                     new = False
                 except ValueError:
-                    index = -1
+                    index = n_children
                     new = True
 
-                self._fast_insert(-1, widget)
+                self._fast_insert(len(self), widget, remove_label=True)
                 copy = _name in copyto
 
-                if isinstance(widget, FunctionGui):
+                if not isinstance(widget, (PushButtonPlus, AbstractAction)):
                     if copy:
                         widget = widget.copy()
                     if new:
-                        child_instance._fast_insert(-1, widget)
+                        child_instance._fast_insert(n_children, widget)
                     else:
                         del child_instance[index]
                         child_instance._fast_insert(index, widget)
 
                 else:
+                    # NOTE: wrapping button with action is not supported in the
+                    # method above.
                     widget.visible = copy
                     if new:
                         child_widget = child_instance._create_widget_from_method(
-                            lambda x: None
+                            _empty_func(method_name)
                         )
                         child_widget.text = widget.text
-                        child_instance._fast_insert(-1, child_widget)
+                        child_instance._fast_insert(n_children, child_widget)
                     else:
-                        child_widget: PushButtonPlus | AbstractAction = child_instance[
-                            index
-                        ]
+                        child_widget = child_instance[index]
 
                     child_widget.changed.disconnect()
                     child_widget.changed.connect(widget.changed)
                     child_widget.tooltip = widget.tooltip
                     child_widget._doc = widget._doc
+                    child_widget._get_running = lambda: widget.running
 
                 widget._unwrapped = True
 
                 _found += 1
                 if _found == _n_match:
                     break
 
         else:
             raise RuntimeError(
                 f"{method_name} not found in class {self.__class__.__name__}"
             )
 
+    # fmt: off
+    @overload
+    @classmethod
+    def field(cls, gui_class: type[_M], *, name: str | None = None, label: str | None = None, widget_type: str | None = None, options: dict[str, Any] = {}, record: bool = True, ) -> MagicField[_M, Any]: ...  # noqa
+
+    @overload
+    @classmethod
+    def field(cls, type_of_widget: type[_W], *, name: str | None = None, label: str | None = None, options: dict[str, Any] = {}, record: bool = True) -> MagicField[_W, Any]: ...  # noqa
+
+    @overload
+    @classmethod
+    def field(cls, obj: type[_X], *, name: str | None = None, label: str | None = None, widget_type: str | None = None, options: dict[str, Any] = {}, record: bool = True, ) -> MagicField[ValueWidget, _X]: ...  # noqa
+
+    @overload
+    @classmethod
+    def field(cls, obj: _X, *, name: str | None = None, label: str | None = None, widget_type: str | None = None, options: dict[str, Any] = {}, record: bool = True) -> MagicField[ValueWidget, _X]: ...  # noqa
+
+    @overload
+    @classmethod
+    def field(cls, obj: Any | None, *, name: str | None = None, label: str | None = None, widget_type: type[_W] = None, options: dict[str, Any] = {}, record: bool = True, ) -> MagicField[_W, Any]: ...  # noqa
+
+    @overload
+    @classmethod
+    def field(cls, obj: Any, *, name: str | None = None, label: str | None = None, widget_type: str | None = None, options: dict[str, Any] = {}, record: bool = True, ) -> MagicField[Widget, Any]: ...  # noqa
+
+    @overload
+    @classmethod
+    def field(cls, *, name: str | None = None, label: str | None = None, widget_type: str | type[Widget] | None = None, options: dict[str, Any] = {}, record: bool = True, ) -> MagicField[Widget, Any]: ...  # noqa
+    # fmt: on
+
+    @classmethod
+    def field(
+        cls,
+        obj=Undefined,
+        *,
+        name=None,
+        label=None,
+        widget_type=None,
+        options={},
+        record=True,
+    ) -> MagicField:
+        """
+        Make a MagicField object, with the widget in the child class.
+
+        >>> @magicclass
+        ... class A:
+        ...     @magicclass
+        ...     class B:
+        ...         i = ...  # pre-definition
+        ...     i = B.field(1)
+
+        Parameters
+        ----------
+        obj : Any, default is Undefined
+            Reference to determine what type of widget will be created. If Widget
+            subclass is given, it will be used as is. If other type of class is given,
+            it will used as type annotation. If an object (not type) is given, it will
+            be assumed to be the default value.
+        name : str, optional
+            Name of the widget.
+        label : str, optional
+            Label of the widget.
+        widget_type : str, optional
+            Widget type. This argument will be sent to ``create_widget`` function.
+        options : dict, optional
+            Widget options. This parameter will be passed to the ``options`` keyword
+            argument of ``create_widget``.
+        record : bool, default is True
+            A magic-class specific parameter. If true, record value changes as macro.
+
+        Returns
+        -------
+        MagicField
+        """
+        fld = field(
+            obj,
+            name=name,
+            label=label,
+            widget_type=widget_type,
+            options=options,
+            record=record,
+        )
+        fld.set_destination(cls)
+        return fld
+
+    # fmt: off
+    @overload
+    @classmethod
+    def vfield(cls, widget_type: type[_W], *, name: str | None = None, label: str | None = None, options: dict[str, Any] = {}, record: bool = True, ) -> MagicValueField[_W, Any]: ...  # noqa
+
+    @overload
+    @classmethod
+    def vfield(cls, annotation: type[_X], *, name: str | None = None, label: str | None = None, widget_type: str | None = None, options: dict[str, Any] = {}, record: bool = True, ) -> MagicValueField[ValueWidget, _X]: ...  # noqa
+
+    @overload
+    @classmethod
+    def vfield(cls, obj: _X, *, name: str | None = None, label: str | None = None, widget_type: str | None = None, options: dict[str, Any] = {}, record: bool = True, ) -> MagicValueField[ValueWidget, _X]: ...  # noqa
+
+    @overload
+    @classmethod
+    def vfield(cls, obj: Any, *, name: str | None = None, label: str | None = None, widget_type: type[_W] = None, options: dict[str, Any] = {}, record: bool = True, ) -> MagicValueField[_W, Any]: ...  # noqa
+
+    @overload
+    @classmethod
+    def vfield(cls, obj: Any, *, name: str | None = None, label: str | None = None, widget_type: str | type[Widget] | None = None, options: dict[str, Any] = {}, record: bool = True, ) -> MagicValueField[Widget, Any]: ...  # noqa
+    # fmt: on
+
+    @classmethod
+    def vfield(
+        cls,
+        obj=Undefined,
+        *,
+        name=None,
+        label=None,
+        widget_type=None,
+        options={},
+        record=True,
+    ) -> MagicValueField:
+        fld = vfield(
+            obj,
+            name=name,
+            label=label,
+            widget_type=widget_type,
+            options=options,
+            record=record,
+        )
+        fld.set_destination(cls)
+        return fld
+
     def _convert_attributes_into_widgets(self):
         """
         This function is called in dynamically created __init__. Methods, fields and nested
         classes are converted to magicgui widgets.
         """
         raise NotImplementedError()
 
@@ -588,124 +674,109 @@
         fld : MagicField
             A field object that describes what type of widget it should be.
         """
         raise NotImplementedError()
 
     def _create_widget_from_method(self, obj: MethodType):
         """Convert instance methods into GUI objects, such as push buttons or actions."""
-        text = obj.__name__.replace("_", " ")
-        widget = self._component_class(name=obj.__name__, text=text, gui_only=True)
+        if isinstance(obj, abstractapi):
+            obj.check_resolved()
+
+        if hasattr(obj, "__name__"):
+            obj_name = obj.__name__
+        else:
+            _inner_func = obj
+            while hasattr(_inner_func, "func"):
+                _inner_func = _inner_func.func
+            obj_name = getattr(_inner_func, "__name__", str(_inner_func))
+        text = obj_name.replace("_", " ")
+        widget = self._component_class(name=obj_name, text=text, gui_only=True)
 
         func = _create_gui_method(self, obj)
 
         # Prepare a button or action
         widget.tooltip = Tooltips(func).desc
         widget._doc = func.__doc__
 
         # Get the number of parameters except for empty widgets.
         # With these lines, "bind" method of magicgui works inside magicclass.
-        fgui_classes = callable_to_classes(func)
+        fgui_info = callable_to_classes(func)
         n_empty = len(
-            [_wdg_cls for _wdg_cls in fgui_classes if _wdg_cls is EmptyWidget]
+            [
+                0
+                for _wdg_cls, _prm in fgui_info
+                if _wdg_cls is EmptyWidget or _prm.options.get("bind", None) is not None
+            ]
         )
         nparams = argcount(func) - n_empty
+        if len(fgui_info) == 0:
+            _first_is_file_edit = False
+        else:
+            _first_is_file_edit = issubclass(fgui_info[0][0], FileEdit)
 
         has_preview = get_additional_option(func, "preview", None) is not None
 
         if nparams == 0 and not has_preview:
             # We don't want a dialog with a single widget "Run" to show up.
             def run_function():
                 # NOTE: callback must be defined inside function. Magic class must be
                 # "compiled" otherwise function wrappings are not ready!
                 mgui = _build_mgui(widget, func, self)
                 mgui.native.setParent(self.native, mgui.native.windowFlags())
                 out = mgui()
 
                 return out
 
-        elif nparams == 1 and issubclass(fgui_classes[0], FileEdit) and not has_preview:
+        elif nparams == 1 and _first_is_file_edit and not has_preview:
             # We don't want to open a magicgui dialog and again open a file dialog.
+
             def run_function():
                 mgui = _build_mgui(widget, func, self)
                 mgui.native.setParent(self.native, mgui.native.windowFlags())
-                fdialog: FileEdit = mgui[0]
-                if result := fdialog._show_file_dialog(
-                    fdialog.mode,
-                    caption=fdialog._btn_text,
-                    start_path=str(fdialog.value),
-                    filter=fdialog.filter,
-                ):
-                    fdialog.value = result
-                    out = mgui(result)
-                else:
-                    out = None
+                out = show_dialog_from_mgui(mgui)
+                self._popup_mode.connect_close_callback(mgui)
                 return out
 
         else:
             _prep_func = _define_popup(self, func, widget)
 
             def run_function():
                 mgui = _build_mgui(widget, func, self)
-                if mgui.call_count == 0 and len(mgui.called._slots) == 0:
+                _need_title_bar = self._popup_mode.need_title_bar()
+                if mgui.call_count == 0:  # connect only once
                     _prep_func(mgui)
-                    if self._popup_mode not in (
-                        PopUpMode.popup,
-                        PopUpMode.dock,
-                        PopUpMode.parentsub,
-                        PopUpMode.dialog,
-                    ):
+                    if _need_title_bar:
                         mgui.label = ""
                         # to avoid name collision
                         mgui.name = f"mgui-{id(mgui._function)}"
                         mgui.margins = (0, 0, 0, 0)
-                        title = Separator(
-                            orientation="horizontal", title=text, button=True
-                        )
-                        title.btn_text = "-"
-                        # TODO: should remove mgui from self?
-                        title.btn_clicked.connect(mgui.hide)
-                        mgui.insert(0, title)
+                        if not isinstance(mgui[0], Separator):
+                            title = Separator(
+                                orientation="horizontal", title=text, button=True
+                            )
+                            # TODO: should remove mgui from self?
+                            title.btn_clicked.connect(mgui.hide)
+                            mgui.insert(0, title)
 
                     if self._close_on_run and not mgui._auto_call:
-                        if self._popup_mode not in (
-                            PopUpMode.dock,
-                            PopUpMode.parentsub,
-                            PopUpMode.dialog,
-                        ):
-                            mgui.called.connect(mgui.hide)
-                        elif self._popup_mode in (PopUpMode.dock, PopUpMode.parentsub):
-                            # If FunctioGui is docked or in a subwindow, we should close
-                            # the parent QDockWidget/QMdiSubwindow.
-                            mgui.called.connect(lambda: mgui.parent.hide())
+                        self._popup_mode.connect_close_callback(mgui)
 
-                if nparams == 1 and issubclass(fgui_classes[0], FileEdit):
-                    fdialog: FileEdit = mgui[0]
+                if nparams == 1 and _first_is_file_edit:
+                    fdialog: FileEdit = mgui[int(_need_title_bar)]
                     if result := fdialog._show_file_dialog(
                         fdialog.mode,
                         caption=fdialog._btn_text,
                         start_path=str(fdialog.value),
                         filter=fdialog.filter,
                     ):
                         fdialog.value = result
                     else:
                         return None
 
-                if self._popup_mode not in (
-                    PopUpMode.dock,
-                    PopUpMode.dialog,
-                    PopUpMode.parentsub,
-                ):
-                    widget.mgui.show()
-                elif self._popup_mode == PopUpMode.dock:
-                    mgui.parent.show()  # show dock widget
-                elif self._popup_mode == PopUpMode.parentsub:
-                    mgui.native.parent().setVisible(True)
-                else:
-                    mgui.exec_as_dialog(parent=self)
-
+                self._popup_mode.activate_magicgui(mgui)
                 return None
 
         widget.changed.connect(run_function)
 
         # If design is given, load the options.
         widget.from_options(func)
 
@@ -729,39 +800,41 @@
     def _iter_child_magicclasses(self) -> Iterable[MagicTemplate]:
         """Iterate over all the child magic classes"""
         for child in self.__magicclass_children__:
             yield child
             yield from child._iter_child_magicclasses()
 
     def _call_with_return_callback(self, fname: str, *args, **kwargs) -> None:
-        from ..core import get_function_gui
+        from magicclass.core import get_function_gui
 
         fgui = get_function_gui(self, fname)
         fgui(*args, **kwargs)
         return None
 
 
-class BaseGui(MagicTemplate):
-    def __init__(self, close_on_run, popup_mode, error_mode):
+class BaseGui(MagicTemplate[_W]):
+    def __init__(
+        self, close_on_run=True, popup_mode=PopUpMode.popup, error_mode=ErrorMode.msgbox
+    ):
         self._macro_instance = GuiMacro(
             max_lines=defaults["macro-max-history"],
-            flags={"Get": False, "Return": False},
+            max_undo=defaults["undo-max-history"],
+            ui=self,
         )
         self.__magicclass_parent__: BaseGui | None = None
         self.__magicclass_children__: list[MagicTemplate] = []
         self._close_on_run = close_on_run
         self._popup_mode = popup_mode or PopUpMode.popup
         self._error_mode = error_mode or ErrorMode.msgbox
         self._my_symbol = Symbol.var("ui")
         self._icon = None
 
-        self.macro.widget.__magicclass_parent__ = self
-
     @property
     def icon(self):
+        """Icon of this GUI."""
         return self._icon
 
     @icon.setter
     def icon(self, val):
         icon = get_icon(val)
         qicon = icon.get_qicon(self)
         self._icon = icon
@@ -769,15 +842,15 @@
             self.native.setIcon(qicon)
         else:
             self.native.setWindowIcon(qicon)
         if hasattr(self.native, "setIconSize"):
             self.native.setIconSize(self.native.size())
 
 
-class ContainerLikeGui(BaseGui, mguiLike, MutableSequence):
+class ContainerLikeGui(BaseGui[Action], mguiLike):
     # This class enables similar API between magicgui widgets and additional widgets
     # in magicclass such as menu and toolbar.
     _component_class = Action
     changed = Signal(object)
     _list: list[AbstractAction | ContainerLikeGui]
 
     def reset_choices(self, *_: Any):
@@ -904,40 +977,61 @@
 def _get_widget_name(widget: Widget):
     # To escape reference
     return widget.name
 
 
 def _create_gui_method(self: BaseGui, obj: MethodType):
     func_sig = inspect.signature(obj)
+
     # Method type cannot set __signature__ attribute.
-    @functools_wraps(obj)
+    @functools.wraps(obj)
     def func(*args, **kwargs):
         return obj(*args, **kwargs)
 
     func.__signature__ = func_sig
 
     # This block enables instance methods in "bind" or "choices" of ValueWidget.
     all_params: list[inspect.Parameter] = []
     for param in func.__signature__.parameters.values():
         if isinstance(param.annotation, _AnnotatedAlias):
-            param = MagicParameter.from_parameter(param)
+            annot, opt = split_annotated_type(param.annotation)
+            param = MagicParameter(
+                param.name,
+                param.kind,
+                default=param.default,
+                annotation=annot,
+                gui_options=opt,
+            )
 
         if isinstance(param, MagicParameter):
             _param = MagicParameter(
                 name=param.name,
+                kind=param.kind,
                 default=param.default,
                 annotation=split_annotated_type(param.annotation)[0],
                 gui_options=param.options.copy(),
             )
             _arg_bind = _param.options.get("bind", None)
             _arg_choices = _param.options.get("choices", None)
 
             # If bound method is a class method, use self.method(widget).
             if isinstance(_arg_bind, str):
-                _arg_bind = eval_attribute(type(self), _arg_bind)
+                try:
+                    _arg_bind = eval_attribute(type(self), _arg_bind)
+                except Exception:
+                    pass
+                else:
+                    warnings.warn(
+                        "Binding method name string is deprecated for the safety reason. "
+                        "Please use method itself.",
+                        DeprecationWarning,
+                    )
+
+            if isinstance(_arg_bind, BoundLiteral):
+                _arg_bind = _arg_bind.eval(type(self))
 
             if is_instance_method(_arg_bind):
                 _param.options["bind"] = method_as_getter(self, _arg_bind)
 
             # If a MagicFiled is bound, bind the value of the connected widget.
             elif isinstance(_arg_bind, MagicField):
                 _param.options["bind"] = _arg_bind.as_remote_getter(self)
@@ -959,14 +1053,15 @@
         func.__signature__.additional_options = getattr(
             func_sig, "additional_options", {}
         )
     return func
 
 
 def _build_mgui(widget_: Action | PushButtonPlus, func: Callable, parent: BaseGui):
+    """Build a magicgui from a function for the give button/action."""
     if widget_.mgui is not None:
         return widget_.mgui
     try:
         sig = getattr(func, "__signature__", None)
         if isinstance(sig, MagicMethodSignature):
             opt = sig.additional_options
         else:
@@ -983,106 +1078,50 @@
         call_button = opt.get("call_button", None)
         layout = opt.get("layout", "vertical")
         labels = opt.get("labels", True)
         auto_call = opt.get("auto_call", False)
         mgui = FunctionGuiPlus(
             func, call_button, layout=layout, labels=labels, auto_call=auto_call
         )
-        preview = opt.get("preview", None)
-        if preview is not None:
-            btn_text, previewer = preview
-            mgui.append_preview(previewer.__get__(parent), btn_text)
+        # set function GUI.
+        widget_.mgui = mgui
+        mgui.native.setWindowTitle(widget_.text or widget_.name or "")
+
+        preview_setting = opt.get("preview", None)
+        if preview_setting is not None:
+            btn_text, is_auto_call, previewer = preview_setting
+            mgui.append_preview(
+                previewer.__get__(parent), btn_text, auto_call=is_auto_call
+            )
+        setup_func = opt.get("setup", None)
+        if setup_func is not None:
+            setup_func(parent, mgui)
 
     except Exception as e:
         msg = (
             "Exception was raised during building magicgui from method "
             f"{func.__name__}.\n{e.__class__.__name__}: {e}"
         )
+        widget_.mgui = None
         raise type(e)(msg)
 
-    widget_.mgui = mgui
-    name = widget_.name or ""
-    mgui.native.setWindowTitle(name.replace("_", " ").strip())
-    return mgui
-
+    return _connect_functiongui_event(mgui, opt)
 
-_C = TypeVar("_C", Callable, type)
-
-
-def wraps(template: Callable | inspect.Signature) -> Callable[[_C], _C]:
-    """
-    Update signature using a template. If class is wrapped, then all the methods
-    except for those start with "__" will be wrapped.
 
-    Parameters
-    ----------
-    template : Callable or inspect.Signature object
-        Template function or its signature.
-
-    Returns
-    -------
-    Callable
-        A wrapper which take a function or class as an input and returns same
-        function or class with updated signature(s).
-    """
-
-    def wrapper(f: _C) -> _C:
-        if isinstance(f, type):
-            for name, attr in iter_members(f):
-                if callable(attr) or isinstance(attr, type):
-                    wrapper(attr)
-            return f
-
-        Param = inspect.Parameter
-        old_signature = inspect.signature(f)
-
-        old_params = old_signature.parameters
-
-        if callable(template):
-            template_signature = inspect.signature(template)
-        elif isinstance(template, inspect.Signature):
-            template_signature = template
-        else:
-            raise TypeError(
-                "template must be a callable object or signature, "
-                f"but got {type(template)}."
-            )
-
-        # update empty signatures
-        template_params = template_signature.parameters
-        new_params: list[Param] = []
-
-        for k, v in old_params.items():
-            if v.annotation is Param.empty and v.default is Param.empty:
-                new_params.append(
-                    template_params.get(k, Param(k, Param.POSITIONAL_OR_KEYWORD))
-                )
-            else:
-                new_params.append(v)
-
-        # update empty return annotation
-        if old_signature.return_annotation is inspect.Parameter.empty:
-            return_annotation = template_signature.return_annotation
-        else:
-            return_annotation = old_signature.return_annotation
-
-        f.__signature__ = inspect.Signature(
-            parameters=new_params, return_annotation=return_annotation
-        )
-
-        fdoc = parse(f.__doc__)
-        tempdoc = parse(template.__doc__)
-        fdoc.short_description = fdoc.short_description or tempdoc.short_description
-        fdoc.long_description = fdoc.long_description or tempdoc.long_description
-        fdoc.meta = fdoc.meta or tempdoc.meta
-        f.__doc__ = compose(fdoc)
-
-        return f
-
-    return wrapper
+def _connect_functiongui_event(
+    mgui: FunctionGuiPlus, opt: dict[str, Any]
+) -> FunctionGui:
+    _on_calling = opt.get("on_calling", [])
+    for cb in _on_calling:
+        mgui.calling.connect(cb)
+
+    _on_called = opt.get("on_called", [])
+    for cb in _on_called:
+        mgui.called.connect(lambda: cb(mgui))
+    return mgui
 
 
 def _get_index(container: Container, widget_or_name: Widget | str) -> int:
     """
     Identical to container[widget_or_name], which sometimes doesn't work
     in magic-class.
     """
@@ -1108,195 +1147,17 @@
         if child_instance.__class__.__name__ == child_clsname:
             break
     else:
         raise ValueError(f"{widget_or_name} not found.")
     return child_instance
 
 
-def value_widget_callback(
-    gui: MagicTemplate,
-    widget: ValueWidget,
-    name: str | list[str],
-    getvalue: bool = True,
-):
-    """Define a ValueWidget callback, including macro recording."""
-    if isinstance(name, str):
-        sym_name = Symbol(name)
-    else:
-        sym_name = Symbol(name[0])
-        for n in name[1:]:
-            sym_name = Expr(head=Head.getattr, args=[sym_name, n])
-
-    if getvalue:
-        sub = Expr(head=Head.getattr, args=[sym_name, Symbol("value")])  # name.value
-    else:
-        sub = sym_name
-
-    def _set_value():
-        if not widget.enabled or not gui.macro.active:
-            # If widget is read only, it means that value is set in script (not manually).
-            # Thus this event should not be recorded as a macro.
-            return None
-
-        gui.changed.emit(gui)
-
-        # Make an expression of
-        # >>> x.name.value = value
-        # or
-        # >>> x.name = value
-        target = Expr(Head.getattr, [symbol(gui), sub])
-        expr = Expr(Head.assign, [target, widget.value])
-        if gui.macro._last_setval == target and len(gui.macro) > 0:
-            gui.macro.pop()
-            gui.macro._erase_last()
-        else:
-            gui.macro._last_setval = target
-        gui.macro.append(expr)
-        return None
-
-    return _set_value
-
-
-def nested_function_gui_callback(gui: MagicTemplate, fgui: FunctionGui):
-    """Define a FunctionGui callback, including macro recording."""
-    fgui_name = Symbol(fgui.name)
-
-    def _after_run():
-        if not fgui.enabled or not gui.macro.active:
-            # If widget is read only, it means that value is set in script (not manually).
-            # Thus this event should not be recorded as a macro.
-            return None
-        inputs = get_parameters(fgui)
-        args = [Expr(head=Head.kw, args=[Symbol(k), v]) for k, v in inputs.items()]
-        # args[0] is self
-        sub = Expr(head=Head.getattr, args=[symbol(gui), fgui_name])  # {x}.func
-        expr = Expr(head=Head.call, args=[sub] + args[1:])  # {x}.func(args...)
-
-        if fgui._auto_call:
-            # Auto-call will cause many redundant macros. To avoid this, only the last input
-            # will be recorded in magic-class.
-            last_expr = gui.macro[-1]
-            if (
-                last_expr.head == Head.call
-                and last_expr.args[0].head == Head.getattr
-                and last_expr.at(0, 1) == expr.at(0, 1)
-                and len(gui.macro) > 0
-            ):
-                gui.macro.pop()
-                gui.macro._erase_last()
-
-        gui.macro.append(expr)
-        gui.macro._last_setval = None
-
-    return _after_run
-
-
-_SELF = inspect.Parameter("self", inspect.Parameter.POSITIONAL_OR_KEYWORD)
-
-
-def _inject_recorder(func: Callable, is_method: bool = True) -> Callable:
-    """Inject macro recording functionality into a function."""
-    sig = get_signature(func)
-    if is_method:
-        sig = sig.replace(
-            parameters=list(sig.parameters.values())[1:],
-            return_annotation=sig.return_annotation,
-        )
-        _func = func
-    else:
-
-        @functools_wraps(func)
-        def _func(self, *args, **kwargs):
-            return func(*args, **kwargs)
-
-        _func.__signature__ = sig.replace(
-            parameters=[_SELF] + list(sig.parameters.values()),
-            return_annotation=sig.return_annotation,
-        )
-
-    _record_macro = _define_macro_recorder(sig, _func)
-
-    if not isinstance(_func, thread_worker):
-
-        @functools_wraps(_func)
-        def _recordable(bgui: MagicTemplate, *args, **kwargs):
-            with bgui.macro.blocked():
-                out = _func.__get__(bgui)(*args, **kwargs)
-            if bgui.macro.active:
-                _record_macro(bgui, *args, **kwargs)
-            return out
-
-        if hasattr(_func, "__signature__"):
-            _recordable.__signature__ = _func.__signature__
-        return _recordable
-
-    else:
-        _func._set_recorder(_record_macro)
-        return _func
-
-
-def _define_macro_recorder(sig: inspect.Signature, func: Callable):
-    if isinstance(sig, MagicMethodSignature):
-        opt = sig.additional_options
-        _auto_call = opt.get("auto_call", False)
-    else:
-        _auto_call = False
-
-    if sig.return_annotation is inspect.Parameter.empty:
-
-        def _record_macro(bgui: MagicTemplate, *args, **kwargs):
-            bound = sig.bind(*args, **kwargs)
-            kwargs = dict(bound.arguments.items())
-            expr = Expr.parse_method(bgui, func, (), kwargs)
-            if _auto_call:
-                # Auto-call will cause many redundant macros. To avoid this, only the last
-                # input will be recorded in magic-class.
-                last_expr = bgui.macro[-1]
-                if (
-                    last_expr.head == Head.call
-                    and last_expr.args[0].head == Head.getattr
-                    and last_expr.at(0, 1) == expr.at(0, 1)
-                    and len(bgui.macro) > 0
-                ):
-                    bgui.macro.pop()
-                    bgui.macro._erase_last()
-
-            bgui.macro.append(expr)
-            bgui.macro._last_setval = None
-            return None
-
-    else:
-        _cname_ = "_call_with_return_callback"
-
-        def _record_macro(bgui: MagicTemplate, *args, **kwargs):
-            bound = sig.bind(*args, **kwargs)
-            kwargs = dict(bound.arguments.items())
-            expr = Expr.parse_method(bgui, _cname_, (func.__name__,), kwargs)
-            if _auto_call:
-                # Auto-call will cause many redundant macros. To avoid this, only the last
-                # input will be recorded in magic-class.
-                last_expr = bgui.macro[-1]
-                if (
-                    last_expr.head == Head.call
-                    and last_expr.args[0].head == Head.getattr
-                    and last_expr.at(0, 1) == expr.at(0, 1)
-                    and last_expr.args[1] == expr.args[1]
-                    and len(bgui.macro) > 0
-                ):
-                    bgui.macro.pop()
-                    bgui.macro._erase_last()
-
-            bgui.macro.append(expr)
-            bgui.macro._last_setval = None
-            return None
-
-    return _record_macro
-
-
-def convert_attributes(cls: type[_T], hide: tuple[type, ...]) -> dict[str, Any]:
+def convert_attributes(
+    cls: type[_T], hide: tuple[type, ...], record: bool = True
+) -> dict[str, Any]:
     """
     Convert class attributes into macro recordable ones.
 
     Returned dictionary can be directly used for the third argument of
     ``type`` constructor. To avoid converting all the callables in
     subclasses, subclasses that will be iterated over can be restricted
     using ``hide`` argument.
@@ -1310,43 +1171,73 @@
 
     Returns
     -------
     dict
         New namespace.
     """
     _dict: dict[str, Callable] = {}
-    _pass_type = (property, classmethod, staticmethod, type, Widget)
+    _pass = (
+        property,
+        classmethod,
+        staticmethod,
+        type,
+        Widget,
+        MagicField,
+        abstractapi,
+    )
     mro = [c for c in cls.__mro__ if c not in hide]
+    default = None if record else "false"
     for subcls in reversed(mro):
         for name, obj in subcls.__dict__.items():
+            _isfunc = callable(obj)
             if isinstance(obj, _MagicTemplateMeta):
                 new_attr = copy_class(obj, cls, name=name)
-            elif (
-                name.startswith("_") or isinstance(obj, _pass_type) or not callable(obj)
-            ):
+            elif name.startswith("_") or isinstance(obj, _pass) or not _isfunc:
                 # private method, non-action-like object, not-callable object are passed.
                 new_attr = obj
-            elif callable(obj) and get_additional_option(obj, "record", True):
-                new_attr = _inject_recorder(obj)
+            elif _isfunc:
+                _record_policy = get_additional_option(obj, "record", default)
+                if _record_policy is None:
+                    new_attr = inject_recorder(obj)
+                elif _record_policy == "false":
+                    new_attr = obj
+                elif _record_policy == "all-false":
+                    new_attr = inject_silencer(obj)
+                else:
+                    raise ValueError(f"Invalid record policy: {_record_policy}")
             else:
                 new_attr = obj
 
             _dict[name] = new_attr
+    # replace the macro object with the dummy one.
+    if not record:
+        _dict["macro"] = macro
     return _dict
 
 
+_dummy_macro = DummyMacro()
+
+
+@property
+def macro(self: BaseGui):
+    """Return the dummy macro object"""
+    return _dummy_macro
+
+
 def _define_popup(self: BaseGui, obj, widget: PushButtonPlus | Action):
     # deal with popup mode.
     popup_mode = self._popup_mode
     if popup_mode == PopUpMode.popup:
         # To be popped up correctly, window flags of FunctionGui should be
         # "windowFlags" and should appear at the center.
         def _prep(mgui: FunctionGui):
-            mgui.native.setParent(self.native, mgui.native.windowFlags())
-            move_to_screen_center(mgui.native)
+            if mgui.native.parent() is not self.native:
+                mgui.native.setParent(self.native, mgui.native.windowFlags())
+                mgui.show()
+                move_to_screen_center(mgui.native)
 
     elif popup_mode == PopUpMode.parentlast:
 
         def _prep(mgui: FunctionGui):
             parent_self = self._search_parent_magicclass()
             parent_self.append(mgui)
 
@@ -1376,15 +1267,14 @@
             i = _get_index(child_self, widget)
             child_self.insert(i + 1, mgui)
 
     elif popup_mode == PopUpMode.dock:
         from .class_gui import MainWindowClassGui
 
         def _prep(mgui: FunctionGui):
-
             parent_self = self._search_parent_magicclass()
             viewer = parent_self.parent_viewer
             if viewer is None:
                 if isinstance(parent_self, MainWindowClassGui):
                     parent_self.add_dock_widget(mgui)
                 else:
                     msg = (
@@ -1439,15 +1329,15 @@
             if isinstance(condition, str):
                 try:
                     need_confirmation = eval(condition, {}, all_args)
                 except Exception as e:
                     msg = e.args[0]
                     e.args = (
                         f"Exception happened on evaluating condition {condition!r}.\n"
-                        f"{type(e).__name__}: {msg}"
+                        f"{type(e).__name__}: {msg}",
                     )
                     raise e
             elif callable(condition):
                 need_confirmation = condition(self)
             else:
                 warnings.warn(
                     f"Condition {condition} should be callable or string but got type "
@@ -1461,16 +1351,23 @@
 
     if hasattr(method, "__signature__"):
         _method.__signature__ = method.__signature__
 
     return _method
 
 
-def _cleanup_tb(tb: TracebackType):
-    """Remove useless info from a traceback object."""
-    current_tb = tb
-    while current_tb is not None:
-        if current_tb.tb_frame.f_code.co_name == "_recordable":
-            tb = current_tb.tb_next
-            break
-        current_tb = current_tb.tb_next
-    return tb
+def _empty_func(name: str) -> Callable[[Any], None]:
+    """Create a named function that does nothing."""
+    f = lambda x: None
+    f.__name__ = name
+    return f
+
+
+def _find_viewer_ancestor(widget: QWidget) -> napari.Viewer | None:
+    """Return the closest parent napari Viewer."""
+    parent = widget.parent()
+    while parent:
+        if hasattr(parent, "_qt_viewer"):  # QMainWindow
+            return parent._qt_viewer.viewer
+
+        parent = parent.parent()
+    return None
```

### Comparing `magic-class-0.6.9/magicclass/_gui/_dock_widget.py` & `magic_class-0.7.0rc0/magicclass/_gui/_dock_widget.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from operator import ior
 from qtpy.QtWidgets import QDockWidget as _QDockWidget, QMainWindow, QWidget
 from qtpy.QtCore import Qt
 
 
 class QtDockWidget(_QDockWidget):
     areas = {
-        "left": Qt.LeftDockWidgetArea,
-        "right": Qt.RightDockWidgetArea,
-        "top": Qt.TopDockWidgetArea,
-        "bottom": Qt.BottomDockWidgetArea,
+        "left": Qt.DockWidgetArea.LeftDockWidgetArea,
+        "right": Qt.DockWidgetArea.RightDockWidgetArea,
+        "top": Qt.DockWidgetArea.TopDockWidgetArea,
+        "bottom": Qt.DockWidgetArea.BottomDockWidgetArea,
     }
 
     def __init__(
         self,
         parent: QMainWindow,
         widget: QWidget,
         *,
@@ -31,13 +31,13 @@
 
             if any(area not in areas for area in allowed_areas):
                 raise ValueError(
                     f"all allowed_areas argument must be in {set(areas.keys())}"
                 )
             allowed_areas = reduce(ior, [areas[a] for a in allowed_areas])
         else:
-            allowed_areas = Qt.AllDockWidgetAreas
+            allowed_areas = Qt.DockWidgetArea.AllDockWidgetAreas
         self.qt_area = areas[area]
         self.setAllowedAreas(allowed_areas)
         self.setWidget(widget)
         self.setMinimumHeight(50)
         self.setMinimumWidth(50)
```

### Comparing `magic-class-0.6.9/magicclass/_gui/_function_gui.py` & `magic_class-0.7.0rc0/magicclass/widgets/pywidgets/dict.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,147 +1,157 @@
 from __future__ import annotations
-from typing import Any, TYPE_CHECKING, Callable, TypeVar
-import re
-from magicgui.widgets import PushButton
-from magicgui.widgets._concrete import _LabeledWidget
-from magicgui.widgets._bases import ValueWidget, ButtonWidget, ContainerWidget
-from magicgui.widgets._function_gui import FunctionGui
-
-from ..widgets import Separator
-
-if TYPE_CHECKING:
-    from magicgui.widgets import Widget
-
-
-_R = TypeVar("_R")
-
-
-class FunctionGuiPlus(FunctionGui[_R]):
-    """FunctionGui class with a parameter recording functionality etc."""
-
-    _dialog_widget = None
-
-    def __call__(self, *args: Any, update_widget: bool = False, **kwargs: Any) -> _R:
-        sig = self.__signature__
-        try:
-            bound = sig.bind(*args, **kwargs)
-        except TypeError as e:
-            if "missing a required argument" in str(e):
-                match = re.search("argument: '(.+)'", str(e))
-                missing = match.groups()[0] if match else "<param>"
-                msg = (
-                    f"{e} in call to '{self._callable_name}{sig}'.\n"
-                    "To avoid this error, you can bind a value or callback to the "
-                    f"parameter:\n\n    {self._callable_name}.{missing}.bind(value)"
-                    "\n\nOr use the 'bind' option in the set_option decorator:\n\n"
-                    f"    @set_option({missing}={{'bind': value}})\n"
-                    f"    def {self._callable_name}{sig}: ..."
-                )
-                raise TypeError(msg) from None
-            else:
-                raise
+from typing import Any, Iterable, MutableMapping
+from qtpy.QtWidgets import QTableWidget, QTableWidgetItem
 
-        if update_widget:
-            self._auto_call, before = False, self._auto_call
+from .object import BaseWidget, ContextMenuMixin, PyObjectBound
+
+
+class DictWidget(BaseWidget, MutableMapping):
+    def __init__(self, value=None, **kwargs):
+        super().__init__(**kwargs)
+
+        self._tablewidget = PyTableWidget(self.native)
+        self._tablewidget.setParentWidget(self)
+        self._tablewidget.setEditTriggers(QTableWidget.NoEditTriggers)
+        self._tablewidget.verticalHeader().setDefaultSectionSize(30)
+        self._dict: dict[str, int] = {}  # mapping from key to row
+
+        self.set_widget(self._tablewidget)
+
+        @self._tablewidget.itemDoubleClicked.connect
+        def _(item: PyTableWidgetItem):
+            type_ = type(item.obj)
+            callbacks = self._callbacks.get(type_, [])
+            self.running = True
             try:
-                self.update(bound.arguments)
+                for callback in callbacks:
+                    try:
+                        callback(item.obj, self._tablewidget.row(item))
+                    except TypeError:
+                        callback(item.obj)
             finally:
-                self._auto_call = before
+                self.running = False
 
-        bound.apply_defaults()
+        if value is not None:
+            self.update(dict(value))
 
-        # 1. Parameter recording
-        # This is important when bound function set by {"bind": f} updates something.
-        # When the value is referred via "__signature__" the bound function get called
-        # and updated againg.
-        self._previous_bound = bound
-
-        self._tqdm_depth = 0  # reset the tqdm stack count
-
-        # 2. Running flag
-        # We sometimes want to know if the function is called programmatically or
-        # from GUI. The "running" argument is True only when it's called via GUI.
-        self.running = True
-        try:
-            value = self._function(*bound.args, **bound.kwargs)
-        finally:
-            self.running = False
-
-        self._call_count += 1
-        if self._result_widget is not None:
-            with self._result_widget.changed.blocked():
-                self._result_widget.value = value
-
-        return_type = sig.return_annotation
-        if return_type:
-            from magicgui.type_map import _type2callback
-
-            for callback in _type2callback(return_type):
-                callback(self, value, return_type)
-        self.called.emit(value)
-        return value
-
-    def insert(self, key: int, widget: Widget):
-        """Insert widget at ``key``."""
-        if isinstance(widget, (ValueWidget, ContainerWidget)):
-            widget.changed.connect(lambda: self.changed.emit(self))
-        _widget = widget
-
-        if self.labels:
-            # no labels for button widgets (push buttons, checkboxes, have their own)
-            if not isinstance(widget, (_LabeledWidget, ButtonWidget, Separator)):
-                _widget = _LabeledWidget(widget)
-                widget.label_changed.connect(self._unify_label_widths)
-
-        if key < 0:
-            key += len(self)
-        self._list.insert(key, widget)
-        # NOTE: if someone has manually mucked around with self.native.layout()
-        # it's possible that indices will be off.
-        self._widget._mgui_insert_widget(key, _widget)
-        self._unify_label_widths()
-
-    def append_preview(self, f: Callable, text: str = "Preview"):
-        """Append a preview button to the widget."""
-        return append_preview(self, f, text)
-
-    def exec_as_dialog(self, parent=None):
-        """Show container as a dialog."""
-        if self._dialog_widget is None:
-            from magicgui.widgets import Dialog
+    def __len__(self) -> int:
+        return self._tablewidget.rowCount()
 
-            dlg = Dialog(widgets=[self], labels=False)
-            self._dialog_widget = dlg
-        else:
-            dlg = self._dialog_widget
-        dlg.native.setParent(parent.native, dlg.native.windowFlags())
-        if self._dialog_widget.exec():
-            self()
-        return self._dialog_widget
-
-    def reset_choices(self, *_: Any):
-        if self.visible:
-            return super().reset_choices()
-        with self.changed.blocked():
-            # in magicclass, magicgui tagged to a button or an action may be invisible,
-            # which causes unexpected function call
-            super().reset_choices()
-        return None
-
-
-def append_preview(self: FunctionGui, f: Callable, text: str = "Preview"):
-    """Append a preview button to a FunctionGui widget."""
-
-    btn = PushButton(text=text)
-    if isinstance(self[-1], PushButton):
-        self.insert(len(self) - 1, btn)
-    else:
-        self.append(btn)
-
-    @btn.changed.connect
-    def _call_preview():
-        sig = self.__signature__
-        bound = sig.bind()
-        bound.apply_defaults()
-        return f(*bound.args, **bound.kwargs)
+    @property
+    def value(self) -> dict[str, Any]:
+        return {k: self._tablewidget.item(row, 0) for k, row in self._dict}
+
+    def __getitem__(self, k: str) -> Any:
+        row = self._dict[k]
+        return self._tablewidget.item(row, 0).obj
 
-    return f
+    def __setitem__(self, k: str, obj: Any) -> None:
+        if not isinstance(k, str):
+            raise ValueError("Can only use str type as keys.")
+
+        if k in self._dict.keys():
+            row = self._dict[k]
+        else:
+            row = len(self)
+            self._dict[k] = row
+            self._tablewidget.insertRow(row)
+            if row == 0:
+                self._tablewidget.insertColumn(0)
+                self._tablewidget.setHorizontalHeaderItem(0, QTableWidgetItem("value"))
+            key_item = QTableWidgetItem(k)
+            self._tablewidget.setVerticalHeaderItem(row, key_item)
+
+        name = self._delegates.get(type(obj), str)(obj)
+        value_item = PyTableWidgetItem(obj, name)
+        tooltip = self._tooltip.get(type(obj), str)(obj)
+        value_item.setToolTip(tooltip)
+        self._tablewidget.setItem(row, 0, value_item)
+
+    def __delitem__(self, k: str) -> None:
+        row = self._dict.pop(k)
+        self._tablewidget.removeRow(row)
+
+    def __iter__(self) -> Iterable[str]:
+        return iter(self._dict)
+
+    def keys(self):
+        """
+        Return the view of dictionary keys.
+        """
+        return self._dict.keys()
+
+    def values(self) -> DictValueView:
+        """
+        Return the view of dictionary values as Python objects.
+        """
+        return DictValueView(self._tablewidget)
+
+    def items(self) -> DictItemView:
+        """
+        Return the view of dictionary keys and values as strings and Python objects.
+        """
+        return DictItemView(self._tablewidget)
+
+    def update(self, d: dict[str, Any]):
+        """
+        Update the dictionary contents.
+        """
+        for k, v in d.items():
+            self[k] = v
+
+    def clear(self) -> None:
+        """
+        Clear dictionary contents.
+        """
+        self._tablewidget.clear()
+        self._dict.clear()
+
+    def pop(self, k: str):
+        """
+        Pop a dictionary content.
+        """
+        row = self._dict.pop(k)
+        out = self._tablewidget.item(row, 0).obj
+        self._tablewidget.removeRow(row)
+        return out
+
+    def get(self, k: str, default=None):
+        self._dict.get(k, default)
+
+
+class PyTableWidget(ContextMenuMixin, QTableWidget):
+    def item(self, row: int, column: int) -> PyTableWidgetItem:
+        return super().item(row, column)
+
+    def itemAt(self, *p) -> PyTableWidgetItem:
+        return super().itemAt(*p)
+
+    def __init__(self, parent: None) -> None:
+        super().__init__(parent=parent)
+        self.setContextMenu()
+
+
+class PyTableWidgetItem(PyObjectBound, QTableWidgetItem):
+    def __init__(self, obj=None, name=None):
+        super().__init__()
+        self.setObject(obj, name)
+
+
+class DictValueView:
+    def __init__(self, widget: PyTableWidget):
+        self.widget = widget
+
+    def __iter__(self):
+        for row in range(self.widget.rowCount()):
+            yield self.widget.item(row, 0).obj
+
+
+class DictItemView:
+    def __init__(self, widget: PyTableWidget):
+        self.widget = widget
+
+    def __iter__(self):
+        for row in range(self.widget.rowCount()):
+            key = self.widget.verticalHeaderItem(row).text()
+            value = self.widget.item(row, 0).obj
+            yield key, value
```

### Comparing `magic-class-0.6.9/magicclass/_gui/_icon.py` & `magic_class-0.7.0rc0/magicclass/_gui/_icon.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     _source: QImage
 
     def __init__(self, source: Any):
         import numpy as np
 
         arr = np.asarray(source)
 
-        from magicgui import _mpl_image
+        from magicgui.widgets._image import _mpl_image
 
         img = _mpl_image.Image()
 
         img.set_data(arr)
 
         val: np.ndarray = img.make_image()
         h, w, _ = val.shape
```

### Comparing `magic-class-0.6.9/magicclass/_gui/_message_box.py` & `magic_class-0.7.0rc0/magicclass/_gui/_message_box.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,20 @@
     """An message box widget for displaying Python exception."""
 
     def __init__(self, title: str, text_or_exception: str | Exception, parent):
         if isinstance(text_or_exception, str):
             text = text_or_exception
             exc = None
         else:
-            text = text_or_exception.args[0]
+            if len(text_or_exception.args) > 0:
+                text = str(text_or_exception)
+                if len(text) > 1000:
+                    text = text[:1000] + "..."
+            else:
+                text = ""
             exc = text_or_exception
         super().__init__(
             QMessageBox.Icon.Critical,
             str(title),
             str(text),
             QMessageBox.StandardButton.Ok | QMessageBox.StandardButton.Help,
             parent=parent,
@@ -122,17 +127,21 @@
                 )
                 np_imported = True
             except ImportError:
                 np_imported = False
 
             vbtb = IPython.core.ultratb.VerboseTB(color_scheme=color)
             if as_html:
-                ansi_string = vbtb.text(*info).replace(" ", "&nbsp;")
-                html = "".join(ansi2html(ansi_string))
-                html = html.replace("\n", "<br>")
+                ansi_string = (
+                    vbtb.text(*info)
+                    .replace(" ", "&nbsp;")
+                    .replace("<", "&lt;")
+                    .replace(">", "&gt;")
+                )
+                html = "".join(ansi2html(ansi_string)).replace("\n", "<br>")
                 html = (
                     f"<span style='font-family: monaco,{_FONT},monospace;'>"
                     + html
                     + "</span>"
                 )
                 tb_text = html
             else:
```

### Comparing `magic-class-0.6.9/magicclass/_gui/_napari_type.py` & `magic_class-0.7.0rc0/magicclass/_gui/_napari_type.py`

 * *Files identical despite different names*

### Comparing `magic-class-0.6.9/magicclass/_gui/class_gui.py` & `magic_class-0.7.0rc0/magicclass/_gui/class_gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,44 @@
 from __future__ import annotations
 from typing import Any, Callable, Sequence, TypeVar
 import warnings
+from psygnal import Signal
 from qtpy.QtWidgets import QMenuBar, QWidget, QMainWindow, QBoxLayout, QDockWidget
 from qtpy.QtCore import Qt
-from magicgui.widgets import Container, MainWindow, Label, FunctionGui, Image, Table
-from magicgui.widgets._bases import Widget, ButtonWidget, ValueWidget, ContainerWidget
-from magicgui.widgets._concrete import _LabeledWidget, ContainerWidget
+from magicgui.widgets import (
+    Container,
+    MainWindow,
+    Label,
+    FunctionGui,
+    Image,
+    Table,
+    Widget,
+)
+from magicgui.widgets.bases import (
+    ButtonWidget,
+    ValueWidget,
+    ContainerWidget,
+    ContainerWidget,
+)
+from magicgui.types import Undefined
+from magicgui.widgets._concrete import _LabeledWidget
 from macrokit import Symbol
 
-
 from .keybinding import register_shortcut
 from .mgui_ext import PushButtonPlus
 from .toolbar import ToolBarGui, QtTabToolBar
 from .menu_gui import MenuGui, ContextMenuGui
 from ._base import (
     BaseGui,
     PopUpMode,
     ErrorMode,
-    value_widget_callback,
-    nested_function_gui_callback,
 )
 from .utils import format_error, connect_magicclasses
-from ..widgets import (
+from ._macro_utils import value_widget_callback, nested_function_gui_callback
+from magicclass.widgets import (
     ButtonContainer,
     GroupBoxContainer,
     FrameContainer,
     ListContainer,
     SubWindowsContainer,
     ScrollableContainer,
     DraggableContainer,
@@ -34,32 +47,32 @@
     SplitterContainer,
     StackedContainer,
     TabbedContainer,
     ToolBoxContainer,
     FreeWidget,
 )
 
-from ..utils import iter_members, Tooltips
-from ..fields import MagicField
-from ..signature import get_additional_option
-from .._app import run_app
+from magicclass.utils import iter_members, Tooltips
+from magicclass.fields import MagicField
+from magicclass.signature import get_additional_option
+from magicclass._app import run_app
 
 # For Containers that belong to these classes, menubar must be set to _qwidget.layout().
 _USE_OUTER_LAYOUT = (
     ScrollableContainer,
     DraggableContainer,
     SplitterContainer,
     TabbedContainer,
     SubWindowsContainer,
 )
 
 _MCLS_PAREMT = "__magicclass_parent__"
 
 
-class ClassGuiBase(BaseGui):
+class ClassGuiBase(BaseGui[Widget]):
     # This class is always inherited by @magicclass decorator.
     _component_class = PushButtonPlus
     _container_widget: type
     _remove_child_margins: bool
     native: QWidget
 
     def _create_widget_from_field(self, name: str, fld: MagicField):
@@ -74,25 +87,27 @@
         if isinstance(widget, BaseGui):
             widget.__magicclass_parent__ = self
             self.__magicclass_children__.append(widget)
             widget._my_symbol = Symbol(name)
 
         if isinstance(widget, (ValueWidget, ContainerWidget)):
             # If the field has callbacks, connect it to the newly generated widget.
-            if (
-                isinstance(widget, ValueWidget) or hasattr(widget, "value")
-            ) and fld.record:
-                # By default, set value function will be connected to the widget.
+            if fld.record:
                 getvalue = type(fld) is MagicField
-                f = value_widget_callback(self, widget, name, getvalue=getvalue)
-                widget.changed.connect(f)
+                if isinstance(widget, ValueWidget):
+                    if widget._bound_value is Undefined:
+                        f = value_widget_callback(self, widget, name, getvalue=getvalue)
+                        widget.changed.connect(f)
+                elif hasattr(widget, "value"):
+                    f = value_widget_callback(self, widget, name, getvalue=getvalue)
+                    widget.changed.connect(f)
 
         elif fld.callbacks:
             warnings.warn(
-                f"{type(widget).__name__} does not have value-change callback. "
+                f"{type(widget).__name__} does not have `changed` signal. "
                 "Connecting callback functions does no effect.",
                 UserWarning,
             )
 
         return widget
 
     def _convert_attributes_into_widgets(self):
@@ -110,14 +125,15 @@
         n_insert = 0
         base_members = {x[0] for x in iter_members(self._container_widget)}
         base_members |= {x[0] for x in iter_members(ClassGuiBase)}
 
         _hist: list[tuple[str, str, str]] = []  # for traceback
         _annot = ClassGuiBase.__annotations__.keys()
         _ignore_types = (property, classmethod, staticmethod)
+
         for name, attr in filter(lambda x: x[0] not in base_members, iter_members(cls)):
             if name in _annot or isinstance(attr, _ignore_types):
                 continue
 
             try:
                 if isinstance(attr, type):
                     # Nested magic-class
@@ -202,28 +218,30 @@
                     self._toolbar.addToolBar(
                         widget.native, widget.name.replace("_", " ")
                     )
                     _hist.append((name, type(attr), "ToolBarGui"))
 
                 elif isinstance(widget, (Widget, Callable)):
                     if (not isinstance(widget, Widget)) and callable(widget):
-                        # Methods or any callable objects, but FunctionGui is not included.
-                        # NOTE: Here any custom callable objects could be given. Some callable
-                        # objects can be incompatible (like "Signal" object in magicgui) but
-                        # useful. Those callable objects should be passed from widget construction.
                         if name.startswith("_") or not get_additional_option(
                             attr, "gui", True
                         ):
                             keybinding = get_additional_option(attr, "keybinding", None)
                             if keybinding:
                                 register_shortcut(
                                     keys=keybinding, parent=self.native, target=widget
                                 )
                             continue
+                        if isinstance(widget, Signal):
+                            continue
                         try:
+                            # Methods or any callable objects, but FunctionGui is not included.
+                            # NOTE: Here any custom callable objects could be given. Some callable
+                            # objects can be incompatible but useful. Those callable objects should
+                            # be passed from widget construction.
                             widget = self._create_widget_from_method(widget)
                         except AttributeError as e:
                             warnings.warn(
                                 f"Could not convert {widget!r} into a widget "
                                 f"due to AttributeError: {e}",
                                 UserWarning,
                             )
@@ -248,15 +266,15 @@
                         if not widget.name:
                             widget.name = name
                         if hasattr(widget, "text") and not widget.text:
                             widget.text = widget.name.replace("_", " ")
 
                     # Now, "widget" is a Widget object. Add widget in a way similar to "insert" method
                     # of Container.
-                    if name.startswith("_"):
+                    if widget.name.startswith("_"):
                         continue
 
                     moveto = get_additional_option(attr, "into")
                     copyto = get_additional_option(attr, "copyto", [])
                     if moveto is not None or copyto:
                         self._unwrap_method(name, widget, moveto, copyto)
                     else:
@@ -267,26 +285,28 @@
 
             except Exception as e:
                 format_error(e, _hist, name, attr)
 
         self._unify_label_widths()
         return None
 
-    def _fast_insert(self, key: int, obj: Widget | Callable) -> None:
+    def _fast_insert(
+        self, key: int, obj: Widget | Callable, remove_label: bool = False
+    ) -> None:
         if isinstance(obj, Callable):
-            # Sometimes uses want to dynamically add new functions to GUI.
+            # Sometimes users want to dynamically add new functions to GUI.
             if isinstance(obj, FunctionGui):
                 if obj.parent is None:
                     f = nested_function_gui_callback(self, obj)
                     obj.called.connect(f)
                 widget = obj
             else:
-                from ._base import _inject_recorder
+                from ._base import inject_recorder
 
-                obj = _inject_recorder(obj, is_method=False).__get__(self)
+                obj = inject_recorder(obj, is_method=False).__get__(self)
                 widget = self._create_widget_from_method(obj)
 
             method_name = getattr(obj, "__name__", None)
             if method_name and not hasattr(self, method_name):
                 object.__setattr__(self, method_name, obj)
         else:
             widget = obj
@@ -316,33 +336,40 @@
                     len(self.__magicclass_children__) > 0
                     and widget is not self.__magicclass_children__[-1]
                 ):
                     # nested magic classes are already in the list
                     self.__magicclass_children__.append(widget)
                     widget._my_symbol = Symbol(widget.name)
 
-                # NOTE: This is not safe. Attributes could collision and macro recording
-                # may break if not correctly named.
-
         _widget = widget
 
         if self.labels:
             # no labels for button widgets (push buttons, checkboxes, have their own)
-            if not isinstance(widget, _hide_labels):
+            if not isinstance(widget, _hide_labels) and not remove_label:
                 _widget = _LabeledWidget(widget)
                 widget.label_changed.connect(self._unify_label_widths)
 
         if key < 0:
             key += len(self)
         self._list.insert(key, widget)
         self._widget._mgui_insert_widget(key, _widget)
+
+        # NOTE: Function GUI is invisible by some reason...
+        # See https://github.com/hanjinliu/magic-class/issues/53
+        if isinstance(widget, FunctionGui):
+            widget.visible = True
         return None
 
 
 def find_window_ancestor(widget: Widget) -> SubWindowsClassGui:
+    """
+    Try to find a window ancestor of the given widget.
+
+    This function is used only for subwindows.
+    """
     parent_self = widget
     while (parent := getattr(parent_self, "__magicclass_parent__", None)) is not None:
         parent_self = parent
         if isinstance(parent_self, SubWindowsClassGui):
             break
 
     if not isinstance(parent_self, SubWindowsClassGui):
@@ -369,24 +396,23 @@
 
     def wrapper(cls_: type[ClassGuiBase]):
         cls: type[_C | ClassGuiBase] = type(
             cls_.__name__, (container, ClassGuiBase), {}
         )
 
         def __init__(
-            self: cls,
+            self: ClassGuiBase,
             layout: str = "vertical",
             close_on_run: bool = None,
             popup_mode: str | PopUpMode = None,
             error_mode: str | ErrorMode = None,
             labels: bool = True,
             name: str = None,
             visible: bool = None,
         ):
-
             container.__init__(
                 self, layout=layout, labels=labels, name=name, visible=visible
             )
             BaseGui.__init__(
                 self,
                 close_on_run=close_on_run,
                 popup_mode=popup_mode,
@@ -397,65 +423,64 @@
             self._toolbar = None
 
             self.native.setObjectName(self.name)
             self.native.setWindowTitle(self.name)
 
         # ui["x"] will not return widget if x is a MagicValueField.
         # To ensure __getitem__ returns a Widget, this method should be overriden.
-        def __getitem__(self: cls, key):
+        def __getitem__(self: ClassGuiBase, key):
             """Get item by integer, str, or slice."""
             if isinstance(key, str):
                 for widget in self._list:
                     if key == widget.name:
                         return widget
             return container.__getattr__(self, key)
 
-        def __setattr__(self: cls, name: str, value: Any) -> None:
+        def __setattr__(self, name: str, value: Any) -> None:
             if not isinstance(getattr(self.__class__, name, None), MagicField):
                 container.__setattr__(self, name, value)
             else:
                 object.__setattr__(self, name, value)
 
-        def insert(self: cls, key: int, widget: Widget) -> None:
+        def insert(self: ClassGuiBase, key: int, widget: Widget) -> None:
             self._fast_insert(key, widget)
             self._unify_label_widths()
             return None
 
-        def reset_choices(self: cls, *_: Any):
+        def reset_choices(self: ClassGuiBase, *_: Any):
             """Reset child Categorical widgets"""
             all_widgets: set[Widget] = set()
 
             for item in self._list:
                 widget = getattr(item, "_inner_widget", item)
                 all_widgets.add(widget)
             for widget in self.__magicclass_children__:
                 all_widgets.add(widget)
 
             for w in all_widgets:
                 if hasattr(w, "reset_choices"):
                     w.reset_choices()
             return None
 
-        def show(self: cls, run: bool = True) -> None:
+        def show(self: ClassGuiBase, run: bool = True) -> None:
             """
             Show GUI. If any of the parent GUI is a dock widget in napari, then this
             will also show up as a dock widget (floating if in popup mode).
 
             Parameters
             ----------
             run : bool, default is True
                 *Unlike magicgui, this parameter should always be True* unless you want
                 to close the window immediately. If true, application gets executed if
                 needed.
             """
-            if self.__magicclass_parent__ is not None and self.parent is None:
+            mcls_parent = self.__magicclass_parent__
+            if mcls_parent is not None and self.parent is None:
                 # If child magic class is closed before, we have to set parent again.
-                self.native.setParent(
-                    self.__magicclass_parent__.native, self.native.windowFlags()
-                )
+                self.native.setParent(mcls_parent.native, self.native.windowFlags())
 
             viewer = self.parent_viewer
             if viewer is not None and self.parent is not None:
                 name = self.parent.objectName()
                 if name in viewer.window._dock_widgets and isinstance(
                     self.parent, QDockWidget
                 ):
@@ -468,20 +493,25 @@
                         name=self.name.replace("_", " ").strip(),
                         area=_area,
                         allowed_areas=["left", "right"],
                     )
                     dock.setFloating(_floating)
             else:
                 container.show(self, run=False)
+                if mcls_parent is not None:
+                    topleft = mcls_parent.native.geometry().topLeft()
+                    topleft.setX(topleft.x() + 20)
+                    topleft.setY(topleft.y() + 20)
+                    self.native.move(topleft)
                 self.native.activateWindow()
                 if run:
                     run_app()
             return None
 
-        def close(self: cls):
+        def close(self: ClassGuiBase):
             """Close GUI. if this widget is a dock widget, then also close it."""
 
             current_self = self._search_parent_magicclass()
 
             viewer = current_self.parent_viewer
             if viewer is not None:
                 try:
@@ -492,21 +522,21 @@
             container.close(self)
 
             return None
 
         if issubclass(container, MainWindow):
             # Similar to napari's viewer.window.add_dock_widget.
             # See napari/_qt/widgets/qt_viewer_dock_widget.py
-            from ..wrappers import nogui
+            from magicclass.wrappers import nogui
 
             # This function will be detected as non-reserved method so that magicclass will
             # try to convert it into widget. Should decorate with @nogui.
             @nogui
             def add_dock_widget(
-                self: cls,
+                self: MainWindowClassGui,
                 widget: Widget,
                 *,
                 name: str = "",
                 area: str = "right",
                 allowed_areas: Sequence[str] | None = None,
             ):
                 """
@@ -539,15 +569,15 @@
                 self.native.addDockWidget(QtDockWidget.areas[area], dock)
                 if isinstance(widget, BaseGui):
                     widget.__magicclass_parent__ = self
                     self.__magicclass_children__.append(widget)
                     widget._my_symbol = Symbol(name)
 
             @nogui
-            def remove_dock_widget(self: cls, widget: Widget):
+            def remove_dock_widget(self: MainWindowClassGui, widget: Widget):
                 from ._dock_widget import QtDockWidget
 
                 dock = None
                 i_dock = -1
                 for i, child in enumerate(self.__magicclass_children__):
                     if child is widget:
                         dock = child.native.parent()
@@ -558,21 +588,26 @@
                         break
                 else:
                     raise RuntimeError("Dock widget not found.")
 
                 self.native.removeDockWidget(dock)
                 self.__magicclass_children__.pop(i_dock)
 
+            def close(self: ClassGuiBase):
+                """Close GUI."""
+                self.native.close()
+                return None
+
             @property
-            def status(self: cls) -> str:
+            def status(self: MainWindowClassGui) -> str:
                 """Get status tip."""
                 return self.native.statusTip()
 
             @status.setter
-            def status(self: cls, text: str):
+            def status(self: MainWindowClassGui, text: str):
                 """Set status tip."""
                 self.native.setStatusTip(text)
                 self.native.statusBar().showMessage(text, 5000)
 
             cls.add_dock_widget = add_dock_widget
             cls.remove_dock_widget = remove_dock_widget
             cls.status = status
```

### Comparing `magic-class-0.6.9/magicclass/_gui/keybinding.py` & `magic_class-0.7.0rc0/magicclass/_gui/keybinding.py`

 * *Files 6% similar despite different names*

```diff
@@ -173,16 +173,21 @@
         return True
     else:
         return Key(s) in MODIFIERS
 
 
 def parse_key_combo(key_combo: str) -> QtKey:
     # For compatibility with napari
-    parsed = re.split("-(?=.+)", key_combo)
-    return strs2keycombo(*parsed)
+    parsed = re.split(r"\+(?=.+)", key_combo)
+    try:
+        out = strs2keycombo(*parsed)
+    except ValueError:
+        parsed = re.split("-(?=.+)", key_combo)
+        out = strs2keycombo(*parsed)
+    return out
 
 
 def strs2keycombo(*args: tuple[str | Key, ...]) -> KeyCombo:
     *modifiers, key = args
     if len(modifiers) > 2:
         raise ValueError("More than two modifiers found.")
     return tuple(Key.to_qtmodifier(m) for m in modifiers) + (Key.to_qtkey(key),)
```

### Comparing `magic-class-0.6.9/magicclass/_gui/menu_gui.py` & `magic_class-0.7.0rc0/magicclass/_gui/menu_gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 from __future__ import annotations
 from typing import Callable
 import warnings
-from magicgui.widgets import Image, Table, Label, FunctionGui
-from magicgui.widgets._bases import ButtonWidget
-from magicgui.widgets._bases.widget import Widget
+from magicgui.widgets import Image, Table, Label, FunctionGui, Widget
+from magicgui.widgets.bases import ButtonWidget
 from macrokit import Symbol
+from psygnal import Signal
 from qtpy.QtWidgets import QMenu
 from qtpy.QtCore import Qt
 
 from .mgui_ext import AbstractAction, WidgetAction, _LabeledWidgetAction
 from .keybinding import register_shortcut
 from ._base import (
     BaseGui,
     PopUpMode,
     ErrorMode,
     ContainerLikeGui,
-    nested_function_gui_callback,
-    _inject_recorder,
 )
 from .utils import format_error, connect_magicclasses
+from ._macro_utils import nested_function_gui_callback, inject_recorder
 
-from ..signature import get_additional_option
-from ..fields import MagicField
-from ..widgets import Separator, FreeWidget
-from ..utils import iter_members, Tooltips
+from magicclass.signature import get_additional_option
+from magicclass.fields import MagicField
+from magicclass.widgets import Separator, FreeWidget
+from magicclass.utils import iter_members, Tooltips
 
 
 def _check_popupmode(popup_mode: PopUpMode):
     if popup_mode in (PopUpMode.above, PopUpMode.below, PopUpMode.first):
         msg = (
             f"magicmenu does not support popup mode {popup_mode.value}."
             "PopUpMode.popup is used instead"
@@ -56,26 +55,31 @@
     ):
         popup_mode = _check_popupmode(popup_mode)
 
         super().__init__(
             close_on_run=close_on_run, popup_mode=popup_mode, error_mode=error_mode
         )
         name = name or self.__class__.__name__
-        self.native = QMenu(name, parent)
+        self._native = QMenu(name, parent)
         self.native.setToolTipsVisible(True)
         self.name = name
         self._list: list[MenuGuiBase | AbstractAction] = []
         self.labels = labels
 
+    @property
+    def native(self):
+        """The native Qt widget."""
+        return self._native
+
     def _convert_attributes_into_widgets(self):
         cls = self.__class__
 
         # Add class docstring as tooltip.
         _tooltips = Tooltips(cls)
-        self.native.setToolTip(_tooltips.desc)
+        self.tooltip = _tooltips.desc
 
         # Bind all the methods and annotations
         base_members = {x[0] for x in iter_members(MenuGuiBase)}
 
         _hist: list[tuple[str, str, str]] = []  # for traceback
         _ignore_types = (property, classmethod, staticmethod)
 
@@ -95,15 +99,16 @@
                         widget.tooltip = _tooltips.attributes.get(name, "")
 
                 else:
                     # convert class method into instance method
                     widget = getattr(self, name, None)
 
                 if isinstance(widget, FunctionGui):
-                    widget[0].bind(self)  # set self to the first argument
+                    widget = attr.copy()
+                    widget[0].bind(self)  # bind self to the first argument
 
                 elif isinstance(widget, BaseGui):
                     connect_magicclasses(self, widget, name)
 
                     if isinstance(widget, MenuGuiBase):
                         widget.native.setParent(
                             self.native, widget.native.windowFlags()
@@ -125,27 +130,29 @@
                         ):
                             keybinding = get_additional_option(attr, "keybinding", None)
                             if keybinding:
                                 register_shortcut(
                                     keys=keybinding, parent=self.native, target=widget
                                 )
                             continue
+                        if isinstance(widget, Signal):
+                            continue
                         widget = self._create_widget_from_method(widget)
 
                     elif hasattr(widget, "__magicclass_parent__") or hasattr(
                         widget.__class__, "__magicclass_parent__"
                     ):
                         if isinstance(widget, BaseGui):
                             widget._my_symbol = Symbol(name)
                         # magic-class has to know its parent.
                         # if __magicclass_parent__ is defined as a property, hasattr must be called
                         # with a type object (not instance).
                         widget.__magicclass_parent__ = self
 
-                    if name.startswith("_"):
+                    if widget.name.startswith("_"):
                         continue
                     moveto = get_additional_option(attr, "into")
                     copyto = get_additional_option(attr, "copyto", [])
                     if moveto is not None or copyto:
                         self._unwrap_method(name, widget, moveto, copyto)
                     else:
                         self._fast_insert(len(self), widget)
@@ -155,25 +162,28 @@
             except Exception as e:
                 format_error(e, _hist, name, attr)
 
         self._unify_label_widths()
         return None
 
     def _fast_insert(
-        self, key: int, obj: Callable | MenuGuiBase | AbstractAction
+        self,
+        key: int,
+        obj: Callable | MenuGuiBase | AbstractAction,
+        remove_label: bool = False,
     ) -> None:
         if isinstance(obj, Callable):
             # Sometimes users want to dynamically add new functions to GUI.
             if isinstance(obj, FunctionGui):
                 if obj.parent is None:
                     f = nested_function_gui_callback(self, obj)
                     obj.called.connect(f)
                 _obj = obj
             else:
-                obj = _inject_recorder(obj, is_method=False).__get__(self)
+                obj = inject_recorder(obj, is_method=False).__get__(self)
                 _obj = self._create_widget_from_method(obj)
 
             method_name = getattr(obj, "__name__", None)
             if method_name and not hasattr(self, method_name):
                 object.__setattr__(self, method_name, obj)
         else:
             _obj = obj
@@ -203,16 +213,17 @@
                     FreeWidget,
                     Label,
                     FunctionGui,
                     Image,
                     Table,
                 )
                 _obj_labeled = _obj
-                if (not isinstance(_obj.widget, _hide_labels)) and self.labels:
-                    _obj_labeled = _LabeledWidgetAction.from_action(_obj)
+                if self.labels:
+                    if not isinstance(_obj.widget, _hide_labels) and not remove_label:
+                        _obj_labeled = _LabeledWidgetAction.from_action(_obj)
                 _obj_labeled.parent = self
                 insert_action_like(self.native, key, _obj_labeled.native)
 
             self._list.insert(key, _obj)
         else:
             raise TypeError(f"{type(_obj)} is not supported.")
 
@@ -242,29 +253,26 @@
     key : int
         Position to insert.
     obj : QMenu or QAction or str
         Object to be inserted.
     """
     actions = qmenu.actions()
     l = len(actions)
-    if key < 0:
-        key = key + l
-    if key == l:
+    if key in (l, -1):
         if isinstance(obj, QMenu):
             qmenu.addMenu(obj).setText(obj.objectName().replace("_", " "))
         elif isinstance(obj, str):
             if obj:
                 qmenu.addSection(obj)
             else:
                 qmenu.addSeparator()
         else:
             qmenu.addAction(obj)
     else:
-        new_action = actions[key]
-        before = new_action
+        before = actions[key]
         if isinstance(obj, QMenu):
             qmenu.insertMenu(before, obj).setText(obj.objectName().replace("_", " "))
         elif isinstance(obj, str):
             if obj:
                 qmenu.insertSection(before, obj)
             else:
                 qmenu.insertSeparator(before)
```

### Comparing `magic-class-0.6.9/magicclass/_gui/mgui_ext.py` & `magic_class-0.7.0rc0/magicclass/_gui/mgui_ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 from __future__ import annotations
-from typing import Callable, Iterable, Any, Generic, TypeVar
+from typing import Callable, Iterable, Any, Generic, TypeVar, Union
+from typing_extensions import TypeGuard
 from qtpy.QtWidgets import (
     QPushButton,
     QAction,
     QWidgetAction,
     QToolButton,
     QWidget,
     QMenu,
 )
 from psygnal import Signal
-from magicgui.widgets import PushButton
+from magicgui.widgets import PushButton, Widget
+from magicgui.widgets.bases import ValueWidget
 from magicgui.widgets._concrete import _LabeledWidget
-from magicgui.widgets._bases import Widget, ValueWidget
 from magicgui.backends._qtpy.widgets import QBaseButtonWidget
 from ._function_gui import FunctionGuiPlus
 from ._icon import get_icon
 
 # magicgui widgets that need to be extended to fit into magicclass
+Clickable = Union["PushButtonPlus", "Action"]
+
+
+def is_clickable(wdt: Widget) -> TypeGuard[Clickable]:
+    return isinstance(wdt, (PushButtonPlus, Action))
 
 
 class PushButtonPlus(PushButton):
     """A Qt specific PushButton widget with a magicgui bound."""
 
     def __init__(self, text: str | None = None, **kwargs):
         super().__init__(text=text, **kwargs)
         self.native: QPushButton
         self._icon = None
         self.mgui: FunctionGuiPlus | None = None  # tagged function GUI
         self._doc = ""
         self._unwrapped = False
+        self._get_running: Callable[[], bool] | None = None
 
     @property
     def running(self) -> bool:
         """Return true if embedded magicgui widget is running from GUI."""
-        return getattr(self.mgui, "running", False)
+        if self._get_running is None:
+            return getattr(self.mgui, "running", False)
+        return self._get_running()
 
     def set_shortcut(self, key):
         """Set keyboard shortcut to the button."""
         self.native.setShortcut(key)
 
     def reset_choices(self, *_: Any):
         """Reset child Categorical widgets."""
@@ -115,16 +124,16 @@
 
         for k, v in options.items():
             setattr(self, k, v)
         return None
 
 
 class _QToolButton(QBaseButtonWidget):
-    def __init__(self):
-        super().__init__(QToolButton)
+    def __init__(self, **kwargs):
+        super().__init__(QToolButton, **kwargs)
 
 
 class ToolButtonPlus(PushButtonPlus):
     """Buttons for toolbar in magic-class."""
 
     def __init__(self, text: str | None = None, **kwargs):
         kwargs["widget_type"] = _QToolButton
@@ -246,18 +255,22 @@
         if text:
             self.text = text
         if name:
             self.native.setObjectName(name)
         self._callbacks = []
 
         self.native.triggered.connect(lambda: self.changed.emit(self.value))
+        self._get_running: Callable[[], bool] | None = None
 
     @property
     def running(self) -> bool:
-        return getattr(self.mgui, "running", False)
+        """Return true if embedded magicgui widget is running from GUI."""
+        if self._get_running is None:
+            return getattr(self.mgui, "running", False)
+        return self._get_running()
 
     def set_shortcut(self, key):
         self.native.setShortcut(key)
         return None
 
     def reset_choices(self, *_: Any):
         """Reset child Categorical widgets."""
@@ -286,14 +299,17 @@
 
     @icon.setter
     def icon(self, val):
         icon = get_icon(val)
         icon.install(self)
         self._icon = icon
 
+    def trigger(self):
+        return self.native.trigger()
+
     def from_options(self, options: dict[str] | Callable):
         if callable(options):
             try:
                 options = options.__signature__.caller_options
             except AttributeError:
                 return None
```

### Comparing `magic-class-0.6.9/magicclass/_gui/toolbar.py` & `magic_class-0.7.0rc0/magicclass/_gui/toolbar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from __future__ import annotations
 from typing import Callable, TYPE_CHECKING, Any
 import warnings
-from magicgui.widgets import Image, Table, Label, FunctionGui
-from magicgui.widgets._bases import ButtonWidget
-from magicgui.widgets._bases.widget import Widget
+from magicgui.widgets import Image, Table, Label, FunctionGui, Widget
+from magicgui.widgets.bases import ButtonWidget
 from macrokit import Symbol
+from psygnal import Signal
 from qtpy.QtWidgets import QToolBar, QMenu, QWidgetAction, QTabWidget
 
 
 from .mgui_ext import AbstractAction, _LabeledWidgetAction, WidgetAction, ToolButtonPlus
 from .keybinding import register_shortcut
 from ._base import (
     BaseGui,
     PopUpMode,
     ErrorMode,
     ContainerLikeGui,
-    nested_function_gui_callback,
-    _inject_recorder,
 )
 from .utils import format_error, connect_magicclasses
 from .menu_gui import ContextMenuGui, MenuGui, MenuGuiBase, insert_action_like
+from ._macro_utils import inject_recorder, nested_function_gui_callback
 
-from ..signature import get_additional_option
-from ..fields import MagicField
-from ..widgets import FreeWidget, Separator
-from ..utils import iter_members, Tooltips
+from magicclass.signature import get_additional_option
+from magicclass.fields import MagicField
+from magicclass.widgets import FreeWidget, Separator
+from magicclass.utils import iter_members, Tooltips
+from magicclass.wrappers import abstractapi
 
 if TYPE_CHECKING:
-    from napari.viewer import Viewer
+    import napari
 
 
 def _check_popupmode(popup_mode: PopUpMode):
     if popup_mode in (PopUpMode.above, PopUpMode.below, PopUpMode.first):
         msg = (
             f"magictoolbar does not support popup mode {popup_mode.value}."
             "PopUpMode.popup is used instead"
@@ -82,19 +82,24 @@
     ):
         popup_mode = _check_popupmode(popup_mode)
 
         super().__init__(
             close_on_run=close_on_run, popup_mode=popup_mode, error_mode=error_mode
         )
         name = name or self.__class__.__name__
-        self.native = QToolBar(name, parent)
+        self._native = QToolBar(name, parent)
         self.name = name
         self._list: list[MenuGuiBase | AbstractAction] = []
         self.labels = labels
 
+    @property
+    def native(self):
+        """The native Qt widget."""
+        return self._native
+
     def reset_choices(self, *_: Any):
         """Reset child Categorical widgets"""
         super().reset_choices()
 
         # If parent magic-class is added to napari viewer, the style sheet need update because
         # QToolButton has inappropriate style.
         # Detecting this event using "reset_choices" is not a elegant way, but works for now.
@@ -133,15 +138,16 @@
                         widget.tooltip = _tooltips.attributes.get(name, "")
 
                 else:
                     # convert class method into instance method
                     widget = getattr(self, name, None)
 
                 if isinstance(widget, FunctionGui):
-                    widget[0].bind(self)  # set self to the first argument
+                    widget = attr.copy()
+                    widget[0].bind(self)  # bind self to the first argument
 
                 elif isinstance(widget, BaseGui):
                     connect_magicclasses(self, widget, name)
 
                     if isinstance(widget, MenuGui):
                         tb = ToolButtonPlus(widget.name)
                         tb.set_menu(widget.native)
@@ -177,14 +183,16 @@
                         ):
                             keybinding = get_additional_option(attr, "keybinding", None)
                             if keybinding:
                                 register_shortcut(
                                     keys=keybinding, parent=self.native, target=widget
                                 )
                             continue
+                        if isinstance(widget, Signal):
+                            continue
                         widget = self._create_widget_from_method(widget)
 
                         # contextmenu
                         contextmenu = get_additional_option(attr, "context_menu", None)
                         if contextmenu is not None:
                             contextmenu: ContextMenuGui
                             contextmenu._set_magic_context_menu(widget)
@@ -196,15 +204,15 @@
                         if isinstance(widget, BaseGui):
                             widget._my_symbol = Symbol(name)
                         # magic-class has to know its parent.
                         # if __magicclass_parent__ is defined as a property, hasattr must be called
                         # with a type object (not instance).
                         widget.__magicclass_parent__ = self
 
-                    if name.startswith("_"):
+                    if widget.name.startswith("_"):
                         continue
 
                     moveto = get_additional_option(attr, "into")
                     copyto = get_additional_option(attr, "copyto", [])
                     if moveto is not None or copyto:
                         self._unwrap_method(name, widget, moveto, copyto)
                     else:
@@ -214,15 +222,17 @@
 
             except Exception as e:
                 format_error(e, _hist, name, attr)
 
         self._unify_label_widths()
         return None
 
-    def _fast_insert(self, key: int, obj: AbstractAction | Callable) -> None:
+    def _fast_insert(
+        self, key: int, obj: AbstractAction | Callable, remove_label: bool = False
+    ) -> None:
         """
         Insert object into the toolbar. Could be widget or callable.
 
         Parameters
         ----------
         key : int
             Position to insert.
@@ -233,15 +243,15 @@
             # Sometimes users want to dynamically add new functions to GUI.
             if isinstance(obj, FunctionGui):
                 if obj.parent is None:
                     f = nested_function_gui_callback(self, obj)
                     obj.called.connect(f)
                 _obj = obj
             else:
-                obj = _inject_recorder(obj, is_method=False).__get__(self)
+                obj = inject_recorder(obj, is_method=False).__get__(self)
                 _obj = self._create_widget_from_method(obj)
 
             method_name = getattr(obj, "__name__", None)
             if method_name and not hasattr(self, method_name):
                 object.__setattr__(self, method_name, obj)
         else:
             _obj = obj
@@ -263,28 +273,29 @@
                     FreeWidget,
                     Label,
                     FunctionGui,
                     Image,
                     Table,
                 )
                 _obj_labeled = _obj
-                if (not isinstance(_obj.widget, _hide_labels)) and self.labels:
-                    _obj_labeled = _LabeledWidgetAction.from_action(_obj)
+                if self.labels:
+                    if not isinstance(_obj.widget, _hide_labels) and not remove_label:
+                        _obj_labeled = _LabeledWidgetAction.from_action(_obj)
                 _obj_labeled.parent = self
                 insert_action_like(self.native, key, _obj_labeled.native)
             self._list.insert(key, _obj)
         else:
             raise TypeError(f"{type(_obj)} is not supported.")
 
     def insert(self, key: int, obj: AbstractAction) -> None:
         self._fast_insert(key, obj)
         self._unify_label_widths()
 
 
-def _create_stylesheet(viewer: Viewer):
+def _create_stylesheet(viewer: napari.Viewer):
     if viewer is None:
         return ""
     w = viewer.window._qt_window
     styles = []
     for s in w.styleSheet().split("\n\n"):
         if s.startswith("QPushButton ") or s.startswith("QPushButton:"):
             styles.append("QToolButton" + s[11:])
```

### Comparing `magic-class-0.6.9/magicclass/_gui/utils.py` & `magic_class-0.7.0rc0/magicclass/_gui/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 from typing import Any, TYPE_CHECKING, Callable, TypeVar
 from types import FunctionType
 
+from magicgui import __version__ as _magicgui_version
 from magicgui.widgets import FunctionGui, Widget
-from magicgui.widgets._bases.value_widget import UNSET
+from magicgui.types import Undefined
 from magicgui.type_map import get_widget_class
-from magicgui.signature import magic_signature, MagicParameter, split_annotated_type
+from magicgui.signature import magic_signature, MagicParameter
 
 from macrokit import Symbol
+from magicclass.signature import split_annotated_type
 
 if TYPE_CHECKING:
     from ._base import BaseGui
+    from magicgui.widgets import FunctionGui, FileEdit
 
 
 def get_parameters(fgui: FunctionGui):
     return {k: v.default for k, v in fgui.__signature__.parameters.items()}
 
 
 _C = TypeVar("_C", bound=type)
@@ -91,22 +94,38 @@
     """Connect magicclass parent/child."""
 
     child.__magicclass_parent__ = parent
     parent.__magicclass_children__.append(child)
     child._my_symbol = Symbol(child_name)
 
 
-def callable_to_classes(f: Callable) -> list[type[Widget]]:
+def callable_to_classes(f: Callable) -> list[tuple[type[Widget], MagicParameter]]:
     """Get list of classes that will be generated by the magicgui type map."""
     sig = magic_signature(f)
-    return [_parameter_to_widget_class(p) for p in sig.parameters.values()]
+    return [(_parameter_to_widget_class(p), p) for p in sig.parameters.values()]
+
+
+def show_dialog_from_mgui(mgui: FunctionGui):
+    """Show file dialog from given magicgui widget."""
+    fdialog: FileEdit = mgui[0]
+    if result := fdialog._show_file_dialog(
+        fdialog.mode,
+        caption=fdialog._btn_text,
+        start_path=str(fdialog.value),
+        filter=fdialog.filter,
+    ):
+        fdialog.value = result
+        out = mgui(result)
+    else:
+        out = None
+    return out
 
 
 TZ_EMPTY = "__no__default__"
 
 
 def _parameter_to_widget_class(param: MagicParameter):
-    value = UNSET if param.default in (param.empty, TZ_EMPTY) else param.default
+    value = Undefined if param.default in (param.empty, TZ_EMPTY) else param.default
     annotation, options = split_annotated_type(param.annotation)
     options = options.copy()
-    wdg_class, _ = get_widget_class(value, annotation, options)
+    wdg_class, _ = get_widget_class(value, annotation, options, raise_on_unknown=False)
     return wdg_class
```

### Comparing `magic-class-0.6.9/magicclass/_register_types.py` & `magic_class-0.7.0rc0/magicclass/_register_types.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 from __future__ import annotations
 import macrokit as mk
 from macrokit import Expr, Head, symbol
 from enum import Enum
-from pathlib import Path
+import pathlib
 import datetime
-from .types import Color
-from .widgets import ColorEdit
-from .widgets.sequence import ListDataView
-from ._gui._base import MagicTemplate
+from magicclass.types import Color, Path, ExprStr
+from magicclass.widgets import ColorEdit, EvalLineEdit
+from magicclass._gui._base import MagicTemplate
 
 # classes
 _datetime = Expr(Head.getattr, [datetime, datetime.datetime])
 _date = Expr(Head.getattr, [datetime, datetime.date])
 _time = Expr(Head.getattr, [datetime, datetime.time])
+_timedelta = Expr(Head.getattr, [datetime, datetime.timedelta])
 
 # magicgui-style input
 mk.register_type(Enum, lambda e: symbol(e.value))
-mk.register_type(Path, lambda e: f"r'{e}'")
-mk.register_type(ListDataView, lambda e: list(e))
+mk.register_type(pathlib.Path, lambda e: f"r'{e}'")
+mk.register_type(float, lambda e: str(round(e, 8)))
+
+try:
+    from magicgui.widgets._concrete import ListDataView
+except ImportError:
+    pass
+else:
+    mk.register_type(ListDataView, lambda e: list(e))
+
 mk.register_type(
     datetime.datetime,
     lambda e: Expr.parse_call(
         _datetime, (e.year, e.month, e.day, e.hour, e.minute), {}
     ),
 )
+
 mk.register_type(
     datetime.date, lambda e: Expr.parse_call(_date, (e.year, e.month, e.day), {})
 )
 mk.register_type(
     datetime.time, lambda e: Expr.parse_call(_time, (e.hour, e.minute), {})
 )
+mk.register_type(
+    datetime.timedelta, lambda e: Expr.parse_call(_timedelta, (e.days, e.seconds), {})
+)
 
 
 @mk.register_type(MagicTemplate)
 def find_myname(gui: MagicTemplate):
     """This function is the essential part of macro recording"""
     parent = gui.__magicclass_parent__
     if parent is None:
@@ -41,7 +53,11 @@
     else:
         return Expr(Head.getattr, [find_myname(parent), gui._my_symbol])
 
 
 import magicgui as mgui
 
 mgui.register_type(Color, widget_type=ColorEdit)
+mgui.register_type(Path.Save, widget_type="FileEdit", mode="w")
+mgui.register_type(Path.Dir, widget_type="FileEdit", mode="d")
+mgui.register_type(Path.Multiple, widget_type="FileEdit", mode="rm")
+mgui.register_type(ExprStr, widget_type=EvalLineEdit)
```

### Comparing `magic-class-0.6.9/magicclass/core.py` & `magic_class-0.7.0rc0/magicclass/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 from functools import wraps as functools_wraps
 import inspect
+from types import ModuleType
 from weakref import WeakValueDictionary
 from typing import Any, TYPE_CHECKING, Callable
+from macrokit import Symbol, Expr
 
-from ._gui.class_gui import (
+from magicclass._gui.class_gui import (
     ClassGuiBase,
     ClassGui,
     FrameClassGui,
     GroupBoxClassGui,
     MainWindowClassGui,
     SubWindowsClassGui,
     ScrollableClassGui,
@@ -18,38 +20,43 @@
     HCollapsibleClassGui,
     SplitClassGui,
     TabbedClassGui,
     StackedClassGui,
     ToolBoxClassGui,
     ListClassGui,
 )
-from ._gui._base import (
+from magicclass._gui._base import (
     PopUpMode,
     ErrorMode,
     defaults,
     MagicTemplate,
     check_override,
     convert_attributes,
 )
-from ._gui import ContextMenuGui, MenuGui, ToolBarGui
-from ._app import get_app
-from .types import WidgetType
-from . import _register_types  # activate type registration things.
+from magicclass._gui import ContextMenuGui, MenuGui, ToolBarGui
+from magicclass._app import get_app
+from magicclass.types import WidgetType
+
+# activate type registration things.
+from magicclass import _register_types
+
+del _register_types
 
 if TYPE_CHECKING:
-    from .stylesheets import StyleSheet
-    from ._gui import MenuGuiBase
-    from ._gui._function_gui import FunctionGuiPlus
-    from .types import WidgetTypeStr, PopUpModeStr, ErrorModeStr
-    from .help import HelpWidget
+    from magicclass.stylesheets import StyleSheet
+    from magicclass._gui import MenuGuiBase
+    from magicclass._gui.mgui_ext import Clickable
+    from magicclass._gui._function_gui import FunctionGuiPlus
+    from magicclass.types import WidgetTypeStr, PopUpModeStr, ErrorModeStr
+    from magicclass.help import HelpWidget
     from macrokit import Macro
 
-_BASE_CLASS_SUFFIX = "_Base"
+_BASE_CLASS_SUFFIX = ".base"
 
-_TYPE_MAP = {
+_TYPE_MAP: dict[WidgetType, type[ClassGuiBase]] = {
     WidgetType.none: ClassGui,
     WidgetType.scrollable: ScrollableClassGui,
     WidgetType.draggable: DraggableClassGui,
     WidgetType.split: SplitClassGui,
     WidgetType.collapsible: CollapsibleClassGui,
     WidgetType.hcollapsible: HCollapsibleClassGui,
     WidgetType.button: ButtonClassGui,
@@ -73,53 +80,59 @@
     visible: bool | None = None,
     close_on_run: bool = None,
     popup_mode: PopUpModeStr | PopUpMode = None,
     error_mode: ErrorModeStr | ErrorMode = None,
     widget_type: WidgetTypeStr | WidgetType = WidgetType.none,
     icon: Any | None = None,
     stylesheet: str | StyleSheet = None,
+    properties: dict[str, Any] = None,
+    record: bool = True,
+    symbol: str = "ui",
 ):
     """
     Decorator that can convert a Python class into a widget.
 
-    .. code-block:: python
-
-        @magicclass
-        class C:
-            ...
-        ui = C()
-        ui.show()  # open GUI
+    >>> @magicclass
+    >>> class C:
+    >>>     ...
+    >>> ui = C()
+    >>> ui.show()  # open GUI
 
     Parameters
     ----------
     class_ : type, optional
         Class to be decorated.
     layout : str, "vertical" or "horizontal", default is "vertical"
         Layout of the main widget.
     labels : bool, default is True
         If true, magicgui labels are shown.
     name : str, optional
         Name of GUI.
     visible : bool, optional
         Initial visibility of GUI. Useful when magic class is nested.
     close_on_run : bool, default is True
-        If True, magicgui created by every method will be deleted after the method is completed without
-        exceptions, i.e. magicgui is more like a dialog.
-    popup : bool, default is True
-        Deprecated.
+        If True, magicgui created by every method will be deleted after the method is
+        completed without exceptions, i.e. magicgui is more like a dialog.
     popup_mode : str or PopUpMode, default is PopUpMode.popup
         Option of how to popup FunctionGui widget when a button is clicked.
     error_mode : str or ErrorMode, default is ErrorMode.msgbox
         Option of how to raise errors during function calls.
     widget_type : WidgetType or str, optional
         Widget type of container.
     icon : Any, optional
         Path to the icon image or any object that can be converted into an icon.
     stylesheet : str or StyleSheet object, optional
         Set stylesheet to the widget if given.
+    properties : dict, optional
+        Set properties to the widget if given. This argument is useful when you want
+        to set width, height or margin without defining __post_init__.
+    record : bool, default is True
+        If True, macro recording is enabled.
+    symbol : str, default is "ui"
+        The identifier used in macro to represent this widget.
 
     Returns
     -------
     Decorated class or decorator.
     """
     if popup_mode is None:
         popup_mode = defaults["popup_mode"]
@@ -145,15 +158,15 @@
         # get class attributes first
         doc = cls.__doc__
         sig = inspect.signature(cls)
         annot = cls.__dict__.get("__annotations__", {})
         mod = cls.__module__
         qualname = cls.__qualname__
 
-        new_attrs = convert_attributes(cls, hide=class_gui.__mro__)
+        new_attrs = convert_attributes(cls, hide=class_gui.__mro__, record=record)
         oldclass = type(cls.__name__ + _BASE_CLASS_SUFFIX, (cls,), {})
         newclass = type(cls.__name__, (class_gui, oldclass), new_attrs)
 
         newclass.__signature__ = sig
         newclass.__doc__ = doc
         newclass.__module__ = mod
         newclass.__qualname__ = qualname
@@ -178,21 +191,15 @@
             )
 
             # Inheriting Container's constructor is the most intuitive way.
             if kwargs and "__init__" not in cls.__dict__:
                 gui_kwargs.update(kwargs)
                 kwargs = {}
 
-            class_gui.__init__(
-                self,
-                **gui_kwargs,
-            )
-            # prepare macro
-            macrowidget = self.macro.widget.native
-            macrowidget.setParent(self.native, macrowidget.windowFlags())
+            class_gui.__init__(self, **gui_kwargs)
 
             with self.macro.blocked():
                 super(oldclass, self).__init__(*args, **kwargs)
 
             self._convert_attributes_into_widgets()
 
             if widget_type in (WidgetType.collapsible, WidgetType.button):
@@ -201,14 +208,18 @@
             if icon:
                 self.icon = icon
             if stylesheet:
                 self.native.setStyleSheet(str(stylesheet))
             if hasattr(self, "__post_init__"):
                 with self.macro.blocked():
                     self.__post_init__()
+            if properties:
+                for k, v in properties.items():
+                    setattr(self, k, v)
+            self._my_symbol = _as_symbol(symbol)
 
         newclass.__init__ = __init__
 
         # Users may want to override repr
         newclass.__repr__ = oldclass.__repr__
 
         return newclass
@@ -224,14 +235,15 @@
     *,
     close_on_run: bool = None,
     popup_mode: str | PopUpMode = None,
     error_mode: str | ErrorMode = None,
     labels: bool = True,
     name: str | None = None,
     icon: Any | None = None,
+    record: bool = True,
 ):
     """Decorator that converts a Python class into a menu bar."""
     return _call_magicmenu(**locals(), menugui_class=MenuGui)
 
 
 def magiccontext(
     class_: type = None,
@@ -239,14 +251,15 @@
     into: Callable | None = None,
     close_on_run: bool = None,
     popup_mode: str | PopUpMode = None,
     error_mode: str | ErrorMode = None,
     labels: bool = True,
     name: str | None = None,
     icon: Any | None = None,
+    record: bool = True,
 ):
     """Decorator that converts a Python class into a context menu."""
 
     if popup_mode is None:
         popup_mode = defaults["popup_mode"]
     if close_on_run is None:
         close_on_run = defaults["close_on_run"]
@@ -270,15 +283,15 @@
 
         # get class attributes first
         doc = cls.__doc__
         sig = inspect.signature(cls)
         mod = cls.__module__
         qualname = cls.__qualname__
 
-        new_attrs = convert_attributes(cls, hide=ContextMenuGui.__mro__)
+        new_attrs = convert_attributes(cls, hide=ContextMenuGui.__mro__, record=record)
         oldclass = type(cls.__name__ + _BASE_CLASS_SUFFIX, (cls,), {})
         newclass = type(cls.__name__, (ContextMenuGui, oldclass), new_attrs)
 
         newclass.__signature__ = sig
         newclass.__doc__ = doc
         newclass.__module__ = mod
         newclass.__qualname__ = qualname
@@ -297,21 +310,15 @@
             )
 
             # Inheriting Container's constructor is the most intuitive way.
             if kwargs and "__init__" not in cls.__dict__:
                 gui_kwargs.update(kwargs)
                 kwargs = {}
 
-            ContextMenuGui.__init__(
-                self,
-                **gui_kwargs,
-            )
-
-            macrowidget = self.macro.widget.native
-            macrowidget.setParent(self.native, macrowidget.windowFlags())
+            ContextMenuGui.__init__(self, **gui_kwargs)
 
             with self.macro.blocked():
                 super(oldclass, self).__init__(*args, **kwargs)
 
             self._convert_attributes_into_widgets()
 
             if icon:
@@ -339,27 +346,29 @@
     *,
     close_on_run: bool = None,
     popup_mode: str | PopUpMode = None,
     error_mode: str | ErrorMode = None,
     labels: bool = True,
     name: str | None = None,
     icon: Any | None = None,
+    record: bool = True,
 ):
     """Decorator that converts a Python class into a menu bar."""
     return _call_magicmenu(**locals(), menugui_class=ToolBarGui)
 
 
 def _call_magicmenu(
     class_: type = None,
     close_on_run: bool = True,
     popup_mode: str | PopUpMode = None,
     error_mode: str | ErrorMode = None,
     labels: bool = True,
     name: str = None,
     icon: Any | None = None,
+    record: bool = True,
     menugui_class: type[MenuGuiBase] = None,
 ):
     """
     Parameters
     ----------
     class_ : type, optional
         Class to be decorated.
@@ -399,15 +408,15 @@
 
         # get class attributes first
         doc = cls.__doc__
         sig = inspect.signature(cls)
         mod = cls.__module__
         qualname = cls.__qualname__
 
-        new_attrs = convert_attributes(cls, hide=menugui_class.__mro__)
+        new_attrs = convert_attributes(cls, hide=menugui_class.__mro__, record=record)
         oldclass = type(cls.__name__ + _BASE_CLASS_SUFFIX, (cls,), {})
         newclass = type(cls.__name__, (menugui_class, oldclass), new_attrs)
 
         newclass.__signature__ = sig
         newclass.__doc__ = doc
         newclass.__module__ = mod
         newclass.__qualname__ = qualname
@@ -426,21 +435,15 @@
             )
 
             # Inheriting Container's constructor is the most intuitive way.
             if kwargs and "__init__" not in cls.__dict__:
                 gui_kwargs.update(kwargs)
                 kwargs = {}
 
-            menugui_class.__init__(
-                self,
-                **gui_kwargs,
-            )
-
-            macrowidget = self.macro.widget.native
-            macrowidget.setParent(self.native, macrowidget.windowFlags())
+            menugui_class.__init__(self, **gui_kwargs)
 
             with self.macro.blocked():
                 super(oldclass, self).__init__(*args, **kwargs)
 
             self._convert_attributes_into_widgets()
 
             if icon:
@@ -488,33 +491,81 @@
         if parent is None:
             parent = ui.native
         help_widget = HelpWidget(ui, parent=parent)
         _HELPS[ui_id] = help_widget
     return help_widget
 
 
-def get_function_gui(ui: MagicTemplate, name: str) -> FunctionGuiPlus:
+def get_button(ui: MagicTemplate | ModuleType, name: str | None = None) -> Clickable:
     """
-    Get the FunctionGui object hidden beneath push button or menu.
+    Get the button/action object for the given method.
 
-    This function is a helper function for magicclass.
+    This function is a helper function for magicclass. Using this method is
+    always safer than directly accessing it by ``ui["method"]``.
+    Either of following expression is allowed.
+
+    >>> get_button(ui, "method")
+    >>> get_button(ui.method)
+
+    """
+    if name is None:
+        if hasattr(ui, "__self__") and callable(ui):
+            func = ui
+            ui = func.__self__
+            name = func.__name__
+        else:
+            raise TypeError(
+                "The first argument of `get_button() must be a method if "
+                "the method name is not given."
+            )
+    widget: Clickable = ui[name]
 
-    Parameters
-    ----------
-    ui : MagicTemplate
-        Any of a magic-class instance.
-    name : str
-        Name of method (or strictly speaking, the name of PushButton).
+    if not hasattr(widget, "mgui"):
+        raise TypeError(f"Widget {widget} does not have FunctionGui inside it.")
 
-    Returns
-    -------
-    FunctionGuiPlus
-        FunctionGui object.
-    """
-    func = getattr(ui, name)
+    if widget._unwrapped:
+        from magicclass.signature import get_additional_option
+
+        opt = get_additional_option(getattr(ui, name), "into", None)
+        if opt is not None:
+            for child_instance in ui._iter_child_magicclasses():
+                _name = child_instance.__class__.__name__
+                if _name == opt:
+                    widget = child_instance[name]
+                    return widget
+            raise ValueError(f"Could not find {opt} in {ui}.")
+    return widget
+
+
+def get_function_gui(
+    ui: MagicTemplate | ModuleType, name: str = None
+) -> FunctionGuiPlus:
+    """
+    Get the FunctionGui object hidden beneath push button or menu action.
+
+    This function is a helper function for magicclass. Using this method is
+    always safer than directly accessing it by ``ui["method"].mgui``.
+    Either of following expression is allowed.
+
+    >>> get_function_gui(ui, "method")
+    >>> get_function_gui(ui.method)
+
+    """
+    if name is None:
+        if hasattr(ui, "__self__") and callable(ui):
+            func = ui
+            ui = func.__self__
+            name = func.__name__
+        else:
+            raise TypeError(
+                "The first argument of `get_function_gui() must be a method if "
+                "the method name is not given."
+            )
+    else:
+        func = getattr(ui, name)
     widget = ui[name]
 
     if not hasattr(widget, "mgui"):
         raise TypeError(f"Widget {widget} does not have FunctionGui inside it.")
 
     if widget.mgui is not None:
         return widget.mgui
@@ -559,72 +610,53 @@
     Parameters
     ----------
     ui : MagicTemplate
         Magic class instance.
     macro : Macro or str, optional
         An executable macro or string that dictates how GUI will be updated.
     """
-    from macrokit import Head, Expr, Macro
+    from macrokit import Head, Macro
 
     if macro is None:
         macro = ui.macro
     elif isinstance(macro, str):
         s = macro
         macro = Macro()
         for line in s.split("\n"):
             macro.append(line)
     elif not isinstance(macro, Macro):
         raise TypeError(
             f"The second argument must be a Macro or str, got {type(macro)}."
         )
 
     for expr in macro:
-        if expr.head == Head.call:
+        if expr.head is Head.call:
             # ui.func(...)
-            ui_f, *arguments = expr.args
-            fname = str(ui_f.args[1])
+            fname = str(expr.at(0, 1))
+            args, kwargs = expr.eval_call_args()
             if fname.startswith("_"):
                 if fname != "_call_with_return_callback":
                     continue
-                args, kwargs = _arguments_to_values(arguments)
                 fgui = get_function_gui(ui, args[0])
 
             else:
-                args, kwargs = _arguments_to_values(arguments)
                 fgui = get_function_gui(ui, fname)
 
             with fgui.changed.blocked():
                 for key, value in kwargs.items():
                     getattr(fgui, key).value = value
 
-        elif expr.head == Head.assign:
+        elif expr.head is Head.assign:
             # ui.field.value = ...
             # ui.vfield = ...
             expr.eval({}, {str(ui._my_symbol): ui})
 
     return None
 
 
-def _tuple(*args) -> tuple:
-    return args
-
-
-def _arguments_to_values(arguments) -> tuple[tuple, dict[str, Any]]:
-    from macrokit import Head, Expr, symbol
-
-    for i, arg in enumerate(arguments):
-        if isinstance(arg, Expr) and arg.head == Head.kw:
-            break
-    args = arguments[:i]
-    kwargs: list[Expr] = arguments[i:]
-    args = Expr(Head.call, [_tuple] + args).eval({symbol(_tuple): _tuple})
-    kwargs = Expr(Head.call, [dict] + kwargs).eval()
-    return args, kwargs
-
-
 class Parameters:
     def __init__(self):
         self.__name__ = self.__class__.__name__
         self.__qualname__ = self.__class__.__qualname__
 
         sig = [
             inspect.Parameter(name="self", kind=inspect.Parameter.POSITIONAL_OR_KEYWORD)
@@ -657,19 +689,24 @@
         for a, param in zip(args, params):
             setattr(self, param, a)
 
     def as_dict(self) -> dict[str, Any]:
         """
         Convert parameter fields into a dictionary.
 
-        .. code-block:: python
-
-            class params(Parameters):
-                i = 1
-                j = 2
-
-            p = params()
-            p.as_dict() # {"i": 1, "j": 2}
+        >>> class params(Parameters):
+        >>>     i = 1
+        >>>     j = 2
 
+        >>> p = params()
+        >>> p.as_dict() # {"i": 1, "j": 2}
         """
         params = list(self.__signature__.parameters.keys())[1:]
         return {param: getattr(self, param) for param in params}
+
+
+def _as_symbol(s: str) -> Symbol | Expr:
+    if isinstance(s, str):
+        return Symbol(s)
+    elif not isinstance(s, (Symbol, Expr)):
+        raise TypeError(f"Expected a string or Symbol, got {type(s)}.")
+    return s
```

### Comparing `magic-class-0.6.9/magicclass/ext/_doc.py` & `magic_class-0.7.0rc0/magicclass/ext/_doc.py`

 * *Files identical despite different names*

### Comparing `magic-class-0.6.9/magicclass/ext/dask/progress.py` & `magic_class-0.7.0rc0/magicclass/ext/dask/progress.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 from __future__ import annotations
 from functools import wraps
+import inspect
 from typing import Any, Callable, TYPE_CHECKING
 from dask.diagnostics import Callback as DaskCallback
 from psygnal import Signal
 from superqt.utils import FunctionWorker, GeneratorWorker, create_worker
 
-from ...utils import move_to_screen_center, QtSignal
-from ...utils.qthreading import (
+from magicclass.utils import move_to_screen_center, QtSignal
+from magicclass.utils.qthreading import (
     CallbackList,
     DefaultProgressBar,
     thread_worker,
     ProgressDict,
 )
 
 if TYPE_CHECKING:
-    from ..._gui import BaseGui
+    from magicclass._gui import BaseGui
 
 
 class DaskProgressBar(DefaultProgressBar, DaskCallback):
     """A progress bar widget for dask computation."""
 
     computed = Signal(object)
+    new_cycle = Signal(int)
 
     def __init__(
         self,
         max: int = 100,
         minimum: float = 0.5,
         dt: float = 0.1,
     ):
         self._minimum = minimum
         self._dt = dt
         self._frac = 0.0
         self._n_computation = 0
         super().__init__(max=max)
-        self.footer[1].visible = self.footer[2].visible = False
         self._computed_signal = QtSignal()
         self._computed_signal.connect(self._on_computed)
 
     def __enter__(self):
         self._n_computation = 0
         self._on_timer_updated()
         return super().__enter__()
 
     def _start(self, dsk):
         self._state = None
         self._frac = 0.0
+        self.new_cycle.emit(self._n_computation)
         self._n_computation += 1
+        self._timer.reset()
         self._start_thread()
         return None
 
     def _on_computed(self, result):
         s = self._state
         if not s:
             self._frac = 0.0
@@ -67,42 +70,50 @@
         return None
 
     def _posttask(self, key, result, dsk, state, worker_id):
         self._computed_signal.emit(result)
         self._time_signal.emit()
         return None
 
-    def _finish(self, dsk, state, errored):
+    def _finish(self, dsk=None, state=None, errored=None):
         self._frac = 1.0
         self._running = False
         self._thread_timer.join()
-        self._timer.reset()
         return None
 
     def _on_timer_updated(self, _=None):
-        if self._n_computation > 1:
-            _prefix = f"({self._n_computation}) "
-        else:
-            _prefix = ""
         if self._timer.sec < 3600:
-            self.time_label.value = _prefix + self._timer.format_time(
-                "{min:0>2}:{sec:0>2}"
-            )
+            self.time_label.value = self._timer.format_time("{min:0>2}:{sec:0>2}")
         else:
-            self.time_label.value = _prefix + self._timer.format_time()
+            self.time_label.value = self._timer.format_time()
         return None
 
     def set_worker(self, worker: GeneratorWorker | FunctionWorker):
         """Set currently running worker."""
         self._worker = worker
-        if isinstance(self._worker, GeneratorWorker):
-            raise TypeError("Cannot set generator.")
-        self.footer[1].visible = False
-        self.footer[2].visible = False
-        self._time_signal.emit()
+        if not isinstance(self._worker, GeneratorWorker):
+            # FunctionWorker does not have yielded/aborted signals.
+            self.hide_footer()
+            return None
+        # initialize abort_button
+        self.abort_button.text = "Abort"
+        self.abort_button.changed.connect(self._abort_worker)
+        self.abort_button.enabled = True
+
+        # initialize pause_button
+        self.pause_button.text = "Pause"
+        self.pause_button.enabled = True
+        self.pause_button.changed.connect(self._toggle_pause)
+
+        @self._worker.paused.connect
+        def _on_pause():
+            self.pause_button.text = "Resume"
+            self.pause_button.enabled = True
+            self._timer.stop()
+
         return None
 
 
 class dask_thread_worker(thread_worker):
     """
     Create a dask's worker in a superqt/napari style.
 
@@ -151,14 +162,15 @@
 
     def _create_method(self, gui: BaseGui):
         if self._progress is None:
             self._progress = {
                 "pbar": None,
                 "desc": "Progress",
                 "total": 100,
+                "descs": [],
             }
         else:
             self._progress["pbar"] = None
 
         return super()._create_method(gui)
 
     def _create_qt_worker(
@@ -166,28 +178,71 @@
     ) -> FunctionWorker | GeneratorWorker:
         gui_id = id(gui)
 
         pbar = self._DEFAULT_PROGRESS_BAR(max=self._DEFAULT_TOTAL)
         self._progressbars[gui_id] = pbar
         for c in self.computed._iter_as_method(gui):
             pbar.computed.connect(c)
+        if descs := self._progress.get("descs"):
+            if callable(descs):
+                arguments = self.__signature__.bind(gui, *args, **kwargs)
+                arguments.apply_defaults()
+                _descs = lambda: descs(**_filter_args(descs, arguments.arguments))
+            else:
+                _descs = lambda: iter(descs)
+            self._progress["desc"] = next(_descs(), "<No description>")
+            it = _descs()
+
+            @pbar.new_cycle.connect
+            def _(i: int):
+                pbar.set_description(next(it, "<No description>"))
+
         pbar.native.setParent(gui.native, self.__class__._WINDOW_FLAG)
         move_to_screen_center(pbar.native)
 
         worker = create_worker(
-            self._define_function(pbar).__get__(gui),
+            self._define_function(pbar, gui).__get__(gui),
             _ignore_errors=self._ignore_errors,
             _start_thread=False,
             *args,
             **kwargs,
         )
+        if self.is_generator:
+
+            @self.yielded.connect
+            def _(*args):
+                pbar.value = 0
 
         return worker
 
-    def _define_function(self, pbar):
-        @wraps(self._func)
-        def _wrapped(*args, **kwargs):
-            with pbar:
-                out = self._func(*args, **kwargs)
-            return out
+    def _define_function(self, pbar, gui: BaseGui):
+        if inspect.isgeneratorfunction(self._func):
+
+            @wraps(self._func)
+            def _wrapped(*args, **kwargs):
+                with pbar:
+                    with gui.macro.blocked():
+                        out = yield from self._func(*args, **kwargs)
+                return out
+
+        else:
+
+            @wraps(self._func)
+            def _wrapped(*args, **kwargs):
+                with pbar:
+                    with gui.macro.blocked():
+                        out = self._func(*args, **kwargs)
+                return out
 
         return _wrapped
+
+
+def _filter_args(fn: Callable, arguments: dict[str, Any]) -> dict[str, Any]:
+    sig = inspect.signature(fn)
+    params = sig.parameters
+    nparams = len(params)
+    if nparams == 0:
+        return {}
+    if list(sig.parameters.values())[-1] == inspect.Parameter.VAR_KEYWORD:
+        return arguments
+    existing_args = set(sig.parameters.keys())
+    return {k: v for k, v in arguments.items() if k in existing_args}
```

### Comparing `magic-class-0.6.9/magicclass/ext/dask/resource.py` & `magic_class-0.7.0rc0/magicclass/ext/dask/resource.py`

 * *Files identical despite different names*

### Comparing `magic-class-0.6.9/magicclass/ext/napari/_magicgui.py` & `magic_class-0.7.0rc0/magicclass/ext/napari/_magicgui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 from __future__ import annotations
 
 from typing import Iterable, Callable, TYPE_CHECKING
 from magicgui import register_type, application as app
 from magicgui.widgets import Container, ComboBox, Label, Widget
-from magicgui.widgets._bases import CategoricalWidget
 
+import macrokit as mk
+
+import napari
 from napari.utils._magicgui import find_viewer_ancestor
 
 if TYPE_CHECKING:
     from .types import Features, FeatureColumn
 
 
-def get_features(widget: CategoricalWidget) -> list[tuple[str, Features]]:
+def get_features(widget: Widget) -> list[tuple[str, Features]]:
     """Get all the non-empty feature data from the viewer."""
     viewer = find_viewer_ancestor(widget)
     if viewer is None:
         return []
+    viewer_mock = mk.Mock("viewer")
     features: list[Features] = []
     for layer in viewer.layers:
         if len(feat := getattr(layer, "features", [])) > 0:
+            # very dirty solution ...
+            feat._macrokit_expr = viewer_mock.layers[layer.name].features
             features.append((layer.name, feat))
     return features
 
 
 # Widget
 class ColumnChoice(Container):
     def __init__(
@@ -115,14 +120,16 @@
         df = self._dataframe_cbox.value
         colnames = [cbox.value for cbox in self._column_names_cbox]
         return (df, colnames)
 
 
 def _register_mgui_types():
     from .types import Features, FeatureColumn, FeatureInfoInstance
+    import macrokit as mk
+    from macrokit.mock import Mock
 
     register_type(Features, choices=get_features, nullable=False)
 
     register_type(
         FeatureColumn,
         widget_type=ColumnChoice,
         data_choices=get_features,
@@ -130,7 +137,11 @@
     )
 
     register_type(
         FeatureInfoInstance,
         widget_type=ColumnNameChoice,
         data_choices=get_features,
     )
+
+    @mk.register_type(Features)
+    def _format_feature(x: Features) -> str:
+        return getattr(x, "_macrokit_expr", mk.Symbol.make_symbol_str(x))
```

### Comparing `magic-class-0.6.9/magicclass/ext/napari/types.py` & `magic_class-0.7.0rc0/magicclass/ext/napari/types.py`

 * *Files identical despite different names*

### Comparing `magic-class-0.6.9/magicclass/ext/napari/utils.py` & `magic_class-0.7.0rc0/magicclass/ext/napari/utils.py`

 * *Files identical despite different names*

### Comparing `magic-class-0.6.9/magicclass/ext/napari/viewer.py` & `magic_class-0.7.0rc0/magicclass/ext/napari/viewer.py`

 * *Files identical despite different names*

### Comparing `magic-class-0.6.9/magicclass/ext/napari/widgets.py` & `magic_class-0.7.0rc0/magicclass/ext/napari/widgets.py`

 * *Files identical despite different names*

### Comparing `magic-class-0.6.9/magicclass/ext/pyqtgraph/__init__.py` & `magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `magic-class-0.6.9/magicclass/ext/pyqtgraph/components.py` & `magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,20 @@
 
     @border.setter
     def border(self, value):
         value = convert_color_code(value)
         self.native.setPen(pg.mkPen(value))
         self.native._updateView()
 
+class Grid(GraphicComponent):
+    native: pg.GridItem
+    
+    def __init__(self) -> None:
+        self.native = pg.GridItem()
+
 
 class TextItem(GraphicComponent):
     """A text item with napari-like API."""
 
     native: pg.TextItem
 
     def __init__(
```

### Comparing `magic-class-0.6.9/magicclass/ext/pyqtgraph/graph_items.py` & `magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/graph_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 from typing import Sequence
 import pyqtgraph as pg
+from qtpy import QtGui
 from qtpy.QtCore import Qt
 import numpy as np
+from numpy.typing import NDArray
 
 from .._shared_utils import convert_color_code, to_rgba
 
 # compatibility with matplotlib
 _LINE_STYLE = {
-    "-": Qt.SolidLine,
-    "--": Qt.DashLine,
-    ":": Qt.DotLine,
-    "-.": Qt.DashDotLine,
+    "-": Qt.PenStyle.SolidLine,
+    "--": Qt.PenStyle.DashLine,
+    ":": Qt.PenStyle.DotLine,
+    "-.": Qt.PenStyle.DashDotLine,
 }
 
 _SYMBOL_MAP = {
     "*": "star",
     "D": "d",
     "^": "t1",
     "<": "t3",
@@ -180,28 +182,30 @@
         self.native = pg.ScatterPlotItem(
             x=x, y=y, pen=pen, brush=brush, size=size, symbol=symbol
         )
         self.name = name
 
     @property
     def symbol(self):
+        """Get the symbol of the scatter plot."""
         return self.native.opts["symbol"]
 
     @symbol.setter
     def symbol(self, value):
         value = _SYMBOL_MAP.get(value, value)
         self.native.setSymbol(value)
 
     @property
     def size(self):
-        return self.native.opts["symbolSize"]
+        """Get the size of the scatter plot."""
+        return self.native.opts["size"]
 
     @size.setter
     def size(self, size: float):
-        self.native.setSymbolSize(size)
+        self.native.setSize(size)
 
 
 class Curve(PlotDataLayer):
     native: pg.PlotDataItem
 
     def __init__(
         self,
@@ -247,26 +251,26 @@
         return self.native.opts["symbolSize"]
 
     @size.setter
     def size(self, size: float):
         self.native.setSymbolSize(size)
 
     @property
-    def edge_color(self) -> np.ndarray:
+    def edge_color(self) -> NDArray[np.float64]:
         rgba = self.native.opts["pen"].color().getRgb()
         return np.array(rgba) / 255
 
     @edge_color.setter
     def edge_color(self, value: str | Sequence):
         value = convert_color_code(value)
         self.native.setPen(value)
         self.native.setSymbolPen(value)
 
     @property
-    def face_color(self) -> np.ndarray:
+    def face_color(self) -> NDArray[np.float64]:
         rgba = self.native.opts["symbolBrush"].color().getRgb()
         return np.array(rgba) / 255
 
     @face_color.setter
     def face_color(self, value: str | Sequence):
         value = convert_color_code(value)
         self.native.setBrush(value)
@@ -323,25 +327,25 @@
         )
         pen = pg.mkPen(edge_color, width=lw, style=_LINE_STYLE[ls])
         brush = pg.mkBrush(face_color)
         self.native = pg.BarGraphItem(x=x, height=y, width=width, pen=pen, brush=brush)
         self.name = name
 
     @property
-    def edge_color(self) -> np.ndarray:
+    def edge_color(self) -> NDArray[np.float64]:
         rgba = self.native.opts["pen"].color().getRgb()
         return np.array(rgba) / 255
 
     @edge_color.setter
     def edge_color(self, value: str | Sequence):
         value = convert_color_code(value)
         self.native.setOpts(pen=pg.mkPen(value))
 
     @property
-    def face_color(self) -> np.ndarray:
+    def face_color(self) -> NDArray[np.float64]:
         rgba = self.native.opts["brush"].color().getRgb()
         return np.array(rgba) / 255
 
     @face_color.setter
     def face_color(self, value: str | Sequence):
         value = convert_color_code(value)
         self.native.setOpts(brush=pg.mkBrush(value))
@@ -400,15 +404,15 @@
 
     @intercept.setter
     def intercept(self, value: float):
         value = float(value)
         self.native.setPos((0, value))
 
     @property
-    def pos(self) -> np.ndarray:
+    def pos(self) -> NDArray[np.float64]:
         return np.array(self.native.getPos())
 
     @pos.setter
     def pos(self, value):
         self.native.setPos(value)
 
     @property
@@ -417,15 +421,15 @@
         return self.native.angle
 
     @angle.setter
     def angle(self, value: float):
         self.native.setAngle(value)
 
     @property
-    def edge_color(self) -> np.ndarray:
+    def edge_color(self) -> NDArray[np.float64]:
         return to_rgba(self.native.pen)
 
     @edge_color.setter
     def edge_color(self, value):
         value = convert_color_code(value)
         self.native.setPen(value, width=self.lw, style=self.ls)
 
@@ -484,25 +488,25 @@
         brush = pg.mkBrush(face_color)
         curve1 = pg.PlotCurveItem(x=x, y=y1, pen=pen)
         curve2 = pg.PlotCurveItem(x=x, y=y2, pen=pen)
         self.native = pg.FillBetweenItem(curve1, curve2, brush=brush, pen=pen)
         self.name = name
 
     @property
-    def edge_color(self) -> np.ndarray:
+    def edge_color(self) -> NDArray[np.float64]:
         rgba = self.native.curves[0].opts["pen"].color().getRgb()
         return np.array(rgba) / 255
 
     @edge_color.setter
     def edge_color(self, value: str | Sequence):
         value = convert_color_code(value)
         self.native.setPen(pg.mkPen(value))
 
     @property
-    def face_color(self) -> np.ndarray:
+    def face_color(self) -> NDArray[np.float64]:
         rgba = self.native.curves[0].opts["brush"].color().getRgb()
         return np.array(rgba) / 255
 
     @face_color.setter
     def face_color(self, value: str | Sequence):
         value = convert_color_code(value)
         self.native.setBrush(pg.mkBrush(value))
@@ -548,67 +552,72 @@
     def __init__(
         self,
         x: Sequence[float],
         y: Sequence[float],
         texts: Sequence[str],
         color=None,
         name: str = None,
+        size: int = 9,
+        anchor: tuple[float, float] = (0.0, 0.0),
     ):
         self.native = pg.ItemGroup()
         if color is None:
             color = "white"
         for x_, y_, text_ in zip(x, y, texts):
             item = pg.TextItem(text_, color=convert_color_code(color))
             item.setPos(x_, y_)
             self.native.addItem(item)
 
         self.name = name
+        self._font = QtGui.QFont()
+        self.size = size
+        self.anchor = anchor
 
     @property
     def text_items(self) -> list[pg.TextItem]:
         return self.native.childItems()
 
     def __getitem__(self, key: int | slice) -> TextItemView:
         return TextItemView(self.text_items[key])
 
     @property
-    def xdata(self) -> np.ndarray:
+    def xdata(self) -> NDArray[np.float64]:
         return np.array([item.pos().x() for item in self.text_items])
 
     @property
-    def ydata(self) -> np.ndarray:
+    def ydata(self) -> NDArray[np.float64]:
         return np.array([item.pos().y() for item in self.text_items])
 
     @property
-    def color(self) -> np.ndarray:
+    def color(self) -> NDArray[np.float64]:
         """Text color."""
         rgba = np.stack([item.color.getRgb() for item in self.text_items])
         return rgba / 255
 
     @color.setter
     def color(self, value):
         value = convert_color_code(value)
         for item in self.text_items:
             item.setText(item.toPlainText(), value)
 
     @property
-    def background_color(self) -> np.ndarray:
+    def background_color(self) -> NDArray[np.float64]:
         """Text background color."""
         return np.stack([to_rgba(item.fill) for item in self.text_items])
 
     @background_color.setter
     def background_color(self, value):
         value = convert_color_code(value)
         brush = pg.mkBrush(value)
         for item in self.text_items:
             item.fill = brush
             item._updateView()
 
     @property
-    def border(self) -> np.ndarray:
+    def border(self) -> NDArray[np.float64]:
         """Border color of text bounding box."""
         if isinstance(self.native, list):
             return np.stack([to_rgba(item.border) for item in self.native])
         else:
             return to_rgba(self.native.border)
 
     @border.setter
@@ -627,27 +636,38 @@
 
     @text.setter
     def text(self, value: str):
         for item in self.text_items:
             item.setText(value)
 
     @property
-    def anchor(self) -> np.ndarray:
-        """Text anchor position."""
+    def anchor(self) -> NDArray[np.float64]:
+        """Relative text anchor position."""
         out = []
         for item in self.text_items:
             anchor = item.anchor
             out.append([anchor.x(), anchor.y()])
         return np.array(out)
 
     @anchor.setter
     def anchor(self, value):
         for item in self.text_items:
             item.setAnchor(value)
 
+    @property
+    def size(self) -> float:
+        """Text point size."""
+        return self._font.pointSizeF()
+
+    @size.setter
+    def size(self, value: float):
+        self._font.setPointSizeF(value)
+        for item in self.text_items:
+            item.setFont(self._font)
+
 
 class TextItemView:
     def __init__(self, textitem: pg.TextItem | list[pg.TextItem]):
         self.native = textitem
 
     @property
     def color(self) -> np.ndarray:
@@ -716,15 +736,14 @@
         if isinstance(self.native, list):
             return [item.toPlainText() for item in self.native]
         else:
             return self.native.toPlainText()
 
     @text.setter
     def text(self, value: str):
-
         if isinstance(self.native, list):
             for item in self.native:
                 item.setText(value)
         else:
             self.native.setText(value)
 
     @property
@@ -745,14 +764,48 @@
         if isinstance(self.native, list):
             for item in self.native:
                 item.setAnchor(value)
         else:
             self.native.setAnchor(value)
 
 
+class Target(LayerItem):
+    native: pg.TargetItem
+
+    def __init__(
+        self,
+        pos,
+        size: int,
+        edge_color=None,
+        name: str | None = None,
+        lw: float = 1,
+        ls: str = "-",
+    ):
+        if edge_color is None:
+            edge_color = "yellow"
+        edge_color = convert_color_code(edge_color)
+        pen = pg.mkPen(edge_color, width=lw, style=_LINE_STYLE[ls])
+        self.native = pg.TargetItem(pos, size=size, pen=pen)
+        self.name = name
+
+    @property
+    def pos(self):
+        """Position in (x, y)"""
+        point = self.native.pos()
+        return point.x(), point.y()
+
+    @pos.setter
+    def pos(self, value):
+        self.native.setPos(value)
+
+    @property
+    def size(self):
+        return self.native.scale
+
+
 def _set_default_colors(face_color, edge_color, default_f, default_e):
     if face_color is None:
         face_color = default_f
     else:
         face_color = convert_color_code(face_color)
     if edge_color is None:
         edge_color = default_e
```

### Comparing `magic-class-0.6.9/magicclass/ext/pyqtgraph/mouse_event.py` & `magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/mouse_event.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,35 +3,37 @@
 from qtpy.QtCore import Qt
 from pyqtgraph.GraphicsScene.mouseEvents import MouseClickEvent as _MouseClickEvent
 from ._const import Modifier, Button
 
 
 def _factorize_modifiers(mod):
     out = []
-    if mod & Qt.ShiftModifier:
+    if mod & Qt.KeyboardModifier.ShiftModifier:
         out.append(Modifier.shift)
-    if mod & Qt.ControlModifier:
+    if mod & Qt.KeyboardModifier.ControlModifier:
         out.append(Modifier.control)
-    if mod & Qt.AltModifier:
+    if mod & Qt.KeyboardModifier.AltModifier:
         out.append(Modifier.alt)
     return tuple(out)
 
 
 def _factorize_buttons(mod):
     out = []
-    if mod & Qt.LeftButton:
+    if mod & Qt.MouseButton.LeftButton:
         out.append(Button.left)
-    if mod & Qt.RightButton:
+    if mod & Qt.MouseButton.RightButton:
         out.append(Button.right)
-    if mod & Qt.MiddleButton:
+    if mod & Qt.MouseButton.MiddleButton:
         out.append(Button.middle)
     return tuple(out)
 
 
 class MouseClickEvent(_MouseClickEvent):
+    """More pythonic way to access the button and modifiers"""
+
     def __init__(self, event: _MouseClickEvent, coord_item):
         self.accepted = event.accepted
         self.currentItem = (
             coord_item  # This enables mapping from event position to coordinates.
         )
         self._double = event._double
         self._scenePos = event._scenePos
@@ -53,7 +55,11 @@
     def modifiers(self):
         modifiers = super().modifiers()
         return _factorize_modifiers(modifiers)
 
     def buttons(self):
         buttons = super().buttons()
         return _factorize_buttons(buttons)
+
+    def __repr__(self):
+        cls = type(self).__name__
+        return f"{cls}(pos={self.pos()}, buttons={self.buttons()}, modifiers={self.modifiers()})"
```

### Comparing `magic-class-0.6.9/magicclass/ext/pyqtgraph/tests/test_qtgraph.py` & `magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/tests/test_qtgraph.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from magicclass import field, magicclass
 from magicclass.ext.pyqtgraph import QtPlotCanvas
 import numpy as np
 
-def test_plot_canvas():
-    @magicclass
-    class A:
-        plot = field(QtPlotCanvas)
+@magicclass
+class A:
+    plot = field(QtPlotCanvas)
 
+def test_curve():
     ui = A()
+    ui.show(run=False)
     ndata = 100
     data = np.random.random(ndata)
 
-    # test curve
     ui.plot.add_curve(data)
     ui.plot.add_curve(np.arange(ndata)*2, data)
     item = ui.plot.add_curve(data, face_color="green", edge_color="green", name="test", lw=2, ls=":")
     item.visible
     item.visible = False
     item.face_color
     item.face_color = "yellow"
@@ -30,17 +30,21 @@
     for sym in ["o", "s", "D", "^", "<", "v", ">", "*"]:
         item.symbol = sym
     item.xdata = item.xdata + 1
     item.ydata = item.ydata + 1
     assert item.ndata == ndata
 
     assert len(ui.plot.layers) == 3
-    ui.plot.layers.clear()
+    ui.close()
 
-    # test scatter
+def test_scatter():
+    ui = A()
+    ui.show(run=False)
+    ndata = 100
+    data = np.random.random(ndata)
     ui.plot.add_scatter(data)
     ui.plot.add_scatter(np.arange(ndata)*2, data)
     item = ui.plot.add_scatter(data, face_color="green", edge_color="green", name="test", lw=2, ls=":", size=6, symbol="*")
     item.visible
     item.visible = False
     item.face_color
     item.face_color = "yellow"
@@ -54,17 +58,21 @@
     for sym in ["o", "s", "D", "^", "<", "v", ">", "*"]:
         item.symbol = sym
     item.xdata = item.xdata + 1
     item.ydata = item.ydata + 1
     assert item.ndata == ndata
 
     assert len(ui.plot.layers) == 3
-    ui.plot.layers.clear()
+    ui.close()
 
-    # test bar
+def test_bar():
+    ui = A()
+    ui.show(run=False)
+    ndata = 100
+    data = np.random.random(ndata)
     ui.plot.add_bar(data)
     ui.plot.add_bar(np.arange(ndata)*2, data)
     item = ui.plot.add_bar(data, face_color="green", edge_color="green", name="test", lw=2, ls=":")
     item.visible
     item.visible = False
     item.face_color
     item.face_color = "yellow"
@@ -76,16 +84,21 @@
     for ls in ["-", "--", ":", "-."]:
         item.ls = ls
     item.xdata = item.xdata + 1
     item.ydata = item.ydata + 1
     assert item.ndata == ndata
 
     assert len(ui.plot.layers) == 3
-    ui.plot.layers.clear()
+    ui.close()
 
+def test_hist():
+    ui = A()
+    ui.show(run=False)
+    ndata = 100
+    data = np.random.random(ndata)
     ui.plot.add_hist(data)
     item = ui.plot.add_hist(data, bins=14, range=[-0.5, 1.5], density=True)
     item.visible
     item.visible = False
     item.face_color
     item.face_color = "yellow"
     item.edge_color
@@ -93,26 +106,38 @@
     item.lw
     item.lw = 1
     item.ls
     for ls in ["-", "--", ":", "-."]:
         item.ls = ls
 
     assert len(ui.plot.layers) == 2
+    ui.close()
+
+def test_infline():
+    ui = A()
+    ui.plot.add_infline(0.5, 0.3)  # slope/intercept
+    ui.plot.add_infline(0.5, intercept=0.3)  # slope/intercept
+    ui.plot.add_infline(slope=0.5, intercept=0.3)  # slope/intercept
+    ui.plot.add_infline((1, 1), 83)  # pos/degree
+    ui.plot.add_infline((1, 1), degree=83)  # pos/degree
+    ui.plot.add_infline(pos=(1, 1), degree=83)  # pos/degree
 
-    # test region
+def test_region():
+    ui = A()
     ui.plot.region.visible
     ui.plot.region.visible = True
     ui.plot.region.value
     ui.plot.region.value = [-1, 2]
     ui.plot.region.enabled
     ui.plot.region.enabled = True
     ui.plot.region.color
     ui.plot.region.color = "blue"
 
-    # test legend
+def test_legend():
+    ui = A()
     ui.plot.legend.visible
     ui.plot.legend.visible = True
     ui.plot.legend.color
     ui.plot.legend.color = "black"
     ui.plot.legend.size
     ui.plot.legend.size = 10
     ui.plot.legend.background_color
```

### Comparing `magic-class-0.6.9/magicclass/ext/pyqtgraph/widgets.py` & `magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/widgets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 from __future__ import annotations
+import warnings
 import pyqtgraph as pg
 from pyqtgraph import colormap as cmap
 from typing import Generic, Iterator, Sequence, TypeVar, overload, MutableSequence
 import numpy as np
 
-from .components import Legend, Region, ScaleBar, TextItem
+from .components import Grid, Legend, Region, ScaleBar, TextItem
 from .graph_items import (
     BarPlot,
     Curve,
     FillBetween,
     InfLine,
     LayerItem,
     Scatter,
     Histogram,
+    Target,
     TextGroup,
 )
 from .mouse_event import MouseClickEvent
-from .._shared_utils import convert_color_code, to_rgba
-from .._doc import write_docs
-from ...widgets.utils import FreeWidget
-from ..._app import get_app
+
+from psygnal import Signal, SignalInstance
+
+from magicclass.ext._shared_utils import convert_color_code, to_rgba
+from magicclass.ext._doc import write_docs
+from magicclass.widgets.utils import FreeWidget
+from magicclass._app import get_app
 
 BOTTOM = "bottom"
 LEFT = "left"
 
 
 class LayerList(MutableSequence[LayerItem]):
     """A napari-like layer list for plot item handling."""
@@ -51,23 +56,25 @@
 
     def __setitem__(self, key, value):
         raise NotImplementedError("Can't set item")
 
     def __delitem__(self, key: int | str):
         return self.parent._remove_item(key)
 
-    def append(self, item: LayerItem):
+    def append(self, item: LayerItem) -> None:
         if not isinstance(item, LayerItem):
             raise TypeError(f"Cannot append type {type(item)}.")
         self.parent._add_item(item)
+        return None
 
-    def insert(self, pos: int, item: LayerItem):
+    def insert(self, pos: int, item: LayerItem) -> None:
         if not isinstance(item, LayerItem):
             raise TypeError(f"Cannot insert type {type(item)}.")
         self.parent._insert_item(pos, item)
+        return None
 
     def __len__(self):
         return len(self.parent._items)
 
     def clear(self):
         for _ in range(len(self)):
             self.parent._remove_item(-1)
@@ -87,35 +94,27 @@
         """Target widget to add graphics items."""
         raise NotImplementedError()
 
     @property
     def layers(self) -> LayerList:
         return LayerList(self)
 
-    @overload
-    def add_curve(self, x: Sequence[float], **kwargs) -> Curve:
-        ...
-
-    @overload
-    def add_curve(self, x: Sequence[float], y: Sequence[float], **kwargs) -> Curve:
-        ...
-
     @write_docs
     def add_curve(
         self,
-        x=None,
-        y=None,
+        x: Sequence[float] | None = None,
+        y: Sequence[float] | None = None,
         face_color=None,
         edge_color=None,
         color=None,
         size: float = 7,
         name: str | None = None,
         lw: float = 1,
         ls: str = "-",
-        symbol=None,
+        symbol: str = None,
     ) -> Curve:
         """
         Add a line plot like ``plt.plot(x, y)``.
 
         Parameters
         ----------
         {x}{y}{face_color}{edge_color}{color}
@@ -141,27 +140,19 @@
             lw=lw,
             ls=ls,
             symbol=symbol,
         )
         self._add_item(item)
         return item
 
-    @overload
-    def add_scatter(self, x: Sequence[float], **kwargs) -> Scatter:
-        ...
-
-    @overload
-    def add_scatter(self, x: Sequence[float], y: Sequence[float], **kwargs) -> Scatter:
-        ...
-
     @write_docs
     def add_scatter(
         self,
-        x=None,
-        y=None,
+        x: Sequence[float] | None = None,
+        y: Sequence[float] | None = None,
         face_color=None,
         edge_color=None,
         color=None,
         size: float = 7,
         name: str | None = None,
         lw: float = 1,
         ls: str = "-",
@@ -246,27 +237,19 @@
             name=name,
             lw=lw,
             ls=ls,
         )
         self._add_item(item)
         return item
 
-    @overload
-    def add_bar(self, x: Sequence[float], **kwargs) -> BarPlot:
-        ...
-
-    @overload
-    def add_bar(self, x: Sequence[float], y: Sequence[float], **kwargs) -> BarPlot:
-        ...
-
     @write_docs
     def add_bar(
         self,
-        x=None,
-        y=None,
+        x: Sequence[float] | None = None,
+        y: Sequence[float] | None = None,
         width: float = 0.6,
         face_color=None,
         edge_color=None,
         color=None,
         name: str | None = None,
         lw: float = 1,
         ls: str = "-",
@@ -298,30 +281,20 @@
             name=name,
             lw=lw,
             ls=ls,
         )
         self._add_item(item)
         return item
 
-    @overload
-    def add_fillbetween(self, x: Sequence[float], **kwargs) -> FillBetween:
-        ...
-
-    @overload
-    def add_fillbetween(
-        self, x: Sequence[float], y: Sequence[float], **kwargs
-    ) -> FillBetween:
-        ...
-
     @write_docs
     def add_fillbetween(
         self,
-        x=None,
-        y1=None,
-        y2=None,
+        x: Sequence[float] | None = None,
+        y1: Sequence[float] | None = None,
+        y2: Sequence[float] | None = None,
         face_color=None,
         edge_color=None,
         color=None,
         name: str | None = None,
         lw: float = 1,
         ls: str = "-",
     ) -> FillBetween:
@@ -336,14 +309,15 @@
             face_color=face_color,
             edge_color=edge_color,
             name=name,
             lw=lw,
             ls=ls,
         )
         self._add_item(item)
+        return item
 
     @overload
     def add_infline(
         self,
         slope: float,
         intercept: float,
         color=None,
@@ -371,21 +345,32 @@
         color=None,
         name: str | None = None,
         lw: float = 1,
         ls: str = "-",
         **kwargs,
     ) -> InfLine:
         if kwargs:
-            if args:
-                raise TypeError(
-                    "Cannot mix args and kwargs for infinite line parameters."
+            if "angle" in kwargs:
+                # backward compatibility
+                warnings.warn(
+                    "`angle` keyword argument is deprecated. Please use `degree` instead."
                 )
+                kwargs["degree"] = kwargs.pop("angle")
+            if len(args) == 1:
+                if "degree" in kwargs:
+                    kwargs["pos"] = args[0]
+                elif "intercept" in kwargs:
+                    kwargs["slope"] = args[0]
+                else:
+                    raise ValueError(f"{args=}, {kwargs=} is invalid input.")
+            elif len(args) == 2:
+                raise ValueError(f"{args=}, {kwargs=} is invalid input.")
             keys = set(kwargs.keys())
-            if keys <= {"pos", "angle"}:
-                args = (kwargs.get("pos", (0, 0)), kwargs.get("angle", 0))
+            if keys <= {"pos", "degree"}:
+                args = (kwargs.get("pos", (0, 0)), kwargs.get("degree", 0))
             elif keys <= {"slope", "intercept"}:
                 args = (kwargs.get("slope", (0, 0)), kwargs.get("intercept", 0))
             else:
                 raise ValueError(f"{kwargs} is invalid input.")
 
         nargs = len(args)
         if nargs == 1:
@@ -408,32 +393,64 @@
             raise TypeError(
                 "Arguments of 'add_infline' should be either 'add_infline(slope, intercept)' "
                 "or 'add_infline(pos, degree)'."
             )
 
         item = InfLine(pos, angle, edge_color=color, name=name, lw=lw, ls=ls)
         self._add_item(item)
+        return item
 
     @overload
-    def add_text(self, x: float, y: float, text: str, **kwargs) -> TextGroup:
+    def add_text(
+        self,
+        x: float,
+        y: float,
+        text: str,
+        color=None,
+        name: str | None = None,
+        size: float = 9.0,
+        anchor: tuple[float, float] = (0.0, 0.0),
+    ) -> TextGroup:
         ...
 
     @overload
     def add_text(
-        self, x: Sequence[float], y: Sequence[float], text: Sequence[str], **kwargs
+        self,
+        x: Sequence[float],
+        y: Sequence[float],
+        text: Sequence[str],
+        color=None,
+        name: str | None = None,
+        size: float = 9.0,
+        anchor: tuple[float, float] = (0.0, 0.0),
     ) -> TextGroup:
         ...
 
-    def add_text(self, x, y, text, color=None, name=None) -> TextGroup:
+    def add_text(
+        self,
+        x,
+        y,
+        text,
+        color=None,
+        name=None,
+        size: int = 9,
+        anchor: tuple[float, float] = (0.0, 0.0),
+    ) -> TextGroup:
         if np.isscalar(x) and np.isscalar(y):
             x = [x]
             y = [y]
             text = [text]
-        item = TextGroup(x, y, text, color, name)
+        item = TextGroup(x, y, text, color, name, size=size, anchor=anchor)
         self._add_item(item)
+        return item
+
+    def add_target(self, pos, size: int = 10, color=None, name=None) -> Target:
+        item = Target(pos, size=size, edge_color=color, name=name)
+        self._add_item(item)
+        return item
 
     def _add_item(self, item: LayerItem):
         item.zorder = len(self._items)
         self._graphics.addItem(item.native)
         self._items.append(item)
 
     def _insert_item(self, pos: int, item: LayerItem):
@@ -485,21 +502,42 @@
         i = 0
         while name in existing_names:
             name = f"{prefix}-{i}"
             i += 1
         return name
 
 
+class SignalCompat:
+    def __init__(self, signal: SignalInstance, name: str):
+        self.signal = signal
+        self.name = name
+
+    def _warn(self):
+        warnings.warn(
+            f"Use of `{self.name}.append` is deprecated. Please use `{self.signal.name}.connect` instead.",
+            DeprecationWarning,
+        )
+
+    def append(self, slot):
+        self._warn()
+        self.signal.connect(slot)
+
+
 class HasViewBox(HasDataItems):
+    range_changed = Signal(object)
+    mouse_clicked = Signal(MouseClickEvent)
+
     def __init__(self, viewbox: pg.ViewBox):
         self._viewbox = viewbox
         self._items: list[LayerItem] = []
 
         # prepare mouse event
-        self.mouse_click_callbacks = []
+        self.mouse_click_callbacks = SignalCompat(
+            self.mouse_clicked, "mouse_click_callbacks"
+        )
 
         # This ROI is not editable. Mouse click event will use it to determine
         # the origin of the coordinate system.
         self._coordinate_fiducial = pg.ROI((0, 0))
         self._coordinate_fiducial.setVisible(False)
         self._viewbox.addItem(self._coordinate_fiducial, ignoreBounds=True)
 
@@ -510,16 +548,18 @@
         # Here plot items always have a linear region item as a default one,
         # we can use it as the referene.
         ev = MouseClickEvent(e, self._coordinate_fiducial)
         x, y = ev.pos()
         [xmin, xmax], [ymin, ymax] = self._viewbox.viewRange()
 
         if xmin <= x <= xmax and ymin <= y <= ymax:
-            for callback in self.mouse_click_callbacks:
-                callback(ev)
+            self.mouse_clicked.emit(ev)
+
+    def _range_changed(self):
+        self.range_changed.emit(self._viewbox.viewRange())
 
     @property
     def xlim(self):
         """Range limits of X-axis."""
         (xmin, xmax), _ = self._viewbox.viewRange()
         return xmin, xmax
 
@@ -557,14 +597,17 @@
         return to_rgba(self._viewbox.border)
 
     @border.setter
     def border(self, value):
         value = convert_color_code(value)
         self._viewbox.setBorder(value)
 
+    def auto_range(self):
+        self._viewbox.autoRange()
+
 
 class SimpleViewBox(HasViewBox):
     def __init__(self):
         super().__init__(pg.ViewBox())
 
     @property
     def _graphics(self):
@@ -637,18 +680,23 @@
         return self.pgitem.titleLabel.text
 
     @title.setter
     def title(self, value: str):
         value = str(value)
         self.pgitem.setTitle(value)
 
+    def show_grid(self, x: bool = True, y: bool = True, alpha: float | None = None):
+        """Show grid lines."""
+        self.pgitem.showGrid(x, y, alpha=alpha)
+
     def _update_scene(self):
         # Since plot item does not have graphics scene before being added to
         # a graphical layout, mouse event should be connected afterward.
         self.pgitem.scene().sigMouseClicked.connect(self._mouse_clicked)
+        self.pgitem.sigRangeChanged.connect(self._range_changed)
 
 
 class ViewBoxExt(pg.ViewBox):
     def __init__(
         self,
         parent=None,
         border=None,
@@ -734,14 +782,15 @@
 
         self._cmap = "gray"
 
     def _update_scene(self):
         # Since plot item does not have graphics scene before being added to
         # a graphical layout, mouse event should be connected afterward.
         self._image_item.scene().sigMouseClicked.connect(self._mouse_clicked)
+        self._viewbox.sigRangeChanged.connect(self._range_changed)
 
     @property
     def text_overlay(self) -> TextItem:
         """Text overlay on the image."""
         return self._text_overlay
 
     @property
```

### Comparing `magic-class-0.6.9/magicclass/ext/qtconsole/__init__.py` & `magic_class-0.7.0rc0/magicclass/ext/qtconsole/__init__.py`

 * *Files identical despite different names*

### Comparing `magic-class-0.6.9/magicclass/ext/qtconsole/_qt.py` & `magic_class-0.7.0rc0/magicclass/ext/qtconsole/_qt.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 from qtconsole.rich_jupyter_widget import RichJupyterWidget
 
 # See napari_console
 # https://github.com/napari/napari-console
 class _Console(RichJupyterWidget):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        self._connected = False
 
     def connect_parent(self, ui: Widget):
         from IPython import get_ipython
         from IPython.terminal.interactiveshell import TerminalInteractiveShell
         from ipykernel.connect import get_connection_file
         from ipykernel.inprocess.ipkernel import InProcessInteractiveShell
         from ipykernel.zmqshell import ZMQInteractiveShell
         from qtconsole.client import QtKernelClient
         from qtconsole.inprocess import QtInProcessKernelManager
 
+        if self._connected:
+            return
         if not isinstance(ui, Widget):
             raise TypeError(f"Cannot connect QtConsole to {type(ui)}.")
 
         shell = get_ipython()
 
         if shell is None:
             # If there is no currently running instance create an in-process
@@ -32,26 +35,28 @@
             kernel_client = kernel_manager.client()
             kernel_client.start_channels()
 
             self.kernel_manager = kernel_manager
             self.kernel_client = kernel_client
             self.shell = kernel_manager.kernel.shell
             self.push = self.shell.push
+            self._connected = True
         elif type(shell) == InProcessInteractiveShell:
             # If there is an existing running InProcessInteractiveShell
             # it is likely because multiple viewers have been launched from
             # the same process. In that case create a new kernel.
             # Connect existing kernel
             kernel_manager = QtInProcessKernelManager(kernel=shell.kernel)
             kernel_client = kernel_manager.client()
 
             self.kernel_manager = kernel_manager
             self.kernel_client = kernel_client
             self.shell = kernel_manager.kernel.shell
             self.push = self.shell.push
+            self._connected = True
         elif isinstance(shell, TerminalInteractiveShell):
             # if launching from an ipython terminal then adding a console is
             # not supported. Instead users should use the ipython terminal for
             # the same functionality.
             self.kernel_client = None
             self.kernel_manager = None
             self.shell = None
@@ -64,12 +69,13 @@
             kernel_client.load_connection_file()
             kernel_client.start_channels()
 
             self.kernel_manager = None
             self.kernel_client = kernel_client
             self.shell = shell
             self.push = self.shell.push
+            self._connected = True
         else:
             raise ValueError("ipython shell not recognized; " f"got {type(shell)}")
 
         self.parent_ui = ui
         self.shell.push({"ui": ui})
```

### Comparing `magic-class-0.6.9/magicclass/ext/qtconsole/widgets.py` & `magic_class-0.7.0rc0/magicclass/ext/qtconsole/widgets.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,7 +43,12 @@
         cursor.insertText(lines[-1])
 
     def execute(self):
         """Execute current code block."""
         code = self.value
         self.console.execute()
         self.executed.emit(code)
+
+    def update_console(self, namespace: dict = {}, **kwargs):
+        """Update console namespace"""
+        kwargs = dict(namespace, **kwargs)
+        self.console.push(kwargs)
```

### Comparing `magic-class-0.6.9/magicclass/ext/vispy/_base.py` & `magic_class-0.7.0rc0/magicclass/ext/vispy/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,50 +4,58 @@
 from typing import TYPE_CHECKING, Callable
 import weakref
 
 from vispy import scene
 from vispy.scene import ViewBox, transforms
 from vispy.app import MouseEvent
 
-from ...widgets import FreeWidget
-from ..._app import get_app
+from magicclass.widgets import FreeWidget
+from magicclass._app import get_app
 
 
 if TYPE_CHECKING:
     from vispy.visuals import Visual
 
 
 class LayerItem:
     _visual: Visual
-    name: str
+    _name: str
 
     def __repr__(self) -> str:
         return f"<{type(self).__name__} {self.name}>"
 
     @property
     def visible(self) -> bool:
         """Layer visibility."""
         return self._visual.visible
 
     @visible.setter
     def visible(self, v: bool) -> None:
+        """Set layer visibility."""
         self._visual.visible = v
 
     def _get_transform(self) -> transforms.MatrixTransform:
         return self._visual.transform
 
     def affine_transform(self, mtx: np.ndarray):
         """Apply affine transformation to the layer."""
         self._visual.transform = transforms.MatrixTransform(mtx)
 
     @property
     def translate(self) -> np.ndarray:
         mtx = self._get_transform().matrix
         return mtx[:3, 4]
 
+    def _get_bbox(self) -> tuple[np.ndarray, np.ndarray]:
+        raise NotImplementedError
+
+    @property
+    def name(self) -> str:
+        return self._name
+
 
 class HasViewBox:
     """The base class for all the vispy based visual objects."""
 
     def __init__(self, viewbox: ViewBox):
         from .layerlist import LayerList
```

### Comparing `magic-class-0.6.9/magicclass/ext/vispy/layer2d.py` & `magic_class-0.7.0rc0/magicclass/ext/vtk/volume.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,212 +1,160 @@
 from __future__ import annotations
 from typing import Sequence
+import vtk
+import vedo
+from vedo.utils import numpy2vtk
 import numpy as np
-from numpy.typing import ArrayLike
-from vispy.scene import visuals, ViewBox
-from vispy.color import get_color_dict
-from ._base import LayerItem
-from .._shared_utils import convert_color_code, to_rgba
-
-
-_SYMBOL_MAP = {
-    "s": "square",
-    "D": "diamond",
-}
-
-
-class PlotDataLayer(LayerItem):
-    _visual: visuals.LinePlot | visuals.Markers
-    _data: np.ndarray
+from magicgui.widgets import FloatSlider
 
-    @property
-    def xdata(self) -> np.ndarray:
-        return self._data[:, 0]
-
-    @xdata.setter
-    def xdata(self, value: Sequence[float]):
-        x = np.atleast_2d(value)
-        y = self._data[:, 1]
-        self._visual.set_data(np.concatenate([x, y], axis=1))
-
-    @property
-    def ydata(self) -> np.ndarray:
-        return self._data[:, 1]
-
-    @ydata.setter
-    def ydata(self, value: Sequence[float]):
-        x = self._data[:, 0]
-        y = np.atleast_2d(value)
-        self._visual.set_data(np.concatenate([x, y], axis=1))
-
-    @property
-    def ndata(self) -> int:
-        return self.xdata.size
-
-    @property
-    def name(self) -> str:
-        return self._name
-
-    @name.setter
-    def name(self, value: str):
-        self._name = str(value)
-
-    def add(self, points: np.ndarray | Sequence):
-        """Add new points to the plot data item."""
-        points = np.atleast_2d(points)
-        if points.shape[1] != 2:
-            raise ValueError("Points must be of the shape (N, 2).")
-        data = np.concatenate([self._data, points], axis=1)
-        self._visual.set_data(data)
-        return None
+from .components import VtkComponent
+from .const import Mode, Rendering
 
-    def remove(self, i: int | Sequence[int]):
-        """Remove the i-th data."""
-        if isinstance(i, int):
-            i = [i]
-        sl = list(set(range(self.ndata)) - set(i))
-        x = self.xdata[sl]
-        y = self.ydata[sl]
-        self._visual.set_data(np.concatenate([x, y], axis=1))
-        return None
-
-    @property
-    def edge_color(self) -> np.ndarray:
-        """Edge color of the data."""
-        col = self._visual._line.color
-        return to_rgba(col)
-
-    @edge_color.setter
-    def edge_color(self, value: str | Sequence):
-        value = convert_color_code(value)
-        self._visual.set_data(edge_color=value)
-
-    @property
-    def face_color(self) -> np.ndarray:
-        """Face color of the data."""
-        col = self._visual._markers._data["face_color"]
-        return to_rgba(col)
-
-    @face_color.setter
-    def face_color(self, value: str | Sequence):
-        value = convert_color_code(value)
-        self._visual.set_data(face_color=value)
-
-    color = property()
-
-    @color.setter
-    def color(self, value: str | Sequence):
-        """Set face color and edge color at the same time."""
-        self.face_color = value
-        self.edge_color = value
-
-
-class Curve(PlotDataLayer):
-    def __init__(
-        self,
-        viewbox: ViewBox,
-        x: ArrayLike,
-        y: ArrayLike = None,
-        face_color=None,
-        edge_color=None,
-        size: float = 7,
-        name: str | None = None,
-        lw: float = 1,
-        ls: str = "-",  # not implemented yet
-        symbol=None,
-    ) -> None:
-        symbol = _SYMBOL_MAP.get(symbol, symbol)
-        if symbol is None:
-            face_color = None
-        self._viewbox = viewbox
-        self._visual = visuals.LinePlot(
-            np.stack([x, y], axis=1),
-            color=edge_color,
-            symbol=symbol,
-            parent=self._viewbox.scene,
-            width=lw,
-            marker_size=size,
-            face_color=face_color,
-            edge_color=face_color,
-        )
-        self._name = name
-        self._visual.update()
-
-
-class Scatter(PlotDataLayer):
-    def __init__(
-        self,
-        viewbox: ViewBox,
-        x: ArrayLike,
-        y: ArrayLike = None,
-        face_color=None,
-        edge_color=None,
-        size: float = 7,
-        name: str | None = None,
-        symbol="o",
-    ) -> None:
-        symbol = _SYMBOL_MAP.get(symbol, symbol)
-        self._viewbox = viewbox
-        self._visual = visuals.Markers(
-            pos=np.stack([x, y], axis=1),
-            symbol=symbol,
-            parent=self._viewbox.scene,
-            size=size,
-            face_color=face_color,
-            edge_color=edge_color,
-        )
-        self._name = name
-        self._visual.update()
-
-
-class Histogram(LayerItem):
-    def __init__(
-        self,
-        viewbox: ViewBox,
-        data: np.ndarray,
-        bins: int = 10,
-        face_color=None,
-        edge_color=None,
-        name: str | None = None,
-    ) -> None:
-        self._viewbox = viewbox
-        self._visual = visuals.Histogram(
-            data,
-            bins=bins,
-            # color=edge_color,
-            parent=self._viewbox.scene,
-        )
-
-        if isinstance(face_color, str):
-            rgb_html = get_color_dict()[face_color][1:]
-            face_color = np.array(
-                [
-                    int(rgb_html[0:2], 16) / 255,
-                    int(rgb_html[2:4], 16) / 255,
-                    int(rgb_html[4:6], 16) / 255,
-                ]
+from magicclass.fields import vfield
+from magicclass.widgets import FloatRangeSlider
+from magicclass.types import Color
+
+
+def split_rgba(col: str | Sequence[float]) -> tuple[str | Sequence[float], float]:
+    if not isinstance(col, str):
+        if len(col) == 3:
+            rgb, alpha = col, 255
+        else:
+            rgb, alpha = col[:3], col[3]
+    elif col.startswith("#"):
+        l = len(col)
+        if l == 9:
+            rgb = int(col[1:7], base=16) / 255
+            alpha = int(col[7:], base=16) / 255
+        elif l == 7:
+            rgb = int(col[1:7], base=16) / 255
+            alpha = 1.0
+        else:
+            raise ValueError(f"Informal color code: {col}.")
+    else:
+        rgb, alpha = col, 255
+    return [int(c * 255) for c in rgb], alpha * 255
+
+
+class Volume(VtkComponent, base=vedo.Volume):
+    _obj: vedo.Volume
+
+    def __init__(self, data, _parent):
+        super().__init__(data, _parent=_parent, _emit=False)
+        self._current_obj = self._obj
+        self.rendering = Rendering.composite
+        self.mode = Mode.volume
+        self.color = np.array([0.7, 0.7, 0.7])
+        self.data = data
+        self.contrast_limits = self._lims
+        self.iso_threshold = np.mean(self._lims)
+        self.widgets.emit_all()
+
+    @property
+    def data(self) -> np.ndarray:
+        return self._data
+
+    @data.setter
+    def data(self, v):
+        self._data = np.asarray(v)
+        self._cache_lims()
+        vimg = vtk.vtkImageData()
+        varr = numpy2vtk(self._data.ravel(order="F"), dtype=float)
+        varr.SetName("input_scalars")
+        vimg.SetDimensions(self._data.shape)
+        vimg.GetPointData().AddArray(varr)
+        vimg.GetPointData().SetActiveScalars(varr.GetName())
+        self._obj._update(vimg)
+        self._update_actor()
+
+    def _cache_lims(self):
+        self._lims = self._data.min(), self._data.max()
+        self.widgets.contrast_limits.min = self._lims[0]
+        self.widgets.contrast_limits.max = self._lims[1]
+        self.widgets.iso_threshold.min = self._lims[0]
+        self.widgets.iso_threshold.max = self._lims[1]
+
+    color = vfield(Color)
+    mode = vfield(Mode.volume)
+    rendering = vfield(Rendering.mip)
+    iso_threshold = vfield(float, widget_type=FloatSlider)
+    contrast_limits = vfield(tuple[float, float], widget_type=FloatRangeSlider)
+    visible = vfield(True, name="visibility")
+
+    @visible.connect
+    def _on_visible_change(self, v: bool):
+        if v:
+            self._current_obj.on()
+        else:
+            self._current_obj.off()
+        self._update()
+
+    @color.connect
+    def _on_color_change(self, col):
+        rgb, alpha = split_rgba(col)
+        vmin, vmax = self.contrast_limits
+        self._obj.color(rgb, vmin=vmin, vmax=vmax)
+        self._obj.alpha([0, alpha])
+        self._update_cmap()
+
+    @rendering.connect
+    def _on_rendering_change(self, v: Rendering):
+        self._obj.mode(v.value)
+        self._update_cmap()
+
+    @iso_threshold.connect
+    def _on_iso_threshold_change(self, v):
+        if self.mode in (Mode.iso, Mode.wireframe):
+            self._update_actor()
+
+    @mode.connect
+    def _on_mode_change(self, v):
+        self._update_actor()
+
+    @contrast_limits.connect
+    def _on_contrast_limits_change(self, v):
+        self._update_cmap()
+
+    def _update_cmap(self):
+        vmin, vmax = self.contrast_limits
+        rgb, alpha = split_rgba(self.color)
+        if self.mode == Mode.volume:
+            self._current_obj.color(
+                [[0, 0, 0], rgb],
+                alpha=[0, alpha],
+                vmin=vmin,
+                vmax=vmax,
             )
-
-        if isinstance(edge_color, str):
-            rgb_html = get_color_dict()[edge_color][1:]
-            edge_color = np.array(
-                [
-                    int(rgb_html[0:2], 16) / 255,
-                    int(rgb_html[2:4], 16) / 255,
-                    int(rgb_html[4:6], 16) / 255,
-                ]
+        else:
+            self._current_obj.color(
+                rgb,
+                alpha=alpha,
             )
+        self._update()
 
-        self._visual.mesh_data.set_face_colors(
-            np.stack([face_color] * self._visual.mesh_data.n_faces, axis=0)
-        )
-        self._visual.mesh_data.set_vertex_colors(
-            np.stack([edge_color] * self._visual.mesh_data.n_vertices, axis=0)
-        )
-        self._visual.mesh_data_changed()
-
-        self._name = name
-        self._visual.update()
-
-    @property
-    def name(self):
-        return self._name
+    def _update_actor(self):
+        vmin, vmax = self.contrast_limits
+        rgb, alpha = split_rgba(self.color)
+        if self.mode == Mode.volume:
+            actor = self._obj
+        elif self.mode == Mode.mesh:
+            actor = self._obj.tomesh()
+        elif self.mode == Mode.iso:
+            actor = self._obj.isosurface(value=self.iso_threshold)
+        elif self.mode == Mode.wireframe:
+            actor = (
+                self._obj.isosurface(value=self.iso_threshold)
+                .color(rgb, alpha=alpha)
+                .wireframe()
+            )
+        elif self.mode == Mode.lego:
+            actor = self._obj.legosurface(vmin=vmin, vmax=vmax)
+        else:
+            raise RuntimeError()
+
+        plotter = self._parent_ref()
+        plotter.remove(self._current_obj)
+        plotter.add(actor)
+        plotter.qt_widget.Render()
+        self._current_obj = actor
+        self._update_cmap()
+        return None
```

### Comparing `magic-class-0.6.9/magicclass/ext/vispy/layer3d.py` & `magic_class-0.7.0rc0/magicclass/fields/_property.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,387 +1,325 @@
 from __future__ import annotations
-from typing import Tuple
-import numpy as np
-from vispy.scene import visuals, ViewBox
-from vispy.visuals import (
-    VolumeVisual,
-    ImageVisual,
-    IsosurfaceVisual,
-    MeshVisual,
-)
-from vispy.visuals.filters import WireframeFilter
-from ._base import LayerItem
-
-from magicgui.widgets import FloatSlider
-from ...widgets import FloatRangeSlider
-from ...fields import HasFields, vfield
-from ...types import Color
-
-
-class Image(LayerItem, HasFields):
-    RENDERINGS = [
-        "translucent",
-        "mip",
-        "minip",
-        "attenuated_mip",
-        "additive",
-        "iso",
-        "average",
-    ]
-    INTERPOLATIONS = ["nearest", "linear"]
 
-    def __init__(
-        self,
-        data,
-        viewbox: ViewBox,
-        contrast_limits: tuple[float, float] | None = None,
-        rendering: str = "mip",
-        iso_threshold: float | None = None,
-        name: str = "",
-        attenuation: float = 1.0,
-        cmap: str = "grays",
-        gamma: str = 1.0,
-        interpolation: str = "linear",
-    ):
-        self._data = data
-        self._cache_lims()
+from typing import Generic, TypeVar, Callable, Any
+import inspect
+from psygnal import debounced, Signal
+from magicgui.signature import magic_signature
+from magicgui.widgets import create_widget, Container, PushButton
+from magicgui.widgets.bases import ValueWidget
+from magicclass.signature import split_annotated_type
+from ._fields import MagicField
+from ._define import define_callback
+
+_V = TypeVar("_V")
 
-        if contrast_limits is None:
-            contrast_limits = np.min(self._data), np.max(self._data)
-        if iso_threshold is None:
-            iso_threshold = np.mean(contrast_limits)
-
-        self._viewbox = viewbox
-        self._create_visual(
-            self._data,
-            clim=contrast_limits,
-            cmap=cmap,
-            rendering=rendering,
-            iso_threshold=iso_threshold,
-            attenuation=attenuation,
-            gamma=gamma,
-            interpolation=interpolation,
-        )
 
-        self._name = name
+class _ButtonedWidget(Container):
+    """A widget wrapper that adds a button to set the value."""
 
-        self.contrast_limits = contrast_limits
-        self.rendering = rendering
-        self.iso_threshold = iso_threshold
-        self.attenuation = attenuation
-        self._cmap = cmap
-        self.gamma = gamma
-        self.interpolation = interpolation
+    restoring = Signal()
 
-    def _create_visual(
+    def __init__(
         self,
-        data: np.ndarray,
-        clim: tuple[float, float],
-        cmap: str,
-        rendering: str,
-        iso_threshold: float,
-        attenuation: float,
-        gamma: float,
-        interpolation: str | None = None,
+        widget: ValueWidget,
+        layout: str = "horizontal",
+        call_button: str | bool | None = None,
+        auto_call: bool = False,
+        **kwargs,
     ):
-        if data.ndim == 2:
-            if interpolation is None:
-                interpolation = "nearest"
-            self._visual: ImageVisual = visuals.Image(
-                data,
-                clim=clim,
-                method="auto",
-                cmap=cmap,
-                gamma=gamma,
-                interpolation=interpolation,
-                parent=self._viewbox.scene,
-            )
+        if not hasattr(widget, "value"):
+            raise TypeError("widget must have a value attribute")
+        self._child_widget = widget
+
+        widgets = [widget]
+        if call_button is None:
+            call_button = not auto_call
+
+        self._call_button: PushButton | None = None
+        if call_button:
+            text = call_button if isinstance(call_button, str) else "Set"
+            self._call_button = PushButton(gui_only=True, text=text, name="call_button")
+            widgets.append(self._call_button)
+
+        super().__init__(layout=layout, widgets=widgets, labels=False, **kwargs)
+        self.margins = (0, 0, 0, 0)
+        # disconnect the existing signals
+        widget.changed.disconnect()
+        if self._call_button is not None:
+            self._call_button.changed.disconnect()
+            self._call_button.changed.connect(self._button_clicked)
+        self._auto_call = auto_call
+        self._inner_value = widget.value
 
-        elif data.ndim == 3:
-            if interpolation is None:
-                interpolation = "linear"
-            self._visual: VolumeVisual = visuals.Volume(
-                data,
-                clim=clim,
-                method=rendering,
-                threshold=iso_threshold,
-                attenuation=attenuation,
-                cmap=cmap,
-                gamma=gamma,
-                interpolation=interpolation,
-                parent=self._viewbox.scene,
-            )
+        if auto_call:
+            widget.changed.connect(self.set_value)
         else:
-            raise ValueError("Only 2D and 3D images are supported.")
 
-    @property
-    def data(self) -> np.ndarray:
-        return self._data
+            @self.restoring.connect
+            def _restore():
+                with widget.changed.blocked():
+                    self.widget.value = self._inner_value
+                return None
+
+            widget.changed.connect(self._create_debounced())
+
+    @classmethod
+    def from_options(
+        cls: type[_ButtonedWidget],
+        annotation: type,
+        layout: str = "horizontal",
+        widget_type: type | None = None,
+        options: dict | None = None,
+        call_button: str | bool | None = None,
+        auto_call=False,
+        **kwargs,
+    ):
+        """Construct a ButtonedWidget in a ``create_widget`` format."""
+        widget = create_widget(
+            annotation=annotation,
+            widget_type=widget_type,
+            options=options,
+        )
+        return cls(widget, layout, call_button, auto_call, **kwargs)
 
-    @data.setter
-    def data(self, value) -> None:
-        value = np.asarray(value)
-        if self._visual is None or value.ndim != self._data.ndim:
-            self._visual.parent = None
-            del self._visual
-            self._create_visual(value, None)
-        else:
-            self._visual.set_data(value)
-        self._data = value
-        self._cache_lims()
-        self._visual.update()
+    def __repr__(self) -> str:
+        return f"{type(self).__name__}({self.widget!r})"
 
     @property
-    def name(self) -> str:
-        return self._name
-
-    def _cache_lims(self):
-        self._lims = np.min(self._data), np.max(self._data)
-        self.widgets.contrast_limits.min = self._lims[0]
-        self.widgets.contrast_limits.max = self._lims[1]
-        self.widgets.iso_threshold.min = self._lims[0]
-        self.widgets.iso_threshold.max = self._lims[1]
-
-    # fmt: off
-    rendering = vfield(str, options={"choices": RENDERINGS, "value": "mip"})
-    contrast_limits = vfield(Tuple[float, float], widget_type=FloatRangeSlider)
-    iso_threshold = vfield(float, widget_type=FloatSlider)
-    gamma = vfield(float, widget_type=FloatSlider, options={"min": 0., "max": 1.})
-    attenuation = vfield(float, widget_type=FloatSlider, options={"min": 0., "max": 1.})
-    interpolation = vfield(str, options={"choices": INTERPOLATIONS})
-    # fmt: on
-
-    @contrast_limits.connect
-    def _on_constrast_limits_change(self, value):
-        if hasattr(self, "_visual"):
-            self._visual.clim = value
-            self._visual.update()
-
-    @rendering.connect
-    def _on_rendering_change(self, value):
-        self._visual.method = value
-        self._visual.update()
-
-    @iso_threshold.connect
-    def _on_iso_threshold_change(self, value):
-        if hasattr(self, "_visual"):
-            self._visual.threshold = max(value, self._lims[0] + 1e-6)
-            self._visual.update()
-
-    @gamma.connect
-    def _on_gamma_change(self, value):
-        self._visual.gamma = value
-        self._visual.update()
-
-    @attenuation.connect
-    def _on_attenuation_change(self, value):
-        self._visual.attenuation = value
-        self._visual.update()
-
-    @interpolation.connect
-    def _on_interpolation_change(self, value):
-        self._visual.interpolation = value
-        self._visual.update()
-
-
-class _SurfaceBase(LayerItem):
-    _visual: visuals.Mesh | visuals.Isosurface
-    _wireframe: WireframeFilter
+    def value(self) -> Any:
+        """The value that has been set (not the widget)."""
+        return self._inner_value
+
+    @value.setter
+    def value(self, value: Any) -> None:
+        return self.set_value(value)
+
+    def set_value(self, value: Any) -> None:
+        """Method version of setting the value."""
+        self.widget.value = value
+        self._inner_value = self.widget.value
+        self.changed.emit(self._inner_value)
+        return None
 
-    def __init__(
-        self,
-        data,
-        viewbox: ViewBox,
-        face_color=None,
-        edge_color=None,
-        shading="none",
-        name: str = "",
-        **kwargs,
-    ):
-        self._viewbox = viewbox
-        self._create_visual(data, **kwargs)
-        self._wireframe = WireframeFilter()
-        self._visual.attach(self._wireframe)
-        self._data = data
-
-        if edge_color is None:
-            edge_color = [0.7, 0.7, 0.7, 1.0]
-        self.edge_color = edge_color
-
-        if face_color is None:
-            face_color = [0.7, 0.7, 0.7, 1.0]
-        self.face_color = face_color
+    def _button_clicked(self):
+        self._inner_value = self.widget.value
+        self.changed.emit(self._inner_value)
+        return None
 
-        self.shading = shading
-        self._name = name
+    @property
+    def widget(self) -> ValueWidget:
+        """The central child widget."""
+        return self._child_widget
 
     @property
-    def name(self) -> str:
-        return self._name
+    def call_button(self) -> PushButton | None:
+        """The call button widget."""
+        return self._call_button
 
-    def _create_visual(self, data):
-        raise NotImplementedError()
+    def _create_debounced(self):
+        @debounced(timeout=1000)
+        def _reset_value(val):
+            if self.widget.native.hasFocus():
+                _reset_value(val)
+            else:
+                self.restoring.emit()
 
-    def _on_face_color_change(self, color):
-        self._visual.color = color
+        return lambda v: _reset_value(v)
 
-    def _on_edge_color_change(self, color):
-        self._wireframe.color = color
-        self._visual.update()
 
-    color = property(fget=None)
+class magicproperty(MagicField[_ButtonedWidget], Generic[_V]):
+    """
+    A property-like descriptor that returns a field for magicgui widgets.
 
-    @color.setter
-    def color(self, color):
-        self.face_color = color
-        self.edge_color = color
+    For instance, the following code
 
-    def _on_edge_width_change(self, value):
-        self._wireframe.width = value
-        self._visual.update()
+    >>> @magicproperty
+    >>> def x(self):
+    >>>     return self._x
 
-    def _on_shading_change(self, v):
-        if v == "none":
-            v = None
-        self._visual._shading = v
+    >>> @x.setter
+    >>> def x(self, val: int):
+    >>>     self._x = val
 
+    will create a magicgui widget with a button "Set".
+    """
 
-class IsoSurface(_SurfaceBase, HasFields):
     def __init__(
         self,
-        data,
-        viewbox: ViewBox,
-        contrast_limits=None,
-        iso_threshold=None,
-        face_color=None,
-        edge_color=None,
-        shading="smooth",
+        fget: Callable[[Any], _V] | None = None,
+        fset: Callable[[Any, _V], None] | None = None,
+        fdel: Callable[[Any], None] | None = None,
+        *,
         name: str | None = None,
-    ):
-        data = np.asarray(data)
-        data = data.transpose(list(range(data.ndim))[::-1])
-
-        if contrast_limits is None:
-            contrast_limits = np.min(data), np.max(data)
-
-        if iso_threshold is None:
-            iso_threshold = np.mean(contrast_limits)
+        label: str | None = None,
+        annotation: Any = None,
+        widget_type: type | str | None = None,
+        auto_call: bool = False,
+        layout: str = "horizontal",
+        call_button: bool | str | None = None,
+        options: dict[str, Any] | None = None,
+        record: bool = True,
+    ) -> None:
+        def _create_buttoned_gui(obj):
+            return _ButtonedWidget.from_options(
+                annotation=self.annotation,
+                layout=layout,
+                widget_type=self.widget_type,
+                options=self.options,
+                call_button=call_button,
+                auto_call=auto_call,
+                name=self.name,
+            )
 
         super().__init__(
-            data,
-            viewbox=viewbox,
-            face_color=face_color,
-            edge_color=edge_color,
-            shading=shading,
-            iso_threshold=iso_threshold,
             name=name,
+            label=label,
+            annotation=annotation,
+            widget_type=widget_type,
+            options=options,
+            record=record,
+            constructor=_create_buttoned_gui,
         )
-        self._cache_lims()
 
-        self.contrast_limits = contrast_limits
-        self.iso_threshold = iso_threshold
+        self._fget = self._default_fget
+        self._fset = self._default_fset
 
-    def _create_visual(self, data, iso_threshold):
-        self._visual: IsosurfaceVisual = visuals.Isosurface(
-            data, level=iso_threshold, parent=self._viewbox.scene
-        )
-        return None
-
-    def _cache_lims(self):
-        self._lims = np.min(self._data), np.max(self._data)
-        self.widgets.contrast_limits.min = self._lims[0]
-        self.widgets.contrast_limits.max = self._lims[1]
-        self.widgets.iso_threshold.min = self._lims[0]
-        self.widgets.iso_threshold.max = self._lims[1]
-
-    @property
-    def data(self) -> np.ndarray:
-        return self._data
+        if fget:
+            self.getter(fget)
+        if fset:
+            self.setter(fset)
+        if fdel:
+            self.deleter(fdel)
+
+    @classmethod
+    def from_setter(
+        cls: type[magicproperty],
+        fset: Callable[[Any, _V], None] = None,
+        *,
+        name: str | None = None,
+        label: str | None = None,
+        annotation: Any = None,
+        widget_type: type | str | None = None,
+        auto_call: bool = False,
+        layout: str = "horizontal",
+        call_button: bool | str | None = None,
+        options: dict[str, Any] | None = None,
+        record: bool = True,
+    ) -> magicproperty[_V]:
+        """
+        Directly create a magicproperty from a setter function.
+
+        Example
+        -------
+        >>> @magicproperty.from_setter
+        >>> def x(self, val: int):
+        ...     print(f"setting x to {val}")
+
+        >>> @magicproperty.from_setter(label="X")
+        >>> def x(self, val: int):
+        ...     print(f"setting x to {val}")
+
+        """
+
+        def _wrapper(fset):
+            return cls(
+                fset=fset,
+                name=name,
+                label=label,
+                annotation=annotation,
+                widget_type=widget_type,
+                auto_call=auto_call,
+                layout=layout,
+                call_button=call_button,
+                options=options,
+                record=record,
+            )
 
-    @data.setter
-    def data(self, value) -> None:
-        value = np.asarray(value)
-        self._visual.set_data(value)
-        self._data = value
-        self._visual.update()
-        self._cache_lims()
-
-    # fmt: off
-    contrast_limits = vfield(Tuple[float, float], widget_type=FloatRangeSlider)
-    shading = vfield(str, options={"choices": ["none", "float", "smooth"], "value": "smooth"})
-    iso_threshold = vfield(float, widget_type=FloatSlider)
-    face_color = vfield(Color)
-    edge_color = vfield(Color)
-    edge_width = vfield(float, widget_type=FloatSlider, options={"min": 0.5, "max": 10.0, "value": 1.0})
-    # fmt: on
-
-    @contrast_limits.connect
-    def _on_contrast_limits_change(self, value):
-        self._visual.clim = value
-        self._visual.update()
-
-    @iso_threshold.connect
-    def _on_iso_threshold_change(self, value):
-        self._visual.level = max(self.iso_threshold, self._lims[0] + 1e-6)
-        self._visual.update()
-
-    shading.connect(_SurfaceBase._on_shading_change)
-    face_color.connect(_SurfaceBase._on_face_color_change)
-    edge_color.connect(_SurfaceBase._on_edge_color_change)
-    edge_width.connect(_SurfaceBase._on_edge_width_change)
+        return _wrapper if fset is None else _wrapper(fset)
 
+    def copy(self) -> magicproperty[_V]:
+        raise NotImplementedError
 
-class Surface(_SurfaceBase, HasFields):
-    def __init__(
-        self,
-        data,
-        viewbox: ViewBox,
-        face_color=None,
-        edge_color=None,
-        shading="none",
-        name: str | None = None,
-    ):
-        super().__init__(
-            data,
-            viewbox,
-            face_color=face_color,
-            edge_color=edge_color,
-            shading=shading,
-            name=name,
-        )
+    def getter(self, fget: Callable[[Any], _V]) -> magicproperty[_V]:
+        """Define a getter function."""
+        self._fget = fget
+        if self.label is None:
+            self.label = fget.__name__.replace("_", " ")
+        if return_annotation := fget.__annotations__.get("return", None):
+            self.annotation = return_annotation
+        return self
+
+    __call__ = getter
+
+    def setter(self, fset: Callable[[Any, _V], None]) -> magicproperty[_V]:
+        """Define a setter function."""
+        self._fset = fset
+        if self.label is None:
+            self.label = fset.__name__.replace("_", " ")
+
+        _self, _val = magic_signature(fset).parameters.values()
+        annot, opt = split_annotated_type(_val.annotation)
+        if not self.options:
+            self.options = opt
+        if "widget_type" in opt:
+            self.widget_type = opt.pop("widget_type")
+        if self.annotation in (None, inspect.Parameter.empty):
+            self.annotation = annot
+        return self
+
+    def deleter(self, fdel: Callable[[Any], None]) -> magicproperty[_V]:
+        """Define a deleter function."""
+        self._fdel = fdel
+        return self
+
+    def __set_name__(self, owner: type, name: str) -> None:
+        super().__set_name__(owner, name)
+        if not hasattr(owner, "__annotations__"):
+            return None
+        if annotation := owner.__annotations__.get(name):
+            self.annotation = annotation
+
+    def _default_fget(self, obj) -> _V:
+        """Return the widget value by default."""
+        return self.get_widget(obj).value
+
+    def _default_fset(self, obj, val) -> None:
+        """Do nothing other than updating the value."""
+
+    def __get__(self, obj: Any, objtype: Any = None) -> _V:
+        if obj is None:
+            return self
+        return self._fget(obj)
+
+    def __set__(self, obj: Any, value: _V) -> None:
+        if obj is None:
+            raise AttributeError(f"Cannot set {self.__class__.__name__}.")
+        # first set the value on the widget to check if it's valid
+        gui = self.get_widget(obj)
+        old_value = gui.value
+        with gui.changed.blocked():
+            gui.value = value
+            try:
+                self._fset(obj, value)
+            except Exception:
+                gui.value = old_value
+                raise
 
-    def _create_visual(self, data):
-        self._visual: MeshVisual = visuals.Mesh(
-            vertices=data[0], faces=data[1], parent=self._viewbox.scene
-        )
-        self.data = data
+        gui.changed.emit(value)
 
-    @property
-    def data(self):
-        return self._data
+        return None
 
-    @data.setter
-    def data(self, value) -> None:
-        if len(value) == 2:
-            verts, faces = value
-            vals = None
-        elif len(value) == 3:
-            verts, faces, vals = value
-        else:
-            raise ValueError("Data must be vertices, faces (, values).")
-        self._visual.set_data(vertices=verts, faces=faces, vertex_values=vals)
-        self._data = (verts, faces, vals)
-        self._visual.update()
-
-    shading = vfield(
-        str, options={"choices": ["none", "float", "smooth"], "value": "smooth"}
-    )
-    face_color = vfield(Color)
-    edge_color = vfield(Color)
-    edge_width = vfield(
-        float, widget_type=FloatSlider, options={"min": 0.5, "max": 10.0, "value": 1.0}
-    )
-
-    shading.connect(_SurfaceBase._on_shading_change)
-    face_color.connect(_SurfaceBase._on_face_color_change)
-    edge_color.connect(_SurfaceBase._on_edge_color_change)
-    edge_width.connect(_SurfaceBase._on_edge_width_change)
+    def __delete__(self, obj: Any) -> None:
+        if self._fdel is not None:
+            return self._fdel(obj)
+        raise AttributeError("can't delete attribute")
+
+    def get_widget(self, obj: Any) -> _ButtonedWidget:
+        """A light-weight version."""
+        obj_id = id(obj)
+        if (widget := self._guis.get(obj_id, None)) is None:
+            self._guis[obj_id] = widget = self.construct(obj)
+            widget.name = self.name
+            for callback in self._callbacks:
+                widget.changed.connect(define_callback(obj, callback))
+            widget.changed.connect(lambda val: self._fset(obj, val))
+        return widget
```

### Comparing `magic-class-0.6.9/magicclass/ext/vispy/layerlist.py` & `magic_class-0.7.0rc0/magicclass/ext/vispy/layerlist.py`

 * *Files identical despite different names*

### Comparing `magic-class-0.6.9/magicclass/ext/vispy/plot_api.py` & `magic_class-0.7.0rc0/magicclass/ext/pyqtgraph/plot_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
-from typing import overload, TYPE_CHECKING
+
+from typing import overload, TYPE_CHECKING, Sequence
 import numpy as np
-from .widgets2d import VispyPlotCanvas, VispyMultiPlotCanvas, VispyImageCanvas
+from .widgets import QtPlotCanvas, QtMultiPlotCanvas, QtImageCanvas
 
 if TYPE_CHECKING:
-    from .widgets2d import Has2DViewBox, MultiPlot
+    from .widgets import HasViewBox, _MultiPlot
 
-CURRENT_MULTI_CANVAS: MultiPlot = None
-CURRENT_CANVAS: Has2DViewBox = None
+CURRENT_MULTI_CANVAS: _MultiPlot | None = None
+CURRENT_CANVAS: HasViewBox | None = None
 
 
-def _current_canvas() -> VispyPlotCanvas:
+def gca() -> QtPlotCanvas:
     global CURRENT_CANVAS
     if CURRENT_CANVAS is None:
-        CURRENT_CANVAS = VispyPlotCanvas()
+        CURRENT_CANVAS = QtPlotCanvas()
     return CURRENT_CANVAS
 
 
 def _set_current_canvas(canvas):
     global CURRENT_CANVAS
     CURRENT_CANVAS = canvas
     return canvas
@@ -27,24 +28,23 @@
     global CURRENT_MULTI_CANVAS
     CURRENT_MULTI_CANVAS = multi
     return multi
 
 
 def gcf():
     if CURRENT_MULTI_CANVAS is None:
-        return CURRENT_CANVAS
-    return CURRENT_CANVAS
+        return gca()
+    return CURRENT_MULTI_CANVAS
 
 
-def gca():
-    return CURRENT_CANVAS
+gcw = gcf
 
 
 def figure():
-    _set_current_canvas(VispyPlotCanvas())
+    _set_current_canvas(QtPlotCanvas())
     return CURRENT_CANVAS
 
 
 @overload
 def subplot(pos: int):
     ...
 
@@ -58,15 +58,15 @@
     if len(args) == 1 and args[0] >= 111:
         if args[0] >= 1000:
             raise ValueError(f"Too large: {args[0]}")
         args = (args[0] // 100, args[0] // 10 % 10, args[0] % 10)
 
     row, col, idx = args
     if CURRENT_MULTI_CANVAS is None:
-        _set_current_multi_canvas(VispyMultiPlotCanvas(row, col))
+        _set_current_multi_canvas(QtMultiPlotCanvas(row, col))
     else:
         if not CURRENT_MULTI_CANVAS.shape == (row, col):
             raise ValueError("Shape of subplots does not match")
     return _set_current_canvas(CURRENT_MULTI_CANVAS[idx - 1])
 
 
 def plot(
@@ -76,16 +76,16 @@
     edge_color=None,
     color=None,
     size: float = 7,
     name: str | None = None,
     lw: float = 1,
     ls: str = "-",
     symbol=None,
-) -> VispyPlotCanvas:
-    return _current_canvas().add_curve(
+) -> QtPlotCanvas:
+    return gca().add_curve(
         x=x,
         y=y,
         face_color=face_color,
         edge_color=edge_color,
         color=color,
         size=size,
         name=name,
@@ -100,39 +100,63 @@
     y=None,
     face_color=None,
     edge_color=None,
     color=None,
     size: float = 7,
     name: str | None = None,
     symbol=None,
-) -> VispyPlotCanvas:
-    return _current_canvas().add_scatter(
+) -> QtPlotCanvas:
+    return gca().add_scatter(
         x=x,
         y=y,
         face_color=face_color,
         edge_color=edge_color,
         color=color,
         size=size,
         name=name,
         symbol=symbol,
     )
 
 
+def hist(
+    data: Sequence[float],
+    bins: int | Sequence | str = 10,
+    range=None,
+    density: bool = False,
+    face_color=None,
+    edge_color=None,
+    color=None,
+    name: str | None = None,
+    lw: float = 1,
+    ls: str = "-",
+) -> QtPlotCanvas:
+    return gca().add_hist(
+        data,
+        bins=bins,
+        range=range,
+        density=density,
+        face_color=face_color,
+        edge_color=edge_color,
+        color=color,
+        name=name,
+        lw=lw,
+        ls=ls,
+    )
+
+
 def show():
     if CURRENT_MULTI_CANVAS is not None:
         CURRENT_MULTI_CANVAS.show()
     else:
-        CURRENT_CANVAS.show()
-    _set_current_canvas(None)
-    _set_current_multi_canvas(None)
+        gca().show()
 
 
 def imshow(image, cmap=None, vmin=None, vmax=None):
     image = np.asarray(image)
-    canvas = VispyImageCanvas()
+    canvas = QtImageCanvas()
     _set_current_canvas(canvas)
     canvas.image = image
 
     if cmap is not None:
         canvas.cmap = cmap
 
     if vmin is not None or vmax is not None:
```

### Comparing `magic-class-0.6.9/magicclass/ext/vispy/tests/test_vispy2d.py` & `magic_class-0.7.0rc0/magicclass/ext/vispy/tests/test_vispy2d.py`

 * *Files identical despite different names*

### Comparing `magic-class-0.6.9/magicclass/ext/vispy/widgets2d.py` & `magic_class-0.7.0rc0/magicclass/ext/vispy/widgets2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from vispy import scene
 from vispy.scene import visuals, ViewBox
 
 from .layer2d import Curve, Scatter, Histogram
 from ._base import HasViewBox, SceneCanvas, MultiPlot
 
 from .._doc import write_docs
-from ...widgets import FreeWidget
-from ..._app import get_app
+from magicclass.widgets import FreeWidget
+from magicclass._app import get_app
 
 
 class Has2DViewBox(HasViewBox):
     @property
     def xrange(self) -> tuple[float, float]:
         """Range of X dimension."""
         return self._viewbox.camera._xlim
@@ -43,15 +43,14 @@
         color=None,
         size: float = 7,
         name: str | None = None,
         lw: float = 1,
         ls: str = "-",
         symbol=None,
     ):
-
         """
         Add a line plot like ``plt.plot(x, y)``.
 
         Parameters
         ----------
         {x}{y}{face_color}{edge_color}{color}
         size: float, default is 7
@@ -93,60 +92,75 @@
         face_color=None,
         edge_color=None,
         color=None,
         size: float = 7,
         name: str | None = None,
         symbol=None,
     ):
-
         """
-        Add a line plot like ``plt.plot(x, y)``.
+        Add a scatter plot like ``plt.scatter(x, y)``.
 
         Parameters
         ----------
         {x}{y}{face_color}{edge_color}{color}
         size: float, default is 7
             Symbol size.
         {name}{symbol}
 
         Returns
         -------
-        Curve
-            A plot item of a curve.
+        Scatter
+            A plot item of a scatter.
         """
         x, y = _check_xy(x, y)
         face_color, edge_color = _check_colors(face_color, edge_color, color)
         if isinstance(edge_color, np.ndarray) and edge_color.ndim == 1:
             edge_color = np.stack([edge_color] * y.size, axis=0)
-        line = Scatter(
+        scatter = Scatter(
             self._viewbox,
             x,
             y,
             face_color=face_color,
             edge_color=edge_color,
             size=size,
             name=name,
             symbol=symbol,
         )
-        self._layerlist.append(line)
+        self._layerlist.append(scatter)
         if len(self._layerlist) == 1:
             self.xrange = (np.min(x), np.max(x))
             self.yrange = (np.min(y), np.max(y))
-        return line
+        return scatter
 
     @write_docs
     def add_hist(
         self,
         data,
         bins: int = 10,
         face_color=None,
         edge_color=None,
-        color=None,
+        color="white",
         name: str | None = None,
     ) -> Histogram:
+        """
+        Add a histogram like ``plt.hist(x)``.
+
+        Parameters
+        ----------
+        data: array-like
+            Input 1D data.
+        bins: int, default is 10
+            Number of bins to draw the histogram.
+        {face_color}{edge_color}{color}{name}
+
+        Returns
+        -------
+        Histogram
+            A plot item of a histogram.
+        """
         data = np.asarray(data)
         face_color, edge_color = _check_colors(face_color, edge_color, color)
 
         hist = Histogram(
             self._viewbox,
             data=data,
             bins=bins,
@@ -338,16 +352,16 @@
 
 
 class VispyPlotCanvas(FreeWidget, PlotItem):
     """A Vispy based 2-D plot canvas for curve, histogram, bar plot etc."""
 
     def __init__(self, **kwargs):
         app = get_app()
-        # prepare widget
 
+        # prepare widget
         _scene = SceneCanvas(keys="interactive")
         _scene.create_native()
         viewbox = _scene.central_widget.add_view()
         PlotItem.__init__(self, viewbox)
         super().__init__(**kwargs)
         self.set_widget(_scene.native)
```

### Comparing `magic-class-0.6.9/magicclass/ext/vtk/components.py` & `magic_class-0.7.0rc0/magicclass/ext/vtk/components.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
-from typing import Callable, Generic, Tuple, TypeVar, overload
+from typing import Callable, Generic, TypeVar, overload
 import weakref
 import vedo
-import numpy as np
 from .const import Representation
-from ...fields import vfield, HasFields
-from ...types import Color
+from magicclass.fields import vfield, HasFields
+from magicclass.types import Color
 
 _VtkType = TypeVar("_VtkType", bound=vedo.BaseActor)
 
 
 class VtkComponent(HasFields):
     _vtk_type: type[_VtkType] | Callable[..., _VtkType]
 
@@ -41,57 +40,64 @@
         if v:
             self._obj.on()
         else:
             self._obj.off()
         self._update()
 
     def _update(self):
-        self._parent_ref().window.Render()
+        self._parent_ref().qt_widget.Render()
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}<{hex(id(self))}>"
 
 
 class Points(VtkComponent, base=vedo.Points):
     _obj: vedo.Points
     color = vfield(Color)
     size = vfield(float)
     spherical = vfield(False)
     occlusion = vfield(float)
-    pos = vfield(Tuple[float, float, float])
     scale = vfield(float)
 
+    def __init__(
+        self,
+        data,
+        color=(0.2, 0.2, 0.2),
+        alpha=1,
+        radius=4,
+        _parent: vedo.Plotter = None,
+        _emit: bool = True,
+    ):
+        super().__init__(
+            data, c=color, alpha=alpha, r=radius, _parent=_parent, _emit=_emit
+        )
+
     @color.connect
     def _on_color_change(self, v):
         self._obj.color(v[:3])
         self._update()
 
     @size.connect
     def _on_size_change(self, v):
-        self._obj.PointSize(v)
+        self._obj.point_size(v)
         self._update()
 
     @spherical.connect
     def _on_spherical_change(self, v):
-        self._obj.RenderPointsAsSpheres(v)
+        self._obj.render_points_as_spheres(v)
         self._update()
 
     @occlusion.connect
     def _on_occlusion_change(self, v):
         self._obj.occlusion(v)
         self._update()
 
-    @pos.connect
-    def _on_pos_change(self, v):
-        self._obj.pos(*v)
-        self._update()
-
     @scale.connect
     def _on_scale_change(self, v):
-        self._obj.scale(v, absolute=True)
+        self._obj.scale(v, reset=True)
         self._update()
 
 
 class Mesh(VtkComponent, base=vedo.Mesh):
     _obj: vedo.Mesh
 
     color = vfield(Color)
@@ -112,15 +118,15 @@
     @occlusion.connect
     def _on_occlusion_change(self, v):
         self._obj.occlusion(v)
         self._update()
 
     @scale.connect
     def _on_scale_change(self, v):
-        self._obj.scale(v, absolute=True)
+        self._obj.scale(v, reset=True)
         self._update()
 
     @representation.connect
     def _on_representation_change(self, v: Representation) -> None:
         self._obj.property.SetRepresentation(v.value)
         self._update()
 
@@ -132,25 +138,25 @@
     @backface_color.connect
     def _on_backface_color_change(self, v):
         self._obj.backColor([v * 255 for v in v[:3]])
         self._update()
 
     @frontface_culling.connect
     def _on_frontface_culling_change(self, v):
-        self._obj.frontFaceCulling(v)
+        self._obj.frontface_culling(v)
         self._update()
 
     @backface_culling.connect
     def _on_backface_culling_change(self, v):
-        self._obj.backFaceCulling(v)
+        self._obj.backface_culling(v)
         self._update()
 
     @lines_as_tubes.connect
     def _on_lines_as_tubes_change(self, v):
-        self._obj.renderLinesAsTubes(v)
+        self._obj.render_lines_as_tubes(v)
         self._update()
 
 
 # fmt: off
 class Path(Mesh, base=vedo.Line): ...
 class Sphere(Mesh, base=vedo.Sphere): ...
 class Spheres(Mesh, base=vedo.Spheres): ...
```

### Comparing `magic-class-0.6.9/magicclass/ext/vtk/const.py` & `magic_class-0.7.0rc0/magicclass/ext/vtk/const.py`

 * *Files identical despite different names*

### Comparing `magic-class-0.6.9/magicclass/ext/vtk/widgets.py` & `magic_class-0.7.0rc0/magicclass/ext/vtk/widgets.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,86 @@
 from __future__ import annotations
+
+from typing import TYPE_CHECKING
 import weakref
 import numpy as np
 import vedo
-from qtpy import QtWidgets as QtW
-from vtkmodules.qt.QVTKRenderWindowInteractor import QVTKRenderWindowInteractor
+from qtpy import QtWidgets as QtW, QtGui
+
+if TYPE_CHECKING:
+    from vtkmodules.qt.QVTKRenderWindowInteractor import QVTKRenderWindowInteractor
+else:
+    from vtk.qt.QVTKRenderWindowInteractor import QVTKRenderWindowInteractor
+
 from psygnal.containers import EventedList
 from .const import AxesMode
 from .volume import Volume
-from .components import Mesh, VtkComponent, get_object_type
+from .components import Mesh, VtkComponent, get_object_type, Points
 
-from ...widgets import FreeWidget
-from ...types import Color
+from magicclass.widgets import FreeWidget
+from magicclass.types import Color
 
 
 class QtVtkCanvas(QtW.QWidget):
     def __init__(self, parent=None):
         super().__init__(parent=parent)
         _layout = QtW.QVBoxLayout()
+        _layout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(_layout)
+        vedo.settings.default_backend = "vtk"  # Avoid using Jupyter backend
         self._vtk_widget = QVTKRenderWindowInteractor(parent=self)
-        self.plt = vedo.Plotter(qtWidget=self._vtk_widget, bg="black", axes=0)
+        self.plt = vedo.Plotter(qt_widget=self._vtk_widget, bg="black", axes=0)
         self.plt.show()
 
         _layout.addWidget(self._vtk_widget)
 
+    def closeEvent(self, a0: QtGui.QCloseEvent) -> None:
+        self._vtk_widget.close()
+        return super().closeEvent(a0)
 
-class LayerList(EventedList):
+
+class LayerList(EventedList[VtkComponent]):
     def __init__(self, data=(), parent: VtkCanvas = None):
         super().__init__(data=data)
         self._parent_ref = weakref.ref(parent)
         self.events.inserted.connect(self._on_inserted)
         self.events.removed.connect(self._on_removed)
 
     @property
     def parent(self) -> VtkCanvas:
         return self._parent_ref()
 
     def _on_inserted(self, i: int, obj: VtkComponent):
-        self.parent._qwidget.plt.add(obj._obj)
-        self.parent._qwidget.plt.window.Render()
+        self.parent._qt_vtk_canvas.plt.add(obj._obj, render=True)
         if len(self) == 1:
-            self.parent._qwidget.plt.show(zoom=True)
+            self.parent._qt_vtk_canvas.plt.show(zoom=True)
 
     def _on_removed(self, i: int, obj: VtkComponent):
-        self.parent._qwidget.plt.remove(obj._obj)
-        self.parent._qwidget.plt.window.Render()
-        if len(self) == 1:
-            self.parent._qwidget.plt.show(zoom=True)
+        self.parent._qt_vtk_canvas.plt.remove(obj._obj.name, render=True)
 
 
 class VtkCanvas(FreeWidget):
     def __init__(self):
         """
         A Visualization toolkit (VTK) canvas for magicclass.
 
         This widget is useful for visualizing surface and mesh.
         """
         super().__init__()
-        self._qwidget = QtVtkCanvas()
-        self.set_widget(self._qwidget)
+        self._qt_vtk_canvas = QtVtkCanvas()
+        self.set_widget(self._qt_vtk_canvas)
         self._layers = LayerList(parent=self)
 
     @property
     def layers(self):
         return self._layers
 
     def screenshot(self) -> np.ndarray:
         """Get screenshot as a numpy array."""
-        pic: vedo.Picture = self._qwidget.plt.topicture()
+        pic: vedo.Picture = self._qt_vtk_canvas.plt.topicture()
         img = pic.tonumpy()
         return img
 
     def add_volume(
         self,
         volume: np.ndarray,
         color: Color = (0.7, 0.7, 0.7),
@@ -90,50 +99,69 @@
             Initial visualization mode of the volume.
 
         Returns
         -------
         Volume
             A volume layer.
         """
-        vol = Volume(volume, _parent=self._qwidget.plt)
+        vol = Volume(volume, _parent=self._qt_vtk_canvas.plt)
         self.layers.append(vol)
-        self._qwidget.plt.add(vol._current_obj)
+        self._qt_vtk_canvas.plt.add(vol._current_obj)
         vol.color = color
         vol.mode = mode
         if len(self.layers) == 1:
-            self._qwidget.plt.show(zoom=True)
+            self._qt_vtk_canvas.plt.show(zoom=True)
         return vol
 
     def add_object(self, *args, object_type: str = None, **kwargs):
         obj = get_object_type(object_type.capitalize())(
-            *args, **kwargs, _parent=self._qwidget.plt
+            *args, **kwargs, _parent=self._qt_vtk_canvas.plt
         )
         self.layers.append(obj)
         if len(self.layers) == 1:
-            self._qwidget.plt.show()
+            self._qt_vtk_canvas.plt.show()
         return obj
 
     def add_surface(self, data: tuple[np.ndarray, np.ndarray] | tuple[np.ndarray]):
-        mesh = Mesh(data, _parent=self._qwidget.plt)
+        mesh = Mesh(data, _parent=self._qt_vtk_canvas.plt)
         self.layers.append(mesh)
         if len(self.layers) == 1:
-            self._qwidget.plt.show(zoom=True)
+            self._qt_vtk_canvas.plt.show(zoom=True)
         return mesh
 
+    def add_points(
+        self,
+        data: np.ndarray,
+        color=(0.2, 0.2, 0.2),
+        alpha=1,
+        radius=4,
+    ):
+        points = Points(
+            data,
+            color=color,
+            alpha=alpha,
+            radius=radius,
+            _parent=self._qt_vtk_canvas.plt,
+        )
+        self.layers.append(points)
+        if len(self.layers) == 1:
+            self._qt_vtk_canvas.plt.show(zoom=True)
+        return points
+
     @property
     def axes(self) -> str:
         """The axes object."""
-        return AxesMode(self._qwidget.plt.axes).name
+        return AxesMode(self._qt_vtk_canvas.plt.axes).name
 
     @axes.setter
     def axes(self, v):
-        if self._qwidget.plt.axes_instances:
-            current_axes = self._qwidget.plt.axes_instances[0]
+        if self._qt_vtk_canvas.plt.axes_instances:
+            current_axes = self._qt_vtk_canvas.plt.axes_instances[0]
         else:
             current_axes = None
         a = getattr(AxesMode, v).value
         try:
-            self._qwidget.plt.remove(current_axes)
+            self._qt_vtk_canvas.plt.remove(current_axes)
         except TypeError:
             current_axes.EnabledOff()
-        self._qwidget.plt.axes_instances = [None]
-        self._qwidget.plt.show(axes=a)
+        self._qt_vtk_canvas.plt.axes_instances = [None]
+        self._qt_vtk_canvas.plt.show(axes=a)
```

### Comparing `magic-class-0.6.9/magicclass/fields/_fields.py` & `magic_class-0.7.0rc0/magicclass/fields/_fields.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,85 +1,86 @@
 from __future__ import annotations
 from typing import (
     Any,
     TYPE_CHECKING,
     Callable,
+    Sequence,
     TypeVar,
     overload,
     Generic,
-    Union,
 )
 from typing_extensions import Literal, _AnnotatedAlias
-from pathlib import Path
-import datetime
-import sys
-from enum import Enum
-from magicgui.widgets import create_widget
-from magicgui.widgets._bases import Widget, ValueWidget, ContainerWidget
-from magicgui.widgets._bases.value_widget import UNSET
+from magicgui.widgets import create_widget, Widget
+from magicgui.widgets.bases import (
+    ValueWidget,
+    ContainerWidget,
+    CategoricalWidget,
+)
+from magicgui.types import Undefined
+from magicclass.types import MGUI_SIMPLE_TYPES
+
+from ._define import define_callback, define_callback_gui
 
-from ..utils import (
-    argcount,
+from magicclass.utils import (
     is_instance_method,
     method_as_getter,
     eval_attribute,
+    is_type_like,
 )
-from .._gui.mgui_ext import Action, WidgetAction
+from magicclass.signature import MagicMethodSignature
+from magicclass._gui.mgui_ext import Action, WidgetAction
 
 if TYPE_CHECKING:
-    from magicgui.widgets._protocols import WidgetProtocol
     from typing_extensions import Self
-    from .._gui._base import MagicTemplate
-    from .._gui.mgui_ext import AbstractAction
+    from magicclass._gui._base import MagicTemplate
+    from magicclass._gui.mgui_ext import AbstractAction
 
     _M = TypeVar("_M", bound=MagicTemplate)
-
-if sys.version_info >= (3, 10):
-    from typing import _BaseGenericAlias
-else:
-    from typing_extensions import _BaseGenericAlias
+    _X = TypeVar("_X", bound=MGUI_SIMPLE_TYPES)
 
 
 class _FieldObject:
     name: str
     tooltip: str
 
     def get_widget(self, obj: Any) -> Widget:
         raise NotImplementedError()
 
 
 _W = TypeVar("_W", bound=Widget)
-_V = TypeVar("_V", bound=object)
+_V = TypeVar("_V")
+_U = TypeVar("_U")
+_F = TypeVar("_F", bound=Callable)
 
 
-class MagicField(_FieldObject, Generic[_W, _V]):
+class MagicField(_FieldObject, Generic[_W]):
     """
     Field class for magicgui construction.
 
     This object is compatible with dataclass. MagicField object is in "ready for
     widget construction" state.
     """
 
     default_object = object()
 
     def __init__(
         self,
-        value: Any = UNSET,
+        value: Any = Undefined,
         name: str | None = None,
         label: str | None = None,
         annotation: Any = None,
         widget_type: type | str | None = None,
         options: dict[str, Any] | None = None,
         record: bool = True,
         constructor: Callable[..., Widget] | None = None,
     ):
         if options is None:
             options = {}
-        if value is UNSET:
-            value = options.pop("value", UNSET)
+        if value is Undefined:
+            value = options.pop("value", Undefined)
 
         if constructor is None:
 
             def _create_widget(obj):
                 return create_widget(
                     self.value,
                     name=self.name,
@@ -102,49 +103,136 @@
         self._guis: dict[int, _M] = {}
         self._record = record
 
         # MagicField has to remenber the first class that referred to itself so
         # that it can "know" the namespace it belongs to.
         self._parent_class: type | None = None
 
+        # This attribute will be used when wrapped field/vfield is used.
+        self._destination_class: type | None = None
+
     def __repr__(self):
         attrs = ["value", "name", "widget_type", "record", "options"]
         kw = ", ".join(f"{a}={getattr(self, a)!r}" for a in attrs)
         return f"{self.__class__.__name__}({kw})"
 
     def __set_name__(self, owner: type, name: str) -> None:
         self._parent_class = owner
         if self.name is None:
             self.name = name
 
+        if self._destination_class is not None:
+            from magicclass.wrappers import abstractapi
+
+            api = getattr(self._destination_class, name, None)
+            if isinstance(api, abstractapi):
+                api.resolve()
+                api.__signature__ = MagicMethodSignature([])
+
+    def set_destination(self, dest: type) -> None:
+        self._destination_class = dest
+        return None
+
+    def with_options(
+        self,
+        value: Any = Undefined,
+        tooltip: str = Undefined,
+        visible: bool = Undefined,
+        enabled: bool = Undefined,
+        gui_only: bool = Undefined,
+        bind=Undefined,
+        **kwargs,
+    ) -> Self:
+        """
+        Method ot add options to the field.
+
+        Following expressions returns the same field.
+        >>> x = field(int, options={"max": 10})
+        >>> x = field(int).with_options(max=10)
+        """
+        kwargs = dict(
+            value=value,
+            tooltip=tooltip,
+            visible=visible,
+            enabled=enabled,
+            gui_only=gui_only,
+            bind=bind,
+            **kwargs,
+        )
+        to_pop: list[str] = []
+        for k, v in kwargs.items():
+            if v is Undefined:
+                to_pop.append(k)
+        for k in to_pop:
+            kwargs.pop(k)
+        if "value" in kwargs:
+            self.value = kwargs.pop("value")
+        self.options.update(kwargs)
+        return self
+
+    @overload
+    def with_choices(
+        self, choices: Sequence[tuple[str, _U]]
+    ) -> MagicField[CategoricalWidget, _U]:
+        ...
+
+    @overload
+    def with_choices(self, choices: Sequence[_U]) -> MagicField[CategoricalWidget, _U]:
+        ...
+
+    @overload
+    def with_choices(
+        self, choices: Callable[..., Sequence[tuple[str, _U]]]
+    ) -> MagicField[CategoricalWidget, _U]:
+        ...
+
+    @overload
+    def with_choices(
+        self, choices: Callable[..., Sequence[_U]]
+    ) -> MagicField[CategoricalWidget, _U]:
+        ...
+
+    def with_choices(self, choices):
+        """Method to add choices to the field."""
+        self.options["choices"] = choices
+        return self
+
+    @property
+    def __signature__(self):
+        """This property is necessary to hack _unwrap_method."""
+        additional_options = {}
+        if self._destination_class is not None:
+            additional_options["into"] = self._destination_class.__name__
+        return MagicMethodSignature([], additional_options=additional_options)
+
     @property
     def constructor(self) -> Callable[..., Widget]:
         """Get widget constructor."""
         return self._constructor
 
     @property
     def callbacks(self) -> tuple[Callable, ...]:
         """Return callbacks in an immutable way."""
         return tuple(self._callbacks)
 
     @property
     def record(self) -> bool:
         return self._record
 
-    def construct(self, obj) -> Widget:
+    def construct(self, obj) -> _W:
         """Construct a widget."""
         constructor = self.constructor
         _arg_choices = self.options.get("choices", None)
         if isinstance(_arg_choices, str):
             _arg_choices = eval_attribute(type(obj), _arg_choices)
 
         if is_instance_method(_arg_choices):
             self.options["choices"] = method_as_getter(obj, _arg_choices)
         try:
-            if _is_subclass(constructor, Widget):
+            if _is_magicclass(constructor):
                 widget = constructor(**self.options)
             else:
                 widget = constructor(obj)
                 if not isinstance(widget, Widget):
                     raise TypeError(
                         f"{self.__class__.__name__} {self.name} created non-widget "
                         f"object {type(widget)}."
@@ -152,15 +240,15 @@
 
         finally:
             if _arg_choices is not None:
                 self.options["choices"] = _arg_choices
 
         return widget
 
-    def copy(self) -> Self[_W, _V]:
+    def copy(self) -> MagicField[_W]:
         """Copy object."""
         return self.__class__(
             value=self.value,
             name=self.name,
             label=self.label,
             annotation=self.annotation,
             widget_type=self.widget_type,
@@ -175,50 +263,47 @@
         return cls(constructor=func)
 
     def get_widget(self, obj: Any) -> _W:
         """
         Get a widget from ``obj``. This function will be called every time MagicField is referred
         by ``obj.field``.
         """
-        from .._gui import MagicTemplate
+        from magicclass._gui import MagicTemplate
 
         obj_id = id(obj)
-        if obj_id in self._guis.keys():
-            widget = self._guis[obj_id]
-        else:
-            widget = self.construct(obj)
+        if (widget := self._guis.get(obj_id, None)) is None:
+            self._guis[obj_id] = widget = self.construct(obj)
             widget.name = self.name
-            self._guis[obj_id] = widget
 
             if isinstance(widget, (ValueWidget, ContainerWidget)):
                 if isinstance(obj, MagicTemplate):
-                    _def = _define_callback_gui
+                    _def = define_callback_gui
                 else:
-                    _def = _define_callback
+                    _def = define_callback
                 for callback in self._callbacks:
                     # funcname = callback.__name__
                     widget.changed.connect(_def(obj, callback))
 
         return widget
 
     def get_action(self, obj: Any) -> AbstractAction:
         """
         Get an action from ``obj``. This function will be called every time MagicField is referred
         by ``obj.field``.
         """
-        from .._gui import MagicTemplate
+        from magicclass._gui import MagicTemplate
 
         obj_id = id(obj)
         if obj_id in self._guis.keys():
             action = self._guis[obj_id]
         else:
             if type(self.value) is bool or self.annotation is bool:
                 # we should not use "isinstance" or "issubclass" because subclass
                 # may be mapped to different widget by users.
-                value = False if self.value is UNSET else self.value
+                value = False if self.value is Undefined else self.value
                 action = Action(
                     checkable=True,
                     checked=value,
                     text=self.name.replace("_", " "),
                     name=self.name,
                 )
                 for k, v in self.options.items():
@@ -228,24 +313,24 @@
                 widget.name = self.name
                 action = WidgetAction(widget)
 
             self._guis[obj_id] = action
 
             if action.support_value:
                 if isinstance(obj, MagicTemplate):
-                    _def = _define_callback_gui
+                    _def = define_callback_gui
                 else:
-                    _def = _define_callback
+                    _def = define_callback
                 for callback in self._callbacks:
                     # funcname = callback.__name__
                     action.changed.connect(_def(obj, callback))
 
         return action
 
-    def as_getter(self, obj: Any) -> Callable[[Any], _V]:
+    def as_getter(self, obj: Any) -> Callable[[Any], Any]:
         """Make a function that get the value of Widget or Action."""
         return lambda w: self._guis[id(obj)].value
 
     def as_remote_getter(self, obj: Any):
         """Called when a MagicField is used in Bound method."""
         qualname = self._parent_class.__qualname__
         _LOCALS = "<locals>."
@@ -275,15 +360,15 @@
                     "thus cannot be used as a bound value."
                 )
             return self.as_getter(ins)(w)
 
         return _func
 
     @overload
-    def __get__(self, obj: Literal[None], objtype=None) -> MagicField[_W, _V]:
+    def __get__(self, obj: Literal[None], objtype=None) -> MagicField[_W]:
         ...
 
     @overload
     def __get__(self, obj: Any, objtype=None) -> _W:
         ...
 
     def __get__(self, obj, objtype=None):
@@ -297,15 +382,15 @@
 
     def ready(self) -> bool:
         """Return true if field is ready to create widgets."""
         return not self.not_ready()
 
     def not_ready(self) -> bool:
         return (
-            self.value is UNSET
+            self.value is Undefined
             and self.annotation is None
             and self.widget_type is None
             and "choices" not in self.options
         )
 
     def to_widget(self) -> _W:
         """
@@ -335,15 +420,15 @@
         Raises
         ------
         ValueError
             If there is not enough information to build an action.
         """
         return self.get_action(self.default_object)
 
-    def connect(self, func: Callable) -> Callable:
+    def connect(self, func: _F) -> _F:
         """Set callback function to "ready to connect" state."""
         if not callable(func):
             raise TypeError("Cannot connect non-callable object")
         self._callbacks.append(func)
         return func
 
     def disconnect(self, func: Callable) -> None:
@@ -352,21 +437,22 @@
         This method does NOT disconnect callbacks from widgets that are
         already created.
         """
         i = self._callbacks.index(func)
         self._callbacks.pop(i)
         return None
 
-    def wraps(
-        self,
-        method: Callable | None = None,
-        *,
-        template: Callable | None = None,
-        copy: bool = False,
-    ):
+    # fmt: off
+    @overload
+    def wraps(self, method: _F, *, template: Callable | None = None, copy: bool = False) -> _F: ...
+    @overload
+    def wraps(self, method: None = ..., *, template: Callable | None = None, copy: bool = False) -> Callable[[_F], _F]: ...
+    # fmt: on
+
+    def wraps(self, method, *, template=None, copy=False):
         """
         Call the ``wraps`` class method of magic class.
 
         This method is needed when a child magic class is defined outside the main magic
         class, and integrated into the main magic class by ``field`` function, like below
 
         .. code-block:: python
@@ -393,15 +479,15 @@
             If true, wrapped method is still enabled.
 
         Returns
         -------
         Callable
             Same method as input, but has updated signature.
         """
-        from .._gui import BaseGui
+        from magicclass._gui import BaseGui
 
         cls = self.constructor
         if not (isinstance(cls, type) and issubclass(cls, BaseGui)):
             raise TypeError(
                 "The wraps method cannot be used for any objects but magic class."
             )
         return cls.wraps(method=method, template=template, copy=copy)
@@ -435,38 +521,41 @@
 
     @property
     def widget_type(self) -> type[Widget]:
         """Return type of the resulting widget."""
         return self._widget_type
 
 
-class MagicValueField(MagicField[_W, _V]):
+class MagicValueField(MagicField[ValueWidget[_V]]):
     """
     Field class for magicgui construction. Unlike MagicField, object of this class
     always returns value itself.
     """
 
     @overload
-    def __get__(self, obj: Literal[None], objtype=None) -> MagicValueField[_W, _V] | _V:
+    def __get__(self, obj: Literal[None], objtype=None) -> MagicValueField[_V] | _V:
         ...
 
     @overload
     def __get__(self, obj: Any, objtype=None) -> _V:
         ...
 
     def __get__(self, obj, objtype=None):
         if obj is None:
             return self
         return self._postgethook(obj, self.get_widget(obj).value)
 
-    def __set__(self, obj: _M, value: _V) -> None:
+    def __set__(self, obj: MagicTemplate, value: _V) -> None:
         if obj is None:
             raise AttributeError(f"Cannot set {self.__class__.__name__}.")
         self.get_widget(obj).value = self._presethook(obj, value)
 
+    def copy(self) -> MagicValueField[_V]:
+        return super().copy()
+
     def post_get_hook(self, hook: Callable[[Any, _V], Any] | Callable[[_V], Any]):
         """
         Define a post-get hook for the field.
 
         If a post-get hook is set, value will always be converted before returned.
         Following example shows how to convert ``x`` to a float every time it gets
         accessed.
@@ -513,230 +602,273 @@
             raise TypeError("Pre-set hook must be callable.")
         if is_instance_method(hook):
             self._presethook = hook
         else:
             self._presethook = lambda _, x: hook(x)
         return hook
 
-    def _postgethook(self, obj, value):
+    def _postgethook(self, obj, value: _V) -> _V:
         return value
 
-    def _presethook(self, obj, value):
+    def _presethook(self, obj, value: _V) -> _V:
         return value
 
+    @overload
+    def with_choices(
+        self, choices: Sequence[tuple[str, _U]]
+    ) -> MagicValueField[CategoricalWidget[_U], _U]:
+        ...
 
-# magicgui symple types
-_X = TypeVar(
-    "_X",
-    bound=Union[
-        int,
-        float,
-        bool,
-        str,
-        Path,
-        datetime.datetime,
-        datetime.date,
-        datetime.time,
-        Enum,
-        range,
-        slice,
-        list,
-        tuple,
-    ],
-)
+    @overload
+    def with_choices(
+        self, choices: Sequence[_U]
+    ) -> MagicValueField[CategoricalWidget[_U], _U]:
+        ...
+
+    @overload
+    def with_choices(
+        self, choices: Callable[..., Sequence[tuple[str, _U]]]
+    ) -> MagicValueField[CategoricalWidget[_U], _U]:
+        ...
+
+    @overload
+    def with_choices(
+        self, choices: Callable[..., Sequence[_U]]
+    ) -> MagicValueField[CategoricalWidget[_U], _U]:
+        ...
+
+    def with_choices(self, choices):
+        """Method to add choices to the field."""
+        return super().with_choices(choices)
 
 
 @overload
 def field(
-    obj: _X,
+    gui_class: type[_M],
     *,
     name: str | None = None,
     label: str | None = None,
-    widget_type: str | type[WidgetProtocol] | type[Widget] | None = None,
+    widget_type: str | None = None,
     options: dict[str, Any] = {},
     record: bool = True,
-) -> MagicField[ValueWidget, _X]:
+) -> MagicField[_M]:
     ...
 
 
 @overload
 def field(
-    widget_type: type[_W],
+    obj: type[_W],
     *,
     name: str | None = None,
     label: str | None = None,
     options: dict[str, Any] = {},
     record: bool = True,
-) -> MagicField[_W, Any]:
+) -> MagicField[_W]:
     ...
 
 
 @overload
 def field(
     obj: type[_X],
     *,
     name: str | None = None,
     label: str | None = None,
-    widget_type: str | type[WidgetProtocol] | type[Widget] | None = None,
+    widget_type: str | None = None,
     options: dict[str, Any] = {},
     record: bool = True,
-) -> MagicField[ValueWidget, _X]:
+) -> MagicField[ValueWidget[_X]]:
     ...
 
 
 @overload
 def field(
-    gui_class: type[_M],
+    obj: _X,
     *,
     name: str | None = None,
     label: str | None = None,
-    widget_type: str | type[WidgetProtocol] | type[Widget] | None = None,
+    widget_type: str | None = None,
     options: dict[str, Any] = {},
     record: bool = True,
-) -> MagicField[_M, Any]:
+) -> MagicField[ValueWidget[_X]]:
     ...
 
 
 @overload
 def field(
-    obj: Any,
+    obj: Any | None = None,
     *,
     name: str | None = None,
     label: str | None = None,
     widget_type: type[_W] = None,
     options: dict[str, Any] = {},
     record: bool = True,
-) -> MagicField[_W, Any]:
+) -> MagicField[_W]:
     ...
 
 
 @overload
 def field(
     obj: Any,
     *,
     name: str | None = None,
     label: str | None = None,
-    widget_type: str | type[WidgetProtocol] | None = None,
+    widget_type: str | None = None,
     options: dict[str, Any] = {},
     record: bool = True,
-) -> MagicField[Widget, Any]:
+) -> MagicField[Widget]:
     ...
 
 
+@overload
 def field(
-    obj: Any = UNSET,
     *,
     name: str | None = None,
     label: str | None = None,
-    widget_type: str | type[WidgetProtocol] | None = None,
+    widget_type: str | type[Widget] | None = None,
     options: dict[str, Any] = {},
     record: bool = True,
-) -> MagicField[Widget, Any]:
+) -> MagicField[Widget]:
+    ...
+
+
+def field(
+    obj=Undefined,
+    *,
+    name=None,
+    label=None,
+    widget_type=None,
+    options={},
+    record=True,
+):
     """
     Make a MagicField object.
 
     >>> i = field(1)
     >>> i = field(widget_type="Slider")
 
     Parameters
     ----------
-    obj : Any, default is UNSET
+    obj : Any, default is Undefined
         Reference to determine what type of widget will be created. If Widget
         subclass is given, it will be used as is. If other type of class is given,
         it will used as type annotation. If an object (not type) is given, it will
         be assumed to be the default value.
     name : str, optional
         Name of the widget.
     label : str, optional
         Label of the widget.
     widget_type : str, optional
         Widget type. This argument will be sent to ``create_widget`` function.
-    options : WidgetOptions, optional
+    options : dict, optional
         Widget options. This parameter will be passed to the ``options`` keyword
         argument of ``create_widget``.
     record : bool, default is True
         A magic-class specific parameter. If true, record value changes as macro.
 
     Returns
     -------
     MagicField
     """
     return _get_field(obj, name, label, widget_type, options, record, MagicField)
 
 
 @overload
 def vfield(
-    obj: _X,
+    widget_type: type[ValueWidget[_V]],
     *,
     name: str | None = None,
     label: str | None = None,
-    widget_type: str | type[WidgetProtocol] | type[Widget] | None = None,
     options: dict[str, Any] = {},
     record: bool = True,
-) -> MagicValueField[ValueWidget, _X]:
+) -> MagicValueField[_V]:
     ...
 
 
 @overload
 def vfield(
-    widget_type: type[_W],
+    widget_type: type[Widget],
     *,
     name: str | None = None,
     label: str | None = None,
     options: dict[str, Any] = {},
     record: bool = True,
-) -> MagicValueField[_W, Any]:
+) -> MagicValueField[Any]:
     ...
 
 
 @overload
 def vfield(
-    annotation: type[_X],
+    obj: type[_X],
     *,
     name: str | None = None,
     label: str | None = None,
-    widget_type: str | type[WidgetProtocol] | type[Widget] | None = None,
+    widget_type: str | type[Widget] | None = None,
     options: dict[str, Any] = {},
     record: bool = True,
-) -> MagicValueField[ValueWidget, _X]:
+) -> MagicValueField[_X]:
     ...
 
 
 @overload
 def vfield(
-    obj: Any,
+    obj: _X,
     *,
     name: str | None = None,
     label: str | None = None,
-    widget_type: type[_W] = None,
+    widget_type: str | type[Widget] | None = None,
+    options: dict[str, Any] = {},
+    record: bool = True,
+) -> MagicValueField[_X]:
+    ...
+
+
+@overload
+def vfield(
+    obj: Any | None = None,
+    *,
+    name: str | None = None,
+    label: str | None = None,
+    widget_type: type[ValueWidget[_V]] = None,
     options: dict[str, Any] = {},
     record: bool = True,
-) -> MagicValueField[_W, Any]:
+) -> MagicValueField[_V]:
     ...
 
 
 @overload
 def vfield(
     obj: Any,
     *,
     name: str | None = None,
     label: str | None = None,
-    widget_type: str | type[WidgetProtocol] | type[Widget] | None = None,
+    widget_type: str | type[Widget] | None = None,
     options: dict[str, Any] = {},
     record: bool = True,
-) -> MagicValueField[Widget, Any]:
+) -> MagicValueField[Any]:
+    ...
+
+
+@overload
+def vfield(
+    *,
+    name: str | None = None,
+    label: str | None = None,
+    widget_type: str | type[Widget] | None = None,
+    options: dict[str, Any] = {},
+    record: bool = True,
+) -> MagicValueField[Any]:
     ...
 
 
 def vfield(
-    obj: Any = UNSET,
+    obj: Any = Undefined,
     *,
     name: str | None = None,
     label: str | None = None,
-    widget_type: str | type[WidgetProtocol] | None = None,
+    widget_type: str | None = None,
     options: dict[str, Any] = {},
     record: bool = True,
 ) -> MagicValueField[Widget, Any]:
     """
     Make a MagicValueField object.
 
     >>> i = vfield(1)
@@ -745,26 +877,26 @@
     Unlike MagicField, value itself can be accessed.
 
     >>> ui.i      # int is returned
     >>> ui.i = 3  # set value to the widget.
 
     Parameters
     ----------
-    obj : Any, default is UNSET
+    obj : Any, default is Undefined
         Reference to determine what type of widget will be created. If Widget
         subclass is given, it will be used as is. If other type of class is given,
         it will used as type annotation. If an object (not type) is given, it will
         be assumed to be the default value.
     name : str, optional
         Name of the widget.
     label : str, optional
         Label of the widget.
     widget_type : str, optional
         Widget type. This argument will be sent to ``create_widget`` function.
-    options : WidgetOptions, optional
+    options : dict, optional
         Widget options. This parameter will be passed to the ``options`` keyword
         argument of ``create_widget``.
     record : bool, default is True
         A magic-class specific parameter. If true, record value changes as macro.
 
     Returns
     -------
@@ -809,92 +941,48 @@
     return MagicValueField.from_callable(func)
 
 
 def _get_field(
     obj,
     name: str,
     label: str,
-    widget_type: str | type[WidgetProtocol] | None,
+    widget_type: str | None,
     options: dict[str, Any],
     record: bool,
     field_class: type[MagicField],
 ) -> MagicField:
     if not isinstance(options, dict):
         raise TypeError(f"Field options must be a dict, got {type(options)}")
     options = options.copy()
     kwargs = dict(
         name=name, label=label, record=record, annotation=None, options=options
     )
-    if isinstance(obj, (type, _BaseGenericAlias)):
+    if is_type_like(obj):
         if isinstance(obj, _AnnotatedAlias):
-            from magicgui.signature import split_annotated_type
+            from magicclass.signature import split_annotated_type
 
             tp, widget_option = split_annotated_type(obj)
             kwargs.update(annotation=tp)
             options.update(**widget_option)
-        if _is_subclass(obj, Widget):
+        if _is_magicclass(obj):
             if widget_type is not None:
                 raise ValueError("Cannot specify Widget type twice.")
             f = field_class(constructor=obj, widget_type=obj, **kwargs)
         else:
             if kwargs["annotation"] is None:
                 kwargs.update(annotation=obj)
             f = field_class(widget_type=widget_type, **kwargs)
-    elif obj is UNSET:
+    elif obj is Undefined:
         f = field_class(widget_type=widget_type, **kwargs)
     else:
         f = field_class(value=obj, widget_type=widget_type, **kwargs)
 
     return f
 
 
-def _is_subclass(obj: Any, class_or_tuple):
+def _is_magicclass(obj: Any):
+    from magicclass._gui import BaseGui
+
     try:
-        return issubclass(obj, class_or_tuple)
+        return issubclass(obj, (Widget, BaseGui))
     except Exception:
         return False
-
-
-def _define_callback(self: Any, callback: Callable):
-    """Define a callback function from a method."""
-    return callback.__get__(self)
-
-
-def _define_callback_gui(self: MagicTemplate, callback: Callable):
-    """Define a callback function from a method of a magic-class."""
-
-    *_, clsname, funcname = callback.__qualname__.split(".")
-    mro = self.__class__.__mro__
-    for base in mro:
-        if base.__name__ == clsname:
-            _func: Callable = getattr(base, funcname).__get__(self)
-            _func = _normalize_argcount(_func)
-
-            def _callback(v):
-                with self.macro.blocked():
-                    _func(v)
-                return None
-
-            break
-    else:
-
-        def _callback(v):
-            # search for parent instances that have the same name.
-            current_self = self
-            while not (
-                hasattr(current_self, funcname)
-                and current_self.__class__.__qualname__.split(".")[-1] == clsname
-            ):
-                current_self = current_self.__magicclass_parent__
-            _func = _normalize_argcount(getattr(current_self, funcname))
-
-            with self.macro.blocked():
-                _func(v)
-            return None
-
-    return _callback
-
-
-def _normalize_argcount(func: Callable) -> Callable[[Any], Any]:
-    if argcount(func) == 0:
-        return lambda v: func()
-    return func
```

### Comparing `magic-class-0.6.9/magicclass/fields/_group.py` & `magic_class-0.7.0rc0/magicclass/fields/_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,20 @@
     TYPE_CHECKING,
     Callable,
     Iterator,
     TypeVar,
     overload,
 )
 from abc import ABCMeta
-from magicgui.widgets import Container
-from magicgui.widgets._bases import Widget
+from magicgui.widgets import Container, Widget
 from psygnal import SignalInstance
 
 from ._fields import MagicField, MagicValueField, _FieldObject
-from ..utils import Tooltips
+from ._define import define_callback, define_callback_gui
+from magicclass.utils import Tooltips
 
 if TYPE_CHECKING:
     from typing_extensions import Self, Literal
 
 
 class _FieldGroupMeta(ABCMeta):
     _fields: dict[str, MagicField]
@@ -309,16 +309,24 @@
     def __set__(self, obj, value) -> None:
         raise AttributeError(f"Cannot set value to {self.__class__.__name__}.")
 
     def get_widget(self, obj) -> Container:
         _id = id(obj)
         wdt = self._containers.get(_id, None)
         if wdt is None:
+            from .._gui import MagicTemplate
+
             wdt = self.copy()
             self._containers[_id] = wdt
+            if isinstance(obj, MagicTemplate):
+                _def = define_callback_gui
+            else:
+                _def = define_callback
+            for callback in self._callbacks:
+                wdt.changed.connect(_def(obj, callback))
         return wdt
 
     def connect(self, callback: Callable):
         # self.changed.connect(callback)  NOTE: the original container doesn't need signals!
         self._callbacks.append(callback)
         return callback
 
@@ -404,14 +412,18 @@
         """Convert view into a Container widget."""
         if keys is None:
             widgets = list(self)
         else:
             widgets = [getattr(self, name) for name in keys]
         return Container(layout=layout, widgets=widgets, labels=labels, **kwargs)
 
+    def show(self, run=False):
+        """Create a container and show it."""
+        return self.as_container().show(run=run)
+
     def emit_all(self) -> None:
         """Emit all the signals with current value."""
         for wdt, sig in zip(self.iterwidgets(), self.itersignals()):
             if sig is not None:
                 sig.emit(wdt.value)
```

### Comparing `magic-class-0.6.9/magicclass/help.py` & `magic_class-0.7.0rc0/magicclass/help.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,56 @@
 from __future__ import annotations
 import weakref
 
-from magicgui.widgets import FunctionGui, Image
-from magicgui.widgets._bases.widget import Widget
-from magicgui.widgets._function_gui import _docstring_to_html
+from magicgui.widgets import FunctionGui, Image, Widget
 
 import qtpy
-from qtpy.QtWidgets import QWidget, QTreeWidget, QTreeWidgetItem, QSplitter
+from qtpy import QtWidgets as QtW, QtGui
 from qtpy.QtCore import Qt
 from typing import Any, Callable, Iterator, TYPE_CHECKING
 
-from .widgets.containers import SplitterContainer
-from .widgets.misc import ConsoleTextEdit
+from magicclass.widgets.containers import SplitterContainer
+from magicclass.widgets.misc import ConsoleTextEdit
 
-from ._gui.mgui_ext import Action, PushButtonPlus, WidgetAction
-from ._gui._base import MagicTemplate
-from .widgets import DraggableContainer, FreeWidget, Separator
-from ._gui.class_gui import (
+from magicclass._gui.mgui_ext import Action, PushButtonPlus, WidgetAction
+from magicclass._gui._base import MagicTemplate
+from magicclass.widgets import DraggableContainer, FreeWidget, Separator
+from magicclass._gui.class_gui import (
     CollapsibleClassGui,
     DraggableClassGui,
     ScrollableClassGui,
     ButtonClassGui,
 )
-from .utils import iter_members, Tooltips, get_signature
+from magicclass.utils import iter_members, Tooltips
 
 if TYPE_CHECKING:
     import numpy as np
 
 # TODO: find, key-binding
 
 
-class _HelpWidget(QSplitter):
+class _HelpWidget(QtW.QSplitter):
     """
     A Qt widget that will show information of a magic-class widget, built from its
     class structure, function docstrings and type annotations.
     """
 
     _initial_image_size = 250
 
     def __init__(self, ui=None, parent=None) -> None:
-        super().__init__(orientation=Qt.Horizontal, parent=parent)
-        self.setWindowFlag(Qt.Window)
-        self._tree = QTreeWidget(self)
+        super().__init__(orientation=Qt.Orientation.Horizontal, parent=parent)
+        self.setWindowFlag(Qt.WindowType.Window)
+        self._tree = QtW.QTreeWidget(self)
         self._tree.itemClicked.connect(self._on_treeitem_clicked)
         self._text = ConsoleTextEdit()
         self._text.read_only = True
         self._mgui_image = Image()
         c = DraggableContainer(widgets=[self._mgui_image])
 
-        def wheelEvent(event):
+        def wheelEvent(event: QtGui.QWheelEvent):
             ang = event.angleDelta().y()
             v0 = self._mgui_image.min_height
             if ang > 0:
                 v = v0 * 1.1
             else:
                 v = v0 / 1.1
             self._resize_image(int(v))
@@ -136,15 +134,15 @@
             self._update_ui_view(item.ui)
             item.setExpanded(True)
         else:
             self._on_treeitem_clicked(item.parent())
         self._resize_image(self._initial_image_size)
 
 
-class UiBoundTreeItem(QTreeWidgetItem):
+class UiBoundTreeItem(QtW.QTreeWidgetItem):
     def __init__(self, parent, ui=None):
         super().__init__(parent)
         if ui is not None:
             self._ui = weakref.ref(ui)
         else:
             self._ui = None
 
@@ -254,15 +252,15 @@
         raise TypeError(type(widget))
     doc = doc.rstrip("<h3>Parameters</h3><ul></ul>")  # If parameter info was not given
     if doc == "":
         doc = "(No document found)"
     return doc
 
 
-def _render(qwidget: QWidget) -> np.ndarray:
+def _render(qwidget: QtW.QWidget) -> np.ndarray:
     """Render Qt widgets. Used in certain type of containers."""
     import numpy as np
 
     img = qwidget.grab().toImage()
     bits = img.constBits()
     h, w, c = img.height(), img.width(), 4
     if qtpy.API_NAME == "PySide2":
@@ -324,7 +322,22 @@
         else:
             kb = get_additional_option(attr, "keybinding", None)
             if kb:
                 keystr = as_shortcut(kb).toString()
                 keymap[keystr] = (name, Tooltips(attr).desc)
 
     return keymap
+
+
+def _docstring_to_html(docs: str) -> str:
+    """Convert docstring into rich text html."""
+    from docstring_parser import parse
+    import re
+
+    ds = parse(docs)
+
+    ptemp = "<li><p><strong>{}</strong> (<em>{}</em>) - {}</p></li>"
+    plist = [ptemp.format(p.arg_name, p.type_name, p.description) for p in ds.params]
+    params = "<h3>Parameters</h3><ul>{}</ul>".format("".join(plist))
+    short = f"<p>{ds.short_description}</p>" if ds.short_description else ""
+    long = f"<p>{ds.long_description}</p>" if ds.long_description else ""
+    return re.sub(r"``?([^`]+)``?", r"<code>\1</code>", f"{short}{long}{params}")
```

### Comparing `magic-class-0.6.9/magicclass/signature.py` & `magic_class-0.7.0rc0/magicclass/signature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from __future__ import annotations
-from typing import Any, TypedDict
-from typing_extensions import _AnnotatedAlias
-from magicgui.signature import MagicSignature, split_annotated_type
+from typing import Any, Callable, TypedDict
+from typing_extensions import _AnnotatedAlias, get_args
+from magicgui.signature import MagicSignature
 from magicgui.widgets import FunctionGui
-from magicgui.types import WidgetOptions
 import inspect
-from .utils import get_signature
+from magicclass.utils import get_signature
 
 
 class AdditionalOptions(TypedDict):
     record: bool
     keybinding: str
     into: str
     copyto: str
     moveto: str
     gui: bool
+    on_called: list[Callable]
 
 
 def upgrade_signature(
     func,
     gui_options: dict = None,
-    caller_options: WidgetOptions = None,
+    caller_options: dict = None,
     additional_options: AdditionalOptions = None,
 ):
     """
     Upgrade function signature to MagicMethodSignature. The input function may have
     a inspect.Signature or magicgui.signature.Magicsignature.
 
     Parameters
     ----------
     func : callable
         Input function.
     gui_options : dict, optional
         Options of FunctionGui.
-    caller_options : WidgetOptions, optional
+    caller_options : dict, optional
         Options of PushButton.
     additional_options : AdditionalOptions, optional
         Additional options that will be used in magic class.
 
     Returns
     -------
     callable
@@ -143,17 +143,17 @@
             return_annotation=sig.return_annotation,
             gui_options=gui_options,
             caller_options=caller_options,
             additional_options=additional_options,
         )
 
     @classmethod
-    def get_gui_options(cls, sig: inspect.Signature | MagicSignature) -> WidgetOptions:
+    def get_gui_options(cls, sig: inspect.Signature | MagicSignature) -> dict:
         if type(sig) is inspect.Signature:
-            out: WidgetOptions = {}
+            out: dict = {}
             for k, v in sig.parameters.items():
                 annot = v.annotation
                 if isinstance(annot, _AnnotatedAlias):
                     _, widget_option = split_annotated_type(annot)
                     out[k] = widget_option
             return out
         else:
@@ -179,7 +179,24 @@
         return cls(
             parameters,
             return_annotation=return_annotation,
             gui_options=cls.get_gui_options(self),
             caller_options=self.caller_options,
             additional_options=self.additional_options,
         )
+
+
+def split_annotated_type(annotation: _AnnotatedAlias) -> tuple[Any, dict]:
+    """Split an Annotated type into its base type and options dict."""
+    if not isinstance(annotation, _AnnotatedAlias):
+        raise TypeError("Type hint must be an 'Annotated' type.")
+
+    typ, *meta = get_args(annotation)
+    all_meta = {}
+    for m in meta:
+        if not isinstance(m, dict):
+            raise TypeError(
+                "Invalid Annotated format for magicgui. Arguments must be a dict"
+            )
+        all_meta.update(m)
+
+    return typ, all_meta
```

### Comparing `magic-class-0.6.9/magicclass/stylesheets/__init__.py` & `magic_class-0.7.0rc0/magicclass/stylesheets/__init__.py`

 * *Files identical despite different names*

### Comparing `magic-class-0.6.9/magicclass/testing.py` & `magic_class-0.7.0rc0/magicclass/testing.py`

 * *Files identical despite different names*

### Comparing `magic-class-0.6.9/magicclass/utils/_click.py` & `magic_class-0.7.0rc0/magicclass/utils/_click.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 from functools import wraps
 from typing import Callable, Iterable, Union, TYPE_CHECKING, Iterator
 
 if TYPE_CHECKING:
-    from .._gui import BaseGui
-    from .._gui.mgui_ext import Action
-    from magicgui.widgets._bases import ButtonWidget
+    from magicgui.widgets.bases import ButtonWidget
+    from magicclass._gui import BaseGui
+    from magicclass._gui.mgui_ext import Action
 
 nStrings = Union[str, Iterable[str]]
 
 
 def click(
     enables: nStrings | None = None,
     disables: nStrings | None = None,
```

### Comparing `magic-class-0.6.9/magicclass/utils/_functions.py` & `magic_class-0.7.0rc0/magicclass/utils/_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,29 @@
 import inspect
 from types import MethodType
 from typing import Any, TYPE_CHECKING, Callable, Iterable
 import warnings
 from docstring_parser import parse
 
 if TYPE_CHECKING:
-    from .._gui import BaseGui
+    from magicclass._gui import BaseGui
+
+try:
+    from typing import _BaseGenericAlias
+except ImportError:
+    from typing_extensions import _BaseGenericAlias
+
+_type_like = (type, _BaseGenericAlias)
+
+try:
+    from types import GenericAlias
+
+    _type_like += (GenericAlias,)
+except ImportError:
+    pass
 
 
 def iter_members(cls: type, exclude_prefix: str = "__") -> Iterable[tuple[str, Any]]:
     """
     Iterate over all the members in the order of source code line number.
     This function is identical to inspect.getmembers except for the order
     of the results. We have to sort the name in the order of line number.
@@ -218,7 +232,11 @@
                 raise TypeError(f"{name} type mismatch.")
             if hasattr(attr, "__signature__"):
                 dst_attr.__signature__ = attr.__signature__
             if attr.__doc__:
                 dst_attr.__doc__ = attr.__doc__
 
     return None
+
+
+def is_type_like(x: Any) -> bool:
+    return isinstance(x, _type_like) or hasattr(x, "__supertype__")
```

### Comparing `magic-class-0.6.9/magicclass/utils/qt.py` & `magic_class-0.7.0rc0/magicclass/utils/qt.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,17 @@
     """Get the center coordinate of the screen."""
     _screen_rect = QtGui.QGuiApplication.primaryScreen().geometry()
     return _screen_rect.center()
 
 
 def move_to_screen_center(qwidget: QWidget) -> None:
     """Move a QWidget to the center of screen."""
-    qwidget.move(screen_center() - qwidget.rect().center())
+    point = screen_center() - qwidget.rect().center()
+    qwidget.move(point)
+    qwidget.adjustSize()
     return None
 
 
 def screen_scale() -> float:
     """Get the scale of main screen."""
     from qtpy.QtGui import QGuiApplication
 
@@ -104,15 +106,19 @@
 
     if isinstance(obj, str):
         clipboard.setText(obj)
     elif isinstance(obj, np.ndarray):
         if obj.dtype != np.uint8:
             raise ValueError(f"Cannot copy an array of dtype {obj.dtype} to clipboard.")
         # See https://gist.github.com/smex/5287589
-        qimg_format = QImage.Format_RGB888 if obj.ndim == 3 else QImage.Format_Indexed8
+        qimg_format = (
+            QImage.Format.Format_RGB888
+            if obj.ndim == 3
+            else QImage.Format.Format_Indexed8
+        )
         *_, h, w = obj.shape
         qimg = QImage(obj.data, w, h, obj.strides[0], qimg_format)
         gray_color_table = [qRgb(i, i, i) for i in range(256)]
         qimg.setColorTable(gray_color_table)
         clipboard.setImage(qimg)
     elif isinstance(obj, pd.DataFrame):
         clipboard.setText(obj.to_csv(sep="\t"))
```

### Comparing `magic-class-0.6.9/magicclass/utils/qthreading.py` & `magic_class-0.7.0rc0/magicclass/_gui/_macro.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,803 +1,591 @@
 from __future__ import annotations
-import threading
-import time
-from timeit import default_timer
-import inspect
-from functools import partial, wraps
-from typing import (
-    Any,
-    Callable,
-    TYPE_CHECKING,
-    Iterable,
-    Union,
-    overload,
-    TypeVar,
-    Generic,
-    Protocol,
-    runtime_checkable,
-)
-from typing_extensions import TypedDict, ParamSpec
-
-from superqt.utils import create_worker, GeneratorWorker, FunctionWorker
-from qtpy.QtCore import Qt
-from magicgui.widgets import ProgressBar, Container, Widget, PushButton, Label
-from magicgui.application import use_app
+from pathlib import Path
 
-from . import get_signature, move_to_screen_center
-from .qtsignal import QtSignal
+from typing import TYPE_CHECKING, Any, Callable, Iterable, overload
+import warnings
+from qtpy import QtWidgets as QtW, QtCore
+from macrokit import Symbol, Expr, Head, BaseMacro, parse
+from magicgui.widgets import FileEdit, LineEdit
+
+from magicclass.widgets import CodeEdit, TabbedContainer, ScrollableContainer, Dialog
+from magicclass.utils import move_to_screen_center
+from magicclass.undo import ImplementsUndo, RedoAction, UndoCallback
+from magicclass._gui.runner import CommandRunnerMenu
 
 if TYPE_CHECKING:
-    from .._gui import BaseGui
-    from .._gui.mgui_ext import PushButtonPlus, Action
-    from .._gui._macro import GuiMacro
-    from ..fields import MagicField
+    from ._base import BaseGui
+    from .mgui_ext import Clickable
 
-__all__ = ["thread_worker", "Timer", "Callback"]
 
+class MacroEdit(TabbedContainer):
+    """A text edit embeded with a custom menu bar."""
 
-class ProgressDict(TypedDict):
-    """Supported keys for the progress argument."""
+    window_count = 0
 
-    desc: str | Callable
-    total: str | Callable
-    pbar: ProgressBar | _SupportProgress | MagicField
-
-
-@runtime_checkable
-class _SupportProgress(Protocol):
-    """
-    A progress protocol.
-
-    Progressbar must be implemented with methods ``__init__``, ``set_description``,
-    ``show``, ``close`` and properties ``value``, ``max``. Optionally ``set_worker``
-    can be used so that progressbar has an access to the worker object.
-    """
-
-    def __init__(self, max: int = 1, **kwargs):
-        raise NotImplementedError()
-
-    @property
-    def value(self) -> int:
-        """Return the current progress."""
-        raise NotImplementedError()
-
-    @value.setter
-    def value(self, v) -> None:
-        """Set the current progress."""
-        raise NotImplementedError()
-
-    @property
-    def max(self) -> int:
-        """Return the maximum progress value."""
-        raise NotImplementedError()
-
-    @max.setter
-    def max(self, v) -> None:
-        """Set the maximum progress value."""
-        raise NotImplementedError()
-
-    def set_description(self, desc: str):
-        """Set the description of the progressbar."""
-        raise NotImplementedError()
-
-    def show(self):
-        """Show the progressbar."""
-        raise NotImplementedError()
-
-    def close(self):
-        """Close the progressbar."""
-        raise NotImplementedError()
-
-
-_P = ParamSpec("_P")
-_R1 = TypeVar("_R1")
-_R2 = TypeVar("_R2")
-
-
-class CallbackList(Generic[_R1]):
-    """List of callback functions."""
-
-    def __init__(self):
-        self._callbacks: list[Callable[[Any, _R1], _R2] | Callable[[Any], _R2]] = []
+    def __init__(self, **kwargs):
+        super().__init__(labels=False, **kwargs)
+        self.native: QtW.QWidget
+        self.__magicclass_parent__: BaseGui | None = None
+        self.native.setWindowTitle("Macro")
+        self.native_tab_widget.setTabBarAutoHide(True)
+        self._native_macro = None
+        self._recorded_macro = None
+        self._set_menubar()
+
+    def _add_code_edit(self, name: str = "macro", native: bool = False) -> CodeEdit:
+        """Add a new code edit widget as a new tab."""
+        from magicclass._gui._base import defaults
+
+        textedit = CodeEdit(name=name)
+        if native:
+            if self._native_macro is not None:
+                raise ValueError("Native macro already exists.")
+            textedit.read_only = True
+            self._native_macro = textedit
+
+        self.append(textedit)
+        if defaults["macro-highlight"]:
+            textedit.syntax_highlight()
+        textedit.__magicclass_parent__ = self.__magicclass_parent__
+        textedit.executing.connect(self._on_executing)
+        return textedit
+
+    def _on_executing(self, desc: str):
+        if desc == "exec-line":
+            self._execute_selected()
+        elif desc == "register-command":
+            self._create_command()
+        else:
+            raise RuntimeError(f"Unknown executing description: {desc}")
 
-    @property
-    def callbacks(self) -> tuple[Callable[[Any, _R1], _R2] | Callable[[Any], _R2], ...]:
-        return tuple(self._callbacks)
+    def get_selected_expr(self) -> Expr:
+        """Return the selected code in the current code editor."""
+        all_code: str = self.textedit.value
+        selected = self.textedit.selected
+
+        # to safely run code, every line should be fully selected even if the
+        # selected region does not raise SyntaxError.
+        l = len(selected)
+        start = all_code.find(selected)
+        end = start + l
+        if start != 0 and "\n" not in all_code[start - 1 : start + 1]:
+            raise SyntaxError("Select full line(s).")
+        if end < l and "\n" not in all_code[end : end + 2]:
+            raise SyntaxError("Select full line(s).")
+
+        code = parse(selected.strip())
+        return code
+
+    def _create_command(self):
+        """Create command from the selected code."""
+        parent = self._search_parent_magicclass()
+        code = self.get_selected_expr()
+        fn = lambda: code.eval({Symbol.var("ui"): parent})
+        tooltip = f"<b><code>{code}</code></b>"
+        # replace \n with <br> to show multiline code in tooltip
+        tooltip = tooltip.replace("\n", "<br>")
+        self._command_menu.add_action(fn, tooltip=tooltip)
+
+    def _rename_command(self):
+        """Rename currently registered commands."""
+        cnt = ScrollableContainer()
+        for i, action in enumerate(self._command_menu):
+            cnt.append(
+                LineEdit(label=str(i), value=action.text, tooltip=action.tooltip)
+            )
+        dlg = Dialog(widgets=[cnt], parent=self)
+        dlg.exec()
+        for i, line in enumerate(cnt):
+            action = self._command_menu[i]
+            action.text = line.value
+
+    @property
+    def textedit(self) -> CodeEdit | None:
+        """Return the current code editor"""
+        wdt = self[self.current_index]
+        if isinstance(wdt, CodeEdit):
+            return wdt
+        raise ValueError("This tab is not a code editor.")
+
+    @property
+    def native_macro(self) -> CodeEdit | None:
+        """The code edit widget for the native macro"""
+        return self._native_macro
+
+    @property
+    def recorded_macro(self) -> CodeEdit | None:
+        """The code edit widget for the recording macro"""
+        return self._recorded_macro
+
+    def load(self, path: str):
+        """Load macro text from a file."""
+        _path = Path(path)
+        with open(_path) as f:
+            edit = self.new_tab(_path.stem)
+            edit.value = f.read()
+
+    def save(self, path: str):
+        """Save current macro text."""
+        path = str(path)
+        with open(path, mode="w") as f:
+            f.write(self.textedit.value)
+
+    def _close(self, e=None):
+        """Close widget."""
+        return self.close()
+
+    def execute(self):
+        """Execute macro."""
+        self._execute(parse(self.textedit.value))
+
+    def _create_native_duplicate(self, e=None):
+        new = self.new_tab("script")
+        new.value = self.native_macro.value
+
+    def new_tab(self, name: str | None = None) -> CodeEdit:
+        if name is None:
+            name = "script"
+        # find unique name
+        suffix = 0
+        tab_name = name
+        existing_names = {tab.name for tab in self}
+        while tab_name in existing_names:
+            tab_name = f"{name}-{suffix}"
+            suffix += 1
+        new = self._add_code_edit(tab_name)
+        self.current_index = len(self) - 1
+        return new
 
-    def connect(
-        self, callback: Callable[[Any, _R1], _R2] | Callable[[Any], _R2]
-    ) -> Callable[[Any, _R1], _R2] | Callable[[Any], _R2]:
+    def new_window(self, name: str = None) -> MacroEdit:
         """
-        Append a callback function to the callback list.
+        Create a new window with same parent magic class widget.
 
         Parameters
         ----------
-        callback : Callable
-            Callback function.
-        """
-        if not callable(callback):
-            raise TypeError("Can only connect callable object.")
-        self._callbacks.append(callback)
-        return callback
-
-    def disconnect(
-        self, callback: Callable[[Any, _R1], _R2] | Callable[[Any], _R2]
-    ) -> Callable[[Any, _R1], _R2] | Callable[[Any], _R2]:
-        """
-        Remove callback function from the callback list.
+        name : str, optional
+            Widget name. This name will be the title.
 
-        Parameters
-        ----------
-        callback : Callable
-            Callback function to be removed.
+        Returns
+        -------
+        MacroEdit
+            New MacroEdit widget.
         """
-        self._callbacks.remove(callback)
-        return callback
-
-    def _iter_as_method(self, obj: BaseGui) -> Iterable[Callable]:
-        for ref in self._callbacks:
-            yield _make_method(ref, obj)
-
-
-def _make_method(func, obj: BaseGui):
-    def f(*args, **kwargs):
-        with obj.macro.blocked():
-            out = func.__get__(obj)(*args, **kwargs)
-        return out
-
-    return f
-
-
-class NapariProgressBar(_SupportProgress):
-    """A progressbar class that provides napari progress bar with same API."""
-
-    def __init__(self, value: int = 0, max: int = 1000):
-        from napari.utils import progress
-
-        with progress._all_instances.events.changed.blocker():
-            self._pbar = progress(total=max)
-            self._pbar.n = value
-
-    @property
-    def value(self) -> int:
-        return self._pbar.n
+        if name is None:
+            name = f"Macro-{self.__class__.window_count}"
+            self.__class__.window_count += 1
+        new = self.__class__(name=name)
+        new.__magicclass_parent__ = self.__magicclass_parent__
+        new.native.setParent(self.native.parent(), new.native.windowFlags())
+        new._add_code_edit()
+        new.show()
+        geometry = self.native.geometry()
+        geometry.moveTopLeft(geometry.topLeft() + QtCore.QPoint(20, 20))
+        new.native.setGeometry(geometry)
+        return new
+
+    def duplicate(self, name: str = None):
+        warnings.warn(
+            "duplicate() is deprecated. MacroEdit is now a tabbed widget. "
+            "Use 'new_window()' or 'new_tab()' instead.",
+            DeprecationWarning,
+        )
+        current = self.textedit
+        text = current.value
+        new = self.new_window(name=name)
+        new.textedit.value = text
+        return new
+
+    def new(self, name: str = None):
+        warnings.warn(
+            "new() is deprecated. MacroEdit is now a tabbed widget. "
+            "Use 'new_window()' or 'new_tab()' instead.",
+            DeprecationWarning,
+        )
+        return self.new_window(name=name)
 
-    @value.setter
-    def value(self, v) -> None:
-        self._pbar.n = v
-        self._pbar.events.value(value=self._pbar.n)
+    def _new_tab(self, e=None):
+        self.new_tab()
 
-    @property
-    def max(self) -> int:
-        return self._pbar.total
+    def _duplicate_tab(self, e=None):
+        current_value = self.textedit.value
+        new = self.new_tab(self.textedit.name)
+        new.value = current_value
+        self.current_index = len(self) - 1
+
+    def _delete_tab(self, e=None):
+        if len(self) == 0:
+            return
+        index = self.current_index
+        if self[index] is not self.native_macro:
+            """Don't delete the native macro tab."""
+            del self[index]
 
-    @max.setter
-    def max(self, v) -> None:
-        self._pbar.total = v
+    def _zoom_in(self, e=None):
+        self.textedit.zoom_in()
 
-    def set_description(self, v: str) -> None:
-        self._pbar.set_description(v)
-
-    @property
-    def visible(self) -> bool:
-        return False
+    def _zoom_out(self, e=None):
+        self.textedit.zoom_out()
 
     def show(self):
-        type(self._pbar)._all_instances.events.changed(added={self._pbar}, removed={})
-
-    def close(self):
-        self._pbar.close()
-
-
-class Timer:
-    """A timer class with intuitive API."""
-
-    def __init__(self):
-        self.reset()
-
-    def __repr__(self) -> str:
-        """Return string in format hh:mm:ss"""
-        return self.format_time()
-
-    @property
-    def sec(self) -> float:
-        """Return current second."""
-        self.lap()
-        return self._t_total
-
-    def start(self):
-        """Start timer."""
-        self._t0 = default_timer()
-        self._running = True
-
-    def stop(self) -> float:
-        """Stop timer."""
-        self.lap()
-        self._running = False
-
-    def lap(self) -> float:
-        """Return lap time."""
-        if self._running:
-            now = default_timer()
-            self._t_total += now - self._t0
-            self._t0 = now
-        return self._t_total
-
-    def reset(self):
-        """Reset timer."""
-        self._t0 = default_timer()
-        self._t_total = 0.0
-        self._running = False
-        return None
-
-    def format_time(self, fmt: str = "{hour:0>2}:{min:0>2}:{sec:0>2}") -> str:
-        """Format current time."""
-        min_all, sec = divmod(self.sec, 60)
-        hour, min = divmod(min_all, 60)
-        return fmt.format(hour=int(hour), min=int(min), sec=int(sec))
-
-
-class DefaultProgressBar(Container, _SupportProgress):
-    """The default progressbar widget."""
-
-    def __init__(self, max: int = 1):
-        self.progress_label = Label(value="Progress")
-        self.pbar = ProgressBar(value=0, max=max)
-        self.time_label = Label(value="00:00")
-        self.pause_button = PushButton(text="Pause")
-        self.abort_button = PushButton(text="Abort")
-        cnt = Container(
-            layout="horizontal",
-            widgets=[self.time_label, self.pause_button, self.abort_button],
-            labels=False,
-        )
-        cnt.margins = (0, 0, 0, 0)
-        self.footer = cnt
-        self.pbar.min_width = 360
-        self._timer = Timer()
-        self._time_signal = QtSignal()
-        self._time_signal.connect(self._on_timer_updated)
-
-        super().__init__(widgets=[self.progress_label, self.pbar, cnt], labels=False)
-
-    def _on_timer_updated(self, _=None):
-        if self._timer.sec < 3600:
-            self.time_label.value = self._timer.format_time("{min:0>2}:{sec:0>2}")
+        if self.parent is None:
+            ui = self.__magicclass_parent__
+            self.native.setParent(ui.native, self.native.windowFlags())
+        super().show()
+        move_to_screen_center(self.native)
+        self.textedit.native.setFocus()
+
+    def _execute(self, code: Expr):
+        """Run macro."""
+        parent = self._search_parent_magicclass()
+        try:
+            if str(code) == "":
+                raise ValueError("No code selected")
+            ns = {Symbol.var("ui"): parent}
+            if (viewer := parent.parent_viewer) is not None:
+                ns.setdefault(Symbol.var("viewer"), viewer)
+            code.eval(ns)
+        except Exception as e:
+            parent._error_mode.get_handler()(e, self)
+
+    def _execute_selected(self, e=None):
+        """Run selected line of macro."""
+        self._execute(self.get_selected_expr())
+
+    def execute_lines(self, indices: int | slice | Iterable[int]):
+        all_text: str = self.textedit.value
+        lines = all_text.split("\n")
+        if isinstance(indices, int):
+            input_text = lines[indices]
+        elif isinstance(indices, slice):
+            input_text = "\n".join(lines[indices])
         else:
-            self.time_label.value = self._timer.format_time()
-        return None
-
-    def _start_thread(self):
-        # Start background thread
-        self._running = True
-        self._thread_timer = threading.Thread(target=self._update_timer_label)
-        self._thread_timer.daemon = True
-        self._thread_timer.start()
-        self._timer.start()
-        return None
+            input_text = "\n".join(lines[i] for i in indices)
+        code = parse(input_text)
+        return self._execute(code)
+
+    def _search_parent_magicclass(self) -> BaseGui:
+        current_self = self
+        while getattr(current_self, "__magicclass_parent__", None) is not None:
+            current_self = current_self.__magicclass_parent__
+        return current_self
+
+    def _new_window(self, e=None):
+        self.new_window()
+
+    def _load(self, e=None):
+        """Load macro"""
+        fdialog = FileEdit(mode="r", filter="*.txt;*.py")
+        result = fdialog._show_file_dialog(
+            fdialog.mode,
+            caption=fdialog._btn_text,
+            start_path=str(fdialog.value),
+            filter=fdialog.filter,
+        )
+        if result:
+            self.load(result)
 
-    def _update_timer_label(self):
-        """Background thread for updating the progress bar"""
-        while self._running:
-            if self._timer._running:
-                self._time_signal.emit()
+    def _save(self, e=None):
+        """Save text."""
+        fdialog = FileEdit(mode="w", filter="*.txt;*.py")
+        result = fdialog._show_file_dialog(
+            fdialog.mode,
+            caption=fdialog._btn_text,
+            start_path=str(fdialog.value),
+            filter=fdialog.filter,
+        )
+        if result:
+            self.save(result)
 
-            time.sleep(0.1)
+    def _start_recording(self):
+        index = self.current_index
+        if self[index] is self.native_macro:
+            self.new_tab("record")
+        self._recorded_macro = self.textedit
+
+    def _finish_recording(self):
+        self._recorded_macro = None
+
+    def _set_menubar(self):
+        self._menubar = QtW.QMenuBar(self.native)
+        self.native.layout().setMenuBar(self._menubar)
+
+        # fmt: off
+        self._file_menu = QtW.QMenu("File", self.native)
+        self._file_menu.setToolTipsVisible(True)
+        self._menubar.addMenu(self._file_menu)
+
+        self._file_menu.addAction(_action("New window", self._new_window, tooltip="Open a new macro editor"))
+        self._file_menu.addSeparator()
+        self._file_menu.addAction(_action("Open file", self._load, "Ctrl+O", tooltip="Open a python file"))
+        self._file_menu.addAction(_action("Save", self._save, "Ctrl+S", tooltip="Save the macro as a python file"))
+        self._file_menu.addSeparator()
+        self._file_menu.addAction(_action("Close", self._close, tooltip="Close this macro editor"))
+
+        self._tab_menu = QtW.QMenu("Tab", self.native)
+        self._tab_menu.setToolTipsVisible(True)
+        self._menubar.addMenu(self._tab_menu)
+        self._tab_menu.addAction(_action("New tab", self._new_tab, "Ctrl+T", tooltip="Open a new empty tab"))
+        self._tab_menu.addAction(_action("Duplicate tab", self._duplicate_tab, "Ctrl+D", tooltip="Duplicate current tab as a new tab"))
+        self._tab_menu.addAction(_action("Current macro in new tab", self._create_native_duplicate, tooltip="Duplicate current GUI macro in a new tab"))
+        self._tab_menu.addAction(_action("Delete tab", self._delete_tab, "Ctrl+W", tooltip="Delete current tab"))
+        self._tab_menu.addSeparator()
+        self._tab_menu.addAction(_action("Zoom in", self._zoom_in, "Ctrl+Shift+.", tooltip="Zoom in the text"))
+        self._tab_menu.addAction(_action("Zoom out", self._zoom_out, "Ctrl+Shift+,", tooltip="Zoom out the text"))
+
+
+        # set macro menu
+        self._macro_menu = QtW.QMenu("Macro", self.native)
+        self._macro_menu.setToolTipsVisible(True)
+        self._menubar.addMenu(self._macro_menu)
+
+        self._macro_menu.addAction(_action("Execute", self.execute, "Ctrl+F5", tooltip="Execute the entire script of the current tab"))
+        self._macro_menu.addAction(_action("Execute selected lines", self._execute_selected, "Ctrl+Shift+F5", tooltip="Execute the selected lines of the current tab"))
+        self._macro_menu.addSeparator()
+        _action_start = _action("Start recording", self._start_recording, tooltip="Open a new tab and start recording GUI operations in it")
+        self._macro_menu.addAction(_action_start)
+        _action_finish = _action("Finish recording", self._finish_recording, tooltip="Finish the recording task started by 'Start recording' menu")
+        self._macro_menu.addAction(_action_finish)
+
+        _action_finish.setEnabled(False)
+        _action_start.triggered.connect(lambda: _action_finish.setEnabled(True))
+        _action_finish.triggered.connect(lambda: _action_finish.setEnabled(False))
+
+        self._command_menu = CommandRunnerMenu(
+            "Command",
+            parent=self.native,
+            magicclass_parent=self._search_parent_magicclass(),
+        )
+        self._command_menu.native.setToolTipsVisible(True)
+        self._menubar.addMenu(self._command_menu.native)
+        self._command_menu.native.addAction(_action("Create command", self._create_command, tooltip="Create a command using the selected lines"))
+        self._command_menu.native.addAction(_action("Rename command", self._rename_command, tooltip="Rename regeistered commands."))
+        self._command_menu.native.addSeparator()
+        # fmt: on
+
+
+def _action(
+    text: str, slot: Callable, shortcut: str | None = None, tooltip: str | None = None
+):
+    """Create a QAction object. Backend compatible."""
+    action = QtW.QAction(text)
+    action.triggered.connect(slot)
+    if shortcut:
+        action.setShortcut(shortcut)
+    if tooltip:
+        action.setToolTip(tooltip)
+    return action
+
+
+class GuiMacro(BaseMacro):
+    """Macro object with GUI-specific functions."""
+
+    def __init__(self, ui: BaseGui = None, max_lines: int = 10000, max_undo: int = 100):
+        from datetime import datetime
+
+        super().__init__()
+        self._max_lines = max_lines
+        self._max_undo = max_undo
+        self.on_appended.append(self._on_macro_added)
+        self.on_popped.append(self._on_macro_popped)
+
+        self._widget = MacroEdit(name="Macro")
+        self._widget.__magicclass_parent__ = ui
+        self._widget._add_code_edit(native=True)
+        now = datetime.now()
+        self.append(Expr(Head.comment, [now.strftime("%Y/%m/%d %H:%M:%S")]))
+
+        self._stack_undo: list[ImplementsUndo] = []
+        self._stack_redo: list[tuple[Expr, ImplementsUndo]] = []
+
+    @property
+    def widget(self) -> MacroEdit:
+        """Returns the macro editor."""
+        return self._widget
+
+    @property
+    def _gui_parent(self) -> BaseGui:
+        """The parent GUI object."""
+        return self.widget.__magicclass_parent__
+
+    def clear_undo_stack(self) -> None:
+        """Clear all the history of undo/redo."""
+        self._stack_undo.clear()
+        self._stack_redo.clear()
+
+    def append_with_undo(self, expr: Expr, undo: UndoCallback) -> None:
+        """Append an expression with its undo action."""
+        if not isinstance(undo, UndoCallback):
+            if callable(undo):
+                undo = UndoCallback(undo)
+            else:
+                raise TypeError(f"undo must be callable, not {type(undo)}")
+        self.append(expr)
+        self._append_undo(undo)
         return None
 
-    def _finish(self):
-        self._running = False
-        self._thread_timer.join()
+    def _append_undo(self, undo: ImplementsUndo) -> None:
+        self._stack_undo.append(undo)
+        self._stack_redo.clear()
+        if len(self._stack_undo) > self._max_undo:
+            self._stack_undo.pop(0)
         return None
 
-    @property
-    def paused(self) -> bool:
-        """True if paused."""
-        return not self._timer._running
-
-    @property
-    def value(self) -> int:
-        """Progress bar value."""
-        return self.pbar.value
-
-    @value.setter
-    def value(self, v):
-        self.pbar.value = v
+    def _pop_undo(self) -> ImplementsUndo:
+        return self._stack_undo.pop()
 
     @property
-    def max(self) -> int:
-        return self.pbar.max
-
-    @max.setter
-    def max(self, v):
-        self.pbar.max = v
-
-    def set_description(self, desc: str):
-        """Set description as the label of the progressbar."""
-        self.progress_label.value = desc
-        return None
-
-    def set_worker(self, worker: GeneratorWorker | FunctionWorker):
-        """Set currently running worker."""
-        self._worker = worker
-        self._worker.finished.connect(self._finish)
-        self._worker.started.connect(self._start_thread)
-        if not isinstance(self._worker, GeneratorWorker):
-            # FunctionWorker does not have yielded/aborted signals.
-            self.footer[1].visible = False
-            self.footer[2].visible = False
-            return None
-        # initialize abort_button
-        self.abort_button.text = "Abort"
-        self.abort_button.changed.connect(self._abort_worker)
-        self.abort_button.enabled = True
-
-        # initialize pause_button
-        self.pause_button.text = "Pause"
-        self.pause_button.enabled = True
-        self.pause_button.changed.connect(self._toggle_pause)
-
-        @self._worker.paused.connect
-        def _on_pause():
-            self.pause_button.text = "Resume"
-            self.pause_button.enabled = True
-            self._timer.stop()
-
-        return None
+    def undo_stack(self) -> dict[str, list[Expr]]:
+        """Return a copy of undo stack info."""
+        n_undo = len(self._stack_undo)
+        return dict(
+            undo=[expr.copy() for expr in self.args[-n_undo:]],
+            redo=[expr.copy() for expr, _ in self._stack_redo],
+        )
 
-    def _toggle_pause(self):
-        if self.paused:
-            self._worker.resume()
-            self.pause_button.text = "Pause"
-            self._timer.start()
+    def undo(self):
+        """Undo the last operation if undo is defined."""
+        if len(self._stack_undo) == 0:
+            return
+        undo = self._stack_undo.pop()
+        try:
+            with self.blocked():
+                undo.run()
+        except Exception as e:
+            self._stack_undo.append(undo)
+            raise e
         else:
-            self._worker.pause()
-            self.pause_button.text = "Pausing"
-            self.pause_button.enabled = False
-
-        return None
+            expr = self.pop()
+            self._stack_redo.append((expr, undo))
 
-    def _abort_worker(self):
-        self.pause_button.text = "Pause"
-        self.abort_button.text = "Aborting"
-        self.pause_button.enabled = False
-        self.abort_button.enabled = False
-        self._worker.quit()
-        return None
-
-
-class Aborted(RuntimeError):
-    """Raised when worker is aborted."""
-
-    @classmethod
-    def raise_(cls, *args):
-        """A function version of "raise"."""
-        if not args:
-            args = ("Aborted.",)
-        raise cls(*args)
-
-
-ProgressBarLike = Union[ProgressBar, _SupportProgress]
-
-
-class thread_worker:
-    """Create a worker in a superqt/napari style."""
-
-    _DEFAULT_PROGRESS_BAR = DefaultProgressBar
-    _DEFAULT_TOTAL = 0
-    _WINDOW_FLAG = (
-        Qt.WindowType.WindowTitleHint
-        | Qt.WindowType.WindowMinimizeButtonHint
-        | Qt.WindowType.Window
-    )
-
-    def __init__(
-        self,
-        f: Callable[_P, _R1] | None = None,
-        *,
-        ignore_errors: bool = False,
-        progress: ProgressDict | None = None,
-    ) -> None:
-        self._func: Callable[_P, _R1] | None = None
-        self._callback_dict_ = {
-            "started": CallbackList(),
-            "returned": CallbackList(),
-            "errored": CallbackList(),
-            "yielded": CallbackList(),
-            "finished": CallbackList(),
-            "aborted": CallbackList(),
-        }
-
-        self._ignore_errors = ignore_errors
-        self._objects: dict[int, BaseGui] = {}
-        self._progressbars: dict[int, ProgressBarLike | None] = {}
-        self._recorder: Callable[_P, Any] | None = None
-
-        if f is not None:
-            self(f)
-
-        if progress:
-            if isinstance(progress, bool):
-                progress = {}
-
-            progress.setdefault("desc", None)
-            progress.setdefault("total", 0)
-            progress.setdefault("pbar", None)
-
-        self._progress = progress
-
-    @property
-    def func(self) -> Callable[_P, _R1]:
-        return self._func
-
-    @classmethod
-    def set_default(cls, pbar_cls: Callable | str):
-        """
-        Set the default progressbar class.
-
-        This class method is useful when there is an user-defined class that
-        follows ``_SupportProgress`` protocol.
-
-        Parameters
-        ----------
-        pbar_cls : callable or str
-            The default class. In principle this parameter does not have to be a
-            class. As long as ``pbar_cls(max=...)`` returns a ``_SupportProgress``
-            object it works. Either "default" or "napari" is also accepted.
-
-        """
-        if isinstance(pbar_cls, str):
-            if pbar_cls == "napari":
-                pbar_cls = NapariProgressBar
-            elif pbar_cls == "default":
-                pbar_cls = DefaultProgressBar
+    def redo(self):
+        """Redo the last undo operation."""
+        if len(self._stack_redo) == 0:
+            return
+        if not self.active:
+            raise ValueError("Cannot redo when the macro is blocked.")
+        expr, undo = self._stack_redo.pop()
+        try:
+            redo_action = undo.redo_action
+            if redo_action.matches("default"):
+                ns = {self._gui_parent._my_symbol: self._gui_parent}
+                parent = self._gui_parent
+                if (viewer := parent.parent_viewer) is not None:
+                    ns.setdefault(Symbol.var("viewer"), viewer)
+                with self.blocked():
+                    expr.eval(ns)
+            elif redo_action.matches("custom"):
+                redo_action: RedoAction.Custom
+                redo_action.run()
             else:
-                raise ValueError(
-                    f"Unknown progress bar {pbar_cls!r}. Must be either 'default' or "
-                    "'napari', or a proper type object."
-                )
-        cls._DEFAULT_PROGRESS_BAR = pbar_cls
-        return pbar_cls
-
-    @staticmethod
-    def to_callback(callback: Callable, *args, **kwargs) -> Callback:
-        """Convert a callback to a callback object."""
-        cb = Callback(callback)
-        if args or kwargs:
-            cb = cb(*args, **kwargs)
-        return cb
-
-    @property
-    def is_generator(self) -> bool:
-        """True if bound function is a generator function."""
-        return inspect.isgeneratorfunction(self._func)
+                raise ValueError(f"Redo is not defined for {undo}")
+        except Exception as e:
+            self._stack_redo.append((expr, undo))
+            raise e
+        else:
+            self.append(expr)
+            self._stack_undo.append(undo)
 
-    @property
-    def __doc__(self) -> str:
-        """Synchronize docstring with bound function."""
-        return self.func.__doc__
-
-    @__doc__.setter
-    def __doc__(self, doc: str):
-        self.func.__doc__ = doc
+    def copy(self) -> BaseMacro:
+        """Copy the macro instance."""
+        # GuiMacro does not support deepcopy (and apparently _widget should not be copied)
+        from copy import deepcopy
 
-    def _set_recorder(self, recorder: Callable[_P, Any]):
-        """
-        Set macro recorder function.
-        Must accept ``recorder(bgui, *args, **kwargs)``.
-        """
-        self._recorder = recorder
-        return None
+        return BaseMacro(deepcopy(self.args))
 
     @overload
-    def __call__(self, f: Callable[_P, _R1]) -> thread_worker:
+    def __getitem__(self, key: int) -> Expr:
         ...
 
     @overload
-    def __call__(self, bgui: BaseGui, *args, **kwargs) -> Any:
+    def __getitem__(self, key: slice) -> BaseMacro:
         ...
 
-    def __call__(self, *args, **kwargs):
-        if self._func is None:
-            f = args[0]
-            self._func = f
-            wraps(f)(self)  # NOTE: __name__ etc. are updated here.
-            return self
-        else:
-            return self._func(*args, **kwargs)
+    def __getitem__(self, key):
+        if isinstance(key, slice):
+            return BaseMacro(self._args)[key]
+        return super().__getitem__(key)
+
+    def subset(self, indices: Iterable[int]) -> BaseMacro:
+        """Generate a subset of macro."""
+        args = [self._args[i] for i in indices]
+        return BaseMacro(args)
+
+    def get_command(self, key: int) -> Callable[[], Any]:
+        """Get the command function at the give index."""
+        action = self.widget._command_menu[key]
+        return lambda: action.trigger()
 
-    def __get__(self, gui: BaseGui, objtype=None):
-        if gui is None:
-            return self
-
-        gui_id = id(gui)
-        if gui_id in self._objects:
-            return self._objects[gui_id]
-
-        _create_worker = self._create_method(gui)
-        _create_worker.__signature__ = self._get_method_signature()
-
-        self._objects[gui_id] = _create_worker  # cache
-        return _create_worker
-
-    def _create_qt_worker(
-        self, gui, *args, **kwargs
-    ) -> FunctionWorker | GeneratorWorker:
-        """Create a worker object."""
-        worker = create_worker(
-            self._func.__get__(gui),
-            _ignore_errors=self._ignore_errors,
-            _start_thread=False,
-            *args,
-            **kwargs,
-        )
-        return worker
-
-    def _create_method(self, gui: BaseGui):
-        from ..fields import MagicField
-
-        @wraps(self)
-        def _create_worker(*args, **kwargs):
-            # create a worker object
-            worker = self._create_qt_worker(gui, *args, **kwargs)
-            is_generator = isinstance(worker, GeneratorWorker)
-
-            if self._progress:
-                # prepare progress bar
-                _pbar = self._progress["pbar"]
-                desc, total = self._normalize_desc_and_total(gui, *args, **kwargs)
-                if not is_generator:
-                    total = self._DEFAULT_TOTAL
-
-                # create progressbar widget (or any proper widget)
-                if _pbar is None:
-                    pbar = self._find_progressbar(gui, desc=desc, total=total)
-                elif isinstance(_pbar, MagicField):
-                    pbar = _pbar.get_widget(gui)
-                    if not isinstance(pbar, ProgressBar):
-                        raise TypeError(f"{_pbar.name} does not create a ProgressBar.")
-                    pbar.label = desc or _pbar.name
-                    pbar.max = total
-                else:
-                    pbar = _pbar
-                    pbar.set_description(desc)
-
-                worker.started.connect(init_pbar.__get__(pbar))
-
-            self._bind_callbacks(worker, gui)
-
-            # bind macro-recorder if exists
-            if self._recorder is not None:
-                worker.returned.connect(lambda _: self._recorder(gui, *args, **kwargs))
-
-            if self._progress:
-                if not getattr(pbar, "visible", False):
-                    # return the progressbar to the initial state
-                    worker.finished.connect(close_pbar.__get__(pbar))
-                if pbar.max != 0 and is_generator:
-                    worker.pbar = pbar  # avoid garbage collection
-                    worker.yielded.connect(increment.__get__(pbar))
-
-                if hasattr(pbar, "set_worker"):
-                    # if _SupportProgress object support set_worker
-                    pbar.set_worker(worker)
-
-            _obj: PushButtonPlus | Action = gui[self._func.__name__]
-            if _obj.running:
-                worker.errored.connect(
-                    partial(gui._error_mode.get_handler(), parent=gui)
-                )
-                if is_generator:
-                    worker.aborted.connect(
-                        gui._error_mode.wrap_handler(Aborted.raise_, parent=gui)
-                    )
+    def get_evaluator(
+        self,
+        key: int | slice | Iterable[int],
+        ns: dict[str, Any] = {},
+    ) -> Callable[[], Any]:
+        """Get the function that evaluate the macro lines at given indices."""
+        if isinstance(key, (int, slice)):
+            subset = self[key]
+        else:
+            subset = self.subset(key)
+        ns = dict(ns)
+        ui = self._gui_parent
+        ns.setdefault("ui", ui)
+        if (viewer := ui.parent_viewer) is not None:
+            ns.setdefault("viewer", viewer)
+        return lambda: subset.eval(ns)
 
-                worker.start()
+    def repeat_method(
+        self, index: int = -1, same_args: bool = False, wait: bool = False
+    ) -> None:
+        _object, _args, _kwargs = self[index].split_call()
+        _ui, *_attributes, _last = _object.split_getattr()
+        ui = self._gui_parent
+        assert _ui == ui._my_symbol
+        ins = ui
+        for attr in _attributes:
+            ins = getattr(ins, attr.name)
+
+        wdt: Clickable = ins[_last.name]
+        if not wait:
+            if same_args:
+                wdt.mgui.call_button.changed()
             else:
-                # If function is called from script, some events must get processed by
-                # the application while keep script stopping at each line of code.
-                app = use_app()
-                worker.returned.connect(app.process_events)
-                worker.started.connect(app.process_events)
-                if isinstance(worker, GeneratorWorker):
-                    worker.yielded.connect(app.process_events)
-                worker.run()
-
-            return None
-
-        return _create_worker
-
-    def _get_method_signature(self) -> inspect.Signature:
-        sig = self.__signature__
-        params = list(sig.parameters.values())[1:]
-        return sig.replace(parameters=params)
-
-    def _bind_callbacks(self, worker: FunctionWorker | GeneratorWorker, gui: BaseGui):
-        # bind callbacks
-        is_generator = isinstance(worker, GeneratorWorker)
-        for c in self.started._iter_as_method(gui):
-            worker.started.connect(c)
-        for c in self.returned._iter_as_method(gui):
-            worker.returned.connect(c)
-        worker.returned.connect(partial(Callback.catch, macro=gui.macro))
-        for c in self.errored._iter_as_method(gui):
-            worker.errored.connect(c)
-        for c in self.finished._iter_as_method(gui):
-            worker.finished.connect(c)
-
-        if is_generator:
-            for c in self.aborted._iter_as_method(gui):
-                worker.aborted.connect(c)
-            for c in self.yielded._iter_as_method(gui):
-                worker.yielded.connect(c)
-            worker.yielded.connect(partial(Callback.catch, macro=gui.macro))
-
-    @property
-    def __signature__(self) -> inspect.Signature:
-        """Get the signature of the bound function."""
-        return get_signature(self._func)
-
-    @__signature__.setter
-    def __signature__(self, sig: inspect.Signature) -> None:
-        """Update signature of the bound function."""
-        if not isinstance(sig, inspect.Signature):
-            raise TypeError(f"Cannot set type {type(sig)}.")
-        self._func.__signature__ = sig
-        return None
-
-    def _find_progressbar(self, gui: BaseGui, desc: str | None = None, total: int = 0):
-        """Find available progressbar. Create a new one if not found."""
-        from ..fields import MagicField
-
-        gui_id = id(gui)
-        if gui_id in self._progressbars:
-            _pbar = self._progressbars[gui_id]
+                wdt.changed()
         else:
-            for name, attr in gui.__class__.__dict__.items():
-                if isinstance(attr, MagicField):
-                    attr = attr.get_widget(gui)
-                if isinstance(attr, ProgressBar):
-                    _pbar = self._progressbars[gui_id] = attr
-                    if desc is None:
-                        desc = name
-                    break
+            if same_args:
+                wdt.mgui()
             else:
-                _pbar = self._progressbars[gui_id] = None
-                if desc is None:
-                    desc = "Progress"
-
-        if _pbar is None:
-            _pbar = self.__class__._DEFAULT_PROGRESS_BAR(max=total)
-            if isinstance(_pbar, Widget) and _pbar.parent is None:
-                # Popup progressbar as a splashscreen if it is not a child widget.
-                _pbar.native.setParent(gui.native, self.__class__._WINDOW_FLAG)
-                move_to_screen_center(_pbar.native)
-        else:
-            _pbar.max = total
-
-        # try to set description
-        if hasattr(_pbar, "set_description"):
-            _pbar.set_description(desc)
-        else:
-            _pbar.label = desc
-        return _pbar
-
-    def _normalize_desc_and_total(self, gui, *args, **kwargs):
-        _desc = self._progress["desc"]
-        _total = self._progress["total"]
-
-        all_args = None
-        # progress bar description
-        if callable(_desc):
-            arguments = self.__signature__.bind(gui, *args, **kwargs)
-            arguments.apply_defaults()
-            all_args = arguments.arguments
-            desc = _desc(**all_args)
-        else:
-            desc = str(_desc or self._func.__name__)
-
-        # total number of steps
-        if isinstance(_total, str):
-            if all_args is None:
-                arguments = self.__signature__.bind(gui, *args, **kwargs)
-                arguments.apply_defaults()
-                all_args = arguments.arguments
-            total = eval(_total, {}, all_args)
-        elif callable(_total):
-            total = _total(gui)
-        elif isinstance(_total, int):
-            total = _total
-        else:
-            raise TypeError("'total' must be int, callable or evaluatable string.")
-
-        return desc, total
+                raise NotImplementedError(
+                    "wait=True and same_args=False is not implemented yet."
+                )
+        return None
 
-    @property
-    def started(self) -> CallbackList[None]:
-        """Event that will be emitted on started."""
-        return self._callback_dict_["started"]
+    def _on_macro_added(self, expr=None):
+        line = str(self.args[-1])
+        if wdt := self.widget.native_macro:
+            wdt.append(line)
+        if wdt := self.widget.recorded_macro:
+            wdt.append(line)
+        if len(self) > self._max_lines:
+            del self[0]
 
-    @property
-    def returned(self) -> CallbackList[_R1]:
-        """Event that will be emitted on returned."""
-        return self._callback_dict_["returned"]
+    def _on_macro_popped(self, expr=None):
+        self._erase_last()
 
-    @property
-    def errored(self) -> CallbackList[Exception]:
-        """Event that will be emitted on errored."""
-        return self._callback_dict_["errored"]
+    def _erase_last(self):
+        if wdt := self.widget.native_macro:
+            wdt.erase_last()
+        if wdt := self.widget.recorded_macro:
+            wdt.erase_last()
 
-    @property
-    def yielded(self) -> CallbackList[_R1]:
-        """Event that will be emitted on yielded."""
-        if not self.is_generator:
-            raise TypeError(
-                f"Worker of non-generator function {self._func!r} does not have "
-                "yielded signal."
-            )
-        return self._callback_dict_["yielded"]
 
-    @property
-    def finished(self) -> CallbackList[None]:
-        """Event that will be emitted on finished."""
-        return self._callback_dict_["finished"]
+class DummyMacro(BaseMacro):
+    def insert(self, index, expr):
+        pass
 
-    @property
-    def aborted(self) -> CallbackList[None]:
-        """Event that will be emitted on aborted."""
-        if not self.is_generator:
-            raise TypeError(
-                f"Worker of non-generator function {self._func!r} does not have "
-                "aborted signal."
-            )
-        return self._callback_dict_["aborted"]
+    def _append_undo(self, undo) -> None:
+        return None
 
+    def _pop_undo(self) -> None:
+        return None
 
-def init_pbar(pbar: ProgressBarLike):
-    """Initialize progressbar."""
-    pbar.value = 0
-    pbar.show()
-    return None
-
-
-def close_pbar(pbar: ProgressBarLike):
-    """Close progressbar."""
-    if isinstance(pbar, ProgressBar):
-        _labeled_widget = pbar._labeled_widget()
-        if _labeled_widget is not None:
-            pbar = _labeled_widget
-    pbar.close()
-    return None
-
-
-def increment(pbar: ProgressBarLike):
-    """Increment progressbar."""
-    if pbar.value == pbar.max:
-        pbar.max = 0
-    else:
-        pbar.value += 1
-    return None
-
-
-class Callback:
-    """Callback object that can be recognized by thread_worker."""
-
-    def __init__(self, f: Callable[[], Any]):
-        if not callable(f):
-            raise TypeError(f"{f} is not callable.")
-        self._func = f
-
-    @staticmethod
-    def catch(out, macro: GuiMacro):
-        if isinstance(out, Callback):
-            with macro.blocked():
-                out._func()
-
-    def __call__(self, *args, **kwargs) -> Callback:
-        """Return a partial callback."""
-        return self.__class__(partial(self._func, *args, *kwargs))
-
-    def __get__(self, obj, type=None) -> Callback:
-        if obj is None:
-            return self
-        return self(obj)
+    def clear_undo_stack(self) -> None:
+        return None
```

### Comparing `magic-class-0.6.9/magicclass/widgets/__init__.py` & `magic_class-0.7.0rc0/magicclass/widgets/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-"""
-Advanced widgets for magic class GUI.
-These widgets are all compatible with the ``append`` method of Container widgets.
-"""
+"""magicgui-compatible widgets."""
 
 from magicgui.widgets import *  # to avoid importing both magicgui.widgets and magicclass.widgets
 
 from .containers import (
     ButtonContainer,
     GroupBoxContainer,
     FrameContainer,
@@ -24,47 +21,54 @@
 from .color import ColorEdit, ColorSlider
 from .misc import (
     OptionalWidget,
     ConsoleTextEdit,
     CheckButton,
     RangeSlider,
     FloatRangeSlider,
+    HistoryLineEdit,
+    HistoryFileEdit,
     SpreadSheet,
 )
 from .plot import Figure, SeabornFigure
 from .separator import Separator
-from .sequence import ListEdit, TupleEdit
 from .utils import FreeWidget
 from .logger import Logger
+from .codeedit import CodeEdit
+from .toggle_switch import ToggleSwitch
+from .eval import EvalLineEdit
 
 __all__ = [
     "ButtonContainer",
+    "CodeEdit",
     "ColorEdit",
     "ColorSlider",
     "ConsoleTextEdit",
     "CheckButton",
     "CollapsibleContainer",
     "DictWidget",
     "DraggableContainer",
+    "EvalLineEdit",
     "FrameContainer",
     "Figure",
     "FloatRangeSlider",
     "FreeWidget",
     "GroupBoxContainer",
     "HCollapsibleContainer",
-    "ListEdit",
+    "HistoryFileEdit",
+    "HistoryLineEdit",
     "ListContainer",
     "ListWidget",
     "Logger",
     "OptionalWidget",
     "RangeSlider",
     "SeabornFigure",
     "Separator",
     "ScrollableContainer",
     "SubWindowsContainer",
     "SplitterContainer",
     "SpreadSheet",
     "StackedContainer",
     "TabbedContainer",
+    "ToggleSwitch",
     "ToolBoxContainer",
-    "TupleEdit",
 ]
```

### Comparing `magic-class-0.6.9/magicclass/widgets/_mpl_canvas.py` & `magic_class-0.7.0rc0/magicclass/widgets/_mpl_canvas.py`

 * *Files identical despite different names*

### Comparing `magic-class-0.6.9/magicclass/widgets/color.py` & `magic_class-0.7.0rc0/magicclass/widgets/color.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     QLabel,
     QDoubleSpinBox,
     QSlider,
 )
 from qtpy.QtGui import QColor
 from qtpy.QtCore import Qt, Signal as QtSignal
 
-from magicgui.widgets._bases.value_widget import ValueWidget
+from magicgui.widgets.bases import ValueWidget
 from magicgui.backends._qtpy.widgets import QBaseValueWidget
 from magicgui.application import use_app
 from .utils import merge_super_sigs
 
 
 def rgba_to_qcolor(rgba: Iterable[float]) -> QColor:
     return QColor(*[int(round(255 * c)) for c in rgba])
@@ -37,32 +37,32 @@
 
 # modified from napari/_qt/widgets/qt_color_swatch.py
 class QColorSwatch(QFrame):
     colorChanged = QtSignal()
 
     def __init__(self, parent=None):
         super().__init__(parent)
-        self.setCursor(Qt.PointingHandCursor)
+        self.setCursor(Qt.CursorShape.PointingHandCursor)
         self._color: tuple[float, float, float, float] = (0.0, 0.0, 0.0, 0.0)
         self.colorChanged.connect(self._update_swatch_style)
         self.setMinimumWidth(40)
 
     def heightForWidth(self, w: int) -> int:
         return int(w * 0.667)
 
     def _update_swatch_style(self, _=None) -> None:
         rgba = f'rgba({",".join(str(int(x*255)) for x in self._color)})'
         self.setStyleSheet("QColorSwatch {background-color: " + rgba + ";}")
 
     def mouseReleaseEvent(self, event):
         """Show QColorPopup picker when the user clicks on the swatch."""
-        if event.button() == Qt.LeftButton:
+        if event.button() == Qt.MouseButton.LeftButton:
             initial = self.getQColor()
             dlg = QColorDialog(initial, self)
-            dlg.setOptions(QColorDialog.ShowAlphaChannel)
+            dlg.setOptions(QColorDialog.ColorDialogOption.ShowAlphaChannel)
             ok = dlg.exec_()
             if ok:
                 self.setColor(dlg.selectedColor())
 
     def getQColor(self) -> QColor:
         return rgba_to_qcolor(self._color)
 
@@ -165,16 +165,16 @@
 
 # See https://stackoverflow.com/questions/42820380/use-float-for-qslider
 class QDoubleSlider(QSlider):
     changed = QtSignal(float)
 
     def __init__(self, parent=None, decimals: int = 3):
         super().__init__(parent=parent)
-        self.scale = 10 ** decimals
-        self.setOrientation(Qt.Horizontal)
+        self.scale = 10**decimals
+        self.setOrientation(Qt.Orientation.Horizontal)
         self.valueChanged.connect(self.doubleValueChanged)
 
     def doubleValueChanged(self):
         value = float(super().value()) / self.scale
         self.changed.emit(value)
 
     def value(self):
@@ -234,15 +234,15 @@
         qlabel.setFixedWidth(15)
         qslider = QDoubleSlider()
         qslider.setMaximum(1.0)
         qslider.setSingleStep(0.001)
         qspinbox = QDoubleSpinBox()
         qspinbox.setMaximum(1.0)
         qspinbox.setSingleStep(0.001)
-        qspinbox.setAlignment(Qt.AlignRight)
+        qspinbox.setAlignment(Qt.AlignmentFlag.AlignRight)
 
         qspinbox.setButtonSymbols(QDoubleSpinBox.ButtonSymbols.NoButtons)
         qspinbox.setStyleSheet("background:transparent; border: 0;")
 
         qslider.changed.connect(qspinbox.setValue)
         qslider.changed.connect(lambda e: self.setColor(self.color()))
         qspinbox.editingFinished.connect(qslider.setValue)
@@ -274,23 +274,23 @@
             sl.setValue(c)
         self.colorChanged.emit(self.color())
 
 
 class _ColorEdit(QBaseValueWidget):
     _qwidget: QColorEdit
 
-    def __init__(self):
-        super().__init__(QColorEdit, "color", "setColor", "colorChanged")
+    def __init__(self, **kwargs):
+        super().__init__(QColorEdit, "color", "setColor", "colorChanged", **kwargs)
 
 
 class _ColorSlider(QBaseValueWidget):
     _qwidget: QColorSlider
 
-    def __init__(self):
-        super().__init__(QColorSlider, "color", "setColor", "colorChanged")
+    def __init__(self, **kwargs):
+        super().__init__(QColorSlider, "color", "setColor", "colorChanged", **kwargs)
 
 
 @merge_super_sigs
 class ColorEdit(ValueWidget):
     """
     A widget for editing colors.
```

### Comparing `magic-class-0.6.9/magicclass/widgets/containers.py` & `magic_class-0.7.0rc0/magicclass/widgets/containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
+
 from typing import Any, TypeVar, Callable
 import warnings
-from qtpy import QtWidgets as QtW
+from qtpy import QtWidgets as QtW, QtCore
 from qtpy.QtCore import Qt, QEvent, QSize
+
 from magicgui.application import use_app
-from magicgui.widgets._bases import Widget
-from magicgui.widgets._concrete import ContainerWidget
+from magicgui.widgets import Widget
+from magicgui.widgets._concrete import _LabeledWidget
 from magicgui.backends._qtpy.widgets import (
     QBaseWidget,
     Container as ContainerBase,
     MainWindow as MainWindowBase,
 )
+from magicgui.widgets.bases import ContainerWidget
 
 from .utils import merge_super_sigs
 
 # Container variations that is useful in making GUI designs better.
 
 C = TypeVar("C", bound=ContainerWidget)
 
@@ -42,24 +45,24 @@
     msg = "'btn_text' is deprecated and will be removed soon. Please use 'text'."
     warnings.warn(msg, DeprecationWarning)
 
 
 class _Splitter(ContainerBase):
     _qwidget: QtW.QWidget
 
-    def __init__(self, layout="vertical", scrollable: bool = False):
+    def __init__(self, layout="vertical", scrollable: bool = False, **kwargs):
         QBaseWidget.__init__(self, QtW.QWidget)
         # SetLayout is not supported for QSplitter.
         # Layout is just a dummy.
         self._splitter = QtW.QSplitter(self._qwidget)
         if layout == "horizontal":
-            self._splitter.setOrientation(Qt.Horizontal)
+            self._splitter.setOrientation(Qt.Orientation.Horizontal)
             self._layout = QtW.QHBoxLayout()
         else:
-            self._splitter.setOrientation(Qt.Vertical)
+            self._splitter.setOrientation(Qt.Orientation.Vertical)
             self._layout = QtW.QVBoxLayout()
 
         self._scroll_area = None
         self._qwidget.setLayout(QtW.QVBoxLayout())
         self._qwidget.layout().addWidget(self._splitter)
         self._qwidget.layout().setContentsMargins(0, 0, 0, 0)
 
@@ -75,15 +78,15 @@
     def _mgui_set_margins(self, margins: tuple[int, int, int, int]) -> None:
         pass
 
 
 class _ToolBox(ContainerBase):
     _qwidget: QtW.QToolBox
 
-    def __init__(self, layout="vertical", scrollable: bool = False):
+    def __init__(self, layout="vertical", scrollable: bool = False, **kwargs):
         QBaseWidget.__init__(self, QtW.QToolBox)
 
         if layout == "horizontal":
             msg = "Horizontal ToolBox is not implemented yet."
             warnings.warn(msg, UserWarning)
 
         self._layout = self._qwidget.layout()
@@ -98,213 +101,260 @@
                 widget.native.setParent(None)
                 break
         else:
             raise ValueError(f"Widget {widget.name} not found.")
 
 
 class _Tab(ContainerBase):
-    def __init__(self, layout="vertical", scrollable: bool = False):
+    def __init__(self, layout="vertical", scrollable: bool = False, **kwargs):
         QBaseWidget.__init__(self, QtW.QWidget)
 
         if layout == "horizontal":
             self._layout: QtW.QLayout = QtW.QHBoxLayout()
         else:
             self._layout = QtW.QVBoxLayout()
         self._scroll_area = None
         self._tab_widget = QtW.QTabWidget(self._qwidget)
         self._tab_widget.setLayout(self._layout)
         self._qwidget.setLayout(QtW.QVBoxLayout())
         self._qwidget.layout().addWidget(self._tab_widget)
         self._qwidget.layout().setContentsMargins(0, 0, 0, 0)
 
     def _mgui_insert_widget(self, position: int, widget: Widget):
-        self._tab_widget.insertTab(position, widget.native, widget.name)
+        if isinstance(widget, _LabeledWidget):
+            tabname = widget._label_widget.value
+        else:
+            tabname = widget.name or widget.label
+        self._tab_widget.insertTab(position, widget.native, tabname)
 
     def _mgui_remove_widget(self, widget: Widget):
         for i in range(self._tab_widget.count()):
             if self._tab_widget.widget(i) is widget.native:
                 self._tab_widget.removeTab(i)
                 widget.native.setParent(None)
                 break
         else:
             raise ValueError(f"Widget {widget.name} not found.")
 
 
 class _Stack(ContainerBase):
-    def __init__(self, layout="vertical", scrollable: bool = False):
+    def __init__(self, layout="vertical", scrollable: bool = False, **kwargs):
         QBaseWidget.__init__(self, QtW.QWidget)
 
         if layout == "horizontal":
             self._layout: QtW.QLayout = QtW.QHBoxLayout()
         else:
             self._layout = QtW.QVBoxLayout()
 
         self._stacked_widget = QtW.QStackedWidget(self._qwidget)
         self._stacked_widget.setContentsMargins(0, 0, 0, 0)
-        self._inner_widget = QtW.QWidget(self._qwidget)
+        self._inner_qwidget = QtW.QWidget(self._qwidget)
         self._qwidget.setLayout(self._layout)
         self._layout.addWidget(self._stacked_widget)
-        self._layout.addWidget(self._inner_widget)
+        self._layout.addWidget(self._inner_qwidget)
 
     def _mgui_insert_widget(self, position: int, widget: Widget):
         self._stacked_widget.insertWidget(position, widget.native)
 
     def _mgui_remove_widget(self, widget: Widget):
         self._stacked_widget.removeWidget(widget.native)
         widget.native.setParent(None)
 
 
 class _ScrollableContainer(ContainerBase):
-    def __init__(self, layout="vertical", scrollable: bool = False):
+    def __init__(self, layout="vertical", scrollable: bool = False, **kwargs):
         QBaseWidget.__init__(self, QtW.QWidget)
         self._scroll_area = QtW.QScrollArea(self._qwidget)
         if layout == "horizontal":
             self._layout: QtW.QLayout = QtW.QHBoxLayout()
-            self._layout.setAlignment(Qt.AlignCenter)
+            self._layout.setAlignment(Qt.AlignmentFlag.AlignCenter)
         else:
             self._layout = QtW.QVBoxLayout()
-            self._layout.setAlignment(Qt.AlignTop)
+            self._layout.setAlignment(Qt.AlignmentFlag.AlignTop)
 
         self._scroll_area.setWidgetResizable(True)
         self._scroll_area.setContentsMargins(0, 0, 0, 0)
-        self._inner_widget = QtW.QWidget(self._scroll_area)
-        self._inner_widget.setLayout(self._layout)
-        self._scroll_area.setWidget(self._inner_widget)
+        self._inner_qwidget = QtW.QWidget(self._scroll_area)
+        self._inner_qwidget.setLayout(self._layout)
+        self._scroll_area.setWidget(self._inner_qwidget)
 
         self._qwidget.setLayout(QtW.QVBoxLayout())
         self._qwidget.layout().addWidget(self._scroll_area)
         self._qwidget.layout().setContentsMargins(0, 0, 0, 0)
 
 
 class _WheelDisabledScrollArea(QtW.QScrollArea):
     def eventFilter(self, source, event: QEvent):
-        if event.type() == QEvent.Wheel:
+        if event.type() == QEvent.Type.Wheel:
             return True
         return super().eventFilter(source, event)
 
 
 class _DraggableContainer(ContainerBase):
-    def __init__(self, layout="vertical", scrollable: bool = False):
+    def __init__(self, layout="vertical", scrollable: bool = False, **kwargs):
         QBaseWidget.__init__(self, QtW.QWidget)
         self._scroll_area = _WheelDisabledScrollArea(self._qwidget)
         if layout == "horizontal":
             self._layout: QtW.QLayout = QtW.QHBoxLayout()
-            self._layout.setAlignment(Qt.AlignCenter)
+            self._layout.setAlignment(Qt.AlignmentFlag.AlignCenter)
         else:
             self._layout = QtW.QVBoxLayout()
-            self._layout.setAlignment(Qt.AlignTop)
+            self._layout.setAlignment(Qt.AlignmentFlag.AlignTop)
 
         self._scroll_area.setWidgetResizable(True)
         self._scroll_area.setContentsMargins(0, 0, 0, 0)
-        self._inner_widget = QtW.QWidget(self._scroll_area)
-        self._inner_widget.setLayout(self._layout)
-        self._scroll_area.setWidget(self._inner_widget)
+        self._inner_qwidget = QtW.QWidget(self._scroll_area)
+        self._inner_qwidget.setLayout(self._layout)
+        self._scroll_area.setWidget(self._inner_qwidget)
 
         self._qwidget.setLayout(QtW.QVBoxLayout())
         self._qwidget.layout().addWidget(self._scroll_area)
         self._qwidget.layout().setContentsMargins(0, 0, 0, 0)
         QtW.QScroller.grabGesture(
-            self._scroll_area, QtW.QScroller.LeftMouseButtonGesture
+            self._scroll_area, QtW.QScroller.ScrollerGestureType.LeftMouseButtonGesture
         )
 
-        self._scroll_area.setVerticalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
-        self._scroll_area.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
+        self._scroll_area.setVerticalScrollBarPolicy(
+            Qt.ScrollBarPolicy.ScrollBarAlwaysOff
+        )
+        self._scroll_area.setHorizontalScrollBarPolicy(
+            Qt.ScrollBarPolicy.ScrollBarAlwaysOff
+        )
 
 
 class _ButtonContainer(ContainerBase):
-    def __init__(self, layout="vertical", text="", scrollable: bool = False):
+    def __init__(self, layout="vertical", text="", scrollable: bool = False, **kwargs):
         QBaseWidget.__init__(self, QtW.QWidget)
         if layout == "horizontal":
             self._layout: QtW.QLayout = QtW.QHBoxLayout()
         else:
             self._layout = QtW.QVBoxLayout()
 
         self._qwidget = QtW.QPushButton()
-        self._inner_widget = QtW.QWidget()
-        self._inner_widget.setParent(self._qwidget, self._inner_widget.windowFlags())
-        self._inner_widget.setLayout(self._layout)
+        self._inner_qwidget = QtW.QWidget()
+        self._inner_qwidget.setParent(self._qwidget, self._inner_qwidget.windowFlags())
+        self._inner_qwidget.setLayout(self._layout)
 
         self._qwidget.setText(text)
-        self._qwidget.clicked.connect(lambda x: self._inner_widget.show())
+        self._qwidget.clicked.connect(lambda x: self._inner_qwidget.show())
 
 
 _VERTICAL_SETTING = {
     "expanded-arrow": Qt.ArrowType.DownArrow,
     "collapsed-arrow": Qt.ArrowType.RightArrow,
-    "align": Qt.AlignTop,
+    "align": Qt.AlignmentFlag.AlignTop,
     "text-align": "left",
+    "property-name": b"maximumHeight",
     "layout": QtW.QVBoxLayout,
 }
 _HORIZONTAL_SETTING = {
     "expanded-arrow": Qt.ArrowType.RightArrow,
     "collapsed-arrow": Qt.ArrowType.LeftArrow,
-    "align": Qt.AlignLeft,
+    "align": Qt.AlignmentFlag.AlignLeft,
     "text-align": "center",
+    "property-name": b"maximumWidth",
     "layout": QtW.QHBoxLayout,
 }
 
 
+# modified from superqt\collapsible\_collapsible.py
 class _QCollapsible(QtW.QWidget):
+    def __init__(self, parent: QtW.QWidget | None = None, layout: str = "vertical"):
+        super().__init__(parent)
+
+        if layout == "horizontal":
+            _layout: QtW.QLayout = QtW.QHBoxLayout()
+        else:
+            _layout = QtW.QVBoxLayout()
+
+        _layout.setContentsMargins(0, 0, 0, 0)
+        self.setLayout(_layout)
+        self._collapsed = True
+
+        self._animation = QtCore.QPropertyAnimation(self)
+        self._animation.setEasingCurve(QtCore.QEasingCurve.Type.InOutCubic)
+
+    def setPropertyName(self, name: bytes):
+        self._animation.setPropertyName(name)
+        self._animation.setStartValue(0)
+        self._animation.setDuration(300)
+        self._animation.setTargetObject(self)
+
     def sizeHint(self) -> QSize:
-        if self.isVisible():
+        if not self._collapsed:
             return super().sizeHint()
         else:
             return QSize(0, 0)
 
+    def collapsed(self):
+        return self._collapsed
+
+    def setCollapsed(self, col: bool):
+        if col:
+            direction = QtCore.QPropertyAnimation.Direction.Backward
+        else:
+            direction = QtCore.QPropertyAnimation.Direction.Forward
+        self._collapsed = col
+        _content_height = self.sizeHint().height() + 10
+        self._animation.setDirection(direction)
+        self._animation.setEndValue(_content_height)
+        self._animation.start()
+
 
 class _Collapsibles(ContainerBase):
     _setting: dict[str, Any]
 
-    def __init__(self, layout="vertical", text="", scrollable: bool = False):
-        QBaseWidget.__init__(self, QtW.QWidget)
-        if layout == "horizontal":
-            self._layout: QtW.QLayout = QtW.QHBoxLayout()
-        else:
-            self._layout = QtW.QVBoxLayout()
+    def __init__(
+        self,
+        layout: str = "vertical",
+        text: str = "",
+        scrollable: bool = False,
+        **kwargs,
+    ):
+        QBaseWidget.__init__(self, QtW.QWidget, **kwargs)
 
         self._get_setting()
         self._qwidget = QtW.QWidget()
         self._qwidget.setLayout(self._setting["layout"]())
-        self._inner_widget = _QCollapsible(self._qwidget)
-        self._inner_widget.setLayout(self._layout)
+        self._inner_qwidget = _QCollapsible(self._qwidget, layout)
+        self._inner_qwidget.setPropertyName(self._setting["property-name"])
+        self._layout = self._inner_qwidget.layout()
 
         self._qwidget.layout().setSpacing(0)
-        self._layout.setContentsMargins(0, 0, 0, 0)
 
         self._expand_btn = QtW.QToolButton(self._qwidget)
-        self._expand_btn.setToolButtonStyle(Qt.ToolButtonTextBesideIcon)
-        self._expand_btn.setArrowType(self._setting["collapsed-arrow"])
+        self._expand_btn.setToolButtonStyle(Qt.ToolButtonStyle.ToolButtonTextBesideIcon)
+        self._expand_btn.setArrowType(self._setting["expanded-arrow"])
         self._expand_btn.setText(text)
         self._expand_btn.setCheckable(True)
-        self._expand_btn.setChecked(False)
+        self._expand_btn.setChecked(True)
         self._expand_btn.setStyleSheet(
             f"""
             QToolButton {{
                 border: none;
                 text-align: {self._setting['text-align']};
                 }}
             """
         )
         self._expand_btn.clicked.connect(self._mgui_change_expand)
-        self._mgui_change_expand()
 
         self._qwidget.layout().addWidget(self._expand_btn, 0, self._setting["align"])
-        self._qwidget.layout().addWidget(self._inner_widget, 0, self._setting["align"])
+        self._qwidget.layout().addWidget(self._inner_qwidget, 0, self._setting["align"])
         self._qwidget.layout().setContentsMargins(0, 0, 0, 0)
 
     @property
     def collapsed(self) -> bool:
         return not self._expand_btn.isChecked()
 
     def _collapse(self):
-        self._inner_widget.setVisible(False)
+        self._inner_qwidget.setCollapsed(True)
         self._expand_btn.setArrowType(self._setting["collapsed-arrow"])
 
     def _expand(self):
-        self._inner_widget.setVisible(True)
+        self._inner_qwidget.setCollapsed(False)
         self._expand_btn.setArrowType(self._setting["expanded-arrow"])
 
     def _mgui_change_expand(self):
         if self.collapsed:
             self._collapse()
         else:
             self._expand()
@@ -341,29 +391,29 @@
         item = self.itemAt(event.pos())
         dest = self.itemWidget(item)
         if dest is None:
             self.setItemWidget(item, widget)
 
 
 class _ListContainer(ContainerBase):
-    def __init__(self, layout="vertical", scrollable: bool = False):
+    def __init__(self, layout="vertical", scrollable: bool = False, **kwargs):
         QBaseWidget.__init__(self, QtW.QWidget)
         self._listwidget = _QListWidget(self._qwidget)
         if layout == "horizontal":
             self._layout: QtW.QLayout = QtW.QHBoxLayout()
         else:
             self._layout = QtW.QVBoxLayout()
         self._layout.setContentsMargins(0, 0, 0, 0)
         self._layout.addWidget(self._listwidget)
         self._qwidget.setLayout(self._layout)
 
         if layout == "horizontal":
-            self._listwidget.setFlow(QtW.QListView.LeftToRight)
+            self._listwidget.setFlow(QtW.QListView.Flow.LeftToRight)
         else:
-            self._listwidget.setFlow(QtW.QListView.TopToBottom)
+            self._listwidget.setFlow(QtW.QListView.Flow.TopToBottom)
 
     def _mgui_insert_widget(self, position: int, widget: Widget):
         item = QtW.QListWidgetItem(self._listwidget)
         item.setSizeHint(widget.native.sizeHint())
         self._listwidget.insertItem(position, item)
         self._listwidget.setItemWidget(item, widget.native)
 
@@ -381,18 +431,20 @@
         widget.native.setParent(None)
 
 
 class _SubWindowsContainer(ContainerBase):
     # The close button in QMdiArea completely deletes the sub window widget. This accident
     # can be avoided by defining a custom window flag.
     _NoCloseButtonFlag = (
-        Qt.CustomizeWindowHint | Qt.WindowTitleHint | Qt.WindowMinMaxButtonsHint
+        Qt.WindowType.CustomizeWindowHint
+        | Qt.WindowType.WindowTitleHint
+        | Qt.WindowType.WindowMinMaxButtonsHint
     )
 
-    def __init__(self, layout="vertical", scrollable: bool = False):
+    def __init__(self, layout="vertical", scrollable: bool = False, **kwargs):
         QBaseWidget.__init__(self, QtW.QWidget)
         self._mdiarea = QtW.QMdiArea(self._qwidget)
         if layout == "horizontal":
             self._layout: QtW.QLayout = QtW.QHBoxLayout()
         else:
             self._layout = QtW.QVBoxLayout()
 
@@ -405,39 +457,39 @@
 
     def _mgui_remove_widget(self, widget: Widget):
         self._mdiarea.removeSubWindow(widget.native)
         widget.native.setParent(None)
 
 
 class _GroupBoxContainer(ContainerBase):
-    def __init__(self, layout="vertical", scrollable: bool = False):
+    def __init__(self, layout="vertical", scrollable: bool = False, **kwargs):
         QBaseWidget.__init__(self, QtW.QWidget)
 
         # To precisely control margins, _layout should not be set to the QGroupBox widget.
         self._groupbox = QtW.QGroupBox(self._qwidget)
         if layout == "horizontal":
             self._layout: QtW.QLayout = QtW.QHBoxLayout()
         else:
             self._layout = QtW.QVBoxLayout()
 
-        self._inner_widget = QtW.QWidget(self._groupbox)
-        self._inner_widget.setLayout(self._layout)
+        self._inner_qwidget = QtW.QWidget(self._groupbox)
+        self._inner_qwidget.setLayout(self._layout)
         self._groupbox.setLayout(QtW.QHBoxLayout())
-        self._groupbox.layout().addWidget(self._inner_widget)
+        self._groupbox.layout().addWidget(self._inner_qwidget)
 
         self._qwidget.setLayout(QtW.QVBoxLayout())
         self._qwidget.layout().addWidget(self._groupbox)
         self._qwidget.layout().setContentsMargins(0, 0, 0, 0)
 
     def _set_title(self, title: str):
         self._groupbox.setTitle(title)
 
 
 class _FrameContainer(_GroupBoxContainer):
-    def __init__(self, layout="vertical", scrollable: bool = False):
+    def __init__(self, layout="vertical", scrollable: bool = False, **kwargs):
         super().__init__(layout=layout)
         self._groupbox.setTitle("")
 
 
 # Container Widgets
 
 
@@ -460,33 +512,41 @@
 
 
 @wrap_container(base=_Tab)
 class TabbedContainer(ContainerWidget):
     """A tab categorized Container Widget."""
 
     @property
+    def native_tab_widget(self) -> QtW.QTabWidget:
+        return self._widget._tab_widget
+
+    @property
     def current_index(self):
-        return self._widget._tab_widget.currentIndex()
+        return self.native_tab_widget.currentIndex()
 
     @current_index.setter
     def current_index(self, index: int):
-        self._widget._tab_widget.setCurrentIndex(index)
+        self.native_tab_widget.setCurrentIndex(index)
 
 
 @wrap_container(base=_Stack)
 class StackedContainer(ContainerWidget):
     """A stacked Container Widget"""
 
     @property
+    def native_stacked_widget(self) -> QtW.QStackedWidget:
+        return self._widget._stacked_widget
+
+    @property
     def current_index(self):
-        return self._widget._stacked_widget.currentIndex()
+        return self.native_stacked_widget.currentIndex()
 
     @current_index.setter
     def current_index(self, index: int):
-        self._widget._stacked_widget.setCurrentIndex(index)
+        self.native_stacked_widget.setCurrentIndex(index)
 
 
 @wrap_container(base=_ScrollableContainer)
 class ScrollableContainer(ContainerWidget):
     """A scrollable Container Widget."""
```

### Comparing `magic-class-0.6.9/magicclass/widgets/logger.py` & `magic_class-0.7.0rc0/magicclass/widgets/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,56 @@
 from __future__ import annotations
 import sys
 import logging
 from pathlib import Path
-from contextlib import contextmanager
+from contextlib import contextmanager, suppress
 from qtpy import QtWidgets as QtW, QtGui, QtCore
 from qtpy.QtCore import Qt, Signal
 from magicgui.backends._qtpy.widgets import QBaseWidget
 from magicgui.widgets import Widget
 import logging
 from typing import TYPE_CHECKING, Any, Union, overload
-from ..utils import rst_to_html
 
-try:
-    import numpy as np
-    import matplotlib as mpl
-    import matplotlib.pyplot as plt
-    from matplotlib.backends.backend_agg import FigureCanvasAgg
-
-    FigureCanvas = FigureCanvasAgg
-    MATPLOTLIB_AVAILABLE = True
-
-except ImportError:
-    MATPLOTLIB_AVAILABLE = False
+from magicclass.utils import rst_to_html
 
 if TYPE_CHECKING:
     import numpy as np
-    from matplotlib.figure import Figure
-    from PIL import Image
+    from matplotlib.figure import Figure as mpl_Figure
 
 # See https://stackoverflow.com/questions/28655198/best-way-to-display-logs-in-pyqt
 
 
+# Variable "FigureCanvas" should globally updated to plot figure inside the logger
+# However, importing FigureCanvasAgg should be done lazily. Here's how to hack
+# this procedure.
+class FigureCanvasType:
+    def __init__(self):
+        self._canvas_type = None
+
+    @property
+    def FigureCanvasAgg(self):
+        if self._canvas_type is None:
+            from matplotlib.backends.backend_agg import FigureCanvasAgg
+
+            self._canvas_type = FigureCanvasAgg
+        return self._canvas_type
+
+    def __getattr__(self, name):
+        return getattr(self.FigureCanvasAgg, name)
+
+    def __call__(self, *args: Any, **kwds: Any) -> Any:
+        return self.FigureCanvasAgg(*args, **kwds)
+
+
+FigureCanvas = FigureCanvasType()
+
+
 class Output:
+    """Logger output types."""
+
     TEXT = 0
     HTML = 1
     IMAGE = 2
 
 
 Printable = Union[str, QtGui.QImage]
 
@@ -75,26 +90,31 @@
             cursor = self.textCursor()
             cursor.insertImage(obj)
             self.insertPlainText("\n\n")
             self.verticalScrollBar().setValue(self.verticalScrollBar().maximum())
         else:
             raise TypeError("Wrong type.")
         self._post_append()
+        return None
 
     def appendText(self, text: str):
         """Append text in the main thread."""
-        self.process.emit((Output.TEXT, text))
+        self._emit_output(Output.TEXT, text)
 
     def appendHtml(self, html: str):
         """Append HTML in the main thread."""
-        self.process.emit((Output.HTML, html))
+        self._emit_output(Output.HTML, html)
 
     def appendImage(self, qimage: QtGui.QImage):
         """Append image in the main thread."""
-        self.process.emit((Output.IMAGE, qimage))
+        self._emit_output(Output.IMAGE, qimage)
+
+    def _emit_output(self, output: int, obj: Printable):
+        with suppress(RuntimeError):
+            self.process.emit((output, obj))
 
     def _post_append(self):
         """Check the history length."""
         if self._n_lines < self._max_history:
             self._n_lines += 1
             return None
         cursor = self.textCursor()
@@ -122,15 +142,15 @@
             menu.addAction("Copy Image", lambda: self._copy_image(name))
             menu.addAction("Save Image As...", lambda: self._save_image(name))
             menu.addSeparator()
             return menu
 
     def _copy_image(self, name):
         image = self._get_image(name)
-        QtW.QApplication.clipboard().setImage(image)
+        return QtW.QApplication.clipboard().setImage(image)
 
     def _save_image(self, name, format="PNG"):
         """Shows a save dialog for the ImageResource with 'name'."""
         dialog = QtW.QFileDialog(self, "Save Image")
         dialog.setAcceptMode(QtW.QFileDialog.AcceptMode.AcceptSave)
         dialog.setDefaultSuffix(format.lower())
         if self._last_save_path is None:
@@ -138,14 +158,15 @@
         dialog.setDirectory(str(self._last_save_path))
         dialog.setNameFilter(f"{format} file (*.{format.lower()})")
         if dialog.exec_():
             filename = dialog.selectedFiles()[0]
             image = self._get_image(name)
             image.save(filename, format)
             self._last_save_path = Path(filename).parent
+        return None
 
     def _get_image(self, name):
         """Returns the QImage stored as the ImageResource with 'name'."""
         document = self.document()
         image = document.resource(
             QtGui.QTextDocument.ResourceType.ImageResource, QtCore.QUrl(name)
         )
@@ -212,18 +233,21 @@
     current_logger: Logger | None = None
 
     def __init__(self):
         logging.Handler.__init__(self)
         Widget.__init__(
             self, widget_type=QBaseWidget, backend_kwargs={"qwidg": QtLogger}
         )
+        self.native: QtLogger
 
     def emit(self, record):
+        """Handle the logging event."""
         msg = self.format(record)
         self.print(msg)
+        return None
 
     def clear(self):
         """Clear all the histories."""
         self.native.clear()
         return None
 
     def print(self, *msg, sep=" ", end="\n"):
@@ -284,15 +308,15 @@
         vmax=None,
         cmap=None,
         norm=None,
         width=None,
         height=None,
     ) -> None:
         """Print an array as an image in the logger widget. Can be a path."""
-        from magicgui import _mpl_image
+        from magicgui.widgets._image import _mpl_image
 
         img = _mpl_image.Image()
 
         img.set_data(arr)
         img.set_clim(vmin, vmax)
         img.set_cmap(cmap)
         img.set_norm(norm)
@@ -305,35 +329,42 @@
         if width is None and height is None:
             if w / 3 > h / 2:
                 width = 360
             else:
                 height = 240
 
         if width is None:
-            image = image.scaledToHeight(height, QtCore.Qt.SmoothTransformation)
+            image = image.scaledToHeight(
+                height, Qt.TransformationMode.SmoothTransformation
+            )
         else:
-            image = image.scaledToWidth(width, QtCore.Qt.SmoothTransformation)
+            image = image.scaledToWidth(
+                width, Qt.TransformationMode.SmoothTransformation
+            )
 
         self.native.appendImage(image)
         return None
 
-    def print_figure(self, fig: Figure) -> None:
+    def print_figure(self, fig: mpl_Figure) -> None:
         """Print matplotlib Figure object like inline plot."""
+        import numpy as np
+
         fig.canvas.draw()
         data = np.asarray(fig.canvas.renderer.buffer_rgba(), dtype=np.uint8)
         self.print_image(data)
 
         return None
 
     def write(self, msg) -> None:
+        """Handle the print event."""
         self.print(msg, end="")
         return None
 
     def flush(self):
-        pass
+        """Do nothing."""
 
     def close(self) -> None:
         # This method collides between magicgui.widgets.Widget and logging.Handler.
         # Since the close method in Widget is rarely used, here just call the latter.
         return logging.Handler.close(self)
 
     @contextmanager
@@ -342,46 +373,60 @@
         try:
             sys.stdout = self
             yield self
         finally:
             sys.stdout = sys.__stdout__
 
     @contextmanager
-    def set_logger(self, name=None):
+    def set_logger(self, name=None, clear: bool = True):
         """A context manager for logging things in this widget."""
+        logger = logging.getLogger(name)
+        current_handler = logger.handlers
         try:
-            logging.getLogger(name).addHandler(self)
+            if clear:
+                for hd in current_handler:
+                    logger.removeHandler(hd)
+            logger.addHandler(self)
             yield self
         finally:
-            logging.getLogger(name).removeHandler(self)
+            logger.removeHandler(self)
+            if clear:
+                for hd in current_handler:
+                    logger.addHandler(hd)
 
     @overload
     def set_plt(self, style: str | None) -> None:
         ...
 
     @overload
     def set_plt(self, rc_context: dict[str, Any]) -> None:
         ...
 
     @contextmanager
     def set_plt(self, style: str = None, rc_context: dict[str, Any] = {}):
         """A context manager for inline plot in the logger widget."""
-        if not MATPLOTLIB_AVAILABLE:
+        try:
+            import matplotlib as mpl
+            import matplotlib.pyplot as plt
+        except ImportError:
             yield self
             return None
         self.__class__.current_logger = self
 
         if isinstance(style, dict):
             if rc_context:
                 raise TypeError("style must be str.")
             rc_context = style
             style = None
 
         if style is None:
-            style = self._get_proper_plt_style()
+            try:
+                style = self._get_proper_plt_style()
+            except RuntimeError:
+                style = "default"
 
         backend = mpl.get_backend()
         show._called = False
         try:
             mpl.use("module://magicclass.widgets.logger")
             with plt.style.context(style), plt.rc_context(rc_context):
                 yield self
@@ -389,14 +434,16 @@
             if not show._called:
                 show()
             self.__class__.current_logger = None
             mpl.use(backend)
         return None
 
     def _get_proper_plt_style(self) -> dict[str, Any]:
+        import matplotlib.pyplot as plt
+
         color = self._widget._qwidget._get_background_color()[:3]
         is_dark = sum(color) < 382.5  # 255*3/2
         if is_dark:
             params = plt.style.library["dark_background"]
         else:
             keys = plt.style.library["dark_background"].keys()
             with plt.style.context("default"):
@@ -411,14 +458,15 @@
 
 
 # The plt.show function will be overwriten to this.
 # Modified from matplotlib_inline (BSD 3-Clause "New" or "Revised" License)
 # https://github.com/ipython/matplotlib-inline
 def show(close=True, block=None):
     logger = Logger.current_logger
+    import matplotlib.pyplot as plt
     from matplotlib._pylab_helpers import Gcf
 
     try:
         for figure_manager in Gcf.get_all_fig_managers():
             logger.print_figure(figure_manager)
     finally:
         show._called = True
```

### Comparing `magic-class-0.6.9/magicclass/widgets/misc.py` & `magic_class-0.7.0rc0/magicclass/widgets/misc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 from __future__ import annotations
+from pathlib import Path
 import sys
 from typing import (
     TYPE_CHECKING,
     Generic,
     Iterable,
     MutableSequence,
     Any,
     TypeVar,
 )
 from typing_extensions import _AnnotatedAlias, get_args
 from psygnal import Signal
-from qtpy import QtWidgets as QtW
-from qtpy.QtGui import QTextCursor
+from qtpy import QtWidgets as QtW, QtGui
 from qtpy.QtCore import Qt
-from magicgui.signature import split_annotated_type
 from magicgui.widgets import (
     PushButton,
     TextEdit,
     Table,
     Container,
     CheckBox,
+    FileEdit,
     create_widget,
 )
 from magicgui.application import use_app
 from magicgui.widgets import LineEdit
-from magicgui.widgets._bases.value_widget import ValueWidget, UNSET
+from magicgui.types import FileDialogMode
+from magicgui.widgets.bases import ValueWidget
+from magicgui.types import Undefined
 from magicgui.backends._qtpy.widgets import (
     QBaseWidget,
+    QBaseStringWidget,
     LineEdit as BaseLineEdit,
 )
 from .utils import FreeWidget, merge_super_sigs
+from magicclass.signature import split_annotated_type
 
 if TYPE_CHECKING:
     from qtpy.QtWidgets import QTextEdit
     from superqt import QLabeledRangeSlider
 
 
 if sys.platform == "win32":
@@ -58,19 +62,19 @@
     options : dict, optional
         Widget options of the inner value widget.
     """
 
     def __init__(
         self,
         inner_widget: type[ValueWidget] | None = None,
-        text: str = None,
-        layout="vertical",
-        nullable=True,
-        value=UNSET,
-        options=None,
+        text: str | None = None,
+        layout: str = "vertical",
+        nullable: bool = True,
+        value=Undefined,
+        options: dict | None = None,
         **kwargs,
     ):
         if text is None:
             text = "Use default value"
         if options is None:
             options = {}
         self._checkbox = CheckBox(text=text, value=True)
@@ -116,15 +120,15 @@
         if not self._checkbox.value:
             return self._inner_value_widget.value
         else:
             return None
 
     @value.setter
     def value(self, v: Any) -> None:
-        if v is None or v is UNSET:
+        if v is None or v is Undefined:
             self._checkbox.value = True
             self._inner_value_widget.visible = False
         else:
             self._inner_value_widget.value = v
             self._checkbox.value = False
             self._inner_value_widget.visible = True
 
@@ -142,21 +146,22 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         from qtpy.QtGui import QFont, QTextOption
 
         self.native: QTextEdit
         font = QFont(_FONT)
-        font.setStyleHint(QFont.Monospace)
+        font.setStyleHint(QFont.StyleHint.Monospace)
         font.setFixedPitch(True)
         self.native.setFont(font)
-        self.native.setWordWrapMode(QTextOption.NoWrap)
+        self.native.setWordWrapMode(QTextOption.WrapMode.NoWrap)
 
         # set tab width
         self.tab_size = 4
+        self._highlight = None
 
     @property
     def tab_size(self):
         metrics = self.native.fontMetrics()
         return self.native.tabStopWidth() // metrics.width(" ")
 
     @tab_size.setter
@@ -167,37 +172,45 @@
     def append(self, text: str):
         """Append new text."""
         self.native.append(text)
 
     def erase_last(self):
         """Erase the last line."""
         cursor = self.native.textCursor()
-        cursor.movePosition(QTextCursor.End)
-        cursor.select(QTextCursor.LineUnderCursor)
+        cursor.movePosition(QtGui.QTextCursor.MoveOperation.End)
+        cursor.select(QtGui.QTextCursor.SelectionType.LineUnderCursor)
         cursor.removeSelectedText()
         cursor.deletePreviousChar()
         self.native.setTextCursor(cursor)
 
     def erase_first(self):
         """Erase the first line."""
         cursor = self.native.textCursor()
-        cursor.movePosition(QTextCursor.Start)
-        cursor.select(QTextCursor.LineUnderCursor)
+        cursor.movePosition(QtGui.QTextCursor.MoveOperation.Start)
+        cursor.select(QtGui.QTextCursor.SelectionType.LineUnderCursor)
         cursor.removeSelectedText()
-        cursor.movePosition(QTextCursor.Down)
+        cursor.movePosition(QtGui.QTextCursor.MoveOperation.Down)
         cursor.deletePreviousChar()
-        cursor.movePosition(QTextCursor.End)
+        cursor.movePosition(QtGui.QTextCursor.MoveOperation.End)
         self.native.setTextCursor(cursor)
 
     @property
     def selected(self) -> str:
         """Return selected string."""
         cursor = self.native.textCursor()
         return cursor.selectedText().replace("\u2029", "\n")
 
+    def syntax_highlight(self, lang: str = "python", theme: str = "default"):
+        """Highlight syntax."""
+        from superqt.utils import CodeSyntaxHighlight
+
+        highlight = CodeSyntaxHighlight(self.native.document(), lang, theme=theme)
+        self._highlight = highlight
+        return None
+
 
 class CheckButton(PushButton):
     """A checkable button."""
 
     def __init__(self, text: str | None = None, **kwargs):
         super().__init__(text=text, **kwargs)
         self.native.setCheckable(True)
@@ -212,15 +225,15 @@
         return int(value)
 
     def _pre_set_hook(self, value):
         return str(value)
 
 
 class IntEdit(LineEdit):
-    def __init__(self, value=UNSET, **kwargs):
+    def __init__(self, value=Undefined, **kwargs):
         app = use_app()
         assert app.native
         ValueWidget.__init__(
             self,
             value=value,
             widget_type=QIntEdit,
             **kwargs,
@@ -236,15 +249,15 @@
         return float(value)
 
     def _pre_set_hook(self, value):
         return str(value)
 
 
 class FloatEdit(LineEdit):
-    def __init__(self, value=UNSET, **kwargs):
+    def __init__(self, value=Undefined, **kwargs):
         app = use_app()
         assert app.native
         ValueWidget.__init__(
             self,
             value=value,
             widget_type=QFloatEdit,
             **kwargs,
@@ -275,29 +288,29 @@
     See https://github.com/napari/magicgui/pull/337.
     """
 
     changed = Signal(tuple)
 
     def __init__(
         self,
-        value=UNSET,
+        value=Undefined,
         min=0,
         max=1000,
         orientation: str = "horizontal",
         nullable: bool = True,
         **kwargs,
     ):
         sl = self._construct_qt()
         sl.setMinimum(min)
         sl.setMaximum(max)
         sl.valueChanged.connect(self.changed)
         if orientation == "horizontal":
-            sl.setOrientation(Qt.Horizontal)
+            sl.setOrientation(Qt.Orientation.Horizontal)
         elif orientation == "vertical":
-            sl.setOrientation(Qt.Vertical)
+            sl.setOrientation(Qt.Orientation.Vertical)
         else:
             raise ValueError(
                 "Only horizontal and vertical orientation are currently supported"
             )
         self._slider = sl
         super().__init__(
             value=value,
@@ -371,14 +384,21 @@
 
         sl = QLabeledDoubleRangeSlider()
         sl.setHandleLabelPosition(QLabeledDoubleRangeSlider.LabelPosition.LabelsAbove)
         sl.setEdgeLabelMode(QLabeledDoubleRangeSlider.EdgeLabelMode.NoLabel)
         return sl
 
 
+# magicgui>=0.6.0 has its own range sliders.
+try:
+    from magicgui.widgets import RangeSlider, FloatRangeSlider
+except ImportError:
+    pass
+
+
 class _QtSpreadSheet(QtW.QTabWidget):
     def __init__(self):
         super().__init__()
         self.setMovable(True)
         self._n_table = 0
         self.tabBar().tabBarDoubleClicked.connect(self.editTabBarLabel)
         self.tabBar().setContextMenuPolicy(Qt.CustomContextMenu)
@@ -498,7 +518,94 @@
         return self._read_only
 
     @read_only.setter
     def read_only(self, v: bool):
         for table in self._tables:
             table.read_only = v
         self._read_only = v
+
+
+class _QEditableComboBox(QtW.QComboBox):
+    def __init__(self, parent: QtW.QWidget | None = None) -> None:
+        super().__init__(parent)
+        self.setEditable(True)
+        self.setSizePolicy(
+            QtW.QSizePolicy.Policy.Expanding, QtW.QSizePolicy.Policy.Fixed
+        )
+
+    def keyPressEvent(self, event: QtGui.QKeyEvent):
+        if event.key() in (Qt.Key.Key_Down, Qt.Key.Key_Up):
+            self.showPopup()
+        super().keyPressEvent(event)
+
+    def _append_history(self, text: str):
+        i = self.findText(text)
+        if i >= 0:
+            self.removeItem(i)
+        return self.addItem(text)
+
+
+class QHistoryLineEdit(QBaseStringWidget):
+    _qwidget: _QEditableComboBox
+
+    def __init__(self, **kwargs):
+        super().__init__(
+            _QEditableComboBox,
+            "currentText",
+            "setCurrentText",
+            "currentTextChanged",
+            **kwargs,
+        )
+
+
+class HistoryLineEdit(LineEdit):
+    def __init__(self, value=Undefined, **kwargs):
+        app = use_app()
+        assert app.native
+        ValueWidget.__init__(
+            self,
+            value=value,
+            widget_type=QHistoryLineEdit,
+            **kwargs,
+        )
+
+    def append_history(self, text: str):
+        """Append new history to the line edit"""
+        return self.native._append_history(text)
+
+
+class HistoryFileEdit(FileEdit):
+    def __init__(
+        self,
+        mode: FileDialogMode = FileDialogMode.EXISTING_FILE,
+        filter=None,
+        nullable=False,
+        **kwargs,
+    ):
+        value = kwargs.pop("value", None)
+        if value is None:
+            value = ""
+        self.line_edit = HistoryLineEdit(value=value)
+        self.choose_btn = PushButton()
+        self.mode = mode  # sets the button text too
+        self.filter = filter
+        self._nullable = nullable
+        kwargs["widgets"] = [self.line_edit, self.choose_btn]
+        kwargs["labels"] = False
+        kwargs["layout"] = "horizontal"
+        Container.__init__(self, **kwargs)
+        self.margins = (0, 0, 0, 0)
+        self._show_file_dialog = use_app().get_obj("show_file_dialog")
+        self.choose_btn.changed.disconnect()
+        self.line_edit.changed.disconnect()
+        self.choose_btn.changed.connect(self._on_choose_clicked)
+        self.line_edit.changed.connect(lambda: self.changed.emit(self.value))
+
+    def _on_choose_clicked(self):
+        super()._on_choose_clicked()
+        val = self.value
+        if isinstance(val, (str, Path)):
+            val = str(val)
+            if val != ".":
+                self.line_edit.append_history(val)
+        elif isinstance(val, tuple):
+            self.line_edit.append_history("; ".join(map(str, val)))
```

### Comparing `magic-class-0.6.9/magicclass/widgets/plot.py` & `magic_class-0.7.0rc0/magicclass/widgets/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,14 +223,20 @@
         self, *args, **kwargs
     ) -> tuple[ArrayLike | list[ArrayLike], ArrayLike, list | list[list]]:
         out = self.ax.hist(*args, **kwargs)
         self.draw()
         return out
 
     @_inject_mpl_docs
+    def bar(self, *args, **kwargs) -> None:
+        bars = self.ax.bar(*args, **kwargs)
+        self.draw()
+        return bars
+
+    @_inject_mpl_docs
     def text(self, *args, **kwargs) -> Text:
         text = self.ax.text(*args, **kwargs)
         self.draw()
         return text
 
     @_inject_mpl_docs
     def quiver(self, *args, data=None, **kwargs) -> Quiver:
@@ -351,14 +357,20 @@
         return self.ax.twinx()
 
     @_inject_mpl_docs
     def twiny(self) -> Axes:
         return self.ax.twiny()
 
     @_inject_mpl_docs
+    def grid(self, *args, **kwargs) -> None:
+        self.ax.grid(*args, **kwargs)
+        self.draw()
+        return None
+
+    @_inject_mpl_docs
     def box(self, on=None) -> None:
         if on is None:
             on = not self.ax.get_frame_on()
         self.ax.set_frame_on(on)
         return None
 
     @_inject_mpl_docs
```

### Comparing `magic-class-0.6.9/magicclass/widgets/pywidgets/__init__.py` & `magic_class-0.7.0rc0/magicclass/widgets/pywidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `magic-class-0.6.9/magicclass/widgets/pywidgets/dict.py` & `magic_class-0.7.0rc0/magicclass/widgets/pywidgets/tree.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,157 +1,153 @@
 from __future__ import annotations
 from typing import Any, Iterable, MutableMapping
-from qtpy.QtWidgets import QTableWidget, QTableWidgetItem
+from qtpy.QtWidgets import QTreeWidget, QTreeWidgetItem
 
 from .object import BaseWidget, ContextMenuMixin, PyObjectBound
 
+# WIP!
 
-class DictWidget(BaseWidget, MutableMapping):
+
+class DictTreeWidget(BaseWidget, MutableMapping):
     def __init__(self, value=None, **kwargs):
         super().__init__(**kwargs)
 
-        self._tablewidget = PyTableWidget(self.native)
-        self._tablewidget.setParentWidget(self)
-        self._tablewidget.setEditTriggers(QTableWidget.NoEditTriggers)
-        self._tablewidget.verticalHeader().setDefaultSectionSize(30)
+        self._treewidget = PyTreeWidget(self.native)
+        self._treewidget.setParentWidget(self)
         self._dict: dict[str, int] = {}  # mapping from key to row
 
-        self.set_widget(self._tablewidget)
+        self.set_widget(self._treewidget)
 
-        @self._tablewidget.itemDoubleClicked.connect
-        def _(item: PyTableWidgetItem):
+        @self._treewidget.itemDoubleClicked.connect
+        def _(item: PyTreeWidgetItem):
             type_ = type(item.obj)
             callbacks = self._callbacks.get(type_, [])
             self.running = True
             try:
                 for callback in callbacks:
                     try:
-                        callback(item.obj, self._tablewidget.row(item))
+                        callback(item.obj, item)
                     except TypeError:
                         callback(item.obj)
             finally:
                 self.running = False
 
         if value is not None:
             self.update(dict(value))
 
     def __len__(self) -> int:
-        return self._tablewidget.rowCount()
+        return self._treewidget.rowCount()
 
     @property
     def value(self) -> dict[str, Any]:
-        return {k: self._tablewidget.item(row, 0) for k, row in self._dict}
+        return {k: self._treewidget.item(row, 0) for k, row in self._dict}
 
     def __getitem__(self, k: str) -> Any:
         row = self._dict[k]
-        return self._tablewidget.item(row, 0).obj
+        return self._treewidget.item(row, 0).obj
 
     def __setitem__(self, k: str, obj: Any) -> None:
         if not isinstance(k, str):
             raise ValueError("Can only use str type as keys.")
 
         if k in self._dict.keys():
             row = self._dict[k]
         else:
             row = len(self)
             self._dict[k] = row
-            self._tablewidget.insertRow(row)
-            if row == 0:
-                self._tablewidget.insertColumn(0)
-                self._tablewidget.setHorizontalHeaderItem(0, QTableWidgetItem("value"))
-            key_item = QTableWidgetItem(k)
-            self._tablewidget.setVerticalHeaderItem(row, key_item)
+            key_item = QTreeWidgetItem(k)
 
         name = self._delegates.get(type(obj), str)(obj)
-        value_item = PyTableWidgetItem(obj, name)
+        value_item = PyTreeWidgetItem(obj, name)
         tooltip = self._tooltip.get(type(obj), str)(obj)
         value_item.setToolTip(tooltip)
-        self._tablewidget.setItem(row, 0, value_item)
 
     def __delitem__(self, k: str) -> None:
         row = self._dict.pop(k)
-        self._tablewidget.removeRow(row)
 
     def __iter__(self) -> Iterable[str]:
         return iter(self._dict)
 
     def keys(self):
         """
         Return the view of dictionary keys.
         """
         return self._dict.keys()
 
     def values(self) -> DictValueView:
         """
         Return the view of dictionary values as Python objects.
         """
-        return DictValueView(self._tablewidget)
+        return DictValueView(self._treewidget)
 
-    def items(self) -> DictItemView:
-        """
-        Return the view of dictionary keys and values as strings and Python objects.
-        """
-        return DictItemView(self._tablewidget)
+    # def items(self) -> DictItemView:
+    #     """
+    #     Return the view of dictionary keys and values as strings and Python objects.
+    #     """
+    #     return DictItemView(self._treewidget)
 
     def update(self, d: dict[str, Any]):
         """
         Update the dictionary contents.
         """
         for k, v in d.items():
             self[k] = v
 
     def clear(self) -> None:
         """
         Clear dictionary contents.
         """
-        self._tablewidget.clear()
+        self._treewidget.clear()
         self._dict.clear()
 
     def pop(self, k: str):
         """
         Pop a dictionary content.
         """
         row = self._dict.pop(k)
-        out = self._tablewidget.item(row, 0).obj
-        self._tablewidget.removeRow(row)
+        out = self._treewidget.item(row, 0).obj
+        self._treewidget.removeRow(row)
         return out
 
     def get(self, k: str, default=None):
         self._dict.get(k, default)
 
 
-class PyTableWidget(ContextMenuMixin, QTableWidget):
-    def item(self, row: int, column: int) -> PyTableWidgetItem:
+class PyTreeWidget(ContextMenuMixin, QTreeWidget):
+    def item(self, row: int, column: int) -> PyTreeWidgetItem:
         return super().item(row, column)
 
-    def itemAt(self, *p) -> PyTableWidgetItem:
+    def itemAt(self, *p) -> PyTreeWidgetItem:
         return super().itemAt(*p)
 
     def __init__(self, parent: None) -> None:
         super().__init__(parent=parent)
         self.setContextMenu()
 
 
-class PyTableWidgetItem(PyObjectBound, QTableWidgetItem):
+unbound = object()
+
+
+class PyTreeWidgetItem(PyObjectBound, QTreeWidgetItem):
     def __init__(self, obj=None, name=None):
         super().__init__()
         self.setObject(obj, name)
 
 
 class DictValueView:
-    def __init__(self, widget: PyTableWidget):
+    def __init__(self, widget: PyTreeWidget):
         self.widget = widget
 
     def __iter__(self):
         for row in range(self.widget.rowCount()):
             yield self.widget.item(row, 0).obj
 
 
-class DictItemView:
-    def __init__(self, widget: PyTableWidget):
-        self.widget = widget
-
-    def __iter__(self):
-        for row in range(self.widget.rowCount()):
-            key = self.widget.verticalHeaderItem(row).text()
-            value = self.widget.item(row, 0).obj
-            yield key, value
+# class DictItemView:
+#     def __init__(self, widget: PyTableWidget):
+#         self.widget = widget
+
+#     def __iter__(self):
+#         for row in range(self.widget.rowCount()):
+#             key = self.widget.verticalHeaderItem(row).text()
+#             value = self.widget.item(row, 0).obj
+#             yield key, value
```

### Comparing `magic-class-0.6.9/magicclass/widgets/pywidgets/list.py` & `magic_class-0.7.0rc0/magicclass/widgets/pywidgets/list.py`

 * *Files identical despite different names*

### Comparing `magic-class-0.6.9/magicclass/widgets/pywidgets/object.py` & `magic_class-0.7.0rc0/magicclass/widgets/pywidgets/object.py`

 * *Files identical despite different names*

### Comparing `magic-class-0.6.9/magicclass/widgets/separator.py` & `magic_class-0.7.0rc0/magicclass/_gui/runner.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,93 +1,90 @@
 from __future__ import annotations
-from psygnal import Signal
-from qtpy.QtWidgets import QFrame, QLabel, QPushButton, QSizePolicy, QHBoxLayout
-from .utils import FreeWidget
+from pathlib import Path
 
+from typing import TYPE_CHECKING, Any, Callable, Iterator, Union, Sequence
+import weakref
 
-class Separator(FreeWidget):
-    """
-    A Separator widget that can be used in both widgets and menus.
-    This widget is not actually added to menus or toolbars.
-    """
+from qtpy import QtWidgets as QtW
+from macrokit import Expr, Symbol, parse
+from magicclass._gui.mgui_ext import Action
 
-    btn_clicked = Signal(bool)
 
+if TYPE_CHECKING:
+    from magicclass import MagicTemplate
+
+    _ActionLike = Union[Callable[[], Any], Expr]
+
+
+class CommandRunnerMenu(Sequence[Action]):
     def __init__(
         self,
-        orientation: str = "horizontal",
-        title: str = "",
-        name: str = "",
-        button: bool = False,
+        title: str,
+        parent: QtW.QWidget = None,
+        magicclass_parent: MagicTemplate = None,
     ):
-        super().__init__(name=name)
-        self._qtitlebar = _QTitleBar(self.native, title, button)
-        self.set_widget(self._qtitlebar)
-        if button:
-            self._qtitlebar.button.clicked.connect(
-                lambda e: self.btn_clicked.emit(self._qtitlebar.button.isDown())
-            )
-        self._title = title
+        self._native = QtW.QMenu(title, parent)
+        self.native.setToolTipsVisible(True)
+        self.__magicclass_parent__ = magicclass_parent
+        self._command_actions: list[Action] = []
 
     @property
-    def btn_text(self):
-        return self._qtitlebar.button.text()
-
-    @btn_text.setter
-    def btn_text(self, value: str):
-        self._qtitlebar.button.setText(value)
+    def native(self) -> QtW.QMenu:
+        return self._native
 
     @property
-    def title(self) -> str:
-        return self._title
+    def parent_ui(self) -> MagicTemplate:
+        return self.__magicclass_parent__._search_parent_magicclass()
+
+    def __getitem__(self, index: int) -> Action:
+        return self._command_actions[index]
 
+    def __len__(self) -> int:
+        return len(self._command_actions)
 
-class _QTitleBar(QLabel):
-    """See also: napari/_qt/qt_main_window.py."""
+    def __iter__(self) -> Iterator[Action]:
+        return iter(self._command_actions)
+
+    def add_action(
+        self, slot: _ActionLike, text: str = None, tooltip: str = None
+    ) -> CommandRunnerMenu:
+        """Add a function or an expression as an action."""
+        if isinstance(slot, Expr):
+            ns = {Symbol.var("ui"): self.parent_ui}
+            if (viewer := self.parent_ui.parent_viewer) is not None:
+                ns.setdefault(Symbol.var("viewer"), viewer)
+            slot = lambda: slot.eval(ns)
+            slot.__doc__ = f"<b><code>{slot}</code></b>"
+        elif not callable(slot):
+            raise TypeError(f"slot must be callable or an Expr, got {type(slot)}")
+        if text is None:
+            text = f"Command {len(self)}"
+        if tooltip is None:
+            tooltip = getattr(slot, "__doc__", None)
+        tooltip = tooltip.replace("\n", "<br>")
+
+        action = Action(text=text)
+        action.tooltip = tooltip
+        action.native.triggered.connect(slot)
+        self.native.addAction(action.native)
+        self._command_actions.append(action)
+        return self
+
+    def add_file(self, path: str | Path | bytes) -> CommandRunnerMenu:
+        """Add a executable file as an action."""
+        with open(path) as f:
+            expr = parse(f.read())
+        return self.add_action(expr)
 
-    def __init__(self, parent, text: str = "", button: bool = False):
-        super().__init__(parent)
-
-        line = QFrame(parent=self)
-        line.setFrameShape(QFrame.HLine)
-        line.setFrameShadow(QFrame.Sunken)
-        line.setObjectName("Separator")
-        line.setStyleSheet(
-            """
-            QFrame#Separator {
-                background-color: gray;
-            }
-        """
-        )
-
-        layout = QHBoxLayout()
-        layout.setSpacing(4)
-        layout.setContentsMargins(8, 1, 8, 0)
-
-        if button:
-            self.button = QPushButton(self)
-            self.button.setFixedWidth(20)
-            self.button.setStyleSheet(
-                "QPushButton {"
-                "border: 1px solid #555;"
-                "border-radius: 10px;"
-                "border-style: outset;"
-                "padding: 5px"
-                "}"
-            )
-            layout.addWidget(self.button)
-
-        layout.addWidget(line)
-
-        if text:
-            text = QLabel(text, self)
-            text.setSizePolicy(
-                QSizePolicy(QSizePolicy.Policy.Maximum, QSizePolicy.Policy.Maximum)
-            )
-            layout.addWidget(text)
-
-        self.setLayout(layout)
-
-    def sizeHint(self):
-        szh = super().sizeHint()
-        szh.setHeight(20)
-        return szh
+    @property
+    def __magicclass_parent__(self) -> MagicTemplate | None:
+        """Return parent magic class if exists."""
+        if self._magicclass_parent_ref is None:
+            return None
+        parent = self._magicclass_parent_ref()
+        return parent
+
+    @__magicclass_parent__.setter
+    def __magicclass_parent__(self, parent) -> None:
+        if parent is None:
+            return
+        self._magicclass_parent_ref = weakref.ref(parent)
```

### Comparing `magic-class-0.6.9/magicclass/widgets/utils.py` & `magic_class-0.7.0rc0/magicclass/widgets/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import weakref
 from qtpy.QtWidgets import QWidget, QVBoxLayout, QGridLayout, QHBoxLayout
 from magicgui.widgets import Widget
 from magicgui.widgets._concrete import merge_super_sigs as _merge_super_sigs
 from magicgui.backends._qtpy.widgets import QBaseWidget
 
 if TYPE_CHECKING:
-    from .._gui import BaseGui, ContextMenuGui
+    from magicclass._gui import BaseGui, ContextMenuGui
 
 
 class _NotInitialized:
     """This class helps better error handling."""
 
     def __init__(self, msg: str):
         self.msg = msg
```

### Comparing `magic-class-0.6.9/magicclass/wrappers.py` & `magic_class-0.7.0rc0/magicclass/wrappers/_misc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from __future__ import annotations
 import inspect
-from typing import Callable, Iterable, Union, TYPE_CHECKING, TypeVar, overload
+from typing import Any, Callable, TYPE_CHECKING, TypeVar, overload
 import warnings
 from magicgui.widgets import FunctionGui
 
-from .utils import show_messagebox
-from .types import Color
-from .signature import upgrade_signature
+from magicclass.types import Color
+from magicclass.signature import get_additional_option, upgrade_signature
 
 if TYPE_CHECKING:
-    from ._gui import BaseGui
-
-nStrings = Union[str, Iterable[str]]
+    from magicclass._gui import BaseGui
 
 R = TypeVar("R")
 T = TypeVar("T")
 F = TypeVar("F", bound=Callable)
 
 
 def set_options(
@@ -146,18 +143,44 @@
         else:
             upgrade_signature(obj, caller_options=caller_options)
         return obj
 
     return wrapper
 
 
-def do_not_record(method: F) -> F:
-    """Wrapped method will not be recorded in macro."""
-    upgrade_signature(method, additional_options={"record": False})
-    return method
+@overload
+def do_not_record(method: None = None, recursive: bool = True) -> Callable[[F], F]:
+    ...
+
+
+@overload
+def do_not_record(method: F, recursive: bool = True) -> F:
+    ...
+
+
+def do_not_record(method=None, recursive=False):
+    """
+    Wrapped method will not be recorded in macro.
+
+    Parameters
+    ----------
+    recursive : bool, default is False
+        If True, all recordable methods called inside this method will also be
+        suppressed.
+    """
+
+    def wrapper(f):
+        if recursive:
+            record = "all-false"
+        else:
+            record = "false"
+        upgrade_signature(f, additional_options={"record": record})
+        return f
+
+    return wrapper if method is None else wrapper(method)
 
 
 def bind_key(*key) -> Callable[[F], F]:
     """
     Define a keybinding to a button or an action.
     This function accepts several styles of shortcut expression.
 
@@ -173,200 +196,81 @@
     def wrapper(method: F) -> F:
         upgrade_signature(method, additional_options={"keybinding": key})
         return method
 
     return wrapper
 
 
-class Canceled(RuntimeError):
-    """Raised when a function is canceled"""
-
-
-@overload
-def confirm(
-    *,
-    text: str | None,
-    condition: Callable[..., bool] | str | None,
-    callback: Callable[[str, BaseGui], None] | None = None,
-) -> Callable[[F], F]:
-    ...
-
-
-@overload
-def confirm(
-    f: F,
-    *,
-    text: str | None,
-    condition: Callable[..., bool] | str | None,
-    callback: Callable[[str, BaseGui], None] | None = None,
-) -> F:
-    ...
-
-
-def confirm(
-    f: F | None = None,
-    *,
-    text: str | None = None,
-    condition: Callable[[BaseGui], bool] | str = None,
-    callback: Callable[[str, BaseGui], None] | None = None,
-):
-    """
-    Confirm if it is OK to run function in GUI.
-
-    Useful when the function will irreversibly delete or update something in GUI.
-    Confirmation will be executed only when function is called in GUI.
-
-    Parameters
-    ----------
-    text : str, optional
-        Confirmation message, such as "Are you sure to run this function?". Format
-        string can also be used here, in which case arguments will be passed. For
-        instance, to execute confirmation on function ``f(a, b)``, you can use
-        format string ``"Running with a = {a} and b = {b}"`` then confirmation
-        message will be "Running with a = 1, b = 2" if ``f(1, 2)`` is called.
-        By default, message will be "Do you want to run {name}?" where "name" is
-        the function name.
-    condition : callable or str, optional
-        Condition of when confirmation will show up. If callable, it must accept
-        ``condition(self)`` and return boolean object. If string, it must be
-        evaluable as literal with input arguments as local namespace. For instance,
-        function ``f(a, b)`` decorated by ``confirm(condition="a < b + 1")`` will
-        evaluate ``a < b + 1`` to check if confirmation is needed. Always true by
-        default.
-    callback : callable, optional
-        Callback function when confirmation is needed. Must take a ``str`` and a
-        ``BaseGui`` object as inputs. By default, message box will be shown. Useful
-        for testing.
-    """
-    if condition is None:
-        condition = lambda x: True
-    if callback is None:
-        callback = _default_confirmation
-
-    def _decorator(method: F) -> F:
-        _name = method.__name__
-
-        # set text
-        if text is None:
-            _text = f"Do you want to run {_name}?"
-        elif isinstance(text, str):
-            _text = text
-        else:
-            raise TypeError(
-                f"The first argument of 'confirm' must be a str but got {type(text)}."
-            )
-        upgrade_signature(
-            method,
-            additional_options={
-                "confirm": {
-                    "text": _text,
-                    "condition": condition,
-                    "callback": callback,
-                }
-            },
-        )
-        return method
-
-    if f is not None:
-        return _decorator(f)
-    return _decorator
-
-
-def _default_confirmation(text: str, gui: BaseGui):
-    ok = show_messagebox(
-        mode="question",
-        title="Confirmation",
-        text=text,
-        parent=gui.native,
-    )
-    if not ok:
-        raise Canceled("Canceled")
-
-
 def nogui(method: F) -> F:
     """Wrapped method will not be converted into a widget."""
     upgrade_signature(method, additional_options={"gui": False})
     return method
 
 
-def mark_preview(function: Callable, text: str = "Preview") -> Callable[[F], F]:
+def setup_function_gui(target: Callable):
     """
-    Define a preview of a function.
+    Mark a function as a setup function for a FunctionGui.
 
-    This decorator is useful for advanced magicgui creation. A "Preview" button
-    appears in the bottom of the widget built from the input function and the
-    decorated function will be called with the same arguments.
-    Following example shows how to define a previewer that prints the content of
-    the selected file.
+    Function decorated with ``setup_function_gui(func)`` will be called when the
+    FunctionGui widget for method ``func`` was built. This decorator is used to
+    define complicated setting of a FunctionGui, which is not achievable by
+    simple configurations.
+
+    >>> @magicclass
+    >>> class A:
+    ...     def func(self, x: int, xmax: int):
+    ...         # target function
+    ...
+    ...     @setup_function_gui(func)
+    ...     def _setup_func(self, gui: FunctionGui):
+    ...         @gui.xmax.changed.connect
+    ...         def _(xmax_value):
+    ...             gui.x.max = xmax_value
+    """
 
-    .. code-block:: python
+    def wrapper(setup: Callable[[BaseGui, FunctionGui], None]):
+        setup_qualname = setup.__qualname__
+        target_qualname = target.__qualname__
+        setup_qualname_list = setup_qualname.split(".")
+        if (
+            len(setup_qualname_list) > 1
+            and setup_qualname_list[-2] != target_qualname.split(".")[-2]
+        ):
+            # have to search for the proper parent instance
+            def _setup(self: BaseGui, mgui: FunctionGui):
+                prev_ns = setup_qualname_list[-2]
+                while self.__class__.__name__ != prev_ns:
+                    self = self.__magicclass_parent__
+                return setup(self, mgui)
 
-        def func(self, path: Path):
-            ...
+        else:
+            _setup = setup
+        upgrade_signature(target, additional_options={"setup": _setup})
+        upgrade_signature(setup, additional_options={"nogui": True})
+        return setup
 
-        @mark_preview(func)
-        def _func_prev(self, path: Path):
-            with open(path, mode="r") as f:
-                print(f.read())
+    return wrapper
 
-    Parameters
-    ----------
-    function : callable
-        To which function previewer will be defined.
-    text : str, optional
-        Text of preview button.
-    """
 
-    def _wrapper(preview: F) -> F:
-        sig_preview = inspect.signature(preview)
-        sig_func = inspect.signature(function)
-        params_preview = sig_preview.parameters
-        params_func = sig_func.parameters
-
-        less = len(params_func) - len(params_preview)
-        if less == 0:
-            if params_preview.keys() != params_func.keys():
-                raise TypeError(
-                    f"Arguments mismatch between {sig_preview!r} and {sig_func!r}."
-                )
-            # If argument names are identical, input arguments don't have to be filtered.
-            _filter = lambda a: a
-
-        elif less > 0:
-            idx: list[int] = []
-            for i, param in enumerate(params_func.keys()):
-                if param in params_preview:
-                    idx.append(i)
-            # If argument names are not identical, input arguments have to be filtered so
-            # that arguments match the inputs.
-            _filter = lambda _args: (a for i, a in enumerate(_args) if i in idx)
+_Fn = TypeVar("_Fn", bound=Callable[[FunctionGui], Any])
 
-        else:
-            raise TypeError(
-                f"Number of arguments of preview function {preview!r} must be equal"
-                f"or smaller than that of running function {function!r}."
-            )
 
-        def _preview(*args):
-            # find proper parent instance in the case of classes being nested
-            from ._gui import BaseGui
-
-            if len(args) > 0 and isinstance(args[0], BaseGui):
-                ins = args[0]
-                prev_ns = preview.__qualname__.split(".")[-2]
-                while ins.__class__.__name__ != prev_ns:
-                    ins = ins.__magicclass_parent__
-                args = (ins,) + args[1:]
-            # filter input arguments
-            return preview(*_filter(args))
-
-        if not isinstance(function, FunctionGui):
-            upgrade_signature(
-                function, additional_options={"preview": (text, _preview)}
-            )
+def mark_on_calling(function: Callable) -> Callable[[_Fn], _Fn]:
+    def _wrapper(on_calling: _Fn) -> _Fn:
+        if opt := get_additional_option(function, "on_calling", None):
+            opt.append(on_calling)
         else:
-            from ._gui._function_gui import append_preview
+            upgrade_signature(function, additional_options={"on_calling": [on_calling]})
+        return on_calling
 
-            append_preview(function, _preview, text=text)
-        return preview
+    return _wrapper
+
+
+def mark_on_called(function: Callable) -> Callable[[_Fn], _Fn]:
+    def _wrapper(on_called: _Fn) -> _Fn:
+        if opt := get_additional_option(function, "on_called", None):
+            opt.append(on_called)
+        else:
+            upgrade_signature(function, additional_options={"on_called": [on_called]})
+        return on_called
 
     return _wrapper
```

