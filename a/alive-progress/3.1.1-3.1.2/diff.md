# Comparing `tmp/alive-progress-3.1.1.tar.gz` & `tmp/alive-progress-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alive-progress-3.1.1.tar", last modified: Sat Apr  8 04:48:13 2023, max compression
+gzip compressed data, was "dist/alive-progress-3.1.2.tar", last modified: Tue May  9 01:09:06 2023, max compression
```

## Comparing `alive-progress-3.1.1.tar` & `alive-progress-3.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-04-08 04:48:13.000000 alive-progress-3.1.1/
--rw-r--r--   0 rogerio    (501) staff       (20)     1084 2019-08-05 05:55:53.000000 alive-progress-3.1.1/LICENSE
--rw-r--r--   0 rogerio    (501) staff       (20)    76651 2023-04-08 04:48:13.000000 alive-progress-3.1.1/PKG-INFO
--rw-r--r--   0 rogerio    (501) staff       (20)    67805 2023-04-08 04:47:50.000000 alive-progress-3.1.1/README.md
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-04-08 04:48:13.000000 alive-progress-3.1.1/alive_progress/
--rw-r--r--   0 rogerio    (501) staff       (20)      417 2023-04-08 04:47:50.000000 alive-progress-3.1.1/alive_progress/__init__.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-04-08 04:48:13.000000 alive-progress-3.1.1/alive_progress/animations/
--rw-r--r--   0 rogerio    (501) staff       (20)      481 2021-08-26 23:38:44.000000 alive-progress-3.1.1/alive_progress/animations/__init__.py
--rw-r--r--   0 rogerio    (501) staff       (20)     9721 2023-03-24 02:50:30.000000 alive-progress-3.1.1/alive_progress/animations/bars.py
--rw-r--r--   0 rogerio    (501) staff       (20)    13834 2023-03-24 02:50:30.000000 alive-progress-3.1.1/alive_progress/animations/spinner_compiler.py
--rw-r--r--   0 rogerio    (501) staff       (20)    11443 2023-03-24 02:50:30.000000 alive-progress-3.1.1/alive_progress/animations/spinners.py
--rw-r--r--   0 rogerio    (501) staff       (20)     4723 2021-08-26 23:38:44.000000 alive-progress-3.1.1/alive_progress/animations/utils.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-04-08 04:48:13.000000 alive-progress-3.1.1/alive_progress/core/
--rw-r--r--   0 rogerio    (501) staff       (20)        0 2020-07-28 14:16:28.000000 alive-progress-3.1.1/alive_progress/core/__init__.py
--rw-r--r--   0 rogerio    (501) staff       (20)     1351 2022-02-02 06:03:46.000000 alive-progress-3.1.1/alive_progress/core/calibration.py
--rw-r--r--   0 rogerio    (501) staff       (20)     8876 2023-03-24 02:50:30.000000 alive-progress-3.1.1/alive_progress/core/configuration.py
--rw-r--r--   0 rogerio    (501) staff       (20)     5070 2023-04-08 04:47:50.000000 alive-progress-3.1.1/alive_progress/core/hook_manager.py
--rw-r--r--   0 rogerio    (501) staff       (20)    23494 2023-04-08 04:47:50.000000 alive-progress-3.1.1/alive_progress/core/progress.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-04-08 04:48:13.000000 alive-progress-3.1.1/alive_progress/styles/
--rw-r--r--   0 rogerio    (501) staff       (20)      614 2021-08-26 23:38:44.000000 alive-progress-3.1.1/alive_progress/styles/__init__.py
--rw-r--r--   0 rogerio    (501) staff       (20)    11233 2023-03-24 02:50:30.000000 alive-progress-3.1.1/alive_progress/styles/exhibit.py
--rw-r--r--   0 rogerio    (501) staff       (20)     8454 2023-03-24 02:50:30.000000 alive-progress-3.1.1/alive_progress/styles/internal.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-04-08 04:48:13.000000 alive-progress-3.1.1/alive_progress/tools/
--rw-r--r--   0 rogerio    (501) staff       (20)       58 2021-08-26 23:38:44.000000 alive-progress-3.1.1/alive_progress/tools/__init__.py
--rw-r--r--   0 rogerio    (501) staff       (20)     3002 2022-03-22 04:49:57.000000 alive-progress-3.1.1/alive_progress/tools/demo.py
--rw-r--r--   0 rogerio    (501) staff       (20)     1024 2021-08-26 23:38:44.000000 alive-progress-3.1.1/alive_progress/tools/repl.py
--rw-r--r--   0 rogerio    (501) staff       (20)     2717 2022-12-22 05:23:53.000000 alive-progress-3.1.1/alive_progress/tools/sampling.py
--rw-r--r--   0 rogerio    (501) staff       (20)     6634 2021-08-26 23:38:44.000000 alive-progress-3.1.1/alive_progress/tools/unicode_breaks.py
--rw-r--r--   0 rogerio    (501) staff       (20)      399 2021-08-26 23:38:44.000000 alive-progress-3.1.1/alive_progress/tools/utils.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-04-08 04:48:13.000000 alive-progress-3.1.1/alive_progress/utils/
--rw-r--r--   0 rogerio    (501) staff       (20)        0 2022-10-31 01:30:29.000000 alive-progress-3.1.1/alive_progress/utils/__init__.py
--rw-r--r--   0 rogerio    (501) staff       (20)     8811 2022-12-22 05:23:53.000000 alive-progress-3.1.1/alive_progress/utils/cells.py
--rw-r--r--   0 rogerio    (501) staff       (20)     2308 2022-02-11 05:29:12.000000 alive-progress-3.1.1/alive_progress/utils/colors.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-04-08 04:48:13.000000 alive-progress-3.1.1/alive_progress/utils/terminal/
--rw-r--r--   0 rogerio    (501) staff       (20)     2100 2023-03-24 02:50:30.000000 alive-progress-3.1.1/alive_progress/utils/terminal/__init__.py
--rw-r--r--   0 rogerio    (501) staff       (20)      747 2023-03-24 02:50:30.000000 alive-progress-3.1.1/alive_progress/utils/terminal/jupyter.py
--rw-r--r--   0 rogerio    (501) staff       (20)      418 2022-12-22 05:23:53.000000 alive-progress-3.1.1/alive_progress/utils/terminal/non_tty.py
--rw-r--r--   0 rogerio    (501) staff       (20)     1284 2023-03-24 02:50:30.000000 alive-progress-3.1.1/alive_progress/utils/terminal/tty.py
--rw-r--r--   0 rogerio    (501) staff       (20)      550 2023-03-24 02:50:30.000000 alive-progress-3.1.1/alive_progress/utils/terminal/void.py
--rw-r--r--   0 rogerio    (501) staff       (20)     1411 2022-12-22 05:23:53.000000 alive-progress-3.1.1/alive_progress/utils/timing.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-04-08 04:48:13.000000 alive-progress-3.1.1/alive_progress.egg-info/
--rw-r--r--   0 rogerio    (501) staff       (20)    76651 2023-04-08 04:48:13.000000 alive-progress-3.1.1/alive_progress.egg-info/PKG-INFO
--rw-r--r--   0 rogerio    (501) staff       (20)     1223 2023-04-08 04:48:13.000000 alive-progress-3.1.1/alive_progress.egg-info/SOURCES.txt
--rw-r--r--   0 rogerio    (501) staff       (20)        1 2023-04-08 04:48:13.000000 alive-progress-3.1.1/alive_progress.egg-info/dependency_links.txt
--rw-r--r--   0 rogerio    (501) staff       (20)       34 2023-04-08 04:48:13.000000 alive-progress-3.1.1/alive_progress.egg-info/requires.txt
--rw-r--r--   0 rogerio    (501) staff       (20)       15 2023-04-08 04:48:13.000000 alive-progress-3.1.1/alive_progress.egg-info/top_level.txt
--rw-r--r--   0 rogerio    (501) staff       (20)       38 2023-04-08 04:48:13.000000 alive-progress-3.1.1/setup.cfg
--rw-r--r--   0 rogerio    (501) staff       (20)     2306 2022-12-22 05:23:53.000000 alive-progress-3.1.1/setup.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-09 01:09:06.000000 alive-progress-3.1.2/
+-rw-r--r--   0 rogerio    (501) staff       (20)     1084 2019-08-05 05:55:53.000000 alive-progress-3.1.2/LICENSE
+-rw-r--r--   0 rogerio    (501) staff       (20)    75898 2023-05-09 01:09:06.000000 alive-progress-3.1.2/PKG-INFO
+-rw-r--r--   0 rogerio    (501) staff       (20)    67100 2023-04-19 02:55:54.000000 alive-progress-3.1.2/README.md
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress/
+-rw-r--r--   0 rogerio    (501) staff       (20)      417 2023-05-09 01:08:53.000000 alive-progress-3.1.2/alive_progress/__init__.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress/animations/
+-rw-r--r--   0 rogerio    (501) staff       (20)      481 2021-08-26 23:38:44.000000 alive-progress-3.1.2/alive_progress/animations/__init__.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     9721 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/animations/bars.py
+-rw-r--r--   0 rogerio    (501) staff       (20)    13834 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/animations/spinner_compiler.py
+-rw-r--r--   0 rogerio    (501) staff       (20)    11443 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/animations/spinners.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     4723 2021-08-26 23:38:44.000000 alive-progress-3.1.2/alive_progress/animations/utils.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress/core/
+-rw-r--r--   0 rogerio    (501) staff       (20)        0 2020-07-28 14:16:28.000000 alive-progress-3.1.2/alive_progress/core/__init__.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     1351 2022-02-02 06:03:46.000000 alive-progress-3.1.2/alive_progress/core/calibration.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     8876 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/core/configuration.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     5488 2023-05-09 01:08:53.000000 alive-progress-3.1.2/alive_progress/core/hook_manager.py
+-rw-r--r--   0 rogerio    (501) staff       (20)    23500 2023-04-24 17:28:20.000000 alive-progress-3.1.2/alive_progress/core/progress.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress/styles/
+-rw-r--r--   0 rogerio    (501) staff       (20)      614 2021-08-26 23:38:44.000000 alive-progress-3.1.2/alive_progress/styles/__init__.py
+-rw-r--r--   0 rogerio    (501) staff       (20)    11233 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/styles/exhibit.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     8454 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/styles/internal.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress/tools/
+-rw-r--r--   0 rogerio    (501) staff       (20)       58 2021-08-26 23:38:44.000000 alive-progress-3.1.2/alive_progress/tools/__init__.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     3002 2022-03-22 04:49:57.000000 alive-progress-3.1.2/alive_progress/tools/demo.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     1024 2021-08-26 23:38:44.000000 alive-progress-3.1.2/alive_progress/tools/repl.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     2717 2022-12-22 05:23:53.000000 alive-progress-3.1.2/alive_progress/tools/sampling.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     6634 2021-08-26 23:38:44.000000 alive-progress-3.1.2/alive_progress/tools/unicode_breaks.py
+-rw-r--r--   0 rogerio    (501) staff       (20)      399 2021-08-26 23:38:44.000000 alive-progress-3.1.2/alive_progress/tools/utils.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress/utils/
+-rw-r--r--   0 rogerio    (501) staff       (20)        0 2022-10-31 01:30:29.000000 alive-progress-3.1.2/alive_progress/utils/__init__.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     8811 2022-12-22 05:23:53.000000 alive-progress-3.1.2/alive_progress/utils/cells.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     2308 2022-02-11 05:29:12.000000 alive-progress-3.1.2/alive_progress/utils/colors.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress/utils/terminal/
+-rw-r--r--   0 rogerio    (501) staff       (20)     2100 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/utils/terminal/__init__.py
+-rw-r--r--   0 rogerio    (501) staff       (20)      747 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/utils/terminal/jupyter.py
+-rw-r--r--   0 rogerio    (501) staff       (20)      418 2022-12-22 05:23:53.000000 alive-progress-3.1.2/alive_progress/utils/terminal/non_tty.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     1284 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/utils/terminal/tty.py
+-rw-r--r--   0 rogerio    (501) staff       (20)      550 2023-03-24 02:50:30.000000 alive-progress-3.1.2/alive_progress/utils/terminal/void.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     1411 2022-12-22 05:23:53.000000 alive-progress-3.1.2/alive_progress/utils/timing.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress.egg-info/
+-rw-r--r--   0 rogerio    (501) staff       (20)    75898 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress.egg-info/PKG-INFO
+-rw-r--r--   0 rogerio    (501) staff       (20)     1223 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress.egg-info/SOURCES.txt
+-rw-r--r--   0 rogerio    (501) staff       (20)        1 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress.egg-info/dependency_links.txt
+-rw-r--r--   0 rogerio    (501) staff       (20)       34 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress.egg-info/requires.txt
+-rw-r--r--   0 rogerio    (501) staff       (20)       15 2023-05-09 01:09:06.000000 alive-progress-3.1.2/alive_progress.egg-info/top_level.txt
+-rw-r--r--   0 rogerio    (501) staff       (20)       38 2023-05-09 01:09:06.000000 alive-progress-3.1.2/setup.cfg
+-rw-r--r--   0 rogerio    (501) staff       (20)     2306 2022-12-22 05:23:53.000000 alive-progress-3.1.2/setup.py
```

### Comparing `alive-progress-3.1.1/LICENSE` & `alive-progress-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/PKG-INFO` & `alive-progress-3.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,52 +1,73 @@
 Metadata-Version: 2.1
 Name: alive-progress
-Version: 3.1.1
+Version: 3.1.2
 Summary: A new kind of Progress Bar, with real-time throughput, ETA, and very cool animations!
 Home-page: https://github.com/rsalmei/alive-progress
 Author: Rogério Sampaio de Almeida
 Author-email: rsalmei@gmail.com
 License: MIT
 Description: [<img align="right" src="https://cdn.buymeacoffee.com/buttons/default-orange.png" width="217px" height="51x">](https://www.buymeacoffee.com/rsalmei)
         [<img align="right" alt="Donate with PayPal button" src="https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif">](https://www.paypal.com/donate?business=6SWSHEB5ZNS5N&no_recurring=0&item_name=I%27m+the+author+of+alive-progress%2C+clearly+and+about-time.+Thank+you+for+appreciating+my+work%21&currency_code=USD)
         
         ![alive-progress logo](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/alive-logo.gif)
         
-        # alive-progress :)
-        ### A new kind of Progress Bar, with real-time throughput, ETA, and very cool animations!
+        # alive-progress
         
-        [![Maintenance](https://img.shields.io/badge/Maintained-yes-green.svg)](https://gitHub.com/rsalmei/alive-progress/graphs/commit-activity)
+        [![Maintenance](https://img.shields.io/badge/maintained-yes-brightgreen.svg)](https://gitHub.com/rsalmei/alive-progress/graphs/commit-activity)
         [![PyPI version](https://img.shields.io/pypi/v/alive-progress.svg)](https://pypi.python.org/pypi/alive-progress/)
         [![PyPI pyversions](https://img.shields.io/pypi/pyversions/alive-progress.svg)](https://pypi.python.org/pypi/alive-progress/)
-        [![PyPI status](https://img.shields.io/pypi/status/alive-progress.svg)](https://pypi.python.org/pypi/alive-progress/)
         [![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=week&units=international_system&left_color=grey&right_color=orange&left_text=downloads/week)](https://pepy.tech/project/alive-progress)
         [![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=month&units=international_system&left_color=grey&right_color=orange&left_text=/month)](https://pepy.tech/project/alive-progress)
         [![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=total&units=international_system&left_color=grey&right_color=orange&left_text=total)](https://pepy.tech/project/alive-progress)
+        ![GitHub Sponsors](https://img.shields.io/github/sponsors/rsalmei)
+        
+        
+        Have you ever wondered where your lengthy processing was at, and when would it finish? Do you usually hit `RETURN` several times to make sure it didn't crash, or the SSH connection didn't freeze? Have you ever thought it'd be awesome to be able to _pause some processing_ without hassle, return to the Python prompt to manually fix some items, then _seamlessly resume_ it? I did...
+        
+        I've started this new progress bar thinking about all that, behold the **alive-progress**! 😃
+        
+        ![alive-progress demo](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/alive-demo.gif)
+        
+        
+        Introducing the newest concept in progress bars for Python! `alive-progress` is in a class of its own, with an array of cool features that set it apart. Here are a few highlights:
+        - A mesmerizing **live spinner** that clearly shows your lengthy process did not crash and your SSH connection did not freeze, with **visual feedback** reacting to your processing speed.
+        - An efficient **multithreaded** bar that updates itself at a fraction of the actual processing speed to keep **CPU usage low** and avoid terminal spamming (1,000,000 iterations per second equates to roughly 60 updates per second, and you can also calibrate this to your liking).
+        - An **ETA** (expected time of arrival) feature with an intelligent _Exponential Smoothing Algorithm_ that shows the time to completion, allowing you to plan your time and manage your workload more effectively.
+        - Automatic **print** and **logging** hooks that provide seamless integration and effortless tracking, even enriching them with the current bar position when they occur.
+        - It prints a **nice receipt** when the processing finishes, including the elapsed time and the observed throughput.
+        - It detects **under** and **overflows**, enabling you to track hits, misses, or any desired count, not necessarily the actual iterations.
+        - You can **pause** it! That's right, you heard it here first! No other progress bar anywhere has this feature! You can get back to the Python prompt during any processing, adjust some items, and get back into that running process as if it had never stopped! All `alive_bar` widgets are kept as they were, and the elapsed time nicely ignores the paused time!
+        - It is **highly customizable**, with a smorgasbord of spinner and bar styles, as well as several ready-to-use factories to easily generate yours! You can even use the super powerful and cool `check()` tool to help you design your own animations! You can see all the generated frames and cycles exploded on screen, with several verbosity levels, even including an _alive_ rendition! It's boundless creativity at your fingertips!
+        
+        ---
+        ## Table of contents
+        
+        This README is always evolving, so do take a more comprehensive look from time to time... You might find great new details in other sections! 😊
         
         <!-- TOC -->
-        * [alive-progress :)](#alive-progress--)
-            * [A new kind of Progress Bar, with real-time throughput, ETA, and very cool animations!](#a-new-kind-of-progress-bar-with-real-time-throughput-eta-and-very-cool-animations-)
-          * [Introduction](#introduction)
-          * [📌 NEW in 3.1 series!](#-new-in-31-series-)
+        * [alive-progress](#alive-progress)
+          * [Table of contents](#table-of-contents)
+          * [📌 NEW in 3.1 series](#-new-in-31-series)
           * [Using `alive-progress`](#using-alive-progress)
             * [Get it](#get-it)
             * [Try it](#try-it)
             * [Awake it](#awake-it)
             * [Master it](#master-it)
           * [Displaying messages](#displaying-messages)
           * [Auto-iterating](#auto-iterating)
           * [Modes of operation](#modes-of-operation)
-            * [Definite/unknown: Counters](#definiteunknown--counters)
-            * [Manual: Percentages](#manual--percentages)
+            * [Definite/unknown: Counters](#definiteunknown-counters)
+            * [Manual: Percentages](#manual-percentages)
             * [Summary of Modes](#summary-of-modes)
             * [The `bar()` handlers](#the-bar-handlers)
           * [Styles](#styles)
           * [Configuration](#configuration)
           * [Create your own animations](#create-your-own-animations)
-            * [Intro: How do they work?](#intro--how-do-they-work)
+            * [Intro: How do they work?](#intro-how-do-they-work)
             * [A Spinner Compiler, really?](#a-spinner-compiler-really)
             * [Spinner Factories](#spinner-factories)
             * [Bar Factories](#bar-factories)
           * [Advanced](#advanced)
             * [The Pause Mechanism](#the-pause-mechanism)
             * [Loop-less use](#loop-less-use)
             * [FPS Calibration](#fps-calibration)
@@ -56,42 +77,15 @@
           * [Python End of Life notice](#python-end-of-life-notice)
             * [For new Python 2.7 and 3.5](#for-new-python-27-and-35)
             * [For new Python 3.6](#for-new-python-36)
           * [License](#license)
         <!-- TOC -->
         
         
-        This README is always evolving, so do take a more comprehensive look from time to time... You might find great new details in other sections! 😊
-        
-        
-        ## Introduction
-        
-        Have you ever wondered where your lengthy processing was, and when it would finish? Ever found yourself hitting [RETURN] now and then to ensure it didn't hang, or if, in a remote SSH session, the connection was still working? Ever needed to *pause* some processing for a while, return to the Python prompt for a manual inspection or fixing an item, and then *resume* the process seamlessly? I did...
-        
-        I've started this cool progress bar thinking about all that, the **alive-progress**! 😃
-        
-        ![alive-progress demo](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/alive-demo.gif)
-        
-        
-        I like to think of this as a new kind of progress bar for Python since it has, among other things:
-        
-        - a **live spinner** that is incredibly cool and clearly shows your lengthy process did not hang, or your ssh connection did not drop;
-        - a **visual feedback** which reacts to your processing, as the live spinner will go faster or slower with it;
-        - an **efficient** multithreaded bar, which updates itself at a fraction of the actual processing speed (1,000,000 iterations per second equates to roughly 60 updates per second) to keep **CPU usage low** and avoid terminal spamming (you can also calibrate this to your liking);
-        - nice monitoring of both _position and throughput_ of your processing;
-        - an **ETA** (expected time of arrival) with an intelligent _exponential smoothing algorithm_, that shows the time to completion;
-        - automatic **print** and **logging** hooks, which allow print statements and logging messages to work _effortlessly_, right amid an animated bar, and even enriching them with the current bar position when they occur;
-        - a **nice receipt** is printed when your processing finishes, including the last bar rendition, the elapsed time, and the observed throughput;
-        - it detects **under and overflows**, enabling you to track hits, misses, or any desired count, not necessarily the actual iterations;
-        - it automatically detects if there's an **allocated tty**, and if there isn't (like in a shell pipeline), only the final receipt is printed (so you can safely include it in any code, and rest assured your log file won't get thousands of progress lines);
-        - you can **pause** it! I think that's an unprecedented feature for progress bars ANYWHERE — in Python or any other language — no one has ever done it! It's incredible to be able to get back to the Python prompt during any running process! Then you can manually adjust an item or prepare something and get back into that running process as if it had never stopped!! All `alive_bar` widgets are kept as they were, and the elapsed time nicely ignores the paused time!;
-        - it is **customizable**, with a growing smorgasbord of spinner and bar styles, as well as several ready-to-use factories to easily generate yours! Now (📌 new in 2.0), we even have a super powerful and cool `check()` tool, in both spinners and bars, to help you design your own animations! You can see all the frames and cycles exploded on screen, with several verbosity levels, even including an **alive** rendition! It's awesome 😜
-        
-        
-        ## 📌 NEW in 3.1 series!
+        ## 📌 NEW in 3.1 series
         
         A very cool update here! In addition to polishing things up and improving terminal support, now `alive-progress` supports resuming computations!
         
         When processing huge datasets or things that take a long time, you might either use batches or cache partial results. Then, in case it stops and is restarted, you end up skipping all those already done items very quickly, which makes the `alive_bar` think you're processing thousands of items per second, which in turn completely ruins the ETA... But not anymore! Just tell `bar()` that you've skipped items... 👏
         
         You can use it in two ways:
         
@@ -123,15 +117,15 @@
         - new `max_cols` config setting, the number of columns to use if not possible to fetch it, like in jupyter and other platforms which doesn't support size
         - fix fetching the size of the terminal when using stderr
         - officially supports Python 3.11
         - included [ruff](https://github.com/charliermarsh/ruff) linter before building
         
         
         <details>
-        <summary>📌 NEW in 3.0 series!</summary>
+        <summary>📌 NEW in 3.0 series</summary>
         
         Yep, I could finally get this version out! These are the new goodies:
         
         - Units support! You can now label the data you're processing, like `B`, `bytes`, or even `°C`!
         - Automatic scaling! With support for SI (base 1000), IEC (base 1024), and even an alternate SI with base 1024, you'll be well served!
         - Configurable precision! When your numbers are scaled, you get to choose how many decimals they display!
         - Automatic stats scaling for slow throughputs! If your processing takes minutes or more, now you'll see rates per minute, per hour, and even per day! (It works within the auto-scaling system!)
@@ -147,15 +141,15 @@
         - Fix unknown mode always ending with a warning (!)
         
         And last but not least, a more polished layout for you to enjoy your progress!
         ![alive-progress 3.0](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/alive3.0.png)
         </details>
         
         <details>
-        <summary>📌 NEW in 2.4 series!</summary>
+        <summary>📌 NEW in 2.4 series</summary>
         
         Now, `alive_bar` supports *Dual Line* text mode!
         
         If you ever wanted to include longer situational messages within the bar, you probably felt squeezed into one line. You had to shrink the beautifully animated bar or, even worse, remove widgets (!) to be able to see what you needed...
         <br>Not anymore!! You can now make the bar *Dual Line*, and put text below it!
         
         Yes, there's a message below the whole bar, and any other print/logging messages scroll above it!
@@ -176,15 +170,15 @@
         -> Teaching the letter: S, please wait...
         ```
         
         There's also a new `finalize` function parameter in `alive_it` which enables you to set the title and/or text of the final receipt, and improved logging support which detects customized loggers.
         </details>
         
         <details>
-        <summary>📌 NEW in 2.3 series!</summary>
+        <summary>📌 NEW in 2.3 series</summary>
         
         This is all about customization; the core widgets can now be changed:
         - send a string to the `monitor`, `elapsed`, and `stats` widgets to make them look anyway you want!
         
         > It's incredible that these strings support all Python format features, so you can e.g., `{percent:.1%}` 😉.
         
         They can be further customized when on the **final receipt**!
@@ -218,41 +212,41 @@
         Download 7 |████████████⚠︎                           | (!) 30/100 [30%] in 0.8s (38.43/s)
         Download 8 |██████⚠︎                                 | (!) 15/100 [15%] in 0.4s (36.26/s)
         ...
         ```
         </details>
         
         <details>
-        <summary>📌 NEW in 2.2 series!</summary>
+        <summary>📌 NEW in 2.2 series</summary>
         
         Some major new features, often requested, have finally landed!
         - bar title can be dynamically set, changed, or even removed after being displayed
         - new custom fps system, which enables very slow refresh rates (to let it run on those k8s for long periods)
         - the final receipt can be totally hidden (great for special effects, like using the cool spinners standalone)
         - new support for `click.echo()` printing
         - terminal columns detection is safer for exotic environments
         - requires Python 3.7+
         </details>
         
         <details>
-        <summary>📌 NEW in 2.1 series!</summary>
+        <summary>📌 NEW in 2.1 series</summary>
         
         YES! Now `alive-progress` has support for Jupyter Notebooks and also includes a _Disabled_ state! Both were highly sought after, and have finally landed!
         <br>And better, I've implemented an auto-detection mechanism for jupyter notebooks, so it just works, out of the box, without any changes in your code!!
         
         See for yourself:
         
         ![alive-progress demo](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/alive-jupyter.gif)
         
         > It seems to work very well, but at this moment, it should be considered **experimental**.
         > <br>There were instances in which some visual glitches have appeared, like two `alive_bar` refreshes being concatenated together instead of over one another... And it's something I think I can't possibly work around: it seems Jupyter sometimes refresh the canvas at odd times, which makes it lose some data. Please let me know on the issues if something funnier arises.
         </details>
         
         <details>
-        <summary>📌 NEW in 2.0 series!</summary>
+        <summary>📌 NEW in 2.0 series</summary>
         
         This is a major breakthrough in `alive-progress`!
         <br>I took 1 year developing it, and I'm very proud of what I've accomplished \o/
         
         - now, there's complete support for Emojis 🤩 and exotic Unicode chars in general, which required MAJOR refactoring deep within the project, giving rise to what I called "**Cell Architecture**" => now, all internal components use and generate streams of cells instead of characters, and correctly interpret grapheme clusters — those so-called wide chars, which are encoded with a variable number of chars, but always take two cells on screen!! This has enabled us to render complex multi-chars symbols as if they were one, thus making them work on any spinners, bars, texts, borders and backgrounds, even when fractured!!! Pretty advanced stuff 🤓
         - new super cool spinner compiler and runner, which generates complete animations ahead of time, and plays these ready-to-go animations seamlessly, with no overhead at all! 🚀
         - the spinner compiler also includes advanced extra commands to generate and modify animations, like reshape, replace, transpose, or randomize the animation cycles!
@@ -821,17 +815,17 @@
         
         
         ### Forcing animations on PyCharm, Jupyter, etc.
         
         Do these astonishing `alive-progress` animations refuse to display?
         
         PyCharm is awesome, I love it! But I'll never understand why they've disabled emulating a terminal by default... If you do use PyCharm's output console, please enable this on all your Run Configurations:
-        ![alive-progress in pycharm](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/pycharm-terminal.png)
+        <p align="center"><img alt="alive-progress in pycharm" src="https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/pycharm-terminal.png"></p>
         
-        I even recommend you enter `File` > `New Projects Setup` > `Run Configuration Templates`, select `Python`, and also enable it there, so any new ones you create will already have this set.
+        > I even recommend you go into `File` > `New Projects Setup` > `Run Configuration Templates`, select `Python`, and also enable it there, so any new ones you create will already have this set.
         
         In addition to that, some terminals report themselves as "non-interactive", like when running out of a real terminal (PyCharm and Jupyter for example), in shell pipelines (`cat file.txt | python program.py`), or in background processes (not connected to a tty).
         
         When `alive-progress` finds itself in a non-interactive terminal, it automatically disables all kinds of animations, printing only the final receipt. This is made in order to avoid both messing up the pipeline output and spamming your log file with thousands of `alive-progress` refreshes.
         
         So, when you know it's safe, you can force them to see `alive-progress` in all its glory! Here is the `force_tty` argument:
```

### Comparing `alive-progress-3.1.1/README.md` & `alive-progress-3.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,65 @@
 [<img align="right" src="https://cdn.buymeacoffee.com/buttons/default-orange.png" width="217px" height="51x">](https://www.buymeacoffee.com/rsalmei)
 [<img align="right" alt="Donate with PayPal button" src="https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif">](https://www.paypal.com/donate?business=6SWSHEB5ZNS5N&no_recurring=0&item_name=I%27m+the+author+of+alive-progress%2C+clearly+and+about-time.+Thank+you+for+appreciating+my+work%21&currency_code=USD)
 
 ![alive-progress logo](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/alive-logo.gif)
 
-# alive-progress :)
-### A new kind of Progress Bar, with real-time throughput, ETA, and very cool animations!
+# alive-progress
 
-[![Maintenance](https://img.shields.io/badge/Maintained-yes-green.svg)](https://gitHub.com/rsalmei/alive-progress/graphs/commit-activity)
+[![Maintenance](https://img.shields.io/badge/maintained-yes-brightgreen.svg)](https://gitHub.com/rsalmei/alive-progress/graphs/commit-activity)
 [![PyPI version](https://img.shields.io/pypi/v/alive-progress.svg)](https://pypi.python.org/pypi/alive-progress/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/alive-progress.svg)](https://pypi.python.org/pypi/alive-progress/)
-[![PyPI status](https://img.shields.io/pypi/status/alive-progress.svg)](https://pypi.python.org/pypi/alive-progress/)
 [![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=week&units=international_system&left_color=grey&right_color=orange&left_text=downloads/week)](https://pepy.tech/project/alive-progress)
 [![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=month&units=international_system&left_color=grey&right_color=orange&left_text=/month)](https://pepy.tech/project/alive-progress)
 [![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=total&units=international_system&left_color=grey&right_color=orange&left_text=total)](https://pepy.tech/project/alive-progress)
+![GitHub Sponsors](https://img.shields.io/github/sponsors/rsalmei)
+
+
+Have you ever wondered where your lengthy processing was at, and when would it finish? Do you usually hit `RETURN` several times to make sure it didn't crash, or the SSH connection didn't freeze? Have you ever thought it'd be awesome to be able to _pause some processing_ without hassle, return to the Python prompt to manually fix some items, then _seamlessly resume_ it? I did...
+
+I've started this new progress bar thinking about all that, behold the **alive-progress**! 😃
+
+![alive-progress demo](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/alive-demo.gif)
+
+
+Introducing the newest concept in progress bars for Python! `alive-progress` is in a class of its own, with an array of cool features that set it apart. Here are a few highlights:
+- A mesmerizing **live spinner** that clearly shows your lengthy process did not crash and your SSH connection did not freeze, with **visual feedback** reacting to your processing speed.
+- An efficient **multithreaded** bar that updates itself at a fraction of the actual processing speed to keep **CPU usage low** and avoid terminal spamming (1,000,000 iterations per second equates to roughly 60 updates per second, and you can also calibrate this to your liking).
+- An **ETA** (expected time of arrival) feature with an intelligent _Exponential Smoothing Algorithm_ that shows the time to completion, allowing you to plan your time and manage your workload more effectively.
+- Automatic **print** and **logging** hooks that provide seamless integration and effortless tracking, even enriching them with the current bar position when they occur.
+- It prints a **nice receipt** when the processing finishes, including the elapsed time and the observed throughput.
+- It detects **under** and **overflows**, enabling you to track hits, misses, or any desired count, not necessarily the actual iterations.
+- You can **pause** it! That's right, you heard it here first! No other progress bar anywhere has this feature! You can get back to the Python prompt during any processing, adjust some items, and get back into that running process as if it had never stopped! All `alive_bar` widgets are kept as they were, and the elapsed time nicely ignores the paused time!
+- It is **highly customizable**, with a smorgasbord of spinner and bar styles, as well as several ready-to-use factories to easily generate yours! You can even use the super powerful and cool `check()` tool to help you design your own animations! You can see all the generated frames and cycles exploded on screen, with several verbosity levels, even including an _alive_ rendition! It's boundless creativity at your fingertips!
+
+---
+## Table of contents
+
+This README is always evolving, so do take a more comprehensive look from time to time... You might find great new details in other sections! 😊
 
 <!-- TOC -->
-* [alive-progress :)](#alive-progress--)
-    * [A new kind of Progress Bar, with real-time throughput, ETA, and very cool animations!](#a-new-kind-of-progress-bar-with-real-time-throughput-eta-and-very-cool-animations-)
-  * [Introduction](#introduction)
-  * [📌 NEW in 3.1 series!](#-new-in-31-series-)
+* [alive-progress](#alive-progress)
+  * [Table of contents](#table-of-contents)
+  * [📌 NEW in 3.1 series](#-new-in-31-series)
   * [Using `alive-progress`](#using-alive-progress)
     * [Get it](#get-it)
     * [Try it](#try-it)
     * [Awake it](#awake-it)
     * [Master it](#master-it)
   * [Displaying messages](#displaying-messages)
   * [Auto-iterating](#auto-iterating)
   * [Modes of operation](#modes-of-operation)
-    * [Definite/unknown: Counters](#definiteunknown--counters)
-    * [Manual: Percentages](#manual--percentages)
+    * [Definite/unknown: Counters](#definiteunknown-counters)
+    * [Manual: Percentages](#manual-percentages)
     * [Summary of Modes](#summary-of-modes)
     * [The `bar()` handlers](#the-bar-handlers)
   * [Styles](#styles)
   * [Configuration](#configuration)
   * [Create your own animations](#create-your-own-animations)
-    * [Intro: How do they work?](#intro--how-do-they-work)
+    * [Intro: How do they work?](#intro-how-do-they-work)
     * [A Spinner Compiler, really?](#a-spinner-compiler-really)
     * [Spinner Factories](#spinner-factories)
     * [Bar Factories](#bar-factories)
   * [Advanced](#advanced)
     * [The Pause Mechanism](#the-pause-mechanism)
     * [Loop-less use](#loop-less-use)
     * [FPS Calibration](#fps-calibration)
@@ -48,42 +69,15 @@
   * [Python End of Life notice](#python-end-of-life-notice)
     * [For new Python 2.7 and 3.5](#for-new-python-27-and-35)
     * [For new Python 3.6](#for-new-python-36)
   * [License](#license)
 <!-- TOC -->
 
 
-This README is always evolving, so do take a more comprehensive look from time to time... You might find great new details in other sections! 😊
-
-
-## Introduction
-
-Have you ever wondered where your lengthy processing was, and when it would finish? Ever found yourself hitting [RETURN] now and then to ensure it didn't hang, or if, in a remote SSH session, the connection was still working? Ever needed to *pause* some processing for a while, return to the Python prompt for a manual inspection or fixing an item, and then *resume* the process seamlessly? I did...
-
-I've started this cool progress bar thinking about all that, the **alive-progress**! 😃
-
-![alive-progress demo](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/alive-demo.gif)
-
-
-I like to think of this as a new kind of progress bar for Python since it has, among other things:
-
-- a **live spinner** that is incredibly cool and clearly shows your lengthy process did not hang, or your ssh connection did not drop;
-- a **visual feedback** which reacts to your processing, as the live spinner will go faster or slower with it;
-- an **efficient** multithreaded bar, which updates itself at a fraction of the actual processing speed (1,000,000 iterations per second equates to roughly 60 updates per second) to keep **CPU usage low** and avoid terminal spamming (you can also calibrate this to your liking);
-- nice monitoring of both _position and throughput_ of your processing;
-- an **ETA** (expected time of arrival) with an intelligent _exponential smoothing algorithm_, that shows the time to completion;
-- automatic **print** and **logging** hooks, which allow print statements and logging messages to work _effortlessly_, right amid an animated bar, and even enriching them with the current bar position when they occur;
-- a **nice receipt** is printed when your processing finishes, including the last bar rendition, the elapsed time, and the observed throughput;
-- it detects **under and overflows**, enabling you to track hits, misses, or any desired count, not necessarily the actual iterations;
-- it automatically detects if there's an **allocated tty**, and if there isn't (like in a shell pipeline), only the final receipt is printed (so you can safely include it in any code, and rest assured your log file won't get thousands of progress lines);
-- you can **pause** it! I think that's an unprecedented feature for progress bars ANYWHERE — in Python or any other language — no one has ever done it! It's incredible to be able to get back to the Python prompt during any running process! Then you can manually adjust an item or prepare something and get back into that running process as if it had never stopped!! All `alive_bar` widgets are kept as they were, and the elapsed time nicely ignores the paused time!;
-- it is **customizable**, with a growing smorgasbord of spinner and bar styles, as well as several ready-to-use factories to easily generate yours! Now (📌 new in 2.0), we even have a super powerful and cool `check()` tool, in both spinners and bars, to help you design your own animations! You can see all the frames and cycles exploded on screen, with several verbosity levels, even including an **alive** rendition! It's awesome 😜
-
-
-## 📌 NEW in 3.1 series!
+## 📌 NEW in 3.1 series
 
 A very cool update here! In addition to polishing things up and improving terminal support, now `alive-progress` supports resuming computations!
 
 When processing huge datasets or things that take a long time, you might either use batches or cache partial results. Then, in case it stops and is restarted, you end up skipping all those already done items very quickly, which makes the `alive_bar` think you're processing thousands of items per second, which in turn completely ruins the ETA... But not anymore! Just tell `bar()` that you've skipped items... 👏
 
 You can use it in two ways:
 
@@ -115,15 +109,15 @@
 - new `max_cols` config setting, the number of columns to use if not possible to fetch it, like in jupyter and other platforms which doesn't support size
 - fix fetching the size of the terminal when using stderr
 - officially supports Python 3.11
 - included [ruff](https://github.com/charliermarsh/ruff) linter before building
 
 
 <details>
-<summary>📌 NEW in 3.0 series!</summary>
+<summary>📌 NEW in 3.0 series</summary>
 
 Yep, I could finally get this version out! These are the new goodies:
 
 - Units support! You can now label the data you're processing, like `B`, `bytes`, or even `°C`!
 - Automatic scaling! With support for SI (base 1000), IEC (base 1024), and even an alternate SI with base 1024, you'll be well served!
 - Configurable precision! When your numbers are scaled, you get to choose how many decimals they display!
 - Automatic stats scaling for slow throughputs! If your processing takes minutes or more, now you'll see rates per minute, per hour, and even per day! (It works within the auto-scaling system!)
@@ -139,15 +133,15 @@
 - Fix unknown mode always ending with a warning (!)
 
 And last but not least, a more polished layout for you to enjoy your progress!
 ![alive-progress 3.0](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/alive3.0.png)
 </details>
 
 <details>
-<summary>📌 NEW in 2.4 series!</summary>
+<summary>📌 NEW in 2.4 series</summary>
 
 Now, `alive_bar` supports *Dual Line* text mode!
 
 If you ever wanted to include longer situational messages within the bar, you probably felt squeezed into one line. You had to shrink the beautifully animated bar or, even worse, remove widgets (!) to be able to see what you needed...
 <br>Not anymore!! You can now make the bar *Dual Line*, and put text below it!
 
 Yes, there's a message below the whole bar, and any other print/logging messages scroll above it!
@@ -168,15 +162,15 @@
 -> Teaching the letter: S, please wait...
 ```
 
 There's also a new `finalize` function parameter in `alive_it` which enables you to set the title and/or text of the final receipt, and improved logging support which detects customized loggers.
 </details>
 
 <details>
-<summary>📌 NEW in 2.3 series!</summary>
+<summary>📌 NEW in 2.3 series</summary>
 
 This is all about customization; the core widgets can now be changed:
 - send a string to the `monitor`, `elapsed`, and `stats` widgets to make them look anyway you want!
 
 > It's incredible that these strings support all Python format features, so you can e.g., `{percent:.1%}` 😉.
 
 They can be further customized when on the **final receipt**!
@@ -210,41 +204,41 @@
 Download 7 |████████████⚠︎                           | (!) 30/100 [30%] in 0.8s (38.43/s)
 Download 8 |██████⚠︎                                 | (!) 15/100 [15%] in 0.4s (36.26/s)
 ...
 ```
 </details>
 
 <details>
-<summary>📌 NEW in 2.2 series!</summary>
+<summary>📌 NEW in 2.2 series</summary>
 
 Some major new features, often requested, have finally landed!
 - bar title can be dynamically set, changed, or even removed after being displayed
 - new custom fps system, which enables very slow refresh rates (to let it run on those k8s for long periods)
 - the final receipt can be totally hidden (great for special effects, like using the cool spinners standalone)
 - new support for `click.echo()` printing
 - terminal columns detection is safer for exotic environments
 - requires Python 3.7+
 </details>
 
 <details>
-<summary>📌 NEW in 2.1 series!</summary>
+<summary>📌 NEW in 2.1 series</summary>
 
 YES! Now `alive-progress` has support for Jupyter Notebooks and also includes a _Disabled_ state! Both were highly sought after, and have finally landed!
 <br>And better, I've implemented an auto-detection mechanism for jupyter notebooks, so it just works, out of the box, without any changes in your code!!
 
 See for yourself:
 
 ![alive-progress demo](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/alive-jupyter.gif)
 
 > It seems to work very well, but at this moment, it should be considered **experimental**.
 > <br>There were instances in which some visual glitches have appeared, like two `alive_bar` refreshes being concatenated together instead of over one another... And it's something I think I can't possibly work around: it seems Jupyter sometimes refresh the canvas at odd times, which makes it lose some data. Please let me know on the issues if something funnier arises.
 </details>
 
 <details>
-<summary>📌 NEW in 2.0 series!</summary>
+<summary>📌 NEW in 2.0 series</summary>
 
 This is a major breakthrough in `alive-progress`!
 <br>I took 1 year developing it, and I'm very proud of what I've accomplished \o/
 
 - now, there's complete support for Emojis 🤩 and exotic Unicode chars in general, which required MAJOR refactoring deep within the project, giving rise to what I called "**Cell Architecture**" => now, all internal components use and generate streams of cells instead of characters, and correctly interpret grapheme clusters — those so-called wide chars, which are encoded with a variable number of chars, but always take two cells on screen!! This has enabled us to render complex multi-chars symbols as if they were one, thus making them work on any spinners, bars, texts, borders and backgrounds, even when fractured!!! Pretty advanced stuff 🤓
 - new super cool spinner compiler and runner, which generates complete animations ahead of time, and plays these ready-to-go animations seamlessly, with no overhead at all! 🚀
 - the spinner compiler also includes advanced extra commands to generate and modify animations, like reshape, replace, transpose, or randomize the animation cycles!
@@ -813,17 +807,17 @@
 
 
 ### Forcing animations on PyCharm, Jupyter, etc.
 
 Do these astonishing `alive-progress` animations refuse to display?
 
 PyCharm is awesome, I love it! But I'll never understand why they've disabled emulating a terminal by default... If you do use PyCharm's output console, please enable this on all your Run Configurations:
-![alive-progress in pycharm](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/pycharm-terminal.png)
+<p align="center"><img alt="alive-progress in pycharm" src="https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/pycharm-terminal.png"></p>
 
-I even recommend you enter `File` > `New Projects Setup` > `Run Configuration Templates`, select `Python`, and also enable it there, so any new ones you create will already have this set.
+> I even recommend you go into `File` > `New Projects Setup` > `Run Configuration Templates`, select `Python`, and also enable it there, so any new ones you create will already have this set.
 
 In addition to that, some terminals report themselves as "non-interactive", like when running out of a real terminal (PyCharm and Jupyter for example), in shell pipelines (`cat file.txt | python program.py`), or in background processes (not connected to a tty).
 
 When `alive-progress` finds itself in a non-interactive terminal, it automatically disables all kinds of animations, printing only the final receipt. This is made in order to avoid both messing up the pipeline output and spamming your log file with thousands of `alive-progress` refreshes.
 
 So, when you know it's safe, you can force them to see `alive-progress` in all its glory! Here is the `force_tty` argument:
```

### Comparing `alive-progress-3.1.1/alive_progress/animations/bars.py` & `alive-progress-3.1.2/alive_progress/animations/bars.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress/animations/spinner_compiler.py` & `alive-progress-3.1.2/alive_progress/animations/spinner_compiler.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress/animations/spinners.py` & `alive-progress-3.1.2/alive_progress/animations/spinners.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress/animations/utils.py` & `alive-progress-3.1.2/alive_progress/animations/utils.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress/core/calibration.py` & `alive-progress-3.1.2/alive_progress/core/calibration.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress/core/configuration.py` & `alive-progress-3.1.2/alive_progress/core/configuration.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress/core/hook_manager.py` & `alive-progress-3.1.2/alive_progress/core/hook_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,17 +35,26 @@
 
     def write(stream, part):
         if isinstance(part, bytes):
             part = part.decode(ENCODING)
 
         buffer = buffers[stream]
         if part != '\n':
-            if part.startswith('\x1b'):  # if the part starts with ESC, just send it.
-                stream.write(part)
-                return
+            osc = part.find('\x1b]')  # https://en.wikipedia.org/wiki/ANSI_escape_code
+            if osc >= 0:
+                end, s = part.find('\x07', osc + 2), 1  # 1 -> len('\x07')
+                if end < 0:
+                    end, s = part.find('\x1b\\', osc + 2), 2  # 2 -> len('\x1b\\')
+                    if end < 0:
+                        end, s = len(part), 0
+                stream.write(part[osc:end + s])
+                stream.flush()
+                part = part[:osc] + part[end + s:]
+                if not part:
+                    return
             # this will generate a sequence of lines interspersed with None, which will later
             # be rendered as the indent filler to align additional lines under the same header.
             gen = chain.from_iterable(zip(repeat(None), part.splitlines(True)))
             buffer.extend(islice(gen, 1, None))
         else:
             header = get_header()
             spacer = ' ' * len(header)
```

### Comparing `alive-progress-3.1.1/alive_progress/core/progress.py` & `alive-progress-3.1.2/alive_progress/core/progress.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     Also, the bar installs a hook in the system print function that cleans
     any garbage out of the terminal, allowing you to print() effortlessly
     while using the bar.
 
     Use it like this:
 
     >>> from alive_progress import alive_bar
-    ... with alive_bar(123, 'Title') as bar:  # <-- expected total and bar title
+    ... with alive_bar(123, title='Title') as bar:  # <-- expected total and bar title
     ...     for item in <iterable>:
     ...         # process item
     ...         bar()  # makes the bar go forward
 
     The `bar()` method should be called whenever you want the bar to go forward.
     You usually call it in every iteration, but you could do it only when some
     criteria match, depending on what you want to monitor.
```

### Comparing `alive-progress-3.1.1/alive_progress/styles/__init__.py` & `alive-progress-3.1.2/alive_progress/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress/styles/exhibit.py` & `alive-progress-3.1.2/alive_progress/styles/exhibit.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress/styles/internal.py` & `alive-progress-3.1.2/alive_progress/styles/internal.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress/tools/demo.py` & `alive-progress-3.1.2/alive_progress/tools/demo.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress/tools/repl.py` & `alive-progress-3.1.2/alive_progress/tools/repl.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress/tools/sampling.py` & `alive-progress-3.1.2/alive_progress/tools/sampling.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress/tools/unicode_breaks.py` & `alive-progress-3.1.2/alive_progress/tools/unicode_breaks.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress/utils/cells.py` & `alive-progress-3.1.2/alive_progress/utils/cells.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress/utils/colors.py` & `alive-progress-3.1.2/alive_progress/utils/colors.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress/utils/terminal/__init__.py` & `alive-progress-3.1.2/alive_progress/utils/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress/utils/terminal/jupyter.py` & `alive-progress-3.1.2/alive_progress/utils/terminal/jupyter.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress/utils/terminal/tty.py` & `alive-progress-3.1.2/alive_progress/utils/terminal/tty.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress/utils/terminal/void.py` & `alive-progress-3.1.2/alive_progress/utils/terminal/void.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress/utils/timing.py` & `alive-progress-3.1.2/alive_progress/utils/timing.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/alive_progress.egg-info/PKG-INFO` & `alive-progress-3.1.2/alive_progress.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,52 +1,73 @@
 Metadata-Version: 2.1
 Name: alive-progress
-Version: 3.1.1
+Version: 3.1.2
 Summary: A new kind of Progress Bar, with real-time throughput, ETA, and very cool animations!
 Home-page: https://github.com/rsalmei/alive-progress
 Author: Rogério Sampaio de Almeida
 Author-email: rsalmei@gmail.com
 License: MIT
 Description: [<img align="right" src="https://cdn.buymeacoffee.com/buttons/default-orange.png" width="217px" height="51x">](https://www.buymeacoffee.com/rsalmei)
         [<img align="right" alt="Donate with PayPal button" src="https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif">](https://www.paypal.com/donate?business=6SWSHEB5ZNS5N&no_recurring=0&item_name=I%27m+the+author+of+alive-progress%2C+clearly+and+about-time.+Thank+you+for+appreciating+my+work%21&currency_code=USD)
         
         ![alive-progress logo](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/alive-logo.gif)
         
-        # alive-progress :)
-        ### A new kind of Progress Bar, with real-time throughput, ETA, and very cool animations!
+        # alive-progress
         
-        [![Maintenance](https://img.shields.io/badge/Maintained-yes-green.svg)](https://gitHub.com/rsalmei/alive-progress/graphs/commit-activity)
+        [![Maintenance](https://img.shields.io/badge/maintained-yes-brightgreen.svg)](https://gitHub.com/rsalmei/alive-progress/graphs/commit-activity)
         [![PyPI version](https://img.shields.io/pypi/v/alive-progress.svg)](https://pypi.python.org/pypi/alive-progress/)
         [![PyPI pyversions](https://img.shields.io/pypi/pyversions/alive-progress.svg)](https://pypi.python.org/pypi/alive-progress/)
-        [![PyPI status](https://img.shields.io/pypi/status/alive-progress.svg)](https://pypi.python.org/pypi/alive-progress/)
         [![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=week&units=international_system&left_color=grey&right_color=orange&left_text=downloads/week)](https://pepy.tech/project/alive-progress)
         [![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=month&units=international_system&left_color=grey&right_color=orange&left_text=/month)](https://pepy.tech/project/alive-progress)
         [![Downloads](https://static.pepy.tech/personalized-badge/alive-progress?period=total&units=international_system&left_color=grey&right_color=orange&left_text=total)](https://pepy.tech/project/alive-progress)
+        ![GitHub Sponsors](https://img.shields.io/github/sponsors/rsalmei)
+        
+        
+        Have you ever wondered where your lengthy processing was at, and when would it finish? Do you usually hit `RETURN` several times to make sure it didn't crash, or the SSH connection didn't freeze? Have you ever thought it'd be awesome to be able to _pause some processing_ without hassle, return to the Python prompt to manually fix some items, then _seamlessly resume_ it? I did...
+        
+        I've started this new progress bar thinking about all that, behold the **alive-progress**! 😃
+        
+        ![alive-progress demo](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/alive-demo.gif)
+        
+        
+        Introducing the newest concept in progress bars for Python! `alive-progress` is in a class of its own, with an array of cool features that set it apart. Here are a few highlights:
+        - A mesmerizing **live spinner** that clearly shows your lengthy process did not crash and your SSH connection did not freeze, with **visual feedback** reacting to your processing speed.
+        - An efficient **multithreaded** bar that updates itself at a fraction of the actual processing speed to keep **CPU usage low** and avoid terminal spamming (1,000,000 iterations per second equates to roughly 60 updates per second, and you can also calibrate this to your liking).
+        - An **ETA** (expected time of arrival) feature with an intelligent _Exponential Smoothing Algorithm_ that shows the time to completion, allowing you to plan your time and manage your workload more effectively.
+        - Automatic **print** and **logging** hooks that provide seamless integration and effortless tracking, even enriching them with the current bar position when they occur.
+        - It prints a **nice receipt** when the processing finishes, including the elapsed time and the observed throughput.
+        - It detects **under** and **overflows**, enabling you to track hits, misses, or any desired count, not necessarily the actual iterations.
+        - You can **pause** it! That's right, you heard it here first! No other progress bar anywhere has this feature! You can get back to the Python prompt during any processing, adjust some items, and get back into that running process as if it had never stopped! All `alive_bar` widgets are kept as they were, and the elapsed time nicely ignores the paused time!
+        - It is **highly customizable**, with a smorgasbord of spinner and bar styles, as well as several ready-to-use factories to easily generate yours! You can even use the super powerful and cool `check()` tool to help you design your own animations! You can see all the generated frames and cycles exploded on screen, with several verbosity levels, even including an _alive_ rendition! It's boundless creativity at your fingertips!
+        
+        ---
+        ## Table of contents
+        
+        This README is always evolving, so do take a more comprehensive look from time to time... You might find great new details in other sections! 😊
         
         <!-- TOC -->
-        * [alive-progress :)](#alive-progress--)
-            * [A new kind of Progress Bar, with real-time throughput, ETA, and very cool animations!](#a-new-kind-of-progress-bar-with-real-time-throughput-eta-and-very-cool-animations-)
-          * [Introduction](#introduction)
-          * [📌 NEW in 3.1 series!](#-new-in-31-series-)
+        * [alive-progress](#alive-progress)
+          * [Table of contents](#table-of-contents)
+          * [📌 NEW in 3.1 series](#-new-in-31-series)
           * [Using `alive-progress`](#using-alive-progress)
             * [Get it](#get-it)
             * [Try it](#try-it)
             * [Awake it](#awake-it)
             * [Master it](#master-it)
           * [Displaying messages](#displaying-messages)
           * [Auto-iterating](#auto-iterating)
           * [Modes of operation](#modes-of-operation)
-            * [Definite/unknown: Counters](#definiteunknown--counters)
-            * [Manual: Percentages](#manual--percentages)
+            * [Definite/unknown: Counters](#definiteunknown-counters)
+            * [Manual: Percentages](#manual-percentages)
             * [Summary of Modes](#summary-of-modes)
             * [The `bar()` handlers](#the-bar-handlers)
           * [Styles](#styles)
           * [Configuration](#configuration)
           * [Create your own animations](#create-your-own-animations)
-            * [Intro: How do they work?](#intro--how-do-they-work)
+            * [Intro: How do they work?](#intro-how-do-they-work)
             * [A Spinner Compiler, really?](#a-spinner-compiler-really)
             * [Spinner Factories](#spinner-factories)
             * [Bar Factories](#bar-factories)
           * [Advanced](#advanced)
             * [The Pause Mechanism](#the-pause-mechanism)
             * [Loop-less use](#loop-less-use)
             * [FPS Calibration](#fps-calibration)
@@ -56,42 +77,15 @@
           * [Python End of Life notice](#python-end-of-life-notice)
             * [For new Python 2.7 and 3.5](#for-new-python-27-and-35)
             * [For new Python 3.6](#for-new-python-36)
           * [License](#license)
         <!-- TOC -->
         
         
-        This README is always evolving, so do take a more comprehensive look from time to time... You might find great new details in other sections! 😊
-        
-        
-        ## Introduction
-        
-        Have you ever wondered where your lengthy processing was, and when it would finish? Ever found yourself hitting [RETURN] now and then to ensure it didn't hang, or if, in a remote SSH session, the connection was still working? Ever needed to *pause* some processing for a while, return to the Python prompt for a manual inspection or fixing an item, and then *resume* the process seamlessly? I did...
-        
-        I've started this cool progress bar thinking about all that, the **alive-progress**! 😃
-        
-        ![alive-progress demo](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/alive-demo.gif)
-        
-        
-        I like to think of this as a new kind of progress bar for Python since it has, among other things:
-        
-        - a **live spinner** that is incredibly cool and clearly shows your lengthy process did not hang, or your ssh connection did not drop;
-        - a **visual feedback** which reacts to your processing, as the live spinner will go faster or slower with it;
-        - an **efficient** multithreaded bar, which updates itself at a fraction of the actual processing speed (1,000,000 iterations per second equates to roughly 60 updates per second) to keep **CPU usage low** and avoid terminal spamming (you can also calibrate this to your liking);
-        - nice monitoring of both _position and throughput_ of your processing;
-        - an **ETA** (expected time of arrival) with an intelligent _exponential smoothing algorithm_, that shows the time to completion;
-        - automatic **print** and **logging** hooks, which allow print statements and logging messages to work _effortlessly_, right amid an animated bar, and even enriching them with the current bar position when they occur;
-        - a **nice receipt** is printed when your processing finishes, including the last bar rendition, the elapsed time, and the observed throughput;
-        - it detects **under and overflows**, enabling you to track hits, misses, or any desired count, not necessarily the actual iterations;
-        - it automatically detects if there's an **allocated tty**, and if there isn't (like in a shell pipeline), only the final receipt is printed (so you can safely include it in any code, and rest assured your log file won't get thousands of progress lines);
-        - you can **pause** it! I think that's an unprecedented feature for progress bars ANYWHERE — in Python or any other language — no one has ever done it! It's incredible to be able to get back to the Python prompt during any running process! Then you can manually adjust an item or prepare something and get back into that running process as if it had never stopped!! All `alive_bar` widgets are kept as they were, and the elapsed time nicely ignores the paused time!;
-        - it is **customizable**, with a growing smorgasbord of spinner and bar styles, as well as several ready-to-use factories to easily generate yours! Now (📌 new in 2.0), we even have a super powerful and cool `check()` tool, in both spinners and bars, to help you design your own animations! You can see all the frames and cycles exploded on screen, with several verbosity levels, even including an **alive** rendition! It's awesome 😜
-        
-        
-        ## 📌 NEW in 3.1 series!
+        ## 📌 NEW in 3.1 series
         
         A very cool update here! In addition to polishing things up and improving terminal support, now `alive-progress` supports resuming computations!
         
         When processing huge datasets or things that take a long time, you might either use batches or cache partial results. Then, in case it stops and is restarted, you end up skipping all those already done items very quickly, which makes the `alive_bar` think you're processing thousands of items per second, which in turn completely ruins the ETA... But not anymore! Just tell `bar()` that you've skipped items... 👏
         
         You can use it in two ways:
         
@@ -123,15 +117,15 @@
         - new `max_cols` config setting, the number of columns to use if not possible to fetch it, like in jupyter and other platforms which doesn't support size
         - fix fetching the size of the terminal when using stderr
         - officially supports Python 3.11
         - included [ruff](https://github.com/charliermarsh/ruff) linter before building
         
         
         <details>
-        <summary>📌 NEW in 3.0 series!</summary>
+        <summary>📌 NEW in 3.0 series</summary>
         
         Yep, I could finally get this version out! These are the new goodies:
         
         - Units support! You can now label the data you're processing, like `B`, `bytes`, or even `°C`!
         - Automatic scaling! With support for SI (base 1000), IEC (base 1024), and even an alternate SI with base 1024, you'll be well served!
         - Configurable precision! When your numbers are scaled, you get to choose how many decimals they display!
         - Automatic stats scaling for slow throughputs! If your processing takes minutes or more, now you'll see rates per minute, per hour, and even per day! (It works within the auto-scaling system!)
@@ -147,15 +141,15 @@
         - Fix unknown mode always ending with a warning (!)
         
         And last but not least, a more polished layout for you to enjoy your progress!
         ![alive-progress 3.0](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/alive3.0.png)
         </details>
         
         <details>
-        <summary>📌 NEW in 2.4 series!</summary>
+        <summary>📌 NEW in 2.4 series</summary>
         
         Now, `alive_bar` supports *Dual Line* text mode!
         
         If you ever wanted to include longer situational messages within the bar, you probably felt squeezed into one line. You had to shrink the beautifully animated bar or, even worse, remove widgets (!) to be able to see what you needed...
         <br>Not anymore!! You can now make the bar *Dual Line*, and put text below it!
         
         Yes, there's a message below the whole bar, and any other print/logging messages scroll above it!
@@ -176,15 +170,15 @@
         -> Teaching the letter: S, please wait...
         ```
         
         There's also a new `finalize` function parameter in `alive_it` which enables you to set the title and/or text of the final receipt, and improved logging support which detects customized loggers.
         </details>
         
         <details>
-        <summary>📌 NEW in 2.3 series!</summary>
+        <summary>📌 NEW in 2.3 series</summary>
         
         This is all about customization; the core widgets can now be changed:
         - send a string to the `monitor`, `elapsed`, and `stats` widgets to make them look anyway you want!
         
         > It's incredible that these strings support all Python format features, so you can e.g., `{percent:.1%}` 😉.
         
         They can be further customized when on the **final receipt**!
@@ -218,41 +212,41 @@
         Download 7 |████████████⚠︎                           | (!) 30/100 [30%] in 0.8s (38.43/s)
         Download 8 |██████⚠︎                                 | (!) 15/100 [15%] in 0.4s (36.26/s)
         ...
         ```
         </details>
         
         <details>
-        <summary>📌 NEW in 2.2 series!</summary>
+        <summary>📌 NEW in 2.2 series</summary>
         
         Some major new features, often requested, have finally landed!
         - bar title can be dynamically set, changed, or even removed after being displayed
         - new custom fps system, which enables very slow refresh rates (to let it run on those k8s for long periods)
         - the final receipt can be totally hidden (great for special effects, like using the cool spinners standalone)
         - new support for `click.echo()` printing
         - terminal columns detection is safer for exotic environments
         - requires Python 3.7+
         </details>
         
         <details>
-        <summary>📌 NEW in 2.1 series!</summary>
+        <summary>📌 NEW in 2.1 series</summary>
         
         YES! Now `alive-progress` has support for Jupyter Notebooks and also includes a _Disabled_ state! Both were highly sought after, and have finally landed!
         <br>And better, I've implemented an auto-detection mechanism for jupyter notebooks, so it just works, out of the box, without any changes in your code!!
         
         See for yourself:
         
         ![alive-progress demo](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/alive-jupyter.gif)
         
         > It seems to work very well, but at this moment, it should be considered **experimental**.
         > <br>There were instances in which some visual glitches have appeared, like two `alive_bar` refreshes being concatenated together instead of over one another... And it's something I think I can't possibly work around: it seems Jupyter sometimes refresh the canvas at odd times, which makes it lose some data. Please let me know on the issues if something funnier arises.
         </details>
         
         <details>
-        <summary>📌 NEW in 2.0 series!</summary>
+        <summary>📌 NEW in 2.0 series</summary>
         
         This is a major breakthrough in `alive-progress`!
         <br>I took 1 year developing it, and I'm very proud of what I've accomplished \o/
         
         - now, there's complete support for Emojis 🤩 and exotic Unicode chars in general, which required MAJOR refactoring deep within the project, giving rise to what I called "**Cell Architecture**" => now, all internal components use and generate streams of cells instead of characters, and correctly interpret grapheme clusters — those so-called wide chars, which are encoded with a variable number of chars, but always take two cells on screen!! This has enabled us to render complex multi-chars symbols as if they were one, thus making them work on any spinners, bars, texts, borders and backgrounds, even when fractured!!! Pretty advanced stuff 🤓
         - new super cool spinner compiler and runner, which generates complete animations ahead of time, and plays these ready-to-go animations seamlessly, with no overhead at all! 🚀
         - the spinner compiler also includes advanced extra commands to generate and modify animations, like reshape, replace, transpose, or randomize the animation cycles!
@@ -821,17 +815,17 @@
         
         
         ### Forcing animations on PyCharm, Jupyter, etc.
         
         Do these astonishing `alive-progress` animations refuse to display?
         
         PyCharm is awesome, I love it! But I'll never understand why they've disabled emulating a terminal by default... If you do use PyCharm's output console, please enable this on all your Run Configurations:
-        ![alive-progress in pycharm](https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/pycharm-terminal.png)
+        <p align="center"><img alt="alive-progress in pycharm" src="https://raw.githubusercontent.com/rsalmei/alive-progress/main/img/pycharm-terminal.png"></p>
         
-        I even recommend you enter `File` > `New Projects Setup` > `Run Configuration Templates`, select `Python`, and also enable it there, so any new ones you create will already have this set.
+        > I even recommend you go into `File` > `New Projects Setup` > `Run Configuration Templates`, select `Python`, and also enable it there, so any new ones you create will already have this set.
         
         In addition to that, some terminals report themselves as "non-interactive", like when running out of a real terminal (PyCharm and Jupyter for example), in shell pipelines (`cat file.txt | python program.py`), or in background processes (not connected to a tty).
         
         When `alive-progress` finds itself in a non-interactive terminal, it automatically disables all kinds of animations, printing only the final receipt. This is made in order to avoid both messing up the pipeline output and spamming your log file with thousands of `alive-progress` refreshes.
         
         So, when you know it's safe, you can force them to see `alive-progress` in all its glory! Here is the `force_tty` argument:
```

### Comparing `alive-progress-3.1.1/alive_progress.egg-info/SOURCES.txt` & `alive-progress-3.1.2/alive_progress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.1/setup.py` & `alive-progress-3.1.2/setup.py`

 * *Files identical despite different names*

