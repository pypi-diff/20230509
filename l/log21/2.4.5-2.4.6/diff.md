# Comparing `tmp/log21-2.4.5.tar.gz` & `tmp/log21-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log21-2.4.5.tar", last modified: Wed Apr 19 08:03:38 2023, max compression
+gzip compressed data, was "log21-2.4.6.tar", last modified: Tue May  9 19:18:45 2023, max compression
```

## Comparing `log21-2.4.5.tar` & `log21-2.4.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:03:38.226023 log21-2.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-04-19 08:03:28.000000 log21-2.4.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-04-19 08:03:38.226023 log21-2.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-04-19 08:03:28.000000 log21-2.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:03:38.226023 log21-2.4.5/log21/
--rw-r--r--   0 runner    (1001) docker     (123)    21618 2023-04-19 08:03:28.000000 log21-2.4.5/log21/Argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-19 08:03:28.000000 log21-2.4.5/log21/Colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:03:38.226023 log21-2.4.5/log21/CrashReporter/
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-19 08:03:28.000000 log21-2.4.5/log21/CrashReporter/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-04-19 08:03:28.000000 log21-2.4.5/log21/CrashReporter/Reporters.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-19 08:03:28.000000 log21-2.4.5/log21/CrashReporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-19 08:03:28.000000 log21-2.4.5/log21/FileHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-04-19 08:03:28.000000 log21-2.4.5/log21/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-19 08:03:28.000000 log21-2.4.5/log21/Levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-04-19 08:03:28.000000 log21-2.4.5/log21/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-04-19 08:03:28.000000 log21-2.4.5/log21/LoggingWindow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-19 08:03:28.000000 log21-2.4.5/log21/Manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    25534 2023-04-19 08:03:28.000000 log21-2.4.5/log21/PPrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-04-19 08:03:28.000000 log21-2.4.5/log21/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-19 08:03:28.000000 log21-2.4.5/log21/StreamHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-19 08:03:28.000000 log21-2.4.5/log21/TreePrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    20803 2023-04-19 08:03:28.000000 log21-2.4.5/log21/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:03:38.226023 log21-2.4.5/log21.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-04-19 08:03:38.000000 log21-2.4.5/log21.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-19 08:03:38.000000 log21-2.4.5/log21.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:03:38.000000 log21-2.4.5/log21.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 08:03:38.000000 log21-2.4.5/log21.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 08:03:38.000000 log21-2.4.5/log21.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 08:03:38.226023 log21-2.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-19 08:03:28.000000 log21-2.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:45.882230 log21-2.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-05-09 19:18:39.000000 log21-2.4.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-05-09 19:18:45.882230 log21-2.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-05-09 19:18:39.000000 log21-2.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:45.882230 log21-2.4.6/log21/
+-rw-r--r--   0 runner    (1001) docker     (123)    21618 2023-05-09 19:18:39.000000 log21-2.4.6/log21/Argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-05-09 19:18:39.000000 log21-2.4.6/log21/Colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:45.882230 log21-2.4.6/log21/CrashReporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-09 19:18:39.000000 log21-2.4.6/log21/CrashReporter/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-05-09 19:18:39.000000 log21-2.4.6/log21/CrashReporter/Reporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-09 19:18:39.000000 log21-2.4.6/log21/CrashReporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-09 19:18:39.000000 log21-2.4.6/log21/FileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-05-09 19:18:39.000000 log21-2.4.6/log21/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-09 19:18:39.000000 log21-2.4.6/log21/Levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-05-09 19:18:39.000000 log21-2.4.6/log21/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-05-09 19:18:39.000000 log21-2.4.6/log21/LoggingWindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-09 19:18:39.000000 log21-2.4.6/log21/Manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25534 2023-05-09 19:18:39.000000 log21-2.4.6/log21/PPrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-05-09 19:18:39.000000 log21-2.4.6/log21/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-09 19:18:39.000000 log21-2.4.6/log21/StreamHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-05-09 19:18:39.000000 log21-2.4.6/log21/TreePrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20658 2023-05-09 19:18:39.000000 log21-2.4.6/log21/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:45.882230 log21-2.4.6/log21.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-05-09 19:18:45.000000 log21-2.4.6/log21.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-09 19:18:45.000000 log21-2.4.6/log21.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:18:45.000000 log21-2.4.6/log21.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 19:18:45.000000 log21-2.4.6/log21.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 19:18:45.000000 log21-2.4.6/log21.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:18:45.882230 log21-2.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-09 19:18:39.000000 log21-2.4.6/setup.py
```

### Comparing `log21-2.4.5/LICENSE.txt` & `log21-2.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `log21-2.4.5/PKG-INFO` & `log21-2.4.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.4.5
+Version: 2.4.6
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Home-page: https://github.com/MPCodeWriter21/log21
 Author: CodeWriter21(Mehrad Pooryoussof)
 Author-email: <CodeWriter21@gmail.com>
 License: Apache-2.0 License
 Keywords: python,log,colorize,color,logging
 Classifier: Intended Audience :: Developers
@@ -69,17 +69,41 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.4.5
+### 2.4.6
 
-Added `no_color` parameter to ProgressBar.
+Shortened the usage syntax for the CrashReporters:
+
+```python
+import log21
+
+# Define a ConsoleReporter object
+console_reporter = log21.CrashReporter.ConsoleReporter()
+
+
+# This works with other `log21.CrashReporter.Reporter` subclasses as well.
+
+# Old syntax (still supported)
+@console_reporter.reporter
+def divide_old(a, b):
+    return a / b
+
+
+# New Syntax
+@console_reporter.reporter
+def divide_new(a, b):
+    return a / b
+
+```
+
+`console_crash_reporter` and `file_crash_reporter` are removed!
 
 [Full Changes Log](https://github.com/MPCodeWriter21/log21/blob/master/CHANGES-LOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.4.5/README.md` & `log21-2.4.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,41 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.4.5
+### 2.4.6
 
-Added `no_color` parameter to ProgressBar.
+Shortened the usage syntax for the CrashReporters:
+
+```python
+import log21
+
+# Define a ConsoleReporter object
+console_reporter = log21.CrashReporter.ConsoleReporter()
+
+
+# This works with other `log21.CrashReporter.Reporter` subclasses as well.
+
+# Old syntax (still supported)
+@console_reporter.reporter
+def divide_old(a, b):
+    return a / b
+
+
+# New Syntax
+@console_reporter.reporter
+def divide_new(a, b):
+    return a / b
+
+```
+
+`console_crash_reporter` and `file_crash_reporter` are removed!
 
 [Full Changes Log](https://github.com/MPCodeWriter21/log21/blob/master/CHANGES-LOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.4.5/log21/Argparse.py` & `log21-2.4.6/log21/Argparse.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.5/log21/Colors.py` & `log21-2.4.6/log21/Colors.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.5/log21/CrashReporter/Formatters.py` & `log21-2.4.6/log21/CrashReporter/Formatters.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.5/log21/CrashReporter/Reporters.py` & `log21-2.4.6/log21/CrashReporter/Reporters.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,14 +131,17 @@
         if self._exceptions_to_ignore is None:
             self._exceptions_to_ignore = set()
         if exception not in self._exceptions_to_ignore:
             self._exceptions_to_ignore.add(exception)
         else:
             raise ValueError('exception is already in the list of exceptions to ignore')
 
+    def __call__(self, func):
+        return self.reporter(func)
+
 
 class ConsoleReporter(Reporter):
     """
     ConsoleReporter is a Reporter that prints the exception to the console.
     Usage Example:
         >>>
         >>> # Define a ConsoleReporter object
@@ -259,15 +262,15 @@
     """
     EmailReporter is a Reporter that sends an email with the exception.
     Usage Example:
         >>>
         >>> # Define a EmailReporter object
         >>> email_reporter = EmailReporter(
         ...     mail_host='smtp.yandex.ru',
-        ...     mail_port=465,
+        ...     port=465,
         ...     from_address='MyEmail@yandex.ru',
         ...     to_address='CodeWriter21@gmail.com',
         ...     password='My$up3rStr0ngP@assw0rd XD'
         ... )
         ...
         >>> # Define the function you want to wrap
         >>> @email_reporter.reporter
```

### Comparing `log21-2.4.5/log21/FileHandler.py` & `log21-2.4.6/log21/FileHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.5/log21/Formatters.py` & `log21-2.4.6/log21/Formatters.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.5/log21/Logger.py` & `log21-2.4.6/log21/Logger.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.5/log21/LoggingWindow.py` & `log21-2.4.6/log21/LoggingWindow.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.5/log21/Manager.py` & `log21-2.4.6/log21/Manager.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.5/log21/PPrint.py` & `log21-2.4.6/log21/PPrint.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.5/log21/ProgressBar.py` & `log21-2.4.6/log21/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.5/log21/StreamHandler.py` & `log21-2.4.6/log21/StreamHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.5/log21/TreePrint.py` & `log21-2.4.6/log21/TreePrint.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.5/log21/__init__.py` & `log21-2.4.6/log21/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,25 +18,25 @@
 from log21.Argparse import ColorizingArgumentParser
 from log21.FileHandler import DecolorizingFileHandler
 from log21.LoggingWindow import LoggingWindow, LoggingWindowHandler
 from log21.StreamHandler import ColorizingStreamHandler, StreamHandler
 from log21.Formatters import ColorizingFormatter, DecolorizingFormatter
 from log21.Colors import Colors, get_color, get_colors, ansi_escape, get_color_name, closest_color
 
-__version__ = "2.4.5"
+__version__ = "2.4.6"
 __author__ = "CodeWriter21 (Mehrad Pooryoussof)"
 __github__ = "Https://GitHub.com/MPCodeWriter21/log21"
 __all__ = ['ColorizingStreamHandler', 'DecolorizingFileHandler', 'ColorizingFormatter', 'DecolorizingFormatter',
            'get_logger', 'Logger', 'Colors', 'get_color', 'get_colors', 'CRITICAL', 'FATAL', 'ERROR', 'WARNING', 'WARN',
            'INFO', 'DEBUG', 'NOTSET', 'StreamHandler', 'ColorizingArgumentParser', 'PrettyPrinter', 'pformat',
            'pprint', 'pretty_print', 'tree_format', 'TreePrint', 'Manager', 'get_color_name', 'closest_color',
            'ansi_escape', '__version__', '__author__', '__github__', 'debug', 'info', 'warning', 'warn', 'error',
            'critical', 'fatal', 'exception', 'log', 'basic_config', 'basicConfig', 'ProgressBar', 'progress_bar',
-           'LoggingWindow', 'LoggingWindowHandler', 'get_logging_window', 'CrashReporter', 'console_crash_reporter',
-           'file_crash_reporter', 'console_reporter', 'file_reporter']
+           'LoggingWindow', 'LoggingWindowHandler', 'get_logging_window', 'CrashReporter', 'console_reporter',
+           'file_reporter']
 
 _manager = Manager()
 _logging.setLoggerClass(Logger)
 
 
 def _prepare_formatter(fmt: str = None, style: str = '%', datefmt: str = "%H:%M:%S", show_level: bool = True,
                        show_time: bool = True, colorize_time_and_level: bool = True,
@@ -451,11 +451,9 @@
 
     bar = ProgressBar(width=width, prefix=prefix, suffix=suffix, show_percentage=show_percentage)
 
     print(bar.get_bar(progress, total))
 
 
 console_reporter = CrashReporter.ConsoleReporter()
-console_crash_reporter = console_reporter.reporter
 
 file_reporter = CrashReporter.FileReporter(file='crash_report.log')
-file_crash_reporter = file_reporter.reporter
```

### Comparing `log21-2.4.5/log21.egg-info/PKG-INFO` & `log21-2.4.6/log21.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.4.5
+Version: 2.4.6
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Home-page: https://github.com/MPCodeWriter21/log21
 Author: CodeWriter21(Mehrad Pooryoussof)
 Author-email: <CodeWriter21@gmail.com>
 License: Apache-2.0 License
 Keywords: python,log,colorize,color,logging
 Classifier: Intended Audience :: Developers
@@ -69,17 +69,41 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.4.5
+### 2.4.6
 
-Added `no_color` parameter to ProgressBar.
+Shortened the usage syntax for the CrashReporters:
+
+```python
+import log21
+
+# Define a ConsoleReporter object
+console_reporter = log21.CrashReporter.ConsoleReporter()
+
+
+# This works with other `log21.CrashReporter.Reporter` subclasses as well.
+
+# Old syntax (still supported)
+@console_reporter.reporter
+def divide_old(a, b):
+    return a / b
+
+
+# New Syntax
+@console_reporter.reporter
+def divide_new(a, b):
+    return a / b
+
+```
+
+`console_crash_reporter` and `file_crash_reporter` are removed!
 
 [Full Changes Log](https://github.com/MPCodeWriter21/log21/blob/master/CHANGES-LOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.4.5/log21.egg-info/SOURCES.txt` & `log21-2.4.6/log21.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `log21-2.4.5/setup.py` & `log21-2.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 DESCRIPTION = 'A simple logging package that helps you log colorized messages in Windows console.'
-VERSION = '2.4.5'
+VERSION = '2.4.6'
 
 setup(
     name='log21',
     version=VERSION,
     url='https://github.com/MPCodeWriter21/log21',
     author='CodeWriter21(Mehrad Pooryoussof)',
     author_email='<CodeWriter21@gmail.com>',
```

