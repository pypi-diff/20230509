# Comparing `tmp/calcutils-0.1.3.tar.gz` & `tmp/calcutils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Python\calcutils\dist\.tmp-52dgkw2o\calcutils-0.1.3.tar", last modified: Tue May  9 05:31:14 2023, max compression
+gzip compressed data, was "D:\Python\calcutils\dist\.tmp-fnwp_b1g\calcutils-0.1.4.tar", last modified: Tue May  9 06:12:33 2023, max compression
```

## Comparing `calcutils-0.1.3.tar` & `calcutils-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 05:31:14.000000 calcutils-0.1.3/
--rw-rw-rw-   0        0        0       11 2023-05-08 09:36:20.000000 calcutils-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      584 2023-05-09 05:31:14.000000 calcutils-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0        8 2023-05-08 07:30:00.000000 calcutils-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 05:31:14.000000 calcutils-0.1.3/calcutils/
--rw-rw-rw-   0        0        0     1098 2023-05-08 08:27:36.000000 calcutils-0.1.3/calcutils/calcu.p
--rw-rw-rw-   0        0        0    24574 2023-05-09 05:27:26.000000 calcutils-0.1.3/calcutils/calcus.py
--rw-rw-rw-   0        0        0     7827 2023-05-08 10:35:32.000000 calcutils-0.1.3/calcutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-09 05:31:14.000000 calcutils-0.1.3/calcutils.egg-info/
--rw-rw-rw-   0        0        0      584 2023-05-09 05:31:14.000000 calcutils-0.1.3/calcutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-05-09 05:31:14.000000 calcutils-0.1.3/calcutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 05:31:14.000000 calcutils-0.1.3/calcutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-09 05:31:14.000000 calcutils-0.1.3/calcutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      512 2023-05-09 05:30:38.000000 calcutils-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 05:31:14.000000 calcutils-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      489 2023-05-09 04:58:44.000000 calcutils-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 06:12:33.000000 calcutils-0.1.4/
+-rw-rw-rw-   0        0        0       11 2023-05-08 09:36:20.000000 calcutils-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      584 2023-05-09 06:12:33.000000 calcutils-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0        8 2023-05-08 07:30:00.000000 calcutils-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 06:12:33.000000 calcutils-0.1.4/calcutils/
+-rw-rw-rw-   0        0        0     1098 2023-05-08 08:27:36.000000 calcutils-0.1.4/calcutils/calcu.p
+-rw-rw-rw-   0        0        0    24591 2023-05-09 06:11:48.000000 calcutils-0.1.4/calcutils/calcus.py
+-rw-rw-rw-   0        0        0     7827 2023-05-08 10:35:32.000000 calcutils-0.1.4/calcutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 06:12:33.000000 calcutils-0.1.4/calcutils.egg-info/
+-rw-rw-rw-   0        0        0      584 2023-05-09 06:12:33.000000 calcutils-0.1.4/calcutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-05-09 06:12:33.000000 calcutils-0.1.4/calcutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 06:12:33.000000 calcutils-0.1.4/calcutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-09 06:12:33.000000 calcutils-0.1.4/calcutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      512 2023-05-09 06:11:48.000000 calcutils-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 06:12:33.000000 calcutils-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      489 2023-05-09 06:11:48.000000 calcutils-0.1.4/setup.py
```

### Comparing `calcutils-0.1.3/PKG-INFO` & `calcutils-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcutils
-Version: 0.1.3
+Version: 0.1.4
 Summary: A small calcu package
 Home-page: https://github.com/calcu_utils/calcu_utils
 Author: Lahani_Allen
 Author-email: Lahani_Allen <lahani_Allen@utc.com>
 Project-URL: Homepage, https://github.com/calcu_utils/calcu_utils
 Project-URL: Bug Tracker, https://github.com/calcu_utils/calcu_utils/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `calcutils-0.1.3/calcutils/calcu.p` & `calcutils-0.1.4/calcutils/calcu.p`

 * *Files identical despite different names*

### Comparing `calcutils-0.1.3/calcutils/calcus.py` & `calcutils-0.1.4/calcutils/calcus.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 __all__ = ['extract_stack', 'extract_tb', 'format_exception',
            'format_exception_only', 'format_list', 'format_stack',
            'format_tb', 'print_exc', 'format_exc', 'print_exception',
            'print_last', 'print_stack', 'print_tb', 'clear_frames',
            'FrameSummary', 'StackSummary', 'TracebackException',
            'walk_stack', 'walk_tb', 'calc']
 
-
 #
 # Formatting and printing lists of traceback lines.
 #
 
 def print_list(extracted_list, file=None):
     """Print the list of tuples as returned by extract_tb() or
     extract_stack() as a formatted stack trace to the given file."""
@@ -452,14 +451,15 @@
             )
         return result
 
 
 def calc(target=[], t=1):
     if t == 1:
         raise RuntimeError(info)
+    return target
 
 
 class TracebackException:
     """An exception ready for rendering.
 
     The traceback module captures enough attributes from the original exception
     to this intermediary form to ensure that no references are held, while
```

### Comparing `calcutils-0.1.3/calcutils/utils.py` & `calcutils-0.1.4/calcutils/utils.py`

 * *Files identical despite different names*

### Comparing `calcutils-0.1.3/calcutils.egg-info/PKG-INFO` & `calcutils-0.1.4/calcutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcutils
-Version: 0.1.3
+Version: 0.1.4
 Summary: A small calcu package
 Home-page: https://github.com/calcu_utils/calcu_utils
 Author: Lahani_Allen
 Author-email: Lahani_Allen <lahani_Allen@utc.com>
 Project-URL: Homepage, https://github.com/calcu_utils/calcu_utils
 Project-URL: Bug Tracker, https://github.com/calcu_utils/calcu_utils/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `calcutils-0.1.3/pyproject.toml` & `calcutils-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "calcutils"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Lahani_Allen", email="lahani_Allen@utc.com" },
 ]
 description = "A small calcu package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

