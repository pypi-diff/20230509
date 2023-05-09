# Comparing `tmp/stdl-0.4.2.tar.gz` & `tmp/stdl-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdl-0.4.2.tar", last modified: Wed Mar 29 20:36:47 2023, max compression
+gzip compressed data, was "stdl-0.4.3.tar", last modified: Tue May  9 18:36:48 2023, max compression
```

## Comparing `stdl-0.4.2.tar` & `stdl-0.4.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:36:47.208732 stdl-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-29 20:36:37.000000 stdl-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-03-29 20:36:47.208732 stdl-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-29 20:36:37.000000 stdl-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 20:36:47.208732 stdl-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-29 20:36:37.000000 stdl-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:36:47.208732 stdl-0.4.2/stdl/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-29 20:36:37.000000 stdl-0.4.2/stdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-29 20:36:37.000000 stdl-0.4.2/stdl/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-03-29 20:36:37.000000 stdl-0.4.2/stdl/dt.py
--rw-r--r--   0 runner    (1001) docker     (123)    27905 2023-03-29 20:36:37.000000 stdl-0.4.2/stdl/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-03-29 20:36:37.000000 stdl-0.4.2/stdl/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-03-29 20:36:37.000000 stdl-0.4.2/stdl/lst.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-03-29 20:36:37.000000 stdl-0.4.2/stdl/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-03-29 20:36:37.000000 stdl-0.4.2/stdl/str_u.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:36:47.208732 stdl-0.4.2/stdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-03-29 20:36:47.000000 stdl-0.4.2/stdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-29 20:36:47.000000 stdl-0.4.2/stdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 20:36:47.000000 stdl-0.4.2/stdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-29 20:36:47.000000 stdl-0.4.2/stdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-29 20:36:47.000000 stdl-0.4.2/stdl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:36:48.996237 stdl-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-09 18:36:35.000000 stdl-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-09 18:36:48.996237 stdl-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-09 18:36:35.000000 stdl-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-09 18:36:35.000000 stdl-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 18:36:48.996237 stdl-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 18:36:35.000000 stdl-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:36:48.992237 stdl-0.4.3/stdl/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-09 18:36:35.000000 stdl-0.4.3/stdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-09 18:36:35.000000 stdl-0.4.3/stdl/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-09 18:36:35.000000 stdl-0.4.3/stdl/dt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27905 2023-05-09 18:36:35.000000 stdl-0.4.3/stdl/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-09 18:36:35.000000 stdl-0.4.3/stdl/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-09 18:36:35.000000 stdl-0.4.3/stdl/lst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-09 18:36:35.000000 stdl-0.4.3/stdl/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-05-09 18:36:35.000000 stdl-0.4.3/stdl/str_u.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:36:48.996237 stdl-0.4.3/stdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-09 18:36:48.000000 stdl-0.4.3/stdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-09 18:36:48.000000 stdl-0.4.3/stdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 18:36:48.000000 stdl-0.4.3/stdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-09 18:36:48.000000 stdl-0.4.3/stdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 18:36:48.000000 stdl-0.4.3/stdl.egg-info/top_level.txt
```

### Comparing `stdl-0.4.2/LICENSE` & `stdl-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stdl-0.4.2/PKG-INFO` & `stdl-0.4.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: stdl
-Version: 0.4.2
+Version: 0.4.3
 Summary: Extended Python Standard Library
-Home-page: https://github.com/zigai/stdl
-Author: Žiga Ivanšek
-Author-email: ziga.ivansek@gmail.com
-License: MIT
+Author-email: Žiga Ivanšek <ziga.ivansek@gmail.com>
+Project-URL: repository, https://github.com/zigai/stdl
+Project-URL: homepage, https://github.com/zigai/stdl
+Keywords: python utilites,filesystem,string manipulation,logging configuration,list utils,standard library
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
 License-File: LICENSE
 
 # stdl
 [![PyPI version](https://badge.fury.io/py/stdl.svg)](https://badge.fury.io/py/stdl)
 ![Supported versions](https://img.shields.io/badge/python-3.10+-blue.svg)
 [![Downloads](https://static.pepy.tech/badge/stdl)](https://pepy.tech/project/stdl)
 [![license](https://img.shields.io/github/license/zigai/stdl.svg)](https://github.com/zigai/stdl/blob/main/LICENSE)
```

### Comparing `stdl-0.4.2/README.md` & `stdl-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `stdl-0.4.2/stdl/dt.py` & `stdl-0.4.3/stdl/dt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import random
 import time
+from dataclasses import dataclass
 from datetime import date, datetime, timedelta, timezone
 from typing import Generator
 
 from dateutil.parser import parse as parse_datetime_str
 
-from stdl.dataclass import Data, dataclass
-
 local_tz = datetime.now().astimezone().tzinfo
 
 
 @dataclass
-class TimerStop(Data):
+class TimerStop:
     total: timedelta
     since_last: timedelta
     at: float
     label: str | None = None
 
+    def __str__(self) -> str:
+        if self.label is None:
+            return f"total={self.total}, since_last=({self.since_last}), at={fmt_datetime(self.at)}"
+        return f"{self.label} | total={self.total}, since_last={self.since_last}, at={fmt_datetime(self.at)}"
+
 
 class Timer:
     """A simple timer class that keeps track of all the stops."""
 
     def __init__(self, *, ms: bool = True):
         self.ms = ms
         self.reset()
@@ -62,14 +66,18 @@
                 total=timedelta(seconds=0),
                 since_last=timedelta(seconds=0),
                 at=self.start,
                 label="start",
             )
         ]
 
+    def print_stops(self) -> None:
+        for stop in self.stops:
+            print(stop)
+
 
 def fmt_datetime(
     d: str | float | int | None | datetime = None,
     fmt: str = "Ymd",
     d_sep: str = "-",
     t_sep: str = ":",
     *,
```

### Comparing `stdl-0.4.2/stdl/fs.py` & `stdl-0.4.3/stdl/fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -572,15 +572,15 @@
         int: The number of bytes
     """
     # Based on https://stackoverflow.com/a/42865957/2002471
     KB_UNITS = {
         1024: {"B": 1, "KB": 2**10, "MB": 2**20, "GB": 2**30, "TB": 2**40},
         1000: {"B": 1, "KB": 10**3, "MB": 10**6, "GB": 10**9, "TB": 10**12},
     }
-    if not kb_size in KB_UNITS:
+    if kb_size not in KB_UNITS:
         raise ValueError(kb_size)
     if re.fullmatch(r"[\d]+", size):
         return int(size)
     size = size.upper()
     if not re.match(r" ", size):
         size = re.sub(r"([KMGT]?B)", r" \1", size)
     number, unit = [string.strip() for string in size.split()]
```

### Comparing `stdl-0.4.2/stdl/lst.py` & `stdl-0.4.3/stdl/lst.py`

 * *Files identical despite different names*

### Comparing `stdl-0.4.2/stdl/net.py` & `stdl-0.4.3/stdl/net.py`

 * *Files identical despite different names*

### Comparing `stdl-0.4.2/stdl/str_u.py` & `stdl-0.4.3/stdl/str_u.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,14 @@
 
 def colored(
     text: str,
     color: str | None = None,
     background: str | None = None,
     style: str | None = None,
 ):
-
     """
     Returns the text with ansi color, background color and text style codes.
 
     Args:
         text (str): The text that should be colorized.
         color (str, optional): The color to use for the text.
         background (str, optional): The color to use for the background.
@@ -178,15 +177,15 @@
         chrs (str | set): Characters to remove
         replacement (str, optional): If provided, replace the characters with this value.
 
     """
     string = []
     chrs = set(chrs)
     for c in s:
-        if not c in chrs:
+        if c not in chrs:
             string.append(c)
         else:
             if replacement:
                 string.append(replacement)
     return "".join(string)
```

### Comparing `stdl-0.4.2/stdl.egg-info/PKG-INFO` & `stdl-0.4.3/stdl.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: stdl
-Version: 0.4.2
+Version: 0.4.3
 Summary: Extended Python Standard Library
-Home-page: https://github.com/zigai/stdl
-Author: Žiga Ivanšek
-Author-email: ziga.ivansek@gmail.com
-License: MIT
+Author-email: Žiga Ivanšek <ziga.ivansek@gmail.com>
+Project-URL: repository, https://github.com/zigai/stdl
+Project-URL: homepage, https://github.com/zigai/stdl
+Keywords: python utilites,filesystem,string manipulation,logging configuration,list utils,standard library
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
 License-File: LICENSE
 
 # stdl
 [![PyPI version](https://badge.fury.io/py/stdl.svg)](https://badge.fury.io/py/stdl)
 ![Supported versions](https://img.shields.io/badge/python-3.10+-blue.svg)
 [![Downloads](https://static.pepy.tech/badge/stdl)](https://pepy.tech/project/stdl)
 [![license](https://img.shields.io/github/license/zigai/stdl.svg)](https://github.com/zigai/stdl/blob/main/LICENSE)
```

