# Comparing `tmp/PyGObject-stubs-2.6.0.tar.gz` & `tmp/PyGObject-stubs-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGObject-stubs-2.6.0.tar", last modified: Sat Apr  8 07:24:35 2023, max compression
+gzip compressed data, was "PyGObject-stubs-2.7.0.tar", last modified: Tue May  9 17:02:27 2023, max compression
```

## Comparing `PyGObject-stubs-2.6.0.tar` & `PyGObject-stubs-2.7.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 07:24:35.456706 PyGObject-stubs-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-08 07:24:35.456706 PyGObject-stubs-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 07:24:35.448706 PyGObject-stubs-2.6.0/pep517backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/pep517backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/pep517backend/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 07:24:35.456706 PyGObject-stubs-2.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 07:24:35.444706 PyGObject-stubs-2.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 07:24:35.448706 PyGObject-stubs-2.6.0/src/PyGObject_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-08 07:24:35.000000 PyGObject-stubs-2.6.0/src/PyGObject_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-08 07:24:35.000000 PyGObject-stubs-2.6.0/src/PyGObject_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 07:24:35.000000 PyGObject-stubs-2.6.0/src/PyGObject_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-08 07:24:35.000000 PyGObject-stubs-2.6.0/src/PyGObject_stubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-08 07:24:35.000000 PyGObject-stubs-2.6.0/src/PyGObject_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 07:24:35.448706 PyGObject-stubs-2.6.0/src/gi-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 07:24:35.456706 PyGObject-stubs-2.6.0/src/gi-stubs/repository/
--rw-r--r--   0 runner    (1001) docker     (123)   155987 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/Adw.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/AppIndicator3.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    47065 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/Atk.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/AyatanaAppIndicator3.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/Farstream.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/GIRepository.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   129078 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/GLib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/GModule.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    75309 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/GObject.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/GSound.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15989 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/GdkPixbuf.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20001 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/Geoclue.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    63495 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/Ggit.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   304553 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/Gio.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23860 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/Graphene.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19621 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/Gsk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/Gspell.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   165678 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/Gst.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/GstPbutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/Manette.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    46604 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/Pango.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/PangoCairo.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/Rsvg.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22165 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/Vte.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   128468 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/_Gdk3.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   110771 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/_Gdk4.pyi
--rw-r--r--   0 runner    (1001) docker     (123)  1048514 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/_Gtk3.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   658864 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/_Gtk4.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    80128 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/_GtkSource4.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    89364 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/_GtkSource5.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    40235 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/_Soup2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    49071 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/_Soup3.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 07:24:25.000000 PyGObject-stubs-2.6.0/src/gi-stubs/repository/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:02:27.251135 PyGObject-stubs-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-09 17:02:27.251135 PyGObject-stubs-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:02:27.243135 PyGObject-stubs-2.7.0/pep517backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/pep517backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/pep517backend/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 17:02:27.251135 PyGObject-stubs-2.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:02:27.243135 PyGObject-stubs-2.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:02:27.243135 PyGObject-stubs-2.7.0/src/PyGObject_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-09 17:02:27.000000 PyGObject-stubs-2.7.0/src/PyGObject_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-09 17:02:27.000000 PyGObject-stubs-2.7.0/src/PyGObject_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:02:27.000000 PyGObject-stubs-2.7.0/src/PyGObject_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 17:02:27.000000 PyGObject-stubs-2.7.0/src/PyGObject_stubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 17:02:27.000000 PyGObject-stubs-2.7.0/src/PyGObject_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:02:27.243135 PyGObject-stubs-2.7.0/src/gi-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:02:27.251135 PyGObject-stubs-2.7.0/src/gi-stubs/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)   155987 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Adw.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/AppIndicator3.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    47065 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Atk.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/AyatanaAppIndicator3.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Farstream.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/GIRepository.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   129078 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/GLib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/GModule.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    75309 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/GObject.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/GSound.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15989 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/GdkPixbuf.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20001 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Geoclue.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    63495 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Ggit.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   304553 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Gio.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23860 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Graphene.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19621 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Gsk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Gspell.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   165678 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Gst.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/GstPbutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Manette.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    46604 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Pango.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/PangoCairo.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Rsvg.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22165 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/Vte.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   128468 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Gdk3.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   112437 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Gdk4.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)  1058819 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Gtk3.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   681586 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Gtk4.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    80128 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/_GtkSource4.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    89364 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/_GtkSource5.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    40235 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Soup2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    49071 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Soup3.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:02:15.000000 PyGObject-stubs-2.7.0/src/gi-stubs/repository/__init__.pyi
```

### Comparing `PyGObject-stubs-2.6.0/CHANGELOG.md` & `PyGObject-stubs-2.7.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+# 2.7.0 (28 Apr 2023)
+
+## Improvements
+
+* Extract class' docstring
+
+## Typing
+
+* Improve type hints for
+    - Gdk4
+    - Gtk3
+
 # 2.6.0 (08 Apr 2023)
 
 ## Improvements
 
 * Generator: Correctly type optional props
 
 ## Typing
```

### Comparing `PyGObject-stubs-2.6.0/LICENSE` & `PyGObject-stubs-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/PKG-INFO` & `PyGObject-stubs-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGObject-stubs
-Version: 2.6.0
+Version: 2.7.0
 Summary: Typing stubs for PyGObject
 Author: Christoph Reiter
 Author-email: reiter.christoph@gmail.com
 License: LGPL-2.1
 Project-URL: homepage, https://github.com/pygobject/pygobject-stubs
 Project-URL: repository, https://github.com/pygobject/pygobject-stubs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyGObject-stubs-2.6.0/README.md` & `PyGObject-stubs-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/pep517backend/backend.py` & `PyGObject-stubs-2.7.0/pep517backend/backend.py`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/pyproject.toml` & `PyGObject-stubs-2.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 65.0.0"]
 build-backend = "backend"
 backend-path = ["pep517backend"]
 
 [project]
 name = "PyGObject-stubs"
-version = "2.6.0"
+version = "2.7.0"
 description = "Typing stubs for PyGObject"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "LGPL-2.1"}
 authors = [
   {email = "reiter.christoph@gmail.com"},
   {name = "Christoph Reiter"}
```

### Comparing `PyGObject-stubs-2.6.0/src/PyGObject_stubs.egg-info/PKG-INFO` & `PyGObject-stubs-2.7.0/src/PyGObject_stubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGObject-stubs
-Version: 2.6.0
+Version: 2.7.0
 Summary: Typing stubs for PyGObject
 Author: Christoph Reiter
 Author-email: reiter.christoph@gmail.com
 License: LGPL-2.1
 Project-URL: homepage, https://github.com/pygobject/pygobject-stubs
 Project-URL: repository, https://github.com/pygobject/pygobject-stubs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyGObject-stubs-2.6.0/src/PyGObject_stubs.egg-info/SOURCES.txt` & `PyGObject-stubs-2.7.0/src/PyGObject_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/Adw.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Adw.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/AppIndicator3.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/AppIndicator3.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/Atk.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Atk.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/Farstream.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Farstream.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/GIRepository.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/GIRepository.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/GLib.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/GLib.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/GModule.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/GModule.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/GObject.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/GObject.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/GSound.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/GSound.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/GdkPixbuf.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/GdkPixbuf.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/Geoclue.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Geoclue.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/Ggit.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Ggit.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/Gio.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Gio.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/Graphene.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Graphene.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/Gsk.py` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Gsk.py`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/Gspell.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Gspell.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/Gst.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Gst.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/GstPbutils.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/GstPbutils.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/Manette.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Manette.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/Pango.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Pango.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/PangoCairo.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/PangoCairo.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/Rsvg.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Rsvg.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/Vte.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/Vte.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/_Gdk3.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Gdk3.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/_Gdk4.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Gdk4.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any
 from typing import Callable
 from typing import Literal
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Type
+from typing import TypeVar
 
 import cairo
 from gi.repository import GdkPixbuf
 from gi.repository import Gio
 from gi.repository import GLib
 from gi.repository import GObject
 from gi.repository import Pango
@@ -2331,15 +2332,17 @@
 def cairo_set_source_rgba(cr: cairo.Context[_SomeSurface], rgba: RGBA) -> None: ...
 def content_deserialize_async(
     stream: Gio.InputStream,
     mime_type: str,
     type: Type,
     io_priority: int,
     cancellable: Optional[Gio.Cancellable] = None,
-    callback: Optional[Callable[..., None]] = None,
+    callback: Optional[
+        Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+    ] = None,
     *user_data: Any,
 ) -> None: ...
 def content_deserialize_finish(result: Gio.AsyncResult) -> Tuple[bool, Any]: ...
 def content_formats_parse(string: str) -> Optional[ContentFormats]: ...
 def content_register_deserializer(
     mime_type: str,
     type: Type,
@@ -2354,15 +2357,17 @@
 ) -> None: ...
 def content_serialize_async(
     stream: Gio.OutputStream,
     mime_type: str,
     value: Any,
     io_priority: int,
     cancellable: Optional[Gio.Cancellable] = None,
-    callback: Optional[Callable[..., None]] = None,
+    callback: Optional[
+        Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+    ] = None,
     *user_data: Any,
 ) -> None: ...
 def content_serialize_finish(result: Gio.AsyncResult) -> bool: ...
 def drag_action_is_unique(action: DragAction) -> bool: ...
 def events_get_angle(event1: Event, event2: Event) -> Tuple[bool, float]: ...
 def events_get_center(event1: Event, event2: Event) -> Tuple[bool, float, float]: ...
 def events_get_distance(event1: Event, event2: Event) -> Tuple[bool, float]: ...
@@ -2399,73 +2404,83 @@
     def set_timestamp(self, timestamp: int) -> None: ...
 
 class ButtonEvent(Event):
     def get_button(self) -> int: ...
 
 class CairoContext(DrawContext):
     class Props:
-        display: Display
-        surface: Surface
+        display: Optional[Display]
+        surface: Optional[Surface]
     props: Props = ...
     def __init__(self, display: Display = ..., surface: Surface = ...): ...
     def cairo_create(self) -> Optional[cairo.Context]: ...
 
 class Clipboard(GObject.Object):
     class Props:
-        content: ContentProvider
+        content: Optional[ContentProvider]
         display: Display
         formats: ContentFormats
         local: bool
     props: Props = ...
     def __init__(self, display: Display = ...): ...
     def get_content(self) -> Optional[ContentProvider]: ...
     def get_display(self) -> Display: ...
     def get_formats(self) -> ContentFormats: ...
     def is_local(self) -> bool: ...
     def read_async(
         self,
         mime_types: Sequence[str],
         io_priority: int,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[Callable[..., None]] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
         *user_data: Any,
     ) -> None: ...
     def read_finish(
         self, result: Gio.AsyncResult
     ) -> Tuple[Optional[Gio.InputStream], str]: ...
     def read_text_async(
         self,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[Callable[..., None]] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
         *user_data: Any,
     ) -> None: ...
     def read_text_finish(self, result: Gio.AsyncResult) -> Optional[str]: ...
     def read_texture_async(
         self,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[Callable[..., None]] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
         *user_data: Any,
     ) -> None: ...
     def read_texture_finish(self, result: Gio.AsyncResult) -> Optional[Texture]: ...
     def read_value_async(
         self,
         type: Type,
         io_priority: int,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[Callable[..., None]] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
         *user_data: Any,
     ) -> None: ...
     def read_value_finish(self, result: Gio.AsyncResult) -> Any: ...
     def set(self, value: Any) -> None: ...
     def set_content(self, provider: Optional[ContentProvider] = None) -> bool: ...
     def store_async(
         self,
         io_priority: int,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[Callable[..., None]] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
         *user_data: Any,
     ) -> None: ...
     def store_finish(self, result: Gio.AsyncResult) -> bool: ...
 
 class ContentDeserializer(GObject.Object, Gio.AsyncResult):
     def get_cancellable(self) -> Optional[Gio.Cancellable]: ...
     def get_gtype(self) -> Type: ...
@@ -2528,15 +2543,17 @@
     def do_ref_storable_formats(self) -> ContentFormats: ...
     def do_write_mime_type_async(
         self,
         mime_type: str,
         stream: Gio.OutputStream,
         io_priority: int,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[Callable[..., None]] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
         *user_data: Any,
     ) -> None: ...
     def do_write_mime_type_finish(self, result: Gio.AsyncResult) -> bool: ...
     def get_value(self) -> Tuple[bool, Any]: ...
     @classmethod
     def new_for_bytes(cls, mime_type: str, bytes: GLib.Bytes) -> ContentProvider: ...
     @classmethod
@@ -2549,15 +2566,17 @@
     def ref_storable_formats(self) -> ContentFormats: ...
     def write_mime_type_async(
         self,
         mime_type: str,
         stream: Gio.OutputStream,
         io_priority: int,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[Callable[..., None]] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
         *user_data: Any,
     ) -> None: ...
     def write_mime_type_finish(self, result: Gio.AsyncResult) -> bool: ...
 
 class ContentProviderClass(GObject.GPointer):
     parent_class: GObject.ObjectClass = ...
     content_changed: Callable[[ContentProvider], None] = ...
@@ -2586,19 +2605,19 @@
 class CrossingEvent(Event):
     def get_detail(self) -> NotifyType: ...
     def get_focus(self) -> bool: ...
     def get_mode(self) -> CrossingMode: ...
 
 class Cursor(GObject.Object):
     class Props:
-        fallback: Cursor
+        fallback: Optional[Cursor]
         hotspot_x: int
         hotspot_y: int
-        name: str
-        texture: Texture
+        name: Optional[str]
+        texture: Optional[Texture]
     props: Props = ...
     def __init__(
         self,
         fallback: Cursor = ...,
         hotspot_x: int = ...,
         hotspot_y: int = ...,
         name: str = ...,
@@ -2635,20 +2654,20 @@
         has_bidi_layouts: bool
         has_cursor: bool
         modifier_state: ModifierType
         n_axes: int
         name: str
         num_lock_state: bool
         num_touches: int
-        product_id: str
+        product_id: Optional[str]
         scroll_lock_state: bool
         seat: Seat
         source: InputSource
         tool: DeviceTool
-        vendor_id: str
+        vendor_id: Optional[str]
     props: Props = ...
     def __init__(
         self,
         display: Display = ...,
         has_cursor: bool = ...,
         name: str = ...,
         num_touches: int = ...,
@@ -2714,40 +2733,40 @@
     def device_is_grabbed(self, device: Device) -> bool: ...
     def flush(self) -> None: ...
     def get_app_launch_context(self) -> AppLaunchContext: ...
     def get_clipboard(self) -> Clipboard: ...
     @staticmethod
     def get_default() -> Optional[Display]: ...
     def get_default_seat(self) -> Optional[Seat]: ...
-    def get_monitor_at_surface(self, surface: Surface) -> Monitor: ...
+    def get_monitor_at_surface(self, surface: Surface) -> Optional[Monitor]: ...
     def get_monitors(self) -> Gio.ListModel: ...
     def get_name(self) -> str: ...
     def get_primary_clipboard(self) -> Clipboard: ...
     def get_setting(self, name: str, value: Any) -> bool: ...
     def get_startup_notification_id(self) -> Optional[str]: ...
     def is_closed(self) -> bool: ...
     def is_composited(self) -> bool: ...
     def is_rgba(self) -> bool: ...
     def list_seats(self) -> list[Seat]: ...
     def map_keycode(self, keycode: int) -> Tuple[bool, list[KeymapKey], list[int]]: ...
     def map_keyval(self, keyval: int) -> Tuple[bool, list[KeymapKey]]: ...
     def notify_startup_complete(self, startup_id: str) -> None: ...
     @staticmethod
-    def open(display_name: str) -> Optional[Display]: ...
+    def open(display_name: Optional[str] = None) -> Optional[Display]: ...
     def prepare_gl(self) -> bool: ...
     def put_event(self, event: Event) -> None: ...
     def supports_input_shapes(self) -> bool: ...
     def sync(self) -> None: ...
     def translate_key(
         self, keycode: int, state: ModifierType, group: int
     ) -> Tuple[bool, int, int, int, ModifierType]: ...
 
 class DisplayManager(GObject.Object):
     class Props:
-        default_display: Display
+        default_display: Optional[Display]
     props: Props = ...
     def __init__(self, default_display: Display = ...): ...
     @staticmethod
     def get() -> DisplayManager: ...
     def get_default_display(self) -> Optional[Display]: ...
     def list_displays(self) -> list[Display]: ...
     def open_display(self, name: str) -> Optional[Display]: ...
@@ -2795,31 +2814,31 @@
 class DragSurface(GObject.GInterface):
     def present(self, width: int, height: int) -> bool: ...
 
 class DragSurfaceInterface(GObject.GPointer): ...
 
 class DrawContext(GObject.Object):
     class Props:
-        display: Display
-        surface: Surface
+        display: Optional[Display]
+        surface: Optional[Surface]
     props: Props = ...
     def __init__(self, display: Display = ..., surface: Surface = ...): ...
     def begin_frame(self, region: cairo.Region) -> None: ...
     def end_frame(self) -> None: ...
     def get_display(self) -> Optional[Display]: ...
     def get_frame_region(self) -> Optional[cairo.Region]: ...
     def get_surface(self) -> Optional[Surface]: ...
     def is_in_frame(self) -> bool: ...
 
 class Drop(GObject.Object):
     class Props:
         actions: DragAction
         device: Device
         display: Display
-        drag: Drag
+        drag: Optional[Drag]
         formats: ContentFormats
         surface: Surface
     props: Props = ...
     def __init__(
         self,
         actions: DragAction = ...,
         device: Device = ...,
@@ -2835,26 +2854,30 @@
     def get_formats(self) -> ContentFormats: ...
     def get_surface(self) -> Surface: ...
     def read_async(
         self,
         mime_types: Sequence[str],
         io_priority: int,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[Callable[..., None]] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
         *user_data: Any,
     ) -> None: ...
     def read_finish(
         self, result: Gio.AsyncResult
     ) -> Tuple[Optional[Gio.InputStream], str]: ...
     def read_value_async(
         self,
         type: Type,
         io_priority: int,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[Callable[..., None]] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
         *user_data: Any,
     ) -> None: ...
     def read_value_finish(self, result: Gio.AsyncResult) -> Any: ...
     def status(self, actions: DragAction, preferred: DragAction) -> None: ...
 
 class Event:
     def get_axes(self) -> Tuple[bool, list[float]]: ...
@@ -2912,17 +2935,17 @@
     def ref(self) -> FrameTimings: ...
     def unref(self) -> None: ...
 
 class GLContext(DrawContext):
     class Props:
         allowed_apis: GLAPI
         api: GLAPI
-        shared_context: GLContext
-        display: Display
-        surface: Surface
+        shared_context: Optional[GLContext]
+        display: Optional[Display]
+        surface: Optional[Surface]
     props: Props = ...
     def __init__(
         self,
         allowed_apis: GLAPI = ...,
         shared_context: GLContext = ...,
         display: Display = ...,
         surface: Surface = ...,
@@ -3006,28 +3029,30 @@
         stride: int,
     ) -> MemoryTexture: ...
 
 class MemoryTextureClass(GObject.GPointer): ...
 
 class Monitor(GObject.Object):
     class Props:
-        connector: str
+        connector: Optional[str]
+        description: Optional[str]
         display: Display
         geometry: Rectangle
         height_mm: int
-        manufacturer: str
-        model: str
+        manufacturer: Optional[str]
+        model: Optional[str]
         refresh_rate: int
         scale_factor: int
         subpixel_layout: SubpixelLayout
         valid: bool
         width_mm: int
     props: Props = ...
     def __init__(self, display: Display = ...): ...
     def get_connector(self) -> Optional[str]: ...
+    def get_description(self) -> Optional[str]: ...
     def get_display(self) -> Display: ...
     def get_geometry(self) -> Rectangle: ...
     def get_height_mm(self) -> int: ...
     def get_manufacturer(self) -> Optional[str]: ...
     def get_model(self) -> Optional[str]: ...
     def get_refresh_rate(self) -> int: ...
     def get_scale_factor(self) -> int: ...
@@ -3152,15 +3177,15 @@
     def get_tools(self) -> list[DeviceTool]: ...
 
 class Snapshot(GObject.Object): ...
 class SnapshotClass(GObject.GPointer): ...
 
 class Surface(GObject.Object):
     class Props:
-        cursor: Cursor
+        cursor: Optional[Cursor]
         display: Display
         frame_clock: FrameClock
         height: int
         mapped: bool
         scale_factor: int
         width: int
     props: Props = ...
@@ -3208,14 +3233,15 @@
 class Texture(GObject.Object, Paintable, Gio.Icon, Gio.LoadableIcon):
     class Props:
         height: int
         width: int
     props: Props = ...
     def __init__(self, height: int = ..., width: int = ...): ...
     def download(self, data: Sequence[int], stride: int) -> None: ...
+    def get_format(self) -> MemoryFormat: ...
     def get_height(self) -> int: ...
     def get_width(self) -> int: ...
     @classmethod
     def new_for_pixbuf(cls, pixbuf: GdkPixbuf.Pixbuf) -> Texture: ...
     @classmethod
     def new_from_bytes(cls, bytes: GLib.Bytes) -> Texture: ...
     @classmethod
@@ -3227,14 +3253,26 @@
     def save_to_png(self, filename: str) -> bool: ...
     def save_to_png_bytes(self) -> GLib.Bytes: ...
     def save_to_tiff(self, filename: str) -> bool: ...
     def save_to_tiff_bytes(self) -> GLib.Bytes: ...
 
 class TextureClass(GObject.GPointer): ...
 
+class TextureDownloader(GObject.GBoxed):
+    def copy(self) -> TextureDownloader: ...
+    def download_bytes(self) -> Tuple[GLib.Bytes, int]: ...
+    def download_into(self, data: Sequence[int], stride: int) -> None: ...
+    def free(self) -> None: ...
+    def get_format(self) -> MemoryFormat: ...
+    def get_texture(self) -> Texture: ...
+    @classmethod
+    def new(cls, texture: Texture) -> TextureDownloader: ...
+    def set_format(self, format: MemoryFormat) -> None: ...
+    def set_texture(self, texture: Texture) -> None: ...
+
 class TimeCoord(GObject.GPointer):
     time: int = ...
     flags: AxisFlags = ...
     axes: list[float] = ...
 
 class Toplevel(GObject.GInterface):
     def begin_move(
@@ -3302,16 +3340,16 @@
     def get_gesture_phase(self) -> TouchpadGesturePhase: ...
     def get_n_fingers(self) -> int: ...
     def get_pinch_angle_delta(self) -> float: ...
     def get_pinch_scale(self) -> float: ...
 
 class VulkanContext(DrawContext, Gio.Initable):
     class Props:
-        display: Display
-        surface: Surface
+        display: Optional[Display]
+        surface: Optional[Surface]
     props: Props = ...
     def __init__(self, display: Display = ..., surface: Surface = ...): ...
 
 class AnchorHints(GObject.GFlags):
     FLIP = 3
     FLIP_X = 1
     FLIP_Y = 2
```

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/_Gtk3.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Gtk3.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -27,23 +27,23 @@
     CellRendererProgress,
     CellRendererSpin,
     CellRendererSpinner,
     CellRendererText,
     CellRendererToggle,
 )
 
-BINARY_AGE: int = 2434
+BINARY_AGE: int = 2437
 INPUT_ERROR: int = -1
-INTERFACE_AGE: int = 30
+INTERFACE_AGE: int = 32
 LEVEL_BAR_OFFSET_FULL: str = "full"
 LEVEL_BAR_OFFSET_HIGH: str = "high"
 LEVEL_BAR_OFFSET_LOW: str = "low"
 MAJOR_VERSION: int = 3
 MAX_COMPOSE_LEN: int = 7
-MICRO_VERSION: int = 34
+MICRO_VERSION: int = 37
 MINOR_VERSION: int = 24
 PAPER_NAME_A3: str = "iso_a3"
 PAPER_NAME_A4: str = "iso_a4"
 PAPER_NAME_A5: str = "iso_a5"
 PAPER_NAME_B5: str = "iso_b5"
 PAPER_NAME_EXECUTIVE: str = "na_executive"
 PAPER_NAME_LEGAL: str = "na_legal"
@@ -290,14 +290,15 @@
 STYLE_REGION_COLUMN_HEADER: str = "column-header"
 STYLE_REGION_ROW: str = "row"
 STYLE_REGION_TAB: str = "tab"
 TEXT_VIEW_PRIORITY_VALIDATE: int = 125
 TREE_SORTABLE_DEFAULT_SORT_COLUMN_ID: int = -1
 TREE_SORTABLE_UNSORTED_SORT_COLUMN_ID: int = -2
 _introspection_module = ...  # FIXME Constant
+_lock = ...  # FIXME Constant
 _namespace: str = "Gtk"
 _overrides_module = ...  # FIXME Constant
 _version: str = "3.0"
 
 def accel_groups_activate(
     object: GObject.Object, accel_key: int, accel_mods: Gdk.ModifierType
 ) -> bool: ...
@@ -910,15 +911,15 @@
 def selection_remove_all(widget: Widget) -> None: ...
 def set_debug_flags(flags: int) -> None: ...
 def show_uri(screen: Optional[Gdk.Screen], uri: str, timestamp: int) -> bool: ...
 def show_uri_on_window(parent: Optional[Window], uri: str, timestamp: int) -> bool: ...
 def stock_add(items: Sequence[StockItem]) -> None: ...
 def stock_add_static(items: Sequence[StockItem]) -> None: ...
 def stock_list_ids() -> list[str]: ...
-def stock_lookup(*args, **kwargs): ...  # FIXME Function
+def stock_lookup(stock_id: str) -> Optional[StockItem]: ...  # CHECK Wrapped function
 def stock_set_translate_func(
     domain: str, func: Callable[..., str], *data: Any
 ) -> None: ...
 def target_table_free(targets: Sequence[TargetEntry]) -> None: ...
 def target_table_new_from_list(list: TargetList) -> list[TargetEntry]: ...
 def targets_include_image(targets: Sequence[Gdk.Atom], writable: bool) -> bool: ...
 def targets_include_rich_text(
@@ -971,48 +972,46 @@
         translator_credits: str
         version: str
         website: str
         website_label: str
         wrap_license: bool
         use_header_bar: int
         accept_focus: bool
-        application: Application
-        attached_to: Widget
+        application: Optional[Application]
+        attached_to: Optional[Widget]
         decorated: bool
         default_height: int
         default_width: int
         deletable: bool
         destroy_with_parent: bool
         focus_on_map: bool
         focus_visible: bool
         gravity: Gdk.Gravity
         has_resize_grip: bool
         has_toplevel_focus: bool
         hide_titlebar_when_maximized: bool
-        icon: GdkPixbuf.Pixbuf
-        icon_name: str
+        icon: Optional[GdkPixbuf.Pixbuf]
+        icon_name: Optional[str]
         is_active: bool
         is_maximized: bool
         mnemonics_visible: bool
         modal: bool
         resizable: bool
         resize_grip_visible: bool
-        role: str
+        role: Optional[str]
         screen: Gdk.Screen
         skip_pager_hint: bool
         skip_taskbar_hint: bool
-        startup_id: str
-        title: str
+        title: Optional[str]
         transient_for: Optional[Window]
         type: WindowType
         type_hint: Gdk.WindowTypeHint
         urgency_hint: bool
         window_position: WindowPosition
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -1032,27 +1031,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        startup_id: str
+        child: Widget
     props: Props = ...
     parent_instance: Dialog = ...
     priv: AboutDialogPrivate = ...
     def __init__(
         self,
         artists: Sequence[str] = ...,
         authors: Sequence[str] = ...,
@@ -1246,27 +1247,26 @@
 class AccelKey(GObject.GPointer):
     accel_key: int = ...
     accel_mods: Gdk.ModifierType = ...
     accel_flags: int = ...
 
 class AccelLabel(Label, Atk.ImplementorIface, Buildable):
     class Props:
-        accel_closure: Callable[..., Any]
-        accel_widget: Widget
+        accel_closure: Optional[Callable[..., Any]]
+        accel_widget: Optional[Widget]
         angle: float
-        attributes: Pango.AttrList
+        attributes: Optional[Pango.AttrList]
         cursor_position: int
         ellipsize: Pango.EllipsizeMode
         justify: Justification
         label: str
         lines: int
         max_width_chars: int
         mnemonic_keyval: int
-        mnemonic_widget: Widget
-        pattern: str
+        mnemonic_widget: Optional[Widget]
         selectable: bool
         selection_bound: int
         single_line_mode: bool
         track_visited_links: bool
         use_markup: bool
         use_underline: bool
         width_chars: int
@@ -1298,27 +1298,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        pattern: str
     props: Props = ...
     label: Label = ...
     priv: AccelLabelPrivate = ...
     def __init__(
         self,
         accel_closure: Callable[..., Any] = ...,
         accel_widget: Widget = ...,
@@ -1449,15 +1450,15 @@
     @staticmethod
     def unlock_path(accel_path: str) -> None: ...
 
 class AccelMapClass(GObject.GPointer): ...
 
 class Accessible(Atk.Object):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -1600,15 +1601,14 @@
     def set_visible_horizontal(self, visible_horizontal: bool) -> None: ...
     def set_visible_vertical(self, visible_vertical: bool) -> None: ...
     def unblock_activate(self) -> None: ...
 
 class ActionBar(Bin, Atk.ImplementorIface, Buildable):
     class Props:
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -1628,27 +1628,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     bin: Bin = ...
     def __init__(
         self,
         border_width: int = ...,
         child: Widget = ...,
         resize_mode: ResizeMode = ...,
@@ -1744,17 +1745,19 @@
         sensitive: bool = ...,
         visible: bool = ...,
     ): ...
     def add_action(self, action: Action) -> None: ...
     def add_action_with_accel(
         self, action: Action, accelerator: Optional[str] = None
     ) -> None: ...
-    def add_actions(self, *args, **kwargs): ...  # FIXME Method
-    def add_radio_actions(self, *args, **kwargs): ...  # FIXME Method
-    def add_toggle_actions(self, *args, **kwargs): ...  # FIXME Method
+    def add_actions(self, entries, user_data=None): ...  # FIXME Function
+    def add_radio_actions(
+        self, entries, value=None, on_change=None, user_data=None
+    ): ...  # FIXME Function
+    def add_toggle_actions(self, entries, user_data=None): ...  # FIXME Function
     def do_get_action(self, action_name: str) -> Action: ...
     def get_accel_group(self) -> AccelGroup: ...
     def get_action(self, action_name: str) -> Action: ...
     def get_name(self) -> str: ...
     def get_sensitive(self) -> bool: ...
     def get_visible(self) -> bool: ...
     def list_actions(self) -> list[Action]: ...
@@ -1884,15 +1887,14 @@
         right_padding: int
         top_padding: int
         xalign: float
         xscale: float
         yalign: float
         yscale: float
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -1912,27 +1914,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     bin: Bin = ...
     priv: AlignmentPrivate = ...
     def __init__(
         self,
         bottom_padding: int = ...,
         left_padding: int = ...,
@@ -2012,19 +2015,19 @@
     def get_content_type(self) -> str: ...
     def refresh(self) -> None: ...
 
 class AppChooserButton(
     ComboBox, Atk.ImplementorIface, AppChooser, Buildable, CellEditable, CellLayout
 ):
     class Props:
-        heading: str
+        heading: Optional[str]
         show_default_item: bool
         show_dialog_item: bool
         active: int
-        active_id: str
+        active_id: Optional[str]
         add_tearoffs: bool
         button_sensitivity: SensitivityType
         cell_area: CellArea
         column_span_column: int
         entry_text_column: int
         has_entry: bool
         has_frame: bool
@@ -2032,15 +2035,14 @@
         model: TreeModel
         popup_fixed_width: bool
         popup_shown: bool
         row_span_column: int
         tearoff_title: str
         wrap_width: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -2060,29 +2062,30 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         content_type: str
         editing_canceled: bool
+        child: Widget
     props: Props = ...
     parent: ComboBox = ...
     priv: AppChooserButtonPrivate = ...
     def __init__(
         self,
         heading: str = ...,
         show_default_item: bool = ...,
@@ -2163,51 +2166,49 @@
     padding: list[None] = ...
 
 class AppChooserButtonPrivate(GObject.GPointer): ...
 
 class AppChooserDialog(Dialog, Atk.ImplementorIface, AppChooser, Buildable):
     class Props:
         gfile: Gio.File
-        heading: str
+        heading: Optional[str]
         use_header_bar: int
         accept_focus: bool
-        application: Application
-        attached_to: Widget
+        application: Optional[Application]
+        attached_to: Optional[Widget]
         decorated: bool
         default_height: int
         default_width: int
         deletable: bool
         destroy_with_parent: bool
         focus_on_map: bool
         focus_visible: bool
         gravity: Gdk.Gravity
         has_resize_grip: bool
         has_toplevel_focus: bool
         hide_titlebar_when_maximized: bool
-        icon: GdkPixbuf.Pixbuf
-        icon_name: str
+        icon: Optional[GdkPixbuf.Pixbuf]
+        icon_name: Optional[str]
         is_active: bool
         is_maximized: bool
         mnemonics_visible: bool
         modal: bool
         resizable: bool
         resize_grip_visible: bool
-        role: str
+        role: Optional[str]
         screen: Gdk.Screen
         skip_pager_hint: bool
         skip_taskbar_hint: bool
-        startup_id: str
-        title: str
+        title: Optional[str]
         transient_for: Optional[Window]
         type: WindowType
         type_hint: Gdk.WindowTypeHint
         urgency_hint: bool
         window_position: WindowPosition
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -2227,28 +2228,30 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         content_type: str
+        startup_id: str
+        child: Widget
     props: Props = ...
     parent: Dialog = ...
     priv: AppChooserDialogPrivate = ...
     def __init__(
         self,
         gfile: Gio.File = ...,
         heading: str = ...,
@@ -2349,15 +2352,14 @@
         show_fallback: bool
         show_other: bool
         show_recommended: bool
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -2377,29 +2379,30 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         content_type: str
         orientation: Orientation
+        child: Widget
     props: Props = ...
     parent: Box = ...
     priv: AppChooserWidgetPrivate = ...
     def __init__(
         self,
         default_text: str = ...,
         show_all: bool = ...,
@@ -2477,27 +2480,27 @@
     populate_popup: Callable[[AppChooserWidget, Menu, Gio.AppInfo], None] = ...
     padding: list[None] = ...
 
 class AppChooserWidgetPrivate(GObject.GPointer): ...
 
 class Application(Gio.Application, Gio.ActionGroup, Gio.ActionMap):
     class Props:
-        active_window: Window
-        app_menu: Gio.MenuModel
+        active_window: Optional[Window]
+        app_menu: Optional[Gio.MenuModel]
         menubar: Gio.MenuModel
         register_session: bool
         screensaver_active: bool
-        action_group: Gio.ActionGroup
-        application_id: str
+        application_id: Optional[str]
         flags: Gio.ApplicationFlags
         inactivity_timeout: int
         is_busy: bool
         is_registered: bool
         is_remote: bool
-        resource_base_path: str
+        resource_base_path: Optional[str]
+        action_group: Optional[Gio.ActionGroup]
     props: Props = ...
     parent: Gio.Application = ...
     priv: ApplicationPrivate = ...
     def __init__(
         self,
         app_menu: Gio.MenuModel = ...,
         menubar: Gio.MenuModel = ...,
@@ -2559,48 +2562,46 @@
 
 class ApplicationWindow(
     Window, Atk.ImplementorIface, Gio.ActionGroup, Gio.ActionMap, Buildable
 ):
     class Props:
         show_menubar: bool
         accept_focus: bool
-        application: Application
-        attached_to: Widget
+        application: Optional[Application]
+        attached_to: Optional[Widget]
         decorated: bool
         default_height: int
         default_width: int
         deletable: bool
         destroy_with_parent: bool
         focus_on_map: bool
         focus_visible: bool
         gravity: Gdk.Gravity
         has_resize_grip: bool
         has_toplevel_focus: bool
         hide_titlebar_when_maximized: bool
-        icon: GdkPixbuf.Pixbuf
-        icon_name: str
+        icon: Optional[GdkPixbuf.Pixbuf]
+        icon_name: Optional[str]
         is_active: bool
         is_maximized: bool
         mnemonics_visible: bool
         modal: bool
         resizable: bool
         resize_grip_visible: bool
-        role: str
+        role: Optional[str]
         screen: Gdk.Screen
         skip_pager_hint: bool
         skip_taskbar_hint: bool
-        startup_id: str
-        title: str
+        title: Optional[str]
         transient_for: Optional[Window]
         type: WindowType
         type_hint: Gdk.WindowTypeHint
         urgency_hint: bool
         window_position: WindowPosition
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -2620,27 +2621,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        startup_id: str
+        child: Widget
     props: Props = ...
     parent_instance: Window = ...
     priv: ApplicationWindowPrivate = ...
     def __init__(
         self,
         show_menubar: bool = ...,
         accept_focus: bool = ...,
@@ -2758,27 +2761,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
     props: Props = ...
     misc: Misc = ...
     priv: ArrowPrivate = ...
     def __init__(
         self,
         arrow_type: ArrowType = ...,
         shadow_type: ShadowType = ...,
@@ -2825,15 +2828,15 @@
     ): ...
     @classmethod
     def new(cls, arrow_type: ArrowType, shadow_type: ShadowType) -> Arrow: ...
     def set(self, arrow_type: ArrowType, shadow_type: ShadowType) -> None: ...
 
 class ArrowAccessible(WidgetAccessible, Atk.Component, Atk.Image):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -2881,21 +2884,20 @@
 
 class AspectFrame(Frame, Atk.ImplementorIface, Buildable):
     class Props:
         obey_child: bool
         ratio: float
         xalign: float
         yalign: float
-        label: str
-        label_widget: Widget
+        label: Optional[str]
+        label_widget: Optional[Widget]
         label_xalign: float
         label_yalign: float
         shadow_type: ShadowType
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -2915,27 +2917,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     frame: Frame = ...
     priv: AspectFramePrivate = ...
     def __init__(
         self,
         obey_child: bool = ...,
         ratio: float = ...,
@@ -3008,48 +3011,46 @@
 
 class AspectFramePrivate(GObject.GPointer): ...
 
 class Assistant(Window, Atk.ImplementorIface, Buildable):
     class Props:
         use_header_bar: int
         accept_focus: bool
-        application: Application
-        attached_to: Widget
+        application: Optional[Application]
+        attached_to: Optional[Widget]
         decorated: bool
         default_height: int
         default_width: int
         deletable: bool
         destroy_with_parent: bool
         focus_on_map: bool
         focus_visible: bool
         gravity: Gdk.Gravity
         has_resize_grip: bool
         has_toplevel_focus: bool
         hide_titlebar_when_maximized: bool
-        icon: GdkPixbuf.Pixbuf
-        icon_name: str
+        icon: Optional[GdkPixbuf.Pixbuf]
+        icon_name: Optional[str]
         is_active: bool
         is_maximized: bool
         mnemonics_visible: bool
         modal: bool
         resizable: bool
         resize_grip_visible: bool
-        role: str
+        role: Optional[str]
         screen: Gdk.Screen
         skip_pager_hint: bool
         skip_taskbar_hint: bool
-        startup_id: str
-        title: str
+        title: Optional[str]
         transient_for: Optional[Window]
         type: WindowType
         type_hint: Gdk.WindowTypeHint
         urgency_hint: bool
         window_position: WindowPosition
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -3069,27 +3070,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        startup_id: str
+        child: Widget
     props: Props = ...
     parent: Window = ...
     priv: AssistantPrivate = ...
     def __init__(
         self,
         use_header_bar: int = ...,
         accept_focus: bool = ...,
@@ -3214,15 +3217,14 @@
     _gtk_reserved5: None = ...
 
 class AssistantPrivate(GObject.GPointer): ...
 
 class Bin(Container, Atk.ImplementorIface, Buildable):
     class Props:
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -3242,27 +3244,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     container: Container = ...
     priv: BinPrivate = ...
     def __init__(
         self,
         border_width: int = ...,
         child: Widget = ...,
@@ -3374,15 +3377,15 @@
     args: list[BindingArg] = ...
 
 class BooleanCellAccessible(
     RendererCellAccessible, Atk.Action, Atk.Component, Atk.TableCell
 ):
     class Props:
         renderer: CellRenderer
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -3432,15 +3435,14 @@
 
 class Box(Container, Atk.ImplementorIface, Buildable, Orientable):
     class Props:
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -3460,28 +3462,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        child: Widget
     props: Props = ...
     container: Container = ...
     priv: BoxPrivate = ...
     def __init__(
         self,
         baseline_position: BaselinePosition = ...,
         homogeneous: bool = ...,
@@ -3677,24 +3680,23 @@
     _gtk_reserved8: None = ...
 
 class BuilderPrivate(GObject.GPointer): ...
 
 class Button(Bin, Atk.ImplementorIface, Actionable, Activatable, Buildable):
     class Props:
         always_show_image: bool
-        image: Widget
+        image: Optional[Widget]
         image_position: PositionType
         label: str
         relief: ReliefStyle
         use_stock: bool
         use_underline: bool
         xalign: float
         yalign: float
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -3714,31 +3716,32 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
+        child: Widget
     props: Props = ...
     bin: Bin = ...
     priv: ButtonPrivate = ...
     def __init__(
         self,
         always_show_image: bool = ...,
         image: Widget = ...,
@@ -3800,15 +3803,15 @@
     def do_leave(self) -> None: ...
     def do_pressed(self) -> None: ...
     def do_released(self) -> None: ...
     def enter(self) -> None: ...
     def get_alignment(self) -> Tuple[float, float]: ...
     def get_always_show_image(self) -> bool: ...
     def get_event_window(self) -> Gdk.Window: ...
-    def get_focus_on_click(self, *args, **kwargs): ...  # FIXME Method
+    def get_focus_on_click(self, *args, **kwargs): ...  # FIXME Function
     def get_image(self) -> Optional[Widget]: ...
     def get_image_position(self) -> PositionType: ...
     def get_label(self) -> str: ...
     def get_relief(self) -> ReliefStyle: ...
     def get_use_stock(self) -> bool: ...
     def get_use_underline(self) -> bool: ...
     def leave(self) -> None: ...
@@ -3822,25 +3825,25 @@
     def new_with_label(cls, label: str) -> Button: ...
     @classmethod
     def new_with_mnemonic(cls, label: str) -> Button: ...
     def pressed(self) -> None: ...
     def released(self) -> None: ...
     def set_alignment(self, xalign: float, yalign: float) -> None: ...
     def set_always_show_image(self, always_show: bool) -> None: ...
-    def set_focus_on_click(self, *args, **kwargs): ...  # FIXME Method
+    def set_focus_on_click(self, *args, **kwargs): ...  # FIXME Function
     def set_image(self, image: Optional[Widget] = None) -> None: ...
     def set_image_position(self, position: PositionType) -> None: ...
     def set_label(self, label: str) -> None: ...
     def set_relief(self, relief: ReliefStyle) -> None: ...
     def set_use_stock(self, use_stock: bool) -> None: ...
     def set_use_underline(self, use_underline: bool) -> None: ...
 
 class ButtonAccessible(ContainerAccessible, Atk.Action, Atk.Component, Atk.Image):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -3880,15 +3883,14 @@
 class ButtonBox(Box, Atk.ImplementorIface, Buildable, Orientable):
     class Props:
         layout_style: ButtonBoxStyle
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -3908,28 +3910,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        child: Widget
     props: Props = ...
     box: Box = ...
     priv: ButtonBoxPrivate = ...
     def __init__(
         self,
         layout_style: ButtonBoxStyle = ...,
         baseline_position: BaselinePosition = ...,
@@ -4045,27 +4048,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
     props: Props = ...
     widget: Widget = ...
     priv: CalendarPrivate = ...
     def __init__(
         self,
         day: int = ...,
         detail_height_rows: int = ...,
@@ -4154,15 +4157,15 @@
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
 
 class CalendarPrivate(GObject.GPointer): ...
 
 class CellAccessible(Accessible, Atk.Action, Atk.Component, Atk.TableCell):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -4660,15 +4663,14 @@
     clear_attributes: Callable[[CellLayout, CellRenderer], None] = ...
     reorder: Callable[[CellLayout, CellRenderer, int], None] = ...
     get_cells: Callable[[CellLayout], list[CellRenderer]] = ...
     get_area: Callable[[CellLayout], Optional[CellArea]] = ...
 
 class CellRenderer(GObject.InitiallyUnowned):
     class Props:
-        cell_background: str
         cell_background_gdk: Gdk.Color
         cell_background_rgba: Gdk.RGBA
         cell_background_set: bool
         editing: bool
         height: int
         is_expanded: bool
         is_expander: bool
@@ -4676,14 +4678,15 @@
         sensitive: bool
         visible: bool
         width: int
         xalign: float
         xpad: int
         yalign: float
         ypad: int
+        cell_background: str
     props: Props = ...
     parent_instance: GObject.InitiallyUnowned = ...
     priv: CellRendererPrivate = ...
     def __init__(
         self,
         cell_background: str = ...,
         cell_background_gdk: Gdk.Color = ...,
@@ -4808,33 +4811,30 @@
         accel_key: int
         accel_mode: CellRendererAccelMode
         accel_mods: Gdk.ModifierType
         keycode: int
         align_set: bool
         alignment: Pango.Alignment
         attributes: Pango.AttrList
-        background: str
         background_gdk: Gdk.Color
         background_rgba: Gdk.RGBA
         background_set: bool
         editable: bool
         editable_set: bool
         ellipsize: Pango.EllipsizeMode
         ellipsize_set: bool
         family: str
         family_set: bool
         font: str
         font_desc: Pango.FontDescription
-        foreground: str
         foreground_gdk: Gdk.Color
         foreground_rgba: Gdk.RGBA
         foreground_set: bool
         language: str
         language_set: bool
-        markup: str
         max_width_chars: int
         placeholder_text: str
         rise: int
         rise_set: bool
         scale: float
         scale_set: bool
         single_paragraph_mode: bool
@@ -4853,15 +4853,14 @@
         variant: Pango.Variant
         variant_set: bool
         weight: int
         weight_set: bool
         width_chars: int
         wrap_mode: Pango.WrapMode
         wrap_width: int
-        cell_background: str
         cell_background_gdk: Gdk.Color
         cell_background_rgba: Gdk.RGBA
         cell_background_set: bool
         editing: bool
         height: int
         is_expanded: bool
         is_expander: bool
@@ -4869,14 +4868,18 @@
         sensitive: bool
         visible: bool
         width: int
         xalign: float
         xpad: int
         yalign: float
         ypad: int
+        background: str
+        foreground: str
+        markup: str
+        cell_background: str
     props: Props = ...
     parent: CellRendererText = ...
     priv: CellRendererAccelPrivate = ...
     def __init__(
         self,
         accel_key: int = ...,
         accel_mode: CellRendererAccelMode = ...,
@@ -5037,33 +5040,30 @@
     class Props:
         has_entry: bool
         model: TreeModel
         text_column: int
         align_set: bool
         alignment: Pango.Alignment
         attributes: Pango.AttrList
-        background: str
         background_gdk: Gdk.Color
         background_rgba: Gdk.RGBA
         background_set: bool
         editable: bool
         editable_set: bool
         ellipsize: Pango.EllipsizeMode
         ellipsize_set: bool
         family: str
         family_set: bool
         font: str
         font_desc: Pango.FontDescription
-        foreground: str
         foreground_gdk: Gdk.Color
         foreground_rgba: Gdk.RGBA
         foreground_set: bool
         language: str
         language_set: bool
-        markup: str
         max_width_chars: int
         placeholder_text: str
         rise: int
         rise_set: bool
         scale: float
         scale_set: bool
         single_paragraph_mode: bool
@@ -5082,15 +5082,14 @@
         variant: Pango.Variant
         variant_set: bool
         weight: int
         weight_set: bool
         width_chars: int
         wrap_mode: Pango.WrapMode
         wrap_width: int
-        cell_background: str
         cell_background_gdk: Gdk.Color
         cell_background_rgba: Gdk.RGBA
         cell_background_set: bool
         editing: bool
         height: int
         is_expanded: bool
         is_expander: bool
@@ -5098,14 +5097,18 @@
         sensitive: bool
         visible: bool
         width: int
         xalign: float
         xpad: int
         yalign: float
         ypad: int
+        background: str
+        foreground: str
+        markup: str
+        cell_background: str
     props: Props = ...
     parent: CellRendererText = ...
     priv: CellRendererComboPrivate = ...
     def __init__(
         self,
         has_entry: bool = ...,
         model: TreeModel = ...,
@@ -5194,15 +5197,14 @@
         pixbuf: GdkPixbuf.Pixbuf
         pixbuf_expander_closed: GdkPixbuf.Pixbuf
         pixbuf_expander_open: GdkPixbuf.Pixbuf
         stock_detail: str
         stock_id: str
         stock_size: int
         surface: cairo.Surface
-        cell_background: str
         cell_background_gdk: Gdk.Color
         cell_background_rgba: Gdk.RGBA
         cell_background_set: bool
         editing: bool
         height: int
         is_expanded: bool
         is_expander: bool
@@ -5210,14 +5212,15 @@
         sensitive: bool
         visible: bool
         width: int
         xalign: float
         xpad: int
         yalign: float
         ypad: int
+        cell_background: str
     props: Props = ...
     parent: CellRenderer = ...
     priv: CellRendererPixbufPrivate = ...
     def __init__(
         self,
         follow_state: bool = ...,
         gicon: Gio.Icon = ...,
@@ -5262,15 +5265,14 @@
     class Props:
         inverted: bool
         pulse: int
         text: str
         text_xalign: float
         text_yalign: float
         value: int
-        cell_background: str
         cell_background_gdk: Gdk.Color
         cell_background_rgba: Gdk.RGBA
         cell_background_set: bool
         editing: bool
         height: int
         is_expanded: bool
         is_expander: bool
@@ -5279,14 +5281,15 @@
         visible: bool
         width: int
         xalign: float
         xpad: int
         yalign: float
         ypad: int
         orientation: Orientation
+        cell_background: str
     props: Props = ...
     parent_instance: CellRenderer = ...
     priv: CellRendererProgressPrivate = ...
     def __init__(
         self,
         inverted: bool = ...,
         pulse: int = ...,
@@ -5327,33 +5330,30 @@
     class Props:
         adjustment: Adjustment
         climb_rate: float
         digits: int
         align_set: bool
         alignment: Pango.Alignment
         attributes: Pango.AttrList
-        background: str
         background_gdk: Gdk.Color
         background_rgba: Gdk.RGBA
         background_set: bool
         editable: bool
         editable_set: bool
         ellipsize: Pango.EllipsizeMode
         ellipsize_set: bool
         family: str
         family_set: bool
         font: str
         font_desc: Pango.FontDescription
-        foreground: str
         foreground_gdk: Gdk.Color
         foreground_rgba: Gdk.RGBA
         foreground_set: bool
         language: str
         language_set: bool
-        markup: str
         max_width_chars: int
         placeholder_text: str
         rise: int
         rise_set: bool
         scale: float
         scale_set: bool
         single_paragraph_mode: bool
@@ -5372,15 +5372,14 @@
         variant: Pango.Variant
         variant_set: bool
         weight: int
         weight_set: bool
         width_chars: int
         wrap_mode: Pango.WrapMode
         wrap_width: int
-        cell_background: str
         cell_background_gdk: Gdk.Color
         cell_background_rgba: Gdk.RGBA
         cell_background_set: bool
         editing: bool
         height: int
         is_expanded: bool
         is_expander: bool
@@ -5388,14 +5387,18 @@
         sensitive: bool
         visible: bool
         width: int
         xalign: float
         xpad: int
         yalign: float
         ypad: int
+        background: str
+        foreground: str
+        markup: str
+        cell_background: str
     props: Props = ...
     parent: CellRendererText = ...
     priv: CellRendererSpinPrivate = ...
     def __init__(
         self,
         adjustment: Adjustment = ...,
         climb_rate: float = ...,
@@ -5477,15 +5480,14 @@
 class CellRendererSpinPrivate(GObject.GPointer): ...
 
 class CellRendererSpinner(CellRenderer):
     class Props:
         active: bool
         pulse: int
         size: IconSize
-        cell_background: str
         cell_background_gdk: Gdk.Color
         cell_background_rgba: Gdk.RGBA
         cell_background_set: bool
         editing: bool
         height: int
         is_expanded: bool
         is_expander: bool
@@ -5493,14 +5495,15 @@
         sensitive: bool
         visible: bool
         width: int
         xalign: float
         xpad: int
         yalign: float
         ypad: int
+        cell_background: str
     props: Props = ...
     parent: CellRenderer = ...
     priv: CellRendererSpinnerPrivate = ...
     def __init__(
         self,
         active: bool = ...,
         pulse: int = ...,
@@ -5534,33 +5537,30 @@
 class CellRendererSpinnerPrivate(GObject.GPointer): ...
 
 class CellRendererText(CellRenderer):
     class Props:
         align_set: bool
         alignment: Pango.Alignment
         attributes: Pango.AttrList
-        background: str
         background_gdk: Gdk.Color
         background_rgba: Gdk.RGBA
         background_set: bool
         editable: bool
         editable_set: bool
         ellipsize: Pango.EllipsizeMode
         ellipsize_set: bool
         family: str
         family_set: bool
         font: str
         font_desc: Pango.FontDescription
-        foreground: str
         foreground_gdk: Gdk.Color
         foreground_rgba: Gdk.RGBA
         foreground_set: bool
         language: str
         language_set: bool
-        markup: str
         max_width_chars: int
         placeholder_text: str
         rise: int
         rise_set: bool
         scale: float
         scale_set: bool
         single_paragraph_mode: bool
@@ -5579,15 +5579,14 @@
         variant: Pango.Variant
         variant_set: bool
         weight: int
         weight_set: bool
         width_chars: int
         wrap_mode: Pango.WrapMode
         wrap_width: int
-        cell_background: str
         cell_background_gdk: Gdk.Color
         cell_background_rgba: Gdk.RGBA
         cell_background_set: bool
         editing: bool
         height: int
         is_expanded: bool
         is_expander: bool
@@ -5595,14 +5594,18 @@
         sensitive: bool
         visible: bool
         width: int
         xalign: float
         xpad: int
         yalign: float
         ypad: int
+        background: str
+        foreground: str
+        markup: str
+        cell_background: str
     props: Props = ...
     parent: CellRenderer = ...
     priv: CellRendererTextPrivate = ...
     def __init__(
         self,
         align_set: bool = ...,
         alignment: Pango.Alignment = ...,
@@ -5686,15 +5689,14 @@
 class CellRendererToggle(CellRenderer):
     class Props:
         activatable: bool
         active: bool
         inconsistent: bool
         indicator_size: int
         radio: bool
-        cell_background: str
         cell_background_gdk: Gdk.Color
         cell_background_rgba: Gdk.RGBA
         cell_background_set: bool
         editing: bool
         height: int
         is_expanded: bool
         is_expander: bool
@@ -5702,14 +5704,15 @@
         sensitive: bool
         visible: bool
         width: int
         xalign: float
         xpad: int
         yalign: float
         ypad: int
+        cell_background: str
     props: Props = ...
     parent: CellRenderer = ...
     priv: CellRendererTogglePrivate = ...
     def __init__(
         self,
         activatable: bool = ...,
         active: bool = ...,
@@ -5750,23 +5753,22 @@
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
 
 class CellRendererTogglePrivate(GObject.GPointer): ...
 
 class CellView(Widget, Atk.ImplementorIface, Buildable, CellLayout, Orientable):
     class Props:
-        background: str
         background_gdk: Gdk.Color
         background_rgba: Gdk.RGBA
         background_set: bool
         cell_area: CellArea
         cell_area_context: CellAreaContext
         draw_sensitive: bool
         fit_model: bool
-        model: TreeModel
+        model: Optional[TreeModel]
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
         expand: bool
@@ -5785,28 +5787,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        background: str
     props: Props = ...
     parent_instance: Widget = ...
     priv: CellViewPrivate = ...
     def __init__(
         self,
         background: str = ...,
         background_gdk: Gdk.Color = ...,
@@ -5890,24 +5893,23 @@
     ToggleButton, Atk.ImplementorIface, Actionable, Activatable, Buildable
 ):
     class Props:
         active: bool
         draw_indicator: bool
         inconsistent: bool
         always_show_image: bool
-        image: Widget
+        image: Optional[Widget]
         image_position: PositionType
         label: str
         relief: ReliefStyle
         use_stock: bool
         use_underline: bool
         xalign: float
         yalign: float
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -5927,31 +5929,32 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
+        child: Widget
     props: Props = ...
     toggle_button: ToggleButton = ...
     def __init__(
         self,
         active: bool = ...,
         draw_indicator: bool = ...,
         inconsistent: bool = ...,
@@ -6025,21 +6028,20 @@
     _gtk_reserved4: None = ...
 
 class CheckMenuItem(MenuItem, Atk.ImplementorIface, Actionable, Activatable, Buildable):
     class Props:
         active: bool
         draw_as_radio: bool
         inconsistent: bool
-        accel_path: str
+        accel_path: Optional[str]
         label: str
         right_justified: bool
-        submenu: Menu
+        submenu: Optional[Menu]
         use_underline: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -6059,31 +6061,32 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
+        child: Widget
     props: Props = ...
     menu_item: MenuItem = ...
     priv: CheckMenuItemPrivate = ...
     def __init__(
         self,
         active: bool = ...,
         draw_as_radio: bool = ...,
@@ -6153,15 +6156,15 @@
     def set_inconsistent(self, setting: bool) -> None: ...
     def toggled(self) -> None: ...
 
 class CheckMenuItemAccessible(
     MenuItemAccessible, Atk.Action, Atk.Component, Atk.Selection
 ):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -6215,14 +6218,15 @@
     def get(selection: Gdk.Atom) -> Clipboard: ...
     @staticmethod
     def get_default(display: Gdk.Display) -> Clipboard: ...
     def get_display(self) -> Gdk.Display: ...
     @staticmethod
     def get_for_display(display: Gdk.Display, selection: Gdk.Atom) -> Clipboard: ...
     def get_owner(self) -> Optional[GObject.Object]: ...
+    def get_selection(self) -> Gdk.Atom: ...
     def request_contents(
         self, target: Gdk.Atom, callback: Callable[..., None], *user_data: Any
     ) -> None: ...
     def request_image(self, callback: Callable[..., None], *user_data: Any) -> None: ...
     def request_rich_text(
         self, buffer: TextBuffer, callback: Callable[..., None], *user_data: Any
     ) -> None: ...
@@ -6258,24 +6262,23 @@
         alpha: int
         color: Gdk.Color
         rgba: Gdk.RGBA
         show_editor: bool
         title: str
         use_alpha: bool
         always_show_image: bool
-        image: Widget
+        image: Optional[Widget]
         image_position: PositionType
         label: str
         relief: ReliefStyle
         use_stock: bool
         use_underline: bool
         xalign: float
         yalign: float
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -6295,31 +6298,32 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
+        child: Widget
     props: Props = ...
     button: Button = ...
     priv: ColorButtonPrivate = ...
     def __init__(
         self,
         alpha: int = ...,
         color: Gdk.Color = ...,
@@ -6420,48 +6424,46 @@
     def set_use_alpha(self, use_alpha: bool) -> None: ...
 
 class ColorChooserDialog(Dialog, Atk.ImplementorIface, Buildable, ColorChooser):
     class Props:
         show_editor: bool
         use_header_bar: int
         accept_focus: bool
-        application: Application
-        attached_to: Widget
+        application: Optional[Application]
+        attached_to: Optional[Widget]
         decorated: bool
         default_height: int
         default_width: int
         deletable: bool
         destroy_with_parent: bool
         focus_on_map: bool
         focus_visible: bool
         gravity: Gdk.Gravity
         has_resize_grip: bool
         has_toplevel_focus: bool
         hide_titlebar_when_maximized: bool
-        icon: GdkPixbuf.Pixbuf
-        icon_name: str
+        icon: Optional[GdkPixbuf.Pixbuf]
+        icon_name: Optional[str]
         is_active: bool
         is_maximized: bool
         mnemonics_visible: bool
         modal: bool
         resizable: bool
         resize_grip_visible: bool
-        role: str
+        role: Optional[str]
         screen: Gdk.Screen
         skip_pager_hint: bool
         skip_taskbar_hint: bool
-        startup_id: str
-        title: str
+        title: Optional[str]
         transient_for: Optional[Window]
         type: WindowType
         type_hint: Gdk.WindowTypeHint
         urgency_hint: bool
         window_position: WindowPosition
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -6481,29 +6483,31 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         rgba: Gdk.RGBA
         use_alpha: bool
+        startup_id: str
+        child: Widget
     props: Props = ...
     parent_instance: Dialog = ...
     priv: ColorChooserDialogPrivate = ...
     def __init__(
         self,
         show_editor: bool = ...,
         use_header_bar: int = ...,
@@ -6607,15 +6611,14 @@
 ):
     class Props:
         show_editor: bool
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -6635,30 +6638,31 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         rgba: Gdk.RGBA
         use_alpha: bool
         orientation: Orientation
+        child: Widget
     props: Props = ...
     parent_instance: Box = ...
     priv: ColorChooserWidgetPrivate = ...
     def __init__(
         self,
         show_editor: bool = ...,
         baseline_position: BaselinePosition = ...,
@@ -6730,15 +6734,14 @@
         current_rgba: Gdk.RGBA
         has_opacity_control: bool
         has_palette: bool
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -6758,28 +6761,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        child: Widget
     props: Props = ...
     parent_instance: Box = ...
     private_data: ColorSelectionPrivate = ...
     def __init__(
         self,
         current_alpha: int = ...,
         current_color: Gdk.Color = ...,
@@ -6867,48 +6871,46 @@
     class Props:
         cancel_button: Widget
         color_selection: Widget
         help_button: Widget
         ok_button: Widget
         use_header_bar: int
         accept_focus: bool
-        application: Application
-        attached_to: Widget
+        application: Optional[Application]
+        attached_to: Optional[Widget]
         decorated: bool
         default_height: int
         default_width: int
         deletable: bool
         destroy_with_parent: bool
         focus_on_map: bool
         focus_visible: bool
         gravity: Gdk.Gravity
         has_resize_grip: bool
         has_toplevel_focus: bool
         hide_titlebar_when_maximized: bool
-        icon: GdkPixbuf.Pixbuf
-        icon_name: str
+        icon: Optional[GdkPixbuf.Pixbuf]
+        icon_name: Optional[str]
         is_active: bool
         is_maximized: bool
         mnemonics_visible: bool
         modal: bool
         resizable: bool
         resize_grip_visible: bool
-        role: str
+        role: Optional[str]
         screen: Gdk.Screen
         skip_pager_hint: bool
         skip_taskbar_hint: bool
-        startup_id: str
-        title: str
+        title: Optional[str]
         transient_for: Optional[Window]
         type: WindowType
         type_hint: Gdk.WindowTypeHint
         urgency_hint: bool
         window_position: WindowPosition
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -6928,27 +6930,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        startup_id: str
+        child: Widget
     props: Props = ...
     parent_instance: Dialog = ...
     priv: ColorSelectionDialogPrivate = ...
     def __init__(
         self,
         use_header_bar: int = ...,
         accept_focus: bool = ...,
@@ -7033,15 +7037,15 @@
 
 class ColorSelectionDialogPrivate(GObject.GPointer): ...
 class ColorSelectionPrivate(GObject.GPointer): ...
 
 class ComboBox(Bin, Atk.ImplementorIface, Buildable, CellEditable, CellLayout):
     class Props:
         active: int
-        active_id: str
+        active_id: Optional[str]
         add_tearoffs: bool
         button_sensitivity: SensitivityType
         cell_area: CellArea
         column_span_column: int
         entry_text_column: int
         has_entry: bool
         has_frame: bool
@@ -7049,15 +7053,14 @@
         model: TreeModel
         popup_fixed_width: bool
         popup_shown: bool
         row_span_column: int
         tearoff_title: str
         wrap_width: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -7077,28 +7080,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         editing_canceled: bool
+        child: Widget
     props: Props = ...
     parent_instance: Bin = ...
     priv: ComboBoxPrivate = ...
     def __init__(
         self,
         active: int = ...,
         active_id: str = ...,
@@ -7204,15 +7208,15 @@
     def set_row_separator_func(self, func: Callable[..., bool], *data: Any) -> None: ...
     def set_row_span_column(self, row_span: int) -> None: ...
     def set_title(self, title: str) -> None: ...
     def set_wrap_width(self, width: int) -> None: ...
 
 class ComboBoxAccessible(ContainerAccessible, Atk.Action, Atk.Component, Atk.Selection):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -7258,15 +7262,15 @@
     _gtk_reserved3: None = ...
 
 class ComboBoxPrivate(GObject.GPointer): ...
 
 class ComboBoxText(ComboBox, Atk.ImplementorIface, Buildable, CellEditable, CellLayout):
     class Props:
         active: int
-        active_id: str
+        active_id: Optional[str]
         add_tearoffs: bool
         button_sensitivity: SensitivityType
         cell_area: CellArea
         column_span_column: int
         entry_text_column: int
         has_entry: bool
         has_frame: bool
@@ -7274,15 +7278,14 @@
         model: TreeModel
         popup_fixed_width: bool
         popup_shown: bool
         row_span_column: int
         tearoff_title: str
         wrap_width: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -7302,28 +7305,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         editing_canceled: bool
+        child: Widget
     props: Props = ...
     parent_instance: ComboBox = ...
     priv: ComboBoxTextPrivate = ...
     def __init__(
         self,
         active: int = ...,
         active_id: str = ...,
@@ -7403,15 +7407,14 @@
     _gtk_reserved4: None = ...
 
 class ComboBoxTextPrivate(GObject.GPointer): ...
 
 class Container(Widget, Atk.ImplementorIface, Buildable):
     class Props:
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -7431,27 +7434,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     widget: Widget = ...
     priv: ContainerPrivate = ...
     def __init__(
         self,
         border_width: int = ...,
         child: Widget = ...,
@@ -7491,21 +7495,23 @@
         vexpand: bool = ...,
         vexpand_set: bool = ...,
         visible: bool = ...,
         width_request: int = ...,
     ): ...
     def add(self, widget: Widget) -> None: ...
     def check_resize(self) -> None: ...
-    def child_get(self, *args, **kwargs): ...  # FIXME Method
-    def child_get_property(self, *args, **kwargs): ...  # FIXME Method
+    def child_get(self, child, *prop_names): ...  # FIXME Function
+    def child_get_property(
+        self, child, property_name, value=None
+    ): ...  # FIXME Function
     def child_notify(self, child: Widget, child_property: str) -> None: ...
     def child_notify_by_pspec(
         self, child: Widget, pspec: GObject.ParamSpec
     ) -> None: ...
-    def child_set(self, *args, **kwargs): ...  # FIXME Method
+    def child_set(self, child, **kwargs): ...  # FIXME Function
     def child_set_property(
         self, child: Widget, property_name: str, value: Any
     ) -> None: ...
     def child_type(self) -> Type: ...
     def do_add(self, widget: Widget) -> None: ...
     def do_check_resize(self) -> None: ...
     def do_child_type(self) -> Type: ...
@@ -7528,15 +7534,15 @@
     def find_child_property(
         self, property_name: str
     ) -> Optional[GObject.ParamSpec]: ...
     def forall(self, callback: Callable[..., None], *callback_data: Any) -> None: ...
     def foreach(self, callback: Callable[..., None], *callback_data: Any) -> None: ...
     def get_border_width(self) -> int: ...
     def get_children(self) -> list[Widget]: ...
-    def get_focus_chain(self, *args, **kwargs): ...  # FIXME Method
+    def get_focus_chain(self) -> Optional[list[Widget]]: ...  # CHECK Wrapped function
     def get_focus_child(self) -> Optional[Widget]: ...
     def get_focus_hadjustment(self) -> Optional[Adjustment]: ...
     def get_focus_vadjustment(self) -> Optional[Adjustment]: ...
     def get_path_for_child(self, child: Widget) -> WidgetPath: ...
     def get_resize_mode(self) -> ResizeMode: ...
     def handle_border_width(self) -> None: ...
     def install_child_properties(
@@ -7558,15 +7564,15 @@
     def set_focus_vadjustment(self, adjustment: Adjustment) -> None: ...
     def set_reallocate_redraws(self, needs_redraws: bool) -> None: ...
     def set_resize_mode(self, resize_mode: ResizeMode) -> None: ...
     def unset_focus_chain(self) -> None: ...
 
 class ContainerAccessible(WidgetAccessible, Atk.Component):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -7603,15 +7609,15 @@
     add_gtk: Callable[[Container, Widget, None], int] = ...
     remove_gtk: Callable[[Container, Widget, None], int] = ...
 
 class ContainerAccessiblePrivate(GObject.GPointer): ...
 
 class ContainerCellAccessible(CellAccessible, Atk.Action, Atk.Component, Atk.TableCell):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -7728,48 +7734,46 @@
     def ref(self) -> CssSection: ...
     def unref(self) -> None: ...
 
 class Dialog(Window, Atk.ImplementorIface, Buildable):
     class Props:
         use_header_bar: int
         accept_focus: bool
-        application: Application
-        attached_to: Widget
+        application: Optional[Application]
+        attached_to: Optional[Widget]
         decorated: bool
         default_height: int
         default_width: int
         deletable: bool
         destroy_with_parent: bool
         focus_on_map: bool
         focus_visible: bool
         gravity: Gdk.Gravity
         has_resize_grip: bool
         has_toplevel_focus: bool
         hide_titlebar_when_maximized: bool
-        icon: GdkPixbuf.Pixbuf
-        icon_name: str
+        icon: Optional[GdkPixbuf.Pixbuf]
+        icon_name: Optional[str]
         is_active: bool
         is_maximized: bool
         mnemonics_visible: bool
         modal: bool
         resizable: bool
         resize_grip_visible: bool
-        role: str
+        role: Optional[str]
         screen: Gdk.Screen
         skip_pager_hint: bool
         skip_taskbar_hint: bool
-        startup_id: str
-        title: str
+        title: Optional[str]
         transient_for: Optional[Window]
         type: WindowType
         type_hint: Gdk.WindowTypeHint
         urgency_hint: bool
         window_position: WindowPosition
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -7789,27 +7793,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        startup_id: str
+        child: Widget
     props: Props = ...
     window: Window = ...
     priv: DialogPrivate = ...
     def __init__(
         self,
         use_header_bar: int = ...,
         accept_focus: bool = ...,
@@ -7883,26 +7889,26 @@
     ): ...
     _old_arg_names = ...  # FIXME Constant
     action_area = ...  # FIXME Constant
     vbox = ...  # FIXME Constant
 
     def add_action_widget(self, child: Widget, response_id: int) -> None: ...
     def add_button(self, button_text: str, response_id: int) -> Widget: ...
-    def add_buttons(self, *args, **kwargs): ...  # FIXME Method
+    def add_buttons(self, *args): ...  # FIXME Function
     def do_close(self) -> None: ...
     def do_response(self, response_id: int) -> None: ...
     def get_action_area(self) -> Box: ...
     def get_content_area(self) -> Box: ...
     def get_header_bar(self) -> HeaderBar: ...
     def get_response_for_widget(self, widget: Widget) -> int: ...
     def get_widget_for_response(self, response_id: int) -> Optional[Widget]: ...
     @classmethod
     def new(cls) -> Dialog: ...
     def response(self, response_id: int) -> None: ...
-    def run(self, *args, **kwargs): ...  # FIXME Method
+    def run(self, *args, **kwargs): ...  # FIXME Function
     def set_alternative_button_order_from_array(
         self, n_params: int, new_order: Sequence[int]
     ) -> None: ...
     def set_default_response(self, response_id: int) -> None: ...
     def set_response_sensitive(self, response_id: int, setting: bool) -> None: ...
 
 class DialogClass(GObject.GPointer):
@@ -7940,27 +7946,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
     props: Props = ...
     widget: Widget = ...
     dummy: None = ...
     def __init__(
         self,
         app_paintable: bool = ...,
         can_default: bool = ...,
@@ -8013,16 +8019,18 @@
     def copy_clipboard(self) -> None: ...
     def cut_clipboard(self) -> None: ...
     def delete_selection(self) -> None: ...
     def delete_text(self, start_pos: int, end_pos: int) -> None: ...
     def get_chars(self, start_pos: int, end_pos: int) -> str: ...
     def get_editable(self) -> bool: ...
     def get_position(self) -> int: ...
-    def get_selection_bounds(self, *args, **kwargs): ...  # FIXME Method
-    def insert_text(self, *args, **kwargs): ...  # FIXME Method
+    def get_selection_bounds(
+        self,
+    ) -> Tuple[int, int] | Tuple[()]: ...  # CHECK Wrapped function
+    def insert_text(self, text, position): ...  # FIXME Function
     def paste_clipboard(self) -> None: ...
     def select_region(self, start_pos: int, end_pos: int) -> None: ...
     def set_editable(self, is_editable: bool) -> None: ...
     def set_position(self, position: int) -> None: ...
 
 class EditableInterface(GObject.GPointer):
     base_iface: GObject.TypeInterface = ...
@@ -8036,24 +8044,24 @@
     get_selection_bounds: Callable[[Editable], Tuple[bool, int, int]] = ...
     set_position: Callable[[Editable, int], None] = ...
     get_position: Callable[[Editable], int] = ...
 
 class Entry(Widget, Atk.ImplementorIface, Buildable, CellEditable, Editable):
     class Props:
         activates_default: bool
-        attributes: Pango.AttrList
+        attributes: Optional[Pango.AttrList]
         buffer: EntryBuffer
         caps_lock_warning: bool
         completion: EntryCompletion
         cursor_position: int
         editable: bool
         enable_emoji_completion: bool
         has_frame: bool
         im_module: str
-        inner_border: Border
+        inner_border: Optional[Border]
         input_hints: InputHints
         input_purpose: InputPurpose
         invisible_char: int
         invisible_char_set: bool
         max_length: int
         max_width_chars: int
         overwrite_mode: bool
@@ -8079,15 +8087,15 @@
         secondary_icon_stock: str
         secondary_icon_storage_type: ImageType
         secondary_icon_tooltip_markup: str
         secondary_icon_tooltip_text: str
         selection_bound: int
         shadow_type: ShadowType
         show_emoji_icon: bool
-        tabs: Pango.TabArray
+        tabs: Optional[Pango.TabArray]
         text: str
         text_length: int
         truncate_multiline: bool
         visibility: bool
         width_chars: int
         xalign: float
         app_paintable: bool
@@ -8112,27 +8120,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         editing_canceled: bool
     props: Props = ...
     parent_instance: Widget = ...
     priv: EntryPrivate = ...
     def __init__(
         self,
         activates_default: bool = ...,
@@ -8339,15 +8347,15 @@
     def text_index_to_layout_index(self, text_index: int) -> int: ...
     def unset_invisible_char(self) -> None: ...
 
 class EntryAccessible(
     WidgetAccessible, Atk.Action, Atk.Component, Atk.EditableText, Atk.Text
 ):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -8455,15 +8463,15 @@
 
 class EntryCompletion(GObject.Object, Buildable, CellLayout):
     class Props:
         cell_area: CellArea
         inline_completion: bool
         inline_selection: bool
         minimum_key_length: int
-        model: TreeModel
+        model: Optional[TreeModel]
         popup_completion: bool
         popup_set_width: bool
         popup_single_match: bool
         text_column: int
     props: Props = ...
     parent_instance: GObject.Object = ...
     priv: EntryCompletionPrivate = ...
@@ -8564,15 +8572,14 @@
 class EntryPrivate(GObject.GPointer): ...
 
 class EventBox(Bin, Atk.ImplementorIface, Buildable):
     class Props:
         above_child: bool
         visible_window: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -8592,27 +8599,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     bin: Bin = ...
     priv: EventBoxPrivate = ...
     def __init__(
         self,
         above_child: bool = ...,
         visible_window: bool = ...,
@@ -8738,23 +8746,22 @@
     def set_flags(self, flags: EventControllerScrollFlags) -> None: ...
 
 class EventControllerScrollClass(GObject.GPointer): ...
 
 class Expander(Bin, Atk.ImplementorIface, Buildable):
     class Props:
         expanded: bool
-        label: str
+        label: Optional[str]
         label_fill: bool
-        label_widget: Widget
+        label_widget: Optional[Widget]
         resize_toplevel: bool
         spacing: int
         use_markup: bool
         use_underline: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -8774,27 +8781,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     bin: Bin = ...
     priv: ExpanderPrivate = ...
     def __init__(
         self,
         expanded: bool = ...,
         label: str = ...,
@@ -8864,15 +8872,15 @@
     def set_resize_toplevel(self, resize_toplevel: bool) -> None: ...
     def set_spacing(self, spacing: int) -> None: ...
     def set_use_markup(self, use_markup: bool) -> None: ...
     def set_use_underline(self, use_underline: bool) -> None: ...
 
 class ExpanderAccessible(ContainerAccessible, Atk.Action, Atk.Component):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -8990,22 +8998,20 @@
     def unselect_all(self) -> None: ...
     def unselect_file(self, file: Gio.File) -> None: ...
     def unselect_filename(self, filename: str) -> None: ...
     def unselect_uri(self, uri: str) -> None: ...
 
 class FileChooserButton(Box, Atk.ImplementorIface, Buildable, FileChooser, Orientable):
     class Props:
-        dialog: FileChooser
         title: str
         width_chars: int
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -9025,39 +9031,41 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         action: FileChooserAction
         create_folders: bool
         do_overwrite_confirmation: bool
-        extra_widget: Widget
-        filter: FileFilter
+        extra_widget: Optional[Widget]
+        filter: Optional[FileFilter]
         local_only: bool
-        preview_widget: Widget
+        preview_widget: Optional[Widget]
         preview_widget_active: bool
         select_multiple: bool
         show_hidden: bool
         use_preview_label: bool
         orientation: Orientation
+        dialog: FileChooser
+        child: Widget
     props: Props = ...
     parent: Box = ...
     priv: FileChooserButtonPrivate = ...
     def __init__(
         self,
         dialog: FileChooser = ...,
         title: str = ...,
@@ -9139,48 +9147,46 @@
 
 class FileChooserButtonPrivate(GObject.GPointer): ...
 
 class FileChooserDialog(Dialog, Atk.ImplementorIface, Buildable, FileChooser):
     class Props:
         use_header_bar: int
         accept_focus: bool
-        application: Application
-        attached_to: Widget
+        application: Optional[Application]
+        attached_to: Optional[Widget]
         decorated: bool
         default_height: int
         default_width: int
         deletable: bool
         destroy_with_parent: bool
         focus_on_map: bool
         focus_visible: bool
         gravity: Gdk.Gravity
         has_resize_grip: bool
         has_toplevel_focus: bool
         hide_titlebar_when_maximized: bool
-        icon: GdkPixbuf.Pixbuf
-        icon_name: str
+        icon: Optional[GdkPixbuf.Pixbuf]
+        icon_name: Optional[str]
         is_active: bool
         is_maximized: bool
         mnemonics_visible: bool
         modal: bool
         resizable: bool
         resize_grip_visible: bool
-        role: str
+        role: Optional[str]
         screen: Gdk.Screen
         skip_pager_hint: bool
         skip_taskbar_hint: bool
-        startup_id: str
-        title: str
+        title: Optional[str]
         transient_for: Optional[Window]
         type: WindowType
         type_hint: Gdk.WindowTypeHint
         urgency_hint: bool
         window_position: WindowPosition
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -9200,38 +9206,40 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         action: FileChooserAction
         create_folders: bool
         do_overwrite_confirmation: bool
-        extra_widget: Widget
-        filter: FileFilter
+        extra_widget: Optional[Widget]
+        filter: Optional[FileFilter]
         local_only: bool
-        preview_widget: Widget
+        preview_widget: Optional[Widget]
         preview_widget_active: bool
         select_multiple: bool
         show_hidden: bool
         use_preview_label: bool
+        startup_id: str
+        child: Widget
     props: Props = ...
     parent_instance: Dialog = ...
     priv: FileChooserDialogPrivate = ...
     def __init__(
         self,
         use_header_bar: int = ...,
         accept_focus: bool = ...,
@@ -9322,27 +9330,27 @@
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
 
 class FileChooserDialogPrivate(GObject.GPointer): ...
 
 class FileChooserNative(NativeDialog, FileChooser):
     class Props:
-        accept_label: str
-        cancel_label: str
+        accept_label: Optional[str]
+        cancel_label: Optional[str]
         modal: bool
-        title: str
+        title: Optional[str]
         transient_for: Optional[Window]
         visible: bool
         action: FileChooserAction
         create_folders: bool
         do_overwrite_confirmation: bool
-        extra_widget: Widget
-        filter: FileFilter
+        extra_widget: Optional[Widget]
+        filter: Optional[FileFilter]
         local_only: bool
-        preview_widget: Widget
+        preview_widget: Optional[Widget]
         preview_widget_active: bool
         select_multiple: bool
         show_hidden: bool
         use_preview_label: bool
     props: Props = ...
     def __init__(
         self,
@@ -9385,15 +9393,14 @@
     class Props:
         search_mode: bool
         subtitle: str
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -9413,39 +9420,40 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         action: FileChooserAction
         create_folders: bool
         do_overwrite_confirmation: bool
-        extra_widget: Widget
-        filter: FileFilter
+        extra_widget: Optional[Widget]
+        filter: Optional[FileFilter]
         local_only: bool
-        preview_widget: Widget
+        preview_widget: Optional[Widget]
         preview_widget_active: bool
         select_multiple: bool
         show_hidden: bool
         use_preview_label: bool
         orientation: Orientation
+        child: Widget
     props: Props = ...
     parent_instance: Box = ...
     priv: FileChooserWidgetPrivate = ...
     def __init__(
         self,
         search_mode: bool = ...,
         baseline_position: BaselinePosition = ...,
@@ -9504,15 +9512,15 @@
         orientation: Orientation = ...,
     ): ...
     @classmethod
     def new(cls, action: FileChooserAction) -> FileChooserWidget: ...
 
 class FileChooserWidgetAccessible(ContainerAccessible, Atk.Action, Atk.Component):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -9581,15 +9589,14 @@
     uri: str = ...
     display_name: str = ...
     mime_type: str = ...
 
 class Fixed(Container, Atk.ImplementorIface, Buildable):
     class Props:
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -9609,27 +9616,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     container: Container = ...
     priv: FixedPrivate = ...
     def __init__(
         self,
         border_width: int = ...,
         child: Widget = ...,
@@ -9696,15 +9704,14 @@
         column_spacing: int
         homogeneous: bool
         max_children_per_line: int
         min_children_per_line: int
         row_spacing: int
         selection_mode: SelectionMode
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -9724,28 +9731,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        child: Widget
     props: Props = ...
     container: Container = ...
     def __init__(
         self,
         activate_on_single_click: bool = ...,
         column_spacing: int = ...,
         homogeneous: bool = ...,
@@ -9841,15 +9849,15 @@
     ) -> None: ...
     def set_vadjustment(self, adjustment: Adjustment) -> None: ...
     def unselect_all(self) -> None: ...
     def unselect_child(self, child: FlowBoxChild) -> None: ...
 
 class FlowBoxAccessible(ContainerAccessible, Atk.Component, Atk.Selection):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -9885,15 +9893,14 @@
     parent_class: ContainerAccessibleClass = ...
 
 class FlowBoxAccessiblePrivate(GObject.GPointer): ...
 
 class FlowBoxChild(Bin, Atk.ImplementorIface, Buildable):
     class Props:
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -9913,27 +9920,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     parent_instance: Bin = ...
     def __init__(
         self,
         border_width: int = ...,
         child: Widget = ...,
         resize_mode: ResizeMode = ...,
@@ -9979,15 +9987,15 @@
     def get_index(self) -> int: ...
     def is_selected(self) -> bool: ...
     @classmethod
     def new(cls) -> FlowBoxChild: ...
 
 class FlowBoxChildAccessible(ContainerAccessible, Atk.Component):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -10050,24 +10058,23 @@
         font_name: str
         show_size: bool
         show_style: bool
         title: str
         use_font: bool
         use_size: bool
         always_show_image: bool
-        image: Widget
+        image: Optional[Widget]
         image_position: PositionType
         label: str
         relief: ReliefStyle
         use_stock: bool
         use_underline: bool
         xalign: float
         yalign: float
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -10087,38 +10094,39 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
-        font: str
-        font_desc: Pango.FontDescription
+        font: Optional[str]
+        font_desc: Optional[Pango.FontDescription]
         font_features: str
         language: str
         level: FontChooserLevel
         preview_text: str
         show_preview_entry: bool
+        child: Widget
     props: Props = ...
     button: Button = ...
     priv: FontButtonPrivate = ...
     def __init__(
         self,
         font_name: str = ...,
         show_size: bool = ...,
@@ -10236,48 +10244,46 @@
     def set_preview_text(self, text: str) -> None: ...
     def set_show_preview_entry(self, show_preview_entry: bool) -> None: ...
 
 class FontChooserDialog(Dialog, Atk.ImplementorIface, Buildable, FontChooser):
     class Props:
         use_header_bar: int
         accept_focus: bool
-        application: Application
-        attached_to: Widget
+        application: Optional[Application]
+        attached_to: Optional[Widget]
         decorated: bool
         default_height: int
         default_width: int
         deletable: bool
         destroy_with_parent: bool
         focus_on_map: bool
         focus_visible: bool
         gravity: Gdk.Gravity
         has_resize_grip: bool
         has_toplevel_focus: bool
         hide_titlebar_when_maximized: bool
-        icon: GdkPixbuf.Pixbuf
-        icon_name: str
+        icon: Optional[GdkPixbuf.Pixbuf]
+        icon_name: Optional[str]
         is_active: bool
         is_maximized: bool
         mnemonics_visible: bool
         modal: bool
         resizable: bool
         resize_grip_visible: bool
-        role: str
+        role: Optional[str]
         screen: Gdk.Screen
         skip_pager_hint: bool
         skip_taskbar_hint: bool
-        startup_id: str
-        title: str
+        title: Optional[str]
         transient_for: Optional[Window]
         type: WindowType
         type_hint: Gdk.WindowTypeHint
         urgency_hint: bool
         window_position: WindowPosition
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -10297,34 +10303,36 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        font: str
-        font_desc: Pango.FontDescription
+        window: Optional[Gdk.Window]
+        font: Optional[str]
+        font_desc: Optional[Pango.FontDescription]
         font_features: str
         language: str
         level: FontChooserLevel
         preview_text: str
         show_preview_entry: bool
+        startup_id: str
+        child: Widget
     props: Props = ...
     parent_instance: Dialog = ...
     priv: FontChooserDialogPrivate = ...
     def __init__(
         self,
         use_header_bar: int = ...,
         accept_focus: bool = ...,
@@ -10430,15 +10438,14 @@
 class FontChooserWidget(Box, Atk.ImplementorIface, Buildable, FontChooser, Orientable):
     class Props:
         tweak_action: Gio.Action
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -10458,35 +10465,36 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        font: str
-        font_desc: Pango.FontDescription
+        window: Optional[Gdk.Window]
+        font: Optional[str]
+        font_desc: Optional[Pango.FontDescription]
         font_features: str
         language: str
         level: FontChooserLevel
         preview_text: str
         show_preview_entry: bool
         orientation: Orientation
+        child: Widget
     props: Props = ...
     parent_instance: Box = ...
     priv: FontChooserWidgetPrivate = ...
     def __init__(
         self,
         baseline_position: BaselinePosition = ...,
         homogeneous: bool = ...,
@@ -10558,15 +10566,14 @@
     class Props:
         font_name: str
         preview_text: str
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -10586,28 +10593,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        child: Widget
     props: Props = ...
     parent_instance: Box = ...
     priv: FontSelectionPrivate = ...
     def __init__(
         self,
         font_name: str = ...,
         preview_text: str = ...,
@@ -10677,48 +10685,46 @@
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
 
 class FontSelectionDialog(Dialog, Atk.ImplementorIface, Buildable):
     class Props:
         use_header_bar: int
         accept_focus: bool
-        application: Application
-        attached_to: Widget
+        application: Optional[Application]
+        attached_to: Optional[Widget]
         decorated: bool
         default_height: int
         default_width: int
         deletable: bool
         destroy_with_parent: bool
         focus_on_map: bool
         focus_visible: bool
         gravity: Gdk.Gravity
         has_resize_grip: bool
         has_toplevel_focus: bool
         hide_titlebar_when_maximized: bool
-        icon: GdkPixbuf.Pixbuf
-        icon_name: str
+        icon: Optional[GdkPixbuf.Pixbuf]
+        icon_name: Optional[str]
         is_active: bool
         is_maximized: bool
         mnemonics_visible: bool
         modal: bool
         resizable: bool
         resize_grip_visible: bool
-        role: str
+        role: Optional[str]
         screen: Gdk.Screen
         skip_pager_hint: bool
         skip_taskbar_hint: bool
-        startup_id: str
-        title: str
+        title: Optional[str]
         transient_for: Optional[Window]
         type: WindowType
         type_hint: Gdk.WindowTypeHint
         urgency_hint: bool
         window_position: WindowPosition
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -10738,27 +10744,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        startup_id: str
+        child: Widget
     props: Props = ...
     parent_instance: Dialog = ...
     priv: FontSelectionDialogPrivate = ...
     def __init__(
         self,
         use_header_bar: int = ...,
         accept_focus: bool = ...,
@@ -10848,21 +10856,20 @@
     _gtk_reserved4: None = ...
 
 class FontSelectionDialogPrivate(GObject.GPointer): ...
 class FontSelectionPrivate(GObject.GPointer): ...
 
 class Frame(Bin, Atk.ImplementorIface, Buildable):
     class Props:
-        label: str
-        label_widget: Widget
+        label: Optional[str]
+        label_widget: Optional[Widget]
         label_xalign: float
         label_yalign: float
         shadow_type: ShadowType
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -10882,27 +10889,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     bin: Bin = ...
     priv: FramePrivate = ...
     def __init__(
         self,
         label: str = ...,
         label_widget: Widget = ...,
@@ -10959,15 +10967,15 @@
     def set_label(self, label: Optional[str] = None) -> None: ...
     def set_label_align(self, xalign: float, yalign: float) -> None: ...
     def set_label_widget(self, label_widget: Optional[Widget] = None) -> None: ...
     def set_shadow_type(self, type: ShadowType) -> None: ...
 
 class FrameAccessible(ContainerAccessible, Atk.Component):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -11044,27 +11052,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
     props: Props = ...
     parent_instance: Widget = ...
     def __init__(
         self,
         auto_render: bool = ...,
         has_alpha: bool = ...,
         has_depth_buffer: bool = ...,
@@ -11136,15 +11144,15 @@
     resize: Callable[[GLArea, int, int], None] = ...
     create_context: None = ...
     _padding: list[None] = ...
 
 class Gesture(EventController):
     class Props:
         n_points: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         propagation_phase: PropagationPhase
         widget: Widget
     props: Props = ...
     def __init__(
         self,
         n_points: int = ...,
         window: Gdk.Window = ...,
@@ -11183,15 +11191,15 @@
 
 class GestureDrag(GestureSingle):
     class Props:
         button: int
         exclusive: bool
         touch_only: bool
         n_points: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         propagation_phase: PropagationPhase
         widget: Widget
     props: Props = ...
     def __init__(
         self,
         button: int = ...,
         exclusive: bool = ...,
@@ -11211,15 +11219,15 @@
 class GestureLongPress(GestureSingle):
     class Props:
         delay_factor: float
         button: int
         exclusive: bool
         touch_only: bool
         n_points: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         propagation_phase: PropagationPhase
         widget: Widget
     props: Props = ...
     def __init__(
         self,
         delay_factor: float = ...,
         button: int = ...,
@@ -11237,15 +11245,15 @@
 
 class GestureMultiPress(GestureSingle):
     class Props:
         button: int
         exclusive: bool
         touch_only: bool
         n_points: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         propagation_phase: PropagationPhase
         widget: Widget
     props: Props = ...
     def __init__(
         self,
         button: int = ...,
         exclusive: bool = ...,
@@ -11265,15 +11273,15 @@
 class GesturePan(GestureDrag):
     class Props:
         orientation: Orientation
         button: int
         exclusive: bool
         touch_only: bool
         n_points: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         propagation_phase: PropagationPhase
         widget: Widget
     props: Props = ...
     def __init__(
         self,
         orientation: Orientation = ...,
         button: int = ...,
@@ -11290,15 +11298,15 @@
     def set_orientation(self, orientation: Orientation) -> None: ...
 
 class GesturePanClass(GObject.GPointer): ...
 
 class GestureRotate(Gesture):
     class Props:
         n_points: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         propagation_phase: PropagationPhase
         widget: Widget
     props: Props = ...
     def __init__(
         self,
         n_points: int = ...,
         window: Gdk.Window = ...,
@@ -11313,15 +11321,15 @@
 
 class GestureSingle(Gesture):
     class Props:
         button: int
         exclusive: bool
         touch_only: bool
         n_points: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         propagation_phase: PropagationPhase
         widget: Widget
     props: Props = ...
     def __init__(
         self,
         button: int = ...,
         exclusive: bool = ...,
@@ -11344,15 +11352,15 @@
 
 class GestureStylus(GestureSingle):
     class Props:
         button: int
         exclusive: bool
         touch_only: bool
         n_points: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         propagation_phase: PropagationPhase
         widget: Widget
     props: Props = ...
     def __init__(
         self,
         button: int = ...,
         exclusive: bool = ...,
@@ -11372,15 +11380,15 @@
 
 class GestureSwipe(GestureSingle):
     class Props:
         button: int
         exclusive: bool
         touch_only: bool
         n_points: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         propagation_phase: PropagationPhase
         widget: Widget
     props: Props = ...
     def __init__(
         self,
         button: int = ...,
         exclusive: bool = ...,
@@ -11395,15 +11403,15 @@
     def new(cls, widget: Widget) -> GestureSwipe: ...
 
 class GestureSwipeClass(GObject.GPointer): ...
 
 class GestureZoom(Gesture):
     class Props:
         n_points: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         propagation_phase: PropagationPhase
         widget: Widget
     props: Props = ...
     def __init__(
         self,
         n_points: int = ...,
         window: Gdk.Window = ...,
@@ -11434,15 +11442,14 @@
     class Props:
         baseline_row: int
         column_homogeneous: bool
         column_spacing: int
         row_homogeneous: bool
         row_spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -11462,28 +11469,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        child: Widget
     props: Props = ...
     container: Container = ...
     priv: GridPrivate = ...
     def __init__(
         self,
         baseline_row: int = ...,
         column_homogeneous: bool = ...,
@@ -11578,15 +11586,14 @@
 
 class HBox(Box, Atk.ImplementorIface, Buildable, Orientable):
     class Props:
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -11606,28 +11613,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        child: Widget
     props: Props = ...
     box: Box = ...
     def __init__(
         self,
         baseline_position: BaselinePosition = ...,
         homogeneous: bool = ...,
         spacing: int = ...,
@@ -11681,15 +11689,14 @@
 class HButtonBox(ButtonBox, Atk.ImplementorIface, Buildable, Orientable):
     class Props:
         layout_style: ButtonBoxStyle
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -11709,28 +11716,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        child: Widget
     props: Props = ...
     button_box: ButtonBox = ...
     def __init__(
         self,
         layout_style: ButtonBoxStyle = ...,
         baseline_position: BaselinePosition = ...,
         homogeneous: bool = ...,
@@ -11786,15 +11794,14 @@
     class Props:
         max_position: int
         min_position: int
         position: int
         position_set: bool
         wide_handle: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -11814,28 +11821,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        child: Widget
     props: Props = ...
     paned: Paned = ...
     def __init__(
         self,
         position: int = ...,
         position_set: bool = ...,
         wide_handle: bool = ...,
@@ -11910,27 +11918,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
     props: Props = ...
     parent_instance: Widget = ...
     priv: HSVPrivate = ...
     def __init__(
         self,
         app_paintable: bool = ...,
         can_default: bool = ...,
@@ -12028,27 +12036,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
     props: Props = ...
     scale: Scale = ...
     def __init__(
         self,
         digits: int = ...,
         draw_value: bool = ...,
@@ -12140,27 +12148,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
     props: Props = ...
     scrollbar: Scrollbar = ...
     def __init__(
         self,
         adjustment: Adjustment = ...,
         fill_level: float = ...,
@@ -12238,27 +12246,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
     props: Props = ...
     separator: Separator = ...
     def __init__(
         self,
         app_paintable: bool = ...,
         can_default: bool = ...,
@@ -12308,15 +12316,14 @@
     class Props:
         child_detached: bool
         handle_position: PositionType
         shadow_type: ShadowType
         snap_edge: PositionType
         snap_edge_set: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -12336,27 +12343,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     bin: Bin = ...
     priv: HandleBoxPrivate = ...
     def __init__(
         self,
         handle_position: PositionType = ...,
         shadow_type: ShadowType = ...,
@@ -12423,24 +12431,23 @@
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
 
 class HandleBoxPrivate(GObject.GPointer): ...
 
 class HeaderBar(Container, Atk.ImplementorIface, Buildable):
     class Props:
-        custom_title: Widget
+        custom_title: Optional[Widget]
         decoration_layout: str
         decoration_layout_set: bool
         has_subtitle: bool
         show_close_button: bool
         spacing: int
-        subtitle: str
-        title: str
+        subtitle: Optional[str]
+        title: Optional[str]
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -12460,27 +12467,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     container: Container = ...
     def __init__(
         self,
         custom_title: Widget = ...,
         decoration_layout: str = ...,
         decoration_layout_set: bool = ...,
@@ -12544,15 +12552,15 @@
     def set_has_subtitle(self, setting: bool) -> None: ...
     def set_show_close_button(self, setting: bool) -> None: ...
     def set_subtitle(self, subtitle: Optional[str] = None) -> None: ...
     def set_title(self, title: Optional[str] = None) -> None: ...
 
 class HeaderBarAccessible(ContainerAccessible, Atk.Component):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -12623,15 +12631,17 @@
     def do_set_cursor_location(self, area: Gdk.Rectangle) -> None: ...
     def do_set_surrounding(self, text: str, len: int, cursor_index: int) -> None: ...
     def do_set_use_preedit(self, use_preedit: bool) -> None: ...
     def filter_keypress(self, event: Gdk.EventKey) -> bool: ...
     def focus_in(self) -> None: ...
     def focus_out(self) -> None: ...
     def get_preedit_string(self) -> Tuple[str, Pango.AttrList, int]: ...
-    def get_surrounding(self, *args, **kwargs): ...  # FIXME Method
+    def get_surrounding(
+        self,
+    ) -> Optional[Tuple[str, int]]: ...  # CHECK Wrapped function
     def reset(self) -> None: ...
     def set_client_window(self, window: Optional[Gdk.Window] = None) -> None: ...
     def set_cursor_location(self, area: Gdk.Rectangle) -> None: ...
     def set_surrounding(self, text: str, len: int, cursor_index: int) -> None: ...
     def set_use_preedit(self, use_preedit: bool) -> None: ...
 
 class IMContextClass(GObject.GPointer):
@@ -12740,15 +12750,17 @@
     def get_embedded_rect(self) -> Tuple[bool, Gdk.Rectangle]: ...
     def get_filename(self) -> Optional[str]: ...
     def is_symbolic(self) -> bool: ...
     def load_icon(self) -> GdkPixbuf.Pixbuf: ...
     def load_icon_async(
         self,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[Callable[..., None]] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
         *user_data: Any,
     ) -> None: ...
     def load_icon_finish(self, res: Gio.AsyncResult) -> GdkPixbuf.Pixbuf: ...
     # override
     def load_surface(
         self, for_window: Optional[Gdk.Window] = None
     ) -> cairo.ImageSurface: ...
@@ -12762,28 +12774,32 @@
     def load_symbolic_async(
         self,
         fg: Gdk.RGBA,
         success_color: Optional[Gdk.RGBA] = None,
         warning_color: Optional[Gdk.RGBA] = None,
         error_color: Optional[Gdk.RGBA] = None,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[Callable[..., None]] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
         *user_data: Any,
     ) -> None: ...
     def load_symbolic_finish(
         self, res: Gio.AsyncResult
     ) -> Tuple[GdkPixbuf.Pixbuf, bool]: ...
     def load_symbolic_for_context(
         self, context: StyleContext
     ) -> Tuple[GdkPixbuf.Pixbuf, bool]: ...
     def load_symbolic_for_context_async(
         self,
         context: StyleContext,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[Callable[..., None]] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
         *user_data: Any,
     ) -> None: ...
     def load_symbolic_for_context_finish(
         self, res: Gio.AsyncResult
     ) -> Tuple[GdkPixbuf.Pixbuf, bool]: ...
     def load_symbolic_for_style(
         self, style: Style, state: StateType
@@ -12928,24 +12944,23 @@
         column_spacing: int
         columns: int
         item_orientation: Orientation
         item_padding: int
         item_width: int
         margin: int
         markup_column: int
-        model: TreeModel
+        model: Optional[TreeModel]
         pixbuf_column: int
         reorderable: bool
         row_spacing: int
         selection_mode: SelectionMode
         spacing: int
         text_column: int
         tooltip_column: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -12964,31 +12979,32 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         hadjustment: Adjustment
         hscroll_policy: ScrollablePolicy
         vadjustment: Adjustment
         vscroll_policy: ScrollablePolicy
+        child: Widget
     props: Props = ...
     parent: Container = ...
     priv: IconViewPrivate = ...
     def __init__(
         self,
         activate_on_single_click: bool = ...,
         cell_area: CellArea = ...,
@@ -13074,17 +13090,21 @@
     def get_activate_on_single_click(self) -> bool: ...
     def get_cell_rect(
         self, path: TreePath, cell: Optional[CellRenderer] = None
     ) -> Tuple[bool, Gdk.Rectangle]: ...
     def get_column_spacing(self) -> int: ...
     def get_columns(self) -> int: ...
     def get_cursor(self) -> Tuple[bool, TreePath, CellRenderer]: ...
-    def get_dest_item_at_pos(self, *args, **kwargs): ...  # FIXME Method
+    def get_dest_item_at_pos(
+        self, drag_x: int, drag_y: int
+    ) -> Optional[Tuple[TreePath, IconViewDropPosition]]: ...  # CHECK Wrapped function
     def get_drag_dest_item(self) -> Tuple[TreePath, IconViewDropPosition]: ...
-    def get_item_at_pos(self, *args, **kwargs): ...  # FIXME Method
+    def get_item_at_pos(
+        self, x: int, y: int
+    ) -> Optional[Tuple[TreePath, CellRenderer]]: ...  # CHECK Wrapped function
     def get_item_column(self, path: TreePath) -> int: ...
     def get_item_orientation(self) -> Orientation: ...
     def get_item_padding(self) -> int: ...
     def get_item_row(self, path: TreePath) -> int: ...
     def get_item_width(self) -> int: ...
     def get_margin(self) -> int: ...
     def get_markup_column(self) -> int: ...
@@ -13097,15 +13117,17 @@
     def get_selection_mode(self) -> SelectionMode: ...
     def get_spacing(self) -> int: ...
     def get_text_column(self) -> int: ...
     def get_tooltip_column(self) -> int: ...
     def get_tooltip_context(
         self, keyboard_tip: bool
     ) -> Tuple[bool, int, int, TreeModel, TreePath, TreeIter]: ...
-    def get_visible_range(self, *args, **kwargs): ...  # FIXME Method
+    def get_visible_range(
+        self,
+    ) -> Optional[Tuple[TreePath, TreePath]]: ...  # CHECK Wrapped function
     def item_activated(self, path: TreePath) -> None: ...
     @classmethod
     def new(cls) -> IconView: ...
     @classmethod
     def new_with_area(cls, area: CellArea) -> IconView: ...
     @classmethod
     def new_with_model(cls, model: TreeModel) -> IconView: ...
@@ -13145,15 +13167,15 @@
     def unselect_all(self) -> None: ...
     def unselect_path(self, path: TreePath) -> None: ...
     def unset_model_drag_dest(self) -> None: ...
     def unset_model_drag_source(self) -> None: ...
 
 class IconViewAccessible(ContainerAccessible, Atk.Component, Atk.Selection):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -13210,15 +13232,15 @@
 class Image(Misc, Atk.ImplementorIface, Buildable):
     class Props:
         file: str
         gicon: Gio.Icon
         icon_name: str
         icon_set: IconSet
         icon_size: int
-        pixbuf: GdkPixbuf.Pixbuf
+        pixbuf: Optional[GdkPixbuf.Pixbuf]
         pixbuf_animation: GdkPixbuf.PixbufAnimation
         pixel_size: int
         resource: str
         stock: str
         storage_type: ImageType
         surface: cairo.Surface
         use_fallback: bool
@@ -13248,27 +13270,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
     props: Props = ...
     misc: Misc = ...
     priv: ImagePrivate = ...
     def __init__(
         self,
         file: str = ...,
         gicon: Gio.Icon = ...,
@@ -13361,15 +13383,15 @@
     def set_from_resource(self, resource_path: Optional[str] = None) -> None: ...
     def set_from_stock(self, stock_id: str, size: int) -> None: ...
     def set_from_surface(self, surface: Optional[cairo.Surface] = None) -> None: ...
     def set_pixel_size(self, pixel_size: int) -> None: ...
 
 class ImageAccessible(WidgetAccessible, Atk.Component, Atk.Image):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -13407,15 +13429,15 @@
 class ImageAccessiblePrivate(GObject.GPointer): ...
 
 class ImageCellAccessible(
     RendererCellAccessible, Atk.Action, Atk.Component, Atk.Image, Atk.TableCell
 ):
     class Props:
         renderer: CellRenderer
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -13458,25 +13480,23 @@
     _gtk_reserved1: None = ...
     _gtk_reserved2: None = ...
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
 
 class ImageMenuItem(MenuItem, Atk.ImplementorIface, Actionable, Activatable, Buildable):
     class Props:
-        accel_group: AccelGroup
         always_show_image: bool
         image: Widget
         use_stock: bool
-        accel_path: str
+        accel_path: Optional[str]
         label: str
         right_justified: bool
-        submenu: Menu
+        submenu: Optional[Menu]
         use_underline: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -13496,31 +13516,33 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
+        accel_group: AccelGroup
+        child: Widget
     props: Props = ...
     menu_item: MenuItem = ...
     priv: ImageMenuItemPrivate = ...
     def __init__(
         self,
         accel_group: AccelGroup = ...,
         always_show_image: bool = ...,
@@ -13608,15 +13630,14 @@
         message_type: MessageType
         revealed: bool
         show_close_button: bool
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -13636,28 +13657,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        child: Widget
     props: Props = ...
     parent: Box = ...
     priv: InfoBarPrivate = ...
     def __init__(
         self,
         message_type: MessageType = ...,
         revealed: bool = ...,
@@ -13760,27 +13782,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
     props: Props = ...
     widget: Widget = ...
     priv: InvisiblePrivate = ...
     def __init__(
         self,
         screen: Gdk.Screen = ...,
         app_paintable: bool = ...,
@@ -13835,24 +13857,23 @@
     _gtk_reserved4: None = ...
 
 class InvisiblePrivate(GObject.GPointer): ...
 
 class Label(Misc, Atk.ImplementorIface, Buildable):
     class Props:
         angle: float
-        attributes: Pango.AttrList
+        attributes: Optional[Pango.AttrList]
         cursor_position: int
         ellipsize: Pango.EllipsizeMode
         justify: Justification
         label: str
         lines: int
         max_width_chars: int
         mnemonic_keyval: int
-        mnemonic_widget: Widget
-        pattern: str
+        mnemonic_widget: Optional[Widget]
         selectable: bool
         selection_bound: int
         single_line_mode: bool
         track_visited_links: bool
         use_markup: bool
         use_underline: bool
         width_chars: int
@@ -13884,27 +13905,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        pattern: str
     props: Props = ...
     misc: Misc = ...
     priv: LabelPrivate = ...
     def __init__(
         self,
         angle: float = ...,
         attributes: Pango.AttrList = ...,
@@ -14021,15 +14043,15 @@
     def set_use_underline(self, setting: bool) -> None: ...
     def set_width_chars(self, n_chars: int) -> None: ...
     def set_xalign(self, xalign: float) -> None: ...
     def set_yalign(self, yalign: float) -> None: ...
 
 class LabelAccessible(WidgetAccessible, Atk.Component, Atk.Hypertext, Atk.Text):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -14085,15 +14107,14 @@
 class LabelSelectionInfo(GObject.GPointer): ...
 
 class Layout(Container, Atk.ImplementorIface, Buildable, Scrollable):
     class Props:
         height: int
         width: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -14113,31 +14134,32 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         hadjustment: Adjustment
         hscroll_policy: ScrollablePolicy
         vadjustment: Adjustment
         vscroll_policy: ScrollablePolicy
+        child: Widget
     props: Props = ...
     container: Container = ...
     priv: LayoutPrivate = ...
     def __init__(
         self,
         height: int = ...,
         width: int = ...,
@@ -14239,27 +14261,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
     props: Props = ...
     parent: Widget = ...
     priv: LevelBarPrivate = ...
     def __init__(
         self,
         inverted: bool = ...,
@@ -14322,15 +14344,15 @@
     def set_max_value(self, value: float) -> None: ...
     def set_min_value(self, value: float) -> None: ...
     def set_mode(self, mode: LevelBarMode) -> None: ...
     def set_value(self, value: float) -> None: ...
 
 class LevelBarAccessible(WidgetAccessible, Atk.Component, Atk.Value):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -14375,24 +14397,23 @@
 class LevelBarPrivate(GObject.GPointer): ...
 
 class LinkButton(Button, Atk.ImplementorIface, Actionable, Activatable, Buildable):
     class Props:
         uri: str
         visited: bool
         always_show_image: bool
-        image: Widget
+        image: Optional[Widget]
         image_position: PositionType
         label: str
         relief: ReliefStyle
         use_stock: bool
         use_underline: bool
         xalign: float
         yalign: float
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -14412,31 +14433,32 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
+        child: Widget
     props: Props = ...
     parent_instance: Button = ...
     priv: LinkButtonPrivate = ...
     def __init__(
         self,
         uri: str = ...,
         visited: bool = ...,
@@ -14503,15 +14525,15 @@
     def set_uri(self, uri: str) -> None: ...
     def set_visited(self, visited: bool) -> None: ...
 
 class LinkButtonAccessible(
     ButtonAccessible, Atk.Action, Atk.Component, Atk.HyperlinkImpl, Atk.Image
 ):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -14559,15 +14581,14 @@
 class LinkButtonPrivate(GObject.GPointer): ...
 
 class ListBox(Container, Atk.ImplementorIface, Buildable):
     class Props:
         activate_on_single_click: bool
         selection_mode: SelectionMode
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -14587,27 +14608,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     parent_instance: Container = ...
     def __init__(
         self,
         activate_on_single_click: bool = ...,
         selection_mode: SelectionMode = ...,
         border_width: int = ...,
@@ -14698,15 +14720,15 @@
         self, sort_func: Optional[Callable[..., int]] = None, *user_data: Any
     ) -> None: ...
     def unselect_all(self) -> None: ...
     def unselect_row(self, row: ListBoxRow) -> None: ...
 
 class ListBoxAccessible(ContainerAccessible, Atk.Component, Atk.Selection):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -14758,15 +14780,14 @@
     _gtk_reserved3: None = ...
 
 class ListBoxRow(Bin, Atk.ImplementorIface, Actionable, Buildable):
     class Props:
         activatable: bool
         selectable: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -14786,29 +14807,30 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
+        child: Widget
     props: Props = ...
     parent_instance: Bin = ...
     def __init__(
         self,
         activatable: bool = ...,
         selectable: bool = ...,
         border_width: int = ...,
@@ -14864,15 +14886,15 @@
     def new(cls) -> ListBoxRow: ...
     def set_activatable(self, activatable: bool) -> None: ...
     def set_header(self, header: Optional[Widget] = None) -> None: ...
     def set_selectable(self, selectable: bool) -> None: ...
 
 class ListBoxRowAccessible(ContainerAccessible, Atk.Component):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -14914,22 +14936,23 @@
 
 # override
 class ListStore(
     GObject.Object, Buildable, TreeDragDest, TreeDragSource, TreeModel, TreeSortable
 ):
     parent: GObject.Object = ...
     priv: ListStorePrivate = ...
+
     def __init__(self, *args: Any) -> None: ...
     def append(
         self, row: Union[list[Any], tuple[Any, ...], None] = None
     ) -> TreeIter: ...
     def clear(self) -> None: ...
-    def insert(self, *args, **kwargs): ...  # FIXME Method
-    def insert_after(self, *args, **kwargs): ...  # FIXME Method
-    def insert_before(self, *args, **kwargs): ...  # FIXME Method
+    def insert(self, *args, **kwargs): ...
+    def insert_after(self, *args, **kwargs): ...
+    def insert_before(self, *args, **kwargs): ...
     def insert_with_values(
         self, position: int, columns: Sequence[int], values: Sequence[Any]
     ) -> TreeIter: ...
     def insert_with_valuesv(
         self, position: int, columns: Sequence[int], values: Sequence[Any]
     ) -> TreeIter: ...
     def iter_is_valid(self, iter: TreeIter) -> bool: ...
@@ -14970,24 +14993,23 @@
         permission: Gio.Permission
         text_lock: str
         text_unlock: str
         tooltip_lock: str
         tooltip_not_authorized: str
         tooltip_unlock: str
         always_show_image: bool
-        image: Widget
+        image: Optional[Widget]
         image_position: PositionType
         label: str
         relief: ReliefStyle
         use_stock: bool
         use_underline: bool
         xalign: float
         yalign: float
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -15007,31 +15029,32 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
+        child: Widget
     props: Props = ...
     parent: Button = ...
     priv: LockButtonPrivate = ...
     def __init__(
         self,
         permission: Gio.Permission = ...,
         text_lock: str = ...,
@@ -15095,15 +15118,15 @@
     def get_permission(self) -> Gio.Permission: ...
     @classmethod
     def new(cls, permission: Optional[Gio.Permission] = None) -> LockButton: ...
     def set_permission(self, permission: Optional[Gio.Permission] = None) -> None: ...
 
 class LockButtonAccessible(ButtonAccessible, Atk.Action, Atk.Component, Atk.Image):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -15165,15 +15188,14 @@
         rect_anchor_dx: int
         rect_anchor_dy: int
         reserve_toggle_size: bool
         tearoff_state: bool
         tearoff_title: str
         take_focus: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -15193,27 +15215,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     menu_shell: MenuShell = ...
     priv: MenuPrivate = ...
     def __init__(
         self,
         accel_group: AccelGroup = ...,
         accel_path: str = ...,
@@ -15343,15 +15366,15 @@
     def set_reserve_toggle_size(self, reserve_toggle_size: bool) -> None: ...
     def set_screen(self, screen: Optional[Gdk.Screen] = None) -> None: ...
     def set_tearoff_state(self, torn_off: bool) -> None: ...
     def set_title(self, title: Optional[str] = None) -> None: ...
 
 class MenuAccessible(MenuShellAccessible, Atk.Component, Atk.Selection):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -15390,15 +15413,14 @@
 
 class MenuBar(MenuShell, Atk.ImplementorIface, Buildable):
     class Props:
         child_pack_direction: PackDirection
         pack_direction: PackDirection
         take_focus: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -15418,27 +15440,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     menu_shell: MenuShell = ...
     priv: MenuBarPrivate = ...
     def __init__(
         self,
         child_pack_direction: PackDirection = ...,
         pack_direction: PackDirection = ...,
@@ -15501,34 +15524,33 @@
 
 class MenuBarPrivate(GObject.GPointer): ...
 
 class MenuButton(
     ToggleButton, Atk.ImplementorIface, Actionable, Activatable, Buildable
 ):
     class Props:
-        align_widget: Container
+        align_widget: Optional[Container]
         direction: ArrowType
-        menu_model: Gio.MenuModel
-        popover: Popover
-        popup: Menu
+        menu_model: Optional[Gio.MenuModel]
+        popover: Optional[Popover]
+        popup: Optional[Menu]
         use_popover: bool
         active: bool
         draw_indicator: bool
         inconsistent: bool
         always_show_image: bool
-        image: Widget
+        image: Optional[Widget]
         image_position: PositionType
         label: str
         relief: ReliefStyle
         use_stock: bool
         use_underline: bool
         xalign: float
         yalign: float
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -15548,31 +15570,32 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
+        child: Widget
     props: Props = ...
     parent: ToggleButton = ...
     priv: MenuButtonPrivate = ...
     def __init__(
         self,
         align_widget: Container = ...,
         direction: ArrowType = ...,
@@ -15651,15 +15674,15 @@
     def set_popup(self, menu: Optional[Widget] = None) -> None: ...
     def set_use_popover(self, use_popover: bool) -> None: ...
 
 class MenuButtonAccessible(
     ToggleButtonAccessible, Atk.Action, Atk.Component, Atk.Image
 ):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -15710,21 +15733,20 @@
     _gtk_reserved1: None = ...
     _gtk_reserved2: None = ...
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
 
 class MenuItem(Bin, Atk.ImplementorIface, Actionable, Activatable, Buildable):
     class Props:
-        accel_path: str
+        accel_path: Optional[str]
         label: str
         right_justified: bool
-        submenu: Menu
+        submenu: Optional[Menu]
         use_underline: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -15744,31 +15766,32 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
+        child: Widget
     props: Props = ...
     bin: Bin = ...
     priv: MenuItemPrivate = ...
     def __init__(
         self,
         accel_path: str = ...,
         label: str = ...,
@@ -15849,15 +15872,15 @@
     def set_submenu(self, submenu: Optional[Menu] = None) -> None: ...
     def set_use_underline(self, setting: bool) -> None: ...
     def toggle_size_allocate(self, allocation: int) -> None: ...
     def toggle_size_request(self) -> int: ...
 
 class MenuItemAccessible(ContainerAccessible, Atk.Action, Atk.Component, Atk.Selection):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -15913,15 +15936,14 @@
 class MenuItemPrivate(GObject.GPointer): ...
 class MenuPrivate(GObject.GPointer): ...
 
 class MenuShell(Container, Atk.ImplementorIface, Buildable):
     class Props:
         take_focus: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -15941,27 +15963,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     container: Container = ...
     priv: MenuShellPrivate = ...
     def __init__(
         self,
         take_focus: bool = ...,
         border_width: int = ...,
@@ -16031,15 +16054,15 @@
     def prepend(self, child: Widget) -> None: ...
     def select_first(self, search_sensitive: bool) -> None: ...
     def select_item(self, menu_item: Widget) -> None: ...
     def set_take_focus(self, take_focus: bool) -> None: ...
 
 class MenuShellAccessible(ContainerAccessible, Atk.Component, Atk.Selection):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -16096,25 +16119,24 @@
 class MenuShellPrivate(GObject.GPointer): ...
 
 class MenuToolButton(
     ToolButton, Atk.ImplementorIface, Actionable, Activatable, Buildable
 ):
     class Props:
         menu: Menu
-        icon_name: str
-        icon_widget: Widget
-        label: str
-        label_widget: Widget
+        icon_name: Optional[str]
+        icon_widget: Optional[Widget]
+        label: Optional[str]
+        label_widget: Optional[Widget]
         stock_id: str
         use_underline: bool
         is_important: bool
         visible_horizontal: bool
         visible_vertical: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -16134,31 +16156,32 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
+        child: Widget
     props: Props = ...
     parent: ToolButton = ...
     priv: MenuToolButtonPrivate = ...
     def __init__(
         self,
         menu: Menu = ...,
         icon_name: str = ...,
@@ -16234,58 +16257,55 @@
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
 
 class MenuToolButtonPrivate(GObject.GPointer): ...
 
 class MessageDialog(Dialog, Atk.ImplementorIface, Buildable):
     class Props:
-        buttons: ButtonsType
         image: Widget
         message_area: Widget
         message_type: MessageType
         secondary_text: Optional[str]
         secondary_use_markup: bool
         text: str
         use_markup: bool
         use_header_bar: int
         accept_focus: bool
-        application: Application
-        attached_to: Widget
+        application: Optional[Application]
+        attached_to: Optional[Widget]
         decorated: bool
         default_height: int
         default_width: int
         deletable: bool
         destroy_with_parent: bool
         focus_on_map: bool
         focus_visible: bool
         gravity: Gdk.Gravity
         has_resize_grip: bool
         has_toplevel_focus: bool
         hide_titlebar_when_maximized: bool
-        icon: GdkPixbuf.Pixbuf
-        icon_name: str
+        icon: Optional[GdkPixbuf.Pixbuf]
+        icon_name: Optional[str]
         is_active: bool
         is_maximized: bool
         mnemonics_visible: bool
         modal: bool
         resizable: bool
         resize_grip_visible: bool
-        role: str
+        role: Optional[str]
         screen: Gdk.Screen
         skip_pager_hint: bool
         skip_taskbar_hint: bool
-        startup_id: str
-        title: str
+        title: Optional[str]
         transient_for: Optional[Window]
         type: WindowType
         type_hint: Gdk.WindowTypeHint
         urgency_hint: bool
         window_position: WindowPosition
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -16305,27 +16325,30 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        buttons: ButtonsType
+        startup_id: str
+        child: Widget
     props: Props = ...
     parent_instance: Dialog = ...
     priv: MessageDialogPrivate = ...
     def __init__(
         self,
         buttons: ButtonsType = ...,
         image: Widget = ...,
@@ -16450,27 +16473,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
     props: Props = ...
     widget: Widget = ...
     priv: MiscPrivate = ...
     def __init__(
         self,
         xalign: float = ...,
         xpad: int = ...,
@@ -16535,24 +16558,23 @@
         iconic: bool
         inverted: bool
         menu_name: str
         role: ButtonRole
         text: str
         use_markup: bool
         always_show_image: bool
-        image: Widget
+        image: Optional[Widget]
         image_position: PositionType
         label: str
         relief: ReliefStyle
         use_stock: bool
         use_underline: bool
         xalign: float
         yalign: float
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -16572,31 +16594,32 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
+        child: Widget
     props: Props = ...
     def __init__(
         self,
         active: bool = ...,
         centered: bool = ...,
         icon: Gio.Icon = ...,
         iconic: bool = ...,
@@ -16664,21 +16687,21 @@
 class MountOperation(Gio.MountOperation):
     class Props:
         is_showing: bool
         parent: Window
         screen: Gdk.Screen
         anonymous: bool
         choice: int
-        domain: str
+        domain: Optional[str]
         is_tcrypt_hidden_volume: bool
         is_tcrypt_system_volume: bool
-        password: str
+        password: Optional[str]
         password_save: Gio.PasswordSave
         pim: int
-        username: str
+        username: Optional[str]
     props: Props = ...
     parent_instance: Gio.MountOperation = ...
     priv: MountOperationPrivate = ...
     def __init__(
         self,
         parent: Window = ...,
         screen: Gdk.Screen = ...,
@@ -16708,15 +16731,15 @@
     _gtk_reserved4: None = ...
 
 class MountOperationPrivate(GObject.GPointer): ...
 
 class NativeDialog(GObject.Object):
     class Props:
         modal: bool
-        title: str
+        title: Optional[str]
         transient_for: Optional[Window]
         visible: bool
     props: Props = ...
     parent_instance: GObject.Object = ...
     def __init__(
         self,
         modal: bool = ...,
@@ -16748,22 +16771,21 @@
     _gtk_reserved2: None = ...
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
 
 class Notebook(Container, Atk.ImplementorIface, Buildable):
     class Props:
         enable_popup: bool
-        group_name: str
+        group_name: Optional[str]
         page: int
         scrollable: bool
         show_border: bool
         show_tabs: bool
         tab_pos: PositionType
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -16783,27 +16805,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     container: Container = ...
     priv: NotebookPrivate = ...
     def __init__(
         self,
         enable_popup: bool = ...,
         group_name: str = ...,
@@ -16933,15 +16956,15 @@
     ) -> None: ...
     def set_tab_label_text(self, child: Widget, tab_text: str) -> None: ...
     def set_tab_pos(self, pos: PositionType) -> None: ...
     def set_tab_reorderable(self, child: Widget, reorderable: bool) -> None: ...
 
 class NotebookAccessible(ContainerAccessible, Atk.Component, Atk.Selection):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -17046,18 +17069,18 @@
 
 class NotebookPageAccessiblePrivate(GObject.GPointer): ...
 class NotebookPrivate(GObject.GPointer): ...
 
 class NumerableIcon(Gio.EmblemedIcon, Gio.Icon):
     class Props:
         background_icon: Gio.Icon
-        background_icon_name: str
+        background_icon_name: Optional[str]
         count: int
-        label: str
-        style_context: StyleContext
+        label: Optional[str]
+        style_context: Optional[StyleContext]
         gicon: Gio.Icon
     props: Props = ...
     parent: Gio.EmblemedIcon = ...
     priv: NumerableIconPrivate = ...
     def __init__(
         self,
         background_icon: Gio.Icon = ...,
@@ -17089,48 +17112,46 @@
     padding: list[None] = ...
 
 class NumerableIconPrivate(GObject.GPointer): ...
 
 class OffscreenWindow(Window, Atk.ImplementorIface, Buildable):
     class Props:
         accept_focus: bool
-        application: Application
-        attached_to: Widget
+        application: Optional[Application]
+        attached_to: Optional[Widget]
         decorated: bool
         default_height: int
         default_width: int
         deletable: bool
         destroy_with_parent: bool
         focus_on_map: bool
         focus_visible: bool
         gravity: Gdk.Gravity
         has_resize_grip: bool
         has_toplevel_focus: bool
         hide_titlebar_when_maximized: bool
-        icon: GdkPixbuf.Pixbuf
-        icon_name: str
+        icon: Optional[GdkPixbuf.Pixbuf]
+        icon_name: Optional[str]
         is_active: bool
         is_maximized: bool
         mnemonics_visible: bool
         modal: bool
         resizable: bool
         resize_grip_visible: bool
-        role: str
+        role: Optional[str]
         screen: Gdk.Screen
         skip_pager_hint: bool
         skip_taskbar_hint: bool
-        startup_id: str
-        title: str
+        title: Optional[str]
         transient_for: Optional[Window]
         type: WindowType
         type_hint: Gdk.WindowTypeHint
         urgency_hint: bool
         window_position: WindowPosition
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -17150,27 +17171,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        startup_id: str
+        child: Widget
     props: Props = ...
     parent_object: Window = ...
     def __init__(
         self,
         accept_focus: bool = ...,
         application: Application = ...,
         attached_to: Widget = ...,
@@ -17258,15 +17281,14 @@
 
 class OrientableIface(GObject.GPointer):
     base_iface: GObject.TypeInterface = ...
 
 class Overlay(Bin, Atk.ImplementorIface, Buildable):
     class Props:
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -17286,27 +17308,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     parent: Bin = ...
     priv: OverlayPrivate = ...
     def __init__(
         self,
         border_width: int = ...,
         child: Widget = ...,
@@ -17451,15 +17474,14 @@
     class Props:
         max_position: int
         min_position: int
         position: int
         position_set: bool
         wide_handle: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -17479,28 +17501,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        child: Widget
     props: Props = ...
     container: Container = ...
     priv: PanedPrivate = ...
     def __init__(
         self,
         position: int = ...,
         position_set: bool = ...,
@@ -17566,15 +17589,15 @@
     # override
     def pack2(self, child: Widget, resize: bool, shrink: bool) -> None: ...
     def set_position(self, position: int) -> None: ...
     def set_wide_handle(self, wide: bool) -> None: ...
 
 class PanedAccessible(ContainerAccessible, Atk.Component, Atk.Value):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -17666,15 +17689,15 @@
     def set_size(self, width: float, height: float, unit: Unit) -> None: ...
     def to_gvariant(self) -> GLib.Variant: ...
     def to_key_file(self, key_file: GLib.KeyFile, group_name: str) -> None: ...
 
 class PlacesSidebar(ScrolledWindow, Atk.ImplementorIface, Buildable):
     class Props:
         local_only: bool
-        location: Gio.File
+        location: Optional[Gio.File]
         open_flags: PlacesOpenFlags
         populate_all: bool
         show_connect_to_server: bool
         show_desktop: bool
         show_enter_location: bool
         show_other_locations: bool
         show_recent: bool
@@ -17692,15 +17715,14 @@
         propagate_natural_width: bool
         shadow_type: ShadowType
         vadjustment: Adjustment
         vscrollbar_policy: PolicyType
         window_placement: CornerType
         window_placement_set: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -17720,27 +17742,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     def __init__(
         self,
         local_only: bool = ...,
         location: Gio.File = ...,
         open_flags: PlacesOpenFlags = ...,
         populate_all: bool = ...,
@@ -17837,50 +17860,48 @@
     def set_show_trash(self, show_trash: bool) -> None: ...
 
 class PlacesSidebarClass(GObject.GPointer): ...
 
 class Plug(Window, Atk.ImplementorIface, Buildable):
     class Props:
         embedded: bool
-        socket_window: Gdk.Window
+        socket_window: Optional[Gdk.Window]
         accept_focus: bool
-        application: Application
-        attached_to: Widget
+        application: Optional[Application]
+        attached_to: Optional[Widget]
         decorated: bool
         default_height: int
         default_width: int
         deletable: bool
         destroy_with_parent: bool
         focus_on_map: bool
         focus_visible: bool
         gravity: Gdk.Gravity
         has_resize_grip: bool
         has_toplevel_focus: bool
         hide_titlebar_when_maximized: bool
-        icon: GdkPixbuf.Pixbuf
-        icon_name: str
+        icon: Optional[GdkPixbuf.Pixbuf]
+        icon_name: Optional[str]
         is_active: bool
         is_maximized: bool
         mnemonics_visible: bool
         modal: bool
         resizable: bool
         resize_grip_visible: bool
-        role: str
+        role: Optional[str]
         screen: Gdk.Screen
         skip_pager_hint: bool
         skip_taskbar_hint: bool
-        startup_id: str
-        title: str
+        title: Optional[str]
         transient_for: Optional[Window]
         type: WindowType
         type_hint: Gdk.WindowTypeHint
         urgency_hint: bool
         window_position: WindowPosition
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -17900,27 +17921,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        startup_id: str
+        child: Widget
     props: Props = ...
     window: Window = ...
     priv: PlugPrivate = ...
     def __init__(
         self,
         accept_focus: bool = ...,
         application: Application = ...,
@@ -18000,15 +18023,15 @@
     @classmethod
     def new(cls, socket_id: int) -> Plug: ...
     @classmethod
     def new_for_display(cls, display: Gdk.Display, socket_id: int) -> Plug: ...
 
 class PlugAccessible(WindowAccessible, Atk.Component, Atk.Window):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -18061,15 +18084,14 @@
         constrain_to: PopoverConstraint
         modal: bool
         pointing_to: Gdk.Rectangle
         position: PositionType
         relative_to: Widget
         transitions_enabled: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -18089,27 +18111,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     parent_instance: Bin = ...
     priv: PopoverPrivate = ...
     def __init__(
         self,
         constrain_to: PopoverConstraint = ...,
         modal: bool = ...,
@@ -18184,15 +18207,15 @@
     def set_pointing_to(self, rect: Gdk.Rectangle) -> None: ...
     def set_position(self, position: PositionType) -> None: ...
     def set_relative_to(self, relative_to: Optional[Widget] = None) -> None: ...
     def set_transitions_enabled(self, transitions_enabled: bool) -> None: ...
 
 class PopoverAccessible(ContainerAccessible, Atk.Component):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -18237,15 +18260,14 @@
         constrain_to: PopoverConstraint
         modal: bool
         pointing_to: Gdk.Rectangle
         position: PositionType
         relative_to: Widget
         transitions_enabled: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -18265,27 +18287,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     def __init__(
         self,
         visible_submenu: str = ...,
         constrain_to: PopoverConstraint = ...,
         modal: bool = ...,
         pointing_to: Gdk.Rectangle = ...,
@@ -18357,15 +18380,15 @@
         self, cr: cairo.Context[_SomeSurface], dpi_x: float, dpi_y: float
     ) -> None: ...
 
 class PrintOperation(GObject.Object, PrintOperationPreview):
     class Props:
         allow_async: bool
         current_page: int
-        custom_tab_label: str
+        custom_tab_label: Optional[str]
         default_page_setup: PageSetup
         embed_page_setup: bool
         export_filename: str
         has_selection: bool
         job_name: str
         n_pages: int
         n_pages_to_print: int
@@ -18596,15 +18619,15 @@
 class ProgressBar(Widget, Atk.ImplementorIface, Buildable, Orientable):
     class Props:
         ellipsize: Pango.EllipsizeMode
         fraction: float
         inverted: bool
         pulse_step: float
         show_text: bool
-        text: str
+        text: Optional[str]
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
         expand: bool
@@ -18623,27 +18646,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
     props: Props = ...
     parent: Widget = ...
     priv: ProgressBarPrivate = ...
     def __init__(
         self,
         ellipsize: Pango.EllipsizeMode = ...,
@@ -18704,15 +18727,15 @@
     def set_inverted(self, inverted: bool) -> None: ...
     def set_pulse_step(self, fraction: float) -> None: ...
     def set_show_text(self, show_text: bool) -> None: ...
     def set_text(self, text: Optional[str] = None) -> None: ...
 
 class ProgressBarAccessible(WidgetAccessible, Atk.Component, Atk.Value):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -18757,20 +18780,20 @@
     _gtk_reserved4: None = ...
 
 class ProgressBarPrivate(GObject.GPointer): ...
 
 class PyGTKDeprecationWarning:
     args = ...  # FIXME Constant
 
-    def with_traceback(self, *args, **kwargs): ...  # FIXME Method
+    def add_note(self, *args, **kwargs): ...  # FIXME Function
+    def with_traceback(self, *args, **kwargs): ...  # FIXME Function
 
 class RadioAction(ToggleAction, Buildable):
     class Props:
         current_value: int
-        group: RadioAction
         value: int
         active: bool
         draw_as_radio: bool
         action_group: ActionGroup
         always_show_image: bool
         gicon: Gio.Icon
         hide_if_empty: bool
@@ -18782,14 +18805,15 @@
         short_label: str
         stock_id: str
         tooltip: str
         visible: bool
         visible_horizontal: bool
         visible_overflown: bool
         visible_vertical: bool
+        group: Optional[RadioAction]
     props: Props = ...
     parent: ToggleAction = ...
     private_data: RadioActionPrivate = ...
     def __init__(
         self,
         current_value: int = ...,
         group: RadioAction = ...,
@@ -18847,29 +18871,27 @@
 
 class RadioActionPrivate(GObject.GPointer): ...
 
 class RadioButton(
     CheckButton, Atk.ImplementorIface, Actionable, Activatable, Buildable
 ):
     class Props:
-        group: RadioButton
         active: bool
         draw_indicator: bool
         inconsistent: bool
         always_show_image: bool
-        image: Widget
+        image: Optional[Widget]
         image_position: PositionType
         label: str
         relief: ReliefStyle
         use_stock: bool
         use_underline: bool
         xalign: float
         yalign: float
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -18889,31 +18911,33 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
+        group: Optional[RadioButton]
+        child: Widget
     props: Props = ...
     check_button: CheckButton = ...
     priv: RadioButtonPrivate = ...
     def __init__(
         self,
         group: RadioButton = ...,
         active: bool = ...,
@@ -18999,15 +19023,15 @@
     ) -> RadioButton: ...
     def set_group(self, group: Optional[list[RadioButton]] = None) -> None: ...
 
 class RadioButtonAccessible(
     ToggleButtonAccessible, Atk.Action, Atk.Component, Atk.Image
 ):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -19054,25 +19078,23 @@
 
 class RadioButtonPrivate(GObject.GPointer): ...
 
 class RadioMenuItem(
     CheckMenuItem, Atk.ImplementorIface, Actionable, Activatable, Buildable
 ):
     class Props:
-        group: RadioMenuItem
         active: bool
         draw_as_radio: bool
         inconsistent: bool
-        accel_path: str
+        accel_path: Optional[str]
         label: str
         right_justified: bool
-        submenu: Menu
+        submenu: Optional[Menu]
         use_underline: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -19092,31 +19114,33 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
+        group: Optional[RadioMenuItem]
+        child: Widget
     props: Props = ...
     check_menu_item: CheckMenuItem = ...
     priv: RadioMenuItemPrivate = ...
     def __init__(
         self,
         group: RadioMenuItem = ...,
         active: bool = ...,
@@ -19198,15 +19222,15 @@
     ) -> RadioMenuItem: ...
     def set_group(self, group: Optional[list[RadioMenuItem]] = None) -> None: ...
 
 class RadioMenuItemAccessible(
     CheckMenuItemAccessible, Atk.Action, Atk.Component, Atk.Selection
 ):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -19253,27 +19277,25 @@
 
 class RadioMenuItemPrivate(GObject.GPointer): ...
 
 class RadioToolButton(
     ToggleToolButton, Atk.ImplementorIface, Actionable, Activatable, Buildable
 ):
     class Props:
-        group: RadioToolButton
         active: bool
-        icon_name: str
-        icon_widget: Widget
-        label: str
-        label_widget: Widget
+        icon_name: Optional[str]
+        icon_widget: Optional[Widget]
+        label: Optional[str]
+        label_widget: Optional[Widget]
         stock_id: str
         use_underline: bool
         is_important: bool
         visible_horizontal: bool
         visible_vertical: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -19293,31 +19315,33 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
+        group: Optional[RadioToolButton]
+        child: Widget
     props: Props = ...
     parent: ToggleToolButton = ...
     def __init__(
         self,
         group: RadioToolButton = ...,
         active: bool = ...,
         icon_name: str = ...,
@@ -19429,27 +19453,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
     props: Props = ...
     widget: Widget = ...
     priv: RangePrivate = ...
     def __init__(
         self,
         adjustment: Adjustment = ...,
@@ -19533,15 +19557,15 @@
     def set_show_fill_level(self, show_fill_level: bool) -> None: ...
     def set_slider_size_fixed(self, size_fixed: bool) -> None: ...
     def set_upper_stepper_sensitivity(self, sensitivity: SensitivityType) -> None: ...
     def set_value(self, value: float) -> None: ...
 
 class RangeAccessible(WidgetAccessible, Atk.Component, Atk.Value):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -19672,21 +19696,21 @@
         visible: bool
         visible_horizontal: bool
         visible_overflown: bool
         visible_vertical: bool
         filter: RecentFilter
         limit: int
         local_only: bool
-        recent_manager: RecentManager
         select_multiple: bool
         show_icons: bool
         show_not_found: bool
         show_private: bool
         show_tips: bool
         sort_type: RecentSortType
+        recent_manager: RecentManager
     props: Props = ...
     parent_instance: Action = ...
     priv: RecentActionPrivate = ...
     def __init__(
         self,
         show_numbers: bool = ...,
         action_group: ActionGroup = ...,
@@ -19778,48 +19802,46 @@
     def unselect_all(self) -> None: ...
     def unselect_uri(self, uri: str) -> None: ...
 
 class RecentChooserDialog(Dialog, Atk.ImplementorIface, Buildable, RecentChooser):
     class Props:
         use_header_bar: int
         accept_focus: bool
-        application: Application
-        attached_to: Widget
+        application: Optional[Application]
+        attached_to: Optional[Widget]
         decorated: bool
         default_height: int
         default_width: int
         deletable: bool
         destroy_with_parent: bool
         focus_on_map: bool
         focus_visible: bool
         gravity: Gdk.Gravity
         has_resize_grip: bool
         has_toplevel_focus: bool
         hide_titlebar_when_maximized: bool
-        icon: GdkPixbuf.Pixbuf
-        icon_name: str
+        icon: Optional[GdkPixbuf.Pixbuf]
+        icon_name: Optional[str]
         is_active: bool
         is_maximized: bool
         mnemonics_visible: bool
         modal: bool
         resizable: bool
         resize_grip_visible: bool
-        role: str
+        role: Optional[str]
         screen: Gdk.Screen
         skip_pager_hint: bool
         skip_taskbar_hint: bool
-        startup_id: str
-        title: str
+        title: Optional[str]
         transient_for: Optional[Window]
         type: WindowType
         type_hint: Gdk.WindowTypeHint
         urgency_hint: bool
         window_position: WindowPosition
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -19839,37 +19861,39 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         filter: RecentFilter
         limit: int
         local_only: bool
-        recent_manager: RecentManager
         select_multiple: bool
         show_icons: bool
         show_not_found: bool
         show_private: bool
         show_tips: bool
         sort_type: RecentSortType
+        startup_id: str
+        child: Widget
+        recent_manager: RecentManager
     props: Props = ...
     parent_instance: Dialog = ...
     priv: RecentChooserDialogPrivate = ...
     def __init__(
         self,
         use_header_bar: int = ...,
         accept_focus: bool = ...,
@@ -19993,15 +20017,14 @@
         rect_anchor_dx: int
         rect_anchor_dy: int
         reserve_toggle_size: bool
         tearoff_state: bool
         tearoff_title: str
         take_focus: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -20021,39 +20044,40 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         related_action: Action
         use_action_appearance: bool
         filter: RecentFilter
         limit: int
         local_only: bool
-        recent_manager: RecentManager
         select_multiple: bool
         show_icons: bool
         show_not_found: bool
         show_private: bool
         show_tips: bool
         sort_type: RecentSortType
+        child: Widget
+        recent_manager: RecentManager
     props: Props = ...
     parent_instance: Menu = ...
     priv: RecentChooserMenuPrivate = ...
     def __init__(
         self,
         show_numbers: bool = ...,
         accel_group: AccelGroup = ...,
@@ -20141,15 +20165,14 @@
     Box, Atk.ImplementorIface, Buildable, Orientable, RecentChooser
 ):
     class Props:
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -20169,38 +20192,39 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
         filter: RecentFilter
         limit: int
         local_only: bool
-        recent_manager: RecentManager
         select_multiple: bool
         show_icons: bool
         show_not_found: bool
         show_private: bool
         show_tips: bool
         sort_type: RecentSortType
+        child: Widget
+        recent_manager: RecentManager
     props: Props = ...
     parent_instance: Box = ...
     priv: RecentChooserWidgetPrivate = ...
     def __init__(
         self,
         baseline_position: BaselinePosition = ...,
         homogeneous: bool = ...,
@@ -20308,15 +20332,17 @@
 class RecentInfo(GObject.GBoxed):
     def create_app_info(
         self, app_name: Optional[str] = None
     ) -> Optional[Gio.AppInfo]: ...
     def exists(self) -> bool: ...
     def get_added(self) -> int: ...
     def get_age(self) -> int: ...
-    def get_application_info(self, *args, **kwargs): ...  # FIXME Method
+    def get_application_info(
+        self, app_name: str
+    ) -> Optional[Tuple[str, int, int]]: ...  # CHECK Wrapped function
     def get_applications(self) -> list[str]: ...
     def get_description(self) -> str: ...
     def get_display_name(self) -> str: ...
     def get_gicon(self) -> Optional[Gio.Icon]: ...
     def get_groups(self) -> list[str]: ...
     def get_icon(self, size: int) -> Optional[GdkPixbuf.Pixbuf]: ...
     def get_mime_type(self) -> str: ...
@@ -20365,15 +20391,15 @@
     _gtk_recent4: None = ...
 
 class RecentManagerPrivate(GObject.GPointer): ...
 
 class RendererCellAccessible(CellAccessible, Atk.Action, Atk.Component, Atk.TableCell):
     class Props:
         renderer: CellRenderer
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -20429,15 +20455,14 @@
 class Revealer(Bin, Atk.ImplementorIface, Buildable):
     class Props:
         child_revealed: bool
         reveal_child: bool
         transition_duration: int
         transition_type: RevealerTransitionType
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -20457,27 +20482,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     parent_instance: Bin = ...
     def __init__(
         self,
         reveal_child: bool = ...,
         transition_duration: int = ...,
         transition_type: RevealerTransitionType = ...,
@@ -20570,27 +20596,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
     props: Props = ...
     range: Range = ...
     priv: ScalePrivate = ...
     def __init__(
         self,
         digits: int = ...,
@@ -20667,15 +20693,15 @@
     def set_digits(self, digits: int) -> None: ...
     def set_draw_value(self, draw_value: bool) -> None: ...
     def set_has_origin(self, has_origin: bool) -> None: ...
     def set_value_pos(self, pos: PositionType) -> None: ...
 
 class ScaleAccessible(RangeAccessible, Atk.Component, Atk.Value):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -20717,24 +20743,23 @@
 ):
     class Props:
         adjustment: Adjustment
         icons: list[str]
         size: IconSize
         value: float
         always_show_image: bool
-        image: Widget
+        image: Optional[Widget]
         image_position: PositionType
         label: str
         relief: ReliefStyle
         use_stock: bool
         use_underline: bool
         xalign: float
         yalign: float
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -20754,32 +20779,33 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
         orientation: Orientation
+        child: Widget
     props: Props = ...
     parent: Button = ...
     priv: ScaleButtonPrivate = ...
     def __init__(
         self,
         adjustment: Adjustment = ...,
         icons: Sequence[str] = ...,
@@ -20858,15 +20884,15 @@
     def set_icons(self, icons: Sequence[str]) -> None: ...
     def set_value(self, value: float) -> None: ...
 
 class ScaleButtonAccessible(
     ButtonAccessible, Atk.Action, Atk.Component, Atk.Image, Atk.Value
 ):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -20972,27 +20998,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
     props: Props = ...
     range: Range = ...
     def __init__(
         self,
         adjustment: Adjustment = ...,
         fill_level: float = ...,
@@ -21066,15 +21092,14 @@
         propagate_natural_width: bool
         shadow_type: ShadowType
         vadjustment: Adjustment
         vscrollbar_policy: PolicyType
         window_placement: CornerType
         window_placement_set: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -21094,27 +21119,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     container: Bin = ...
     priv: ScrolledWindowPrivate = ...
     def __init__(
         self,
         hadjustment: Adjustment = ...,
         hscrollbar_policy: PolicyType = ...,
@@ -21212,15 +21238,15 @@
     def set_propagate_natural_width(self, propagate: bool) -> None: ...
     def set_shadow_type(self, type: ShadowType) -> None: ...
     def set_vadjustment(self, vadjustment: Optional[Adjustment] = None) -> None: ...
     def unset_placement(self) -> None: ...
 
 class ScrolledWindowAccessible(ContainerAccessible, Atk.Component):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -21270,15 +21296,14 @@
 class ScrolledWindowPrivate(GObject.GPointer): ...
 
 class SearchBar(Bin, Atk.ImplementorIface, Buildable):
     class Props:
         search_mode_enabled: bool
         show_close_button: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -21298,27 +21323,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     parent: Bin = ...
     def __init__(
         self,
         search_mode_enabled: bool = ...,
         show_close_button: bool = ...,
         border_width: int = ...,
@@ -21376,24 +21402,24 @@
     _gtk_reserved2: None = ...
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
 
 class SearchEntry(Entry, Atk.ImplementorIface, Buildable, CellEditable, Editable):
     class Props:
         activates_default: bool
-        attributes: Pango.AttrList
+        attributes: Optional[Pango.AttrList]
         buffer: EntryBuffer
         caps_lock_warning: bool
         completion: EntryCompletion
         cursor_position: int
         editable: bool
         enable_emoji_completion: bool
         has_frame: bool
         im_module: str
-        inner_border: Border
+        inner_border: Optional[Border]
         input_hints: InputHints
         input_purpose: InputPurpose
         invisible_char: int
         invisible_char_set: bool
         max_length: int
         max_width_chars: int
         overwrite_mode: bool
@@ -21419,15 +21445,15 @@
         secondary_icon_stock: str
         secondary_icon_storage_type: ImageType
         secondary_icon_tooltip_markup: str
         secondary_icon_tooltip_text: str
         selection_bound: int
         shadow_type: ShadowType
         show_emoji_icon: bool
-        tabs: Pango.TabArray
+        tabs: Optional[Pango.TabArray]
         text: str
         text_length: int
         truncate_multiline: bool
         visibility: bool
         width_chars: int
         xalign: float
         app_paintable: bool
@@ -21452,27 +21478,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         editing_canceled: bool
     props: Props = ...
     parent: Entry = ...
     def __init__(
         self,
         activates_default: bool = ...,
         attributes: Pango.AttrList = ...,
@@ -21619,27 +21645,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
     props: Props = ...
     widget: Widget = ...
     priv: SeparatorPrivate = ...
     def __init__(
         self,
         app_paintable: bool = ...,
@@ -21690,21 +21716,20 @@
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
 
 class SeparatorMenuItem(
     MenuItem, Atk.ImplementorIface, Actionable, Activatable, Buildable
 ):
     class Props:
-        accel_path: str
+        accel_path: Optional[str]
         label: str
         right_justified: bool
-        submenu: Menu
+        submenu: Optional[Menu]
         use_underline: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -21724,31 +21749,32 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
+        child: Widget
     props: Props = ...
     menu_item: MenuItem = ...
     def __init__(
         self,
         accel_path: str = ...,
         label: str = ...,
         right_justified: bool = ...,
@@ -21813,15 +21839,14 @@
 class SeparatorToolItem(ToolItem, Atk.ImplementorIface, Activatable, Buildable):
     class Props:
         draw: bool
         is_important: bool
         visible_horizontal: bool
         visible_vertical: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -21841,29 +21866,30 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         related_action: Action
         use_action_appearance: bool
+        child: Widget
     props: Props = ...
     parent: ToolItem = ...
     priv: SeparatorToolItemPrivate = ...
     def __init__(
         self,
         draw: bool = ...,
         is_important: bool = ...,
@@ -22130,21 +22156,20 @@
 
 class SettingsValue(GObject.GPointer):
     origin: str = ...
     value: Any = ...
 
 class ShortcutLabel(Box, Atk.ImplementorIface, Buildable, Orientable):
     class Props:
-        accelerator: str
-        disabled_text: str
+        accelerator: Optional[str]
+        disabled_text: Optional[str]
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -22164,28 +22189,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        child: Widget
     props: Props = ...
     def __init__(
         self,
         accelerator: str = ...,
         disabled_text: str = ...,
         baseline_position: BaselinePosition = ...,
         homogeneous: bool = ...,
@@ -22238,24 +22264,21 @@
     def set_accelerator(self, accelerator: str) -> None: ...
     def set_disabled_text(self, disabled_text: str) -> None: ...
 
 class ShortcutLabelClass(GObject.GPointer): ...
 
 class ShortcutsGroup(Box, Atk.ImplementorIface, Buildable, Orientable):
     class Props:
-        accel_size_group: SizeGroup
         height: int
         title: str
-        title_size_group: SizeGroup
         view: str
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -22275,28 +22298,31 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        accel_size_group: SizeGroup
+        title_size_group: SizeGroup
+        child: Widget
     props: Props = ...
     def __init__(
         self,
         accel_size_group: SizeGroup = ...,
         title: str = ...,
         title_size_group: SizeGroup = ...,
         view: str = ...,
@@ -22353,15 +22379,14 @@
         section_name: str
         title: str
         view_name: str
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -22381,28 +22406,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        child: Widget
     props: Props = ...
     def __init__(
         self,
         max_height: int = ...,
         section_name: str = ...,
         title: str = ...,
         view_name: str = ...,
@@ -22451,30 +22477,27 @@
         orientation: Orientation = ...,
     ): ...
 
 class ShortcutsSectionClass(GObject.GPointer): ...
 
 class ShortcutsShortcut(Box, Atk.ImplementorIface, Buildable, Orientable):
     class Props:
-        accel_size_group: SizeGroup
         accelerator: str
         action_name: str
         direction: TextDirection
         icon: Gio.Icon
         icon_set: bool
         shortcut_type: ShortcutType
         subtitle: str
         subtitle_set: bool
         title: str
-        title_size_group: SizeGroup
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -22494,28 +22517,31 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        accel_size_group: SizeGroup
+        title_size_group: SizeGroup
+        child: Widget
     props: Props = ...
     def __init__(
         self,
         accel_size_group: SizeGroup = ...,
         accelerator: str = ...,
         action_name: str = ...,
         direction: TextDirection = ...,
@@ -22574,48 +22600,46 @@
 class ShortcutsShortcutClass(GObject.GPointer): ...
 
 class ShortcutsWindow(Window, Atk.ImplementorIface, Buildable):
     class Props:
         section_name: str
         view_name: str
         accept_focus: bool
-        application: Application
-        attached_to: Widget
+        application: Optional[Application]
+        attached_to: Optional[Widget]
         decorated: bool
         default_height: int
         default_width: int
         deletable: bool
         destroy_with_parent: bool
         focus_on_map: bool
         focus_visible: bool
         gravity: Gdk.Gravity
         has_resize_grip: bool
         has_toplevel_focus: bool
         hide_titlebar_when_maximized: bool
-        icon: GdkPixbuf.Pixbuf
-        icon_name: str
+        icon: Optional[GdkPixbuf.Pixbuf]
+        icon_name: Optional[str]
         is_active: bool
         is_maximized: bool
         mnemonics_visible: bool
         modal: bool
         resizable: bool
         resize_grip_visible: bool
-        role: str
+        role: Optional[str]
         screen: Gdk.Screen
         skip_pager_hint: bool
         skip_taskbar_hint: bool
-        startup_id: str
-        title: str
+        title: Optional[str]
         transient_for: Optional[Window]
         type: WindowType
         type_hint: Gdk.WindowTypeHint
         urgency_hint: bool
         window_position: WindowPosition
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -22635,27 +22659,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        startup_id: str
+        child: Widget
     props: Props = ...
     window: Window = ...
     def __init__(
         self,
         section_name: str = ...,
         view_name: str = ...,
         accept_focus: bool = ...,
@@ -22761,15 +22787,14 @@
     _gtk_reserved4: None = ...
 
 class SizeGroupPrivate(GObject.GPointer): ...
 
 class Socket(Container, Atk.ImplementorIface, Buildable):
     class Props:
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -22789,27 +22814,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     container: Container = ...
     priv: SocketPrivate = ...
     def __init__(
         self,
         border_width: int = ...,
         child: Widget = ...,
@@ -22857,15 +22883,15 @@
     def get_id(self) -> int: ...
     def get_plug_window(self) -> Optional[Gdk.Window]: ...
     @classmethod
     def new(cls) -> Socket: ...
 
 class SocketAccessible(ContainerAccessible, Atk.Component):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -22923,24 +22949,24 @@
         digits: int
         numeric: bool
         snap_to_ticks: bool
         update_policy: SpinButtonUpdatePolicy
         value: float
         wrap: bool
         activates_default: bool
-        attributes: Pango.AttrList
+        attributes: Optional[Pango.AttrList]
         buffer: EntryBuffer
         caps_lock_warning: bool
         completion: EntryCompletion
         cursor_position: int
         editable: bool
         enable_emoji_completion: bool
         has_frame: bool
         im_module: str
-        inner_border: Border
+        inner_border: Optional[Border]
         input_hints: InputHints
         input_purpose: InputPurpose
         invisible_char: int
         invisible_char_set: bool
         max_length: int
         max_width_chars: int
         overwrite_mode: bool
@@ -22966,15 +22992,15 @@
         secondary_icon_stock: str
         secondary_icon_storage_type: ImageType
         secondary_icon_tooltip_markup: str
         secondary_icon_tooltip_text: str
         selection_bound: int
         shadow_type: ShadowType
         show_emoji_icon: bool
-        tabs: Pango.TabArray
+        tabs: Optional[Pango.TabArray]
         text: str
         text_length: int
         truncate_multiline: bool
         visibility: bool
         width_chars: int
         xalign: float
         app_paintable: bool
@@ -22999,27 +23025,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         editing_canceled: bool
         orientation: Orientation
     props: Props = ...
     entry: Entry = ...
     priv: SpinButtonPrivate = ...
     def __init__(
         self,
@@ -23151,15 +23177,15 @@
     def spin(self, direction: SpinType, increment: float) -> None: ...
     def update(self) -> None: ...
 
 class SpinButtonAccessible(
     EntryAccessible, Atk.Action, Atk.Component, Atk.EditableText, Atk.Text, Atk.Value
 ):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -23235,27 +23261,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
     props: Props = ...
     parent: Widget = ...
     priv: SpinnerPrivate = ...
     def __init__(
         self,
         active: bool = ...,
         app_paintable: bool = ...,
@@ -23298,15 +23324,15 @@
     @classmethod
     def new(cls) -> Spinner: ...
     def start(self) -> None: ...
     def stop(self) -> None: ...
 
 class SpinnerAccessible(WidgetAccessible, Atk.Component, Atk.Image):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -23357,18 +23383,17 @@
         hhomogeneous: bool
         homogeneous: bool
         interpolate_size: bool
         transition_duration: int
         transition_running: bool
         transition_type: StackTransitionType
         vhomogeneous: bool
-        visible_child: Widget
-        visible_child_name: str
+        visible_child: Optional[Widget]
+        visible_child_name: Optional[str]
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -23388,27 +23413,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     parent_instance: Container = ...
     def __init__(
         self,
         hhomogeneous: bool = ...,
         homogeneous: bool = ...,
         interpolate_size: bool = ...,
@@ -23521,15 +23547,15 @@
     def set_visible_child_full(
         self, name: str, transition: StackTransitionType
     ) -> None: ...
     def set_visible_child_name(self, name: str) -> None: ...
 
 class StackAccessible(ContainerAccessible, Atk.Component):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -23564,17 +23590,16 @@
     parent_class: ContainerAccessibleClass = ...
 
 class StackClass(GObject.GPointer):
     parent_class: ContainerClass = ...
 
 class StackSidebar(Bin, Atk.ImplementorIface, Buildable):
     class Props:
-        stack: Stack
+        stack: Optional[Stack]
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -23594,27 +23619,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     parent: Bin = ...
     def __init__(
         self,
         stack: Stack = ...,
         border_width: int = ...,
         child: Widget = ...,
@@ -23669,20 +23695,19 @@
     _gtk_reserved4: None = ...
 
 class StackSidebarPrivate(GObject.GPointer): ...
 
 class StackSwitcher(Box, Atk.ImplementorIface, Buildable, Orientable):
     class Props:
         icon_size: int
-        stack: Stack
+        stack: Optional[Stack]
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -23702,28 +23727,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        child: Widget
     props: Props = ...
     widget: Box = ...
     def __init__(
         self,
         icon_size: int = ...,
         stack: Stack = ...,
         baseline_position: BaselinePosition = ...,
@@ -23781,28 +23807,28 @@
     _gtk_reserved2: None = ...
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
 
 class StatusIcon(GObject.Object):
     class Props:
         embedded: bool
-        file: str
-        gicon: Gio.Icon
+        gicon: Optional[Gio.Icon]
         has_tooltip: bool
-        icon_name: str
+        icon_name: Optional[str]
         orientation: Orientation
-        pixbuf: GdkPixbuf.Pixbuf
+        pixbuf: Optional[GdkPixbuf.Pixbuf]
         screen: Gdk.Screen
         size: int
-        stock: str
+        stock: Optional[str]
         storage_type: ImageType
         title: str
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         visible: bool
+        file: str
     props: Props = ...
     parent_instance: GObject.Object = ...
     priv: StatusIconPrivate = ...
     def __init__(
         self,
         file: str = ...,
         gicon: Gio.Icon = ...,
@@ -23885,15 +23911,14 @@
 
 class Statusbar(Box, Atk.ImplementorIface, Buildable, Orientable):
     class Props:
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -23913,28 +23938,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        child: Widget
     props: Props = ...
     parent_widget: Box = ...
     priv: StatusbarPrivate = ...
     def __init__(
         self,
         baseline_position: BaselinePosition = ...,
         homogeneous: bool = ...,
@@ -23989,15 +24015,15 @@
     def pop(self, context_id: int) -> None: ...
     def push(self, context_id: int, text: str) -> int: ...
     def remove(self, context_id: int, message_id: int) -> None: ...
     def remove_all(self, context_id: int) -> None: ...
 
 class StatusbarAccessible(ContainerAccessible, Atk.Component):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -24684,15 +24710,15 @@
     _gtk_reserved10: None = ...
     _gtk_reserved11: None = ...
 
 class StyleContext(GObject.Object):
     class Props:
         direction: TextDirection
         paint_clock: Gdk.FrameClock
-        parent: StyleContext
+        parent: Optional[StyleContext]
         screen: Gdk.Screen
     props: Props = ...
     parent_object: GObject.Object = ...
     priv: StyleContextPrivate = ...
     def __init__(
         self,
         direction: TextDirection = ...,
@@ -24838,28 +24864,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
     props: Props = ...
     parent_instance: Widget = ...
     priv: SwitchPrivate = ...
     def __init__(
@@ -24914,15 +24940,15 @@
     @classmethod
     def new(cls) -> Switch: ...
     def set_active(self, is_active: bool) -> None: ...
     def set_state(self, state: bool) -> None: ...
 
 class SwitchAccessible(WidgetAccessible, Atk.Action, Atk.Component):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -24997,15 +25023,14 @@
     class Props:
         column_spacing: int
         homogeneous: bool
         n_columns: int
         n_rows: int
         row_spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -25025,27 +25050,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     container: Container = ...
     priv: TablePrivate = ...
     def __init__(
         self,
         column_spacing: int = ...,
         homogeneous: bool = ...,
@@ -25088,14 +25114,15 @@
         tooltip_text: str = ...,
         valign: Align = ...,
         vexpand: bool = ...,
         vexpand_set: bool = ...,
         visible: bool = ...,
         width_request: int = ...,
     ): ...
+    # override
     def attach(self, *args, **kwargs): ...  # FIXME Method
     def attach_defaults(
         self,
         widget: Widget,
         left_attach: int,
         right_attach: int,
         top_attach: int,
@@ -25180,21 +25207,20 @@
     flags: int = ...
     info: int = ...
 
 class TearoffMenuItem(
     MenuItem, Atk.ImplementorIface, Actionable, Activatable, Buildable
 ):
     class Props:
-        accel_path: str
+        accel_path: Optional[str]
         label: str
         right_justified: bool
-        submenu: Menu
+        submenu: Optional[Menu]
         use_underline: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -25214,31 +25240,32 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
+        child: Widget
     props: Props = ...
     menu_item: MenuItem = ...
     priv: TearoffMenuItemPrivate = ...
     def __init__(
         self,
         accel_path: str = ...,
         label: str = ...,
@@ -25298,17 +25325,17 @@
     _gtk_reserved2: None = ...
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
 
 class TearoffMenuItemPrivate(GObject.GPointer): ...
 
 class Template:
-    def from_file(self, *args, **kwargs): ...  # FIXME Method
-    def from_resource(self, *args, **kwargs): ...  # FIXME Method
-    def from_string(self, *args, **kwargs): ...  # FIXME Method
+    def from_file(filename): ...  # FIXME Function
+    def from_resource(resource_path): ...  # FIXME Function
+    def from_string(string): ...  # FIXME Function
 
     class Callback: ...
     class Child: ...
 
 class TextAppearance(GObject.GPointer):
     bg_color: Gdk.Color = ...
     fg_color: Gdk.Color = ...
@@ -25460,15 +25487,15 @@
     ) -> bool: ...
     def insert_markup(self, iter: TextIter, markup: str, len: int) -> None: ...
     def insert_pixbuf(self, iter: TextIter, pixbuf: GdkPixbuf.Pixbuf) -> None: ...
     def insert_range(self, iter: TextIter, start: TextIter, end: TextIter) -> None: ...
     def insert_range_interactive(
         self, iter: TextIter, start: TextIter, end: TextIter, default_editable: bool
     ) -> bool: ...
-    def insert_with_tags(self, *args, **kwargs): ...  # FIXME Method
+    def insert_with_tags(self, iter, text, *tags): ...  # FIXME Function
     # override
     def insert_with_tags_by_name(
         self, iter: TextIter, text: str, *tags: Any
     ) -> None: ...
     def move_mark(self, mark: TextMark, where: TextIter) -> None: ...
     def move_mark_by_name(self, name: str, where: TextIter) -> None: ...
     @classmethod
@@ -25483,15 +25510,15 @@
     def register_deserialize_format(
         self, mime_type: str, function: Callable[..., bool], *user_data: Any
     ) -> Gdk.Atom: ...
     def register_deserialize_tagset(
         self, tagset_name: Optional[str] = None
     ) -> Gdk.Atom: ...
     def register_serialize_format(
-        self, mime_type: str, function: Callable[..., Optional[int]], *user_data: Any
+        self, mime_type: str, function: Callable[..., Optional[bytes]], *user_data: Any
     ) -> Gdk.Atom: ...
     def register_serialize_tagset(
         self, tagset_name: Optional[str] = None
     ) -> Gdk.Atom: ...
     def remove_all_tags(self, start: TextIter, end: TextIter) -> None: ...
     def remove_selection_clipboard(self, clipboard: Clipboard) -> None: ...
     def remove_tag(self, tag: TextTag, start: TextIter, end: TextIter) -> None: ...
@@ -25533,15 +25560,15 @@
 class TextBufferPrivate(GObject.GPointer): ...
 
 class TextCellAccessible(
     RendererCellAccessible, Atk.Action, Atk.Component, Atk.TableCell, Atk.Text
 ):
     class Props:
         renderer: CellRenderer
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -25717,15 +25744,15 @@
     def starts_tag(self, tag: Optional[TextTag] = None) -> bool: ...
     def starts_word(self) -> bool: ...
     def toggles_tag(self, tag: Optional[TextTag] = None) -> bool: ...
 
 class TextMark(GObject.Object):
     class Props:
         left_gravity: bool
-        name: str
+        name: Optional[str]
     props: Props = ...
     parent_instance: GObject.Object = ...
     segment: None = ...
     def __init__(self, left_gravity: bool = ..., name: str = ...): ...
     def get_buffer(self) -> TextBuffer: ...
     def get_deleted(self) -> bool: ...
     def get_left_gravity(self) -> bool: ...
@@ -25741,15 +25768,14 @@
     _gtk_reserved2: None = ...
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
 
 class TextTag(GObject.Object):
     class Props:
         accumulative_margin: bool
-        background: str
         background_full_height: bool
         background_full_height_set: bool
         background_gdk: Gdk.Color
         background_rgba: Gdk.RGBA
         background_set: bool
         direction: TextDirection
         editable: bool
@@ -25758,15 +25784,14 @@
         fallback_set: bool
         family: str
         family_set: bool
         font: str
         font_desc: Pango.FontDescription
         font_features: str
         font_features_set: bool
-        foreground: str
         foreground_gdk: Gdk.Color
         foreground_rgba: Gdk.RGBA
         foreground_set: bool
         indent: int
         indent_set: bool
         invisible: bool
         invisible_set: bool
@@ -25775,15 +25800,14 @@
         language: str
         language_set: bool
         left_margin: int
         left_margin_set: bool
         letter_spacing: int
         letter_spacing_set: bool
         name: str
-        paragraph_background: str
         paragraph_background_gdk: Gdk.Color
         paragraph_background_rgba: Gdk.RGBA
         paragraph_background_set: bool
         pixels_above_lines: int
         pixels_above_lines_set: bool
         pixels_below_lines: int
         pixels_below_lines_set: bool
@@ -25814,14 +25838,17 @@
         underline_set: bool
         variant: Pango.Variant
         variant_set: bool
         weight: int
         weight_set: bool
         wrap_mode: WrapMode
         wrap_mode_set: bool
+        background: str
+        foreground: str
+        paragraph_background: str
     props: Props = ...
     parent_instance: GObject.Object = ...
     priv: TextTagPrivate = ...
     def __init__(
         self,
         accumulative_margin: bool = ...,
         background: str = ...,
@@ -25962,19 +25989,18 @@
         monospace: bool
         overwrite: bool
         pixels_above_lines: int
         pixels_below_lines: int
         pixels_inside_wrap: int
         populate_all: bool
         right_margin: int
-        tabs: Pango.TabArray
+        tabs: Optional[Pango.TabArray]
         top_margin: int
         wrap_mode: WrapMode
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -25994,31 +26020,32 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         hadjustment: Adjustment
         hscroll_policy: ScrollablePolicy
         vadjustment: Adjustment
         vscroll_policy: ScrollablePolicy
+        child: Widget
     props: Props = ...
     parent_instance: Container = ...
     priv: TextViewPrivate = ...
     def __init__(
         self,
         accepts_tab: bool = ...,
         bottom_margin: int = ...,
@@ -26210,15 +26237,15 @@
     ContainerAccessible,
     Atk.Component,
     Atk.EditableText,
     Atk.StreamableContent,
     Atk.Text,
 ):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -26602,24 +26629,23 @@
 
 class ToggleButton(Button, Atk.ImplementorIface, Actionable, Activatable, Buildable):
     class Props:
         active: bool
         draw_indicator: bool
         inconsistent: bool
         always_show_image: bool
-        image: Widget
+        image: Optional[Widget]
         image_position: PositionType
         label: str
         relief: ReliefStyle
         use_stock: bool
         use_underline: bool
         xalign: float
         yalign: float
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -26639,31 +26665,32 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
+        child: Widget
     props: Props = ...
     button: Button = ...
     priv: ToggleButtonPrivate = ...
     def __init__(
         self,
         active: bool = ...,
         draw_indicator: bool = ...,
@@ -26734,15 +26761,15 @@
     def set_active(self, is_active: bool) -> None: ...
     def set_inconsistent(self, setting: bool) -> None: ...
     def set_mode(self, draw_indicator: bool) -> None: ...
     def toggled(self) -> None: ...
 
 class ToggleButtonAccessible(ButtonAccessible, Atk.Action, Atk.Component, Atk.Image):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -26790,25 +26817,24 @@
 class ToggleButtonPrivate(GObject.GPointer): ...
 
 class ToggleToolButton(
     ToolButton, Atk.ImplementorIface, Actionable, Activatable, Buildable
 ):
     class Props:
         active: bool
-        icon_name: str
-        icon_widget: Widget
-        label: str
-        label_widget: Widget
+        icon_name: Optional[str]
+        icon_widget: Optional[Widget]
+        label: Optional[str]
+        label_widget: Optional[Widget]
         stock_id: str
         use_underline: bool
         is_important: bool
         visible_horizontal: bool
         visible_vertical: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -26828,31 +26854,32 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
+        child: Widget
     props: Props = ...
     parent: ToolButton = ...
     priv: ToggleToolButtonPrivate = ...
     def __init__(
         self,
         active: bool = ...,
         icon_name: str = ...,
@@ -26924,25 +26951,24 @@
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
 
 class ToggleToolButtonPrivate(GObject.GPointer): ...
 
 class ToolButton(ToolItem, Atk.ImplementorIface, Actionable, Activatable, Buildable):
     class Props:
-        icon_name: str
-        icon_widget: Widget
-        label: str
-        label_widget: Widget
+        icon_name: Optional[str]
+        icon_widget: Optional[Widget]
+        label: Optional[str]
+        label_widget: Optional[Widget]
         stock_id: str
         use_underline: bool
         is_important: bool
         visible_horizontal: bool
         visible_vertical: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -26962,31 +26988,32 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
+        child: Widget
     props: Props = ...
     parent: ToolItem = ...
     priv: ToolButtonPrivate = ...
     def __init__(
         self,
         icon_name: str = ...,
         icon_widget: Widget = ...,
@@ -27074,15 +27101,14 @@
 
 class ToolItem(Bin, Atk.ImplementorIface, Activatable, Buildable):
     class Props:
         is_important: bool
         visible_horizontal: bool
         visible_vertical: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -27102,29 +27128,30 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         related_action: Action
         use_action_appearance: bool
+        child: Widget
     props: Props = ...
     parent: Bin = ...
     priv: ToolItemPrivate = ...
     def __init__(
         self,
         is_important: bool = ...,
         visible_horizontal: bool = ...,
@@ -27218,15 +27245,14 @@
     class Props:
         collapsed: bool
         ellipsize: Pango.EllipsizeMode
         header_relief: ReliefStyle
         label: str
         label_widget: Widget
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -27246,27 +27272,28 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        child: Widget
     props: Props = ...
     parent_instance: Container = ...
     priv: ToolItemGroupPrivate = ...
     def __init__(
         self,
         collapsed: bool = ...,
         ellipsize: Pango.EllipsizeMode = ...,
@@ -27344,15 +27371,14 @@
 
 class ToolPalette(Container, Atk.ImplementorIface, Buildable, Orientable, Scrollable):
     class Props:
         icon_size: IconSize
         icon_size_set: bool
         toolbar_style: ToolbarStyle
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -27372,32 +27398,33 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
         hadjustment: Adjustment
         hscroll_policy: ScrollablePolicy
         vadjustment: Adjustment
         vscroll_policy: ScrollablePolicy
+        child: Widget
     props: Props = ...
     parent_instance: Container = ...
     priv: ToolPalettePrivate = ...
     def __init__(
         self,
         icon_size: IconSize = ...,
         icon_size_set: bool = ...,
@@ -27514,15 +27541,14 @@
 class Toolbar(Container, Atk.ImplementorIface, Buildable, Orientable, ToolShell):
     class Props:
         icon_size: IconSize
         icon_size_set: bool
         show_arrow: bool
         toolbar_style: ToolbarStyle
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -27542,28 +27568,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        child: Widget
     props: Props = ...
     container: Container = ...
     priv: ToolbarPrivate = ...
     def __init__(
         self,
         icon_size: IconSize = ...,
         icon_size_set: bool = ...,
@@ -27729,15 +27756,14 @@
     user_data2: None = ...
     user_data3: None = ...
     def copy(self) -> TreeIter: ...
     def free(self) -> None: ...
 
 # override
 class TreeModel(GObject.GInterface):
-    # override
     def filter_new(self, root: Optional[TreePath] = None) -> TreeModelFilter: ...
     def foreach(self, func: Callable[..., bool], *user_data: Any) -> None: ...
     def get(self, treeiter: TreeIter, *columns: list[str]) -> tuple[Any, ...]: ...
     def get_column_type(self, index_: int) -> Type: ...
     def get_flags(self) -> TreeModelFlags: ...
     def get_iter(self, path: Union[str, TreePath]) -> TreeIter: ...
     def get_iter_first(self) -> Optional[TreeIter]: ...
@@ -27762,19 +27788,17 @@
     def row_inserted(self, path: TreePath, iter: TreeIter) -> None: ...
     def rows_reordered(
         self, path: TreePath, iter: Optional[TreeIter], new_order: list[int]
     ) -> None: ...
     def set_row(self, treeiter: TreeIter, row: list[Any]): ...
     def sort_new_with_model(self) -> TreeModelSort: ...
     def unref_node(self, iter: TreeIter) -> None: ...
-    # override
     def __getitem__(
         self, item: Union[TreeIter, TreePath, str, int]
     ) -> TreeModelRow: ...
-    # override
     def __delitem__(self, item: Union[TreeIter, TreePath, str, int]) -> None: ...
 
 class TreeModelFilter(GObject.Object, TreeDragSource, TreeModel):
     class Props:
         child_model: TreeModel
         virtual_root: TreePath
     props: Props = ...
@@ -27801,15 +27825,15 @@
     def set_modify_func(
         self,
         n_columns: int,
         types: Sequence[Type],
         func: Callable[..., Any],
         *data: Any,
     ) -> None: ...
-    def set_value(self, *args, **kwargs): ...  # FIXME Method
+    def set_value(self, iter, column, value): ...  # FIXME Function
     def set_visible_column(self, column: int) -> None: ...
     # override
     def set_visible_func(
         self,
         func: Callable[[TreeModelFilter, TreeIter, Any], bool],
         data: Optional[Any] = ...,
     ) -> None: ...
@@ -27848,36 +27872,32 @@
     iter_nth_child: Callable[
         [TreeModel, Optional[TreeIter], int], Tuple[bool, TreeIter]
     ] = ...
     iter_parent: Callable[[TreeModel, TreeIter], Tuple[bool, TreeIter]] = ...
     ref_node: Callable[[TreeModel, TreeIter], None] = ...
     unref_node: Callable[[TreeModel, TreeIter], None] = ...
 
+# override
 class TreeModelRow:
-    # override
     iter: TreeIter
-    # override
     model: TreeModel
     next = ...  # FIXME Constant
     parent = ...  # FIXME Constant
     path = ...  # FIXME Constant
     previous = ...  # FIXME Constant
 
-    def get_next(self, *args, **kwargs): ...  # FIXME Method
-    def get_parent(self, *args, **kwargs): ...  # FIXME Method
-    def get_previous(self, *args, **kwargs): ...  # FIXME Method
-    # override
+    def get_next(self): ...  # FIXME Function
+    def get_parent(self): ...  # FIXME Function
+    def get_previous(self): ...  # FIXME Function
     def iterchildren(self) -> Iterator[TreeModelRow]: ...
-    # override
     def __getitem__(self, key: int) -> Any: ...
-    # override
     def __setitem__(self, key: int, value: Any) -> None: ...
 
 class TreeModelRowIter:
-    def next(self, *args, **kwargs): ...  # FIXME Method
+    def next(self): ...  # FIXME Function
 
 class TreeModelSort(GObject.Object, TreeDragSource, TreeModel, TreeSortable):
     class Props:
         model: TreeModel
     props: Props = ...
     parent: GObject.Object = ...
     priv: TreeModelSortPrivate = ...
@@ -27990,17 +28010,19 @@
     _gtk_reserved2: None = ...
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
 
 class TreeSelectionPrivate(GObject.GPointer): ...
 
 class TreeSortable(GObject.GInterface):
-    def get_sort_column_id(self, *args, **kwargs): ...  # FIXME Method
+    def get_sort_column_id(
+        self,
+    ) -> Tuple[int, SortType] | Tuple[None, None]: ...  # CHECK Wrapped function
     def has_default_sort_func(self) -> bool: ...
-    def set_default_sort_func(self, *args, **kwargs): ...  # FIXME Method
+    def set_default_sort_func(self, sort_func, user_data=None): ...  # FIXME Function
     def set_sort_column_id(self, sort_column_id: int, order: SortType) -> None: ...
     # override
     def set_sort_func(
         self,
         sort_column_id: int,
         sort_func: Callable[[TreeModel, TreeIter, TreeIter, Any], Any],
         user_data: Optional[Any] = None,
@@ -28022,17 +28044,17 @@
     parent: GObject.Object = ...
     priv: TreeStorePrivate = ...
     # override
     def append(
         self, parent: Optional[TreeIter], row: Optional[list[Any]] = None
     ) -> TreeIter: ...
     def clear(self) -> None: ...
-    def insert(self, *args, **kwargs): ...  # FIXME Method
-    def insert_after(self, *args, **kwargs): ...  # FIXME Method
-    def insert_before(self, *args, **kwargs): ...  # FIXME Method
+    def insert(self, parent, position, row=None): ...  # FIXME Function
+    def insert_after(self, parent, sibling, row=None): ...  # FIXME Function
+    def insert_before(self, parent, sibling, row=None): ...  # FIXME Function
     def insert_with_values(
         self,
         parent: Optional[TreeIter],
         position: int,
         columns: Sequence[int],
         values: Sequence[Any],
     ) -> TreeIter: ...
@@ -28043,19 +28065,19 @@
         self, iter: TreeIter, position: Optional[TreeIter] = None
     ) -> None: ...
     def move_before(
         self, iter: TreeIter, position: Optional[TreeIter] = None
     ) -> None: ...
     @classmethod
     def new(cls, n_columns: int, types: Sequence[Type]) -> TreeStore: ...
-    def prepend(self, *args, **kwargs): ...  # FIXME Method
+    def prepend(self, parent, row=None): ...  # FIXME Function
     def remove(self, iter: TreeIter) -> bool: ...
-    def set(self, *args, **kwargs): ...  # FIXME Method
+    def set(self, treeiter, *args): ...  # FIXME Function
     def set_column_types(self, n_columns: int, types: Sequence[Type]) -> None: ...
-    def set_value(self, *args, **kwargs): ...  # FIXME Method
+    def set_value(self, treeiter, column, value): ...  # FIXME Function
     def swap(self, a: TreeIter, b: TreeIter) -> None: ...
 
 class TreeStoreClass(GObject.GPointer):
     parent_class: GObject.ObjectClass = ...
     _gtk_reserved1: None = ...
     _gtk_reserved2: None = ...
     _gtk_reserved3: None = ...
@@ -28130,14 +28152,15 @@
         hadjustment: Adjustment
         hscroll_policy: ScrollablePolicy
         vadjustment: Adjustment
         vscroll_policy: ScrollablePolicy
     props: Props = ...
     parent: Container = ...
     priv: TreeViewPrivate = ...
+
     def __init__(
         self,
         activate_on_single_click: bool = ...,
         enable_grid_lines: TreeViewGridLines = ...,
         enable_search: bool = ...,
         enable_tree_lines: bool = ...,
         expander_column: TreeViewColumn = ...,
@@ -28248,15 +28271,15 @@
     def expand_row(self, path: TreePath, open_all: bool) -> bool: ...
     def expand_to_path(self, path: TreePath) -> None: ...
     def get_activate_on_single_click(self) -> bool: ...
     def get_background_area(
         self, path: Optional[TreePath] = None, column: Optional[TreeViewColumn] = None
     ) -> Gdk.Rectangle: ...
     def get_bin_window(self) -> Optional[Gdk.Window]: ...
-    def get_cell_area(self, *args, **kwargs): ...  # FIXME Method
+    def get_cell_area(self, *args, **kwargs): ...
     def get_column(self, n: int) -> Optional[TreeViewColumn]: ...
     def get_columns(self) -> list[TreeViewColumn]: ...
     def get_cursor(self) -> Tuple[TreePath, TreeViewColumn]: ...
     def get_dest_row_at_pos(
         self, drag_x: int, drag_y: int
     ) -> Optional[tuple[TreePath, TreeViewDropPosition]]: ...
     def get_drag_dest_row(self) -> Tuple[TreePath, TreeViewDropPosition]: ...
@@ -28280,20 +28303,19 @@
     def get_rubber_banding(self) -> bool: ...
     def get_rules_hint(self) -> bool: ...
     def get_search_column(self) -> int: ...
     def get_search_entry(self) -> Entry: ...
     def get_selection(self) -> TreeSelection: ...
     def get_show_expanders(self) -> bool: ...
     def get_tooltip_column(self) -> int: ...
-    # override
     def get_tooltip_context(
         self, x: int, y: int, keyboard_tip: bool
     ) -> tuple[bool, int, int, Optional[TreeModel], TreePath, TreeIter]: ...
     def get_vadjustment(self) -> Adjustment: ...
-    def get_visible_range(self, *args, **kwargs): ...  # FIXME Method
+    def get_visible_range(self, *args, **kwargs): ...
     def get_visible_rect(self) -> Gdk.Rectangle: ...
     def insert_column(self, column: TreeViewColumn, position: int) -> int: ...
     def insert_column_with_attributes(
         self, position: int, title: str, cell: CellRenderer, **kwargs: Any
     ) -> None: ...
     def insert_column_with_data_func(
         self,
@@ -28390,15 +28412,15 @@
     def unset_rows_drag_dest(self) -> None: ...
     def unset_rows_drag_source(self) -> None: ...
 
 class TreeViewAccessible(
     ContainerAccessible, Atk.Component, Atk.Selection, Atk.Table, CellAccessibleParent
 ):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -28475,15 +28497,15 @@
         sizing: TreeViewColumnSizing
         sort_column_id: int
         sort_indicator: bool
         sort_order: SortType
         spacing: int
         title: str
         visible: bool
-        widget: Widget
+        widget: Optional[Widget]
         width: int
         x_offset: int
     props: Props = ...
     parent_instance: GObject.InitiallyUnowned = ...
     priv: TreeViewColumnPrivate = ...
     def __init__(
         self,
@@ -28504,15 +28526,17 @@
         title: str = ...,
         visible: bool = ...,
         widget: Widget = ...,
     ): ...
     def add_attribute(
         self, cell_renderer: CellRenderer, attribute: str, column: int
     ) -> None: ...
-    def cell_get_position(self, *args, **kwargs): ...  # FIXME Method
+    def cell_get_position(
+        self, cell_renderer: CellRenderer
+    ) -> Optional[Tuple[int, int]]: ...  # CHECK Wrapped function
     def cell_get_size(
         self, cell_area: Optional[Gdk.Rectangle] = None
     ) -> Tuple[int, int, int, int]: ...
     def cell_is_visible(self) -> bool: ...
     def cell_set_cell_data(
         self,
         tree_model: TreeModel,
@@ -28549,15 +28573,15 @@
     def new(cls) -> TreeViewColumn: ...
     @classmethod
     def new_with_area(cls, area: CellArea) -> TreeViewColumn: ...
     def pack_end(self, cell: CellRenderer, expand: bool) -> None: ...
     def pack_start(self, cell: CellRenderer, expand: bool) -> None: ...
     def queue_resize(self) -> None: ...
     def set_alignment(self, xalign: float) -> None: ...
-    def set_attributes(self, *args, **kwargs): ...  # FIXME Method
+    def set_attributes(self, cell_renderer, **attributes): ...  # FIXME Function
     # override
     def set_cell_data_func(
         self,
         cell_renderer: CellRendererT,
         func: Callable[[TreeViewColumn, CellRendererT, TreeModel, TreeIter, Any], Any],
         func_data: Optional[object] = None,
     ) -> None: ...
@@ -28603,15 +28627,15 @@
         name: str,
         action: Optional[str],
         type: UIManagerItemType,
         top: bool,
     ) -> None: ...
     def add_ui_from_file(self, filename: str) -> int: ...
     def add_ui_from_resource(self, resource_path: str) -> int: ...
-    def add_ui_from_string(self, *args, **kwargs): ...  # FIXME Method
+    def add_ui_from_string(self, buffer): ...  # FIXME Function
     def do_actions_changed(self) -> None: ...
     def do_add_widget(self, widget: Widget) -> None: ...
     def do_connect_proxy(self, action: Action, proxy: Widget) -> None: ...
     def do_disconnect_proxy(self, action: Action, proxy: Widget) -> None: ...
     def do_get_action(self, path: str) -> Action: ...
     def do_get_widget(self, path: str) -> Widget: ...
     def do_post_activate(self, action: Action) -> None: ...
@@ -28620,15 +28644,15 @@
     def get_accel_group(self) -> AccelGroup: ...
     def get_action(self, path: str) -> Action: ...
     def get_action_groups(self) -> list[ActionGroup]: ...
     def get_add_tearoffs(self) -> bool: ...
     def get_toplevels(self, types: UIManagerItemType) -> list[Widget]: ...
     def get_ui(self) -> str: ...
     def get_widget(self, path: str) -> Widget: ...
-    def insert_action_group(self, *args, **kwargs): ...  # FIXME Method
+    def insert_action_group(self, buffer, length=-1): ...  # FIXME Function
     @classmethod
     def new(cls) -> UIManager: ...
     def new_merge_id(self) -> int: ...
     def remove_action_group(self, action_group: ActionGroup) -> None: ...
     def remove_ui(self, merge_id: int) -> None: ...
     def set_add_tearoffs(self, add_tearoffs: bool) -> None: ...
 
@@ -28651,15 +28675,14 @@
 
 class VBox(Box, Atk.ImplementorIface, Buildable, Orientable):
     class Props:
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -28679,28 +28702,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        child: Widget
     props: Props = ...
     box: Box = ...
     def __init__(
         self,
         baseline_position: BaselinePosition = ...,
         homogeneous: bool = ...,
         spacing: int = ...,
@@ -28754,15 +28778,14 @@
 class VButtonBox(ButtonBox, Atk.ImplementorIface, Buildable, Orientable):
     class Props:
         layout_style: ButtonBoxStyle
         baseline_position: BaselinePosition
         homogeneous: bool
         spacing: int
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -28782,28 +28805,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        child: Widget
     props: Props = ...
     button_box: ButtonBox = ...
     def __init__(
         self,
         layout_style: ButtonBoxStyle = ...,
         baseline_position: BaselinePosition = ...,
         homogeneous: bool = ...,
@@ -28859,15 +28883,14 @@
     class Props:
         max_position: int
         min_position: int
         position: int
         position_set: bool
         wide_handle: bool
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -28887,28 +28910,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
+        child: Widget
     props: Props = ...
     paned: Paned = ...
     def __init__(
         self,
         position: int = ...,
         position_set: bool = ...,
         wide_handle: bool = ...,
@@ -28995,27 +29019,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
     props: Props = ...
     scale: Scale = ...
     def __init__(
         self,
         digits: int = ...,
         draw_value: bool = ...,
@@ -29107,27 +29131,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
     props: Props = ...
     scrollbar: Scrollbar = ...
     def __init__(
         self,
         adjustment: Adjustment = ...,
         fill_level: float = ...,
@@ -29205,27 +29229,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         orientation: Orientation
     props: Props = ...
     separator: Separator = ...
     def __init__(
         self,
         app_paintable: bool = ...,
         can_default: bool = ...,
@@ -29271,15 +29295,14 @@
 class VSeparatorClass(GObject.GPointer):
     parent_class: SeparatorClass = ...
 
 class Viewport(Bin, Atk.ImplementorIface, Buildable, Scrollable):
     class Props:
         shadow_type: ShadowType
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -29299,31 +29322,32 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
         hadjustment: Adjustment
         hscroll_policy: ScrollablePolicy
         vadjustment: Adjustment
         vscroll_policy: ScrollablePolicy
+        child: Widget
     props: Props = ...
     bin: Bin = ...
     priv: ViewportPrivate = ...
     def __init__(
         self,
         shadow_type: ShadowType = ...,
         border_width: int = ...,
@@ -29400,24 +29424,23 @@
     class Props:
         use_symbolic: bool
         adjustment: Adjustment
         icons: list[str]
         size: IconSize
         value: float
         always_show_image: bool
-        image: Widget
+        image: Optional[Widget]
         image_position: PositionType
         label: str
         relief: ReliefStyle
         use_stock: bool
         use_underline: bool
         xalign: float
         yalign: float
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -29437,32 +29460,33 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
-        action_name: str
+        window: Optional[Gdk.Window]
+        action_name: Optional[str]
         action_target: GLib.Variant
         related_action: Action
         use_action_appearance: bool
         orientation: Orientation
+        child: Widget
     props: Props = ...
     parent: ScaleButton = ...
     def __init__(
         self,
         use_symbolic: bool = ...,
         adjustment: Adjustment = ...,
         icons: Sequence[str] = ...,
@@ -29556,27 +29580,27 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
     props: Props = ...
     parent_instance: GObject.InitiallyUnowned = ...
     priv: WidgetPrivate = ...
     def __init__(
         self,
         app_paintable: bool = ...,
         can_default: bool = ...,
@@ -29824,23 +29848,23 @@
         targets: Optional[Sequence[TargetEntry]],
         actions: Gdk.DragAction,
     ) -> None: ...
     def drag_source_set_icon_gicon(self, icon: Gio.Icon) -> None: ...
     def drag_source_set_icon_name(self, icon_name: str) -> None: ...
     def drag_source_set_icon_pixbuf(self, pixbuf: GdkPixbuf.Pixbuf) -> None: ...
     def drag_source_set_icon_stock(self, stock_id: str) -> None: ...
-    def drag_source_set_target_list(self, *args, **kwargs): ...  # FIXME Method
+    def drag_source_set_target_list(self, target_list): ...  # FIXME Function
     def drag_source_unset(self) -> None: ...
     def drag_unhighlight(self) -> None: ...
     def draw(self, cr: cairo.Context[_SomeSurface]) -> None: ...
     def ensure_style(self) -> None: ...
     def error_bell(self) -> None: ...
     def event(self, event: Gdk.Event) -> bool: ...
     def find_style_property(self, property_name: str) -> GObject.ParamSpec: ...
-    def freeze_child_notify(self, *args, **kwargs): ...  # FIXME Method
+    def freeze_child_notify(self): ...  # FIXME Function
     def get_accessible(self) -> Atk.Object: ...
     def get_action_group(self, prefix: str) -> Optional[Gio.ActionGroup]: ...
     def get_allocated_baseline(self) -> int: ...
     def get_allocated_height(self) -> int: ...
     def get_allocated_size(self) -> Tuple[Gdk.Rectangle, int]: ...
     def get_allocated_width(self) -> int: ...
     def get_allocation(self) -> Gdk.Rectangle: ...
@@ -30098,27 +30122,29 @@
     def show_now(self) -> None: ...
     def size_allocate(self, allocation: Gdk.Rectangle) -> None: ...
     def size_allocate_with_baseline(
         self, allocation: Gdk.Rectangle, baseline: int
     ) -> None: ...
     def size_request(self) -> Requisition: ...
     def style_attach(self) -> None: ...
-    def style_get_property(self, *args, **kwargs): ...  # FIXME Method
+    def style_get_property(self, property_name, value=None): ...  # FIXME Function
     def thaw_child_notify(self) -> None: ...
-    def translate_coordinates(self, *args, **kwargs): ...  # FIXME Method
+    def translate_coordinates(
+        self, dest_widget: Widget, src_x: int, src_y: int
+    ) -> Optional[Tuple[int, int]]: ...  # CHECK Wrapped function
     def trigger_tooltip_query(self) -> None: ...
     def unmap(self) -> None: ...
     def unparent(self) -> None: ...
     def unrealize(self) -> None: ...
     def unregister_window(self, window: Gdk.Window) -> None: ...
     def unset_state_flags(self, flags: StateFlags) -> None: ...
 
 class WidgetAccessible(Accessible, Atk.Component):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -30317,48 +30343,46 @@
     def unref(self) -> None: ...
 
 class WidgetPrivate(GObject.GPointer): ...
 
 class Window(Bin, Atk.ImplementorIface, Buildable):
     class Props:
         accept_focus: bool
-        application: Application
-        attached_to: Widget
+        application: Optional[Application]
+        attached_to: Optional[Widget]
         decorated: bool
         default_height: int
         default_width: int
         deletable: bool
         destroy_with_parent: bool
         focus_on_map: bool
         focus_visible: bool
         gravity: Gdk.Gravity
         has_resize_grip: bool
         has_toplevel_focus: bool
         hide_titlebar_when_maximized: bool
-        icon: GdkPixbuf.Pixbuf
-        icon_name: str
+        icon: Optional[GdkPixbuf.Pixbuf]
+        icon_name: Optional[str]
         is_active: bool
         is_maximized: bool
         mnemonics_visible: bool
         modal: bool
         resizable: bool
         resize_grip_visible: bool
-        role: str
+        role: Optional[str]
         screen: Gdk.Screen
         skip_pager_hint: bool
         skip_taskbar_hint: bool
-        startup_id: str
-        title: str
+        title: Optional[str]
         transient_for: Optional[Window]
         type: WindowType
         type_hint: Gdk.WindowTypeHint
         urgency_hint: bool
         window_position: WindowPosition
         border_width: int
-        child: Widget
         resize_mode: ResizeMode
         app_paintable: bool
         can_default: bool
         can_focus: bool
         composite_child: bool
         double_buffered: bool
         events: Gdk.EventMask
@@ -30378,27 +30402,29 @@
         margin_left: int
         margin_right: int
         margin_start: int
         margin_top: int
         name: str
         no_show_all: bool
         opacity: float
-        parent: Container
+        parent: Optional[Container]
         receives_default: bool
         scale_factor: int
         sensitive: bool
         style: Style
-        tooltip_markup: str
-        tooltip_text: str
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
         valign: Align
         vexpand: bool
         vexpand_set: bool
         visible: bool
         width_request: int
-        window: Gdk.Window
+        window: Optional[Gdk.Window]
+        startup_id: str
+        child: Widget
     props: Props = ...
     bin: Bin = ...
     priv: WindowPrivate = ...
     def __init__(
         self,
         accept_focus: bool = ...,
         application: Application = ...,
@@ -30616,15 +30642,15 @@
     def stick(self) -> None: ...
     def unfullscreen(self) -> None: ...
     def unmaximize(self) -> None: ...
     def unstick(self) -> None: ...
 
 class WindowAccessible(ContainerAccessible, Atk.Component, Atk.Window):
     class Props:
-        widget: Widget
+        widget: Optional[Widget]
         accessible_component_layer: int
         accessible_component_mdi_zorder: int
         accessible_description: str
         accessible_hypertext_nlinks: int
         accessible_name: str
         accessible_parent: Atk.Object
         accessible_role: Atk.Role
@@ -30690,14 +30716,40 @@
     _gtk_reserved1: None = ...
     _gtk_reserved2: None = ...
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
 
 class WindowGroupPrivate(GObject.GPointer): ...
 class WindowPrivate(GObject.GPointer): ...
+class _MountOperationHandler(GObject.GPointer): ...
+
+class _MountOperationHandlerIface(GObject.GPointer):
+    parent_iface: GObject.TypeInterface = ...
+    handle_ask_password: None = ...
+    handle_ask_question: None = ...
+    handle_close: None = ...
+    handle_show_processes: None = ...
+
+class _MountOperationHandlerProxy(GObject.GPointer):
+    parent_instance: Gio.DBusProxy = ...
+    priv: None = ...
+
+class _MountOperationHandlerProxyClass(GObject.GPointer):
+    parent_class: Gio.DBusProxyClass = ...
+
+class _MountOperationHandlerProxyPrivate(GObject.GPointer): ...
+
+class _MountOperationHandlerSkeleton(GObject.GPointer):
+    parent_instance: Gio.DBusInterfaceSkeleton = ...
+    priv: None = ...
+
+class _MountOperationHandlerSkeletonClass(GObject.GPointer):
+    parent_class: Gio.DBusInterfaceSkeletonClass = ...
+
+class _MountOperationHandlerSkeletonPrivate(GObject.GPointer): ...
 
 class AccelFlags(GObject.GFlags):
     LOCKED = 2
     MASK = 7
     VISIBLE = 1
 
 class ApplicationInhibitFlags(GObject.GFlags):
```

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/_Gtk4.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Gtk4.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 from gi.repository import Graphene
 from gi.repository import Gsk
 from gi.repository import Pango
 
 _SomeSurface = TypeVar("_SomeSurface", bound=cairo.Surface)
 
 ACCESSIBLE_VALUE_UNDEFINED: int = -1
-BINARY_AGE: int = 803
+BINARY_AGE: int = 1001
 IM_MODULE_EXTENSION_POINT_NAME: str = "gtk-im-module"
 INPUT_ERROR: int = -1
-INTERFACE_AGE: int = 3
+INTERFACE_AGE: int = 1
 INVALID_LIST_POSITION: int = 4294967295
 LEVEL_BAR_OFFSET_FULL: str = "full"
 LEVEL_BAR_OFFSET_HIGH: str = "high"
 LEVEL_BAR_OFFSET_LOW: str = "low"
 MAJOR_VERSION: int = 4
 MAX_COMPOSE_LEN: int = 7
 MEDIA_FILE_EXTENSION_POINT_NAME: str = "gtk-media-file"
-MICRO_VERSION: int = 3
-MINOR_VERSION: int = 8
+MICRO_VERSION: int = 1
+MINOR_VERSION: int = 10
 PAPER_NAME_A3: str = "iso_a3"
 PAPER_NAME_A4: str = "iso_a4"
 PAPER_NAME_A5: str = "iso_a5"
 PAPER_NAME_B5: str = "iso_b5"
 PAPER_NAME_EXECUTIVE: str = "na_executive"
 PAPER_NAME_LEGAL: str = "na_legal"
 PAPER_NAME_LETTER: str = "na_letter"
@@ -124,14 +124,15 @@
 def builder_error_quark() -> int: ...
 def check_version(
     required_major: int, required_minor: int, required_micro: int
 ) -> Optional[str]: ...
 def constraint_vfl_parser_error_quark() -> int: ...
 def css_parser_error_quark() -> int: ...
 def css_parser_warning_quark() -> int: ...
+def dialog_error_quark() -> int: ...
 def disable_setlocale() -> None: ...
 def distribute_natural_allocation(
     extra_space: int, n_requested_sizes: int, sizes: Sequence[RequestedSize]
 ) -> int: ...
 def editable_delegate_get_property(
     object: GObject.Object, prop_id: int, value: Any, pspec: GObject.ParamSpec
 ) -> bool: ...
@@ -273,15 +274,17 @@
 def set_debug_flags(flags: DebugFlags) -> None: ...
 def show_uri(parent: Optional[Window], uri: str, timestamp: int) -> None: ...
 def show_uri_full(
     parent: Optional[Window],
     uri: str,
     timestamp: int,
     cancellable: Optional[Gio.Cancellable] = None,
-    callback: Optional[Callable[..., None]] = None,
+    callback: Optional[
+        Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+    ] = None,
     *user_data: Any,
 ) -> None: ...
 def show_uri_full_finish(parent: Window, result: Gio.AsyncResult) -> bool: ...
 def test_accessible_assertion_message_role(
     domain: str,
     file: str,
     line: int,
@@ -530,18 +533,32 @@
     ) -> None: ...
     def set_version(self, version: Optional[str] = None) -> None: ...
     def set_website(self, website: Optional[str] = None) -> None: ...
     def set_website_label(self, website_label: str) -> None: ...
     def set_wrap_license(self, wrap_license: bool) -> None: ...
 
 class Accessible(GObject.GInterface):
+    def get_accessible_parent(self) -> Optional[Accessible]: ...
     def get_accessible_role(self) -> AccessibleRole: ...
+    def get_at_context(self) -> ATContext: ...
+    def get_bounds(self) -> Tuple[bool, int, int, int, int]: ...
+    def get_first_accessible_child(self) -> Optional[Accessible]: ...
+    def get_next_accessible_sibling(self) -> Optional[Accessible]: ...
+    def get_platform_state(self, state: AccessiblePlatformState) -> bool: ...
     def reset_property(self, property: AccessibleProperty) -> None: ...
     def reset_relation(self, relation: AccessibleRelation) -> None: ...
     def reset_state(self, state: AccessibleState) -> None: ...
+    def set_accessible_parent(
+        self,
+        parent: Optional[Accessible] = None,
+        next_sibling: Optional[Accessible] = None,
+    ) -> None: ...
+    def update_next_accessible_sibling(
+        self, new_sibling: Optional[Accessible] = None
+    ) -> None: ...
     def update_property(
         self,
         n_properties: int,
         properties: Sequence[AccessibleProperty],
         values: Sequence[Any],
     ) -> None: ...
     def update_relation(
@@ -550,15 +567,28 @@
         relations: Sequence[AccessibleRelation],
         values: Sequence[Any],
     ) -> None: ...
     def update_state(
         self, n_states: int, states: Sequence[AccessibleState], values: Sequence[Any]
     ) -> None: ...
 
-class AccessibleInterface(GObject.GPointer): ...
+class AccessibleInterface(GObject.GPointer):
+    g_iface: GObject.TypeInterface = ...
+    get_at_context: Callable[[Accessible], Optional[ATContext]] = ...
+    get_platform_state: Callable[[Accessible, AccessiblePlatformState], bool] = ...
+    get_accessible_parent: Callable[[Accessible], Optional[Accessible]] = ...
+    get_first_accessible_child: Callable[[Accessible], Optional[Accessible]] = ...
+    get_next_accessible_sibling: Callable[[Accessible], Optional[Accessible]] = ...
+    get_bounds: Callable[[Accessible], Tuple[bool, int, int, int, int]] = ...
+
+class AccessibleRange(GObject.GInterface): ...
+
+class AccessibleRangeInterface(GObject.GPointer):
+    g_iface: GObject.TypeInterface = ...
+    set_current_value: Callable[[AccessibleRange, float], bool] = ...
 
 class ActionBar(Widget, Accessible, Buildable, ConstraintTarget):
     class Props:
         revealed: bool
         can_focus: bool
         can_target: bool
         css_classes: list[str]
@@ -721,14 +751,59 @@
     changed: Callable[[Adjustment], None] = ...
     value_changed: Callable[[Adjustment], None] = ...
     _gtk_reserved1: None = ...
     _gtk_reserved2: None = ...
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
 
+class AlertDialog(GObject.Object):
+    class Props:
+        buttons: Optional[list[str]]
+        cancel_button: int
+        default_button: int
+        detail: str
+        message: str
+        modal: bool
+    props: Props = ...
+    def __init__(
+        self,
+        buttons: Sequence[str] = ...,
+        cancel_button: int = ...,
+        default_button: int = ...,
+        detail: str = ...,
+        message: str = ...,
+        modal: bool = ...,
+    ): ...
+    def choose(
+        self,
+        parent: Optional[Window] = None,
+        cancellable: Optional[Gio.Cancellable] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
+        *user_data: Any,
+    ) -> None: ...
+    def choose_finish(self, result: Gio.AsyncResult) -> int: ...
+    def get_buttons(self) -> Optional[list[str]]: ...
+    def get_cancel_button(self) -> int: ...
+    def get_default_button(self) -> int: ...
+    def get_detail(self) -> str: ...
+    def get_message(self) -> str: ...
+    def get_modal(self) -> bool: ...
+    def set_buttons(self, labels: Sequence[str]) -> None: ...
+    def set_cancel_button(self, button: int) -> None: ...
+    def set_default_button(self, button: int) -> None: ...
+    def set_detail(self, detail: str) -> None: ...
+    def set_message(self, message: str) -> None: ...
+    def set_modal(self, modal: bool) -> None: ...
+    def show(self, parent: Optional[Window] = None) -> None: ...
+
+class AlertDialogClass(GObject.GPointer):
+    parent_class: GObject.ObjectClass = ...
+
 class AlternativeTrigger(ShortcutTrigger):
     class Props:
         first: ShortcutTrigger
         second: ShortcutTrigger
     props: Props = ...
     def __init__(self, first: ShortcutTrigger = ..., second: ShortcutTrigger = ...): ...
     def get_first(self) -> ShortcutTrigger: ...
@@ -2076,15 +2151,15 @@
     def get_has_frame(self) -> bool: ...
     def get_icon_name(self) -> Optional[str]: ...
     def get_label(self) -> Optional[str]: ...
     def get_use_underline(self) -> bool: ...
     @classmethod
     def new(cls) -> Button: ...
     @classmethod
-    def new_from_icon_name(cls, icon_name: Optional[str] = None) -> Button: ...
+    def new_from_icon_name(cls, icon_name: str) -> Button: ...
     @classmethod
     def new_with_label(cls, label: str) -> Button: ...
     @classmethod
     def new_with_mnemonic(cls, label: str) -> Button: ...
     def set_child(self, child: Optional[Widget] = None) -> None: ...
     def set_has_frame(self, has_frame: bool) -> None: ...
     def set_icon_name(self, icon_name: str) -> None: ...
@@ -2100,15 +2175,20 @@
 class ButtonPrivate(GObject.GPointer): ...
 
 class CClosureExpression(Expression):
     @classmethod
     def new(
         cls,
         value_type: Type,
-        marshal: Optional[Callable[..., None]],
+        marshal: Optional[
+            Callable[
+                [Callable[..., Any], Optional[Any], int, Sequence[Any], None, None],
+                None,
+            ]
+        ],
         n_params: int,
         params: Sequence[Expression],
         callback_func: Callable[[], None],
         *user_data: Any,
     ) -> CClosureExpression: ...
 
 class Calendar(Widget, Accessible, Buildable, ConstraintTarget):
@@ -3649,14 +3729,17 @@
     def set_draw_sensitive(self, draw_sensitive: bool) -> None: ...
     def set_fit_model(self, fit_model: bool) -> None: ...
     def set_model(self, model: Optional[TreeModel] = None) -> None: ...
 
 class CenterBox(Widget, Accessible, Buildable, ConstraintTarget, Orientable):
     class Props:
         baseline_position: BaselinePosition
+        center_widget: Optional[Widget]
+        end_widget: Optional[Widget]
+        start_widget: Optional[Widget]
         can_focus: bool
         can_target: bool
         css_classes: list[str]
         css_name: str
         cursor: Optional[Gdk.Cursor]
         focus_on_click: bool
         focusable: bool
@@ -3689,14 +3772,17 @@
         width_request: int
         accessible_role: AccessibleRole
         orientation: Orientation
     props: Props = ...
     def __init__(
         self,
         baseline_position: BaselinePosition = ...,
+        center_widget: Widget = ...,
+        end_widget: Widget = ...,
+        start_widget: Widget = ...,
         can_focus: bool = ...,
         can_target: bool = ...,
         css_classes: Sequence[str] = ...,
         css_name: str = ...,
         cursor: Gdk.Cursor = ...,
         focus_on_click: bool = ...,
         focusable: bool = ...,
@@ -4208,14 +4294,129 @@
         accessible_role: AccessibleRole = ...,
         rgba: Gdk.RGBA = ...,
         use_alpha: bool = ...,
     ): ...
     @classmethod
     def new(cls) -> ColorChooserWidget: ...
 
+class ColorDialog(GObject.Object):
+    class Props:
+        modal: bool
+        title: str
+        with_alpha: bool
+    props: Props = ...
+    def __init__(self, modal: bool = ..., title: str = ..., with_alpha: bool = ...): ...
+    def choose_rgba(
+        self,
+        parent: Optional[Window] = None,
+        initial_color: Optional[Gdk.RGBA] = None,
+        cancellable: Optional[Gio.Cancellable] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
+        *user_data: Any,
+    ) -> None: ...
+    def choose_rgba_finish(self, result: Gio.AsyncResult) -> Optional[Gdk.RGBA]: ...
+    def get_modal(self) -> bool: ...
+    def get_title(self) -> str: ...
+    def get_with_alpha(self) -> bool: ...
+    @classmethod
+    def new(cls) -> ColorDialog: ...
+    def set_modal(self, modal: bool) -> None: ...
+    def set_title(self, title: str) -> None: ...
+    def set_with_alpha(self, with_alpha: bool) -> None: ...
+
+class ColorDialogButton(Widget, Accessible, Buildable, ConstraintTarget):
+    class Props:
+        dialog: Optional[ColorDialog]
+        rgba: Gdk.RGBA
+        can_focus: bool
+        can_target: bool
+        css_classes: list[str]
+        css_name: str
+        cursor: Optional[Gdk.Cursor]
+        focus_on_click: bool
+        focusable: bool
+        halign: Align
+        has_default: bool
+        has_focus: bool
+        has_tooltip: bool
+        height_request: int
+        hexpand: bool
+        hexpand_set: bool
+        layout_manager: Optional[LayoutManager]
+        margin_bottom: int
+        margin_end: int
+        margin_start: int
+        margin_top: int
+        name: str
+        opacity: float
+        overflow: Overflow
+        parent: Optional[Widget]
+        receives_default: bool
+        root: Optional[Root]
+        scale_factor: int
+        sensitive: bool
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
+        valign: Align
+        vexpand: bool
+        vexpand_set: bool
+        visible: bool
+        width_request: int
+        accessible_role: AccessibleRole
+    props: Props = ...
+    def __init__(
+        self,
+        dialog: ColorDialog = ...,
+        rgba: Gdk.RGBA = ...,
+        can_focus: bool = ...,
+        can_target: bool = ...,
+        css_classes: Sequence[str] = ...,
+        css_name: str = ...,
+        cursor: Gdk.Cursor = ...,
+        focus_on_click: bool = ...,
+        focusable: bool = ...,
+        halign: Align = ...,
+        has_tooltip: bool = ...,
+        height_request: int = ...,
+        hexpand: bool = ...,
+        hexpand_set: bool = ...,
+        layout_manager: LayoutManager = ...,
+        margin_bottom: int = ...,
+        margin_end: int = ...,
+        margin_start: int = ...,
+        margin_top: int = ...,
+        name: str = ...,
+        opacity: float = ...,
+        overflow: Overflow = ...,
+        receives_default: bool = ...,
+        sensitive: bool = ...,
+        tooltip_markup: str = ...,
+        tooltip_text: str = ...,
+        valign: Align = ...,
+        vexpand: bool = ...,
+        vexpand_set: bool = ...,
+        visible: bool = ...,
+        width_request: int = ...,
+        accessible_role: AccessibleRole = ...,
+    ): ...
+    def get_dialog(self) -> Optional[ColorDialog]: ...
+    def get_rgba(self) -> Gdk.RGBA: ...
+    @classmethod
+    def new(cls, dialog: Optional[ColorDialog] = None) -> ColorDialogButton: ...
+    def set_dialog(self, dialog: ColorDialog) -> None: ...
+    def set_rgba(self, color: Gdk.RGBA) -> None: ...
+
+class ColorDialogButtonClass(GObject.GPointer):
+    parent_class: WidgetClass = ...
+
+class ColorDialogClass(GObject.GPointer):
+    parent_class: GObject.ObjectClass = ...
+
 class ColumnView(Widget, Accessible, Buildable, ConstraintTarget, Scrollable):
     class Props:
         columns: Gio.ListModel
         enable_rubberband: bool
         model: Optional[SelectionModel]
         reorderable: bool
         show_column_separators: bool
@@ -4333,54 +4534,73 @@
 class ColumnViewColumn(GObject.Object):
     class Props:
         column_view: Optional[ColumnView]
         expand: bool
         factory: Optional[ListItemFactory]
         fixed_width: int
         header_menu: Optional[Gio.MenuModel]
+        id: Optional[str]
         resizable: bool
         sorter: Optional[Sorter]
         title: Optional[str]
         visible: bool
     props: Props = ...
     def __init__(
         self,
         expand: bool = ...,
         factory: ListItemFactory = ...,
         fixed_width: int = ...,
         header_menu: Gio.MenuModel = ...,
+        id: str = ...,
         resizable: bool = ...,
         sorter: Sorter = ...,
         title: str = ...,
         visible: bool = ...,
     ): ...
     def get_column_view(self) -> Optional[ColumnView]: ...
     def get_expand(self) -> bool: ...
     def get_factory(self) -> Optional[ListItemFactory]: ...
     def get_fixed_width(self) -> int: ...
     def get_header_menu(self) -> Optional[Gio.MenuModel]: ...
+    def get_id(self) -> Optional[str]: ...
     def get_resizable(self) -> bool: ...
     def get_sorter(self) -> Optional[Sorter]: ...
     def get_title(self) -> Optional[str]: ...
     def get_visible(self) -> bool: ...
     @classmethod
     def new(
         cls, title: Optional[str] = None, factory: Optional[ListItemFactory] = None
     ) -> ColumnViewColumn: ...
     def set_expand(self, expand: bool) -> None: ...
     def set_factory(self, factory: Optional[ListItemFactory] = None) -> None: ...
     def set_fixed_width(self, fixed_width: int) -> None: ...
     def set_header_menu(self, menu: Optional[Gio.MenuModel] = None) -> None: ...
+    def set_id(self, id: Optional[str] = None) -> None: ...
     def set_resizable(self, resizable: bool) -> None: ...
     def set_sorter(self, sorter: Optional[Sorter] = None) -> None: ...
     def set_title(self, title: Optional[str] = None) -> None: ...
     def set_visible(self, visible: bool) -> None: ...
 
 class ColumnViewColumnClass(GObject.GPointer): ...
 
+class ColumnViewSorter(Sorter):
+    class Props:
+        primary_sort_column: Optional[ColumnViewColumn]
+        primary_sort_order: SortType
+    props: Props = ...
+    def get_n_sort_columns(self) -> int: ...
+    def get_nth_sort_column(
+        self, position: int
+    ) -> Tuple[Optional[ColumnViewColumn], SortType]: ...
+    def get_primary_sort_column(self) -> Optional[ColumnViewColumn]: ...
+    def get_primary_sort_order(self) -> SortType: ...
+
+class ColumnViewSorterClass(GObject.GPointer):
+    parent_class: SorterClass = ...
+
 class ComboBox(
     Widget, Accessible, Buildable, CellEditable, CellLayout, ConstraintTarget
 ):
     class Props:
         active: int
         active_id: Optional[str]
         button_sensitivity: SensitivityType
@@ -4770,15 +4990,15 @@
     chars: int = ...
     lines: int = ...
     line_bytes: int = ...
     line_chars: int = ...
 
 class CssProvider(GObject.Object, StyleProvider):
     parent_instance: GObject.Object = ...
-    def load_from_data(self, data: Sequence[int]) -> None: ...
+    def load_from_data(self, data: str, length: int) -> None: ...
     def load_from_file(self, file: Gio.File) -> None: ...
     def load_from_path(self, path: str) -> None: ...
     def load_from_resource(self, resource_path: str) -> None: ...
     def load_named(self, name: str, variant: Optional[str] = None) -> None: ...
     @classmethod
     def new(cls) -> CssProvider: ...
     def to_string(self) -> str: ...
@@ -5430,14 +5650,17 @@
     def set_actions(self, actions: Gdk.DragAction) -> None: ...
     def set_formats(self, formats: Optional[Gdk.ContentFormats] = None) -> None: ...
 
 class DropTargetAsyncClass(GObject.GPointer): ...
 class DropTargetClass(GObject.GPointer): ...
 
 class Editable(GObject.GInterface):
+    def delegate_get_accessible_platform_state(
+        self, state: AccessiblePlatformState
+    ) -> bool: ...
     @staticmethod
     def delegate_get_property(
         object: GObject.Object, prop_id: int, value: Any, pspec: GObject.ParamSpec
     ) -> bool: ...
     @staticmethod
     def delegate_set_property(
         object: GObject.Object, prop_id: int, value: Any, pspec: GObject.ParamSpec
@@ -6513,14 +6736,15 @@
 
 class FileChooserNativeClass(GObject.GPointer):
     parent_class: NativeDialogClass = ...
 
 class FileChooserWidget(Widget, Accessible, Buildable, ConstraintTarget, FileChooser):
     class Props:
         search_mode: bool
+        show_time: bool
         subtitle: str
         can_focus: bool
         can_target: bool
         css_classes: list[str]
         css_name: str
         cursor: Optional[Gdk.Cursor]
         focus_on_click: bool
@@ -6597,32 +6821,172 @@
         create_folders: bool = ...,
         filter: FileFilter = ...,
         select_multiple: bool = ...,
     ): ...
     @classmethod
     def new(cls, action: FileChooserAction) -> FileChooserWidget: ...
 
+class FileDialog(GObject.Object):
+    class Props:
+        accept_label: Optional[str]
+        default_filter: Optional[FileFilter]
+        filters: Optional[Gio.ListModel]
+        initial_file: Optional[Gio.File]
+        initial_folder: Optional[Gio.File]
+        initial_name: Optional[str]
+        modal: bool
+        title: str
+    props: Props = ...
+    def __init__(
+        self,
+        accept_label: str = ...,
+        default_filter: FileFilter = ...,
+        filters: Gio.ListModel = ...,
+        initial_file: Gio.File = ...,
+        initial_folder: Gio.File = ...,
+        initial_name: str = ...,
+        modal: bool = ...,
+        title: str = ...,
+    ): ...
+    def get_accept_label(self) -> Optional[str]: ...
+    def get_default_filter(self) -> Optional[FileFilter]: ...
+    def get_filters(self) -> Optional[Gio.ListModel]: ...
+    def get_initial_file(self) -> Optional[Gio.File]: ...
+    def get_initial_folder(self) -> Optional[Gio.File]: ...
+    def get_initial_name(self) -> Optional[str]: ...
+    def get_modal(self) -> bool: ...
+    def get_title(self) -> str: ...
+    @classmethod
+    def new(cls) -> FileDialog: ...
+    def open(
+        self,
+        parent: Optional[Window] = None,
+        cancellable: Optional[Gio.Cancellable] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
+        *user_data: Any,
+    ) -> None: ...
+    def open_finish(self, result: Gio.AsyncResult) -> Optional[Gio.File]: ...
+    def open_multiple(
+        self,
+        parent: Optional[Window] = None,
+        cancellable: Optional[Gio.Cancellable] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
+        *user_data: Any,
+    ) -> None: ...
+    def open_multiple_finish(
+        self, result: Gio.AsyncResult
+    ) -> Optional[Gio.ListModel]: ...
+    def save(
+        self,
+        parent: Optional[Window] = None,
+        cancellable: Optional[Gio.Cancellable] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
+        *user_data: Any,
+    ) -> None: ...
+    def save_finish(self, result: Gio.AsyncResult) -> Optional[Gio.File]: ...
+    def select_folder(
+        self,
+        parent: Optional[Window] = None,
+        cancellable: Optional[Gio.Cancellable] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
+        *user_data: Any,
+    ) -> None: ...
+    def select_folder_finish(self, result: Gio.AsyncResult) -> Optional[Gio.File]: ...
+    def select_multiple_folders(
+        self,
+        parent: Optional[Window] = None,
+        cancellable: Optional[Gio.Cancellable] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
+        *user_data: Any,
+    ) -> None: ...
+    def select_multiple_folders_finish(
+        self, result: Gio.AsyncResult
+    ) -> Optional[Gio.ListModel]: ...
+    def set_accept_label(self, accept_label: Optional[str] = None) -> None: ...
+    def set_default_filter(self, filter: Optional[FileFilter] = None) -> None: ...
+    def set_filters(self, filters: Gio.ListModel) -> None: ...
+    def set_initial_file(self, file: Optional[Gio.File] = None) -> None: ...
+    def set_initial_folder(self, folder: Optional[Gio.File] = None) -> None: ...
+    def set_initial_name(self, name: Optional[str] = None) -> None: ...
+    def set_modal(self, modal: bool) -> None: ...
+    def set_title(self, title: str) -> None: ...
+
+class FileDialogClass(GObject.GPointer):
+    parent_class: GObject.ObjectClass = ...
+
 class FileFilter(Filter, Buildable):
     class Props:
         name: Optional[str]
+        mime_types: list[str]
+        patterns: list[str]
+        suffixes: list[str]
     props: Props = ...
-    def __init__(self, name: str = ...): ...
+    def __init__(
+        self,
+        mime_types: Sequence[str] = ...,
+        name: str = ...,
+        patterns: Sequence[str] = ...,
+        suffixes: Sequence[str] = ...,
+    ): ...
     def add_mime_type(self, mime_type: str) -> None: ...
     def add_pattern(self, pattern: str) -> None: ...
     def add_pixbuf_formats(self) -> None: ...
     def add_suffix(self, suffix: str) -> None: ...
     def get_attributes(self) -> list[str]: ...
     def get_name(self) -> Optional[str]: ...
     @classmethod
     def new(cls) -> FileFilter: ...
     @classmethod
     def new_from_gvariant(cls, variant: GLib.Variant) -> FileFilter: ...
     def set_name(self, name: Optional[str] = None) -> None: ...
     def to_gvariant(self) -> GLib.Variant: ...
 
+class FileLauncher(GObject.Object):
+    class Props:
+        file: Optional[Gio.File]
+    props: Props = ...
+    def __init__(self, file: Gio.File = ...): ...
+    def get_file(self) -> Optional[Gio.File]: ...
+    def launch(
+        self,
+        parent: Optional[Window] = None,
+        cancellable: Optional[Gio.Cancellable] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
+        *user_data: Any,
+    ) -> None: ...
+    def launch_finish(self, result: Gio.AsyncResult) -> bool: ...
+    @classmethod
+    def new(cls, file: Optional[Gio.File] = None) -> FileLauncher: ...
+    def open_containing_folder(
+        self,
+        parent: Optional[Window] = None,
+        cancellable: Optional[Gio.Cancellable] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
+        *user_data: Any,
+    ) -> None: ...
+    def open_containing_folder_finish(self, result: Gio.AsyncResult) -> bool: ...
+    def set_file(self, file: Optional[Gio.File] = None) -> None: ...
+
+class FileLauncherClass(GObject.GPointer):
+    parent_class: GObject.ObjectClass = ...
+
 class Filter(GObject.Object):
     parent_instance: GObject.Object = ...
     def changed(self, change: FilterChange) -> None: ...
     def do_get_strictness(self) -> FilterMatch: ...
     def do_match(self, item: Optional[GObject.Object] = None) -> bool: ...
     def get_strictness(self) -> FilterMatch: ...
     def match(self, item: GObject.Object) -> bool: ...
@@ -7387,14 +7751,203 @@
         level: FontChooserLevel = ...,
         preview_text: str = ...,
         show_preview_entry: bool = ...,
     ): ...
     @classmethod
     def new(cls) -> FontChooserWidget: ...
 
+class FontDialog(GObject.Object):
+    class Props:
+        filter: Optional[Filter]
+        font_map: Optional[Pango.FontMap]
+        language: Optional[Pango.Language]
+        modal: bool
+        title: str
+    props: Props = ...
+    def __init__(
+        self,
+        filter: Filter = ...,
+        font_map: Pango.FontMap = ...,
+        language: Pango.Language = ...,
+        modal: bool = ...,
+        title: str = ...,
+    ): ...
+    def choose_face(
+        self,
+        parent: Optional[Window] = None,
+        initial_value: Optional[Pango.FontFace] = None,
+        cancellable: Optional[Gio.Cancellable] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
+        *user_data: Any,
+    ) -> None: ...
+    def choose_face_finish(
+        self, result: Gio.AsyncResult
+    ) -> Optional[Pango.FontFace]: ...
+    def choose_family(
+        self,
+        parent: Optional[Window] = None,
+        initial_value: Optional[Pango.FontFamily] = None,
+        cancellable: Optional[Gio.Cancellable] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
+        *user_data: Any,
+    ) -> None: ...
+    def choose_family_finish(
+        self, result: Gio.AsyncResult
+    ) -> Optional[Pango.FontFamily]: ...
+    def choose_font(
+        self,
+        parent: Optional[Window] = None,
+        initial_value: Optional[Pango.FontDescription] = None,
+        cancellable: Optional[Gio.Cancellable] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
+        *user_data: Any,
+    ) -> None: ...
+    def choose_font_and_features(
+        self,
+        parent: Optional[Window] = None,
+        initial_value: Optional[Pango.FontDescription] = None,
+        cancellable: Optional[Gio.Cancellable] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
+        *user_data: Any,
+    ) -> None: ...
+    def choose_font_and_features_finish(
+        self, result: Gio.AsyncResult
+    ) -> Tuple[bool, Pango.FontDescription, str, Pango.Language]: ...
+    def choose_font_finish(
+        self, result: Gio.AsyncResult
+    ) -> Optional[Pango.FontDescription]: ...
+    def get_filter(self) -> Optional[Filter]: ...
+    def get_font_map(self) -> Optional[Pango.FontMap]: ...
+    def get_language(self) -> Optional[Pango.Language]: ...
+    def get_modal(self) -> bool: ...
+    def get_title(self) -> str: ...
+    @classmethod
+    def new(cls) -> FontDialog: ...
+    def set_filter(self, filter: Optional[Filter] = None) -> None: ...
+    def set_font_map(self, fontmap: Optional[Pango.FontMap] = None) -> None: ...
+    def set_language(self, language: Pango.Language) -> None: ...
+    def set_modal(self, modal: bool) -> None: ...
+    def set_title(self, title: str) -> None: ...
+
+class FontDialogButton(Widget, Accessible, Buildable, ConstraintTarget):
+    class Props:
+        dialog: Optional[FontDialog]
+        font_desc: Optional[Pango.FontDescription]
+        font_features: Optional[str]
+        language: Optional[Pango.Language]
+        level: FontLevel
+        use_font: bool
+        use_size: bool
+        can_focus: bool
+        can_target: bool
+        css_classes: list[str]
+        css_name: str
+        cursor: Optional[Gdk.Cursor]
+        focus_on_click: bool
+        focusable: bool
+        halign: Align
+        has_default: bool
+        has_focus: bool
+        has_tooltip: bool
+        height_request: int
+        hexpand: bool
+        hexpand_set: bool
+        layout_manager: Optional[LayoutManager]
+        margin_bottom: int
+        margin_end: int
+        margin_start: int
+        margin_top: int
+        name: str
+        opacity: float
+        overflow: Overflow
+        parent: Optional[Widget]
+        receives_default: bool
+        root: Optional[Root]
+        scale_factor: int
+        sensitive: bool
+        tooltip_markup: Optional[str]
+        tooltip_text: Optional[str]
+        valign: Align
+        vexpand: bool
+        vexpand_set: bool
+        visible: bool
+        width_request: int
+        accessible_role: AccessibleRole
+    props: Props = ...
+    def __init__(
+        self,
+        dialog: FontDialog = ...,
+        font_desc: Pango.FontDescription = ...,
+        font_features: str = ...,
+        language: Pango.Language = ...,
+        level: FontLevel = ...,
+        use_font: bool = ...,
+        use_size: bool = ...,
+        can_focus: bool = ...,
+        can_target: bool = ...,
+        css_classes: Sequence[str] = ...,
+        css_name: str = ...,
+        cursor: Gdk.Cursor = ...,
+        focus_on_click: bool = ...,
+        focusable: bool = ...,
+        halign: Align = ...,
+        has_tooltip: bool = ...,
+        height_request: int = ...,
+        hexpand: bool = ...,
+        hexpand_set: bool = ...,
+        layout_manager: LayoutManager = ...,
+        margin_bottom: int = ...,
+        margin_end: int = ...,
+        margin_start: int = ...,
+        margin_top: int = ...,
+        name: str = ...,
+        opacity: float = ...,
+        overflow: Overflow = ...,
+        receives_default: bool = ...,
+        sensitive: bool = ...,
+        tooltip_markup: str = ...,
+        tooltip_text: str = ...,
+        valign: Align = ...,
+        vexpand: bool = ...,
+        vexpand_set: bool = ...,
+        visible: bool = ...,
+        width_request: int = ...,
+        accessible_role: AccessibleRole = ...,
+    ): ...
+    def get_dialog(self) -> Optional[FontDialog]: ...
+    def get_font_desc(self) -> Optional[Pango.FontDescription]: ...
+    def get_font_features(self) -> Optional[str]: ...
+    def get_language(self) -> Optional[Pango.Language]: ...
+    def get_level(self) -> FontLevel: ...
+    def get_use_font(self) -> bool: ...
+    def get_use_size(self) -> bool: ...
+    @classmethod
+    def new(cls, dialog: Optional[FontDialog] = None) -> FontDialogButton: ...
+    def set_dialog(self, dialog: FontDialog) -> None: ...
+    def set_font_desc(self, font_desc: Pango.FontDescription) -> None: ...
+    def set_font_features(self, font_features: Optional[str] = None) -> None: ...
+    def set_language(self, language: Optional[Pango.Language] = None) -> None: ...
+    def set_level(self, level: FontLevel) -> None: ...
+    def set_use_font(self, use_font: bool) -> None: ...
+    def set_use_size(self, use_size: bool) -> None: ...
+
+class FontDialogButtonClass(GObject.GPointer):
+    parent_class: WidgetClass = ...
+
+class FontDialogClass(GObject.GPointer):
+    parent_class: GObject.ObjectClass = ...
+
 class Frame(Widget, Accessible, Buildable, ConstraintTarget):
     class Props:
         child: Optional[Widget]
         label: Optional[str]
         label_widget: Optional[Widget]
         label_xalign: float
         can_focus: bool
@@ -7805,39 +8358,43 @@
     def set_exclusive(self, exclusive: bool) -> None: ...
     def set_touch_only(self, touch_only: bool) -> None: ...
 
 class GestureSingleClass(GObject.GPointer): ...
 
 class GestureStylus(GestureSingle):
     class Props:
+        stylus_only: bool
         button: int
         exclusive: bool
         touch_only: bool
         n_points: int
         name: Optional[str]
         propagation_limit: PropagationLimit
         propagation_phase: PropagationPhase
         widget: Widget
     props: Props = ...
     def __init__(
         self,
+        stylus_only: bool = ...,
         button: int = ...,
         exclusive: bool = ...,
         touch_only: bool = ...,
         n_points: int = ...,
         name: str = ...,
         propagation_limit: PropagationLimit = ...,
         propagation_phase: PropagationPhase = ...,
     ): ...
     def get_axes(self, axes: Sequence[Gdk.AxisUse]) -> Tuple[bool, list[float]]: ...
     def get_axis(self, axis: Gdk.AxisUse) -> Tuple[bool, float]: ...
     def get_backlog(self) -> Tuple[bool, list[Gdk.TimeCoord]]: ...
     def get_device_tool(self) -> Optional[Gdk.DeviceTool]: ...
+    def get_stylus_only(self) -> bool: ...
     @classmethod
     def new(cls) -> GestureStylus: ...
+    def set_stylus_only(self, stylus_only: bool) -> None: ...
 
 class GestureStylusClass(GObject.GPointer): ...
 
 class GestureSwipe(GestureSingle):
     class Props:
         button: int
         exclusive: bool
@@ -8282,14 +8839,15 @@
         input_purpose: InputPurpose
     props: Props = ...
     parent_instance: GObject.Object = ...
     def __init__(
         self, input_hints: InputHints = ..., input_purpose: InputPurpose = ...
     ): ...
     def delete_surrounding(self, offset: int, n_chars: int) -> bool: ...
+    def do_activate_osk(self) -> None: ...
     def do_commit(self, str: str) -> None: ...
     def do_delete_surrounding(self, offset: int, n_chars: int) -> bool: ...
     def do_filter_keypress(self, event: Gdk.Event) -> bool: ...
     def do_focus_in(self) -> None: ...
     def do_focus_out(self) -> None: ...
     def do_get_preedit_string(self) -> Tuple[str, Pango.AttrList, int]: ...
     def do_get_surrounding(self) -> Tuple[bool, str, int]: ...
@@ -8353,19 +8911,19 @@
     get_surrounding: Callable[[IMContext], Tuple[bool, str, int]] = ...
     set_surrounding_with_selection: Callable[
         [IMContext, str, int, int, int], None
     ] = ...
     get_surrounding_with_selection: Callable[
         [IMContext], Tuple[bool, str, int, int]
     ] = ...
+    activate_osk: Callable[[IMContext], None] = ...
     _gtk_reserved1: None = ...
     _gtk_reserved2: None = ...
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
-    _gtk_reserved5: None = ...
 
 class IMContextSimple(IMContext):
     class Props:
         input_hints: InputHints
         input_purpose: InputPurpose
     props: Props = ...
     object: IMContext = ...
@@ -9234,15 +9792,17 @@
     allocate: Callable[[LayoutManager, Widget, int, int, int], None] = ...
     layout_child_type: Type = ...
     create_layout_child: Callable[[LayoutManager, Widget, Widget], LayoutChild] = ...
     root: Callable[[LayoutManager], None] = ...
     unroot: Callable[[LayoutManager], None] = ...
     _padding: list[None] = ...
 
-class LevelBar(Widget, Accessible, Buildable, ConstraintTarget, Orientable):
+class LevelBar(
+    Widget, Accessible, AccessibleRange, Buildable, ConstraintTarget, Orientable
+):
     class Props:
         inverted: bool
         max_value: float
         min_value: float
         mode: LevelBarMode
         value: float
         can_focus: bool
@@ -10268,14 +10828,15 @@
     _gtk_reserved5: None = ...
     _gtk_reserved6: None = ...
     _gtk_reserved7: None = ...
     _gtk_reserved8: None = ...
 
 class MenuButton(Widget, Accessible, Buildable, ConstraintTarget):
     class Props:
+        active: bool
         always_show_arrow: bool
         child: Optional[Widget]
         direction: ArrowType
         has_frame: bool
         icon_name: Optional[str]
         label: Optional[str]
         menu_model: Optional[Gio.MenuModel]
@@ -10316,14 +10877,15 @@
         vexpand_set: bool
         visible: bool
         width_request: int
         accessible_role: AccessibleRole
     props: Props = ...
     def __init__(
         self,
+        active: bool = ...,
         always_show_arrow: bool = ...,
         child: Widget = ...,
         direction: ArrowType = ...,
         has_frame: bool = ...,
         icon_name: str = ...,
         label: str = ...,
         menu_model: Gio.MenuModel = ...,
@@ -10357,28 +10919,30 @@
         valign: Align = ...,
         vexpand: bool = ...,
         vexpand_set: bool = ...,
         visible: bool = ...,
         width_request: int = ...,
         accessible_role: AccessibleRole = ...,
     ): ...
+    def get_active(self) -> bool: ...
     def get_always_show_arrow(self) -> bool: ...
     def get_child(self) -> Optional[Widget]: ...
     def get_direction(self) -> ArrowType: ...
     def get_has_frame(self) -> bool: ...
     def get_icon_name(self) -> Optional[str]: ...
     def get_label(self) -> Optional[str]: ...
     def get_menu_model(self) -> Optional[Gio.MenuModel]: ...
     def get_popover(self) -> Optional[Popover]: ...
     def get_primary(self) -> bool: ...
     def get_use_underline(self) -> bool: ...
     @classmethod
     def new(cls) -> MenuButton: ...
     def popdown(self) -> None: ...
     def popup(self) -> None: ...
+    def set_active(self, active: bool) -> None: ...
     def set_always_show_arrow(self, always_show_arrow: bool) -> None: ...
     def set_child(self, child: Optional[Widget] = None) -> None: ...
     def set_create_popup_func(
         self, func: Optional[Callable[..., None]] = None, *user_data: Any
     ) -> None: ...
     def set_direction(self, direction: ArrowType) -> None: ...
     def set_has_frame(self, has_frame: bool) -> None: ...
@@ -11254,15 +11818,17 @@
         cls, title: Optional[str] = None, parent: Optional[Window] = None
     ) -> PageSetupUnixDialog: ...
     def set_page_setup(self, page_setup: PageSetup) -> None: ...
     def set_print_settings(
         self, print_settings: Optional[PrintSettings] = None
     ) -> None: ...
 
-class Paned(Widget, Accessible, Buildable, ConstraintTarget, Orientable):
+class Paned(
+    Widget, Accessible, AccessibleRange, Buildable, ConstraintTarget, Orientable
+):
     class Props:
         end_child: Optional[Widget]
         max_position: int
         min_position: int
         position: int
         position_set: bool
         resize_end_child: bool
@@ -12453,15 +13019,17 @@
     def is_paused(self) -> bool: ...
     def is_virtual(self) -> bool: ...
     def list_papers(self) -> list[PageSetup]: ...
     @classmethod
     def new(cls, name: str, backend: PrintBackend, virtual_: bool) -> Printer: ...
     def request_details(self) -> None: ...
 
-class ProgressBar(Widget, Accessible, Buildable, ConstraintTarget, Orientable):
+class ProgressBar(
+    Widget, Accessible, AccessibleRange, Buildable, ConstraintTarget, Orientable
+):
     class Props:
         ellipsize: Pango.EllipsizeMode
         fraction: float
         inverted: bool
         pulse_step: float
         show_text: bool
         text: Optional[str]
@@ -12572,15 +13140,17 @@
 
 class PyGTKDeprecationWarning:
     args = ...  # FIXME Constant
 
     def add_note(self, *args, **kwargs): ...  # FIXME Function
     def with_traceback(self, *args, **kwargs): ...  # FIXME Function
 
-class Range(Widget, Accessible, Buildable, ConstraintTarget, Orientable):
+class Range(
+    Widget, Accessible, AccessibleRange, Buildable, ConstraintTarget, Orientable
+):
     class Props:
         adjustment: Adjustment
         fill_level: float
         inverted: bool
         restrict_to_fill_level: bool
         round_digits: int
         show_fill_level: bool
@@ -12878,15 +13448,17 @@
 class Root(GObject.GInterface):
     def get_display(self) -> Gdk.Display: ...
     def get_focus(self) -> Optional[Widget]: ...
     def set_focus(self, focus: Optional[Widget] = None) -> None: ...
 
 class RootInterface(GObject.GPointer): ...
 
-class Scale(Range, Accessible, Buildable, ConstraintTarget, Orientable):
+class Scale(
+    Range, Accessible, AccessibleRange, Buildable, ConstraintTarget, Orientable
+):
     class Props:
         digits: int
         draw_value: bool
         has_origin: bool
         value_pos: PositionType
         adjustment: Adjustment
         fill_level: float
@@ -12999,16 +13571,19 @@
     def set_draw_value(self, draw_value: bool) -> None: ...
     def set_format_value_func(
         self, func: Optional[Callable[..., str]] = None, *user_data: Any
     ) -> None: ...
     def set_has_origin(self, has_origin: bool) -> None: ...
     def set_value_pos(self, pos: PositionType) -> None: ...
 
-class ScaleButton(Widget, Accessible, Buildable, ConstraintTarget, Orientable):
+class ScaleButton(
+    Widget, Accessible, AccessibleRange, Buildable, ConstraintTarget, Orientable
+):
     class Props:
+        active: bool
         adjustment: Adjustment
         icons: list[str]
         value: float
         can_focus: bool
         can_target: bool
         css_classes: list[str]
         css_name: str
@@ -13080,14 +13655,15 @@
         vexpand_set: bool = ...,
         visible: bool = ...,
         width_request: int = ...,
         accessible_role: AccessibleRole = ...,
         orientation: Orientation = ...,
     ): ...
     def do_value_changed(self, value: float) -> None: ...
+    def get_active(self) -> bool: ...
     def get_adjustment(self) -> Adjustment: ...
     def get_minus_button(self) -> Button: ...
     def get_plus_button(self) -> Button: ...
     def get_popup(self) -> Widget: ...
     def get_value(self) -> float: ...
     @classmethod
     def new(
@@ -13431,15 +14007,15 @@
     def set_key_capture_widget(self, widget: Optional[Widget] = None) -> None: ...
     def set_search_mode(self, search_mode: bool) -> None: ...
     def set_show_close_button(self, visible: bool) -> None: ...
 
 class SearchEntry(Widget, Accessible, Buildable, ConstraintTarget, Editable):
     class Props:
         activates_default: bool
-        placeholder_text: str
+        placeholder_text: Optional[str]
         search_delay: int
         can_focus: bool
         can_target: bool
         css_classes: list[str]
         css_name: str
         cursor: Optional[Gdk.Cursor]
         focus_on_click: bool
@@ -13520,18 +14096,20 @@
         enable_undo: bool = ...,
         max_width_chars: int = ...,
         text: str = ...,
         width_chars: int = ...,
         xalign: float = ...,
     ): ...
     def get_key_capture_widget(self) -> Optional[Widget]: ...
+    def get_placeholder_text(self) -> Optional[str]: ...
     def get_search_delay(self) -> int: ...
     @classmethod
     def new(cls) -> SearchEntry: ...
     def set_key_capture_widget(self, widget: Optional[Widget] = None) -> None: ...
+    def set_placeholder_text(self, text: Optional[str] = None) -> None: ...
     def set_search_delay(self, delay: int) -> None: ...
 
 class SelectionFilterModel(GObject.Object, Gio.ListModel):
     class Props:
         item_type: Type
         model: Optional[SelectionModel]
         n_items: int
@@ -14496,14 +15074,17 @@
         center: Graphene.Point,
         hradius: float,
         vradius: float,
         start: float,
         end: float,
         stops: Sequence[Gsk.ColorStop],
     ) -> None: ...
+    def append_scaled_texture(
+        self, texture: Gdk.Texture, filter: Gsk.ScalingFilter, bounds: Graphene.Rect
+    ) -> None: ...
     def append_texture(self, texture: Gdk.Texture, bounds: Graphene.Rect) -> None: ...
     def gl_shader_pop_texture(self) -> None: ...
     @classmethod
     def new(cls) -> Snapshot: ...
     def perspective(self, depth: float) -> None: ...
     def pop(self) -> None: ...
     def push_blend(self, blend_mode: Gsk.BlendMode) -> None: ...
@@ -14512,14 +15093,15 @@
     def push_color_matrix(
         self, color_matrix: Graphene.Matrix, color_offset: Graphene.Vec4
     ) -> None: ...
     def push_cross_fade(self, progress: float) -> None: ...
     def push_gl_shader(
         self, shader: Gsk.GLShader, bounds: Graphene.Rect, take_args: GLib.Bytes
     ) -> None: ...
+    def push_mask(self, mask_mode: Gsk.MaskMode) -> None: ...
     def push_opacity(self, opacity: float) -> None: ...
     def push_repeat(
         self, bounds: Graphene.Rect, child_bounds: Optional[Graphene.Rect] = None
     ) -> None: ...
     def push_rounded_clip(self, bounds: Gsk.RoundedRect) -> None: ...
     def push_shadow(self, shadow: Sequence[Gsk.Shadow]) -> None: ...
     def render_background(
@@ -14611,15 +15193,22 @@
     _gtk_reserved4: None = ...
     _gtk_reserved5: None = ...
     _gtk_reserved6: None = ...
     _gtk_reserved7: None = ...
     _gtk_reserved8: None = ...
 
 class SpinButton(
-    Widget, Accessible, Buildable, CellEditable, ConstraintTarget, Editable, Orientable
+    Widget,
+    Accessible,
+    AccessibleRange,
+    Buildable,
+    CellEditable,
+    ConstraintTarget,
+    Editable,
+    Orientable,
 ):
     class Props:
         adjustment: Adjustment
         climb_rate: float
         digits: int
         numeric: bool
         snap_to_ticks: bool
@@ -15249,14 +15838,18 @@
     def set_match_mode(self, mode: StringFilterMatchMode) -> None: ...
     def set_search(self, search: Optional[str] = None) -> None: ...
 
 class StringFilterClass(GObject.GPointer):
     parent_class: FilterClass = ...
 
 class StringList(GObject.Object, Gio.ListModel, Buildable):
+    class Props:
+        strings: list[str]
+    props: Props = ...
+    def __init__(self, strings: Sequence[str] = ...): ...
     def append(self, string: str) -> None: ...
     def get_string(self, position: int) -> Optional[str]: ...
     @classmethod
     def new(cls, strings: Optional[Sequence[str]] = None) -> StringList: ...
     def remove(self, position: int) -> None: ...
     def splice(
         self, position: int, n_removals: int, additions: Optional[Sequence[str]] = None
@@ -15275,22 +15868,30 @@
     def new(cls, string: str) -> StringObject: ...
 
 class StringObjectClass(GObject.GPointer):
     parent_class: GObject.ObjectClass = ...
 
 class StringSorter(Sorter):
     class Props:
+        collation: Collation
         expression: Optional[Expression]
         ignore_case: bool
     props: Props = ...
-    def __init__(self, expression: Expression = ..., ignore_case: bool = ...): ...
+    def __init__(
+        self,
+        collation: Collation = ...,
+        expression: Expression = ...,
+        ignore_case: bool = ...,
+    ): ...
+    def get_collation(self) -> Collation: ...
     def get_expression(self) -> Optional[Expression]: ...
     def get_ignore_case(self) -> bool: ...
     @classmethod
     def new(cls, expression: Optional[Expression] = None) -> StringSorter: ...
+    def set_collation(self, collation: Collation) -> None: ...
     def set_expression(self, expression: Optional[Expression] = None) -> None: ...
     def set_ignore_case(self, ignore_case: bool) -> None: ...
 
 class StringSorterClass(GObject.GPointer):
     parent_class: SorterClass = ...
 
 class StyleContext(GObject.Object):
@@ -16547,14 +17148,16 @@
         [TreeDragSource, TreePath], Optional[Gdk.ContentProvider]
     ] = ...
     drag_data_delete: Callable[[TreeDragSource, TreePath], bool] = ...
 
 class TreeExpander(Widget, Accessible, Buildable, ConstraintTarget):
     class Props:
         child: Optional[Widget]
+        hide_expander: bool
+        indent_for_depth: bool
         indent_for_icon: bool
         item: Optional[GObject.Object]
         list_row: Optional[TreeListRow]
         can_focus: bool
         can_target: bool
         css_classes: list[str]
         css_name: str
@@ -16589,14 +17192,16 @@
         visible: bool
         width_request: int
         accessible_role: AccessibleRole
     props: Props = ...
     def __init__(
         self,
         child: Widget = ...,
+        hide_expander: bool = ...,
+        indent_for_depth: bool = ...,
         indent_for_icon: bool = ...,
         list_row: TreeListRow = ...,
         can_focus: bool = ...,
         can_target: bool = ...,
         css_classes: Sequence[str] = ...,
         css_name: str = ...,
         cursor: Gdk.Cursor = ...,
@@ -16623,20 +17228,24 @@
         vexpand: bool = ...,
         vexpand_set: bool = ...,
         visible: bool = ...,
         width_request: int = ...,
         accessible_role: AccessibleRole = ...,
     ): ...
     def get_child(self) -> Optional[Widget]: ...
+    def get_hide_expander(self) -> bool: ...
+    def get_indent_for_depth(self) -> bool: ...
     def get_indent_for_icon(self) -> bool: ...
     def get_item(self) -> Optional[GObject.Object]: ...
     def get_list_row(self) -> Optional[TreeListRow]: ...
     @classmethod
     def new(cls) -> TreeExpander: ...
     def set_child(self, child: Optional[Widget] = None) -> None: ...
+    def set_hide_expander(self, hide_expander: bool) -> None: ...
+    def set_indent_for_depth(self, indent_for_depth: bool) -> None: ...
     def set_indent_for_icon(self, indent_for_icon: bool) -> None: ...
     def set_list_row(self, list_row: Optional[TreeListRow] = None) -> None: ...
 
 class TreeExpanderClass(GObject.GPointer):
     parent_class: WidgetClass = ...
 
 class TreeIter(GObject.GBoxed):
@@ -17408,14 +18017,37 @@
     def set_sort_indicator(self, setting: bool) -> None: ...
     def set_sort_order(self, order: SortType) -> None: ...
     def set_spacing(self, spacing: int) -> None: ...
     def set_title(self, title: str) -> None: ...
     def set_visible(self, visible: bool) -> None: ...
     def set_widget(self, widget: Optional[Widget] = None) -> None: ...
 
+class UriLauncher(GObject.Object):
+    class Props:
+        uri: Optional[str]
+    props: Props = ...
+    def __init__(self, uri: str = ...): ...
+    def get_uri(self) -> Optional[str]: ...
+    def launch(
+        self,
+        parent: Optional[Window] = None,
+        cancellable: Optional[Gio.Cancellable] = None,
+        callback: Optional[
+            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
+        ] = None,
+        *user_data: Any,
+    ) -> None: ...
+    def launch_finish(self, result: Gio.AsyncResult) -> bool: ...
+    @classmethod
+    def new(cls, uri: Optional[str] = None) -> UriLauncher: ...
+    def set_uri(self, uri: Optional[str] = None) -> None: ...
+
+class UriLauncherClass(GObject.GPointer):
+    parent_class: GObject.ObjectClass = ...
+
 class Video(Widget, Accessible, Buildable, ConstraintTarget):
     class Props:
         autoplay: bool
         file: Optional[Gio.File]
         loop: bool
         media_stream: Optional[MediaStream]
         can_focus: bool
@@ -17605,17 +18237,20 @@
         cls,
         hadjustment: Optional[Adjustment] = None,
         vadjustment: Optional[Adjustment] = None,
     ) -> Viewport: ...
     def set_child(self, child: Optional[Widget] = None) -> None: ...
     def set_scroll_to_focus(self, scroll_to_focus: bool) -> None: ...
 
-class VolumeButton(ScaleButton, Accessible, Buildable, ConstraintTarget, Orientable):
+class VolumeButton(
+    ScaleButton, Accessible, AccessibleRange, Buildable, ConstraintTarget, Orientable
+):
     class Props:
         use_symbolic: bool
+        active: bool
         adjustment: Adjustment
         icons: list[str]
         value: float
         can_focus: bool
         can_target: bool
         css_classes: list[str]
         css_name: str
@@ -17843,14 +18478,15 @@
     def get_allocated_width(self) -> int: ...
     def get_allocation(self) -> Gdk.Rectangle: ...
     def get_ancestor(self, widget_type: Type) -> Optional[Widget]: ...
     def get_can_focus(self) -> bool: ...
     def get_can_target(self) -> bool: ...
     def get_child_visible(self) -> bool: ...
     def get_clipboard(self) -> Gdk.Clipboard: ...
+    def get_color(self) -> Gdk.RGBA: ...
     def get_css_classes(self) -> list[str]: ...
     def get_css_name(self) -> str: ...
     def get_cursor(self) -> Optional[Gdk.Cursor]: ...
     @staticmethod
     def get_default_direction() -> TextDirection: ...
     def get_direction(self) -> TextDirection: ...
     def get_display(self) -> Gdk.Display: ...
@@ -17920,15 +18556,15 @@
     def insert_before(
         self, parent: Widget, next_sibling: Optional[Widget] = None
     ) -> None: ...
     def install_action(
         self,
         action_name: str,
         parameter_type: Optional[str],
-        activate: Callable[[Widget, str, GLib.Variant], None],
+        activate: Callable[[Widget, str, Optional[GLib.Variant]], None],
     ) -> None: ...
     def install_property_action(self, action_name: str, property_name: str) -> None: ...
     def is_ancestor(self, ancestor: Widget) -> bool: ...
     def is_drawable(self) -> bool: ...
     def is_focus(self) -> bool: ...
     def is_sensitive(self) -> bool: ...
     def is_visible(self) -> bool: ...
@@ -18053,15 +18689,15 @@
     def get_activate_signal(self) -> int: ...
     def get_css_name(self) -> str: ...
     def get_layout_manager_type(self) -> Type: ...
     def install_action(
         self,
         action_name: str,
         parameter_type: Optional[str],
-        activate: Callable[[Widget, str, GLib.Variant], None],
+        activate: Callable[[Widget, str, Optional[GLib.Variant]], None],
     ) -> None: ...
     def install_property_action(self, action_name: str, property_name: str) -> None: ...
     def query_action(
         self, index_: int
     ) -> Tuple[bool, Type, str, GLib.VariantType, str]: ...
     def set_accessible_role(self, accessible_role: AccessibleRole) -> None: ...
     def set_activate_signal(self, signal_id: int) -> None: ...
@@ -18623,14 +19259,19 @@
 
 class AccessibleInvalidState(GObject.GEnum):
     FALSE = 0
     GRAMMAR = 2
     SPELLING = 3
     TRUE = 1
 
+class AccessiblePlatformState(GObject.GEnum):
+    ACTIVE = 2
+    FOCUSABLE = 0
+    FOCUSED = 1
+
 class AccessibleProperty(GObject.GEnum):
     AUTOCOMPLETE = 0
     DESCRIPTION = 1
     HAS_POPUP = 2
     KEY_SHORTCUTS = 3
     LABEL = 4
     LEVEL = 5
@@ -18740,14 +19381,15 @@
     TAB = 64
     TABLE = 65
     TAB_LIST = 66
     TAB_PANEL = 67
     TEXT_BOX = 68
     TIME = 69
     TIMER = 70
+    TOGGLE_BUTTON = 78
     TOOLBAR = 71
     TOOLTIP = 72
     TREE = 73
     TREE_GRID = 74
     TREE_ITEM = 75
     WIDGET = 76
     WINDOW = 77
@@ -18846,14 +19488,19 @@
     OTHER = 1
 
 class CellRendererMode(GObject.GEnum):
     ACTIVATABLE = 1
     EDITABLE = 2
     INERT = 0
 
+class Collation(GObject.GEnum):
+    FILENAME = 2
+    NONE = 0
+    UNICODE = 1
+
 class ConstraintAttribute(GObject.GEnum):
     BASELINE = 11
     BOTTOM = 4
     CENTER_X = 9
     CENTER_Y = 10
     END = 6
     HEIGHT = 8
@@ -18915,14 +19562,21 @@
     DISPLAY_LINE_ENDS = 4
     PARAGRAPHS = 6
     PARAGRAPH_ENDS = 5
     WHITESPACE = 7
     WORDS = 2
     WORD_ENDS = 1
 
+class DialogError(GObject.GEnum):
+    CANCELLED = 1
+    DISMISSED = 2
+    FAILED = 0
+    @staticmethod
+    def quark() -> int: ...
+
 class DirectionType(GObject.GEnum):
     DOWN = 3
     LEFT = 4
     RIGHT = 5
     TAB_BACKWARD = 1
     TAB_FORWARD = 0
     UP = 2
@@ -18966,14 +19620,20 @@
     MORE_STRICT = 2
 
 class FilterMatch(GObject.GEnum):
     ALL = 2
     NONE = 1
     SOME = 0
 
+class FontLevel(GObject.GEnum):
+    FACE = 1
+    FAMILY = 0
+    FEATURES = 3
+    FONT = 2
+
 class IconSize(GObject.GEnum):
     INHERIT = 0
     LARGE = 2
     NORMAL = 1
 
 class IconThemeError(GObject.GEnum):
     FAILED = 1
```

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/_GtkSource4.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/_GtkSource4.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/_GtkSource5.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/_GtkSource5.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/_Soup2.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Soup2.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.6.0/src/gi-stubs/repository/_Soup3.pyi` & `PyGObject-stubs-2.7.0/src/gi-stubs/repository/_Soup3.pyi`

 * *Files identical despite different names*

