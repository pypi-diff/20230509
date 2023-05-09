# Comparing `tmp/cli3-1.1.0.tar.gz` & `tmp/cli3-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli3-1.1.0.tar", last modified: Wed May  3 00:29:46 2023, max compression
+gzip compressed data, was "cli3-1.1.1.tar", last modified: Tue May  9 00:54:21 2023, max compression
```

## Comparing `cli3-1.1.0.tar` & `cli3-1.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-03 00:29:46.302776 cli3-1.1.0/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1064 2020-10-21 03:10:04.000000 cli3-1.1.0/LICENSE
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1537 2023-05-03 00:29:46.302776 cli3-1.1.0/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1038 2022-11-16 03:06:40.000000 cli3-1.1.0/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-03 00:29:46.302776 cli3-1.1.0/cli/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1343 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    13785 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/abc.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     6825 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/app.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     4274 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/argument.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     7041 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/command.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     4501 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/flag.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     4997 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/help.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     7434 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/parser.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-03 00:29:46.302776 cli3-1.1.0/cli/tests/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      111 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/tests/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     5816 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/tests/app.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-03 00:29:46.302776 cli3-1.1.0/cli/tests/content/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      145 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/tests/content/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2599 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/tests/content/v1.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2002 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/tests/content/v2.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    13997 2023-05-03 00:28:41.000000 cli3-1.1.0/cli/wraps.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-03 00:29:46.302776 cli3-1.1.0/cli3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1537 2023-05-03 00:29:46.000000 cli3-1.1.0/cli3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      402 2023-05-03 00:29:46.000000 cli3-1.1.0/cli3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-05-03 00:29:46.000000 cli3-1.1.0/cli3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        7 2023-05-03 00:29:46.000000 cli3-1.1.0/cli3.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        4 2023-05-03 00:29:46.000000 cli3-1.1.0/cli3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-05-03 00:29:46.302776 cli3-1.1.0/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      762 2023-05-03 00:28:52.000000 cli3-1.1.0/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-09 00:54:21.476932 cli3-1.1.1/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1064 2020-10-21 03:10:04.000000 cli3-1.1.1/LICENSE
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1537 2023-05-09 00:54:21.476932 cli3-1.1.1/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1038 2022-11-16 03:06:40.000000 cli3-1.1.1/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-09 00:54:21.472932 cli3-1.1.1/cli/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1343 2023-05-03 02:43:51.000000 cli3-1.1.1/cli/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    13785 2023-05-03 02:43:51.000000 cli3-1.1.1/cli/abc.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     6825 2023-05-03 02:43:51.000000 cli3-1.1.1/cli/app.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4660 2023-05-09 00:41:40.000000 cli3-1.1.1/cli/argument.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     7041 2023-05-09 00:53:27.000000 cli3-1.1.1/cli/command.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4501 2023-05-03 02:43:51.000000 cli3-1.1.1/cli/flag.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4997 2023-05-03 02:43:51.000000 cli3-1.1.1/cli/help.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     7434 2023-05-03 02:43:51.000000 cli3-1.1.1/cli/parser.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-09 00:54:21.472932 cli3-1.1.1/cli/tests/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      111 2023-05-03 02:43:51.000000 cli3-1.1.1/cli/tests/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5816 2023-05-03 02:43:51.000000 cli3-1.1.1/cli/tests/app.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-09 00:54:21.476932 cli3-1.1.1/cli/tests/content/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      145 2023-05-03 02:43:51.000000 cli3-1.1.1/cli/tests/content/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2599 2023-05-03 02:43:51.000000 cli3-1.1.1/cli/tests/content/v1.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2002 2023-05-03 02:43:51.000000 cli3-1.1.1/cli/tests/content/v2.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    14056 2023-05-09 00:39:09.000000 cli3-1.1.1/cli/wraps.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-09 00:54:21.476932 cli3-1.1.1/cli3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1537 2023-05-09 00:54:21.000000 cli3-1.1.1/cli3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      402 2023-05-09 00:54:21.000000 cli3-1.1.1/cli3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-05-09 00:54:21.000000 cli3-1.1.1/cli3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        7 2023-05-09 00:54:21.000000 cli3-1.1.1/cli3.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        4 2023-05-09 00:54:21.000000 cli3-1.1.1/cli3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-05-09 00:54:21.476932 cli3-1.1.1/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      762 2023-05-09 00:53:59.000000 cli3-1.1.1/setup.py
```

### Comparing `cli3-1.1.0/LICENSE` & `cli3-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cli3-1.1.0/PKG-INFO` & `cli3-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli3
-Version: 1.1.0
+Version: 1.1.1
 Summary: A highly configurable, dynamic, fast, and easy solution to managing a command-line application.
 Home-page: https://github.com/imgurbot12/cli
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cli3-1.1.0/README.md` & `cli3-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cli3-1.1.0/cli/__init__.py` & `cli3-1.1.1/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.0/cli/abc.py` & `cli3-1.1.1/cli/abc.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.0/cli/app.py` & `cli3-1.1.1/cli/app.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.0/cli/argument.py` & `cli3-1.1.1/cli/argument.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
     'parse_bool',
     'parse_decimal',
     'parse_duration',
     'parse_new_file',
     'parse_existing_file',
     'parse_list_function',
+    'parse_bytes_function',
 
     'range_args',
     'exact_args',
     'no_args',
 ]
 
 #: regex parser for duration string
@@ -112,14 +113,25 @@
 
     :param typefunc: type-function to convert string into new value
     :param origin:   type to convert list into (set, list, tuple)
     :return:         function to parse a list into a list of a specified type
     """
     return lambda l: origin([typefunc(v) for v in l.split(',')])
 
+def parse_bytes_function(origin: Union[Type[bytes], Type[bytearray]]) -> TypeFunc:
+    """
+    generate bytes parser for the following type
+
+    :param origin: type to convert into
+    :return:       function to parse string into bytes/bytearray
+    """
+    if origin == bytes:
+        return lambda s: s.encode()
+    return lambda s: bytearray(s.encode())
+
 def range_args(min: int = 0, max: Optional[int] = None) -> Callable:
     """
     generate before action function to validate the number of arguments
 
     :param min: minimum number of arguments
     :param max: maximum number of arguments
     :return:    function used to regulate argument numbers
```

### Comparing `cli3-1.1.0/cli/command.py` & `cli3-1.1.1/cli/command.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.0/cli/flag.py` & `cli3-1.1.1/cli/flag.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.0/cli/help.py` & `cli3-1.1.1/cli/help.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.0/cli/parser.py` & `cli3-1.1.1/cli/parser.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.0/cli/tests/app.py` & `cli3-1.1.1/cli/tests/app.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.0/cli/tests/content/v1.py` & `cli3-1.1.1/cli/tests/content/v1.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.0/cli/tests/content/v2.py` & `cli3-1.1.1/cli/tests/content/v2.py`

 * *Files identical despite different names*

### Comparing `cli3-1.1.0/cli/wraps.py` & `cli3-1.1.1/cli/wraps.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,16 +79,18 @@
     :param depth: recursion depth of function (used for debug)
     :return:      compiled typefunction
     """
     # ignore special variables like `Context`
     if hint in (Context, ):
         return
     # parse basic typehints
-    if hint in (str, bytes, bytearray, int, float):
+    if hint in (str, int, float):
         return hint
+    if hint in (bytes, bytearray):
+        return parse_bytes_function(hint)
     if hint in (set, list, tuple):
         return parse_list_function(str, hint)
     if hint == bool:
         return parse_bool
     if hint == Decimal:
         return parse_decimal
     if hint in (Duration, timedelta):
```

### Comparing `cli3-1.1.0/cli3.egg-info/PKG-INFO` & `cli3-1.1.1/cli3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli3
-Version: 1.1.0
+Version: 1.1.1
 Summary: A highly configurable, dynamic, fast, and easy solution to managing a command-line application.
 Home-page: https://github.com/imgurbot12/cli
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cli3-1.1.0/setup.py` & `cli3-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='cli3',
-    version='1.1.0',
+    version='1.1.1',
     license='MIT',
     packages=find_packages(),
     url='https://github.com/imgurbot12/cli',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     description=(
         'A highly configurable, dynamic, fast, and easy '
```

