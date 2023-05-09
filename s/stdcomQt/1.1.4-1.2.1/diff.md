# Comparing `tmp/stdcomQt-1.1.4.tar.gz` & `tmp/stdcomQt-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdcomQt-1.1.4.tar", last modified: Mon Jan 16 20:21:46 2023, max compression
+gzip compressed data, was "stdcomQt-1.2.1.tar", last modified: Tue May  9 16:39:20 2023, max compression
```

## Comparing `stdcomQt-1.1.4.tar` & `stdcomQt-1.2.1.tar`

### file list

```diff
@@ -1,90 +1,84 @@
-drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-01-16 20:21:46.825073 stdcomQt-1.1.4/
--rw-rw-r--   0 ed        (1000) ed        (1000)     1069 2022-10-03 18:54:26.000000 stdcomQt-1.1.4/LICENSE.txt
--rw-rw-r--   0 ed        (1000) ed        (1000)      167 2022-10-03 18:54:26.000000 stdcomQt-1.1.4/MANIFEST.in
--rw-rw-r--   0 ed        (1000) ed        (1000)      750 2023-01-16 20:21:46.825073 stdcomQt-1.1.4/PKG-INFO
--rw-rw-r--   0 ed        (1000) ed        (1000)     2110 2022-11-10 19:29:00.000000 stdcomQt-1.1.4/README.md
--rw-rw-r--   0 ed        (1000) ed        (1000)       58 2022-10-03 18:54:26.000000 stdcomQt-1.1.4/requirements.txt
--rw-rw-r--   0 ed        (1000) ed        (1000)       38 2023-01-16 20:21:46.825073 stdcomQt-1.1.4/setup.cfg
--rw-rw-r--   0 ed        (1000) ed        (1000)     1211 2023-01-16 20:00:47.000000 stdcomQt-1.1.4/setup.py
-drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-01-16 20:21:46.817072 stdcomQt-1.1.4/src/
-drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-01-16 20:21:46.821072 stdcomQt-1.1.4/src/stdcomQt/
--rw-rw-r--   0 ed        (1000) ed        (1000)     1037 2023-01-16 19:46:32.000000 stdcomQt-1.1.4/src/stdcomQt/__init__.py
-drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-01-16 20:21:46.821072 stdcomQt-1.1.4/src/stdcomQt/__pycache__/
--rw-rw-r--   0 ed        (1000) ed        (1000)     1097 2023-01-16 19:58:00.000000 stdcomQt-1.1.4/src/stdcomQt/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 ed        (1000) ed        (1000)     1814 2022-10-04 16:59:55.000000 stdcomQt-1.1.4/src/stdcomQt/__pycache__/pjanicesimple.cpython-310.pyc
--rw-rw-r--   0 ed        (1000) ed        (1000)    15379 2023-01-11 22:02:52.000000 stdcomQt-1.1.4/src/stdcomQt/__pycache__/stdcomQt.cpython-310.pyc
--rw-rw-r--   0 ed        (1000) ed        (1000)    16422 2023-01-16 20:18:15.000000 stdcomQt-1.1.4/src/stdcomQt/__pycache__/stdcomQtC20.cpython-310.pyc
--rw-rw-r--   0 ed        (1000) ed        (1000)     5788 2022-10-04 16:59:55.000000 stdcomQt-1.1.4/src/stdcomQt/__pycache__/stdcomQtPjanice.cpython-310.pyc
--rw-rw-r--   0 ed        (1000) ed        (1000)     1272 2023-01-16 20:15:34.000000 stdcomQt-1.1.4/src/stdcomQt/__pycache__/stdcomQtargs.cpython-310.pyc
--rw-rw-r--   0 ed        (1000) ed        (1000)     2895 2022-10-03 18:57:57.000000 stdcomQt-1.1.4/src/stdcomQt/__pycache__/stdcomipconfigdialog.cpython-310.pyc
--rw-rw-r--   0 ed        (1000) ed        (1000)    10067 2022-11-17 19:34:18.000000 stdcomQt-1.1.4/src/stdcomQt/__pycache__/stdcomutilitywidgets.cpython-310.pyc
--rw-rw-r--   0 ed        (1000) ed        (1000)     1508 2023-01-09 22:07:07.000000 stdcomQt-1.1.4/src/stdcomQt/__pycache__/stdcomvsettings.cpython-310.pyc
--rw-rw-r--   0 ed        (1000) ed        (1000)     4292 2022-10-03 18:57:57.000000 stdcomQt-1.1.4/src/stdcomQt/__pycache__/stedcompostgresconfig.cpython-310.pyc
-drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-01-16 20:21:46.821072 stdcomQt-1.1.4/src/stdcomQt/aicontrols/
--rw-rw-r--   0 ed        (1000) ed        (1000)      260 2022-12-26 18:18:52.000000 stdcomQt-1.1.4/src/stdcomQt/aicontrols/CSVReader.py
--rw-rw-r--   0 ed        (1000) ed        (1000)    19708 2022-12-26 18:14:15.000000 stdcomQt-1.1.4/src/stdcomQt/aicontrols/PID_train.png
--rw-rw-r--   0 ed        (1000) ed        (1000)     1413 2022-12-26 18:14:15.000000 stdcomQt-1.1.4/src/stdcomQt/aicontrols/PID_train_data.csv
--rw-rw-r--   0 ed        (1000) ed        (1000)    11016 2023-01-16 19:58:00.000000 stdcomQt-1.1.4/src/stdcomQt/aicontrols/toys.py
-drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-01-16 20:21:46.821072 stdcomQt-1.1.4/src/stdcomQt/examples/
--rw-rw-r--   0 ed        (1000) ed        (1000)       46 2022-10-04 17:09:06.000000 stdcomQt-1.1.4/src/stdcomQt/examples/Stec.PJanice
--rw-rw-r--   0 ed        (1000) ed        (1000)     1892 2022-10-03 18:54:26.000000 stdcomQt-1.1.4/src/stdcomQt/examples/multipleSubs.py
--rw-rw-r--   0 ed        (1000) ed        (1000)     2341 2022-10-04 17:08:54.000000 stdcomQt-1.1.4/src/stdcomQt/examples/pjaniceExample.py
--rw-rw-r--   0 ed        (1000) ed        (1000)     2760 2022-10-04 16:57:18.000000 stdcomQt-1.1.4/src/stdcomQt/pjanicesimple.py
--rw-rw-r--   0 ed        (1000) ed        (1000)     2224 2022-10-03 18:54:26.000000 stdcomQt-1.1.4/src/stdcomQt/pjanicesimple.ui
--rw-rw-r--   0 ed        (1000) ed        (1000)       95 2023-01-09 21:33:19.000000 stdcomQt-1.1.4/src/stdcomQt/stdcomQt.ResidentSubscriber
--rw-rw-r--   0 ed        (1000) ed        (1000)    16579 2023-01-09 22:08:49.000000 stdcomQt-1.1.4/src/stdcomQt/stdcomQt.py
--rw-rw-r--   0 ed        (1000) ed        (1000)    20200 2023-01-16 20:18:09.000000 stdcomQt-1.1.4/src/stdcomQt/stdcomQtC20.py
--rw-rw-r--   0 ed        (1000) ed        (1000)     6025 2022-10-04 16:59:51.000000 stdcomQt-1.1.4/src/stdcomQt/stdcomQtPjanice.py
--rw-rw-r--   0 ed        (1000) ed        (1000)      954 2023-01-16 20:15:28.000000 stdcomQt-1.1.4/src/stdcomQt/stdcomQtargs.py
--rw-rw-r--   0 ed        (1000) ed        (1000)     4617 2022-10-03 18:54:26.000000 stdcomQt-1.1.4/src/stdcomQt/stdcomipconfigdialog.py
--rw-rw-r--   0 ed        (1000) ed        (1000)     3588 2022-10-03 18:54:26.000000 stdcomQt-1.1.4/src/stdcomQt/stdcomipconfigdialog.ui
--rw-rw-r--   0 ed        (1000) ed        (1000)    11104 2022-11-17 19:34:18.000000 stdcomQt-1.1.4/src/stdcomQt/stdcomutilitywidgets.py
--rw-rw-r--   0 ed        (1000) ed        (1000)     1042 2023-01-09 22:07:07.000000 stdcomQt-1.1.4/src/stdcomQt/stdcomvsettings.py
--rw-rw-r--   0 ed        (1000) ed        (1000)     9263 2022-10-03 18:54:26.000000 stdcomQt-1.1.4/src/stdcomQt/stedcompostgresconfig.py
--rw-rw-r--   0 ed        (1000) ed        (1000)     8439 2022-10-03 18:54:26.000000 stdcomQt-1.1.4/src/stdcomQt/stedcompostgresconfig.ui
-drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-01-16 20:21:46.821072 stdcomQt-1.1.4/src/stdcomQt/utilitys/
--rw-rw-r--   0 ed        (1000) ed        (1000)       51 2022-10-26 18:14:19.000000 stdcomQt-1.1.4/src/stdcomQt/utilitys/Stec.PJanice
--rw-rw-r--   0 ed        (1000) ed        (1000)     2340 2022-10-26 18:05:02.000000 stdcomQt-1.1.4/src/stdcomQt/utilitys/pjaniceExt.py
-drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-01-16 20:21:46.821072 stdcomQt-1.1.4/src/stdcomQt.egg-info/
--rw-rw-r--   0 ed        (1000) ed        (1000)      750 2023-01-16 20:21:46.000000 stdcomQt-1.1.4/src/stdcomQt.egg-info/PKG-INFO
--rw-rw-r--   0 ed        (1000) ed        (1000)     2742 2023-01-16 20:21:46.000000 stdcomQt-1.1.4/src/stdcomQt.egg-info/SOURCES.txt
--rw-rw-r--   0 ed        (1000) ed        (1000)        1 2023-01-16 20:21:46.000000 stdcomQt-1.1.4/src/stdcomQt.egg-info/dependency_links.txt
--rw-rw-r--   0 ed        (1000) ed        (1000)        6 2023-01-16 20:21:46.000000 stdcomQt-1.1.4/src/stdcomQt.egg-info/requires.txt
--rw-rw-r--   0 ed        (1000) ed        (1000)        9 2023-01-16 20:21:46.000000 stdcomQt-1.1.4/src/stdcomQt.egg-info/top_level.txt
-drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-01-16 20:21:46.817072 stdcomQt-1.1.4/text/
-drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-01-16 20:21:46.817072 stdcomQt-1.1.4/text/build/
-drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-01-16 20:21:46.821072 stdcomQt-1.1.4/text/build/html/
--rw-rw-r--   0 ed        (1000) ed        (1000)      230 2023-01-16 20:18:15.000000 stdcomQt-1.1.4/text/build/html/.buildinfo
-drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-01-16 20:21:46.821072 stdcomQt-1.1.4/text/build/html/_modules/
--rw-rw-r--   0 ed        (1000) ed        (1000)     2977 2023-01-16 20:18:15.000000 stdcomQt-1.1.4/text/build/html/_modules/index.html
--rw-rw-r--   0 ed        (1000) ed        (1000)    84027 2023-01-16 20:15:34.000000 stdcomQt-1.1.4/text/build/html/_modules/stdcomQt.html
--rw-rw-r--   0 ed        (1000) ed        (1000)   102794 2023-01-16 20:18:15.000000 stdcomQt-1.1.4/text/build/html/_modules/stdcomQtC20.html
--rw-rw-r--   0 ed        (1000) ed        (1000)    33628 2023-01-16 20:15:34.000000 stdcomQt-1.1.4/text/build/html/_modules/stdcomQtPjanice.html
--rw-rw-r--   0 ed        (1000) ed        (1000)     7448 2023-01-16 20:15:34.000000 stdcomQt-1.1.4/text/build/html/_modules/stdcomQtargs.html
--rw-rw-r--   0 ed        (1000) ed        (1000)    57310 2023-01-16 20:15:34.000000 stdcomQt-1.1.4/text/build/html/_modules/stdcomutilitywidgets.html
--rw-rw-r--   0 ed        (1000) ed        (1000)     7493 2023-01-16 20:15:34.000000 stdcomQt-1.1.4/text/build/html/_modules/stdcomvsettings.html
-drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-01-16 20:21:46.825073 stdcomQt-1.1.4/text/build/html/_sources/
--rw-rw-r--   0 ed        (1000) ed        (1000)      311 2023-01-16 20:04:45.000000 stdcomQt-1.1.4/text/build/html/_sources/code.rst.txt
--rw-rw-r--   0 ed        (1000) ed        (1000)      615 2023-01-16 19:53:06.000000 stdcomQt-1.1.4/text/build/html/_sources/index.rst.txt
-drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-01-16 20:21:46.825073 stdcomQt-1.1.4/text/build/html/_static/
--rw-rw-r--   0 ed        (1000) ed        (1000)    11185 2023-01-16 20:18:15.000000 stdcomQt-1.1.4/text/build/html/_static/alabaster.css
--rw-rw-r--   0 ed        (1000) ed        (1000)    14667 2023-01-16 20:18:15.000000 stdcomQt-1.1.4/text/build/html/_static/basic.css
--rw-rw-r--   0 ed        (1000) ed        (1000)       42 2017-05-15 18:58:47.000000 stdcomQt-1.1.4/text/build/html/_static/custom.css
--rw-rw-r--   0 ed        (1000) ed        (1000)     9630 2021-11-17 15:50:47.000000 stdcomQt-1.1.4/text/build/html/_static/doctools.js
--rw-rw-r--   0 ed        (1000) ed        (1000)      355 2023-01-16 20:18:15.000000 stdcomQt-1.1.4/text/build/html/_static/documentation_options.js
--rw-rw-r--   0 ed        (1000) ed        (1000)      286 2021-01-01 06:53:29.000000 stdcomQt-1.1.4/text/build/html/_static/file.png
--rw-rw-r--   0 ed        (1000) ed        (1000)     4787 2021-06-13 20:25:40.000000 stdcomQt-1.1.4/text/build/html/_static/forkme_right_darkblue_121621.png
--rw-rw-r--   0 ed        (1000) ed        (1000)   288550 2022-02-21 10:29:39.000000 stdcomQt-1.1.4/text/build/html/_static/jquery.js
--rw-rw-r--   0 ed        (1000) ed        (1000)    10854 2023-01-16 20:18:15.000000 stdcomQt-1.1.4/text/build/html/_static/language_data.js
--rw-rw-r--   0 ed        (1000) ed        (1000)       90 2021-01-01 06:53:29.000000 stdcomQt-1.1.4/text/build/html/_static/minus.png
--rw-rw-r--   0 ed        (1000) ed        (1000)       90 2021-01-01 06:53:29.000000 stdcomQt-1.1.4/text/build/html/_static/plus.png
--rw-rw-r--   0 ed        (1000) ed        (1000)     5249 2023-01-16 20:18:15.000000 stdcomQt-1.1.4/text/build/html/_static/pygments.css
--rw-rw-r--   0 ed        (1000) ed        (1000)    16950 2021-12-19 12:55:13.000000 stdcomQt-1.1.4/text/build/html/_static/searchtools.js
--rw-rw-r--   0 ed        (1000) ed        (1000)    68398 2021-12-16 10:20:19.000000 stdcomQt-1.1.4/text/build/html/_static/underscore.js
--rw-rw-r--   0 ed        (1000) ed        (1000)    68534 2023-01-16 20:18:15.000000 stdcomQt-1.1.4/text/build/html/code.html
--rw-rw-r--   0 ed        (1000) ed        (1000)    16637 2023-01-16 20:18:15.000000 stdcomQt-1.1.4/text/build/html/genindex.html
--rw-rw-r--   0 ed        (1000) ed        (1000)     4737 2023-01-16 20:18:15.000000 stdcomQt-1.1.4/text/build/html/index.html
--rw-rw-r--   0 ed        (1000) ed        (1000)      893 2023-01-16 20:18:15.000000 stdcomQt-1.1.4/text/build/html/objects.inv
--rw-rw-r--   0 ed        (1000) ed        (1000)     3907 2023-01-16 20:18:15.000000 stdcomQt-1.1.4/text/build/html/py-modindex.html
--rw-rw-r--   0 ed        (1000) ed        (1000)     2842 2023-01-16 20:18:15.000000 stdcomQt-1.1.4/text/build/html/search.html
--rw-rw-r--   0 ed        (1000) ed        (1000)     6587 2023-01-16 20:18:15.000000 stdcomQt-1.1.4/text/build/html/searchindex.js
+drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-05-09 16:39:20.423776 stdcomQt-1.2.1/
+-rw-rw-r--   0 ed        (1000) ed        (1000)     1069 2022-10-03 18:54:26.000000 stdcomQt-1.2.1/LICENSE.txt
+-rw-rw-r--   0 ed        (1000) ed        (1000)      167 2022-10-03 18:54:26.000000 stdcomQt-1.2.1/MANIFEST.in
+-rw-rw-r--   0 ed        (1000) ed        (1000)      750 2023-05-09 16:39:20.423776 stdcomQt-1.2.1/PKG-INFO
+-rw-rw-r--   0 ed        (1000) ed        (1000)     2110 2022-11-10 19:29:00.000000 stdcomQt-1.2.1/README.md
+-rw-rw-r--   0 ed        (1000) ed        (1000)      189 2023-05-09 16:16:23.000000 stdcomQt-1.2.1/requirements.txt
+-rw-rw-r--   0 ed        (1000) ed        (1000)       38 2023-05-09 16:39:20.423776 stdcomQt-1.2.1/setup.cfg
+-rw-rw-r--   0 ed        (1000) ed        (1000)     1188 2023-05-09 16:17:25.000000 stdcomQt-1.2.1/setup.py
+drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-05-09 16:39:20.415776 stdcomQt-1.2.1/src/
+drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-05-09 16:39:20.419776 stdcomQt-1.2.1/src/stdcomQt/
+-rw-rw-r--   0 ed        (1000) ed        (1000)     1206 2023-05-09 16:05:04.000000 stdcomQt-1.2.1/src/stdcomQt/__init__.py
+drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-05-09 16:39:20.419776 stdcomQt-1.2.1/src/stdcomQt/__pycache__/
+-rw-rw-r--   0 ed        (1000) ed        (1000)     1220 2023-05-09 16:05:42.000000 stdcomQt-1.2.1/src/stdcomQt/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 ed        (1000) ed        (1000)     1814 2022-10-04 16:59:55.000000 stdcomQt-1.2.1/src/stdcomQt/__pycache__/pjanicesimple.cpython-310.pyc
+-rw-rw-r--   0 ed        (1000) ed        (1000)    16164 2023-05-09 16:16:45.000000 stdcomQt-1.2.1/src/stdcomQt/__pycache__/stdcomQt.cpython-310.pyc
+-rw-rw-r--   0 ed        (1000) ed        (1000)    27313 2023-05-04 20:08:06.000000 stdcomQt-1.2.1/src/stdcomQt/__pycache__/stdcomQtC20.cpython-310.pyc
+-rw-rw-r--   0 ed        (1000) ed        (1000)     5788 2022-10-04 16:59:55.000000 stdcomQt-1.2.1/src/stdcomQt/__pycache__/stdcomQtPjanice.cpython-310.pyc
+-rw-rw-r--   0 ed        (1000) ed        (1000)     1272 2023-01-16 20:15:34.000000 stdcomQt-1.2.1/src/stdcomQt/__pycache__/stdcomQtargs.cpython-310.pyc
+-rw-rw-r--   0 ed        (1000) ed        (1000)     2895 2022-10-03 18:57:57.000000 stdcomQt-1.2.1/src/stdcomQt/__pycache__/stdcomipconfigdialog.cpython-310.pyc
+-rw-rw-r--   0 ed        (1000) ed        (1000)    10067 2022-11-17 19:34:18.000000 stdcomQt-1.2.1/src/stdcomQt/__pycache__/stdcomutilitywidgets.cpython-310.pyc
+-rw-rw-r--   0 ed        (1000) ed        (1000)     1501 2023-01-19 18:02:10.000000 stdcomQt-1.2.1/src/stdcomQt/__pycache__/stdcomvsettings.cpython-310.pyc
+-rw-rw-r--   0 ed        (1000) ed        (1000)     4292 2022-10-03 18:57:57.000000 stdcomQt-1.2.1/src/stdcomQt/__pycache__/stedcompostgresconfig.cpython-310.pyc
+drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-05-09 16:39:20.419776 stdcomQt-1.2.1/src/stdcomQt/examples/
+-rw-rw-r--   0 ed        (1000) ed        (1000)       46 2022-10-04 17:09:06.000000 stdcomQt-1.2.1/src/stdcomQt/examples/Stec.PJanice
+-rw-rw-r--   0 ed        (1000) ed        (1000)     1892 2022-10-03 18:54:26.000000 stdcomQt-1.2.1/src/stdcomQt/examples/multipleSubs.py
+-rw-rw-r--   0 ed        (1000) ed        (1000)     2341 2022-10-04 17:08:54.000000 stdcomQt-1.2.1/src/stdcomQt/examples/pjaniceExample.py
+-rw-rw-r--   0 ed        (1000) ed        (1000)     2760 2022-10-04 16:57:18.000000 stdcomQt-1.2.1/src/stdcomQt/pjanicesimple.py
+-rw-rw-r--   0 ed        (1000) ed        (1000)     2224 2022-10-03 18:54:26.000000 stdcomQt-1.2.1/src/stdcomQt/pjanicesimple.ui
+-rw-rw-r--   0 ed        (1000) ed        (1000)    17184 2023-05-09 16:14:57.000000 stdcomQt-1.2.1/src/stdcomQt/stdcomQt.py
+-rw-rw-r--   0 ed        (1000) ed        (1000)    36058 2023-05-04 20:08:05.000000 stdcomQt-1.2.1/src/stdcomQt/stdcomQtC20.py
+-rw-rw-r--   0 ed        (1000) ed        (1000)     6025 2022-10-04 16:59:51.000000 stdcomQt-1.2.1/src/stdcomQt/stdcomQtPjanice.py
+-rw-rw-r--   0 ed        (1000) ed        (1000)      954 2023-01-16 20:15:28.000000 stdcomQt-1.2.1/src/stdcomQt/stdcomQtargs.py
+-rw-rw-r--   0 ed        (1000) ed        (1000)     4617 2022-10-03 18:54:26.000000 stdcomQt-1.2.1/src/stdcomQt/stdcomipconfigdialog.py
+-rw-rw-r--   0 ed        (1000) ed        (1000)     3588 2022-10-03 18:54:26.000000 stdcomQt-1.2.1/src/stdcomQt/stdcomipconfigdialog.ui
+-rw-rw-r--   0 ed        (1000) ed        (1000)    11104 2022-11-17 19:34:18.000000 stdcomQt-1.2.1/src/stdcomQt/stdcomutilitywidgets.py
+-rw-rw-r--   0 ed        (1000) ed        (1000)     1029 2023-01-19 18:02:10.000000 stdcomQt-1.2.1/src/stdcomQt/stdcomvsettings.py
+-rw-rw-r--   0 ed        (1000) ed        (1000)     9263 2022-10-03 18:54:26.000000 stdcomQt-1.2.1/src/stdcomQt/stedcompostgresconfig.py
+-rw-rw-r--   0 ed        (1000) ed        (1000)     8439 2022-10-03 18:54:26.000000 stdcomQt-1.2.1/src/stdcomQt/stedcompostgresconfig.ui
+drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-05-09 16:39:20.419776 stdcomQt-1.2.1/src/stdcomQt/utilitys/
+-rw-rw-r--   0 ed        (1000) ed        (1000)       51 2022-10-26 18:14:19.000000 stdcomQt-1.2.1/src/stdcomQt/utilitys/Stec.PJanice
+-rw-rw-r--   0 ed        (1000) ed        (1000)     2340 2022-10-26 18:05:02.000000 stdcomQt-1.2.1/src/stdcomQt/utilitys/pjaniceExt.py
+drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-05-09 16:39:20.419776 stdcomQt-1.2.1/src/stdcomQt.egg-info/
+-rw-rw-r--   0 ed        (1000) ed        (1000)      750 2023-05-09 16:39:20.000000 stdcomQt-1.2.1/src/stdcomQt.egg-info/PKG-INFO
+-rw-rw-r--   0 ed        (1000) ed        (1000)     2551 2023-05-09 16:39:20.000000 stdcomQt-1.2.1/src/stdcomQt.egg-info/SOURCES.txt
+-rw-rw-r--   0 ed        (1000) ed        (1000)        1 2023-05-09 16:39:20.000000 stdcomQt-1.2.1/src/stdcomQt.egg-info/dependency_links.txt
+-rw-rw-r--   0 ed        (1000) ed        (1000)        6 2023-05-09 16:39:20.000000 stdcomQt-1.2.1/src/stdcomQt.egg-info/requires.txt
+-rw-rw-r--   0 ed        (1000) ed        (1000)        9 2023-05-09 16:39:20.000000 stdcomQt-1.2.1/src/stdcomQt.egg-info/top_level.txt
+drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-05-09 16:39:20.415776 stdcomQt-1.2.1/text/
+drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-05-09 16:39:20.415776 stdcomQt-1.2.1/text/build/
+drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-05-09 16:39:20.419776 stdcomQt-1.2.1/text/build/html/
+-rw-rw-r--   0 ed        (1000) ed        (1000)      230 2023-01-16 20:18:15.000000 stdcomQt-1.2.1/text/build/html/.buildinfo
+drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-05-09 16:39:20.423776 stdcomQt-1.2.1/text/build/html/_modules/
+-rw-rw-r--   0 ed        (1000) ed        (1000)     2977 2023-01-16 20:18:15.000000 stdcomQt-1.2.1/text/build/html/_modules/index.html
+-rw-rw-r--   0 ed        (1000) ed        (1000)    84027 2023-01-16 20:15:34.000000 stdcomQt-1.2.1/text/build/html/_modules/stdcomQt.html
+-rw-rw-r--   0 ed        (1000) ed        (1000)   102794 2023-01-16 20:18:15.000000 stdcomQt-1.2.1/text/build/html/_modules/stdcomQtC20.html
+-rw-rw-r--   0 ed        (1000) ed        (1000)    33628 2023-01-16 20:15:34.000000 stdcomQt-1.2.1/text/build/html/_modules/stdcomQtPjanice.html
+-rw-rw-r--   0 ed        (1000) ed        (1000)     7448 2023-01-16 20:15:34.000000 stdcomQt-1.2.1/text/build/html/_modules/stdcomQtargs.html
+-rw-rw-r--   0 ed        (1000) ed        (1000)    57310 2023-01-16 20:15:34.000000 stdcomQt-1.2.1/text/build/html/_modules/stdcomutilitywidgets.html
+-rw-rw-r--   0 ed        (1000) ed        (1000)     7493 2023-01-16 20:15:34.000000 stdcomQt-1.2.1/text/build/html/_modules/stdcomvsettings.html
+drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-05-09 16:39:20.423776 stdcomQt-1.2.1/text/build/html/_sources/
+-rw-rw-r--   0 ed        (1000) ed        (1000)      311 2023-01-16 20:04:45.000000 stdcomQt-1.2.1/text/build/html/_sources/code.rst.txt
+-rw-rw-r--   0 ed        (1000) ed        (1000)      615 2023-01-16 19:53:06.000000 stdcomQt-1.2.1/text/build/html/_sources/index.rst.txt
+drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2023-05-09 16:39:20.423776 stdcomQt-1.2.1/text/build/html/_static/
+-rw-rw-r--   0 ed        (1000) ed        (1000)    11185 2023-01-16 20:18:15.000000 stdcomQt-1.2.1/text/build/html/_static/alabaster.css
+-rw-rw-r--   0 ed        (1000) ed        (1000)    14667 2023-01-16 20:18:15.000000 stdcomQt-1.2.1/text/build/html/_static/basic.css
+-rw-rw-r--   0 ed        (1000) ed        (1000)       42 2017-05-15 18:58:47.000000 stdcomQt-1.2.1/text/build/html/_static/custom.css
+-rw-rw-r--   0 ed        (1000) ed        (1000)     9630 2021-11-17 15:50:47.000000 stdcomQt-1.2.1/text/build/html/_static/doctools.js
+-rw-rw-r--   0 ed        (1000) ed        (1000)      355 2023-01-16 20:18:15.000000 stdcomQt-1.2.1/text/build/html/_static/documentation_options.js
+-rw-rw-r--   0 ed        (1000) ed        (1000)      286 2021-01-01 06:53:29.000000 stdcomQt-1.2.1/text/build/html/_static/file.png
+-rw-rw-r--   0 ed        (1000) ed        (1000)     4787 2021-06-13 20:25:40.000000 stdcomQt-1.2.1/text/build/html/_static/forkme_right_darkblue_121621.png
+-rw-rw-r--   0 ed        (1000) ed        (1000)   288550 2022-02-21 10:29:39.000000 stdcomQt-1.2.1/text/build/html/_static/jquery.js
+-rw-rw-r--   0 ed        (1000) ed        (1000)    10854 2023-01-16 20:18:15.000000 stdcomQt-1.2.1/text/build/html/_static/language_data.js
+-rw-rw-r--   0 ed        (1000) ed        (1000)       90 2021-01-01 06:53:29.000000 stdcomQt-1.2.1/text/build/html/_static/minus.png
+-rw-rw-r--   0 ed        (1000) ed        (1000)       90 2021-01-01 06:53:29.000000 stdcomQt-1.2.1/text/build/html/_static/plus.png
+-rw-rw-r--   0 ed        (1000) ed        (1000)     5249 2023-01-16 20:18:15.000000 stdcomQt-1.2.1/text/build/html/_static/pygments.css
+-rw-rw-r--   0 ed        (1000) ed        (1000)    16950 2021-12-19 12:55:13.000000 stdcomQt-1.2.1/text/build/html/_static/searchtools.js
+-rw-rw-r--   0 ed        (1000) ed        (1000)    68398 2021-12-16 10:20:19.000000 stdcomQt-1.2.1/text/build/html/_static/underscore.js
+-rw-rw-r--   0 ed        (1000) ed        (1000)    68534 2023-01-16 20:18:15.000000 stdcomQt-1.2.1/text/build/html/code.html
+-rw-rw-r--   0 ed        (1000) ed        (1000)    16637 2023-01-16 20:18:15.000000 stdcomQt-1.2.1/text/build/html/genindex.html
+-rw-rw-r--   0 ed        (1000) ed        (1000)     4737 2023-01-16 20:18:15.000000 stdcomQt-1.2.1/text/build/html/index.html
+-rw-rw-r--   0 ed        (1000) ed        (1000)      893 2023-01-16 20:18:15.000000 stdcomQt-1.2.1/text/build/html/objects.inv
+-rw-rw-r--   0 ed        (1000) ed        (1000)     3907 2023-01-16 20:18:15.000000 stdcomQt-1.2.1/text/build/html/py-modindex.html
+-rw-rw-r--   0 ed        (1000) ed        (1000)     2842 2023-01-16 20:18:15.000000 stdcomQt-1.2.1/text/build/html/search.html
+-rw-rw-r--   0 ed        (1000) ed        (1000)     6587 2023-01-16 20:18:15.000000 stdcomQt-1.2.1/text/build/html/searchindex.js
```

### Comparing `stdcomQt-1.1.4/LICENSE.txt` & `stdcomQt-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/PKG-INFO` & `stdcomQt-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdcomQt
-Version: 1.1.4
+Version: 1.2.1
 Summary: Stec Railway Version StandAlone Subscribers
 Home-page: http://www.vremsoft.com
 Author: ed
 Author-email: srini_durand@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `stdcomQt-1.1.4/README.md` & `stdcomQt-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/setup.py` & `stdcomQt-1.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 from src.stdcomQt.stdcomQt import stdcomQtVersion
 
 setup(
     name='stdcomQt',
     version=stdcomQtVersion,
     license_files = ('LICENSE.txt',),
-    packages=['stdcomQt','stdcomQt.utilitys','stdcomQt.examples', 'stdcomQt.aicontrols' ],
+    packages=['stdcomQt','stdcomQt.utilitys','stdcomQt.examples' ],
     package_dir={'': 'src'},
     url='http://www.vremsoft.com',
     license='',
     author='ed',
     author_email='srini_durand@yahoo.com',
     description='Stec Railway Version StandAlone Subscribers'      ,
     classifiers = [
```

### Comparing `stdcomQt-1.1.4/src/stdcomQt/__init__.py` & `stdcomQt-1.2.1/src/stdcomQt/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from stdcomQt.pjanicesimple import Ui_pJaniceSimple
 from stdcomQt.stdcomipconfigdialog  import Ui_IPConfgDialog
 from stdcomQt.stedcompostgresconfig import Ui_PostgresConfig
 from stdcomQt.stdcomQtPjanice  import pjanicesimpleGeneric
-from stdcomQt.stdcomQt  import stdcomQtVersion, SubObject, stecQSocket, Subscriber
+from stdcomQt.stdcomQt import stdcomQtVersion, SubObject, stecQSocket, Subscriber
 from stdcomQt.stdcomutilitywidgets  import StecIPconfigDialog, StecPostgresConfigWidget, StecTreeMorph
 from stdcomQt.stdcomvsettings  import VSettings
-from stdcomQt.stdcomQtC20 import ExpFilter, Dahlin, PID, ComputerSL, HistoryDelay, F25, MapToZones, RollingAverageFilter
+from stdcomQt.stdcomQtC20 import ExpFilter, Dahlin, PID, ComputerSL, HistoryDelay, F25, F25QueRate, HistoryDelayQueRate, RollingAverageFilter, PIDClassic, F21
 from stdcomQt.stdcomQtargs import stdcomQtargs
+from stdcomQt.stdcomQtC20 import MapToZones
 
-__all__ = ['Ui_pJaniceSimple', 'Ui_IPConfgDialog', 'Ui_PostgresConfig',
+__all__ = [ 'MapToZones', 'Ui_pJaniceSimple', 'Ui_IPConfgDialog', 'Ui_PostgresConfig',
            'pjanicesimpleGeneric', 'stdcomQtVersion', 'SubObject', 'stecQSocket', 'Subscriber',
            'StecIPconfigDialog', 'StecPostgresConfigWidget', 'StecTreeMorph', 'VSettings', 'stdcomQtargs',
-            'ExpFilter', 'Dahlin', 'PID','ComputerSL', 'HistoryDelay', 'F25', 'MapToZones','RollingAverageFilter'
-           ]
+            'ExpFilter', 'Dahlin', 'PID','ComputerSL', 'HistoryDelay', 'F25', 'MapToZones','RollingAverageFilter',
+            'F21', 'PIDClassic',   'F25QueRate','HistoryDelayQueRate'
+
+            ]
```

### Comparing `stdcomQt-1.1.4/src/stdcomQt/__pycache__/__init__.cpython-310.pyc` & `stdcomQt-1.2.1/src/stdcomQt/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jan 16 19:46:32 2023 UTC, .py size: 1037 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,77 @@
-00000000: 6f0d 0d0a 0000 0000 98a9 c563 0d04 0000  o..........c....
+00000000: 6f0d 0d0a 0000 0000 306f 5a64 b604 0000  o.......0oZd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
+00000020: 0002 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 0100 6400 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
 00000080: 6d0f 5a0f 6d10 5a10 0100 6400 6407 6c11  m.Z.m.Z...d.d.l.
 00000090: 6d12 5a12 0100 6400 6408 6c13 6d14 5a14  m.Z...d.d.l.m.Z.
 000000a0: 6d15 5a15 6d16 5a16 6d17 5a17 6d18 5a18  m.Z.m.Z.m.Z.m.Z.
-000000b0: 6d19 5a19 6d1a 5a1a 6d1b 5a1b 0100 6400  m.Z.m.Z.m.Z...d.
-000000c0: 6409 6c1c 6d1d 5a1d 0100 6700 640a a201  d.l.m.Z...g.d...
-000000d0: 5a1e 640b 5300 290c e900 0000 0029 01da  Z.d.S.)......)..
-000000e0: 1055 695f 704a 616e 6963 6553 696d 706c  .Ui_pJaniceSimpl
-000000f0: 6529 01da 1055 695f 4950 436f 6e66 6744  e)...Ui_IPConfgD
-00000100: 6961 6c6f 6729 01da 1155 695f 506f 7374  ialog)...Ui_Post
-00000110: 6772 6573 436f 6e66 6967 2901 da14 706a  gresConfig)...pj
-00000120: 616e 6963 6573 696d 706c 6547 656e 6572  anicesimpleGener
-00000130: 6963 2904 da0f 7374 6463 6f6d 5174 5665  ic)...stdcomQtVe
-00000140: 7273 696f 6eda 0953 7562 4f62 6a65 6374  rsion..SubObject
-00000150: da0b 7374 6563 5153 6f63 6b65 74da 0a53  ..stecQSocket..S
-00000160: 7562 7363 7269 6265 7229 03da 1253 7465  ubscriber)...Ste
-00000170: 6349 5063 6f6e 6669 6744 6961 6c6f 67da  cIPconfigDialog.
-00000180: 1853 7465 6350 6f73 7467 7265 7343 6f6e  .StecPostgresCon
-00000190: 6669 6757 6964 6765 74da 0d53 7465 6354  figWidget..StecT
-000001a0: 7265 654d 6f72 7068 2901 da09 5653 6574  reeMorph)...VSet
-000001b0: 7469 6e67 7329 08da 0945 7870 4669 6c74  tings)...ExpFilt
-000001c0: 6572 da06 4461 686c 696e da03 5049 44da  er..Dahlin..PID.
-000001d0: 0a43 6f6d 7075 7465 7253 4cda 0c48 6973  .ComputerSL..His
-000001e0: 746f 7279 4465 6c61 79da 0346 3235 da0a  toryDelay..F25..
-000001f0: 4d61 7054 6f5a 6f6e 6573 da14 526f 6c6c  MapToZones..Roll
-00000200: 696e 6741 7665 7261 6765 4669 6c74 6572  ingAverageFilter
-00000210: 2901 da0c 7374 6463 6f6d 5174 6172 6773  )...stdcomQtargs
-00000220: 2915 7202 0000 0072 0300 0000 7204 0000  ).r....r....r...
-00000230: 0072 0500 0000 7206 0000 0072 0700 0000  .r....r....r....
-00000240: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-00000250: 0b00 0000 720c 0000 0072 0d00 0000 7216  ....r....r....r.
-00000260: 0000 0072 0e00 0000 720f 0000 0072 1000  ...r....r....r..
-00000270: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00000280: 0072 1400 0000 7215 0000 004e 291f da16  .r....r....N)...
-00000290: 7374 6463 6f6d 5174 2e70 6a61 6e69 6365  stdcomQt.pjanice
-000002a0: 7369 6d70 6c65 7202 0000 00da 1d73 7464  simpler......std
-000002b0: 636f 6d51 742e 7374 6463 6f6d 6970 636f  comQt.stdcomipco
-000002c0: 6e66 6967 6469 616c 6f67 7203 0000 00da  nfigdialogr.....
-000002d0: 1e73 7464 636f 6d51 742e 7374 6564 636f  .stdcomQt.stedco
-000002e0: 6d70 6f73 7467 7265 7363 6f6e 6669 6772  mpostgresconfigr
-000002f0: 0400 0000 da18 7374 6463 6f6d 5174 2e73  ......stdcomQt.s
-00000300: 7464 636f 6d51 7450 6a61 6e69 6365 7205  tdcomQtPjanicer.
-00000310: 0000 00da 1173 7464 636f 6d51 742e 7374  .....stdcomQt.st
-00000320: 6463 6f6d 5174 7206 0000 0072 0700 0000  dcomQtr....r....
-00000330: 7208 0000 0072 0900 0000 da1d 7374 6463  r....r......stdc
-00000340: 6f6d 5174 2e73 7464 636f 6d75 7469 6c69  omQt.stdcomutili
-00000350: 7479 7769 6467 6574 7372 0a00 0000 720b  tywidgetsr....r.
-00000360: 0000 0072 0c00 0000 da18 7374 6463 6f6d  ...r......stdcom
-00000370: 5174 2e73 7464 636f 6d76 7365 7474 696e  Qt.stdcomvsettin
-00000380: 6773 720d 0000 00da 1473 7464 636f 6d51  gsr......stdcomQ
-00000390: 742e 7374 6463 6f6d 5174 4332 3072 0e00  t.stdcomQtC20r..
-000003a0: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
-000003b0: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
-000003c0: 7215 0000 00da 1573 7464 636f 6d51 742e  r......stdcomQt.
-000003d0: 7374 6463 6f6d 5174 6172 6773 7216 0000  stdcomQtargsr...
-000003e0: 00da 075f 5f61 6c6c 5f5f a900 7221 0000  ...__all__..r!..
-000003f0: 0072 2100 0000 fa2a 2f68 6f6d 652f 6564  .r!....*/home/ed
-00000400: 2f73 7464 636f 6d51 742f 7372 632f 7374  /stdcomQt/src/st
-00000410: 6463 6f6d 5174 2f5f 5f69 6e69 745f 5f2e  dcomQt/__init__.
-00000420: 7079 da08 3c6d 6f64 756c 653e 0100 0000  py..<module>....
-00000430: 7314 0000 000c 000c 010c 010c 0118 0114  s...............
-00000440: 010c 0128 010c 010c 02                   ...(.....
+000000b0: 6d19 5a19 6d1a 5a1a 6d1b 5a1b 6d1c 5a1c  m.Z.m.Z.m.Z.m.Z.
+000000c0: 6d1d 5a1d 6d1e 5a1e 0100 6400 6409 6c1f  m.Z.m.Z...d.d.l.
+000000d0: 6d20 5a20 0100 6400 640a 6c13 6d21 5a21  m Z ..d.d.l.m!Z!
+000000e0: 0100 6700 640b a201 5a22 640c 5300 290d  ..g.d...Z"d.S.).
+000000f0: e900 0000 0029 01da 1055 695f 704a 616e  .....)...Ui_pJan
+00000100: 6963 6553 696d 706c 6529 01da 1055 695f  iceSimple)...Ui_
+00000110: 4950 436f 6e66 6744 6961 6c6f 6729 01da  IPConfgDialog)..
+00000120: 1155 695f 506f 7374 6772 6573 436f 6e66  .Ui_PostgresConf
+00000130: 6967 2901 da14 706a 616e 6963 6573 696d  ig)...pjanicesim
+00000140: 706c 6547 656e 6572 6963 2904 da0f 7374  pleGeneric)...st
+00000150: 6463 6f6d 5174 5665 7273 696f 6eda 0953  dcomQtVersion..S
+00000160: 7562 4f62 6a65 6374 da0b 7374 6563 5153  ubObject..stecQS
+00000170: 6f63 6b65 74da 0a53 7562 7363 7269 6265  ocket..Subscribe
+00000180: 7229 03da 1253 7465 6349 5063 6f6e 6669  r)...StecIPconfi
+00000190: 6744 6961 6c6f 67da 1853 7465 6350 6f73  gDialog..StecPos
+000001a0: 7467 7265 7343 6f6e 6669 6757 6964 6765  tgresConfigWidge
+000001b0: 74da 0d53 7465 6354 7265 654d 6f72 7068  t..StecTreeMorph
+000001c0: 2901 da09 5653 6574 7469 6e67 7329 0bda  )...VSettings)..
+000001d0: 0945 7870 4669 6c74 6572 da06 4461 686c  .ExpFilter..Dahl
+000001e0: 696e da03 5049 44da 0a43 6f6d 7075 7465  in..PID..Compute
+000001f0: 7253 4cda 0c48 6973 746f 7279 4465 6c61  rSL..HistoryDela
+00000200: 79da 0346 3235 da0a 4632 3551 7565 5261  y..F25..F25QueRa
+00000210: 7465 da13 4869 7374 6f72 7944 656c 6179  te..HistoryDelay
+00000220: 5175 6552 6174 65da 1452 6f6c 6c69 6e67  QueRate..Rolling
+00000230: 4176 6572 6167 6546 696c 7465 72da 0a50  AverageFilter..P
+00000240: 4944 436c 6173 7369 63da 0346 3231 2901  IDClassic..F21).
+00000250: da0c 7374 6463 6f6d 5174 6172 6773 2901  ..stdcomQtargs).
+00000260: da0a 4d61 7054 6f5a 6f6e 6573 291a 721a  ..MapToZones).r.
+00000270: 0000 0072 0200 0000 7203 0000 0072 0400  ...r....r....r..
+00000280: 0000 7205 0000 0072 0600 0000 7207 0000  ..r....r....r...
+00000290: 0072 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
+000002a0: 720b 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+000002b0: 1900 0000 720e 0000 0072 0f00 0000 7210  ....r....r....r.
+000002c0: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
+000002d0: 0000 721a 0000 0072 1600 0000 7218 0000  ..r....r....r...
+000002e0: 0072 1700 0000 7214 0000 0072 1500 0000  .r....r....r....
+000002f0: 4e29 23da 1673 7464 636f 6d51 742e 706a  N)#..stdcomQt.pj
+00000300: 616e 6963 6573 696d 706c 6572 0200 0000  anicesimpler....
+00000310: da1d 7374 6463 6f6d 5174 2e73 7464 636f  ..stdcomQt.stdco
+00000320: 6d69 7063 6f6e 6669 6764 6961 6c6f 6772  mipconfigdialogr
+00000330: 0300 0000 da1e 7374 6463 6f6d 5174 2e73  ......stdcomQt.s
+00000340: 7465 6463 6f6d 706f 7374 6772 6573 636f  tedcompostgresco
+00000350: 6e66 6967 7204 0000 00da 1873 7464 636f  nfigr......stdco
+00000360: 6d51 742e 7374 6463 6f6d 5174 506a 616e  mQt.stdcomQtPjan
+00000370: 6963 6572 0500 0000 da11 7374 6463 6f6d  icer......stdcom
+00000380: 5174 2e73 7464 636f 6d51 7472 0600 0000  Qt.stdcomQtr....
+00000390: 7207 0000 0072 0800 0000 7209 0000 00da  r....r....r.....
+000003a0: 1d73 7464 636f 6d51 742e 7374 6463 6f6d  .stdcomQt.stdcom
+000003b0: 7574 696c 6974 7977 6964 6765 7473 720a  utilitywidgetsr.
+000003c0: 0000 0072 0b00 0000 720c 0000 00da 1873  ...r....r......s
+000003d0: 7464 636f 6d51 742e 7374 6463 6f6d 7673  tdcomQt.stdcomvs
+000003e0: 6574 7469 6e67 7372 0d00 0000 da14 7374  ettingsr......st
+000003f0: 6463 6f6d 5174 2e73 7464 636f 6d51 7443  dcomQt.stdcomQtC
+00000400: 3230 720e 0000 0072 0f00 0000 7210 0000  20r....r....r...
+00000410: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000420: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+00000430: 1700 0000 7218 0000 00da 1573 7464 636f  ....r......stdco
+00000440: 6d51 742e 7374 6463 6f6d 5174 6172 6773  mQt.stdcomQtargs
+00000450: 7219 0000 0072 1a00 0000 da07 5f5f 616c  r....r......__al
+00000460: 6c5f 5fa9 0072 2500 0000 7225 0000 00fa  l__..r%...r%....
+00000470: 2a2f 686f 6d65 2f65 642f 7374 6463 6f6d  */home/ed/stdcom
+00000480: 5174 2f73 7263 2f73 7464 636f 6d51 742f  Qt/src/stdcomQt/
+00000490: 5f5f 696e 6974 5f5f 2e70 79da 083c 6d6f  __init__.py..<mo
+000004a0: 6475 6c65 3e01 0000 0073 1600 0000 0c00  dule>....s......
+000004b0: 0c01 0c01 0c01 1801 1401 0c01 3401 0c01  ............4...
+000004c0: 0c01 0c02                                ....
```

### Comparing `stdcomQt-1.1.4/src/stdcomQt/__pycache__/pjanicesimple.cpython-310.pyc` & `stdcomQt-1.2.1/src/stdcomQt/__pycache__/pjanicesimple.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/src/stdcomQt/__pycache__/stdcomQt.cpython-310.pyc` & `stdcomQt-1.2.1/src/stdcomQt/__pycache__/stdcomQt.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jan  9 22:08:49 2023 UTC, .py size: 16579 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,962 +1,1011 @@
-00000000: 6f0d 0d0a 0000 0000 7190 bc63 c340 0000  o.......q..c.@..
+00000000: 6f0d 0d0a 0000 0000 8171 5a64 2043 0000  o........qZd C..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 9001 0000 6400  .....@...s....d.
+00000020: 0006 0000 0040 0000 0073 8a01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d08 5a08 0100 6400 6402 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000060: 6d0b 5a0b 0100 6400 6403 6c0c 5a0c 6404  m.Z...d.d.l.Z.d.
-00000070: 5a0d 4700 6405 6406 8400 6406 6507 8303  Z.G.d.d...d.e...
-00000080: 5a0e 4700 6407 6408 8400 6408 6507 8303  Z.G.d.d...d.e...
-00000090: 5a0f 4700 6409 640a 8400 640a 6507 8303  Z.G.d.d...d.e...
-000000a0: 5a10 6511 640b 6b02 72c6 6400 640c 6c12  Z.e.d.k.r.d.d.l.
-000000b0: 6d13 5a14 0100 6515 640d 8301 0100 6400  m.Z...e.d.....d.
-000000c0: 6403 6c16 5a16 640e 6516 6a17 7600 7259  d.l.Z.d.e.j.v.rY
-000000d0: 6515 650d 8301 0100 6516 a018 a100 0100  e.e.....e.......
-000000e0: 6508 6516 6a17 8301 5a19 650f 8300 5a1a  e.e.j...Z.e...Z.
-000000f0: 6510 640f 651a 8302 5a1b 651a a01c 640f  e.d.e...Z.e...d.
-00000100: 6410 a102 0100 651b a01d 6411 a101 0100  d.....e...d.....
-00000110: 651b a01e 6700 6412 a201 a101 0100 6510  e...g.d.......e.
-00000120: 640f 651a 8302 5a1f 651f a01e 6700 6413  d.e...Z.e...g.d.
-00000130: a201 a101 0100 6414 5a20 6510 6520 651a  ......d.Z e.e e.
-00000140: 8302 5a21 6514 8300 5a22 6522 a023 6520  ..Z!e...Z"e".#e 
-00000150: a101 5a24 6524 6403 7500 72b2 0900 6521  ..Z$e$d.u.r...e!
-00000160: a025 a100 5a24 0900 6524 6403 7500 72a4  .%..Z$..e$d.u.r.
-00000170: 6411 6701 5a24 0900 6521 a01e 6524 a101  d.g.Z$..e!..e$..
-00000180: 0100 0900 6522 a026 6520 6524 a102 0100  ....e".&e e$....
-00000190: 6e05 6521 a01e 6524 a101 0100 6519 a027  n.e!..e$....e..'
-000001a0: a100 0100 651a a028 a100 0100 6516 a018  ....e..(....e...
-000001b0: 6400 a101 0100 6403 5300 6403 5300 2915  d.....d.S.d.S.).
-000001c0: e900 0000 0029 08da 0651 4d75 7465 78da  .....)...QMutex.
-000001d0: 0851 5661 7269 616e 74da 0651 5469 6d65  .QVariant..QTime
-000001e0: 72da 0651 4576 656e 74da 0870 7971 7453  r..QEvent..pyqtS
-000001f0: 6c6f 74da 0a70 7971 7453 6967 6e61 6cda  lot..pyqtSignal.
-00000200: 0751 4f62 6a65 6374 da10 5143 6f72 6541  .QObject..QCoreA
-00000210: 7070 6c69 6361 7469 6f6e 2902 da0a 5154  pplication)...QT
-00000220: 6370 536f 636b 6574 da0f 5141 6273 7472  cpSocket..QAbstr
-00000230: 6163 7453 6f63 6b65 744e 7a05 312e 312e  actSocketNz.1.1.
-00000240: 3463 0000 0000 0000 0000 0000 0000 0000  4c..............
-00000250: 0000 0400 0000 0000 0000 73da 0000 0065  ..........s....e
-00000260: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
-00000270: 0565 0683 025a 0765 0465 0565 0583 025a  .e...Z.e.e.e...Z
-00000280: 0864 025a 0964 025a 0a64 035a 0b65 0565  .d.Z.d.Z.d.Z.e.e
-00000290: 0c64 043c 0067 005a 0d64 035a 0e64 055a  .d.<.g.Z.d.Z.d.Z
-000002a0: 0f65 1083 005a 1164 2587 0066 0164 0664  .e...Z.d%..f.d.d
-000002b0: 0784 095a 1267 0066 0164 0864 0984 015a  ...Z.g.f.d.d...Z
-000002c0: 1364 0a64 0b84 005a 1464 0c64 0d84 005a  .d.d...Z.d.d...Z
-000002d0: 1564 0e64 0f84 005a 1664 1064 1184 005a  .d.d...Z.d.d...Z
-000002e0: 1764 1264 1384 005a 1864 2664 1565 1966  .d.d...Z.d&d.e.f
-000002f0: 0264 1664 1784 055a 1a64 1864 1984 005a  .d.d...Z.d.d...Z
-00000300: 1b64 1a64 1b84 005a 1c64 1c64 1d84 005a  .d.d...Z.d.d...Z
-00000310: 1d64 1e64 1f84 005a 1e64 2664 2065 1966  .d.d...Z.d&d e.f
-00000320: 0264 2164 2284 055a 1f64 2364 2484 005a  .d!d"..Z.d#d$..Z
-00000330: 2087 0004 005a 2153 0029 27da 0953 7562   ....Z!S.)'..Sub
-00000340: 4f62 6a65 6374 7a25 0a20 2020 2049 6e74  Objectz%.    Int
-00000350: 6572 6e61 6c20 7573 652c 206e 6f74 2066  ernal use, not f
-00000360: 6f72 2075 7365 7273 0a20 2020 2046 4eda  or users.    FN.
-00000370: 046e 616d 6572 0100 0000 6303 0000 0000  .namer....c.....
-00000380: 0000 0000 0000 0004 0000 0003 0000 0003  ................
-00000390: 0000 0073 3400 0000 7c01 7c00 5f00 6401  ...s4...|.|._.d.
-000003a0: 7d03 7c02 6400 7501 7210 7401 8300 a002  }.|.d.u.r.t.....
-000003b0: 7c02 a101 0100 6e05 7401 8300 a002 a100  |.....n.t.......
-000003c0: 0100 6402 7c00 5f03 6400 5300 2903 4e46  ..d.|._.d.S.).NF
-000003d0: 7201 0000 0029 0472 0d00 0000 da05 7375  r....).r......su
-000003e0: 7065 72da 085f 5f69 6e69 745f 5fda 0d63  per..__init__..c
-000003f0: 6f6e 6e65 6374 6564 5375 6273 2904 da04  onnectedSubs)...
-00000400: 7365 6c66 720d 0000 00da 0650 6172 656e  selfr......Paren
-00000410: 74da 0661 6374 6976 65a9 01da 095f 5f63  t..active....__c
-00000420: 6c61 7373 5f5f a900 fa2a 2f68 6f6d 652f  lass__...*/home/
-00000430: 6564 2f73 7464 636f 6d51 742f 7372 632f  ed/stdcomQt/src/
-00000440: 7374 6463 6f6d 5174 2f73 7464 636f 6d51  stdcomQt/stdcomQ
-00000450: 742e 7079 720f 0000 0017 0000 0073 0c00  t.pyr........s..
-00000460: 0000 0601 0401 0801 0e01 0a02 0a01 7a12  ..............z.
-00000470: 5375 624f 626a 6563 742e 5f5f 696e 6974  SubObject.__init
-00000480: 5f5f 6302 0000 0000 0000 0000 0000 0002  __c.............
-00000490: 0000 0002 0000 0043 0000 0073 2600 0000  .......C...s&...
-000004a0: 7c00 6a00 a001 a100 0100 7c01 7c00 5f02  |.j.......|.|._.
-000004b0: 7c00 6a00 a003 a100 0100 7c00 a004 a100  |.j.......|.....
-000004c0: 0100 6400 5300 a901 4e29 05da 0870 726f  ..d.S...N)...pro
-000004d0: 784c 6f63 6bda 046c 6f63 6bda 0464 6174  xLock..lock..dat
-000004e0: 61da 0675 6e6c 6f63 6bda 0b46 6972 6543  a..unlock..FireC
-000004f0: 6f6e 6e65 6374 a902 7211 0000 0072 1b00  onnect..r....r..
-00000500: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00000510: 00da 0741 6464 4461 7461 1f00 0000 7308  ...AddData....s.
-00000520: 0000 000a 0106 010a 010c 017a 1153 7562  ...........z.Sub
-00000530: 4f62 6a65 6374 2e41 6464 4461 7461 6301  Object.AddDatac.
-00000540: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-00000550: 0000 0043 0000 00f3 1e00 0000 7c00 6a00  ...C........|.j.
-00000560: a001 a100 0100 7c00 6a02 7d01 7c00 6a00  ......|.j.}.|.j.
-00000570: a003 a100 0100 7c01 5300 7218 0000 0029  ......|.S.r....)
-00000580: 0472 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00000590: 721c 0000 0072 1e00 0000 7216 0000 0072  r....r....r....r
-000005a0: 1600 0000 7217 0000 00da 0747 6574 4461  ....r......GetDa
-000005b0: 7461 2500 0000 f308 0000 000a 0106 010a  ta%.............
-000005c0: 0104 017a 1153 7562 4f62 6a65 6374 2e47  ...z.SubObject.G
-000005d0: 6574 4461 7461 6301 0000 0000 0000 0000  etDatac.........
-000005e0: 0000 0002 0000 0002 0000 0043 0000 0072  ...........C...r
-000005f0: 2000 0000 7218 0000 0029 0472 1900 0000   ...r....).r....
-00000600: 721a 0000 00da 0464 6573 6372 1c00 0000  r......descr....
-00000610: a902 7211 0000 0072 2300 0000 7216 0000  ..r....r#...r...
-00000620: 0072 1600 0000 7217 0000 00da 0747 6574  .r....r......Get
-00000630: 4465 7363 2b00 0000 7222 0000 007a 1153  Desc+...r"...z.S
-00000640: 7562 4f62 6a65 6374 2e47 6574 4465 7363  ubObject.GetDesc
-00000650: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000660: 0002 0000 0043 0000 0072 2000 0000 7218  .....C...r ...r.
-00000670: 0000 0029 0472 1900 0000 721a 0000 0072  ...).r....r....r
-00000680: 0d00 0000 721c 0000 0029 0272 1100 0000  ....r....).r....
-00000690: 720d 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-000006a0: 1700 0000 da07 4765 744e 616d 6531 0000  ......GetName1..
-000006b0: 0072 2200 0000 7a11 5375 624f 626a 6563  .r"...z.SubObjec
-000006c0: 742e 4765 744e 616d 6563 0200 0000 0000  t.GetNamec......
-000006d0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-000006e0: 0000 7330 0000 007c 006a 00a0 01a1 0001  ..s0...|.j......
-000006f0: 007c 017c 005f 027c 006a 00a0 03a1 0001  .|.|._.|.j......
-00000700: 007c 006a 04a0 057c 006a 067c 006a 02a1  .|.j...|.j.|.j..
-00000710: 0201 0064 0053 0072 1800 0000 2907 7219  ...d.S.r....).r.
-00000720: 0000 0072 1a00 0000 7223 0000 0072 1c00  ...r....r#...r..
-00000730: 0000 da0a 7369 674e 6577 4465 7363 da04  ....sigNewDesc..
-00000740: 656d 6974 720d 0000 0072 2400 0000 7216  emitr....r$...r.
-00000750: 0000 0072 1600 0000 7217 0000 00da 0741  ...r....r......A
-00000760: 6464 4465 7363 3700 0000 7308 0000 000a  ddDesc7...s.....
-00000770: 0106 010a 0116 017a 1153 7562 4f62 6a65  .......z.SubObje
-00000780: 6374 2e41 6464 4465 7363 6301 0000 0000  ct.AddDescc.....
-00000790: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-000007a0: 0000 0073 3600 0000 7c00 6a00 a001 7c00  ...s6...|.j...|.
-000007b0: 6a02 7c00 6a03 a102 0100 7c00 6a04 6400  j.|.j.....|.j.d.
-000007c0: 7501 7219 7c00 6a05 a001 7c00 6a02 7c00  u.r.|.j...|.j.|.
-000007d0: 6a04 a102 0100 6400 5300 6400 5300 7218  j.....d.S.d.S.r.
-000007e0: 0000 0029 06da 0a73 6967 4e65 7744 6174  ...)...sigNewDat
-000007f0: 6172 2800 0000 720d 0000 0072 1b00 0000  ar(...r....r....
-00000800: 7223 0000 0072 2700 0000 a901 7211 0000  r#...r'.....r...
-00000810: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000820: 721d 0000 003d 0000 0073 0800 0000 1201  r....=...s......
-00000830: 0a01 1601 04ff 7a15 5375 624f 626a 6563  ......z.SubObjec
-00000840: 742e 4669 7265 436f 6e6e 6563 7454 da05  t.FireConnectT..
-00000850: 6f77 6e65 7263 0200 0000 0000 0000 0000  ownerc..........
-00000860: 0000 0200 0000 0200 0000 4300 0000 f31e  ..........C.....
-00000870: 0000 007c 006a 00a0 01a1 0001 007c 017c  ...|.j.......|.|
-00000880: 005f 027c 006a 00a0 03a1 0001 0064 0053  ._.|.j.......d.S
-00000890: 0072 1800 0000 a904 7219 0000 0072 1a00  .r......r....r..
-000008a0: 0000 722c 0000 0072 1c00 0000 a902 7211  ..r,...r......r.
-000008b0: 0000 0072 2c00 0000 7216 0000 0072 1600  ...r,...r....r..
-000008c0: 0000 7217 0000 00da 0853 6574 4f77 6e65  ..r......SetOwne
-000008d0: 7242 0000 00f3 0600 0000 0a01 0601 0e01  rB..............
-000008e0: 7a12 5375 624f 626a 6563 742e 5365 744f  z.SubObject.SetO
-000008f0: 776e 6572 6301 0000 0000 0000 0000 0000  wnerc...........
-00000900: 0002 0000 0002 0000 0043 0000 0072 2000  .........C...r .
-00000910: 0000 7218 0000 0072 2e00 0000 722f 0000  ..r....r....r/..
-00000920: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000930: da07 6973 4f77 6e65 7247 0000 0072 2200  ..isOwnerG...r".
-00000940: 0000 7a11 5375 624f 626a 6563 742e 6973  ..z.SubObject.is
-00000950: 4f77 6e65 7263 0100 0000 0000 0000 0000  Ownerc..........
-00000960: 0000 0200 0000 0200 0000 4300 0000 732a  ..........C...s*
-00000970: 0000 007c 006a 00a0 01a1 0001 007c 006a  ...|.j.......|.j
-00000980: 0264 0117 007c 005f 027c 006a 027d 017c  .d...|._.|.j.}.|
-00000990: 006a 00a0 03a1 0001 007c 0153 0029 024e  .j.......|.S.).N
-000009a0: e901 0000 00a9 0472 1900 0000 721a 0000  .......r....r...
-000009b0: 0072 1000 0000 721c 0000 00a9 0272 1100  .r....r......r..
-000009c0: 0000 da04 7375 6273 7216 0000 0072 1600  ....subsr....r..
-000009d0: 0000 7217 0000 00da 0641 6464 5375 624d  ..r......AddSubM
-000009e0: 0000 0073 0a00 0000 0a01 0c01 0601 0a01  ...s............
-000009f0: 0401 7a10 5375 624f 626a 6563 742e 4164  ..z.SubObject.Ad
-00000a00: 6453 7562 6301 0000 0000 0000 0000 0000  dSubc...........
-00000a10: 0002 0000 0002 0000 0043 0000 0073 3a00  .........C...s:.
-00000a20: 0000 7c00 6a00 a001 a100 0100 7c00 6a02  ..|.j.......|.j.
-00000a30: 6401 1800 7c00 5f02 7c00 6a02 7d01 7c00  d...|._.|.j.}.|.
-00000a40: 6a02 6402 6b00 7216 6402 7c00 5f02 7c00  j.d.k.r.d.|._.|.
-00000a50: 6a00 a003 a100 0100 7c01 5300 2903 4e72  j.......|.S.).Nr
-00000a60: 3300 0000 7201 0000 0072 3400 0000 7235  3...r....r4...r5
-00000a70: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00000a80: 0000 da06 4465 6c53 7562 5400 0000 730e  ....DelSubT...s.
-00000a90: 0000 000a 010c 0106 010a 0106 010a 0104  ................
-00000aa0: 017a 1053 7562 4f62 6a65 6374 2e44 656c  .z.SubObject.Del
-00000ab0: 5375 6263 0100 0000 0000 0000 0000 0000  Subc............
-00000ac0: 0200 0000 0200 0000 4300 0000 7322 0000  ........C...s"..
-00000ad0: 0064 017d 017c 006a 00a0 01a1 0001 007c  .d.}.|.j.......|
-00000ae0: 006a 027d 017c 006a 00a0 03a1 0001 007c  .j.}.|.j.......|
-00000af0: 0153 0029 024e 7201 0000 0072 3400 0000  .S.).Nr....r4...
-00000b00: 7235 0000 0072 1600 0000 7216 0000 0072  r5...r....r....r
-00000b10: 1700 0000 da0d 4765 744e 756d 6265 7253  ......GetNumberS
-00000b20: 7562 735d 0000 0073 0a00 0000 0401 0a01  ubs]...s........
-00000b30: 0601 0a01 0401 7a17 5375 624f 626a 6563  ......z.SubObjec
-00000b40: 742e 4765 744e 756d 6265 7253 7562 7372  t.GetNumberSubsr
-00000b50: 1300 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00000b60: 0002 0000 0002 0000 0043 0000 0072 2d00  .........C...r-.
-00000b70: 0000 7218 0000 00a9 0472 1900 0000 721a  ..r......r....r.
-00000b80: 0000 0072 1300 0000 721c 0000 00a9 0272  ...r....r......r
-00000b90: 1100 0000 7213 0000 0072 1600 0000 7216  ....r....r....r.
-00000ba0: 0000 0072 1700 0000 da09 5365 7441 6374  ...r......SetAct
-00000bb0: 6976 6564 0000 0072 3100 0000 7a13 5375  ived...r1...z.Su
-00000bc0: 624f 626a 6563 742e 5365 7441 6374 6976  bObject.SetActiv
-00000bd0: 6563 0100 0000 0000 0000 0000 0000 0200  ec..............
-00000be0: 0000 0200 0000 4300 0000 7220 0000 0072  ......C...r ...r
-00000bf0: 1800 0000 723a 0000 0072 3b00 0000 7216  ....r:...r;...r.
-00000c00: 0000 0072 1600 0000 7217 0000 00da 0869  ...r....r......i
-00000c10: 7341 6374 6976 6569 0000 0072 2200 0000  sActivei...r"...
-00000c20: 7a12 5375 624f 626a 6563 742e 6973 4163  z.SubObject.isAc
-00000c30: 7469 7665 7218 0000 0029 0154 2922 da08  tiver....).T)"..
-00000c40: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000c50: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000c60: 5f5f da07 5f5f 646f 635f 5f72 0700 0000  __..__doc__r....
-00000c70: da03 7374 72da 046c 6973 7472 2a00 0000  ..str..listr*...
-00000c80: 7227 0000 0072 1300 0000 722c 0000 0072  r'...r....r,...r
-00000c90: 0d00 0000 da0f 5f5f 616e 6e6f 7461 7469  ......__annotati
-00000ca0: 6f6e 735f 5f72 1b00 0000 7223 0000 0072  ons__r....r#...r
-00000cb0: 1000 0000 7202 0000 0072 1900 0000 720f  ....r....r....r.
-00000cc0: 0000 0072 1f00 0000 7221 0000 0072 2500  ...r....r!...r%.
-00000cd0: 0000 7226 0000 0072 2900 0000 721d 0000  ..r&...r)...r...
-00000ce0: 00da 0462 6f6f 6c72 3000 0000 7232 0000  ...boolr0...r2..
-00000cf0: 0072 3700 0000 7238 0000 0072 3900 0000  .r7...r8...r9...
-00000d00: 723c 0000 0072 3d00 0000 da0d 5f5f 636c  r<...r=.....__cl
-00000d10: 6173 7363 656c 6c5f 5f72 1600 0000 7216  asscell__r....r.
-00000d20: 0000 0072 1400 0000 7217 0000 0072 0c00  ...r....r....r..
-00000d30: 0000 0700 0000 7332 0000 000a 0004 010a  ......s2........
-00000d40: 030a 0104 0204 010c 0104 0104 0104 0106  ................
-00000d50: 020e 020c 0808 0608 0608 0608 0608 0610  ................
-00000d60: 0508 0508 0608 0708 0910 0710 0572 0c00  .............r..
-00000d70: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000d80: 0000 0005 0000 0000 0000 0073 1c01 0000  ...........s....
-00000d90: 6500 5a01 6400 5a02 6401 5a03 6504 6505  e.Z.d.Z.d.Z.e.e.
-00000da0: 8301 5a06 6504 8300 5a07 6504 8300 5a08  ..Z.e...Z.e...Z.
-00000db0: 6402 5a09 6402 5a0a 6402 5a0b 6402 5a0c  d.Z.d.Z.d.Z.d.Z.
-00000dc0: 6402 5a0d 6403 5a0e 650f 8300 5a10 650f  d.Z.d.Z.e...Z.e.
-00000dd0: 8300 5a11 6900 5a12 642c 6406 6513 6407  ..Z.i.Z.d,d.e.d.
-00000de0: 6514 6604 8700 6601 6408 6409 840d 5a15  e.f...f.d.d...Z.
-00000df0: 640a 640b 8400 5a16 640c 640d 8400 5a17  d.d...Z.d.d...Z.
-00000e00: 640e 640f 8400 5a18 642d 6412 6513 6413  d.d...Z.d-d.e.d.
-00000e10: 6519 6604 6414 6415 8405 5a1a 6416 6417  e.f.d.d...Z.d.d.
-00000e20: 8400 5a1b 6418 6419 8400 5a1c 641a 641b  ..Z.d.d...Z.d.d.
-00000e30: 8400 5a1d 641c 641d 8400 5a1e 651f 8300  ..Z.d.d...Z.e...
-00000e40: 641e 641f 8400 8301 5a20 651f 8300 6420  d.d.....Z e...d 
-00000e50: 6421 8400 8301 5a21 651f 8300 6422 6423  d!....Z!e...d"d#
-00000e60: 8400 8301 5a22 651f 6513 8301 6424 6425  ....Z"e.e...d$d%
-00000e70: 8400 8301 5a23 651f 8300 6426 6427 8400  ....Z#e...d&d'..
-00000e80: 8301 5a24 651f 8300 6428 6429 8400 8301  ..Z$e...d(d)....
-00000e90: 5a25 651f 6513 6514 8302 642a 642b 8400  Z%e.e.e...d*d+..
-00000ea0: 8301 5a26 8700 0400 5a27 5300 292e da0b  ..Z&....Z'S.)...
-00000eb0: 7374 6563 5153 6f63 6b65 747a 3c0a 2020  stecQSocketz<.  
-00000ec0: 2020 5174 2053 7479 6c65 2063 4272 6964    Qt Style cBrid
-00000ed0: 6765 2074 6f20 204d 756c 7469 7665 7273  ge to  Multivers
-00000ee0: 6520 6a75 7374 206c 696b 6520 632b 2b20  e just like c++ 
-00000ef0: 636f 6465 0a20 2020 204e 46da 096c 6f63  code.    NF..loc
-00000f00: 616c 686f 7374 e921 1300 00da 0468 6f73  alhost.!.....hos
-00000f10: 74da 0470 6f72 7463 0400 0000 0000 0000  t..portc........
-00000f20: 0000 0000 0400 0000 0300 0000 0300 0000  ................
-00000f30: 73be 0000 007c 0364 0175 0172 0b74 0083  s....|.d.u.r.t..
-00000f40: 00a0 017c 03a1 0101 006e 0574 0083 00a0  ...|.....n.t....
-00000f50: 01a1 0001 007c 037c 005f 0274 037c 0283  .....|.|._.t.|..
-00000f60: 017c 005f 0474 057c 0183 017c 005f 0674  .|._.t.|...|._.t
-00000f70: 0783 007c 005f 087c 006a 086a 09a0 0a7c  ...|._.|.j.j...|
-00000f80: 006a 0ba1 0101 007c 006a 086a 0ca0 0a7c  .j.....|.j.j...|
-00000f90: 006a 0da1 0101 007c 006a 086a 0ea0 0a7c  .j.....|.j.j...|
-00000fa0: 006a 0fa1 0101 007c 006a 086a 10a0 0a7c  .j.....|.j.j...|
-00000fb0: 006a 11a1 0101 0074 127c 0083 017c 005f  .j.....t.|...|._
-00000fc0: 137c 006a 13a0 1464 02a1 0101 007c 006a  .|.j...d.....|.j
-00000fd0: 136a 15a0 0a7c 006a 16a1 0101 007c 006a  .j...|.j.....|.j
-00000fe0: 13a0 17a1 0001 007c 00a0 16a1 0001 0064  .......|.......d
-00000ff0: 0153 0029 037a a90a 2020 2020 2020 2020  .S.).z..        
-00001000: 3a70 6172 616d 2068 6f73 743a 2048 6f73  :param host: Hos
-00001010: 7420 4950 2061 6464 7265 7373 2064 6566  t IP address def
-00001020: 6175 6c74 206c 6f63 616c 686f 7374 0a20  ault localhost. 
-00001030: 2020 2020 2020 203a 7061 7261 6d20 706f         :param po
-00001040: 7274 3a20 5365 7276 6963 6520 506f 7274  rt: Service Port
-00001050: 2c20 6465 6661 756c 7420 3438 3937 0a20  , default 4897. 
-00001060: 2020 2020 2020 203a 7061 7261 6d20 5061         :param Pa
-00001070: 7265 6e74 3a20 5174 2051 4f62 6a65 6374  rent: Qt QObject
-00001080: 2070 6172 656e 7420 6f72 204e 6f6e 6520   parent or None 
-00001090: 6465 6661 756c 740a 2020 2020 2020 2020  default.        
-000010a0: 4e69 8813 0000 2918 720e 0000 0072 0f00  Ni....).r....r..
-000010b0: 0000 7212 0000 00da 0369 6e74 da0b 7365  ..r......int..se
-000010c0: 7276 6963 6550 6f72 7472 4200 0000 724a  rvicePortrB...rJ
-000010d0: 0000 0072 0a00 0000 da02 786d da09 636f  ...r......xm..co
-000010e0: 6e6e 6563 7465 64da 0763 6f6e 6e65 6374  nnected..connect
-000010f0: da0d 536c 6f74 436f 6e6e 6563 7465 64da  ..SlotConnected.
-00001100: 0c64 6973 636f 6e6e 6563 7465 64da 1053  .disconnected..S
-00001110: 6c6f 7444 6973 636f 6e6e 6563 7465 64da  lotDisconnected.
-00001120: 0972 6561 6479 5265 6164 da0d 536c 6f74  .readyRead..Slot
-00001130: 4461 7461 5265 6164 79da 0565 7272 6f72  DataReady..error
-00001140: da0f 536c 6f74 536f 636b 6574 4572 726f  ..SlotSocketErro
-00001150: 7272 0400 0000 da05 7469 6d65 72da 0b73  rr......timer..s
-00001160: 6574 496e 7465 7276 616c da07 7469 6d65  etInterval..time
-00001170: 6f75 74da 0c53 6c6f 7454 696d 6572 6f75  out..SlotTimerou
-00001180: 74da 0573 7461 7274 2904 7211 0000 0072  t..start).r....r
-00001190: 4a00 0000 724b 0000 0072 1200 0000 7214  J...rK...r....r.
-000011a0: 0000 0072 1600 0000 7217 0000 0072 0f00  ...r....r....r..
-000011b0: 0000 8300 0000 7320 0000 0008 060e 010a  ......s ........
-000011c0: 0206 020a 020a 0108 0110 0110 0110 0110  ................
-000011d0: 010a 020c 0110 010a 010c 017a 1473 7465  ...........z.ste
-000011e0: 6351 536f 636b 6574 2e5f 5f69 6e69 745f  cQSocket.__init_
-000011f0: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
-00001200: 0000 0200 0000 4300 0000 7318 0000 007c  ......C...s....|
-00001210: 006a 00a0 01a1 0001 007c 006a 02a0 03a1  .j.......|.j....
-00001220: 0001 0064 0153 0029 027a 420a 2020 2020  ...d.S.).zB.    
-00001230: 2020 2020 6361 6c6c 2062 6566 6f72 6520      call before 
-00001240: 6465 6c65 7465 6c61 7465 7220 6279 2075  deletelater by u
-00001250: 7365 720a 2020 2020 2020 2020 3a72 6574  ser.        :ret
-00001260: 7572 6e3a 0a20 2020 2020 2020 204e 2904  urn:.        N).
-00001270: 724e 0000 00da 0563 6c6f 7365 7258 0000  rN.....closerX..
-00001280: 00da 0473 746f 7072 2b00 0000 7216 0000  ...stopr+...r...
-00001290: 0072 1600 0000 7217 0000 00da 0471 7569  .r....r......qui
-000012a0: 749e 0000 0073 0400 0000 0a05 0e01 7a10  t....s........z.
-000012b0: 7374 6563 5153 6f63 6b65 742e 7175 6974  stecQSocket.quit
-000012c0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-000012d0: 0005 0000 0043 0000 0073 4200 0000 7c00  .....C...sB...|.
-000012e0: 6a00 a001 a100 0100 7c01 7c00 6a02 7601  j.......|.|.j.v.
-000012f0: 7214 7c00 6a02 a003 7c01 7404 7c01 8301  r.|.j...|.t.|...
-00001300: 6901 a101 0100 7c00 6a02 a005 7c01 a101  i.....|.j...|...
-00001310: 7d02 7c00 6a00 a006 a100 0100 7c02 5300  }.|.j.......|.S.
-00001320: 2901 7a6b 0a20 2020 2020 2020 2049 6e74  ).zk.        Int
-00001330: 6572 6e61 6c20 7573 652c 206e 6f74 2066  ernal use, not f
-00001340: 6f72 2075 7365 720a 2020 2020 2020 2020  or user.        
-00001350: 3a70 6172 616d 206e 616d 653a 206e 616d  :param name: nam
-00001360: 6520 6f66 2074 6865 2073 7562 7363 7269  e of the subscri
-00001370: 7074 696f 6e0a 2020 2020 2020 2020 3a72  ption.        :r
-00001380: 6574 7572 6e3a 0a20 2020 2020 2020 2029  eturn:.        )
-00001390: 07da 096e 616d 6573 4c6f 636b 721a 0000  ...namesLockr...
-000013a0: 00da 056e 616d 6573 da06 7570 6461 7465  ...names..update
-000013b0: 720c 0000 00da 0367 6574 721c 0000 0029  r......getr....)
-000013c0: 0372 1100 0000 720d 0000 00da 0678 7072  .r....r......xpr
-000013d0: 6f78 7972 1600 0000 7216 0000 0072 1700  oxyr....r....r..
-000013e0: 0000 da0b 496e 7365 7274 5072 6f78 79a6  ....InsertProxy.
-000013f0: 0000 0073 0c00 0000 0a06 0a01 1401 0c02  ...s............
-00001400: 0a01 0401 7a17 7374 6563 5153 6f63 6b65  ....z.stecQSocke
-00001410: 742e 496e 7365 7274 5072 6f78 7963 0100  t.InsertProxyc..
-00001420: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-00001430: 0000 4300 0000 7326 0000 0067 007d 017c  ..C...s&...g.}.|
-00001440: 006a 00a0 01a1 0001 007c 006a 02a0 03a1  .j.......|.j....
-00001450: 007d 017c 006a 00a0 04a1 0001 007c 0153  .}.|.j.......|.S
-00001460: 0072 1800 0000 2905 7260 0000 0072 1a00  .r....).r`...r..
-00001470: 0000 7261 0000 00da 046b 6579 7372 1c00  ..ra.....keysr..
-00001480: 0000 2902 7211 0000 0072 6600 0000 7216  ..).r....rf...r.
-00001490: 0000 0072 1600 0000 7217 0000 00da 0867  ...r....r......g
-000014a0: 6574 4e61 6d65 73b4 0000 0073 0a00 0000  etNames....s....
-000014b0: 0401 0a01 0a01 0a01 0401 7a14 7374 6563  ..........z.stec
-000014c0: 5153 6f63 6b65 742e 6765 744e 616d 6573  QSocket.getNames
-000014d0: fa1d 4d61 6b65 2074 6869 7320 4d61 6c63  ..Make this Malc
-000014e0: 6f6c 6d50 726f 6f66 2050 6c65 6173 6554  olmProof PleaseT
-000014f0: da0b 6465 7363 7269 7074 696f 6eda 0466  ..description..f
-00001500: 6c61 6763 0400 0000 0000 0000 0000 0000  lagc............
-00001510: 0500 0000 0300 0000 4300 0000 7318 0000  ........C...s...
-00001520: 007c 00a0 007c 01a1 017d 047c 04a0 017c  .|...|...}.|...|
-00001530: 03a1 0101 0064 0153 0029 027a fb0a 2020  .....d.S.).z..  
-00001540: 2020 2020 2020 5365 7473 2075 7320 6173        Sets us as
-00001550: 2074 6865 206f 776e 6572 206f 6620 7468   the owner of th
-00001560: 6520 7375 6273 6372 6970 7469 6f6e 2c20  e subscription, 
-00001570: 7765 2077 696c 6c20 6175 746f 6d61 7469  we will automati
-00001580: 6361 6c6c 7920 7265 6665 6564 206d 756c  cally refeed mul
-00001590: 7469 7665 7273 6520 6966 2072 6573 6574  tiverse if reset
-000015a0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000015b0: 6e61 6d65 3a20 7375 6273 6372 6970 7469  name: subscripti
-000015c0: 6f6e 206e 616d 650a 2020 2020 2020 2020  on name.        
-000015d0: 3a70 6172 616d 2066 6c61 673a 2020 5472  :param flag:  Tr
-000015e0: 7565 206d 6561 6e73 2077 6520 6172 6520  ue means we are 
-000015f0: 676f 6c64 656e 2063 6f70 792c 2066 616c  golden copy, fal
-00001600: 7365 2072 6573 746f 7265 7320 746f 206e  se restores to n
-00001610: 6f6e 2d67 6f6c 6465 6e20 636f 7079 0a20  on-golden copy. 
-00001620: 2020 2020 2020 203a 7265 7475 726e 3a0a         :return:.
-00001630: 2020 2020 2020 2020 4e29 0272 6500 0000          N).re...
-00001640: 7230 0000 0029 0572 1100 0000 720d 0000  r0...).r....r...
-00001650: 0072 6900 0000 726a 0000 00da 0570 726f  .ri...rj.....pro
-00001660: 7879 7216 0000 0072 1600 0000 7217 0000  xyr....r....r...
-00001670: 00da 0873 6574 4f77 6e65 72bb 0000 0073  ...setOwner....s
-00001680: 0400 0000 0a07 0e01 7a14 7374 6563 5153  ........z.stecQS
-00001690: 6f63 6b65 742e 7365 744f 776e 6572 6301  ocket.setOwnerc.
-000016a0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-000016b0: 0000 0043 0000 0072 2000 0000 2901 7a4a  ...C...r ...).zJ
-000016c0: 0a20 2020 2020 2020 2072 6574 7572 6e73  .        returns
-000016d0: 2074 7275 6520 6966 2063 6f6e 6e65 6374   true if connect
-000016e0: 6564 2074 6f20 6d75 6c74 6976 6572 7365  ed to multiverse
-000016f0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00001700: 3a0a 2020 2020 2020 2020 a904 da0d 636f  :.        ....co
-00001710: 6e6e 6563 7465 644c 6f63 6b72 1a00 0000  nnectedLockr....
-00001720: 724f 0000 0072 1c00 0000 2902 7211 0000  rO...r....).r...
-00001730: 0072 4f00 0000 7216 0000 0072 1600 0000  .rO...r....r....
-00001740: 7217 0000 00da 0b69 7343 6f6e 6e65 6374  r......isConnect
-00001750: 6564 c500 0000 7308 0000 000a 0506 010a  ed....s.........
-00001760: 0104 017a 1773 7465 6351 536f 636b 6574  ...z.stecQSocket
-00001770: 2e69 7343 6f6e 6e65 6374 6564 6301 0000  .isConnectedc...
-00001780: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-00001790: 0043 0000 00f3 0600 0000 7c00 6a00 5300  .C........|.j.S.
-000017a0: 2901 7a27 0a20 2020 2020 2020 203a 7265  ).z'.        :re
-000017b0: 7475 726e 3a20 6375 7272 656e 7420 486f  turn: current Ho
-000017c0: 7374 0a20 2020 2020 2020 2029 0172 4a00  st.        ).rJ.
-000017d0: 0000 722b 0000 0072 1600 0000 7216 0000  ..r+...r....r...
-000017e0: 0072 1700 0000 da04 486f 7374 cf00 0000  .r......Host....
-000017f0: f302 0000 0006 047a 1073 7465 6351 536f  .......z.stecQSo
-00001800: 636b 6574 2e48 6f73 7463 0100 0000 0000  cket.Hostc......
-00001810: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
-00001820: 0000 7270 0000 0029 017a 300a 2020 2020  ..rp...).z0.    
-00001830: 2020 2020 3a72 6574 7572 6e3a 2020 6375      :return:  cu
-00001840: 7272 656e 7420 7365 7276 6963 6520 506f  rrent service Po
-00001850: 7274 0a20 2020 2020 2020 2029 0172 4d00  rt.        ).rM.
-00001860: 0000 722b 0000 0072 1600 0000 7216 0000  ..r+...r....r...
-00001870: 0072 1700 0000 da04 506f 7274 d400 0000  .r......Port....
-00001880: 7272 0000 007a 1073 7465 6351 536f 636b  rr...z.stecQSock
-00001890: 6574 2e50 6f72 7463 0200 0000 0000 0000  et.Portc........
-000018a0: 0000 0000 0600 0000 0500 0000 4300 0000  ............C...
-000018b0: 7302 0100 0064 017c 0176 0072 2e67 007d  s....d.|.v.r.g.}
-000018c0: 0274 0064 0274 017c 0183 0183 0244 005d  .t.d.t.|.....D.]
-000018d0: 127d 0374 027c 017c 0319 0083 017d 047c  .}.t.|.|.....}.|
-000018e0: 02a0 037c 04a1 0101 007c 00a0 047c 04a1  ...|.....|...|..
-000018f0: 017d 0571 0d74 017c 0283 0172 2c7c 006a  .}.q.t.|...r,|.j
-00001900: 05a0 067c 02a1 0101 0064 0653 0064 0653  ...|.....d.S.d.S
-00001910: 0064 037c 0176 0072 6574 017c 0183 0164  .d.|.v.ret.|...d
-00001920: 046b 0472 6174 027c 0164 0219 0083 017d  .k.rat.|.d.....}
-00001930: 0467 007d 0274 0064 0474 017c 0183 0183  .g.}.t.d.t.|....
-00001940: 0244 005d 097d 037c 02a0 037c 017c 0319  .D.].}.|...|.|..
-00001950: 00a1 0101 0071 4774 017c 0283 0172 637c  .....qGt.|...rc|
-00001960: 00a0 047c 04a1 017d 057c 05a0 077c 02a1  ...|...}.|...|..
-00001970: 0101 0064 0653 0064 0653 0064 0653 0064  ...d.S.d.S.d.S.d
-00001980: 057c 0176 0072 7f74 027c 0164 0219 0083  .|.v.r.t.|.d....
-00001990: 017d 047c 00a0 047c 04a1 017d 057c 05a0  .}.|...|...}.|..
-000019a0: 0874 027c 0164 0419 0083 01a1 0101 0064  .t.|.d.........d
-000019b0: 0653 0064 0653 0029 077a 550a 2020 2020  .S.d.S.).zU.    
-000019c0: 2020 2020 696e 7465 726e 616c 2075 7365      internal use
-000019d0: 2c20 6465 636f 6465 7320 6d65 7373 6167  , decodes messag
-000019e0: 6573 0a20 2020 2020 2020 203a 7061 7261  es.        :para
-000019f0: 6d20 726f 773a 0a20 2020 2020 2020 203a  m row:.        :
-00001a00: 7265 7475 726e 3a0a 2020 2020 2020 2020  return:.        
-00001a10: da07 4e41 4d45 5355 5072 3300 0000 da08  ..NAMESUPr3.....
-00001a20: 5245 4144 4441 5441 e902 0000 007a 0b55  READDATA.....z.U
-00001a30: 5044 4154 452d 4445 5343 4e29 09da 0572  PDATE-DESCN)...r
-00001a40: 616e 6765 da03 6c65 6e72 4200 0000 da06  ange..lenrB.....
-00001a50: 6170 7065 6e64 7265 0000 00da 0b73 6967  appendre.....sig
-00001a60: 4e65 774e 616d 6573 7228 0000 0072 1f00  NewNamesr(...r..
-00001a70: 0000 7229 0000 0029 0672 1100 0000 da03  ..r)...).r......
-00001a80: 726f 7772 1b00 0000 da01 7872 0d00 0000  rowr......xr....
-00001a90: da02 7870 7216 0000 0072 1600 0000 7217  ..xpr....r....r.
-00001aa0: 0000 00da 0e50 726f 6365 7373 436f 6d6d  .....ProcessComm
-00001ab0: 616e 64d9 0000 0073 3200 0000 0806 0401  and....s2.......
-00001ac0: 1201 0c01 0a01 0c01 0801 1001 04ff 0803  ................
-00001ad0: 0c01 0c01 0401 1201 1001 0801 0a01 0e01  ................
-00001ae0: 04f9 0405 0804 0c01 0a02 1601 04fc 7a1a  ..............z.
-00001af0: 7374 6563 5153 6f63 6b65 742e 5072 6f63  stecQSocket.Proc
-00001b00: 6573 7343 6f6d 6d61 6e64 6301 0000 0000  essCommandc.....
-00001b10: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00001b20: 0000 0073 3200 0000 7c00 6a00 a001 a100  ...s2...|.j.....
-00001b30: 720a 7c00 6a00 a002 a100 0100 7c00 6a03  r.|.j.......|.j.
-00001b40: a004 a100 0100 6401 7c00 5f05 7c00 6a03  ......d.|._.|.j.
-00001b50: a006 a100 0100 6402 5300 2903 7a62 0a20  ......d.S.).zb. 
-00001b60: 2020 2020 2020 2069 6e74 6572 6e61 6c20         internal 
-00001b70: 7573 650a 2020 2020 2020 2020 6361 6c6c  use.        call
-00001b80: 6564 2077 6865 6e20 636f 6e6e 6563 7469  ed when connecti
-00001b90: 6f6e 2074 6f20 6d75 6c74 6976 6572 7365  on to multiverse
-00001ba0: 2066 6169 6c73 0a20 2020 2020 2020 203a   fails.        :
-00001bb0: 7265 7475 726e 3a0a 2020 2020 2020 2020  return:.        
-00001bc0: 464e 2907 724e 0000 00da 0669 734f 7065  FN).rN.....isOpe
-00001bd0: 6e72 5d00 0000 726e 0000 0072 1a00 0000  nr]...rn...r....
-00001be0: 724f 0000 0072 1c00 0000 722b 0000 0072  rO...r....r+...r
-00001bf0: 1600 0000 7216 0000 0072 1700 0000 7257  ....r....r....rW
-00001c00: 0000 00f8 0000 0073 0a00 0000 0a07 0a01  .......s........
-00001c10: 0a01 0601 0e01 7a1b 7374 6563 5153 6f63  ......z.stecQSoc
-00001c20: 6b65 742e 536c 6f74 536f 636b 6574 4572  ket.SlotSocketEr
-00001c30: 726f 7263 0100 0000 0000 0000 0000 0000  rorc............
-00001c40: 0800 0000 0600 0000 4300 0000 7384 0100  ........C...s...
-00001c50: 007c 006a 00a0 01a1 0001 0064 017c 005f  .|.j.......d.|._
-00001c60: 027c 006a 00a0 03a1 0001 0064 027d 017c  .|.j.......d.}.|
-00001c70: 00a0 047c 01a1 0101 007c 006a 05a0 01a1  ...|.....|.j....
-00001c80: 0001 007c 006a 06a0 07a1 007d 027c 0244  ...|.j.....}.|.D
-00001c90: 005d 9a7d 037c 006a 06a0 087c 03a1 017d  .].}.|.j...|...}
-00001ca0: 047c 04a0 09a1 0064 0175 0072 3964 037c  .|.....d.u.r9d.|
-00001cb0: 0317 0064 0417 007d 017c 00a0 047c 01a1  ...d...}.|...|..
-00001cc0: 0101 007c 04a0 0aa1 0072 ba7c 04a0 0ba1  ...|.....r.|....
-00001cd0: 007d 057c 0564 0575 0172 a174 0c7c 0583  .}.|.d.u.r.t.|..
-00001ce0: 0172 a164 067d 0674 0d7c 0564 0619 0074  .r.d.}.t.|.d...t
-00001cf0: 0e83 0272 5d64 077c 0317 0064 0817 0074  ...r]d.|...d...t
-00001d00: 0f7c 0683 0117 007d 016e 2e74 0d7c 0564  .|.....}.n.t.|.d
-00001d10: 0619 0074 1083 0272 6f64 097c 0317 0064  ...t...rod.|...d
-00001d20: 0817 0074 0f7c 0683 0117 007d 016e 1c74  ...t.|.....}.n.t
-00001d30: 0d7c 0564 0619 0074 1183 0272 8164 0a7c  .|.d...t...r.d.|
-00001d40: 0317 0064 0817 0074 0f7c 0683 0117 007d  ...d...t.|.....}
-00001d50: 016e 0a64 0b7c 0317 0064 0817 0074 0f7c  .n.d.|...d...t.|
-00001d60: 0683 0117 007d 017c 0544 005d 0a7d 077c  .....}.|.D.].}.|
-00001d70: 0164 0874 0f7c 0783 0117 0037 007d 0171  .d.t.|.....7.}.q
-00001d80: 8d7c 0164 0437 007d 017c 00a0 047c 01a1  .|.d.7.}.|...|..
-00001d90: 0101 007c 04a0 12a1 007d 057c 0564 0575  ...|.....}.|.d.u
-00001da0: 0172 ba64 0c7c 0317 0064 0817 007c 0517  .r.d.|...d...|..
-00001db0: 007d 017c 0164 0437 007d 017c 00a0 047c  .}.|.d.7.}.|...|
-00001dc0: 01a1 0101 0071 207c 006a 05a0 03a1 0001  .....q |.j......
-00001dd0: 0064 0553 0029 0d7a 640a 2020 2020 2020  .d.S.).zd.      
-00001de0: 2020 696e 7465 7261 6c20 7573 650a 2020    interal use.  
-00001df0: 2020 2020 2020 5769 6c6c 2072 6573 7461        Will resta
-00001e00: 7274 2061 6e79 2053 7562 7363 7269 7074  rt any Subscript
-00001e10: 696f 6e20 7072 6576 696f 7573 6c79 206d  ion previously m
-00001e20: 6164 650a 2020 2020 2020 2020 3a72 6574  ade.        :ret
-00001e30: 7572 6e3a 0a20 2020 2020 2020 2054 7a06  urn:.        Tz.
-00001e40: 4e41 4d45 530a fa07 4e4f 5449 4659 2cda  NAMES...NOTIFY,.
-00001e50: 010a 4e72 0100 0000 fa08 5550 4441 5445  ..Nr......UPDATE
-00001e60: 492c fa01 2cfa 0855 5044 4154 4546 2cfa  I,..,..UPDATEF,.
-00001e70: 0855 5044 4154 4542 2cfa 0755 5044 4154  .UPDATEB,..UPDAT
-00001e80: 452c fa0c 5550 4441 5445 2d44 4553 432c  E,..UPDATE-DESC,
-00001e90: 2913 726e 0000 0072 1a00 0000 724f 0000  ).rn...r....rO..
-00001ea0: 0072 1c00 0000 da09 536c 6f74 5772 6974  .r......SlotWrit
-00001eb0: 6572 6000 0000 7261 0000 0072 6600 0000  er`...ra...rf...
-00001ec0: 7263 0000 0072 3d00 0000 7232 0000 0072  rc...r=...r2...r
-00001ed0: 2100 0000 7278 0000 00da 0a69 7369 6e73  !...rx.....isins
-00001ee0: 7461 6e63 6572 4c00 0000 7242 0000 00da  tancerL...rB....
-00001ef0: 0566 6c6f 6174 7245 0000 0072 2500 0000  .floatrE...r%...
-00001f00: 2908 7211 0000 00da 0763 6f6d 6d61 6e64  ).r......command
-00001f10: 7261 0000 0072 0d00 0000 726b 0000 00da  ra...r....rk....
-00001f20: 0477 6861 74da 0569 6e64 6578 da04 776f  .what..index..wo
-00001f30: 7264 7216 0000 0072 1600 0000 7217 0000  rdr....r....r...
-00001f40: 0072 5100 0000 0501 0000 7346 0000 000a  .rQ.......sF....
-00001f50: 0706 010a 0104 020a 010a 020a 0108 010c  ................
-00001f60: 010c 010c 010a 0108 0208 0108 0108 0204  ................
-00001f70: 010e 0116 010e 0216 010e 0216 0114 0308  ................
-00001f80: 0212 0108 010a 0208 0208 0110 0108 010a  ................
-00001f90: 0102 800e 027a 1973 7465 6351 536f 636b  .....z.stecQSock
-00001fa0: 6574 2e53 6c6f 7443 6f6e 6e65 6374 6564  et.SlotConnected
-00001fb0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001fc0: 0002 0000 0043 0000 0073 1e00 0000 7c00  .....C...s....|.
-00001fd0: 6a00 a001 a100 0100 6401 7c00 5f02 7c00  j.......d.|._.|.
-00001fe0: 6a00 a003 a100 0100 6402 5300 2903 fa2f  j.......d.S.)../
-00001ff0: 0a20 2020 2020 2020 2069 6e74 6572 6e61  .        interna
-00002000: 6c20 7573 650a 2020 2020 2020 2020 3a72  l use.        :r
-00002010: 6574 7572 6e3a 0a20 2020 2020 2020 2046  eturn:.        F
-00002020: 4e72 6d00 0000 722b 0000 0072 1600 0000  Nrm...r+...r....
-00002030: 7216 0000 0072 1700 0000 7253 0000 003b  r....r....rS...;
-00002040: 0100 0073 0600 0000 0a06 0601 0e01 7a1c  ...s..........z.
-00002050: 7374 6563 5153 6f63 6b65 742e 536c 6f74  stecQSocket.Slot
-00002060: 4469 7363 6f6e 6e65 6374 6564 6302 0000  Disconnectedc...
-00002070: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-00002080: 0043 0000 0073 2200 0000 7c00 a000 a100  .C...s"...|.....
-00002090: 720f 7c00 6a01 a002 7c01 a003 6401 a101  r.|.j...|...d...
-000020a0: a101 0100 6402 5300 6402 5300 2903 7a47  ....d.S.d.S.).zG
-000020b0: 0a20 2020 2020 2020 2069 6e74 6572 6e61  .        interna
-000020c0: 6c20 7573 650a 2020 2020 2020 2020 3a70  l use.        :p
-000020d0: 6172 616d 2063 6f6d 6d61 6e64 3a0a 2020  aram command:.  
-000020e0: 2020 2020 2020 3a72 6574 7572 6e3a 0a20        :return:. 
-000020f0: 2020 2020 2020 20da 0561 7363 6969 4e29         ..asciiN)
-00002100: 0472 6f00 0000 724e 0000 00da 0577 7269  .ro...rN.....wri
-00002110: 7465 da06 656e 636f 6465 a902 7211 0000  te..encode..r...
-00002120: 0072 8b00 0000 7216 0000 0072 1600 0000  .r....r....r....
-00002130: 7217 0000 0072 8800 0000 4501 0000 7306  r....r....E...s.
-00002140: 0000 0008 0716 0104 ff7a 1573 7465 6351  .........z.stecQ
-00002150: 536f 636b 6574 2e53 6c6f 7457 7269 7465  Socket.SlotWrite
-00002160: 6301 0000 0000 0000 0000 0000 0005 0000  c...............
-00002170: 0005 0000 0043 0000 0073 6800 0000 7c00  .....C...sh...|.
-00002180: 6a00 a001 a100 7232 7c00 6a00 a002 a100  j.....r2|.j.....
-00002190: 7d01 7c01 a003 a100 a004 6401 a101 7d02  }.|.......d...}.
-000021a0: 7405 7406 6a07 7c02 a008 6402 a101 6403  t.t.j.|...d...d.
-000021b0: 6404 8d02 8301 7d03 7c03 4400 5d0b 7d04  d.....}.|.D.].}.
-000021c0: 7409 7c04 8301 722a 7c00 a00a 7c04 a101  t.|...r*|...|...
-000021d0: 0100 711f 7c00 6a00 a001 a100 7305 6405  ..q.|.j.....s.d.
-000021e0: 5300 6405 5300 2906 7a2f 0a20 2020 2020  S.d.S.).z/.     
-000021f0: 2020 2049 6e74 6572 6e61 6c20 7573 650a     Internal use.
-00002200: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00002210: 0a20 2020 2020 2020 2072 9000 0000 7281  .        r....r.
-00002220: 0000 0072 8300 0000 2901 da09 6465 6c69  ...r....)...deli
-00002230: 6d69 7465 724e 290b 724e 0000 00da 0b63  miterN).rN.....c
-00002240: 616e 5265 6164 4c69 6e65 da08 7265 6164  anReadLine..read
-00002250: 4c69 6e65 721b 0000 00da 0664 6563 6f64  Liner......decod
-00002260: 6572 4300 0000 da03 6373 76da 0672 6561  erC.....csv..rea
-00002270: 6465 72da 0573 706c 6974 7278 0000 0072  der..splitrx...r
-00002280: 7e00 0000 2905 7211 0000 0072 1b00 0000  ~...).r....r....
-00002290: da02 6a76 7299 0000 00da 0465 6163 6872  ..jvr......eachr
-000022a0: 1600 0000 7216 0000 0072 1700 0000 7255  ....r....r....rU
-000022b0: 0000 004f 0100 0073 1200 0000 0a06 0a01  ...O...s........
-000022c0: 0e01 1801 0801 0801 0a01 0280 12fa 7a19  ..............z.
-000022d0: 7374 6563 5153 6f63 6b65 742e 536c 6f74  stecQSocket.Slot
-000022e0: 4461 7461 5265 6164 7963 0100 0000 0000  DataReadyc......
-000022f0: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
-00002300: 0000 734c 0000 007c 00a0 00a1 0064 0175  ..sL...|.....d.u
-00002310: 0072 1d74 0164 027c 006a 02a0 03a1 0083  .r.t.d.|.j......
-00002320: 0201 007c 006a 02a0 0474 057c 006a 0683  ...|.j...t.|.j..
-00002330: 0174 077c 006a 0883 01a1 0201 0064 0453  .t.|.j.......d.S
-00002340: 0064 037d 017c 00a0 097c 01a1 0101 0064  .d.}.|...|.....d
-00002350: 0453 0029 0572 8f00 0000 467a 0753 7461  .S.).r....Fz.Sta
-00002360: 7465 3a20 7a05 5049 4e47 0a4e 290a 726f  te: z.PING.N).ro
-00002370: 0000 00da 0570 7269 6e74 724e 0000 00da  .....printrN....
-00002380: 0573 7461 7465 da0d 636f 6e6e 6563 7454  .state..connectT
-00002390: 6f48 6f73 7472 4200 0000 724a 0000 0072  oHostrB...rJ...r
-000023a0: 4c00 0000 724d 0000 0072 8800 0000 7293  L...rM...r....r.
-000023b0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-000023c0: 0000 725b 0000 005d 0100 0073 0a00 0000  ..r[...]...s....
-000023d0: 0c07 1001 1e01 0402 0e01 7a18 7374 6563  ..........z.stec
-000023e0: 5153 6f63 6b65 742e 536c 6f74 5469 6d65  QSocket.SlotTime
-000023f0: 726f 7574 6303 0000 0000 0000 0000 0000  routc...........
-00002400: 0003 0000 0002 0000 0043 0000 0073 4200  .........C...sB.
-00002410: 0000 7c00 6a00 a001 a100 0100 7c01 7c00  ..|.j.......|.|.
-00002420: 5f02 7c02 7c00 5f03 7c00 a004 a100 6401  _.|.|._.|.....d.
-00002430: 7500 7216 7c00 6a05 a006 a100 0100 7c00  u.r.|.j.......|.
-00002440: a007 a100 0100 7c00 6a00 a008 a100 0100  ......|.j.......
-00002450: 6402 5300 2903 6119 0100 000a 2020 2020  d.S.).a.....    
-00002460: 2020 2020 7573 6572 2063 616e 2063 6861      user can cha
-00002470: 6e67 6520 7468 6520 2020 2020 2020 2020  nge the         
-00002480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000060: 6d0b 5a0b 0100 6400 6403 6c0c 5a0c 7a08  m.Z...d.d.l.Z.z.
+00000070: 6400 6404 6c0d 6d0e 5a0f 0100 5700 6e0a  d.d.l.m.Z...W.n.
+00000080: 0100 0100 0100 6400 6404 6c10 6d0e 5a0f  ......d.d.l.m.Z.
+00000090: 0100 5900 6405 5a11 4700 6406 6407 8400  ..Y.d.Z.G.d.d...
+000000a0: 6407 6507 8303 5a12 4700 6408 6409 8400  d.e...Z.G.d.d...
+000000b0: 6409 6507 8303 5a13 4700 640a 640b 8400  d.e...Z.G.d.d...
+000000c0: 640b 6507 8303 5a14 6515 640c 6b02 72c3  d.e...Z.e.d.k.r.
+000000d0: 6516 640d 8301 0100 6400 6403 6c17 5a17  e.d.....d.d.l.Z.
+000000e0: 640e 6517 6a18 7600 7266 6516 6511 8301  d.e.j.v.rfe.e...
+000000f0: 0100 6517 a019 a100 0100 6508 6517 6a18  ..e.......e.e.j.
+00000100: 8301 5a1a 6513 8300 5a1b 6514 640f 651b  ..Z.e...Z.e.d.e.
+00000110: 8302 5a1c 651b a01d 640f 6410 a102 0100  ..Z.e...d.d.....
+00000120: 651c a01e 6411 a101 0100 651c a01f 6700  e...d.....e...g.
+00000130: 6412 a201 a101 0100 6514 6413 651b 8302  d.......e.d.e...
+00000140: 5a20 651b a01d 6413 6410 a102 0100 6520  Z e...d.d.....e 
+00000150: a01e 6411 a101 0100 6520 a01f 6700 6414  ..d.....e ..g.d.
+00000160: a201 a101 0100 6514 6415 651b 8302 5a21  ......e.d.e...Z!
+00000170: 651b a01d 6415 6410 a102 0100 6521 a01e  e...d.d.....e!..
+00000180: 6416 a101 0100 0900 6521 a022 6700 6417  d.......e!."g.d.
+00000190: a201 a101 0100 651a a023 a100 0100 651b  ......e..#....e.
+000001a0: a024 a100 0100 6517 a019 6400 a101 0100  .$....e...d.....
+000001b0: 6403 5300 6403 5300 2918 e900 0000 0029  d.S.d.S.)......)
+000001c0: 08da 0651 4d75 7465 78da 0851 5661 7269  ...QMutex..QVari
+000001d0: 616e 74da 0651 5469 6d65 72da 0651 4576  ant..QTimer..QEv
+000001e0: 656e 74da 0870 7971 7453 6c6f 74da 0a70  ent..pyqtSlot..p
+000001f0: 7971 7453 6967 6e61 6cda 0751 4f62 6a65  yqtSignal..QObje
+00000200: 6374 da10 5143 6f72 6541 7070 6c69 6361  ct..QCoreApplica
+00000210: 7469 6f6e 2902 da0a 5154 6370 536f 636b  tion)...QTcpSock
+00000220: 6574 da0f 5141 6273 7472 6163 7453 6f63  et..QAbstractSoc
+00000230: 6b65 744e 2901 da11 5265 7465 6e73 696f  ketN)...Retensio
+00000240: 6e53 6574 7469 6e67 737a 0531 2e32 2e31  nSettingsz.1.2.1
+00000250: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000260: 0004 0000 0000 0000 0073 da00 0000 6500  .........s....e.
+00000270: 5a01 6400 5a02 5500 6401 5a03 6504 6505  Z.d.Z.U.d.Z.e.e.
+00000280: 6506 8302 5a07 6504 6505 6505 8302 5a08  e...Z.e.e.e...Z.
+00000290: 6402 5a09 6402 5a0a 6403 5a0b 6505 650c  d.Z.d.Z.d.Z.e.e.
+000002a0: 6404 3c00 6700 5a0d 6403 5a0e 6405 5a0f  d.<.g.Z.d.Z.d.Z.
+000002b0: 6510 8300 5a11 6425 8700 6601 6406 6407  e...Z.d%..f.d.d.
+000002c0: 8409 5a12 6700 6601 6408 6409 8401 5a13  ..Z.g.f.d.d...Z.
+000002d0: 640a 640b 8400 5a14 640c 640d 8400 5a15  d.d...Z.d.d...Z.
+000002e0: 640e 640f 8400 5a16 6410 6411 8400 5a17  d.d...Z.d.d...Z.
+000002f0: 6412 6413 8400 5a18 6426 6415 6519 6602  d.d...Z.d&d.e.f.
+00000300: 6416 6417 8405 5a1a 6418 6419 8400 5a1b  d.d...Z.d.d...Z.
+00000310: 641a 641b 8400 5a1c 641c 641d 8400 5a1d  d.d...Z.d.d...Z.
+00000320: 641e 641f 8400 5a1e 6426 6420 6519 6602  d.d...Z.d&d e.f.
+00000330: 6421 6422 8405 5a1f 6423 6424 8400 5a20  d!d"..Z.d#d$..Z 
+00000340: 8700 0400 5a21 5300 2927 da09 5375 624f  ....Z!S.)'..SubO
+00000350: 626a 6563 747a 250a 2020 2020 496e 7465  bjectz%.    Inte
+00000360: 726e 616c 2075 7365 2c20 6e6f 7420 666f  rnal use, not fo
+00000370: 7220 7573 6572 730a 2020 2020 464e da04  r users.    FN..
+00000380: 6e61 6d65 7201 0000 0063 0300 0000 0000  namer....c......
+00000390: 0000 0000 0000 0400 0000 0300 0000 0300  ................
+000003a0: 0000 7334 0000 007c 017c 005f 0064 017d  ..s4...|.|._.d.}
+000003b0: 037c 0264 0075 0172 1074 0183 00a0 027c  .|.d.u.r.t.....|
+000003c0: 02a1 0101 006e 0574 0183 00a0 02a1 0001  .....n.t........
+000003d0: 0064 027c 005f 0364 0053 0029 034e 4672  .d.|._.d.S.).NFr
+000003e0: 0100 0000 2904 720e 0000 00da 0573 7570  ....).r......sup
+000003f0: 6572 da08 5f5f 696e 6974 5f5f da0d 636f  er..__init__..co
+00000400: 6e6e 6563 7465 6453 7562 7329 04da 0473  nnectedSubs)...s
+00000410: 656c 6672 0e00 0000 da06 5061 7265 6e74  elfr......Parent
+00000420: da06 6163 7469 7665 a901 da09 5f5f 636c  ..active....__cl
+00000430: 6173 735f 5fa9 00fa 2a2f 686f 6d65 2f65  ass__...*/home/e
+00000440: 642f 7374 6463 6f6d 5174 2f73 7263 2f73  d/stdcomQt/src/s
+00000450: 7464 636f 6d51 742f 7374 6463 6f6d 5174  tdcomQt/stdcomQt
+00000460: 2e70 7972 1000 0000 1b00 0000 730c 0000  .pyr........s...
+00000470: 0006 0104 0108 010e 010a 020a 017a 1253  .............z.S
+00000480: 7562 4f62 6a65 6374 2e5f 5f69 6e69 745f  ubObject.__init_
+00000490: 5f63 0200 0000 0000 0000 0000 0000 0200  _c..............
+000004a0: 0000 0200 0000 4300 0000 7326 0000 007c  ......C...s&...|
+000004b0: 006a 00a0 01a1 0001 007c 017c 005f 027c  .j.......|.|._.|
+000004c0: 006a 00a0 03a1 0001 007c 00a0 04a1 0001  .j.......|......
+000004d0: 0064 0053 00a9 014e 2905 da08 7072 6f78  .d.S...N)...prox
+000004e0: 4c6f 636b da04 6c6f 636b da04 6461 7461  Lock..lock..data
+000004f0: da06 756e 6c6f 636b da0b 4669 7265 436f  ..unlock..FireCo
+00000500: 6e6e 6563 74a9 0272 1200 0000 721c 0000  nnect..r....r...
+00000510: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00000520: da07 4164 6444 6174 6123 0000 0073 0800  ..AddData#...s..
+00000530: 0000 0a01 0601 0a01 0c01 7a11 5375 624f  ..........z.SubO
+00000540: 626a 6563 742e 4164 6444 6174 6163 0100  bject.AddDatac..
+00000550: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00000560: 0000 4300 0000 f31e 0000 007c 006a 00a0  ..C........|.j..
+00000570: 01a1 0001 007c 006a 027d 017c 006a 00a0  .....|.j.}.|.j..
+00000580: 03a1 0001 007c 0153 0072 1900 0000 2904  .....|.S.r....).
+00000590: 721a 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
+000005a0: 1d00 0000 721f 0000 0072 1700 0000 7217  ....r....r....r.
+000005b0: 0000 0072 1800 0000 da07 4765 7444 6174  ...r......GetDat
+000005c0: 6129 0000 00f3 0800 0000 0a01 0601 0a01  a)..............
+000005d0: 0401 7a11 5375 624f 626a 6563 742e 4765  ..z.SubObject.Ge
+000005e0: 7444 6174 6163 0100 0000 0000 0000 0000  tDatac..........
+000005f0: 0000 0200 0000 0200 0000 4300 0000 7221  ..........C...r!
+00000600: 0000 0072 1900 0000 2904 721a 0000 0072  ...r....).r....r
+00000610: 1b00 0000 da04 6465 7363 721d 0000 00a9  ......descr.....
+00000620: 0272 1200 0000 7224 0000 0072 1700 0000  .r....r$...r....
+00000630: 7217 0000 0072 1800 0000 da07 4765 7444  r....r......GetD
+00000640: 6573 632f 0000 0072 2300 0000 7a11 5375  esc/...r#...z.Su
+00000650: 624f 626a 6563 742e 4765 7444 6573 6363  bObject.GetDescc
+00000660: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000670: 0200 0000 4300 0000 7221 0000 0072 1900  ....C...r!...r..
+00000680: 0000 2904 721a 0000 0072 1b00 0000 720e  ..).r....r....r.
+00000690: 0000 0072 1d00 0000 2902 7212 0000 0072  ...r....).r....r
+000006a0: 0e00 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
+000006b0: 0000 00da 0747 6574 4e61 6d65 3500 0000  .....GetName5...
+000006c0: 7223 0000 007a 1153 7562 4f62 6a65 6374  r#...z.SubObject
+000006d0: 2e47 6574 4e61 6d65 6302 0000 0000 0000  .GetNamec.......
+000006e0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+000006f0: 0073 3000 0000 7c00 6a00 a001 a100 0100  .s0...|.j.......
+00000700: 7c01 7c00 5f02 7c00 6a00 a003 a100 0100  |.|._.|.j.......
+00000710: 7c00 6a04 a005 7c00 6a06 7c00 6a02 a102  |.j...|.j.|.j...
+00000720: 0100 6400 5300 7219 0000 0029 0772 1a00  ..d.S.r....).r..
+00000730: 0000 721b 0000 0072 2400 0000 721d 0000  ..r....r$...r...
+00000740: 00da 0a73 6967 4e65 7744 6573 63da 0465  ...sigNewDesc..e
+00000750: 6d69 7472 0e00 0000 7225 0000 0072 1700  mitr....r%...r..
+00000760: 0000 7217 0000 0072 1800 0000 da07 4164  ..r....r......Ad
+00000770: 6444 6573 633b 0000 0073 0800 0000 0a01  dDesc;...s......
+00000780: 0601 0a01 1601 7a11 5375 624f 626a 6563  ......z.SubObjec
+00000790: 742e 4164 6444 6573 6363 0100 0000 0000  t.AddDescc......
+000007a0: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+000007b0: 0000 7336 0000 007c 006a 00a0 017c 006a  ..s6...|.j...|.j
+000007c0: 027c 006a 03a1 0201 007c 006a 0464 0075  .|.j.....|.j.d.u
+000007d0: 0172 197c 006a 05a0 017c 006a 027c 006a  .r.|.j...|.j.|.j
+000007e0: 04a1 0201 0064 0053 0064 0053 0072 1900  .....d.S.d.S.r..
+000007f0: 0000 2906 da0a 7369 674e 6577 4461 7461  ..)...sigNewData
+00000800: 7229 0000 0072 0e00 0000 721c 0000 0072  r)...r....r....r
+00000810: 2400 0000 7228 0000 00a9 0172 1200 0000  $...r(.....r....
+00000820: 7217 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00000830: 1e00 0000 4100 0000 7308 0000 0012 010a  ....A...s.......
+00000840: 0116 0104 ff7a 1553 7562 4f62 6a65 6374  .....z.SubObject
+00000850: 2e46 6972 6543 6f6e 6e65 6374 54da 056f  .FireConnectT..o
+00000860: 776e 6572 6302 0000 0000 0000 0000 0000  wnerc...........
+00000870: 0002 0000 0002 0000 0043 0000 00f3 1e00  .........C......
+00000880: 0000 7c00 6a00 a001 a100 0100 7c01 7c00  ..|.j.......|.|.
+00000890: 5f02 7c00 6a00 a003 a100 0100 6400 5300  _.|.j.......d.S.
+000008a0: 7219 0000 00a9 0472 1a00 0000 721b 0000  r......r....r...
+000008b0: 0072 2d00 0000 721d 0000 00a9 0272 1200  .r-...r......r..
+000008c0: 0000 722d 0000 0072 1700 0000 7217 0000  ..r-...r....r...
+000008d0: 0072 1800 0000 da08 5365 744f 776e 6572  .r......SetOwner
+000008e0: 4600 0000 f306 0000 000a 0106 010e 017a  F..............z
+000008f0: 1253 7562 4f62 6a65 6374 2e53 6574 4f77  .SubObject.SetOw
+00000900: 6e65 7263 0100 0000 0000 0000 0000 0000  nerc............
+00000910: 0200 0000 0200 0000 4300 0000 7221 0000  ........C...r!..
+00000920: 0072 1900 0000 722f 0000 0072 3000 0000  .r....r/...r0...
+00000930: 7217 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
+00000940: 0769 734f 776e 6572 4b00 0000 7223 0000  .isOwnerK...r#..
+00000950: 007a 1153 7562 4f62 6a65 6374 2e69 734f  .z.SubObject.isO
+00000960: 776e 6572 6301 0000 0000 0000 0000 0000  wnerc...........
+00000970: 0002 0000 0002 0000 0043 0000 0073 2a00  .........C...s*.
+00000980: 0000 7c00 6a00 a001 a100 0100 7c00 6a02  ..|.j.......|.j.
+00000990: 6401 1700 7c00 5f02 7c00 6a02 7d01 7c00  d...|._.|.j.}.|.
+000009a0: 6a00 a003 a100 0100 7c01 5300 2902 4ee9  j.......|.S.).N.
+000009b0: 0100 0000 a904 721a 0000 0072 1b00 0000  ......r....r....
+000009c0: 7211 0000 0072 1d00 0000 a902 7212 0000  r....r......r...
+000009d0: 00da 0473 7562 7372 1700 0000 7217 0000  ...subsr....r...
+000009e0: 0072 1800 0000 da06 4164 6453 7562 5100  .r......AddSubQ.
+000009f0: 0000 730a 0000 000a 010c 0106 010a 0104  ..s.............
+00000a00: 017a 1053 7562 4f62 6a65 6374 2e41 6464  .z.SubObject.Add
+00000a10: 5375 6263 0100 0000 0000 0000 0000 0000  Subc............
+00000a20: 0200 0000 0200 0000 4300 0000 733a 0000  ........C...s:..
+00000a30: 007c 006a 00a0 01a1 0001 007c 006a 0264  .|.j.......|.j.d
+00000a40: 0118 007c 005f 027c 006a 027d 017c 006a  ...|._.|.j.}.|.j
+00000a50: 0264 026b 0072 1664 027c 005f 027c 006a  .d.k.r.d.|._.|.j
+00000a60: 00a0 03a1 0001 007c 0153 0029 034e 7234  .......|.S.).Nr4
+00000a70: 0000 0072 0100 0000 7235 0000 0072 3600  ...r....r5...r6.
+00000a80: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
+00000a90: 00da 0644 656c 5375 6258 0000 0073 0e00  ...DelSubX...s..
+00000aa0: 0000 0a01 0c01 0601 0a01 0601 0a01 0401  ................
+00000ab0: 7a10 5375 624f 626a 6563 742e 4465 6c53  z.SubObject.DelS
+00000ac0: 7562 6301 0000 0000 0000 0000 0000 0002  ubc.............
+00000ad0: 0000 0002 0000 0043 0000 0073 2200 0000  .......C...s"...
+00000ae0: 6401 7d01 7c00 6a00 a001 a100 0100 7c00  d.}.|.j.......|.
+00000af0: 6a02 7d01 7c00 6a00 a003 a100 0100 7c01  j.}.|.j.......|.
+00000b00: 5300 2902 4e72 0100 0000 7235 0000 0072  S.).Nr....r5...r
+00000b10: 3600 0000 7217 0000 0072 1700 0000 7218  6...r....r....r.
+00000b20: 0000 00da 0d47 6574 4e75 6d62 6572 5375  .....GetNumberSu
+00000b30: 6273 6100 0000 730a 0000 0004 010a 0106  bsa...s.........
+00000b40: 010a 0104 017a 1753 7562 4f62 6a65 6374  .....z.SubObject
+00000b50: 2e47 6574 4e75 6d62 6572 5375 6273 7214  .GetNumberSubsr.
+00000b60: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00000b70: 0200 0000 0200 0000 4300 0000 722e 0000  ........C...r...
+00000b80: 0072 1900 0000 a904 721a 0000 0072 1b00  .r......r....r..
+00000b90: 0000 7214 0000 0072 1d00 0000 a902 7212  ..r....r......r.
+00000ba0: 0000 0072 1400 0000 7217 0000 0072 1700  ...r....r....r..
+00000bb0: 0000 7218 0000 00da 0953 6574 4163 7469  ..r......SetActi
+00000bc0: 7665 6800 0000 7232 0000 007a 1353 7562  veh...r2...z.Sub
+00000bd0: 4f62 6a65 6374 2e53 6574 4163 7469 7665  Object.SetActive
+00000be0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000bf0: 0002 0000 0043 0000 0072 2100 0000 7219  .....C...r!...r.
+00000c00: 0000 0072 3b00 0000 723c 0000 0072 1700  ...r;...r<...r..
+00000c10: 0000 7217 0000 0072 1800 0000 da08 6973  ..r....r......is
+00000c20: 4163 7469 7665 6d00 0000 7223 0000 007a  Activem...r#...z
+00000c30: 1253 7562 4f62 6a65 6374 2e69 7341 6374  .SubObject.isAct
+00000c40: 6976 6572 1900 0000 2901 5429 22da 085f  iver....).T)".._
+00000c50: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000c60: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000c70: 5fda 075f 5f64 6f63 5f5f 7207 0000 00da  _..__doc__r.....
+00000c80: 0373 7472 da04 6c69 7374 722b 0000 0072  .str..listr+...r
+00000c90: 2800 0000 7214 0000 0072 2d00 0000 720e  (...r....r-...r.
+00000ca0: 0000 00da 0f5f 5f61 6e6e 6f74 6174 696f  .....__annotatio
+00000cb0: 6e73 5f5f 721c 0000 0072 2400 0000 7211  ns__r....r$...r.
+00000cc0: 0000 0072 0200 0000 721a 0000 0072 1000  ...r....r....r..
+00000cd0: 0000 7220 0000 0072 2200 0000 7226 0000  ..r ...r"...r&..
+00000ce0: 0072 2700 0000 722a 0000 0072 1e00 0000  .r'...r*...r....
+00000cf0: da04 626f 6f6c 7231 0000 0072 3300 0000  ..boolr1...r3...
+00000d00: 7238 0000 0072 3900 0000 723a 0000 0072  r8...r9...r:...r
+00000d10: 3d00 0000 723e 0000 00da 0d5f 5f63 6c61  =...r>.....__cla
+00000d20: 7373 6365 6c6c 5f5f 7217 0000 0072 1700  sscell__r....r..
+00000d30: 0000 7215 0000 0072 1800 0000 720d 0000  ..r....r....r...
+00000d40: 000b 0000 0073 3200 0000 0a00 0401 0a03  .....s2.........
+00000d50: 0a01 0402 0401 0c01 0401 0401 0401 0602  ................
+00000d60: 0e02 0c08 0806 0806 0806 0806 0806 1005  ................
+00000d70: 0805 0806 0807 0809 1007 1005 720d 0000  ............r...
+00000d80: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000d90: 0000 0500 0000 0000 0000 731c 0100 0065  ..........s....e
+00000da0: 005a 0164 005a 0264 015a 0365 0465 0583  .Z.d.Z.d.Z.e.e..
+00000db0: 015a 0665 0483 005a 0765 0483 005a 0864  .Z.e...Z.e...Z.d
+00000dc0: 025a 0964 025a 0a64 025a 0b64 025a 0c64  .Z.d.Z.d.Z.d.Z.d
+00000dd0: 025a 0d64 035a 0e65 0f83 005a 1065 0f83  .Z.d.Z.e...Z.e..
+00000de0: 005a 1169 005a 1264 2c64 0665 1364 0765  .Z.i.Z.d,d.e.d.e
+00000df0: 1466 0487 0066 0164 0864 0984 0d5a 1564  .f...f.d.d...Z.d
+00000e00: 0a64 0b84 005a 1664 0c64 0d84 005a 1764  .d...Z.d.d...Z.d
+00000e10: 0e64 0f84 005a 1864 2d64 1265 1364 1365  .d...Z.d-d.e.d.e
+00000e20: 1966 0464 1464 1584 055a 1a64 1664 1784  .f.d.d...Z.d.d..
+00000e30: 005a 1b64 1864 1984 005a 1c64 1a64 1b84  .Z.d.d...Z.d.d..
+00000e40: 005a 1d64 1c64 1d84 005a 1e65 1f83 0064  .Z.d.d...Z.e...d
+00000e50: 1e64 1f84 0083 015a 2065 1f83 0064 2064  .d.....Z e...d d
+00000e60: 2184 0083 015a 2165 1f83 0064 2264 2384  !....Z!e...d"d#.
+00000e70: 0083 015a 2265 1f65 1383 0164 2464 2584  ...Z"e.e...d$d%.
+00000e80: 0083 015a 2365 1f83 0064 2664 2784 0083  ...Z#e...d&d'...
+00000e90: 015a 2465 1f83 0064 2864 2984 0083 015a  .Z$e...d(d)....Z
+00000ea0: 2565 1f65 1365 1483 0264 2a64 2b84 0083  %e.e.e...d*d+...
+00000eb0: 015a 2687 0004 005a 2753 0029 2eda 0b73  .Z&....Z'S.)...s
+00000ec0: 7465 6351 536f 636b 6574 7a3c 0a20 2020  tecQSocketz<.   
+00000ed0: 2051 7420 5374 796c 6520 6342 7269 6467   Qt Style cBridg
+00000ee0: 6520 746f 2020 4d75 6c74 6976 6572 7365  e to  Multiverse
+00000ef0: 206a 7573 7420 6c69 6b65 2063 2b2b 2063   just like c++ c
+00000f00: 6f64 650a 2020 2020 4e46 da09 6c6f 6361  ode.    NF..loca
+00000f10: 6c68 6f73 74e9 2113 0000 da04 686f 7374  lhost.!.....host
+00000f20: da04 706f 7274 6304 0000 0000 0000 0000  ..portc.........
+00000f30: 0000 0004 0000 0003 0000 0003 0000 0073  ...............s
+00000f40: be00 0000 7c03 6401 7501 720b 7400 8300  ....|.d.u.r.t...
+00000f50: a001 7c03 a101 0100 6e05 7400 8300 a001  ..|.....n.t.....
+00000f60: a100 0100 7c03 7c00 5f02 7403 7c02 8301  ....|.|._.t.|...
+00000f70: 7c00 5f04 7405 7c01 8301 7c00 5f06 7407  |._.t.|...|._.t.
+00000f80: 8300 7c00 5f08 7c00 6a08 6a09 a00a 7c00  ..|._.|.j.j...|.
+00000f90: 6a0b a101 0100 7c00 6a08 6a0c a00a 7c00  j.....|.j.j...|.
+00000fa0: 6a0d a101 0100 7c00 6a08 6a0e a00a 7c00  j.....|.j.j...|.
+00000fb0: 6a0f a101 0100 7c00 6a08 6a10 a00a 7c00  j.....|.j.j...|.
+00000fc0: 6a11 a101 0100 7412 7c00 8301 7c00 5f13  j.....t.|...|._.
+00000fd0: 7c00 6a13 a014 6402 a101 0100 7c00 6a13  |.j...d.....|.j.
+00000fe0: 6a15 a00a 7c00 6a16 a101 0100 7c00 6a13  j...|.j.....|.j.
+00000ff0: a017 a100 0100 7c00 a016 a100 0100 6401  ......|.......d.
+00001000: 5300 2903 7aa9 0a20 2020 2020 2020 203a  S.).z..        :
+00001010: 7061 7261 6d20 686f 7374 3a20 486f 7374  param host: Host
+00001020: 2049 5020 6164 6472 6573 7320 6465 6661   IP address defa
+00001030: 756c 7420 6c6f 6361 6c68 6f73 740a 2020  ult localhost.  
+00001040: 2020 2020 2020 3a70 6172 616d 2070 6f72        :param por
+00001050: 743a 2053 6572 7669 6365 2050 6f72 742c  t: Service Port,
+00001060: 2064 6566 6175 6c74 2034 3839 370a 2020   default 4897.  
+00001070: 2020 2020 2020 3a70 6172 616d 2050 6172        :param Par
+00001080: 656e 743a 2051 7420 514f 626a 6563 7420  ent: Qt QObject 
+00001090: 7061 7265 6e74 206f 7220 4e6f 6e65 2064  parent or None d
+000010a0: 6566 6175 6c74 0a20 2020 2020 2020 204e  efault.        N
+000010b0: 6988 1300 0029 1872 0f00 0000 7210 0000  i....).r....r...
+000010c0: 0072 1300 0000 da03 696e 74da 0b73 6572  .r......int..ser
+000010d0: 7669 6365 506f 7274 7243 0000 0072 4b00  vicePortrC...rK.
+000010e0: 0000 720a 0000 00da 0278 6dda 0963 6f6e  ..r......xm..con
+000010f0: 6e65 6374 6564 da07 636f 6e6e 6563 74da  nected..connect.
+00001100: 0d53 6c6f 7443 6f6e 6e65 6374 6564 da0c  .SlotConnected..
+00001110: 6469 7363 6f6e 6e65 6374 6564 da10 536c  disconnected..Sl
+00001120: 6f74 4469 7363 6f6e 6e65 6374 6564 da09  otDisconnected..
+00001130: 7265 6164 7952 6561 64da 0d53 6c6f 7444  readyRead..SlotD
+00001140: 6174 6152 6561 6479 da05 6572 726f 72da  ataReady..error.
+00001150: 0f53 6c6f 7453 6f63 6b65 7445 7272 6f72  .SlotSocketError
+00001160: 7204 0000 00da 0574 696d 6572 da0b 7365  r......timer..se
+00001170: 7449 6e74 6572 7661 6cda 0774 696d 656f  tInterval..timeo
+00001180: 7574 da0c 536c 6f74 5469 6d65 726f 7574  ut..SlotTimerout
+00001190: da05 7374 6172 7429 0472 1200 0000 724b  ..start).r....rK
+000011a0: 0000 0072 4c00 0000 7213 0000 0072 1500  ...rL...r....r..
+000011b0: 0000 7217 0000 0072 1800 0000 7210 0000  ..r....r....r...
+000011c0: 0087 0000 0073 2000 0000 0806 0e01 0a02  .....s .........
+000011d0: 0602 0a02 0a01 0801 1001 1001 1001 1001  ................
+000011e0: 0a02 0c01 1001 0a01 0c01 7a14 7374 6563  ..........z.stec
+000011f0: 5153 6f63 6b65 742e 5f5f 696e 6974 5f5f  QSocket.__init__
+00001200: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001210: 0002 0000 0043 0000 0073 1800 0000 7c00  .....C...s....|.
+00001220: 6a00 a001 a100 0100 7c00 6a02 a003 a100  j.......|.j.....
+00001230: 0100 6401 5300 2902 7a42 0a20 2020 2020  ..d.S.).zB.     
+00001240: 2020 2063 616c 6c20 6265 666f 7265 2064     call before d
+00001250: 656c 6574 656c 6174 6572 2062 7920 7573  eletelater by us
+00001260: 6572 0a20 2020 2020 2020 203a 7265 7475  er.        :retu
+00001270: 726e 3a0a 2020 2020 2020 2020 4e29 0472  rn:.        N).r
+00001280: 4f00 0000 da05 636c 6f73 6572 5900 0000  O.....closerY...
+00001290: da04 7374 6f70 722c 0000 0072 1700 0000  ..stopr,...r....
+000012a0: 7217 0000 0072 1800 0000 da04 7175 6974  r....r......quit
+000012b0: a200 0000 7304 0000 000a 050e 017a 1073  ....s........z.s
+000012c0: 7465 6351 536f 636b 6574 2e71 7569 7463  tecQSocket.quitc
+000012d0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+000012e0: 0500 0000 4300 0000 7342 0000 007c 006a  ....C...sB...|.j
+000012f0: 00a0 01a1 0001 007c 017c 006a 0276 0172  .......|.|.j.v.r
+00001300: 147c 006a 02a0 037c 0174 047c 0183 0169  .|.j...|.t.|...i
+00001310: 01a1 0101 007c 006a 02a0 057c 01a1 017d  .....|.j...|...}
+00001320: 027c 006a 00a0 06a1 0001 007c 0253 0029  .|.j.......|.S.)
+00001330: 017a 6b0a 2020 2020 2020 2020 496e 7465  .zk.        Inte
+00001340: 726e 616c 2075 7365 2c20 6e6f 7420 666f  rnal use, not fo
+00001350: 7220 7573 6572 0a20 2020 2020 2020 203a  r user.        :
+00001360: 7061 7261 6d20 6e61 6d65 3a20 6e61 6d65  param name: name
+00001370: 206f 6620 7468 6520 7375 6273 6372 6970   of the subscrip
+00001380: 7469 6f6e 0a20 2020 2020 2020 203a 7265  tion.        :re
+00001390: 7475 726e 3a0a 2020 2020 2020 2020 2907  turn:.        ).
+000013a0: da09 6e61 6d65 734c 6f63 6b72 1b00 0000  ..namesLockr....
+000013b0: da05 6e61 6d65 73da 0675 7064 6174 6572  ..names..updater
+000013c0: 0d00 0000 da03 6765 7472 1d00 0000 2903  ......getr....).
+000013d0: 7212 0000 0072 0e00 0000 da06 7870 726f  r....r......xpro
+000013e0: 7879 7217 0000 0072 1700 0000 7218 0000  xyr....r....r...
+000013f0: 00da 0b49 6e73 6572 7450 726f 7879 aa00  ...InsertProxy..
+00001400: 0000 730c 0000 000a 060a 0114 010c 020a  ..s.............
+00001410: 0104 017a 1773 7465 6351 536f 636b 6574  ...z.stecQSocket
+00001420: 2e49 6e73 6572 7450 726f 7879 6301 0000  .InsertProxyc...
+00001430: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+00001440: 0043 0000 0073 2600 0000 6700 7d01 7c00  .C...s&...g.}.|.
+00001450: 6a00 a001 a100 0100 7c00 6a02 a003 a100  j.......|.j.....
+00001460: 7d01 7c00 6a00 a004 a100 0100 7c01 5300  }.|.j.......|.S.
+00001470: 7219 0000 0029 0572 6100 0000 721b 0000  r....).ra...r...
+00001480: 0072 6200 0000 da04 6b65 7973 721d 0000  .rb.....keysr...
+00001490: 0029 0272 1200 0000 7267 0000 0072 1700  .).r....rg...r..
+000014a0: 0000 7217 0000 0072 1800 0000 da08 6765  ..r....r......ge
+000014b0: 744e 616d 6573 b800 0000 730a 0000 0004  tNames....s.....
+000014c0: 010a 010a 010a 0104 017a 1473 7465 6351  .........z.stecQ
+000014d0: 536f 636b 6574 2e67 6574 4e61 6d65 73fa  Socket.getNames.
+000014e0: 1d4d 616b 6520 7468 6973 204d 616c 636f  .Make this Malco
+000014f0: 6c6d 5072 6f6f 6620 506c 6561 7365 54da  lmProof PleaseT.
+00001500: 0b64 6573 6372 6970 7469 6f6e da04 666c  .description..fl
+00001510: 6167 6304 0000 0000 0000 0000 0000 0005  agc.............
+00001520: 0000 0003 0000 0043 0000 0073 1800 0000  .......C...s....
+00001530: 7c00 a000 7c01 a101 7d04 7c04 a001 7c03  |...|...}.|...|.
+00001540: a101 0100 6401 5300 2902 7afb 0a20 2020  ....d.S.).z..   
+00001550: 2020 2020 2053 6574 7320 7573 2061 7320       Sets us as 
+00001560: 7468 6520 6f77 6e65 7220 6f66 2074 6865  the owner of the
+00001570: 2073 7562 7363 7269 7074 696f 6e2c 2077   subscription, w
+00001580: 6520 7769 6c6c 2061 7574 6f6d 6174 6963  e will automatic
+00001590: 616c 6c79 2072 6566 6565 6420 6d75 6c74  ally refeed mult
+000015a0: 6976 6572 7365 2069 6620 7265 7365 740a  iverse if reset.
+000015b0: 2020 2020 2020 2020 3a70 6172 616d 206e          :param n
+000015c0: 616d 653a 2073 7562 7363 7269 7074 696f  ame: subscriptio
+000015d0: 6e20 6e61 6d65 0a20 2020 2020 2020 203a  n name.        :
+000015e0: 7061 7261 6d20 666c 6167 3a20 2054 7275  param flag:  Tru
+000015f0: 6520 6d65 616e 7320 7765 2061 7265 2067  e means we are g
+00001600: 6f6c 6465 6e20 636f 7079 2c20 6661 6c73  olden copy, fals
+00001610: 6520 7265 7374 6f72 6573 2074 6f20 6e6f  e restores to no
+00001620: 6e2d 676f 6c64 656e 2063 6f70 790a 2020  n-golden copy.  
+00001630: 2020 2020 2020 3a72 6574 7572 6e3a 0a20        :return:. 
+00001640: 2020 2020 2020 204e 2902 7266 0000 0072         N).rf...r
+00001650: 3100 0000 2905 7212 0000 0072 0e00 0000  1...).r....r....
+00001660: 726a 0000 0072 6b00 0000 da05 7072 6f78  rj...rk.....prox
+00001670: 7972 1700 0000 7217 0000 0072 1800 0000  yr....r....r....
+00001680: da08 7365 744f 776e 6572 bf00 0000 7304  ..setOwner....s.
+00001690: 0000 000a 070e 017a 1473 7465 6351 536f  .......z.stecQSo
+000016a0: 636b 6574 2e73 6574 4f77 6e65 7263 0100  cket.setOwnerc..
+000016b0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+000016c0: 0000 4300 0000 7221 0000 0029 017a 4a0a  ..C...r!...).zJ.
+000016d0: 2020 2020 2020 2020 7265 7475 726e 7320          returns 
+000016e0: 7472 7565 2069 6620 636f 6e6e 6563 7465  true if connecte
+000016f0: 6420 746f 206d 756c 7469 7665 7273 650a  d to multiverse.
+00001700: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00001710: 0a20 2020 2020 2020 20a9 04da 0d63 6f6e  .        ....con
+00001720: 6e65 6374 6564 4c6f 636b 721b 0000 0072  nectedLockr....r
+00001730: 5000 0000 721d 0000 0029 0272 1200 0000  P...r....).r....
+00001740: 7250 0000 0072 1700 0000 7217 0000 0072  rP...r....r....r
+00001750: 1800 0000 da0b 6973 436f 6e6e 6563 7465  ......isConnecte
+00001760: 64c9 0000 0073 0800 0000 0a05 0601 0a01  d....s..........
+00001770: 0401 7a17 7374 6563 5153 6f63 6b65 742e  ..z.stecQSocket.
+00001780: 6973 436f 6e6e 6563 7465 6463 0100 0000  isConnectedc....
+00001790: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+000017a0: 4300 0000 f306 0000 007c 006a 0053 0029  C........|.j.S.)
+000017b0: 017a 270a 2020 2020 2020 2020 3a72 6574  .z'.        :ret
+000017c0: 7572 6e3a 2063 7572 7265 6e74 2048 6f73  urn: current Hos
+000017d0: 740a 2020 2020 2020 2020 2901 724b 0000  t.        ).rK..
+000017e0: 0072 2c00 0000 7217 0000 0072 1700 0000  .r,...r....r....
+000017f0: 7218 0000 00da 0448 6f73 74d3 0000 00f3  r......Host.....
+00001800: 0200 0000 0604 7a10 7374 6563 5153 6f63  ......z.stecQSoc
+00001810: 6b65 742e 486f 7374 6301 0000 0000 0000  ket.Hostc.......
+00001820: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+00001830: 0072 7100 0000 2901 7a30 0a20 2020 2020  .rq...).z0.     
+00001840: 2020 203a 7265 7475 726e 3a20 2063 7572     :return:  cur
+00001850: 7265 6e74 2073 6572 7669 6365 2050 6f72  rent service Por
+00001860: 740a 2020 2020 2020 2020 2901 724e 0000  t.        ).rN..
+00001870: 0072 2c00 0000 7217 0000 0072 1700 0000  .r,...r....r....
+00001880: 7218 0000 00da 0450 6f72 74d8 0000 0072  r......Port....r
+00001890: 7300 0000 7a10 7374 6563 5153 6f63 6b65  s...z.stecQSocke
+000018a0: 742e 506f 7274 6302 0000 0000 0000 0000  t.Portc.........
+000018b0: 0000 0006 0000 0005 0000 0043 0000 0073  ...........C...s
+000018c0: 0201 0000 6401 7c01 7600 722e 6700 7d02  ....d.|.v.r.g.}.
+000018d0: 7400 6402 7401 7c01 8301 8302 4400 5d12  t.d.t.|.....D.].
+000018e0: 7d03 7402 7c01 7c03 1900 8301 7d04 7c02  }.t.|.|.....}.|.
+000018f0: a003 7c04 a101 0100 7c00 a004 7c04 a101  ..|.....|...|...
+00001900: 7d05 710d 7401 7c02 8301 722c 7c00 6a05  }.q.t.|...r,|.j.
+00001910: a006 7c02 a101 0100 6406 5300 6406 5300  ..|.....d.S.d.S.
+00001920: 6403 7c01 7600 7265 7401 7c01 8301 6404  d.|.v.ret.|...d.
+00001930: 6b04 7261 7402 7c01 6402 1900 8301 7d04  k.rat.|.d.....}.
+00001940: 6700 7d02 7400 6404 7401 7c01 8301 8302  g.}.t.d.t.|.....
+00001950: 4400 5d09 7d03 7c02 a003 7c01 7c03 1900  D.].}.|...|.|...
+00001960: a101 0100 7147 7401 7c02 8301 7263 7c00  ....qGt.|...rc|.
+00001970: a004 7c04 a101 7d05 7c05 a007 7c02 a101  ..|...}.|...|...
+00001980: 0100 6406 5300 6406 5300 6406 5300 6405  ..d.S.d.S.d.S.d.
+00001990: 7c01 7600 727f 7402 7c01 6402 1900 8301  |.v.r.t.|.d.....
+000019a0: 7d04 7c00 a004 7c04 a101 7d05 7c05 a008  }.|...|...}.|...
+000019b0: 7402 7c01 6404 1900 8301 a101 0100 6406  t.|.d.........d.
+000019c0: 5300 6406 5300 2907 7a55 0a20 2020 2020  S.d.S.).zU.     
+000019d0: 2020 2069 6e74 6572 6e61 6c20 7573 652c     internal use,
+000019e0: 2064 6563 6f64 6573 206d 6573 7361 6765   decodes message
+000019f0: 730a 2020 2020 2020 2020 3a70 6172 616d  s.        :param
+00001a00: 2072 6f77 3a0a 2020 2020 2020 2020 3a72   row:.        :r
+00001a10: 6574 7572 6e3a 0a20 2020 2020 2020 20da  eturn:.        .
+00001a20: 074e 414d 4553 5550 7234 0000 00da 0852  .NAMESUPr4.....R
+00001a30: 4541 4444 4154 41e9 0200 0000 7a0b 5550  EADDATA.....z.UP
+00001a40: 4441 5445 2d44 4553 434e 2909 da05 7261  DATE-DESCN)...ra
+00001a50: 6e67 65da 036c 656e 7243 0000 00da 0661  nge..lenrC.....a
+00001a60: 7070 656e 6472 6600 0000 da0b 7369 674e  ppendrf.....sigN
+00001a70: 6577 4e61 6d65 7372 2900 0000 7220 0000  ewNamesr)...r ..
+00001a80: 0072 2a00 0000 2906 7212 0000 00da 0372  .r*...).r......r
+00001a90: 6f77 721c 0000 00da 0178 720e 0000 00da  owr......xr.....
+00001aa0: 0278 7072 1700 0000 7217 0000 0072 1800  .xpr....r....r..
+00001ab0: 0000 da0e 5072 6f63 6573 7343 6f6d 6d61  ....ProcessComma
+00001ac0: 6e64 dd00 0000 7332 0000 0008 0604 0112  nd....s2........
+00001ad0: 010c 010a 010c 0108 0110 0104 ff08 030c  ................
+00001ae0: 010c 0104 0112 0110 0108 010a 010e 0104  ................
+00001af0: f904 0508 040c 010a 0216 0104 fc7a 1a73  .............z.s
+00001b00: 7465 6351 536f 636b 6574 2e50 726f 6365  tecQSocket.Proce
+00001b10: 7373 436f 6d6d 616e 6463 0100 0000 0000  ssCommandc......
+00001b20: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+00001b30: 0000 7332 0000 007c 006a 00a0 01a1 0072  ..s2...|.j.....r
+00001b40: 0a7c 006a 00a0 02a1 0001 007c 006a 03a0  .|.j.......|.j..
+00001b50: 04a1 0001 0064 017c 005f 057c 006a 03a0  .....d.|._.|.j..
+00001b60: 06a1 0001 0064 0253 0029 037a 620a 2020  .....d.S.).zb.  
+00001b70: 2020 2020 2020 696e 7465 726e 616c 2075        internal u
+00001b80: 7365 0a20 2020 2020 2020 2063 616c 6c65  se.        calle
+00001b90: 6420 7768 656e 2063 6f6e 6e65 6374 696f  d when connectio
+00001ba0: 6e20 746f 206d 756c 7469 7665 7273 6520  n to multiverse 
+00001bb0: 6661 696c 730a 2020 2020 2020 2020 3a72  fails.        :r
+00001bc0: 6574 7572 6e3a 0a20 2020 2020 2020 2046  eturn:.        F
+00001bd0: 4e29 0772 4f00 0000 da06 6973 4f70 656e  N).rO.....isOpen
+00001be0: 725e 0000 0072 6f00 0000 721b 0000 0072  r^...ro...r....r
+00001bf0: 5000 0000 721d 0000 0072 2c00 0000 7217  P...r....r,...r.
+00001c00: 0000 0072 1700 0000 7218 0000 0072 5800  ...r....r....rX.
+00001c10: 0000 fc00 0000 730a 0000 000a 070a 010a  ......s.........
+00001c20: 0106 010e 017a 1b73 7465 6351 536f 636b  .....z.stecQSock
+00001c30: 6574 2e53 6c6f 7453 6f63 6b65 7445 7272  et.SlotSocketErr
+00001c40: 6f72 6301 0000 0000 0000 0000 0000 0008  orc.............
+00001c50: 0000 0006 0000 0043 0000 0073 8401 0000  .......C...s....
+00001c60: 7c00 6a00 a001 a100 0100 6401 7c00 5f02  |.j.......d.|._.
+00001c70: 7c00 6a00 a003 a100 0100 6402 7d01 7c00  |.j.......d.}.|.
+00001c80: a004 7c01 a101 0100 7c00 6a05 a001 a100  ..|.....|.j.....
+00001c90: 0100 7c00 6a06 a007 a100 7d02 7c02 4400  ..|.j.....}.|.D.
+00001ca0: 5d9a 7d03 7c00 6a06 a008 7c03 a101 7d04  ].}.|.j...|...}.
+00001cb0: 7c04 a009 a100 6401 7500 7239 6403 7c03  |.....d.u.r9d.|.
+00001cc0: 1700 6404 1700 7d01 7c00 a004 7c01 a101  ..d...}.|...|...
+00001cd0: 0100 7c04 a00a a100 72ba 7c04 a00b a100  ..|.....r.|.....
+00001ce0: 7d05 7c05 6405 7501 72a1 740c 7c05 8301  }.|.d.u.r.t.|...
+00001cf0: 72a1 6406 7d06 740d 7c05 6406 1900 740e  r.d.}.t.|.d...t.
+00001d00: 8302 725d 6407 7c03 1700 6408 1700 740f  ..r]d.|...d...t.
+00001d10: 7c06 8301 1700 7d01 6e2e 740d 7c05 6406  |.....}.n.t.|.d.
+00001d20: 1900 7410 8302 726f 6409 7c03 1700 6408  ..t...rod.|...d.
+00001d30: 1700 740f 7c06 8301 1700 7d01 6e1c 740d  ..t.|.....}.n.t.
+00001d40: 7c05 6406 1900 7411 8302 7281 640a 7c03  |.d...t...r.d.|.
+00001d50: 1700 6408 1700 740f 7c06 8301 1700 7d01  ..d...t.|.....}.
+00001d60: 6e0a 640b 7c03 1700 6408 1700 740f 7c06  n.d.|...d...t.|.
+00001d70: 8301 1700 7d01 7c05 4400 5d0a 7d07 7c01  ....}.|.D.].}.|.
+00001d80: 6408 740f 7c07 8301 1700 3700 7d01 718d  d.t.|.....7.}.q.
+00001d90: 7c01 6404 3700 7d01 7c00 a004 7c01 a101  |.d.7.}.|...|...
+00001da0: 0100 7c04 a012 a100 7d05 7c05 6405 7501  ..|.....}.|.d.u.
+00001db0: 72ba 640c 7c03 1700 6408 1700 7c05 1700  r.d.|...d...|...
+00001dc0: 7d01 7c01 6404 3700 7d01 7c00 a004 7c01  }.|.d.7.}.|...|.
+00001dd0: a101 0100 7120 7c00 6a05 a003 a100 0100  ....q |.j.......
+00001de0: 6405 5300 290d 7a64 0a20 2020 2020 2020  d.S.).zd.       
+00001df0: 2069 6e74 6572 616c 2075 7365 0a20 2020   interal use.   
+00001e00: 2020 2020 2057 696c 6c20 7265 7374 6172       Will restar
+00001e10: 7420 616e 7920 5375 6273 6372 6970 7469  t any Subscripti
+00001e20: 6f6e 2070 7265 7669 6f75 736c 7920 6d61  on previously ma
+00001e30: 6465 0a20 2020 2020 2020 203a 7265 7475  de.        :retu
+00001e40: 726e 3a0a 2020 2020 2020 2020 547a 064e  rn:.        Tz.N
+00001e50: 414d 4553 0afa 074e 4f54 4946 592c da01  AMES...NOTIFY,..
+00001e60: 0a4e 7201 0000 00fa 0855 5044 4154 4549  .Nr......UPDATEI
+00001e70: 2cfa 012c fa08 5550 4441 5445 462c fa08  ,..,..UPDATEF,..
+00001e80: 5550 4441 5445 422c fa07 5550 4441 5445  UPDATEB,..UPDATE
+00001e90: 2cfa 0c55 5044 4154 452d 4445 5343 2c29  ,..UPDATE-DESC,)
+00001ea0: 1372 6f00 0000 721b 0000 0072 5000 0000  .ro...r....rP...
+00001eb0: 721d 0000 00da 0953 6c6f 7457 7269 7465  r......SlotWrite
+00001ec0: 7261 0000 0072 6200 0000 7267 0000 0072  ra...rb...rg...r
+00001ed0: 6400 0000 723e 0000 0072 3300 0000 7222  d...r>...r3...r"
+00001ee0: 0000 0072 7900 0000 da0a 6973 696e 7374  ...ry.....isinst
+00001ef0: 616e 6365 724d 0000 0072 4300 0000 da05  ancerM...rC.....
+00001f00: 666c 6f61 7472 4600 0000 7226 0000 0029  floatrF...r&...)
+00001f10: 0872 1200 0000 da07 636f 6d6d 616e 6472  .r......commandr
+00001f20: 6200 0000 720e 0000 0072 6c00 0000 da04  b...r....rl.....
+00001f30: 7768 6174 da05 696e 6465 78da 0477 6f72  what..index..wor
+00001f40: 6472 1700 0000 7217 0000 0072 1800 0000  dr....r....r....
+00001f50: 7252 0000 0009 0100 0073 4600 0000 0a07  rR.......sF.....
+00001f60: 0601 0a01 0402 0a01 0a02 0a01 0801 0c01  ................
+00001f70: 0c01 0c01 0a01 0802 0801 0801 0802 0401  ................
+00001f80: 0e01 1601 0e02 1601 0e02 1601 1403 0802  ................
+00001f90: 1201 0801 0a02 0802 0801 1001 0801 0a01  ................
+00001fa0: 0280 0e02 7a19 7374 6563 5153 6f63 6b65  ....z.stecQSocke
+00001fb0: 742e 536c 6f74 436f 6e6e 6563 7465 6463  t.SlotConnectedc
+00001fc0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001fd0: 0200 0000 4300 0000 731e 0000 007c 006a  ....C...s....|.j
+00001fe0: 00a0 01a1 0001 0064 017c 005f 027c 006a  .......d.|._.|.j
+00001ff0: 00a0 03a1 0001 0064 0253 0029 03fa 2f0a  .......d.S.)../.
+00002000: 2020 2020 2020 2020 696e 7465 726e 616c          internal
+00002010: 2075 7365 0a20 2020 2020 2020 203a 7265   use.        :re
+00002020: 7475 726e 3a0a 2020 2020 2020 2020 464e  turn:.        FN
+00002030: 726e 0000 0072 2c00 0000 7217 0000 0072  rn...r,...r....r
+00002040: 1700 0000 7218 0000 0072 5400 0000 3f01  ....r....rT...?.
+00002050: 0000 7306 0000 000a 0606 010e 017a 1c73  ..s..........z.s
+00002060: 7465 6351 536f 636b 6574 2e53 6c6f 7444  tecQSocket.SlotD
+00002070: 6973 636f 6e6e 6563 7465 6463 0200 0000  isconnectedc....
+00002080: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+00002090: 4300 0000 7322 0000 007c 00a0 00a1 0072  C...s"...|.....r
+000020a0: 0f7c 006a 01a0 027c 01a0 0364 01a1 01a1  .|.j...|...d....
+000020b0: 0101 0064 0253 0064 0253 0029 037a 470a  ...d.S.d.S.).zG.
+000020c0: 2020 2020 2020 2020 696e 7465 726e 616c          internal
+000020d0: 2075 7365 0a20 2020 2020 2020 203a 7061   use.        :pa
+000020e0: 7261 6d20 636f 6d6d 616e 643a 0a20 2020  ram command:.   
+000020f0: 2020 2020 203a 7265 7475 726e 3a0a 2020       :return:.  
+00002100: 2020 2020 2020 da05 6173 6369 694e 2904        ..asciiN).
+00002110: 7270 0000 0072 4f00 0000 da05 7772 6974  rp...rO.....writ
+00002120: 65da 0665 6e63 6f64 65a9 0272 1200 0000  e..encode..r....
+00002130: 728c 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
+00002140: 1800 0000 7289 0000 0049 0100 0073 0600  ....r....I...s..
+00002150: 0000 0807 1601 04ff 7a15 7374 6563 5153  ........z.stecQS
+00002160: 6f63 6b65 742e 536c 6f74 5772 6974 6563  ocket.SlotWritec
+00002170: 0100 0000 0000 0000 0000 0000 0500 0000  ................
+00002180: 0500 0000 4300 0000 7368 0000 007c 006a  ....C...sh...|.j
+00002190: 00a0 01a1 0072 327c 006a 00a0 02a1 007d  .....r2|.j.....}
+000021a0: 017c 01a0 03a1 00a0 0464 01a1 017d 0274  .|.......d...}.t
+000021b0: 0574 066a 077c 02a0 0864 02a1 0164 0364  .t.j.|...d...d.d
+000021c0: 048d 0283 017d 037c 0344 005d 0b7d 0474  .....}.|.D.].}.t
+000021d0: 097c 0483 0172 2a7c 00a0 0a7c 04a1 0101  .|...r*|...|....
+000021e0: 0071 1f7c 006a 00a0 01a1 0073 0564 0553  .q.|.j.....s.d.S
+000021f0: 0064 0553 0029 067a 2f0a 2020 2020 2020  .d.S.).z/.      
+00002200: 2020 496e 7465 726e 616c 2075 7365 0a20    Internal use. 
+00002210: 2020 2020 2020 203a 7265 7475 726e 3a0a         :return:.
+00002220: 2020 2020 2020 2020 7291 0000 0072 8200          r....r..
+00002230: 0000 7284 0000 0029 01da 0964 656c 696d  ..r....)...delim
+00002240: 6974 6572 4e29 0b72 4f00 0000 da0b 6361  iterN).rO.....ca
+00002250: 6e52 6561 644c 696e 65da 0872 6561 644c  nReadLine..readL
+00002260: 696e 6572 1c00 0000 da06 6465 636f 6465  iner......decode
+00002270: 7244 0000 00da 0363 7376 da06 7265 6164  rD.....csv..read
+00002280: 6572 da05 7370 6c69 7472 7900 0000 727f  er..splitry...r.
+00002290: 0000 0029 0572 1200 0000 721c 0000 00da  ...).r....r.....
+000022a0: 026a 7672 9a00 0000 da04 6561 6368 7217  .jvr......eachr.
+000022b0: 0000 0072 1700 0000 7218 0000 0072 5600  ...r....r....rV.
+000022c0: 0000 5301 0000 7312 0000 000a 060a 010e  ..S...s.........
+000022d0: 0118 0108 0108 010a 0102 8012 fa7a 1973  .............z.s
+000022e0: 7465 6351 536f 636b 6574 2e53 6c6f 7444  tecQSocket.SlotD
+000022f0: 6174 6152 6561 6479 6301 0000 0000 0000  ataReadyc.......
+00002300: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
+00002310: 0073 4c00 0000 7c00 a000 a100 6401 7500  .sL...|.....d.u.
+00002320: 721d 7401 6402 7c00 6a02 a003 a100 8302  r.t.d.|.j.......
+00002330: 0100 7c00 6a02 a004 7405 7c00 6a06 8301  ..|.j...t.|.j...
+00002340: 7407 7c00 6a08 8301 a102 0100 6404 5300  t.|.j.......d.S.
+00002350: 6403 7d01 7c00 a009 7c01 a101 0100 6404  d.}.|...|.....d.
+00002360: 5300 2905 7290 0000 0046 7a07 5374 6174  S.).r....Fz.Stat
+00002370: 653a 207a 0550 494e 470a 4e29 0a72 7000  e: z.PING.N).rp.
+00002380: 0000 da05 7072 696e 7472 4f00 0000 da05  ....printrO.....
+00002390: 7374 6174 65da 0d63 6f6e 6e65 6374 546f  state..connectTo
+000023a0: 486f 7374 7243 0000 0072 4b00 0000 724d  HostrC...rK...rM
+000023b0: 0000 0072 4e00 0000 7289 0000 0072 9400  ...rN...r....r..
+000023c0: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
+000023d0: 0072 5c00 0000 6101 0000 730a 0000 000c  .r\...a...s.....
+000023e0: 0710 011e 0104 020e 017a 1873 7465 6351  .........z.stecQ
+000023f0: 536f 636b 6574 2e53 6c6f 7454 696d 6572  Socket.SlotTimer
+00002400: 6f75 7463 0300 0000 0000 0000 0000 0000  outc............
+00002410: 0300 0000 0200 0000 4300 0000 7342 0000  ........C...sB..
+00002420: 007c 006a 00a0 01a1 0001 007c 017c 005f  .|.j.......|.|._
+00002430: 027c 027c 005f 037c 00a0 04a1 0064 0175  .|.|._.|.....d.u
+00002440: 0072 167c 006a 05a0 06a1 0001 007c 00a0  .r.|.j.......|..
+00002450: 07a1 0001 007c 006a 00a0 08a1 0001 0064  .....|.j.......d
+00002460: 0253 0029 0361 1901 0000 0a20 2020 2020  .S.).a.....     
+00002470: 2020 2075 7365 7220 6361 6e20 6368 616e     user can chan
+00002480: 6765 2074 6865 2020 2020 2020 2020 2020  ge the          
 00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000024a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000024d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000024e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000024f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002510: 2020 2020 636f 6e6e 6563 7469 6f6e 2c20      connection, 
-00002520: 6279 2068 6f73 7420 616e 6420 706f 7274  by host and port
-00002530: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00002540: 686f 7374 3a0a 2020 2020 2020 2020 3a70  host:.        :p
-00002550: 6172 616d 2070 6f72 743a 0a20 2020 2020  aram port:.     
-00002560: 2020 203a 7265 7475 726e 3a0a 2020 2020     :return:.    
-00002570: 2020 2020 544e 2909 7258 0000 0072 5e00      TN).rX...r^.
-00002580: 0000 724a 0000 0072 4d00 0000 726f 0000  ..rJ...rM...ro..
-00002590: 0072 4e00 0000 725d 0000 0072 5b00 0000  .rN...r]...r[...
-000025a0: 725c 0000 0029 0372 1100 0000 724a 0000  r\...).r....rJ..
-000025b0: 0072 4b00 0000 7216 0000 0072 1600 0000  .rK...r....r....
-000025c0: 7217 0000 00da 0b53 6c6f 744e 6577 486f  r......SlotNewHo
-000025d0: 7374 6b01 0000 730e 0000 000a 0806 0106  stk...s.........
-000025e0: 010c 020a 0108 020e 017a 1773 7465 6351  .........z.stecQ
-000025f0: 536f 636b 6574 2e53 6c6f 744e 6577 486f  Socket.SlotNewHo
-00002600: 7374 2903 7248 0000 0072 4900 0000 4e29  st).rH...rI...N)
-00002610: 0272 6800 0000 5429 2872 3e00 0000 723f  .rh...T)(r>...r?
-00002620: 0000 0072 4000 0000 7241 0000 0072 0700  ...r@...rA...r..
-00002630: 0000 7243 0000 0072 7a00 0000 da07 7369  ..rC...rz.....si
-00002640: 6744 6f77 6eda 0673 6967 6e55 7072 4d00  gDown..signUprM.
-00002650: 0000 724a 0000 0072 5800 0000 724e 0000  ..rJ...rX...rN..
-00002660: 0072 1200 0000 724f 0000 0072 0200 0000  .r....rO...r....
-00002670: 7260 0000 0072 6e00 0000 7261 0000 0072  r`...rn...ra...r
-00002680: 4200 0000 724c 0000 0072 0f00 0000 725f  B...rL...r....r_
-00002690: 0000 0072 6500 0000 7267 0000 0072 4500  ...re...rg...rE.
-000026a0: 0000 726c 0000 0072 6f00 0000 7271 0000  ..rl...ro...rq..
-000026b0: 0072 7300 0000 727e 0000 0072 0600 0000  .rs...r~...r....
-000026c0: 7257 0000 0072 5100 0000 7253 0000 0072  rW...rQ...rS...r
-000026d0: 8800 0000 7255 0000 0072 5b00 0000 72a0  ....rU...r[...r.
-000026e0: 0000 0072 4600 0000 7216 0000 0072 1600  ...rF...r....r..
-000026f0: 0000 7214 0000 0072 1700 0000 7247 0000  ..r....r....rG..
-00002700: 0070 0000 0073 4a00 0000 0800 0401 0803  .p...sJ.........
-00002710: 0601 0601 0402 0401 0401 0401 0401 0401  ................
-00002720: 0602 0601 0401 1802 081b 0808 080e 1407  ................
-00002730: 080a 080a 0805 0805 041f 0a01 040c 0a01  ................
-00002740: 0435 0a01 0609 0a01 0409 0a01 040d 0a01  .5..............
-00002750: 080d 1201 7247 0000 0063 0000 0000 0000  ....rG...c......
-00002760: 0000 0000 0000 0000 0000 0500 0000 0000  ................
-00002770: 0000 73d8 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-00002780: 015a 0365 0465 0565 0683 025a 0765 0465  .Z.e.e.e...Z.e.e
-00002790: 0565 0583 025a 0865 0465 0583 015a 0965  .e...Z.e.e...Z.e
-000027a0: 055a 0a64 025a 0b64 025a 0c64 025a 0d64  .Z.d.Z.d.Z.d.Z.d
-000027b0: 025a 0e64 025a 0f64 1e64 0365 0564 0465  .Z.d.Z.d.d.e.d.e
-000027c0: 1066 0487 0066 0164 0564 0684 0d5a 1187  .f...f.d.d...Z..
-000027d0: 0066 0164 0764 0884 085a 1264 0964 0a84  .f.d.d...Z.d.d..
-000027e0: 005a 1364 0b64 0c84 005a 1464 0d64 0e84  .Z.d.d...Z.d.d..
-000027f0: 005a 1564 0f64 1084 005a 1664 1164 1284  .Z.d.d...Z.d.d..
-00002800: 005a 1765 1865 0565 0683 0264 1364 1484  .Z.e.e.e...d.d..
-00002810: 0083 015a 1965 1865 0565 0583 0264 1564  ...Z.e.e.e...d.d
-00002820: 1684 0083 015a 1a64 1f64 1864 1984 015a  .....Z.d.d.d...Z
-00002830: 1b64 1a64 1b84 005a 1c65 1883 0064 1c64  .d.d...Z.e...d.d
-00002840: 1d84 0083 015a 1d87 0004 005a 1e53 0029  .....Z.....Z.S.)
-00002850: 20da 0a53 7562 7363 7269 6265 727a 910a   ..Subscriberz..
-00002860: 2020 2020 5573 6572 2063 6f6e 6e65 6374      User connect
-00002870: 7320 746f 204d 756c 7469 7665 7273 6520  s to Multiverse 
-00002880: 6a75 7374 206c 696b 6520 632b 2b20 636f  just like c++ co
-00002890: 6465 0a20 2020 2053 7562 7363 7269 6265  de.    Subscribe
-000028a0: 7273 2061 7265 2075 7365 6420 6279 2061  rs are used by a
-000028b0: 6e79 2075 7365 7220 746f 2063 6f6e 6e65  ny user to conne
-000028c0: 6374 2074 6f20 6120 6e61 6d65 206f 7220  ct to a name or 
-000028d0: 6372 6561 7465 2061 206e 616d 6520 6f6e  create a name on
-000028e0: 204d 756c 7469 7665 7273 650a 2020 2020   Multiverse.    
-000028f0: 4e72 0d00 0000 da05 636c 6f75 6463 0600  Nr......cloudc..
-00002900: 0000 0000 0000 0000 0000 0700 0000 0400  ................
-00002910: 0000 0300 0000 73cc 0000 007c 0564 0175  ......s....|.d.u
-00002920: 0172 0b74 0083 00a0 017c 05a1 0101 006e  .r.t.....|.....n
-00002930: 0574 0083 00a0 01a1 0001 007c 027c 005f  .t.........|.|._
-00002940: 027c 006a 02a0 037c 01a1 017c 005f 047c  .|.j...|...|._.|
-00002950: 006a 04a0 05a1 007c 005f 067c 037c 005f  .j.....|._.|.|._
-00002960: 077c 047c 005f 087c 006a 046a 09a0 0a7c  .|.|._.|.j.j...|
-00002970: 006a 0ba1 0101 007c 006a 046a 0ca0 0a7c  .j.....|.j.j...|
-00002980: 006a 0da1 0101 007c 006a 0ea0 0a7c 006a  .j.....|.j...|.j
-00002990: 026a 0fa1 0101 007c 006a 04a0 10a1 0064  .j.....|.j.....d
-000029a0: 0275 0072 5864 037c 006a 0617 0064 0417  .u.rXd.|.j...d..
-000029b0: 007d 067c 006a 0ea0 117c 06a1 0101 007c  .}.|.j...|.....|
-000029c0: 006a 04a0 12a1 0001 006e 0774 13a0 1464  .j.......n.t...d
-000029d0: 057c 006a 15a1 0201 007c 006a 04a0 16a1  .|.j.....|.j....
-000029e0: 0001 0064 0153 0029 0661 9d01 0000 0a20  ...d.S.).a..... 
-000029f0: 2020 2020 2020 2053 756e 7363 7269 7074         Sunscript
-00002a00: 696f 6e0a 2020 2020 2020 2020 3a70 6172  ion.        :par
-00002a10: 616d 206e 616d 653a 2053 7562 7363 7269  am name: Subscri
-00002a20: 7074 696f 6e20 6e61 6d65 0a20 2020 2020  ption name.     
-00002a30: 2020 203a 7061 7261 6d20 636c 6f75 643a     :param cloud:
-00002a40: 204e 616d 6520 6f66 2074 6865 2073 7465   Name of the ste
-00002a50: 6351 536f 636b 6574 2063 6c6f 7564 0a20  cQSocket cloud. 
-00002a60: 2020 2020 2020 203a 7061 7261 6d20 4461         :param Da
-00002a70: 7461 4361 6c6c 4261 636b 3a20 4675 6e63  taCallBack: Func
-00002a80: 7469 6f6e 2061 2075 7365 7220 6361 6e20  tion a user can 
-00002a90: 7265 6369 6576 6520 6461 7461 2069 6620  recieve data if 
-00002aa0: 6465 7369 7265 642c 2061 6e64 2069 6620  desired, and if 
-00002ab0: 7468 6520 7573 6572 2064 6f65 7320 6e6f  the user does no
-00002ac0: 7420 7761 6e74 2074 6f20 7573 6520 7369  t want to use si
-00002ad0: 676e 616c 730a 2020 2020 2020 2020 3a70  gnals.        :p
-00002ae0: 6172 616d 2044 6573 6343 616c 6c42 6163  aram DescCallBac
-00002af0: 6b3a 2046 756e 6374 696f 6e20 6120 7573  k: Function a us
-00002b00: 6572 2063 616e 2072 6563 6965 7665 2064  er can recieve d
-00002b10: 6573 6363 6970 7469 6f6e 7320 6966 2064  escciptions if d
-00002b20: 6573 6972 6564 2c20 616e 6420 6966 2074  esired, and if t
-00002b30: 6865 2075 7365 7220 646f 6573 206e 6f74  he user does not
-00002b40: 2077 616e 7420 746f 2075 7365 2073 6967   want to use sig
-00002b50: 6e61 6c73 0a20 2020 2020 2020 203a 7061  nals.        :pa
-00002b60: 7261 6d20 5061 7265 6e74 3a20 514f 626a  ram Parent: QObj
-00002b70: 6563 7420 7061 7265 6e74 206f 7220 4e6f  ect parent or No
-00002b80: 6e65 0a20 2020 2020 2020 204e 4672 8000  ne.        NFr..
-00002b90: 0000 7281 0000 00e9 0a00 0000 2917 720e  ..r.........).r.
-00002ba0: 0000 0072 0f00 0000 72a4 0000 0072 6500  ...r....r....re.
-00002bb0: 0000 726b 0000 0072 2600 0000 720d 0000  ..rk...r&...r...
-00002bc0: 00da 0c66 756e 6374 696f 6e44 6174 61da  ...functionData.
-00002bd0: 0c66 756e 6374 696f 6e44 6573 6372 2700  .functionDescr'.
-00002be0: 0000 7250 0000 00da 076e 6577 4465 7363  ..rP.....newDesc
-00002bf0: 722a 0000 00da 076e 6577 4461 7461 da13  r*.....newData..
-00002c00: 7369 6755 7064 6174 654d 756c 7469 7665  sigUpdateMultive
-00002c10: 7273 6572 8800 0000 723d 0000 0072 2800  rser....r=...r(.
-00002c20: 0000 723c 0000 0072 0400 0000 da0a 7369  ..r<...r......si
-00002c30: 6e67 6c65 5368 6f74 da0f 5374 6172 7453  ngleShot..StartS
-00002c40: 696e 676c 6553 686f 7472 3700 0000 2907  ingleShotr7...).
-00002c50: 7211 0000 0072 0d00 0000 72a4 0000 00da  r....r....r.....
-00002c60: 0c44 6174 6143 616c 6c42 6163 6bda 0c44  .DataCallBack..D
-00002c70: 6573 6343 616c 6c42 6163 6b72 1200 0000  escCallBackr....
-00002c80: 728b 0000 0072 1400 0000 7216 0000 0072  r....r....r....r
-00002c90: 1700 0000 720f 0000 0090 0100 0073 2200  ....r........s".
-00002ca0: 0000 0809 0e01 0a02 0602 0e01 0c01 0601  ................
-00002cb0: 0601 1001 1001 1001 0e02 0e01 0c01 0c01  ................
-00002cc0: 0e03 0e02 7a13 5375 6273 6372 6962 6572  ....z.Subscriber
-00002cd0: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-00002ce0: 0000 0000 0000 0300 0000 0300 0000 0300  ................
-00002cf0: 0000 7346 0000 007c 006a 00a0 01a1 007d  ..sF...|.j.....}
-00002d00: 017c 0164 016b 0172 1c7c 006a 00a0 0264  .|.d.k.r.|.j...d
-00002d10: 02a1 0101 0064 037c 006a 0317 0064 0417  .....d.|.j...d..
-00002d20: 007d 027c 006a 04a0 057c 02a1 0101 0074  .}.|.j...|.....t
-00002d30: 0683 00a0 07a1 0001 0064 0553 0029 067a  .........d.S.).z
-00002d40: 2a0a 2020 2020 2020 2020 4465 6c65 7465  *.        Delete
-00002d50: 7320 6c61 7465 7220 696e 6865 7269 7469  s later inheriti
-00002d60: 6564 0a20 2020 2020 2020 2072 0100 0000  ed.        r....
-00002d70: 467a 0a52 454d 4f56 4553 5542 2c72 8100  Fz.REMOVESUB,r..
-00002d80: 0000 4e29 0872 6b00 0000 7238 0000 0072  ..N).rk...r8...r
-00002d90: 3c00 0000 720d 0000 0072 aa00 0000 7228  <...r....r....r(
-00002da0: 0000 0072 0e00 0000 da0b 6465 6c65 7465  ...r......delete
-00002db0: 4c61 7465 7229 0372 1100 0000 7236 0000  Later).r....r6..
-00002dc0: 0072 8b00 0000 7214 0000 0072 1600 0000  .r....r....r....
-00002dd0: 7217 0000 0072 af00 0000 b101 0000 730c  r....r........s.
-00002de0: 0000 000a 0408 010c 010e 010c 010e 027a  ...............z
-00002df0: 1653 7562 7363 7269 6265 722e 6465 6c65  .Subscriber.dele
-00002e00: 7465 4c61 7465 7263 0100 0000 0000 0000  teLaterc........
-00002e10: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00002e20: 7270 0000 0029 017a 310a 2020 2020 2020  rp...).z1.      
-00002e30: 2020 5573 6572 7320 6361 6e20 6174 7461    Users can atta
-00002e40: 6368 2075 7365 7220 6461 7461 2068 6572  ch user data her
-00002e50: 650a 2020 2020 2020 2020 a901 da08 7573  e.        ....us
-00002e60: 6572 4461 7461 722b 0000 0072 1600 0000  erDatar+...r....
-00002e70: 7216 0000 0072 1700 0000 da08 5573 6572  r....r......User
-00002e80: 4461 7461 be01 0000 7272 0000 007a 1353  Data....rr...z.S
-00002e90: 7562 7363 7269 6265 722e 5573 6572 4461  ubscriber.UserDa
-00002ea0: 7461 6302 0000 0000 0000 0000 0000 0002  tac.............
-00002eb0: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
-00002ec0: 7c01 7c00 5f00 6401 5300 2902 7a5b 0a20  |.|._.d.S.).z[. 
-00002ed0: 2020 2020 2020 2073 6574 7320 7573 6572         sets user
-00002ee0: 2064 6174 6120 6c6f 6361 6c6c 7920 666f   data locally fo
-00002ef0: 7220 7573 6572 2074 6f20 6465 6369 6465  r user to decide
-00002f00: 2077 6861 7420 746f 2064 6f20 7769 7468   what to do with
-00002f10: 2063 616e 2062 6520 616e 7974 6869 6e67   can be anything
-00002f20: 0a20 2020 2020 2020 204e 72b0 0000 0029  .        Nr....)
-00002f30: 0272 1100 0000 72b1 0000 0072 1600 0000  .r....r....r....
-00002f40: 7216 0000 0072 1700 0000 da0b 5365 7455  r....r......SetU
-00002f50: 7365 7244 6174 61c4 0100 00f3 0200 0000  serData.........
-00002f60: 0a04 7a16 5375 6273 6372 6962 6572 2e53  ..z.Subscriber.S
-00002f70: 6574 5573 6572 4461 7461 6301 0000 0000  etUserDatac.....
-00002f80: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00002f90: 0000 00f3 0a00 0000 7c00 6a00 a001 a100  ........|.j.....
-00002fa0: 5300 2901 7a30 0a20 2020 2020 2020 203a  S.).z0.        :
-00002fb0: 7265 7475 726e 3a20 5468 6520 6461 7461  return: The data
-00002fc0: 2069 6620 6974 2065 7869 7374 730a 2020   if it exists.  
-00002fd0: 2020 2020 2020 2902 726b 0000 0072 2100        ).rk...r!.
-00002fe0: 0000 722b 0000 0072 1600 0000 7216 0000  ..r+...r....r...
-00002ff0: 0072 1700 0000 da04 4461 7461 cb01 0000  .r......Data....
-00003000: 72b4 0000 007a 0f53 7562 7363 7269 6265  r....z.Subscribe
-00003010: 722e 4461 7461 6301 0000 0000 0000 0000  r.Datac.........
-00003020: 0000 0001 0000 0002 0000 0043 0000 0072  ...........C...r
-00003030: b500 0000 2901 7a30 0a20 2020 2020 2020  ....).z0.       
-00003040: 203a 7265 7475 726e 3a20 4465 7363 7269   :return: Descri
-00003050: 7074 696f 6e20 6966 2065 7869 7374 730a  ption if exists.
-00003060: 2020 2020 2020 2020 2902 726b 0000 0072          ).rk...r
-00003070: 2500 0000 722b 0000 0072 1600 0000 7216  %...r+...r....r.
-00003080: 0000 0072 1700 0000 da04 4465 7363 d101  ...r......Desc..
-00003090: 0000 72b4 0000 007a 0f53 7562 7363 7269  ..r....z.Subscri
-000030a0: 6265 722e 4465 7363 6301 0000 0000 0000  ber.Descc.......
-000030b0: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-000030c0: 0072 7000 0000 7218 0000 0029 01da 044e  .rp...r....)...N
-000030d0: 616d 6572 2b00 0000 7216 0000 0072 1600  amer+...r....r..
-000030e0: 0000 7217 0000 0072 b800 0000 d701 0000  ..r....r........
-000030f0: 7302 0000 0006 017a 0f53 7562 7363 7269  s......z.Subscri
-00003100: 6265 722e 4e61 6d65 6303 0000 0000 0000  ber.Namec.......
-00003110: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
-00003120: 0073 2c00 0000 7c00 6a00 a001 7c01 7c02  .s,...|.j...|.|.
-00003130: a102 0100 7c00 6a02 6401 7501 7214 7c00  ....|.j.d.u.r.|.
-00003140: a002 7c01 7c02 a102 0100 6401 5300 6401  ..|.|.....d.S.d.
-00003150: 5300 2902 7a6f 0a20 2020 2020 2020 2069  S.).zo.        i
-00003160: 6e74 656e 616c 2075 7365 0a20 2020 2020  ntenal use.     
-00003170: 2020 203a 7061 7261 6d20 6e61 6d65 3a20     :param name: 
-00003180: 7375 6273 6372 6970 7469 6f6e 206e 616d  subscription nam
-00003190: 650a 2020 2020 2020 2020 3a70 6172 616d  e.        :param
-000031a0: 2064 6174 613a 2044 6174 610a 2020 2020   data: Data.    
-000031b0: 2020 2020 3a72 6574 7572 6e3a 0a20 2020      :return:.   
-000031c0: 2020 2020 204e 2903 da0d 7369 6755 7064       N)...sigUpd
-000031d0: 6174 6544 6174 6172 2800 0000 72a6 0000  ateDatar(...r...
-000031e0: 0029 0372 1100 0000 720d 0000 0072 1b00  .).r....r....r..
-000031f0: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00003200: 0072 a900 0000 d901 0000 7308 0000 000e  .r........s.....
-00003210: 080a 0110 0104 ff7a 1253 7562 7363 7269  .......z.Subscri
-00003220: 6265 722e 6e65 7744 6174 6163 0300 0000  ber.newDatac....
-00003230: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00003240: 4300 0000 733e 0000 007c 017c 006a 006b  C...s>...|.|.j.k
-00003250: 0272 1b7c 006a 01a0 027c 006a 007c 02a1  .r.|.j...|.j.|..
-00003260: 0201 007c 006a 0364 0175 0172 1d7c 00a0  ...|.j.d.u.r.|..
-00003270: 037c 006a 007c 02a1 0201 0064 0153 0064  .|.j.|.....d.S.d
-00003280: 0153 0064 0153 0029 027a 6b0a 2020 2020  .S.d.S.).zk.    
-00003290: 2020 2020 696e 7465 726e 616c 2075 7365      internal use
-000032a0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000032b0: 6465 7363 3a20 6e65 7720 6465 7363 7269  desc: new descri
-000032c0: 7074 696f 6e20 636f 6d69 6e67 2066 726f  ption coming fro
-000032d0: 6d20 6d75 6c74 6976 6572 7365 0a20 2020  m multiverse.   
-000032e0: 2020 2020 203a 7265 7475 726e 3a0a 2020       :return:.  
-000032f0: 2020 2020 2020 4e29 0472 0d00 0000 da0d        N).r......
-00003300: 7369 6755 7064 6174 6544 6573 6372 2800  sigUpdateDescr(.
-00003310: 0000 72a7 0000 0029 0372 1100 0000 720d  ..r....).r....r.
-00003320: 0000 0072 2300 0000 7216 0000 0072 1600  ...r#...r....r..
-00003330: 0000 7217 0000 0072 a800 0000 e501 0000  ..r....r........
-00003340: 730c 0000 000a 0710 010a 0112 0104 fd04  s...............
-00003350: 027a 1253 7562 7363 7269 6265 722e 6e65  .z.Subscriber.ne
-00003360: 7744 6573 6372 0100 0000 6303 0000 0000  wDescr....c.....
-00003370: 0000 0000 0000 0006 0000 0005 0000 0043  ...............C
-00003380: 0000 0073 fa00 0000 7400 7c01 8301 7277  ...s....t.|...rw
-00003390: 7401 7c01 6401 1900 7402 8302 7217 6402  t.|.d...t...r.d.
-000033a0: 7c00 6a03 1700 6403 1700 7404 7c02 8301  |.j...d...t.|...
-000033b0: 1700 7d03 6e31 7401 7c01 6401 1900 7405  ..}.n1t.|.d...t.
-000033c0: 8302 722a 6404 7c00 6a03 1700 6403 1700  ..r*d.|.j...d...
-000033d0: 7404 7c02 8301 1700 7d03 6e1e 7401 7c01  t.|.....}.n.t.|.
-000033e0: 6401 1900 7406 8302 723d 6405 7c00 6a03  d...t...r=d.|.j.
-000033f0: 1700 6403 1700 7404 7c02 8301 1700 7d03  ..d...t.|.....}.
-00003400: 6e0b 6406 7c00 6a03 1700 6403 1700 7404  n.d.|.j...d...t.
-00003410: 7c02 8301 1700 7d03 7c01 4400 5d0a 7d04  |.....}.|.D.].}.
-00003420: 7c03 6403 7404 7c04 8301 1700 3700 7d03  |.d.t.|.....7.}.
-00003430: 714a 7c03 6407 3700 7d03 7c00 6a07 a008  qJ|.d.7.}.|.j...
-00003440: 7c03 a101 0100 7c00 6a09 a00a a100 7d05  |.....|.j.....}.
-00003450: 7c05 6408 7500 7279 7c00 6a0b a00c a100  |.d.u.ry|.j.....
-00003460: 6409 7500 727b 7c00 6a09 a00d 7c01 a101  d.u.r{|.j...|...
-00003470: 0100 640a 5300 640a 5300 640a 5300 640a  ..d.S.d.S.d.S.d.
-00003480: 5300 290b 7ac9 0a20 2020 2020 2020 2055  S.).z..        U
-00003490: 7365 7220 6361 6e20 7570 6461 7465 206d  ser can update m
-000034a0: 756c 7469 7665 7273 6520 7769 7468 2064  ultiverse with d
-000034b0: 6174 610a 2020 2020 2020 2020 3a70 6172  ata.        :par
-000034c0: 616d 2077 6861 743a 2044 6174 6120 746f  am what: Data to
-000034d0: 2073 656e 6420 746f 204d 756c 6976 6572   send to Muliver
-000034e0: 7365 0a20 2020 2020 2020 203a 7061 7261  se.        :para
-000034f0: 6d20 696e 6465 783a 2020 5a65 726f 2064  m index:  Zero d
-00003500: 6566 6175 6c74 2c20 6275 7420 6974 2063  efault, but it c
-00003510: 616e 2062 6520 7365 6e74 2069 6e20 7468  an be sent in th
-00003520: 6520 6d69 6464 6c65 206f 6620 616e 2061  e middle of an a
-00003530: 7272 6172 790a 2020 2020 2020 2020 3a72  rrary.        :r
-00003540: 6574 7572 6e3a 0a20 2020 2020 2020 2072  eturn:.        r
-00003550: 0100 0000 7282 0000 0072 8300 0000 7284  ....r....r....r.
-00003560: 0000 0072 8500 0000 7286 0000 0072 8100  ...r....r....r..
-00003570: 0000 5446 4e29 0e72 7800 0000 7289 0000  ..TFN).rx...r...
-00003580: 0072 4c00 0000 720d 0000 0072 4200 0000  .rL...r....rB...
-00003590: 728a 0000 0072 4500 0000 72aa 0000 0072  r....rE...r....r
-000035a0: 2800 0000 726b 0000 0072 3200 0000 72a4  (...rk...r2...r.
-000035b0: 0000 0072 6f00 0000 721f 0000 0029 0672  ...ro...r....).r
-000035c0: 1100 0000 728c 0000 0072 8d00 0000 728b  ....r....r....r.
-000035d0: 0000 0072 8e00 0000 da06 6d61 7374 6572  ...r......master
-000035e0: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
-000035f0: 0a55 7064 6174 6544 6174 61f1 0100 0073  .UpdateData....s
-00003600: 2200 0000 0807 0e02 1801 0e02 1801 0e02  "...............
-00003610: 1801 1603 0802 1201 0801 0c02 0a01 1601  ................
-00003620: 1001 04eb 0814 7a15 5375 6273 6372 6962  ......z.Subscrib
-00003630: 6572 2e55 7064 6174 6544 6174 6163 0200  er.UpdateDatac..
-00003640: 0000 0000 0000 0000 0000 0400 0000 0300  ................
-00003650: 0000 4300 0000 735e 0000 0064 017c 006a  ..C...s^...d.|.j
-00003660: 0017 0064 0217 007c 0117 007d 027c 0264  ...d...|...}.|.d
-00003670: 0337 007d 027c 006a 01a0 027c 02a1 0101  .7.}.|.j...|....
-00003680: 007c 006a 03a0 04a1 007d 037c 0364 0475  .|.j.....}.|.d.u
-00003690: 0072 2b7c 006a 05a0 06a1 0064 0575 0072  .r+|.j.....d.u.r
-000036a0: 2d7c 006a 03a0 077c 01a1 0101 0064 0653  -|.j...|.....d.S
-000036b0: 0064 0653 0064 0653 0029 077a 880a 2020  .d.S.d.S.).z..  
-000036c0: 2020 2020 2020 6966 2077 6520 6172 6520        if we are 
-000036d0: 7468 6520 676f 6c64 656e 2063 6f70 792c  the golden copy,
-000036e0: 2077 6520 6361 6e20 7365 6e64 2061 204d   we can send a M
-000036f0: 616c 636f 6c6d 2070 726f 6f66 2064 6573  alcolm proof des
-00003700: 6372 6970 746f 720a 2020 2020 2020 2020  criptor.        
-00003710: 3a70 6172 616d 2077 6861 743a 2074 6865  :param what: the
-00003720: 2064 6573 6372 6970 746f 720a 2020 2020   descriptor.    
-00003730: 2020 2020 3a72 6574 7572 6e3a 0a20 2020      :return:.   
-00003740: 2020 2020 2072 8700 0000 7283 0000 0072       r....r....r
-00003750: 8100 0000 5446 4e29 0872 0d00 0000 72aa  ....TFN).r....r.
-00003760: 0000 0072 2800 0000 726b 0000 0072 3200  ...r(...rk...r2.
-00003770: 0000 72a4 0000 0072 6f00 0000 7229 0000  ..r....ro...r)..
-00003780: 0029 0472 1100 0000 728c 0000 0072 8b00  .).r....r....r..
-00003790: 0000 72bb 0000 0072 1600 0000 7216 0000  ..r....r....r...
-000037a0: 0072 1700 0000 da0a 5570 6461 7465 4465  .r......UpdateDe
-000037b0: 7363 0f02 0000 730e 0000 0012 0608 010c  sc....s.........
-000037c0: 010a 0116 0110 0108 ff7a 1553 7562 7363  .........z.Subsc
-000037d0: 7269 6265 722e 5570 6461 7465 4465 7363  riber.UpdateDesc
-000037e0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-000037f0: 0005 0000 0043 0000 0073 4800 0000 7c00  .....C...sH...|.
-00003800: a000 a100 7d01 7c01 6401 7501 7211 7c00  ....}.|.d.u.r.|.
-00003810: a001 7c00 6a02 7c00 a000 a100 a102 0100  ..|.j.|.........
-00003820: 7c00 a003 a100 7d02 7c02 6401 7501 7222  |.....}.|.d.u.r"
-00003830: 7c00 a004 7c00 6a02 7c02 a102 0100 6401  |...|.j.|.....d.
-00003840: 5300 6401 5300 2902 7a2f 0a20 2020 2020  S.d.S.).z/.     
-00003850: 2020 2069 6e74 6572 616e 6c20 7573 650a     interanl use.
-00003860: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00003870: 0a20 2020 2020 2020 204e 2905 72b6 0000  .        N).r...
-00003880: 0072 a900 0000 720d 0000 0072 b700 0000  .r....r....r....
-00003890: 72a8 0000 0029 0372 1100 0000 721b 0000  r....).r....r...
-000038a0: 0072 2300 0000 7216 0000 0072 1600 0000  .r#...r....r....
-000038b0: 7217 0000 0072 ac00 0000 1c02 0000 730e  r....r........s.
-000038c0: 0000 0008 0608 0112 0108 0208 0112 0104  ................
-000038d0: ff7a 1a53 7562 7363 7269 6265 722e 5374  .z.Subscriber.St
-000038e0: 6172 7453 696e 676c 6553 686f 7429 034e  artSingleShot).N
-000038f0: 4e4e 2901 7201 0000 0029 1f72 3e00 0000  NN).r....).r>...
-00003900: 723f 0000 0072 4000 0000 7241 0000 0072  r?...r@...rA...r
-00003910: 0700 0000 7242 0000 0072 4300 0000 72b9  ....rB...rC...r.
-00003920: 0000 0072 ba00 0000 72aa 0000 0072 0d00  ...r....r....r..
-00003930: 0000 726b 0000 0072 a400 0000 72b1 0000  ..rk...r....r...
-00003940: 0072 a600 0000 72a7 0000 0072 4700 0000  .r....r....rG...
-00003950: 720f 0000 0072 af00 0000 72b2 0000 0072  r....r....r....r
-00003960: b300 0000 72b6 0000 0072 b700 0000 72b8  ....r....r....r.
-00003970: 0000 0072 0600 0000 72a9 0000 0072 a800  ...r....r....r..
-00003980: 0000 72bc 0000 0072 bd00 0000 72ac 0000  ..r....r....r...
-00003990: 0072 4600 0000 7216 0000 0072 1600 0000  .rF...r....r....
-000039a0: 7214 0000 0072 1700 0000 72a3 0000 007f  r....r....r.....
-000039b0: 0100 0073 3400 0000 0800 0401 0a04 0a01  ...s4...........
-000039c0: 0801 0402 0401 0401 0401 0402 0401 1802  ................
-000039d0: 0c21 080d 0806 0807 0806 0806 0802 0a01  .!..............
-000039e0: 080b 0a01 0a0b 081e 040d 1201 72a3 0000  ............r...
-000039f0: 00da 085f 5f6d 6169 6e5f 5f29 01da 1152  ...__main__)...R
-00003a00: 6574 656e 7369 6f6e 5365 7474 696e 6773  etensionSettings
-00003a10: da08 7374 6463 6f6d 5174 7a09 2d2d 7665  ..stdcomQtz.--ve
-00003a20: 7273 696f 6eda 0668 656c 6c6f 3254 da07  rsion..hello2T..
-00003a30: 5465 7374 696e 6729 0372 0100 0000 72a5  Testing).r....r.
-00003a40: 0000 00e9 1400 0000 2903 e9de 0000 0072  ........)......r
-00003a50: a500 0000 72c3 0000 007a 0f68 656c 6c6f  ....r....z.hello
-00003a60: 2e72 6573 7369 6465 6e74 2929 da0c 5079  .ressident))..Py
-00003a70: 5174 352e 5174 436f 7265 7202 0000 0072  Qt5.QtCorer....r
-00003a80: 0300 0000 7204 0000 0072 0500 0000 7206  ....r....r....r.
-00003a90: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
-00003aa0: 0000 da0f 5079 5174 352e 5174 4e65 7477  ....PyQt5.QtNetw
-00003ab0: 6f72 6b72 0a00 0000 720b 0000 0072 9800  orkr....r....r..
-00003ac0: 0000 da0f 7374 6463 6f6d 5174 5665 7273  ....stdcomQtVers
-00003ad0: 696f 6e72 0c00 0000 7247 0000 0072 a300  ionr....rG...r..
-00003ae0: 0000 723e 0000 00da 0f73 7464 636f 6d76  ..r>.....stdcomv
-00003af0: 7365 7474 696e 6773 72bf 0000 00da 0252  settingsr......R
-00003b00: 5372 9d00 0000 da03 7379 73da 0461 7267  Sr......sys..arg
-00003b10: 76da 0465 7869 74da 0361 7070 da01 77da  v..exit..app..w.
-00003b20: 0168 726c 0000 0072 bd00 0000 72bc 0000  .hrl...r....r...
-00003b30: 00da 0268 68da 0c72 6573 6964 656e 7454  ...hh..residentT
-00003b40: 6578 74da 0c72 6573 6964 656e 7454 6573  ext..residentTes
-00003b50: 74da 0872 7365 7474 696e 67da 0f47 6574  t..rsetting..Get
-00003b60: 5265 7369 6465 6e74 4461 7461 721b 0000  ResidentDatar...
-00003b70: 0072 b600 0000 da10 5361 7665 5265 7369  .r......SaveResi
-00003b80: 6465 6e74 4461 7461 da05 6578 6563 5f72  dentData..exec_r
-00003b90: 5f00 0000 7216 0000 0072 1600 0000 7216  _...r....r....r.
-00003ba0: 0000 0072 1700 0000 da08 3c6d 6f64 756c  ...r......<modul
-00003bb0: 653e 0100 0000 7358 0000 0028 0010 0108  e>....sX...(....
-00003bc0: 0104 0310 0110 6900 7f00 7f10 1100 7f08  ......i.........
-00003bd0: 330c 0208 0208 010a 0208 0108 010a 0206  3...............
-00003be0: 010a 020c 010a 020e 010a 020e 0104 020a  ................
-00003bf0: 0106 020a 0108 0202 0208 0102 0208 0106  ................
-00003c00: 0102 020a 0102 020e 010a 0308 0508 010e  ................
-00003c10: 0104 cc                                  ...
+00002510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002520: 2020 2063 6f6e 6e65 6374 696f 6e2c 2062     connection, b
+00002530: 7920 686f 7374 2061 6e64 2070 6f72 740a  y host and port.
+00002540: 2020 2020 2020 2020 3a70 6172 616d 2068          :param h
+00002550: 6f73 743a 0a20 2020 2020 2020 203a 7061  ost:.        :pa
+00002560: 7261 6d20 706f 7274 3a0a 2020 2020 2020  ram port:.      
+00002570: 2020 3a72 6574 7572 6e3a 0a20 2020 2020    :return:.     
+00002580: 2020 2054 4e29 0972 5900 0000 725f 0000     TN).rY...r_..
+00002590: 0072 4b00 0000 724e 0000 0072 7000 0000  .rK...rN...rp...
+000025a0: 724f 0000 0072 5e00 0000 725c 0000 0072  rO...r^...r\...r
+000025b0: 5d00 0000 2903 7212 0000 0072 4b00 0000  ]...).r....rK...
+000025c0: 724c 0000 0072 1700 0000 7217 0000 0072  rL...r....r....r
+000025d0: 1800 0000 da0b 536c 6f74 4e65 7748 6f73  ......SlotNewHos
+000025e0: 746f 0100 0073 0e00 0000 0a08 0601 0601  to...s..........
+000025f0: 0c02 0a01 0802 0e01 7a17 7374 6563 5153  ........z.stecQS
+00002600: 6f63 6b65 742e 536c 6f74 4e65 7748 6f73  ocket.SlotNewHos
+00002610: 7429 0372 4900 0000 724a 0000 004e 2902  t).rI...rJ...N).
+00002620: 7269 0000 0054 2928 723f 0000 0072 4000  ri...T)(r?...r@.
+00002630: 0000 7241 0000 0072 4200 0000 7207 0000  ..rA...rB...r...
+00002640: 0072 4400 0000 727b 0000 00da 0773 6967  .rD...r{.....sig
+00002650: 446f 776e da06 7369 676e 5570 724e 0000  Down..signUprN..
+00002660: 0072 4b00 0000 7259 0000 0072 4f00 0000  .rK...rY...rO...
+00002670: 7213 0000 0072 5000 0000 7202 0000 0072  r....rP...r....r
+00002680: 6100 0000 726f 0000 0072 6200 0000 7243  a...ro...rb...rC
+00002690: 0000 0072 4d00 0000 7210 0000 0072 6000  ...rM...r....r`.
+000026a0: 0000 7266 0000 0072 6800 0000 7246 0000  ..rf...rh...rF..
+000026b0: 0072 6d00 0000 7270 0000 0072 7200 0000  .rm...rp...rr...
+000026c0: 7274 0000 0072 7f00 0000 7206 0000 0072  rt...r....r....r
+000026d0: 5800 0000 7252 0000 0072 5400 0000 7289  X...rR...rT...r.
+000026e0: 0000 0072 5600 0000 725c 0000 0072 a100  ...rV...r\...r..
+000026f0: 0000 7247 0000 0072 1700 0000 7217 0000  ..rG...r....r...
+00002700: 0072 1500 0000 7218 0000 0072 4800 0000  .r....r....rH...
+00002710: 7400 0000 734a 0000 0008 0004 0108 0306  t...sJ..........
+00002720: 0106 0104 0204 0104 0104 0104 0104 0106  ................
+00002730: 0206 0104 0118 0208 1b08 0808 0e14 0708  ................
+00002740: 0a08 0a08 0508 0504 1f0a 0104 0c0a 0104  ................
+00002750: 350a 0106 090a 0104 090a 0104 0d0a 0108  5...............
+00002760: 0d12 0172 4800 0000 6300 0000 0000 0000  ...rH...c.......
+00002770: 0000 0000 0000 0000 0005 0000 0000 0000  ................
+00002780: 0073 f200 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+00002790: 5a03 6504 6505 6506 8302 5a07 6504 6505  Z.e.e.e...Z.e.e.
+000027a0: 6505 8302 5a08 6504 6505 8301 5a09 6505  e...Z.e.e...Z.e.
+000027b0: 5a0a 6402 5a0b 6402 5a0c 6402 5a0d 6402  Z.d.Z.d.Z.d.Z.d.
+000027c0: 5a0e 6402 5a0f 6403 5a10 6424 6404 6505  Z.d.Z.d.Z.d$d.e.
+000027d0: 6405 6511 6604 8700 6601 6406 6407 840d  d.e.f...f.d.d...
+000027e0: 5a12 8700 6601 6408 6409 8408 5a13 640a  Z...f.d.d...Z.d.
+000027f0: 640b 8400 5a14 640c 640d 8400 5a15 640e  d...Z.d.d...Z.d.
+00002800: 640f 8400 5a16 6410 6411 8400 5a17 6412  d...Z.d.d...Z.d.
+00002810: 6413 8400 5a18 6519 6505 6506 8302 6414  d...Z.e.e.e...d.
+00002820: 6415 8400 8301 5a1a 6519 6505 6505 8302  d.....Z.e.e.e...
+00002830: 6416 6417 8400 8301 5a1b 6425 6419 641a  d.d.....Z.d%d.d.
+00002840: 8401 5a1c 641b 6700 6602 641c 641d 8404  ..Z.d.g.f.d.d...
+00002850: 5a1d 641e 641f 8400 5a1e 6420 6421 8400  Z.d.d...Z.d d!..
+00002860: 5a1f 6519 8300 6422 6423 8400 8301 5a20  Z.e...d"d#....Z 
+00002870: 8700 0400 5a21 5300 2926 da0a 5375 6273  ....Z!S.)&..Subs
+00002880: 6372 6962 6572 7a91 0a20 2020 2055 7365  criberz..    Use
+00002890: 7220 636f 6e6e 6563 7473 2074 6f20 4d75  r connects to Mu
+000028a0: 6c74 6976 6572 7365 206a 7573 7420 6c69  ltiverse just li
+000028b0: 6b65 2063 2b2b 2063 6f64 650a 2020 2020  ke c++ code.    
+000028c0: 5375 6273 6372 6962 6572 7320 6172 6520  Subscribers are 
+000028d0: 7573 6564 2062 7920 616e 7920 7573 6572  used by any user
+000028e0: 2074 6f20 636f 6e6e 6563 7420 746f 2061   to connect to a
+000028f0: 206e 616d 6520 6f72 2063 7265 6174 6520   name or create 
+00002900: 6120 6e61 6d65 206f 6e20 4d75 6c74 6976  a name on Multiv
+00002910: 6572 7365 0a20 2020 204e 4672 0e00 0000  erse.    NFr....
+00002920: da05 636c 6f75 6463 0600 0000 0000 0000  ..cloudc........
+00002930: 0000 0000 0700 0000 0400 0000 0300 0000  ................
+00002940: 73d2 0000 007c 0564 0175 0172 0b74 0083  s....|.d.u.r.t..
+00002950: 00a0 017c 05a1 0101 006e 0574 0083 00a0  ...|.....n.t....
+00002960: 01a1 0001 0064 027c 005f 027c 027c 005f  .....d.|._.|.|._
+00002970: 037c 006a 03a0 047c 01a1 017c 005f 057c  .|.j...|...|._.|
+00002980: 006a 05a0 06a1 007c 005f 077c 037c 005f  .j.....|._.|.|._
+00002990: 087c 047c 005f 097c 006a 056a 0aa0 0b7c  .|.|._.|.j.j...|
+000029a0: 006a 0ca1 0101 007c 006a 056a 0da0 0b7c  .j.....|.j.j...|
+000029b0: 006a 0ea1 0101 007c 006a 0fa0 0b7c 006a  .j.....|.j...|.j
+000029c0: 036a 10a1 0101 007c 006a 05a0 11a1 0064  .j.....|.j.....d
+000029d0: 0275 0072 5b64 037c 006a 0717 0064 0417  .u.r[d.|.j...d..
+000029e0: 007d 067c 006a 0fa0 127c 06a1 0101 007c  .}.|.j...|.....|
+000029f0: 006a 05a0 13a1 0001 006e 0774 14a0 1564  .j.......n.t...d
+00002a00: 057c 006a 16a1 0201 007c 006a 05a0 17a1  .|.j.....|.j....
+00002a10: 0001 0064 0153 0029 0661 9d01 0000 0a20  ...d.S.).a..... 
+00002a20: 2020 2020 2020 2053 756e 7363 7269 7074         Sunscript
+00002a30: 696f 6e0a 2020 2020 2020 2020 3a70 6172  ion.        :par
+00002a40: 616d 206e 616d 653a 2053 7562 7363 7269  am name: Subscri
+00002a50: 7074 696f 6e20 6e61 6d65 0a20 2020 2020  ption name.     
+00002a60: 2020 203a 7061 7261 6d20 636c 6f75 643a     :param cloud:
+00002a70: 204e 616d 6520 6f66 2074 6865 2073 7465   Name of the ste
+00002a80: 6351 536f 636b 6574 2063 6c6f 7564 0a20  cQSocket cloud. 
+00002a90: 2020 2020 2020 203a 7061 7261 6d20 4461         :param Da
+00002aa0: 7461 4361 6c6c 4261 636b 3a20 4675 6e63  taCallBack: Func
+00002ab0: 7469 6f6e 2061 2075 7365 7220 6361 6e20  tion a user can 
+00002ac0: 7265 6369 6576 6520 6461 7461 2069 6620  recieve data if 
+00002ad0: 6465 7369 7265 642c 2061 6e64 2069 6620  desired, and if 
+00002ae0: 7468 6520 7573 6572 2064 6f65 7320 6e6f  the user does no
+00002af0: 7420 7761 6e74 2074 6f20 7573 6520 7369  t want to use si
+00002b00: 676e 616c 730a 2020 2020 2020 2020 3a70  gnals.        :p
+00002b10: 6172 616d 2044 6573 6343 616c 6c42 6163  aram DescCallBac
+00002b20: 6b3a 2046 756e 6374 696f 6e20 6120 7573  k: Function a us
+00002b30: 6572 2063 616e 2072 6563 6965 7665 2064  er can recieve d
+00002b40: 6573 6363 6970 7469 6f6e 7320 6966 2064  escciptions if d
+00002b50: 6573 6972 6564 2c20 616e 6420 6966 2074  esired, and if t
+00002b60: 6865 2075 7365 7220 646f 6573 206e 6f74  he user does not
+00002b70: 2077 616e 7420 746f 2075 7365 2073 6967   want to use sig
+00002b80: 6e61 6c73 0a20 2020 2020 2020 203a 7061  nals.        :pa
+00002b90: 7261 6d20 5061 7265 6e74 3a20 514f 626a  ram Parent: QObj
+00002ba0: 6563 7420 7061 7265 6e74 206f 7220 4e6f  ect parent or No
+00002bb0: 6e65 0a20 2020 2020 2020 204e 4672 8100  ne.        NFr..
+00002bc0: 0000 7282 0000 00e9 0a00 0000 2918 720f  ..r.........).r.
+00002bd0: 0000 0072 1000 0000 da12 7265 7369 6465  ...r......reside
+00002be0: 6e74 5375 6273 6372 6962 6572 72a5 0000  ntSubscriberr...
+00002bf0: 0072 6600 0000 726c 0000 0072 2700 0000  .rf...rl...r'...
+00002c00: 720e 0000 00da 0c66 756e 6374 696f 6e44  r......functionD
+00002c10: 6174 61da 0c66 756e 6374 696f 6e44 6573  ata..functionDes
+00002c20: 6372 2800 0000 7251 0000 00da 076e 6577  cr(...rQ.....new
+00002c30: 4465 7363 722b 0000 00da 076e 6577 4461  Descr+.....newDa
+00002c40: 7461 da13 7369 6755 7064 6174 654d 756c  ta..sigUpdateMul
+00002c50: 7469 7665 7273 6572 8900 0000 723e 0000  tiverser....r>..
+00002c60: 0072 2900 0000 723d 0000 0072 0400 0000  .r)...r=...r....
+00002c70: da0a 7369 6e67 6c65 5368 6f74 da0f 5374  ..singleShot..St
+00002c80: 6172 7453 696e 676c 6553 686f 7472 3800  artSingleShotr8.
+00002c90: 0000 2907 7212 0000 0072 0e00 0000 72a5  ..).r....r....r.
+00002ca0: 0000 00da 0c44 6174 6143 616c 6c42 6163  .....DataCallBac
+00002cb0: 6bda 0c44 6573 6343 616c 6c42 6163 6b72  k..DescCallBackr
+00002cc0: 1300 0000 728c 0000 0072 1500 0000 7217  ....r....r....r.
+00002cd0: 0000 0072 1800 0000 7210 0000 0095 0100  ...r....r.......
+00002ce0: 0073 2400 0000 0809 0e01 0a02 0602 0601  .s$.............
+00002cf0: 0e01 0c01 0601 0601 1001 1001 1001 0e02  ................
+00002d00: 0e01 0c01 0c01 0e03 0e02 7a13 5375 6273  ..........z.Subs
+00002d10: 6372 6962 6572 2e5f 5f69 6e69 745f 5f63  criber.__init__c
+00002d20: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+00002d30: 0300 0000 0300 0000 7346 0000 007c 006a  ........sF...|.j
+00002d40: 00a0 01a1 007d 017c 0164 016b 0172 1c7c  .....}.|.d.k.r.|
+00002d50: 006a 00a0 0264 02a1 0101 0064 037c 006a  .j...d.....d.|.j
+00002d60: 0317 0064 0417 007d 027c 006a 04a0 057c  ...d...}.|.j...|
+00002d70: 02a1 0101 0074 0683 00a0 07a1 0001 0064  .....t.........d
+00002d80: 0553 0029 067a 2a0a 2020 2020 2020 2020  .S.).z*.        
+00002d90: 4465 6c65 7465 7320 6c61 7465 7220 696e  Deletes later in
+00002da0: 6865 7269 7469 6564 0a20 2020 2020 2020  heritied.       
+00002db0: 2072 0100 0000 467a 0a52 454d 4f56 4553   r....Fz.REMOVES
+00002dc0: 5542 2c72 8200 0000 4e29 0872 6c00 0000  UB,r....N).rl...
+00002dd0: 7239 0000 0072 3d00 0000 720e 0000 0072  r9...r=...r....r
+00002de0: ac00 0000 7229 0000 0072 0f00 0000 da0b  ....r)...r......
+00002df0: 6465 6c65 7465 4c61 7465 7229 0372 1200  deleteLater).r..
+00002e00: 0000 7237 0000 0072 8c00 0000 7215 0000  ..r7...r....r...
+00002e10: 0072 1700 0000 7218 0000 0072 b100 0000  .r....r....r....
+00002e20: b701 0000 730c 0000 000a 0408 010c 010e  ....s...........
+00002e30: 010c 010e 027a 1653 7562 7363 7269 6265  .....z.Subscribe
+00002e40: 722e 6465 6c65 7465 4c61 7465 7263 0100  r.deleteLaterc..
+00002e50: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+00002e60: 0000 4300 0000 7271 0000 0029 017a 310a  ..C...rq...).z1.
+00002e70: 2020 2020 2020 2020 5573 6572 7320 6361          Users ca
+00002e80: 6e20 6174 7461 6368 2075 7365 7220 6461  n attach user da
+00002e90: 7461 2068 6572 650a 2020 2020 2020 2020  ta here.        
+00002ea0: a901 da08 7573 6572 4461 7461 722c 0000  ....userDatar,..
+00002eb0: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00002ec0: da08 5573 6572 4461 7461 c401 0000 7273  ..UserData....rs
+00002ed0: 0000 007a 1353 7562 7363 7269 6265 722e  ...z.Subscriber.
+00002ee0: 5573 6572 4461 7461 6302 0000 0000 0000  UserDatac.......
+00002ef0: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
+00002f00: 0073 0a00 0000 7c01 7c00 5f00 6401 5300  .s....|.|._.d.S.
+00002f10: 2902 7a5b 0a20 2020 2020 2020 2073 6574  ).z[.        set
+00002f20: 7320 7573 6572 2064 6174 6120 6c6f 6361  s user data loca
+00002f30: 6c6c 7920 666f 7220 7573 6572 2074 6f20  lly for user to 
+00002f40: 6465 6369 6465 2077 6861 7420 746f 2064  decide what to d
+00002f50: 6f20 7769 7468 2063 616e 2062 6520 616e  o with can be an
+00002f60: 7974 6869 6e67 0a20 2020 2020 2020 204e  ything.        N
+00002f70: 72b2 0000 0029 0272 1200 0000 72b3 0000  r....).r....r...
+00002f80: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00002f90: da0b 5365 7455 7365 7244 6174 61ca 0100  ..SetUserData...
+00002fa0: 00f3 0200 0000 0a04 7a16 5375 6273 6372  ........z.Subscr
+00002fb0: 6962 6572 2e53 6574 5573 6572 4461 7461  iber.SetUserData
+00002fc0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00002fd0: 0002 0000 0043 0000 00f3 0a00 0000 7c00  .....C........|.
+00002fe0: 6a00 a001 a100 5300 2901 7a30 0a20 2020  j.....S.).z0.   
+00002ff0: 2020 2020 203a 7265 7475 726e 3a20 5468       :return: Th
+00003000: 6520 6461 7461 2069 6620 6974 2065 7869  e data if it exi
+00003010: 7374 730a 2020 2020 2020 2020 2902 726c  sts.        ).rl
+00003020: 0000 0072 2200 0000 722c 0000 0072 1700  ...r"...r,...r..
+00003030: 0000 7217 0000 0072 1800 0000 da04 4461  ..r....r......Da
+00003040: 7461 d101 0000 72b6 0000 007a 0f53 7562  ta....r....z.Sub
+00003050: 7363 7269 6265 722e 4461 7461 6301 0000  scriber.Datac...
+00003060: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00003070: 0043 0000 0072 b700 0000 2901 7a30 0a20  .C...r....).z0. 
+00003080: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00003090: 4465 7363 7269 7074 696f 6e20 6966 2065  Description if e
+000030a0: 7869 7374 730a 2020 2020 2020 2020 2902  xists.        ).
+000030b0: 726c 0000 0072 2600 0000 722c 0000 0072  rl...r&...r,...r
+000030c0: 1700 0000 7217 0000 0072 1800 0000 da04  ....r....r......
+000030d0: 4465 7363 d701 0000 72b6 0000 007a 0f53  Desc....r....z.S
+000030e0: 7562 7363 7269 6265 722e 4465 7363 6301  ubscriber.Descc.
+000030f0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00003100: 0000 0043 0000 0072 7100 0000 7219 0000  ...C...rq...r...
+00003110: 0029 01da 044e 616d 6572 2c00 0000 7217  .)...Namer,...r.
+00003120: 0000 0072 1700 0000 7218 0000 0072 ba00  ...r....r....r..
+00003130: 0000 dd01 0000 7302 0000 0006 017a 0f53  ......s......z.S
+00003140: 7562 7363 7269 6265 722e 4e61 6d65 6303  ubscriber.Namec.
+00003150: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+00003160: 0000 0043 0000 0073 4a00 0000 7c00 6a00  ...C...sJ...|.j.
+00003170: a001 7c01 7c02 a102 0100 7c00 6a02 6401  ..|.|.....|.j.d.
+00003180: 7501 7212 7c00 a002 7c01 7c02 a102 0100  u.r.|...|.|.....
+00003190: 7403 8300 7d03 7c00 6a04 6402 6b02 7223  t...}.|.j.d.k.r#
+000031a0: 7c03 a005 7c00 6a06 7c02 a102 0100 6401  |...|.j.|.....d.
+000031b0: 5300 6401 5300 2903 7a6f 0a20 2020 2020  S.d.S.).zo.     
+000031c0: 2020 2069 6e74 656e 616c 2075 7365 0a20     intenal use. 
+000031d0: 2020 2020 2020 203a 7061 7261 6d20 6e61         :param na
+000031e0: 6d65 3a20 7375 6273 6372 6970 7469 6f6e  me: subscription
+000031f0: 206e 616d 650a 2020 2020 2020 2020 3a70   name.        :p
+00003200: 6172 616d 2064 6174 613a 2044 6174 610a  aram data: Data.
+00003210: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00003220: 0a20 2020 2020 2020 204e 5429 07da 0d73  .        NT)...s
+00003230: 6967 5570 6461 7465 4461 7461 7229 0000  igUpdateDatar)..
+00003240: 0072 a800 0000 da02 5253 72a7 0000 00da  .r......RSr.....
+00003250: 1053 6176 6552 6573 6964 656e 7444 6174  .SaveResidentDat
+00003260: 6172 0e00 0000 2904 7212 0000 0072 0e00  ar....).r....r..
+00003270: 0000 721c 0000 00da 0272 7372 1700 0000  ..r......rsr....
+00003280: 7217 0000 0072 1800 0000 72ab 0000 00df  r....r....r.....
+00003290: 0100 0073 0e00 0000 0e08 0a01 0c01 0602  ...s............
+000032a0: 0a01 1201 04ff 7a12 5375 6273 6372 6962  ......z.Subscrib
+000032b0: 6572 2e6e 6577 4461 7461 6303 0000 0000  er.newDatac.....
+000032c0: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+000032d0: 0000 0073 3e00 0000 7c01 7c00 6a00 6b02  ...s>...|.|.j.k.
+000032e0: 721b 7c00 6a01 a002 7c00 6a00 7c02 a102  r.|.j...|.j.|...
+000032f0: 0100 7c00 6a03 6401 7501 721d 7c00 a003  ..|.j.d.u.r.|...
+00003300: 7c00 6a00 7c02 a102 0100 6401 5300 6401  |.j.|.....d.S.d.
+00003310: 5300 6401 5300 2902 7a6b 0a20 2020 2020  S.d.S.).zk.     
+00003320: 2020 2069 6e74 6572 6e61 6c20 7573 650a     internal use.
+00003330: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
+00003340: 6573 633a 206e 6577 2064 6573 6372 6970  esc: new descrip
+00003350: 7469 6f6e 2063 6f6d 696e 6720 6672 6f6d  tion coming from
+00003360: 206d 756c 7469 7665 7273 650a 2020 2020   multiverse.    
+00003370: 2020 2020 3a72 6574 7572 6e3a 0a20 2020      :return:.   
+00003380: 2020 2020 204e 2904 720e 0000 00da 0d73       N).r......s
+00003390: 6967 5570 6461 7465 4465 7363 7229 0000  igUpdateDescr)..
+000033a0: 0072 a900 0000 2903 7212 0000 0072 0e00  .r....).r....r..
+000033b0: 0000 7224 0000 0072 1700 0000 7217 0000  ..r$...r....r...
+000033c0: 0072 1800 0000 72aa 0000 00ef 0100 0073  .r....r........s
+000033d0: 0c00 0000 0a07 1001 0a01 1201 04fd 0402  ................
+000033e0: 7a12 5375 6273 6372 6962 6572 2e6e 6577  z.Subscriber.new
+000033f0: 4465 7363 7201 0000 0063 0300 0000 0000  Descr....c......
+00003400: 0000 0000 0000 0600 0000 0500 0000 4300  ..............C.
+00003410: 0000 73fa 0000 0074 007c 0183 0172 7774  ..s....t.|...rwt
+00003420: 017c 0164 0119 0074 0283 0272 1764 027c  .|.d...t...r.d.|
+00003430: 006a 0317 0064 0317 0074 047c 0283 0117  .j...d...t.|....
+00003440: 007d 036e 3174 017c 0164 0119 0074 0583  .}.n1t.|.d...t..
+00003450: 0272 2a64 047c 006a 0317 0064 0317 0074  .r*d.|.j...d...t
+00003460: 047c 0283 0117 007d 036e 1e74 017c 0164  .|.....}.n.t.|.d
+00003470: 0119 0074 0683 0272 3d64 057c 006a 0317  ...t...r=d.|.j..
+00003480: 0064 0317 0074 047c 0283 0117 007d 036e  .d...t.|.....}.n
+00003490: 0b64 067c 006a 0317 0064 0317 0074 047c  .d.|.j...d...t.|
+000034a0: 0283 0117 007d 037c 0144 005d 0a7d 047c  .....}.|.D.].}.|
+000034b0: 0364 0374 047c 0483 0117 0037 007d 0371  .d.t.|.....7.}.q
+000034c0: 4a7c 0364 0737 007d 037c 006a 07a0 087c  J|.d.7.}.|.j...|
+000034d0: 03a1 0101 007c 006a 09a0 0aa1 007d 057c  .....|.j.....}.|
+000034e0: 0564 0875 0072 797c 006a 0ba0 0ca1 0064  .d.u.ry|.j.....d
+000034f0: 0975 0072 7b7c 006a 09a0 0d7c 01a1 0101  .u.r{|.j...|....
+00003500: 0064 0a53 0064 0a53 0064 0a53 0064 0a53  .d.S.d.S.d.S.d.S
+00003510: 0029 0b7a c90a 2020 2020 2020 2020 5573  .).z..        Us
+00003520: 6572 2063 616e 2075 7064 6174 6520 6d75  er can update mu
+00003530: 6c74 6976 6572 7365 2077 6974 6820 6461  ltiverse with da
+00003540: 7461 0a20 2020 2020 2020 203a 7061 7261  ta.        :para
+00003550: 6d20 7768 6174 3a20 4461 7461 2074 6f20  m what: Data to 
+00003560: 7365 6e64 2074 6f20 4d75 6c69 7665 7273  send to Mulivers
+00003570: 650a 2020 2020 2020 2020 3a70 6172 616d  e.        :param
+00003580: 2069 6e64 6578 3a20 205a 6572 6f20 6465   index:  Zero de
+00003590: 6661 756c 742c 2062 7574 2069 7420 6361  fault, but it ca
+000035a0: 6e20 6265 2073 656e 7420 696e 2074 6865  n be sent in the
+000035b0: 206d 6964 646c 6520 6f66 2061 6e20 6172   middle of an ar
+000035c0: 7261 7279 0a20 2020 2020 2020 203a 7265  rary.        :re
+000035d0: 7475 726e 3a0a 2020 2020 2020 2020 7201  turn:.        r.
+000035e0: 0000 0072 8300 0000 7284 0000 0072 8500  ...r....r....r..
+000035f0: 0000 7286 0000 0072 8700 0000 7282 0000  ..r....r....r...
+00003600: 0054 464e 290e 7279 0000 0072 8a00 0000  .TFN).ry...r....
+00003610: 724d 0000 0072 0e00 0000 7243 0000 0072  rM...r....rC...r
+00003620: 8b00 0000 7246 0000 0072 ac00 0000 7229  ....rF...r....r)
+00003630: 0000 0072 6c00 0000 7233 0000 0072 a500  ...rl...r3...r..
+00003640: 0000 7270 0000 0072 2000 0000 2906 7212  ..rp...r ...).r.
+00003650: 0000 0072 8d00 0000 728e 0000 0072 8c00  ...r....r....r..
+00003660: 0000 728f 0000 00da 066d 6173 7465 7272  ..r......masterr
+00003670: 1700 0000 7217 0000 0072 1800 0000 da0a  ....r....r......
+00003680: 5570 6461 7465 4461 7461 fb01 0000 7322  UpdateData....s"
+00003690: 0000 0008 070e 0218 010e 0218 010e 0218  ................
+000036a0: 0116 0308 0212 0108 010c 020a 0116 0110  ................
+000036b0: 0104 eb08 147a 1553 7562 7363 7269 6265  .....z.Subscribe
+000036c0: 722e 5570 6461 7465 4461 7461 728d 0000  r.UpdateDatar...
+000036d0: 0063 0200 0000 0000 0000 0000 0000 0400  .c..............
+000036e0: 0000 0400 0000 4300 0000 734a 0000 0064  ......C...sJ...d
+000036f0: 017c 005f 0074 0183 007d 027c 02a0 027c  .|._.t...}.|...|
+00003700: 006a 03a1 017d 037c 0364 0275 0072 1e7c  .j...}.|.d.u.r.|
+00003710: 02a0 047c 006a 037c 01a1 0201 007c 00a0  ...|.j.|.....|..
+00003720: 057c 01a1 0101 0064 0253 007c 00a0 057c  .|.....d.S.|...|
+00003730: 03a1 0101 0064 0253 0029 037a e50a 2020  .....d.S.).z..  
+00003740: 2020 2020 2020 5570 6461 7465 7320 7468        Updates th
+00003750: 6520 6465 6661 756c 7473 2069 6620 6e6f  e defaults if no
+00003760: 7420 616c 7265 6164 7920 7365 742c 2061  t already set, a
+00003770: 6e64 2062 726f 6164 6361 7374 2074 6865  nd broadcast the
+00003780: 2064 6566 6175 6c74 7320 6f72 2074 6865   defaults or the
+00003790: 2073 6176 6520 7661 6c75 6573 2074 6f20   save values to 
+000037a0: 7468 6520 776f 726c 640a 2020 2020 2020  the world.      
+000037b0: 2020 6966 2074 6865 2064 6566 6175 6c74    if the default
+000037c0: 2061 7265 2061 6c72 6561 6479 2065 7869   are already exi
+000037d0: 7369 7469 6e67 2c20 6974 2075 7365 7320  siting, it uses 
+000037e0: 7468 656d 2c20 656c 7365 2069 6620 6372  them, else if cr
+000037f0: 6561 7465 206e 6577 2064 6566 6175 6c74  eate new default
+00003800: 7320 616e 6420 6265 6769 6e73 2074 6f20  s and begins to 
+00003810: 7573 6520 7468 656d 2e0a 2020 2020 2020  use them..      
+00003820: 2020 544e 2906 72a7 0000 0072 bc00 0000    TN).r....r....
+00003830: da0f 4765 7452 6573 6964 656e 7444 6174  ..GetResidentDat
+00003840: 6172 0e00 0000 72bd 0000 0072 c100 0000  ar....r....r....
+00003850: 2904 7212 0000 0072 8d00 0000 72be 0000  ).r....r....r...
+00003860: 0072 1c00 0000 7217 0000 0072 1700 0000  .r....r....r....
+00003870: 7218 0000 00da 1a55 7064 6174 6552 6573  r......UpdateRes
+00003880: 6964 656e 7444 6174 6144 6566 616c 7574  identDataDefalut
+00003890: 7319 0200 0073 0e00 0000 0605 0601 0c01  s....s..........
+000038a0: 0801 0e01 0e01 0e02 7a25 5375 6273 6372  ........z%Subscr
+000038b0: 6962 6572 2e55 7064 6174 6552 6573 6964  iber.UpdateResid
+000038c0: 656e 7444 6174 6144 6566 616c 7574 7363  entDataDefalutsc
+000038d0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000038e0: 0200 0000 4300 0000 730a 0000 0064 017c  ....C...s....d.|
+000038f0: 005f 0064 0053 0029 024e 4629 0172 a700  ._.d.S.).NF).r..
+00003900: 0000 722c 0000 0072 1700 0000 7217 0000  ..r,...r....r...
+00003910: 0072 1800 0000 da15 5374 6f70 5265 7369  .r......StopResi
+00003920: 6465 6e74 5265 636f 7264 696e 6727 0200  dentRecording'..
+00003930: 0073 0200 0000 0a01 7a20 5375 6273 6372  .s......z Subscr
+00003940: 6962 6572 2e53 746f 7052 6573 6964 656e  iber.StopResiden
+00003950: 7452 6563 6f72 6469 6e67 6302 0000 0000  tRecordingc.....
+00003960: 0000 0000 0000 0004 0000 0003 0000 0043  ...............C
+00003970: 0000 0073 5e00 0000 6401 7c00 6a00 1700  ...s^...d.|.j...
+00003980: 6402 1700 7c01 1700 7d02 7c02 6403 3700  d...|...}.|.d.7.
+00003990: 7d02 7c00 6a01 a002 7c02 a101 0100 7c00  }.|.j...|.....|.
+000039a0: 6a03 a004 a100 7d03 7c03 6404 7500 722b  j.....}.|.d.u.r+
+000039b0: 7c00 6a05 a006 a100 6405 7500 722d 7c00  |.j.....d.u.r-|.
+000039c0: 6a03 a007 7c01 a101 0100 6406 5300 6406  j...|.....d.S.d.
+000039d0: 5300 6406 5300 2907 7a88 0a20 2020 2020  S.d.S.).z..     
+000039e0: 2020 2069 6620 7765 2061 7265 2074 6865     if we are the
+000039f0: 2067 6f6c 6465 6e20 636f 7079 2c20 7765   golden copy, we
+00003a00: 2063 616e 2073 656e 6420 6120 4d61 6c63   can send a Malc
+00003a10: 6f6c 6d20 7072 6f6f 6620 6465 7363 7269  olm proof descri
+00003a20: 7074 6f72 0a20 2020 2020 2020 203a 7061  ptor.        :pa
+00003a30: 7261 6d20 7768 6174 3a20 7468 6520 6465  ram what: the de
+00003a40: 7363 7269 7074 6f72 0a20 2020 2020 2020  scriptor.       
+00003a50: 203a 7265 7475 726e 3a0a 2020 2020 2020   :return:.      
+00003a60: 2020 7288 0000 0072 8400 0000 7282 0000    r....r....r...
+00003a70: 0054 464e 2908 720e 0000 0072 ac00 0000  .TFN).r....r....
+00003a80: 7229 0000 0072 6c00 0000 7233 0000 0072  r)...rl...r3...r
+00003a90: a500 0000 7270 0000 0072 2a00 0000 2904  ....rp...r*...).
+00003aa0: 7212 0000 0072 8d00 0000 728c 0000 0072  r....r....r....r
+00003ab0: c000 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
+00003ac0: 0000 00da 0a55 7064 6174 6544 6573 6329  .....UpdateDesc)
+00003ad0: 0200 0073 0e00 0000 1206 0801 0c01 0a01  ...s............
+00003ae0: 1601 1001 08ff 7a15 5375 6273 6372 6962  ......z.Subscrib
+00003af0: 6572 2e55 7064 6174 6544 6573 6363 0100  er.UpdateDescc..
+00003b00: 0000 0000 0000 0000 0000 0300 0000 0500  ................
+00003b10: 0000 4300 0000 7348 0000 007c 00a0 00a1  ..C...sH...|....
+00003b20: 007d 017c 0164 0175 0172 117c 00a0 017c  .}.|.d.u.r.|...|
+00003b30: 006a 027c 00a0 00a1 00a1 0201 007c 00a0  .j.|.........|..
+00003b40: 03a1 007d 027c 0264 0175 0172 227c 00a0  ...}.|.d.u.r"|..
+00003b50: 047c 006a 027c 02a1 0201 0064 0153 0064  .|.j.|.....d.S.d
+00003b60: 0153 0029 027a 2f0a 2020 2020 2020 2020  .S.).z/.        
+00003b70: 696e 7465 7261 6e6c 2075 7365 0a20 2020  interanl use.   
+00003b80: 2020 2020 203a 7265 7475 726e 3a0a 2020       :return:.  
+00003b90: 2020 2020 2020 4e29 0572 b800 0000 72ab        N).r....r.
+00003ba0: 0000 0072 0e00 0000 72b9 0000 0072 aa00  ...r....r....r..
+00003bb0: 0000 2903 7212 0000 0072 1c00 0000 7224  ..).r....r....r$
+00003bc0: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00003bd0: 0000 72ae 0000 0036 0200 0073 0e00 0000  ..r....6...s....
+00003be0: 0806 0801 1201 0802 0801 1201 04ff 7a1a  ..............z.
+00003bf0: 5375 6273 6372 6962 6572 2e53 7461 7274  Subscriber.Start
+00003c00: 5369 6e67 6c65 5368 6f74 2903 4e4e 4e29  SingleShot).NNN)
+00003c10: 0172 0100 0000 2922 723f 0000 0072 4000  .r....)"r?...r@.
+00003c20: 0000 7241 0000 0072 4200 0000 7207 0000  ..rA...rB...r...
+00003c30: 0072 4300 0000 7244 0000 0072 bb00 0000  .rC...rD...r....
+00003c40: 72bf 0000 0072 ac00 0000 720e 0000 0072  r....r....r....r
+00003c50: 6c00 0000 72a5 0000 0072 b300 0000 72a8  l...r....r....r.
+00003c60: 0000 0072 a900 0000 72a7 0000 0072 4800  ...r....r....rH.
+00003c70: 0000 7210 0000 0072 b100 0000 72b4 0000  ..r....r....r...
+00003c80: 0072 b500 0000 72b8 0000 0072 b900 0000  .r....r....r....
+00003c90: 72ba 0000 0072 0600 0000 72ab 0000 0072  r....r....r....r
+00003ca0: aa00 0000 72c1 0000 0072 c300 0000 72c4  ....r....r....r.
+00003cb0: 0000 0072 c500 0000 72ae 0000 0072 4700  ...r....r....rG.
+00003cc0: 0000 7217 0000 0072 1700 0000 7215 0000  ..r....r....r...
+00003cd0: 0072 1800 0000 72a4 0000 0083 0100 0073  .r....r........s
+00003ce0: 3a00 0000 0800 0401 0a04 0a01 0801 0402  :...............
+00003cf0: 0401 0401 0401 0402 0401 0401 1802 0c22  ..............."
+00003d00: 080d 0806 0807 0806 0806 0802 0a01 080f  ................
+00003d10: 0a01 0a0b 0e1e 080e 0802 040d 1201 72a4  ..............r.
+00003d20: 0000 00da 085f 5f6d 6169 6e5f 5fda 0873  .....__main__..s
+00003d30: 7464 636f 6d51 747a 092d 2d76 6572 7369  tdcomQtz.--versi
+00003d40: 6f6e da06 6865 6c6c 6f31 54da 0754 6573  on..hello1T..Tes
+00003d50: 7469 6e67 2903 7201 0000 0072 a600 0000  ting).r....r....
+00003d60: e914 0000 00da 0668 656c 6c6f 3229 03e9  .......hello2)..
+00003d70: 6400 0000 e9c8 0000 0069 2c01 0000 da0c  d........i,.....
+00003d80: 7265 7369 6465 6e74 5465 7874 7a14 5465  residentTextz.Te
+00003d90: 7374 696e 6720 7265 7369 6465 6e74 5465  sting residentTe
+00003da0: 7874 2903 69e8 0300 0069 d007 0000 69b8  xt).i....i....i.
+00003db0: 0b00 0029 25da 0c50 7951 7435 2e51 7443  ...)%..PyQt5.QtC
+00003dc0: 6f72 6572 0200 0000 7203 0000 0072 0400  orer....r....r..
+00003dd0: 0000 7205 0000 0072 0600 0000 7207 0000  ..r....r....r...
+00003de0: 0072 0800 0000 7209 0000 00da 0f50 7951  .r....r......PyQ
+00003df0: 7435 2e51 744e 6574 776f 726b 720a 0000  t5.QtNetworkr...
+00003e00: 0072 0b00 0000 7299 0000 00da 0f73 7464  .r....r......std
+00003e10: 636f 6d76 7365 7474 696e 6773 720c 0000  comvsettingsr...
+00003e20: 0072 bc00 0000 da18 7374 6463 6f6d 5174  .r......stdcomQt
+00003e30: 2e73 7464 636f 6d76 7365 7474 696e 6773  .stdcomvsettings
+00003e40: da0f 7374 6463 6f6d 5174 5665 7273 696f  ..stdcomQtVersio
+00003e50: 6e72 0d00 0000 7248 0000 0072 a400 0000  nr....rH...r....
+00003e60: 723f 0000 0072 9e00 0000 da03 7379 73da  r?...r......sys.
+00003e70: 0461 7267 76da 0465 7869 74da 0361 7070  .argv..exit..app
+00003e80: da01 77da 0168 726d 0000 0072 c500 0000  ..w..hrm...r....
+00003e90: 72c1 0000 00da 0268 68da 0368 6868 72c3  r......hh..hhhr.
+00003ea0: 0000 00da 0565 7865 635f 7260 0000 0072  .....exec_r`...r
+00003eb0: 1700 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
+00003ec0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00003ed0: 0073 4e00 0000 2800 1001 0801 0202 1001  .sN...(.........
+00003ee0: 0601 0e01 0402 1001 1069 007f 007f 1011  .........i......
+00003ef0: 007f 0842 0802 0801 0a02 0801 0801 0a02  ...B............
+00003f00: 0601 0a02 0c01 0a02 0e01 0a02 0c01 0a01  ................
+00003f10: 0e01 0a02 0c01 0a01 0201 0e01 0802 0801  ................
+00003f20: 0e01 04e1                                ....
```

### Comparing `stdcomQt-1.1.4/src/stdcomQt/__pycache__/stdcomQtPjanice.cpython-310.pyc` & `stdcomQt-1.2.1/src/stdcomQt/__pycache__/stdcomQtPjanice.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/src/stdcomQt/__pycache__/stdcomQtargs.cpython-310.pyc` & `stdcomQt-1.2.1/src/stdcomQt/__pycache__/stdcomQtargs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/src/stdcomQt/__pycache__/stdcomipconfigdialog.cpython-310.pyc` & `stdcomQt-1.2.1/src/stdcomQt/__pycache__/stdcomipconfigdialog.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/src/stdcomQt/__pycache__/stdcomutilitywidgets.cpython-310.pyc` & `stdcomQt-1.2.1/src/stdcomQt/__pycache__/stdcomutilitywidgets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/src/stdcomQt/__pycache__/stdcomvsettings.cpython-310.pyc` & `stdcomQt-1.2.1/src/stdcomQt/__pycache__/stdcomvsettings.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jan  9 22:07:07 2023 UTC, .py size: 1042 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0b90 bc63 1204 0000  o..........c....
+00000000: 6f0d 0d0a 0000 0000 a285 c963 0504 0000  o..........c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 6d01 5a01 0100 0900 4700 6402  d.l.m.Z.....G.d.
 00000040: 6403 8400 6403 6501 8303 5a02 4700 6404  d...d.e...Z.G.d.
 00000050: 6405 8400 6405 6501 8303 5a03 6406 5300  d...d.e...Z.d.S.
 00000060: 2907 e900 0000 0029 01da 0951 5365 7474  )......)...QSett
 00000070: 696e 6773 6300 0000 0000 0000 0000 0000  ingsc...........
@@ -55,41 +55,40 @@
 00000360: 0200 0000 0400 0000 0300 0000 7206 0000  ............r...
 00000370: 0072 0700 0000 7208 0000 0072 0c00 0000  .r....r....r....
 00000380: 720e 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
 00000390: 0a00 0000 1300 0000 7212 0000 007a 1a52  ........r....z.R
 000003a0: 6574 656e 7369 6f6e 5365 7474 696e 6773  etensionSettings
 000003b0: 2e5f 5f69 6e69 745f 5fda 046e 616d 6563  .__init__..namec
 000003c0: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-000003d0: 0400 0000 4300 0000 7312 0000 007c 00a0  ....C...s....|..
-000003e0: 007c 006a 017c 02a1 027d 0264 0053 00a9  .|.j.|...}.d.S..
-000003f0: 014e 2902 da08 7365 7456 616c 7565 721b  .N)...setValuer.
-00000400: 0000 00a9 0372 0d00 0000 721b 0000 00da  .....r....r.....
-00000410: 0464 6174 6172 1000 0000 7210 0000 0072  .datar....r....r
-00000420: 1100 0000 da10 5361 7665 5265 7369 6465  ......SaveReside
-00000430: 6e74 4461 7461 1900 0000 7302 0000 0012  ntData....s.....
-00000440: 027a 2252 6574 656e 7369 6f6e 5365 7474  .z"RetensionSett
-00000450: 696e 6773 2e53 6176 6552 6573 6964 656e  ings.SaveResiden
-00000460: 7444 6174 614e 721f 0000 0063 0300 0000  tDataNr....c....
-00000470: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00000480: 4300 0000 7334 0000 007c 0264 0075 0072  C...s4...|.d.u.r
-00000490: 0667 007d 027c 00a0 007c 017c 02a1 027d  .g.}.|...|.|...}
-000004a0: 027c 0264 0075 0073 1674 017c 0283 0164  .|.d.u.s.t.|...d
-000004b0: 016b 0272 1864 0053 007c 0253 0029 024e  .k.r.d.S.|.S.).N
-000004c0: 7201 0000 0029 02da 0576 616c 7565 da03  r....)...value..
-000004d0: 6c65 6e72 1e00 0000 7210 0000 0072 1000  lenr....r....r..
-000004e0: 0000 7211 0000 00da 0f47 6574 5265 7369  ..r......GetResi
-000004f0: 6465 6e74 4461 7461 1d00 0000 730c 0000  dentData....s...
-00000500: 0008 0104 010c 0214 0104 0104 017a 2152  .............z!R
-00000510: 6574 656e 7369 6f6e 5365 7474 696e 6773  etensionSettings
-00000520: 2e47 6574 5265 7369 6465 6e74 4461 7461  .GetResidentData
-00000530: 2901 721a 0000 0072 1c00 0000 2908 7213  ).r....r....).r.
-00000540: 0000 0072 1400 0000 7215 0000 0072 1700  ...r....r....r..
-00000550: 0000 720a 0000 0072 2000 0000 7223 0000  ..r....r ...r#..
-00000560: 0072 1800 0000 7210 0000 0072 1000 0000  .r....r....r....
-00000570: 720e 0000 0072 1100 0000 7219 0000 0011  r....r....r.....
-00000580: 0000 0073 0800 0000 0800 1402 0e06 1c04  ...s............
-00000590: 7219 0000 004e 2904 da0c 5079 5174 352e  r....N)...PyQt5.
-000005a0: 5174 436f 7265 7202 0000 0072 0300 0000  QtCorer....r....
-000005b0: 7219 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
-000005c0: 1000 0000 7211 0000 00da 083c 6d6f 6475  ....r......<modu
-000005d0: 6c65 3e01 0000 0073 0800 0000 0c00 0202  le>....s........
-000005e0: 1003 140b                                ....
+000003d0: 0400 0000 4300 0000 7310 0000 007c 00a0  ....C...s....|..
+000003e0: 007c 017c 02a1 0201 0064 0053 00a9 014e  .|.|.....d.S...N
+000003f0: 2901 da08 7365 7456 616c 7565 a903 720d  )...setValue..r.
+00000400: 0000 0072 1b00 0000 da04 6461 7461 7210  ...r......datar.
+00000410: 0000 0072 1000 0000 7211 0000 00da 1053  ...r....r......S
+00000420: 6176 6552 6573 6964 656e 7444 6174 6119  aveResidentData.
+00000430: 0000 0073 0200 0000 1001 7a22 5265 7465  ...s......z"Rete
+00000440: 6e73 696f 6e53 6574 7469 6e67 732e 5361  nsionSettings.Sa
+00000450: 7665 5265 7369 6465 6e74 4461 7461 4e72  veResidentDataNr
+00000460: 1f00 0000 6303 0000 0000 0000 0000 0000  ....c...........
+00000470: 0003 0000 0004 0000 0043 0000 0073 3400  .........C...s4.
+00000480: 0000 7c02 6400 7500 7206 6700 7d02 7c00  ..|.d.u.r.g.}.|.
+00000490: a000 7c01 7c02 a102 7d02 7c02 6400 7500  ..|.|...}.|.d.u.
+000004a0: 7316 7401 7c02 8301 6401 6b02 7218 6400  s.t.|...d.k.r.d.
+000004b0: 5300 7c02 5300 2902 4e72 0100 0000 2902  S.|.S.).Nr....).
+000004c0: da05 7661 6c75 65da 036c 656e 721e 0000  ..value..lenr...
+000004d0: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
+000004e0: da0f 4765 7452 6573 6964 656e 7444 6174  ..GetResidentDat
+000004f0: 611c 0000 0073 0c00 0000 0801 0401 0c02  a....s..........
+00000500: 1401 0401 0401 7a21 5265 7465 6e73 696f  ......z!Retensio
+00000510: 6e53 6574 7469 6e67 732e 4765 7452 6573  nSettings.GetRes
+00000520: 6964 656e 7444 6174 6129 0172 1a00 0000  identData).r....
+00000530: 721c 0000 0029 0872 1300 0000 7214 0000  r....).r....r...
+00000540: 0072 1500 0000 7217 0000 0072 0a00 0000  .r....r....r....
+00000550: 7220 0000 0072 2300 0000 7218 0000 0072  r ...r#...r....r
+00000560: 1000 0000 7210 0000 0072 0e00 0000 7211  ....r....r....r.
+00000570: 0000 0072 1900 0000 1100 0000 7308 0000  ...r........s...
+00000580: 0008 0014 020e 061c 0372 1900 0000 4e29  .........r....N)
+00000590: 04da 0c50 7951 7435 2e51 7443 6f72 6572  ...PyQt5.QtCorer
+000005a0: 0200 0000 7203 0000 0072 1900 0000 7210  ....r....r....r.
+000005b0: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
+000005c0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000005d0: 7308 0000 000c 0002 0210 0314 0b         s............
```

### Comparing `stdcomQt-1.1.4/src/stdcomQt/__pycache__/stedcompostgresconfig.cpython-310.pyc` & `stdcomQt-1.2.1/src/stdcomQt/__pycache__/stedcompostgresconfig.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/src/stdcomQt/examples/multipleSubs.py` & `stdcomQt-1.2.1/src/stdcomQt/examples/multipleSubs.py`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/src/stdcomQt/examples/pjaniceExample.py` & `stdcomQt-1.2.1/src/stdcomQt/examples/pjaniceExample.py`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/src/stdcomQt/pjanicesimple.py` & `stdcomQt-1.2.1/src/stdcomQt/pjanicesimple.py`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/src/stdcomQt/pjanicesimple.ui` & `stdcomQt-1.2.1/src/stdcomQt/pjanicesimple.ui`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/src/stdcomQt/stdcomQt.py` & `stdcomQt-1.2.1/src/stdcomQt/stdcomQt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from PyQt5.QtCore import QMutex, QVariant, QTimer, QEvent, pyqtSlot, pyqtSignal, QObject, QCoreApplication
 from PyQt5.QtNetwork import QTcpSocket, QAbstractSocket
 import csv
 
+try:
+    from stdcomvsettings import RetensionSettings as RS
+except:
+    from stdcomQt.stdcomvsettings import RetensionSettings as RS
 
-stdcomQtVersion = "1.1.4"
+stdcomQtVersion = "1.2.1"
 class SubObject(QObject):
     """
     Internal use, not for users
     """
     sigNewData = pyqtSignal(str, list)
     sigNewDesc = pyqtSignal(str, str)
 
@@ -392,14 +396,15 @@
     name = str
     proxy = None
     cloud = None
     userData = None
 
     functionData = None
     functionDesc = None
+    residentSubscriber = False
 
     def __init__(self, name: str, cloud: stecQSocket, DataCallBack=None, DescCallBack=None, Parent=None):
         """
         Sunscription
         :param name: Subscription name
         :param cloud: Name of the stecQSocket cloud
         :param DataCallBack: Function a user can recieve data if desired, and if the user does not want to use signals
@@ -407,14 +412,15 @@
         :param Parent: QObject parent or None
         """
         if Parent is not None:
             super().__init__(Parent)
         else:
             super().__init__()
 
+        self.residentSubscriber = False
         self.cloud = cloud
         self.proxy = self.cloud.InsertProxy(name)
         self.name = self.proxy.GetName()
         self.functionData = DataCallBack
         self.functionDesc = DescCallBack
         self.proxy.sigNewDesc.connect(self.newDesc)
         self.proxy.sigNewData.connect(self.newData)
@@ -478,14 +484,18 @@
         :param data: Data
         :return:
         """
         self.sigUpdateData.emit(name, data)
         if self.functionData is not None:
             self.functionData(name, data)
 
+        rs = RS()
+        if self.residentSubscriber == True :
+            rs.SaveResidentData(self.name, data)
+
     @pyqtSlot(str, str)
     def newDesc(self, name, desc):
         """
         internal use
         :param desc: new description coming from multiverse
         :return:
         """
@@ -520,14 +530,30 @@
             command += "\n"
 
             self.sigUpdateMultiverse.emit(command)
             master = self.proxy.isOwner()
             if master is True and self.cloud.isConnected() is False:
                 self.proxy.AddData(what)
 
+    def UpdateResidentDataDefaluts(self, what : [] ):
+        """
+        Updates the defaults if not already set, and broadcast the defaults or the save values to the world
+        if the default are already exisiting, it uses them, else if create new defaults and begins to use them.
+        """
+        self.residentSubscriber = True
+        rs = RS()
+        data = rs.GetResidentData(self.name)
+        if data is  None :
+            rs.SaveResidentData(self.name, what)
+            self.UpdateData(what)
+        else:
+            self.UpdateData(data)
+
+    def StopResidentRecording(self):
+        self.residentSubscriber = False
     def UpdateDesc(self, what):
         """
         if we are the golden copy, we can send a Malcolm proof descriptor
         :param what: the descriptor
         :return:
         """
         command = "UPDATE-DESC," + self.name + "," + what
@@ -547,67 +573,39 @@
         if data is not None:
             self.newData(self.name, self.Data())
 
         desc = self.Desc()
         if desc is not None:
             self.newDesc(self.name, desc)
 
-
-
-
-
-
-
-
 if __name__ == '__main__':
 
-    from stdcomvsettings import RetensionSettings as RS
-
     print("stdcomQt")
     import sys
 
     if "--version" in sys.argv:
         print(stdcomQtVersion)
         sys.exit()
 
     app = QCoreApplication(sys.argv)
     w = stecQSocket()
 
-    h = Subscriber("hello2", w)
-    w.setOwner("hello2", True)
+    h = Subscriber("hello1", w)
+    w.setOwner("hello1", True)
 
     h.UpdateDesc("Testing")
     h.UpdateData([0, 10, 20])
 
     hh = Subscriber("hello2", w)
-    hh.UpdateData([222, 10, 20])
-
-    residentText = "hello.ressident"
-    residentTest =  Subscriber(residentText , w)
-
-    rsetting = RS()
-    data = rsetting.GetResidentData(residentText)
-
-    if data is None :
-
-        """ no resident data check for real data"""
-        data = residentTest.Data()
-
-        """ No Data has been output yet"""
-        if data is None:
-            data = ["Testing"]
-
-        """ updata to multiverse """
-        residentTest.UpdateData(data)
-
-        """ Save resident data """
-        rsetting.SaveResidentData(residentText, data)
-
-    else:
-        residentTest.UpdateData(data)
-
-
+    w.setOwner("hello2", True)
+    hh.UpdateDesc("Testing")
+    hh.UpdateData([100, 200, 300])
 
+    hhh = Subscriber("residentText", w)
+    w.setOwner("residentText", True)
+    hhh.UpdateDesc("Testing residentText")
+    """ this set the defaults to something, if not already set"""
+    hhh.UpdateResidentDataDefaluts([1000,2000,3000])
 
     app.exec_()
     w.quit()
     sys.exit(0)
```

### Comparing `stdcomQt-1.1.4/src/stdcomQt/stdcomQtPjanice.py` & `stdcomQt-1.2.1/src/stdcomQt/stdcomQtPjanice.py`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/src/stdcomQt/stdcomQtargs.py` & `stdcomQt-1.2.1/src/stdcomQt/stdcomQtargs.py`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/src/stdcomQt/stdcomipconfigdialog.py` & `stdcomQt-1.2.1/src/stdcomQt/stdcomipconfigdialog.py`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/src/stdcomQt/stdcomipconfigdialog.ui` & `stdcomQt-1.2.1/src/stdcomQt/stdcomipconfigdialog.ui`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/src/stdcomQt/stdcomutilitywidgets.py` & `stdcomQt-1.2.1/src/stdcomQt/stdcomutilitywidgets.py`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/src/stdcomQt/stdcomvsettings.py` & `stdcomQt-1.2.1/src/stdcomQt/stdcomvsettings.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,16 +19,15 @@
     def __init__(self, project: str = "stdcomQt.ResidentSubscriber"):
         """
         :param project:   default is "stec-opc" Should be the Project you or instance of the Project
         """
         super().__init__(project, QSettings.IniFormat)
 
     def SaveResidentData(self, name : str, data):
-
-        data = self.setValue(self.name, data)
+        self.setValue(name, data)
 
     def GetResidentData(self, name : str , data : [] = None ) :
         if data is None:
             data = []
 
         data = self.value(name, data)
         if data is None or len(data) == 0:
```

### Comparing `stdcomQt-1.1.4/src/stdcomQt/stedcompostgresconfig.py` & `stdcomQt-1.2.1/src/stdcomQt/stedcompostgresconfig.py`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/src/stdcomQt/stedcompostgresconfig.ui` & `stdcomQt-1.2.1/src/stdcomQt/stedcompostgresconfig.ui`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/src/stdcomQt/utilitys/pjaniceExt.py` & `stdcomQt-1.2.1/src/stdcomQt/utilitys/pjaniceExt.py`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/src/stdcomQt.egg-info/PKG-INFO` & `stdcomQt-1.2.1/src/stdcomQt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdcomQt
-Version: 1.1.4
+Version: 1.2.1
 Summary: Stec Railway Version StandAlone Subscribers
 Home-page: http://www.vremsoft.com
 Author: ed
 Author-email: srini_durand@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `stdcomQt-1.1.4/src/stdcomQt.egg-info/SOURCES.txt` & `stdcomQt-1.2.1/src/stdcomQt.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 src/stdcomQt/__init__.py
 src/stdcomQt/pjanicesimple.py
 src/stdcomQt/pjanicesimple.ui
-src/stdcomQt/stdcomQt.ResidentSubscriber
 src/stdcomQt/stdcomQt.py
 src/stdcomQt/stdcomQtC20.py
 src/stdcomQt/stdcomQtPjanice.py
 src/stdcomQt/stdcomQtargs.py
 src/stdcomQt/stdcomipconfigdialog.py
 src/stdcomQt/stdcomipconfigdialog.ui
 src/stdcomQt/stdcomutilitywidgets.py
@@ -28,18 +27,14 @@
 src/stdcomQt/__pycache__/stdcomQtC20.cpython-310.pyc
 src/stdcomQt/__pycache__/stdcomQtPjanice.cpython-310.pyc
 src/stdcomQt/__pycache__/stdcomQtargs.cpython-310.pyc
 src/stdcomQt/__pycache__/stdcomipconfigdialog.cpython-310.pyc
 src/stdcomQt/__pycache__/stdcomutilitywidgets.cpython-310.pyc
 src/stdcomQt/__pycache__/stdcomvsettings.cpython-310.pyc
 src/stdcomQt/__pycache__/stedcompostgresconfig.cpython-310.pyc
-src/stdcomQt/aicontrols/CSVReader.py
-src/stdcomQt/aicontrols/PID_train.png
-src/stdcomQt/aicontrols/PID_train_data.csv
-src/stdcomQt/aicontrols/toys.py
 src/stdcomQt/examples/Stec.PJanice
 src/stdcomQt/examples/multipleSubs.py
 src/stdcomQt/examples/pjaniceExample.py
 src/stdcomQt/utilitys/Stec.PJanice
 src/stdcomQt/utilitys/pjaniceExt.py
 text/build/html/.buildinfo
 text/build/html/code.html
```

### Comparing `stdcomQt-1.1.4/text/build/html/_modules/index.html` & `stdcomQt-1.2.1/text/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/_modules/stdcomQt.html` & `stdcomQt-1.2.1/text/build/html/_modules/stdcomQt.html`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/_modules/stdcomQtC20.html` & `stdcomQt-1.2.1/text/build/html/_modules/stdcomQtC20.html`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/_modules/stdcomQtPjanice.html` & `stdcomQt-1.2.1/text/build/html/_modules/stdcomQtPjanice.html`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/_modules/stdcomQtargs.html` & `stdcomQt-1.2.1/text/build/html/_modules/stdcomQtargs.html`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/_modules/stdcomutilitywidgets.html` & `stdcomQt-1.2.1/text/build/html/_modules/stdcomutilitywidgets.html`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/_modules/stdcomvsettings.html` & `stdcomQt-1.2.1/text/build/html/_modules/stdcomvsettings.html`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/_sources/index.rst.txt` & `stdcomQt-1.2.1/text/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/_static/alabaster.css` & `stdcomQt-1.2.1/text/build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/_static/basic.css` & `stdcomQt-1.2.1/text/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/_static/doctools.js` & `stdcomQt-1.2.1/text/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/_static/forkme_right_darkblue_121621.png` & `stdcomQt-1.2.1/text/build/html/_static/forkme_right_darkblue_121621.png`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/_static/jquery.js` & `stdcomQt-1.2.1/text/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/_static/language_data.js` & `stdcomQt-1.2.1/text/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/_static/pygments.css` & `stdcomQt-1.2.1/text/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/_static/searchtools.js` & `stdcomQt-1.2.1/text/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/_static/underscore.js` & `stdcomQt-1.2.1/text/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/code.html` & `stdcomQt-1.2.1/text/build/html/code.html`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/genindex.html` & `stdcomQt-1.2.1/text/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/index.html` & `stdcomQt-1.2.1/text/build/html/index.html`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/objects.inv` & `stdcomQt-1.2.1/text/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/py-modindex.html` & `stdcomQt-1.2.1/text/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/search.html` & `stdcomQt-1.2.1/text/build/html/search.html`

 * *Files identical despite different names*

### Comparing `stdcomQt-1.1.4/text/build/html/searchindex.js` & `stdcomQt-1.2.1/text/build/html/searchindex.js`

 * *Files identical despite different names*

