# Comparing `tmp/PyNOT-redux-1.3.tar.gz` & `tmp/PyNOT-redux-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNOT-redux-1.3.tar", last modified: Tue Apr 25 14:38:29 2023, max compression
+gzip compressed data, was "PyNOT-redux-1.3.1.tar", last modified: Tue May  9 07:53:04 2023, max compression
```

## Comparing `PyNOT-redux-1.3.tar` & `PyNOT-redux-1.3.1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 14:38:29.634014 PyNOT-redux-1.3/
--rw-r--r--   0 krogager   (501) staff       (20)     8196 2023-04-24 12:09:15.000000 PyNOT-redux-1.3/.DS_Store
--rw-r--r--   0 krogager   (501) staff       (20)       66 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/.gitattributes
--rw-r--r--   0 krogager   (501) staff       (20)     1878 2022-05-09 07:03:03.000000 PyNOT-redux-1.3/.gitignore
--rw-r--r--   0 krogager   (501) staff       (20)     1079 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/LICENSE
--rw-r--r--   0 krogager   (501) staff       (20)      202 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/MANIFEST.in
--rw-r--r--   0 krogager   (501) staff       (20)    13888 2023-04-25 14:38:29.633835 PyNOT-redux-1.3/PKG-INFO
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 14:38:29.617897 PyNOT-redux-1.3/PyNOT_redux.egg-info/
--rw-r--r--   0 krogager   (501) staff       (20)    13888 2023-04-25 14:38:29.000000 PyNOT-redux-1.3/PyNOT_redux.egg-info/PKG-INFO
--rw-r--r--   0 krogager   (501) staff       (20)     2169 2023-04-25 14:38:29.000000 PyNOT-redux-1.3/PyNOT_redux.egg-info/SOURCES.txt
--rw-r--r--   0 krogager   (501) staff       (20)        1 2023-04-25 14:38:29.000000 PyNOT-redux-1.3/PyNOT_redux.egg-info/dependency_links.txt
--rw-r--r--   0 krogager   (501) staff       (20)       42 2023-04-25 14:38:29.000000 PyNOT-redux-1.3/PyNOT_redux.egg-info/entry_points.txt
--rw-r--r--   0 krogager   (501) staff       (20)      113 2023-04-25 14:38:29.000000 PyNOT-redux-1.3/PyNOT_redux.egg-info/requires.txt
--rw-r--r--   0 krogager   (501) staff       (20)        6 2023-04-25 14:38:29.000000 PyNOT-redux-1.3/PyNOT_redux.egg-info/top_level.txt
--rw-r--r--   0 krogager   (501) staff       (20)    13260 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/README.md
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 14:38:29.625752 PyNOT-redux-1.3/pynot/
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/.extract_msg
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/.identify_msg
--rw-r--r--   0 krogager   (501) staff       (20)       86 2023-02-25 17:32:13.000000 PyNOT-redux-1.3/pynot/.instrument.cfg
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/.response_msg
--rw-r--r--   0 krogager   (501) staff       (20)        4 2023-04-25 14:38:05.000000 PyNOT-redux-1.3/pynot/VERSION
--rw-r--r--   0 krogager   (501) staff       (20)     1110 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)     6867 2022-06-01 17:21:45.000000 PyNOT-redux-1.3/pynot/alfosc.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 14:38:29.629320 PyNOT-redux-1.3/pynot/calib/
--rw-r--r--   0 krogager   (501) staff       (20)      701 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/HeAr_linelist.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1073 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/HeNe_linelist.dat
--rw-r--r--   0 krogager   (501) staff       (20)      828 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/ThAr_linelist.dat
--rw-r--r--   0 krogager   (501) staff       (20)      340 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/al-gr18_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      228 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/al-gr19_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      318 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/al-gr4_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      186 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/al-gr7_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)    19712 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/alfosc_filters.dat
--rw-r--r--   0 krogager   (501) staff       (20)     6013 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/default_options.yml
--rw-r--r--   0 krogager   (501) staff       (20)     3751 2023-04-25 06:53:15.000000 PyNOT-redux-1.3/pynot/calib/default_options_img.yml
--rw-r--r--   0 krogager   (501) staff       (20)      343 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/ef-gr13_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      322 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/ef-gr14_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      300 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/ef-gr1_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      279 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/ef-gr3_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      709 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/efosc_filters.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1638 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/lapalma.ext
--rw-r--r--   0 krogager   (501) staff       (20)      519 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/lasilla.ext
--rw-r--r--   0 krogager   (501) staff       (20)     1425 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/paranal.ext
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 14:38:29.632424 PyNOT-redux-1.3/pynot/calib/std/
--rw-r--r--   0 krogager   (501) staff       (20)     1454 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/bd174708.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1393 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/bd262606.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1254 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/bd332642.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1083 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/bd75325.dat
--rw-r--r--   0 krogager   (501) staff       (20)     4228 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/eg21.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1251 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/feige110.dat
--rw-r--r--   0 krogager   (501) staff       (20)     2738 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/feige34.dat
--rw-r--r--   0 krogager   (501) staff       (20)     8611 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/gd153.dat
--rw-r--r--   0 krogager   (501) staff       (20)   129806 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/gd50.dat
--rw-r--r--   0 krogager   (501) staff       (20)     8631 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/gd71.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1373 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/hd19445.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1376 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/hd84937.dat
--rw-r--r--   0 krogager   (501) staff       (20)     2609 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/hd93521.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1557 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/he3.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1255 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/hiltner600.dat
--rw-r--r--   0 krogager   (501) staff       (20)     4247 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/ltt3864.dat
--rw-r--r--   0 krogager   (501) staff       (20)      368 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/tcs_namelist.txt
--rw-r--r--   0 krogager   (501) staff       (20)     1807 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/wolf1346.dat
--rw-r--r--   0 krogager   (501) staff       (20)    26026 2022-04-22 11:31:36.000000 PyNOT-redux-1.3/pynot/calibs.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 14:38:29.633157 PyNOT-redux-1.3/pynot/data/
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/data/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)     1744 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/data/alfosc.rules
--rw-r--r--   0 krogager   (501) staff       (20)     1348 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/data/efosc.rules
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 14:38:29.633623 PyNOT-redux-1.3/pynot/data/help/
--rw-r--r--   0 krogager   (501) staff       (20)     7423 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/data/help/welcome_msg_extract.html
--rw-r--r--   0 krogager   (501) staff       (20)     3876 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/data/help/welcome_msg_identify.html
--rw-r--r--   0 krogager   (501) staff       (20)     1594 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/data/help/welcome_msg_response.html
--rw-r--r--   0 krogager   (501) staff       (20)     3471 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/data/io.py
--rw-r--r--   0 krogager   (501) staff       (20)     4699 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/data/obs.py
--rw-r--r--   0 krogager   (501) staff       (20)    26160 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/data/organizer.py
--rw-r--r--   0 krogager   (501) staff       (20)     7812 2022-06-01 17:24:49.000000 PyNOT-redux-1.3/pynot/efosc.py
--rw-r--r--   0 krogager   (501) staff       (20)   114866 2022-06-13 08:59:11.000000 PyNOT-redux-1.3/pynot/extract_gui.py
--rw-r--r--   0 krogager   (501) staff       (20)    23413 2022-05-05 20:36:46.000000 PyNOT-redux-1.3/pynot/extraction.py
--rw-r--r--   0 krogager   (501) staff       (20)    19746 2023-04-25 06:53:15.000000 PyNOT-redux-1.3/pynot/fitsio.py
--rw-r--r--   0 krogager   (501) staff       (20)     8829 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/functions.py
--rw-r--r--   0 krogager   (501) staff       (20)    50862 2022-06-01 17:19:24.000000 PyNOT-redux-1.3/pynot/identify_gui.py
--rw-r--r--   0 krogager   (501) staff       (20)    12773 2022-11-17 14:10:06.000000 PyNOT-redux-1.3/pynot/insconfig.py
--rw-r--r--   0 krogager   (501) staff       (20)     2614 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/logging.py
--rw-r--r--   0 krogager   (501) staff       (20)    47613 2023-04-25 06:53:15.000000 PyNOT-redux-1.3/pynot/main.py
--rw-r--r--   0 krogager   (501) staff       (20)    30199 2023-04-24 16:45:04.000000 PyNOT-redux-1.3/pynot/phot.py
--rw-r--r--   0 krogager   (501) staff       (20)    14938 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/phot_redux.py
--rw-r--r--   0 krogager   (501) staff       (20)    28868 2022-04-20 11:44:59.000000 PyNOT-redux-1.3/pynot/redux.py
--rw-r--r--   0 krogager   (501) staff       (20)     5048 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/reports.py
--rw-r--r--   0 krogager   (501) staff       (20)    37586 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/response.py
--rw-r--r--   0 krogager   (501) staff       (20)    26610 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/response_gui.py
--rw-r--r--   0 krogager   (501) staff       (20)    20722 2022-05-03 16:23:47.000000 PyNOT-redux-1.3/pynot/scired.py
--rw-r--r--   0 krogager   (501) staff       (20)    18099 2022-05-06 15:28:38.000000 PyNOT-redux-1.3/pynot/scombine.py
--rw-r--r--   0 krogager   (501) staff       (20)     2337 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/tasks.py
--rw-r--r--   0 krogager   (501) staff       (20)     9913 2023-04-25 14:38:05.000000 PyNOT-redux-1.3/pynot/transients.py
--rw-r--r--   0 krogager   (501) staff       (20)     3391 2022-05-06 15:28:38.000000 PyNOT-redux-1.3/pynot/txtio.py
--rw-r--r--   0 krogager   (501) staff       (20)    28434 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/wavecal.py
--rw-r--r--   0 krogager   (501) staff       (20)    13375 2023-04-25 06:53:15.000000 PyNOT-redux-1.3/pynot/wcs.py
--rw-r--r--   0 krogager   (501) staff       (20)     2384 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/welcome.py
--rw-r--r--   0 krogager   (501) staff       (20)      104 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pyproject.toml
--rw-r--r--   0 krogager   (501) staff       (20)       38 2023-04-25 14:38:29.634047 PyNOT-redux-1.3/setup.cfg
--rw-r--r--   0 krogager   (501) staff       (20)     5210 2023-02-25 17:18:36.000000 PyNOT-redux-1.3/setup.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-09 07:53:04.928146 PyNOT-redux-1.3.1/
+-rw-r--r--   0 krogager   (501) staff       (20)     8196 2023-05-07 20:58:18.000000 PyNOT-redux-1.3.1/.DS_Store
+-rw-r--r--   0 krogager   (501) staff       (20)       66 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/.gitattributes
+-rw-r--r--   0 krogager   (501) staff       (20)     1898 2023-05-09 07:51:28.000000 PyNOT-redux-1.3.1/.gitignore
+-rw-r--r--   0 krogager   (501) staff       (20)     1079 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/LICENSE
+-rw-r--r--   0 krogager   (501) staff       (20)      202 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/MANIFEST.in
+-rw-r--r--   0 krogager   (501) staff       (20)    13890 2023-05-09 07:53:04.927996 PyNOT-redux-1.3.1/PKG-INFO
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-09 07:53:04.913170 PyNOT-redux-1.3.1/PyNOT_redux.egg-info/
+-rw-r--r--   0 krogager   (501) staff       (20)    13890 2023-05-09 07:53:04.000000 PyNOT-redux-1.3.1/PyNOT_redux.egg-info/PKG-INFO
+-rw-r--r--   0 krogager   (501) staff       (20)     2169 2023-05-09 07:53:04.000000 PyNOT-redux-1.3.1/PyNOT_redux.egg-info/SOURCES.txt
+-rw-r--r--   0 krogager   (501) staff       (20)        1 2023-05-09 07:53:04.000000 PyNOT-redux-1.3.1/PyNOT_redux.egg-info/dependency_links.txt
+-rw-r--r--   0 krogager   (501) staff       (20)       42 2023-05-09 07:53:04.000000 PyNOT-redux-1.3.1/PyNOT_redux.egg-info/entry_points.txt
+-rw-r--r--   0 krogager   (501) staff       (20)      113 2023-05-09 07:53:04.000000 PyNOT-redux-1.3.1/PyNOT_redux.egg-info/requires.txt
+-rw-r--r--   0 krogager   (501) staff       (20)        6 2023-05-09 07:53:04.000000 PyNOT-redux-1.3.1/PyNOT_redux.egg-info/top_level.txt
+-rw-r--r--   0 krogager   (501) staff       (20)    13260 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/README.md
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-09 07:53:04.921216 PyNOT-redux-1.3.1/pynot/
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/.extract_msg
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/.identify_msg
+-rw-r--r--   0 krogager   (501) staff       (20)       86 2023-02-25 17:32:13.000000 PyNOT-redux-1.3.1/pynot/.instrument.cfg
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/.response_msg
+-rw-r--r--   0 krogager   (501) staff       (20)        6 2023-05-09 07:51:38.000000 PyNOT-redux-1.3.1/pynot/VERSION
+-rw-r--r--   0 krogager   (501) staff       (20)     1110 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)     6867 2022-06-01 17:21:45.000000 PyNOT-redux-1.3.1/pynot/alfosc.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-09 07:53:04.923966 PyNOT-redux-1.3.1/pynot/calib/
+-rw-r--r--   0 krogager   (501) staff       (20)      701 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/HeAr_linelist.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1073 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/HeNe_linelist.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      828 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/ThAr_linelist.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      340 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/al-gr18_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      228 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/al-gr19_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      318 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/al-gr4_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      186 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/al-gr7_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)    19712 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/alfosc_filters.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     6013 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/default_options.yml
+-rw-r--r--   0 krogager   (501) staff       (20)     3751 2023-04-25 06:53:15.000000 PyNOT-redux-1.3.1/pynot/calib/default_options_img.yml
+-rw-r--r--   0 krogager   (501) staff       (20)      343 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/ef-gr13_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      322 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/ef-gr14_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      300 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/ef-gr1_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      279 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/ef-gr3_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      709 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/efosc_filters.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1638 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/lapalma.ext
+-rw-r--r--   0 krogager   (501) staff       (20)      519 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/lasilla.ext
+-rw-r--r--   0 krogager   (501) staff       (20)     1425 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/paranal.ext
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-09 07:53:04.926647 PyNOT-redux-1.3.1/pynot/calib/std/
+-rw-r--r--   0 krogager   (501) staff       (20)     1454 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/bd174708.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1393 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/bd262606.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1254 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/bd332642.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1083 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/bd75325.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     4228 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/eg21.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1251 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/feige110.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     2738 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/feige34.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     8611 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/gd153.dat
+-rw-r--r--   0 krogager   (501) staff       (20)   129806 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/gd50.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     8631 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/gd71.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1373 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/hd19445.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1376 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/hd84937.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     2609 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/hd93521.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1557 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/he3.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1255 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/hiltner600.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     4247 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/ltt3864.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      368 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/tcs_namelist.txt
+-rw-r--r--   0 krogager   (501) staff       (20)     1807 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/wolf1346.dat
+-rw-r--r--   0 krogager   (501) staff       (20)    26026 2022-04-22 11:31:36.000000 PyNOT-redux-1.3.1/pynot/calibs.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-09 07:53:04.927325 PyNOT-redux-1.3.1/pynot/data/
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/data/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)     1744 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/data/alfosc.rules
+-rw-r--r--   0 krogager   (501) staff       (20)     1348 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/data/efosc.rules
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-09 07:53:04.927772 PyNOT-redux-1.3.1/pynot/data/help/
+-rw-r--r--   0 krogager   (501) staff       (20)     7423 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/data/help/welcome_msg_extract.html
+-rw-r--r--   0 krogager   (501) staff       (20)     3876 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/data/help/welcome_msg_identify.html
+-rw-r--r--   0 krogager   (501) staff       (20)     1594 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/data/help/welcome_msg_response.html
+-rw-r--r--   0 krogager   (501) staff       (20)     3471 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/data/io.py
+-rw-r--r--   0 krogager   (501) staff       (20)     4699 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/data/obs.py
+-rw-r--r--   0 krogager   (501) staff       (20)    26160 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/data/organizer.py
+-rw-r--r--   0 krogager   (501) staff       (20)     7812 2022-06-01 17:24:49.000000 PyNOT-redux-1.3.1/pynot/efosc.py
+-rw-r--r--   0 krogager   (501) staff       (20)   114866 2022-06-13 08:59:11.000000 PyNOT-redux-1.3.1/pynot/extract_gui.py
+-rw-r--r--   0 krogager   (501) staff       (20)    23413 2022-05-05 20:36:46.000000 PyNOT-redux-1.3.1/pynot/extraction.py
+-rw-r--r--   0 krogager   (501) staff       (20)    19746 2023-04-25 06:53:15.000000 PyNOT-redux-1.3.1/pynot/fitsio.py
+-rw-r--r--   0 krogager   (501) staff       (20)     8829 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/functions.py
+-rw-r--r--   0 krogager   (501) staff       (20)    50862 2022-06-01 17:19:24.000000 PyNOT-redux-1.3.1/pynot/identify_gui.py
+-rw-r--r--   0 krogager   (501) staff       (20)    12773 2022-11-17 14:10:06.000000 PyNOT-redux-1.3.1/pynot/insconfig.py
+-rw-r--r--   0 krogager   (501) staff       (20)     2614 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/logging.py
+-rw-r--r--   0 krogager   (501) staff       (20)    47613 2023-04-25 06:53:15.000000 PyNOT-redux-1.3.1/pynot/main.py
+-rw-r--r--   0 krogager   (501) staff       (20)    30199 2023-04-24 16:45:04.000000 PyNOT-redux-1.3.1/pynot/phot.py
+-rw-r--r--   0 krogager   (501) staff       (20)    14938 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/phot_redux.py
+-rw-r--r--   0 krogager   (501) staff       (20)    28868 2022-04-20 11:44:59.000000 PyNOT-redux-1.3.1/pynot/redux.py
+-rw-r--r--   0 krogager   (501) staff       (20)     5048 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/reports.py
+-rw-r--r--   0 krogager   (501) staff       (20)    37586 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/response.py
+-rw-r--r--   0 krogager   (501) staff       (20)    26610 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/response_gui.py
+-rw-r--r--   0 krogager   (501) staff       (20)    20722 2022-05-03 16:23:47.000000 PyNOT-redux-1.3.1/pynot/scired.py
+-rw-r--r--   0 krogager   (501) staff       (20)    18099 2022-05-06 15:28:38.000000 PyNOT-redux-1.3.1/pynot/scombine.py
+-rw-r--r--   0 krogager   (501) staff       (20)     2337 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/tasks.py
+-rw-r--r--   0 krogager   (501) staff       (20)     9913 2023-04-25 14:38:05.000000 PyNOT-redux-1.3.1/pynot/transients.py
+-rw-r--r--   0 krogager   (501) staff       (20)     3391 2022-05-06 15:28:38.000000 PyNOT-redux-1.3.1/pynot/txtio.py
+-rw-r--r--   0 krogager   (501) staff       (20)    28434 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/wavecal.py
+-rw-r--r--   0 krogager   (501) staff       (20)    13346 2023-05-09 07:51:11.000000 PyNOT-redux-1.3.1/pynot/wcs.py
+-rw-r--r--   0 krogager   (501) staff       (20)     2384 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/welcome.py
+-rw-r--r--   0 krogager   (501) staff       (20)      104 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pyproject.toml
+-rw-r--r--   0 krogager   (501) staff       (20)       38 2023-05-09 07:53:04.928182 PyNOT-redux-1.3.1/setup.cfg
+-rw-r--r--   0 krogager   (501) staff       (20)     5210 2023-02-25 17:18:36.000000 PyNOT-redux-1.3.1/setup.py
```

### Comparing `PyNOT-redux-1.3/.DS_Store` & `PyNOT-redux-1.3.1/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -267,16 +267,16 @@
 000010a0: 6c69 7374 3030 d601 0203 0405 0607 0707  list00..........
 000010b0: 070b 075d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
 000010c0: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
 000010d0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
 000010e0: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
 000010f0: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
 00001100: 6f77 5369 6465 6261 7209 0909 095f 1019  owSidebar...._..
-00001110: 7b7b 3339 322c 2031 3432 7d2c 207b 3131  {{392, 142}, {11
-00001120: 3230 2c20 3635 357d 7d09 0815 232f 3b52  20, 655}}...#/;R
+00001110: 7b7b 3234 342c 2031 3631 7d2c 207b 3132  {{244, 161}, {12
+00001120: 3638 2c20 3539 357d 7d09 0815 232f 3b52  68, 595}}...#/;R
 00001130: 5f6b 6c6d 6e6f 8b00 0000 0000 0001 0100  _klmno..........
 00001140: 0000 0000 0000 0d00 0000 0000 0000 0000  ................
 00001150: 0000 0000 0000 8c00 0000 0400 6400 6f00  ............d.o.
 00001160: 6300 7376 5372 6e6c 6f6e 6700 0000 0100  c.svSrnlong.....
 00001170: 0000 0700 4c00 4900 4300 4500 4e00 5300  ....L.I.C.E.N.S.
 00001180: 4549 6c6f 6362 6c6f 6200 0000 1000 0001  EIlocblob.......
 00001190: 8b00 0000 2eff ffff ffff ff00 0000 0000  ................
```

### Comparing `PyNOT-redux-1.3/.gitignore` & `PyNOT-redux-1.3.1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -128,7 +128,9 @@
 dmypy.json
 
 # Pyre type checker
 .pyre/
 test/implement_identify/identify_gui.py
 pynot/.instrument.cfg
 .DS_Store
+.DS_Store
+.DS_Store
```

### Comparing `PyNOT-redux-1.3/LICENSE` & `PyNOT-redux-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/PKG-INFO` & `PyNOT-redux-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNOT-redux
-Version: 1.3
+Version: 1.3.1
 Summary: Data Reduction Pipeline for NOT/ALFOSC
 Home-page: https://github.com/jkrogager/PyNOT
 Author: Jens-Kristian Krogager
 Author-email: krogager.jk@gmail.com
 License: MIT
 Keywords: spectroscopy astronomy longslit data processing pipeline
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PyNOT-redux-1.3/PyNOT_redux.egg-info/PKG-INFO` & `PyNOT-redux-1.3.1/PyNOT_redux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNOT-redux
-Version: 1.3
+Version: 1.3.1
 Summary: Data Reduction Pipeline for NOT/ALFOSC
 Home-page: https://github.com/jkrogager/PyNOT
 Author: Jens-Kristian Krogager
 Author-email: krogager.jk@gmail.com
 License: MIT
 Keywords: spectroscopy astronomy longslit data processing pipeline
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PyNOT-redux-1.3/PyNOT_redux.egg-info/SOURCES.txt` & `PyNOT-redux-1.3.1/PyNOT_redux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/README.md` & `PyNOT-redux-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/__init__.py` & `PyNOT-redux-1.3.1/pynot/__init__.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/alfosc.py` & `PyNOT-redux-1.3.1/pynot/alfosc.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/HeAr_linelist.dat` & `PyNOT-redux-1.3.1/pynot/calib/HeAr_linelist.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/HeNe_linelist.dat` & `PyNOT-redux-1.3.1/pynot/calib/HeNe_linelist.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/ThAr_linelist.dat` & `PyNOT-redux-1.3.1/pynot/calib/ThAr_linelist.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/alfosc_filters.dat` & `PyNOT-redux-1.3.1/pynot/calib/alfosc_filters.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/default_options.yml` & `PyNOT-redux-1.3.1/pynot/calib/default_options.yml`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/default_options_img.yml` & `PyNOT-redux-1.3.1/pynot/calib/default_options_img.yml`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/efosc_filters.dat` & `PyNOT-redux-1.3.1/pynot/calib/efosc_filters.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/lapalma.ext` & `PyNOT-redux-1.3.1/pynot/calib/lapalma.ext`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/lasilla.ext` & `PyNOT-redux-1.3.1/pynot/calib/lasilla.ext`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/paranal.ext` & `PyNOT-redux-1.3.1/pynot/calib/paranal.ext`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/std/bd174708.dat` & `PyNOT-redux-1.3.1/pynot/calib/std/bd174708.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/std/bd262606.dat` & `PyNOT-redux-1.3.1/pynot/calib/std/bd262606.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/std/bd332642.dat` & `PyNOT-redux-1.3.1/pynot/calib/std/bd332642.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/std/bd75325.dat` & `PyNOT-redux-1.3.1/pynot/calib/std/bd75325.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/std/eg21.dat` & `PyNOT-redux-1.3.1/pynot/calib/std/eg21.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/std/feige110.dat` & `PyNOT-redux-1.3.1/pynot/calib/std/feige110.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/std/feige34.dat` & `PyNOT-redux-1.3.1/pynot/calib/std/feige34.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/std/gd153.dat` & `PyNOT-redux-1.3.1/pynot/calib/std/gd153.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/std/gd50.dat` & `PyNOT-redux-1.3.1/pynot/calib/std/gd50.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/std/gd71.dat` & `PyNOT-redux-1.3.1/pynot/calib/std/gd71.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/std/hd19445.dat` & `PyNOT-redux-1.3.1/pynot/calib/std/hd19445.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/std/hd84937.dat` & `PyNOT-redux-1.3.1/pynot/calib/std/hd84937.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/std/hd93521.dat` & `PyNOT-redux-1.3.1/pynot/calib/std/hd93521.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/std/he3.dat` & `PyNOT-redux-1.3.1/pynot/calib/std/he3.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/std/hiltner600.dat` & `PyNOT-redux-1.3.1/pynot/calib/std/hiltner600.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/std/ltt3864.dat` & `PyNOT-redux-1.3.1/pynot/calib/std/ltt3864.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calib/std/wolf1346.dat` & `PyNOT-redux-1.3.1/pynot/calib/std/wolf1346.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/calibs.py` & `PyNOT-redux-1.3.1/pynot/calibs.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/data/alfosc.rules` & `PyNOT-redux-1.3.1/pynot/data/alfosc.rules`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/data/efosc.rules` & `PyNOT-redux-1.3.1/pynot/data/efosc.rules`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/data/help/welcome_msg_extract.html` & `PyNOT-redux-1.3.1/pynot/data/help/welcome_msg_extract.html`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/data/help/welcome_msg_identify.html` & `PyNOT-redux-1.3.1/pynot/data/help/welcome_msg_identify.html`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/data/help/welcome_msg_response.html` & `PyNOT-redux-1.3.1/pynot/data/help/welcome_msg_response.html`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/data/io.py` & `PyNOT-redux-1.3.1/pynot/data/io.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/data/obs.py` & `PyNOT-redux-1.3.1/pynot/data/obs.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/data/organizer.py` & `PyNOT-redux-1.3.1/pynot/data/organizer.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/efosc.py` & `PyNOT-redux-1.3.1/pynot/efosc.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/extract_gui.py` & `PyNOT-redux-1.3.1/pynot/extract_gui.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/extraction.py` & `PyNOT-redux-1.3.1/pynot/extraction.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/fitsio.py` & `PyNOT-redux-1.3.1/pynot/fitsio.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/functions.py` & `PyNOT-redux-1.3.1/pynot/functions.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/identify_gui.py` & `PyNOT-redux-1.3.1/pynot/identify_gui.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/insconfig.py` & `PyNOT-redux-1.3.1/pynot/insconfig.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/logging.py` & `PyNOT-redux-1.3.1/pynot/logging.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/main.py` & `PyNOT-redux-1.3.1/pynot/main.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/phot.py` & `PyNOT-redux-1.3.1/pynot/phot.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/phot_redux.py` & `PyNOT-redux-1.3.1/pynot/phot_redux.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/redux.py` & `PyNOT-redux-1.3.1/pynot/redux.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/reports.py` & `PyNOT-redux-1.3.1/pynot/reports.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/response.py` & `PyNOT-redux-1.3.1/pynot/response.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/response_gui.py` & `PyNOT-redux-1.3.1/pynot/response_gui.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/scired.py` & `PyNOT-redux-1.3.1/pynot/scired.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/scombine.py` & `PyNOT-redux-1.3.1/pynot/scombine.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/tasks.py` & `PyNOT-redux-1.3.1/pynot/tasks.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/transients.py` & `PyNOT-redux-1.3.1/pynot/transients.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/txtio.py` & `PyNOT-redux-1.3.1/pynot/txtio.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/wavecal.py` & `PyNOT-redux-1.3.1/pynot/wavecal.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/pynot/wcs.py` & `PyNOT-redux-1.3.1/pynot/wcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,15 +280,14 @@
     # Fit the WCS transformation:    
     _, crval, CD, _ = get_WCS(hdr)
     msg.append("          - Fitting WCS transformation using %i sources" % len(matched_ref))
     wcs_keys = update_WCS(matched_sep, matched_ref, crval, CD)
     hdr.update(wcs_keys)
     hdr.add_comment("PyNOT: WCS calibration using Gaia %s" % gaia_dr.upper())
     hdr['RADESYSa'] = 'ICRS'
-    hdr['RADECSYS'] = 'ICRS'
     msg.append("          - Updating WCS information")
 
 
     # -- Plot solution:
     plt.close('all')
     warnings.simplefilter('ignore', category=AstropyWarning)
     wcs_new = WCS(hdr)
```

### Comparing `PyNOT-redux-1.3/pynot/welcome.py` & `PyNOT-redux-1.3.1/pynot/welcome.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3/setup.py` & `PyNOT-redux-1.3.1/setup.py`

 * *Files identical despite different names*

