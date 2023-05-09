# Comparing `tmp/log21-2.4.6.tar.gz` & `tmp/log21-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log21-2.4.6.tar", last modified: Tue May  9 19:18:45 2023, max compression
+gzip compressed data, was "log21-2.4.7.tar", last modified: Tue May  9 19:44:45 2023, max compression
```

## Comparing `log21-2.4.6.tar` & `log21-2.4.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:45.882230 log21-2.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-05-09 19:18:39.000000 log21-2.4.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-05-09 19:18:45.882230 log21-2.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-05-09 19:18:39.000000 log21-2.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:45.882230 log21-2.4.6/log21/
--rw-r--r--   0 runner    (1001) docker     (123)    21618 2023-05-09 19:18:39.000000 log21-2.4.6/log21/Argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-05-09 19:18:39.000000 log21-2.4.6/log21/Colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:45.882230 log21-2.4.6/log21/CrashReporter/
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-09 19:18:39.000000 log21-2.4.6/log21/CrashReporter/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-05-09 19:18:39.000000 log21-2.4.6/log21/CrashReporter/Reporters.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-09 19:18:39.000000 log21-2.4.6/log21/CrashReporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-09 19:18:39.000000 log21-2.4.6/log21/FileHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-05-09 19:18:39.000000 log21-2.4.6/log21/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-09 19:18:39.000000 log21-2.4.6/log21/Levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-05-09 19:18:39.000000 log21-2.4.6/log21/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-05-09 19:18:39.000000 log21-2.4.6/log21/LoggingWindow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-09 19:18:39.000000 log21-2.4.6/log21/Manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    25534 2023-05-09 19:18:39.000000 log21-2.4.6/log21/PPrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-05-09 19:18:39.000000 log21-2.4.6/log21/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-09 19:18:39.000000 log21-2.4.6/log21/StreamHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-05-09 19:18:39.000000 log21-2.4.6/log21/TreePrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    20658 2023-05-09 19:18:39.000000 log21-2.4.6/log21/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:45.882230 log21-2.4.6/log21.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-05-09 19:18:45.000000 log21-2.4.6/log21.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-09 19:18:45.000000 log21-2.4.6/log21.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:18:45.000000 log21-2.4.6/log21.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 19:18:45.000000 log21-2.4.6/log21.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 19:18:45.000000 log21-2.4.6/log21.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:18:45.882230 log21-2.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-09 19:18:39.000000 log21-2.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:44:45.972288 log21-2.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-05-09 19:44:39.000000 log21-2.4.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-05-09 19:44:45.972288 log21-2.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-05-09 19:44:39.000000 log21-2.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:44:45.972288 log21-2.4.7/log21/
+-rw-r--r--   0 runner    (1001) docker     (123)    21618 2023-05-09 19:44:39.000000 log21-2.4.7/log21/Argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-05-09 19:44:39.000000 log21-2.4.7/log21/Colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:44:45.972288 log21-2.4.7/log21/CrashReporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-09 19:44:39.000000 log21-2.4.7/log21/CrashReporter/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-05-09 19:44:39.000000 log21-2.4.7/log21/CrashReporter/Reporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-09 19:44:39.000000 log21-2.4.7/log21/CrashReporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-09 19:44:39.000000 log21-2.4.7/log21/FileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-05-09 19:44:39.000000 log21-2.4.7/log21/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-09 19:44:39.000000 log21-2.4.7/log21/Levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-05-09 19:44:39.000000 log21-2.4.7/log21/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-05-09 19:44:39.000000 log21-2.4.7/log21/LoggingWindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-09 19:44:39.000000 log21-2.4.7/log21/Manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25534 2023-05-09 19:44:39.000000 log21-2.4.7/log21/PPrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-05-09 19:44:39.000000 log21-2.4.7/log21/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-09 19:44:39.000000 log21-2.4.7/log21/StreamHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-05-09 19:44:39.000000 log21-2.4.7/log21/TreePrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20658 2023-05-09 19:44:39.000000 log21-2.4.7/log21/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:44:45.972288 log21-2.4.7/log21.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-05-09 19:44:45.000000 log21-2.4.7/log21.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-09 19:44:45.000000 log21-2.4.7/log21.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:44:45.000000 log21-2.4.7/log21.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 19:44:45.000000 log21-2.4.7/log21.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 19:44:45.000000 log21-2.4.7/log21.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:44:45.972288 log21-2.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-09 19:44:39.000000 log21-2.4.7/setup.py
```

### Comparing `log21-2.4.6/LICENSE.txt` & `log21-2.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `log21-2.4.6/PKG-INFO` & `log21-2.4.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.4.6
+Version: 2.4.7
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Home-page: https://github.com/MPCodeWriter21/log21
 Author: CodeWriter21(Mehrad Pooryoussof)
 Author-email: <CodeWriter21@gmail.com>
 License: Apache-2.0 License
 Keywords: python,log,colorize,color,logging
 Classifier: Intended Audience :: Developers
@@ -69,41 +69,20 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.4.6
+### 2.4.7
 
-Shortened the usage syntax for the CrashReporters:
-
-```python
-import log21
-
-# Define a ConsoleReporter object
-console_reporter = log21.CrashReporter.ConsoleReporter()
-
-
-# This works with other `log21.CrashReporter.Reporter` subclasses as well.
-
-# Old syntax (still supported)
-@console_reporter.reporter
-def divide_old(a, b):
-    return a / b
-
-
-# New Syntax
-@console_reporter.reporter
-def divide_new(a, b):
-    return a / b
-
-```
-
-`console_crash_reporter` and `file_crash_reporter` are removed!
+Added `extra_values` argument to `CrashReporter.Formatter` which will let you pass extra static or dynamic values to the
+report formatter.
+They can be used in the format string. For dynamic values you can pass a function that takes no
+arguments as the value.
 
 [Full Changes Log](https://github.com/MPCodeWriter21/log21/blob/master/CHANGES-LOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.4.6/README.md` & `log21-2.4.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -49,41 +49,20 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.4.6
+### 2.4.7
 
-Shortened the usage syntax for the CrashReporters:
-
-```python
-import log21
-
-# Define a ConsoleReporter object
-console_reporter = log21.CrashReporter.ConsoleReporter()
-
-
-# This works with other `log21.CrashReporter.Reporter` subclasses as well.
-
-# Old syntax (still supported)
-@console_reporter.reporter
-def divide_old(a, b):
-    return a / b
-
-
-# New Syntax
-@console_reporter.reporter
-def divide_new(a, b):
-    return a / b
-
-```
-
-`console_crash_reporter` and `file_crash_reporter` are removed!
+Added `extra_values` argument to `CrashReporter.Formatter` which will let you pass extra static or dynamic values to the
+report formatter.
+They can be used in the format string. For dynamic values you can pass a function that takes no
+arguments as the value.
 
 [Full Changes Log](https://github.com/MPCodeWriter21/log21/blob/master/CHANGES-LOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.4.6/log21/Argparse.py` & `log21-2.4.7/log21/Argparse.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.6/log21/Colors.py` & `log21-2.4.7/log21/Colors.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.6/log21/CrashReporter/Formatters.py` & `log21-2.4.7/log21/CrashReporter/Formatters.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,65 @@
 # log21.CrashReporter.Formatters.py
 # CodeWriter21
 
 import traceback
 
 from datetime import datetime as _datetime
+from typing import Dict as _Dict, Union as _Union, Callable as _Callable, Any as _Any
 
 __all__ = ['Formatter', 'CONSOLE_REPORTER_FORMAT', 'FILE_REPORTER_FORMAT', 'EMAIL_REPORTER_FORMAT']
 
+RESERVED_KEYS = (
+    '__name__',
+    'type',
+    'message',
+    'traceback',
+    'name',
+    'file',
+    'lineno',
+    'function',
+    'asctime'
+)
+
 
 class Formatter:
-    def __init__(self, format_: str, style: str = '%', datefmt: str = '%Y-%m-%d %H:%M:%S'):
+    def __init__(self, format_: str, style: str = '%', datefmt: str = '%Y-%m-%d %H:%M:%S',
+                 extra_values: _Dict[str, _Union[str, _Callable, _Any]] = None):
         self._format = format_
 
         if style in ['%', '{']:
             self.__style = style
         else:
             raise ValueError('Invalid style: "' + str(style) + '" Valid styles: %, {')
 
         self.datefmt = datefmt
+        self.extra_values = dict()
+        if extra_values:
+            for key in extra_values:
+                if key in RESERVED_KEYS:
+                    raise ValueError(f'`{key}` is a reserved-key and cannot be used in `extra_values`.')
+                self.extra_values[key] = extra_values[key]
 
     def format(self, exception: BaseException):
         exception_dict = {
             '__name__': __name__,
             'type': type(exception),
             'message': exception.args[0],
             'traceback': traceback.format_tb(exception.__traceback__.tb_next),
             'name': exception.__class__.__name__,
             'file': exception.__traceback__.tb_next.tb_frame.f_code.co_filename,
             'lineno': exception.__traceback__.tb_next.tb_lineno,
             'function': exception.__traceback__.tb_next.tb_frame.f_code.co_name,
             'asctime': _datetime.now().strftime(self.datefmt),
         }
+        for key, value in self.extra_values.items():
+            if callable(value):
+                exception_dict[key] = value()
+            else:
+                exception_dict[key] = value
 
         if self.__style == '%':
             return self._format % exception_dict
         elif self.__style == '{':
             return self._format.format(**exception_dict)
         else:
             raise ValueError('Invalid style: "' + str(self.__style) + '" Valid styles: %, {')
```

### Comparing `log21-2.4.6/log21/CrashReporter/Reporters.py` & `log21-2.4.7/log21/CrashReporter/Reporters.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.6/log21/FileHandler.py` & `log21-2.4.7/log21/FileHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.6/log21/Formatters.py` & `log21-2.4.7/log21/Formatters.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.6/log21/Logger.py` & `log21-2.4.7/log21/Logger.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.6/log21/LoggingWindow.py` & `log21-2.4.7/log21/LoggingWindow.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.6/log21/Manager.py` & `log21-2.4.7/log21/Manager.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.6/log21/PPrint.py` & `log21-2.4.7/log21/PPrint.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.6/log21/ProgressBar.py` & `log21-2.4.7/log21/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.6/log21/StreamHandler.py` & `log21-2.4.7/log21/StreamHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.6/log21/TreePrint.py` & `log21-2.4.7/log21/TreePrint.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.6/log21/__init__.py` & `log21-2.4.7/log21/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from log21.Argparse import ColorizingArgumentParser
 from log21.FileHandler import DecolorizingFileHandler
 from log21.LoggingWindow import LoggingWindow, LoggingWindowHandler
 from log21.StreamHandler import ColorizingStreamHandler, StreamHandler
 from log21.Formatters import ColorizingFormatter, DecolorizingFormatter
 from log21.Colors import Colors, get_color, get_colors, ansi_escape, get_color_name, closest_color
 
-__version__ = "2.4.6"
+__version__ = "2.4.7"
 __author__ = "CodeWriter21 (Mehrad Pooryoussof)"
 __github__ = "Https://GitHub.com/MPCodeWriter21/log21"
 __all__ = ['ColorizingStreamHandler', 'DecolorizingFileHandler', 'ColorizingFormatter', 'DecolorizingFormatter',
            'get_logger', 'Logger', 'Colors', 'get_color', 'get_colors', 'CRITICAL', 'FATAL', 'ERROR', 'WARNING', 'WARN',
            'INFO', 'DEBUG', 'NOTSET', 'StreamHandler', 'ColorizingArgumentParser', 'PrettyPrinter', 'pformat',
            'pprint', 'pretty_print', 'tree_format', 'TreePrint', 'Manager', 'get_color_name', 'closest_color',
            'ansi_escape', '__version__', '__author__', '__github__', 'debug', 'info', 'warning', 'warn', 'error',
```

### Comparing `log21-2.4.6/log21.egg-info/PKG-INFO` & `log21-2.4.7/log21.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.4.6
+Version: 2.4.7
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Home-page: https://github.com/MPCodeWriter21/log21
 Author: CodeWriter21(Mehrad Pooryoussof)
 Author-email: <CodeWriter21@gmail.com>
 License: Apache-2.0 License
 Keywords: python,log,colorize,color,logging
 Classifier: Intended Audience :: Developers
@@ -69,41 +69,20 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.4.6
+### 2.4.7
 
-Shortened the usage syntax for the CrashReporters:
-
-```python
-import log21
-
-# Define a ConsoleReporter object
-console_reporter = log21.CrashReporter.ConsoleReporter()
-
-
-# This works with other `log21.CrashReporter.Reporter` subclasses as well.
-
-# Old syntax (still supported)
-@console_reporter.reporter
-def divide_old(a, b):
-    return a / b
-
-
-# New Syntax
-@console_reporter.reporter
-def divide_new(a, b):
-    return a / b
-
-```
-
-`console_crash_reporter` and `file_crash_reporter` are removed!
+Added `extra_values` argument to `CrashReporter.Formatter` which will let you pass extra static or dynamic values to the
+report formatter.
+They can be used in the format string. For dynamic values you can pass a function that takes no
+arguments as the value.
 
 [Full Changes Log](https://github.com/MPCodeWriter21/log21/blob/master/CHANGES-LOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.4.6/log21.egg-info/SOURCES.txt` & `log21-2.4.7/log21.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `log21-2.4.6/setup.py` & `log21-2.4.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 DESCRIPTION = 'A simple logging package that helps you log colorized messages in Windows console.'
-VERSION = '2.4.6'
+VERSION = '2.4.7'
 
 setup(
     name='log21',
     version=VERSION,
     url='https://github.com/MPCodeWriter21/log21',
     author='CodeWriter21(Mehrad Pooryoussof)',
     author_email='<CodeWriter21@gmail.com>',
```

