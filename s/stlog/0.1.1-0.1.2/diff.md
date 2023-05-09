# Comparing `tmp/stlog-0.1.1.tar.gz` & `tmp/stlog-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stlog-0.1.1.tar", max compression
+gzip compressed data, was "stlog-0.1.2.tar", max compression
```

## Comparing `stlog-0.1.1.tar` & `stlog-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2023-05-06 14:19:55.564902 stlog-0.1.1/LICENSE
--rw-r--r--   0        0        0     8415 2023-05-06 14:19:55.564902 stlog-0.1.1/README.md
--rw-r--r--   0        0        0     1089 2023-05-06 14:20:16.933072 stlog-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      593 2023-05-06 14:20:16.585071 stlog-0.1.1/stlog/__init__.py
--rw-r--r--   0        0        0     2658 2023-05-06 14:19:55.568902 stlog-0.1.1/stlog/adapter.py
--rw-r--r--   0        0        0     7783 2023-05-06 14:19:55.568902 stlog-0.1.1/stlog/base.py
--rw-r--r--   0        0        0     2638 2023-05-06 14:19:55.568902 stlog-0.1.1/stlog/context.py
--rw-r--r--   0        0        0    14032 2023-05-06 14:19:55.568902 stlog-0.1.1/stlog/formatter.py
--rw-r--r--   0        0        0     2499 2023-05-06 14:19:55.568902 stlog-0.1.1/stlog/handler.py
--rw-r--r--   0        0        0     5276 2023-05-06 14:19:55.568902 stlog-0.1.1/stlog/kvformatter.py
--rw-r--r--   0        0        0     5249 2023-05-06 14:19:55.568902 stlog-0.1.1/stlog/output.py
--rw-r--r--   0        0        0     7077 2023-05-06 14:19:55.568902 stlog-0.1.1/stlog/setup.py
--rw-r--r--   0        0        0     8967 1970-01-01 00:00:00.000000 stlog-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-09 08:47:04.585869 stlog-0.1.2/LICENSE
+-rw-r--r--   0        0        0     8415 2023-05-09 08:47:04.585869 stlog-0.1.2/README.md
+-rw-r--r--   0        0        0     1089 2023-05-09 08:47:29.667365 stlog-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      593 2023-05-09 08:47:29.267341 stlog-0.1.2/stlog/__init__.py
+-rw-r--r--   0        0        0     2658 2023-05-09 08:47:04.593870 stlog-0.1.2/stlog/adapter.py
+-rw-r--r--   0        0        0     7783 2023-05-09 08:47:04.593870 stlog-0.1.2/stlog/base.py
+-rw-r--r--   0        0        0     2638 2023-05-09 08:47:04.593870 stlog-0.1.2/stlog/context.py
+-rw-r--r--   0        0        0    14032 2023-05-09 08:47:04.593870 stlog-0.1.2/stlog/formatter.py
+-rw-r--r--   0        0        0     2499 2023-05-09 08:47:04.593870 stlog-0.1.2/stlog/handler.py
+-rw-r--r--   0        0        0     5276 2023-05-09 08:47:04.593870 stlog-0.1.2/stlog/kvformatter.py
+-rw-r--r--   0        0        0     5426 2023-05-09 08:47:04.593870 stlog-0.1.2/stlog/output.py
+-rw-r--r--   0        0        0     7077 2023-05-09 08:47:04.593870 stlog-0.1.2/stlog/setup.py
+-rw-r--r--   0        0        0     8967 1970-01-01 00:00:00.000000 stlog-0.1.2/PKG-INFO
```

### Comparing `stlog-0.1.1/LICENSE` & `stlog-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stlog-0.1.1/README.md` & `stlog-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `stlog-0.1.1/pyproject.toml` & `stlog-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stlog"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Fabien MARTY <fabien.marty@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "stlog"}]
 
 [tool.poetry.dependencies]
```

### Comparing `stlog-0.1.1/stlog/__init__.py` & `stlog-0.1.2/stlog/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,8 +33,8 @@
     "base": False,
     "adapter": False,
     "handler": False,
     "context": False,
     "warn": False,
     "fatal": False,
 }
-VERSION = "0.1.1"
+VERSION = "0.1.2"
```

### Comparing `stlog-0.1.1/stlog/adapter.py` & `stlog-0.1.2/stlog/adapter.py`

 * *Files identical despite different names*

### Comparing `stlog-0.1.1/stlog/base.py` & `stlog-0.1.2/stlog/base.py`

 * *Files identical despite different names*

### Comparing `stlog-0.1.1/stlog/context.py` & `stlog-0.1.2/stlog/context.py`

 * *Files identical despite different names*

### Comparing `stlog-0.1.1/stlog/formatter.py` & `stlog-0.1.2/stlog/formatter.py`

 * *Files identical despite different names*

### Comparing `stlog-0.1.1/stlog/handler.py` & `stlog-0.1.2/stlog/handler.py`

 * *Files identical despite different names*

### Comparing `stlog-0.1.1/stlog/kvformatter.py` & `stlog-0.1.2/stlog/kvformatter.py`

 * *Files identical despite different names*

### Comparing `stlog-0.1.1/stlog/output.py` & `stlog-0.1.2/stlog/output.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import sys
 import typing
 from dataclasses import dataclass, field
 
 from stlog.base import StlogError
 from stlog.formatter import (
+    Formatter,
     HumanFormatter,
     RichHumanFormatter,
 )
 from stlog.handler import CustomRichHandler
 
 RICH_INSTALLED: bool = False
 try:
@@ -114,15 +115,16 @@
             )
         self.set_handler(CustomRichHandler(console=self.console))
 
 
 def make_stream_or_rich_stream_output(
     stream: typing.TextIO = sys.stderr,
     use_rich: bool | None = DEFAULT_USE_RICH,
-    formatter_kwargs: dict[str, typing.Any] | None = None,
+    rich_formatter: Formatter | None = None,
+    not_rich_formatter: Formatter | None = None,
     **kwargs,
 ) -> StreamOutput:
     """Create automatically a `stlog.output.RichStreamOutput` or a (classic)`stlog.output.StreamOutput`.
 
     To get a `stlog.output.RichStreamOutput`, following conditions must be true:
 
     - `rich` library must be installed and available in python path
@@ -133,35 +135,36 @@
     NOTE: the default value of the `use_rich` parameter is `None` (automatic) but it can be forced by
     the `STLOG_USE_RICH` env variable.
 
     Attributes:
         stream: the stream to use (`typing.TextIO`), default to `sys.stderr`.
         use_rich: if None, use [rich output](https://github.com/Textualize/rich/blob/master/README.md) if possible
             (rich installed and supported tty), if True/False force the usage (or not).
-        formatter_kwargs: extra parameters for the formatter (can be a `HumanFormatter` or a `RichHumanFormatter`)
+        rich_formatter: Formatter to use if rich is available/selected (None => default RichHumanFormatter instance).
+        not_rich_formatter: Formatter to use if rich is not available/selected (None => default HumanFormatter instance).
 
     """
     if "formatter" in kwargs:
         raise StlogError(
-            "you can't use formatter in kwargs for this function (buy you can use formatter_kwargs to tune it)"
+            "you can't use formatter in kwargs for this function (buy you can use rich_formatter/not_rich_formatter instead)"
         )
     _use_rich: bool = False
     if use_rich is not None:
         # manual mode
         _use_rich = use_rich
     else:
         # automatic mode
         if RICH_INSTALLED:
             c = Console(file=stream)
             _use_rich = c.is_terminal
     if _use_rich:
         return RichStreamOutput(
             stream=stream,
-            formatter=RichHumanFormatter(**(formatter_kwargs or {})),
+            formatter=rich_formatter or RichHumanFormatter(),
             **kwargs,
         )
     else:
         return StreamOutput(
             stream=stream,
-            formatter=HumanFormatter(**(formatter_kwargs or {})),
+            formatter=not_rich_formatter or HumanFormatter(),
             **kwargs,
         )
```

### Comparing `stlog-0.1.1/stlog/setup.py` & `stlog-0.1.2/stlog/setup.py`

 * *Files identical despite different names*

### Comparing `stlog-0.1.1/PKG-INFO` & `stlog-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stlog
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: MIT
 Author: Fabien MARTY
 Author-email: fabien.marty@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

