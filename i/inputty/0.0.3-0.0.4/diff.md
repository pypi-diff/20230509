# Comparing `tmp/inputty-0.0.3.tar.gz` & `tmp/inputty-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inputty-0.0.3.tar", last modified: Tue May  9 15:11:15 2023, max compression
+gzip compressed data, was "inputty-0.0.4.tar", last modified: Tue May  9 16:07:03 2023, max compression
```

## Comparing `inputty-0.0.3.tar` & `inputty-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-09 15:11:15.026111 inputty-0.0.3/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 inputty-0.0.3/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)      738 2023-05-09 15:11:15.026111 inputty-0.0.3/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)       96 2023-05-09 13:23:03.000000 inputty-0.0.3/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-09 15:11:15.026111 inputty-0.0.3/inputty/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      124 2023-05-09 13:45:56.000000 inputty-0.0.3/inputty/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-09 15:10:13.000000 inputty-0.0.3/inputty/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-09 15:11:15.026111 inputty-0.0.3/inputty/src/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 inputty-0.0.3/inputty/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     6493 2023-05-09 15:10:06.000000 inputty-0.0.3/inputty/src/input.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-09 15:11:15.026111 inputty-0.0.3/inputty.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      738 2023-05-09 15:11:14.000000 inputty-0.0.3/inputty.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      249 2023-05-09 15:11:14.000000 inputty-0.0.3/inputty.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-09 15:11:14.000000 inputty-0.0.3/inputty.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        8 2023-05-09 15:11:14.000000 inputty-0.0.3/inputty.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-09 15:11:15.026111 inputty-0.0.3/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1157 2023-05-09 13:25:02.000000 inputty-0.0.3/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-09 16:07:03.891454 inputty-0.0.4/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 inputty-0.0.4/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      825 2023-05-09 16:07:03.891454 inputty-0.0.4/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)       96 2023-05-09 13:23:03.000000 inputty-0.0.4/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-09 16:07:03.888121 inputty-0.0.4/inputty/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      124 2023-05-09 13:45:56.000000 inputty-0.0.4/inputty/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-09 16:05:13.000000 inputty-0.0.4/inputty/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-09 16:07:03.891454 inputty-0.0.4/inputty/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 inputty-0.0.4/inputty/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     6491 2023-05-09 16:05:05.000000 inputty-0.0.4/inputty/src/input.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-09 16:07:03.891454 inputty-0.0.4/inputty.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      825 2023-05-09 16:07:03.000000 inputty-0.0.4/inputty.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      249 2023-05-09 16:07:03.000000 inputty-0.0.4/inputty.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-09 16:07:03.000000 inputty-0.0.4/inputty.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        8 2023-05-09 16:07:03.000000 inputty-0.0.4/inputty.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-09 16:07:03.891454 inputty-0.0.4/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1157 2023-05-09 13:25:02.000000 inputty-0.0.4/setup.py
```

### Comparing `inputty-0.0.3/LICENSE.txt` & `inputty-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inputty-0.0.3/PKG-INFO` & `inputty-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inputty
-Version: 0.0.3
+Version: 0.0.4
 Summary: """A collection of modules that supports cCLI inputs."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: cli,input
@@ -20,14 +20,20 @@
 ```bash
 pip install inputty
 ```
 
 
 # Version History
 
+Version 0.0.4 9 May 2023
+
+1. Fix integer index bug (in _get_valid_input_list)
+
+------
+
 Version 0.0.3 9 May 2023
 
 1. Fix <RTN> and remove self.allow_null
 
 ------
 
 Version 0.0.2 9 May 2023
```

### Comparing `inputty-0.0.3/inputty/src/input.py` & `inputty-0.0.4/inputty/src/input.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         for key in self.processes:
             processes = {}
             if key == INTEGER_SELECTION:
                 (min_, max_) = self.processes[key][2]
                 integer_range = range(min_, max_+1)
                 for index in integer_range:
                     valid_inputs.append(str(index))
-                    processes[str(index+1)] = (self.processes[key][0], [index])
+                    processes[str(index)] = (self.processes[key][0], [index])
                 self.processes = {**self.processes, **processes}
                 valid_list.append(f'an integer({min_}-{max_})')
             else:
                 valid_inputs.append(key)
                 valid_list.append(key)
         return (valid_inputs, valid_list)
```

### Comparing `inputty-0.0.3/inputty.egg-info/PKG-INFO` & `inputty-0.0.4/inputty.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inputty
-Version: 0.0.3
+Version: 0.0.4
 Summary: """A collection of modules that supports cCLI inputs."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: cli,input
@@ -20,14 +20,20 @@
 ```bash
 pip install inputty
 ```
 
 
 # Version History
 
+Version 0.0.4 9 May 2023
+
+1. Fix integer index bug (in _get_valid_input_list)
+
+------
+
 Version 0.0.3 9 May 2023
 
 1. Fix <RTN> and remove self.allow_null
 
 ------
 
 Version 0.0.2 9 May 2023
```

### Comparing `inputty-0.0.3/setup.py` & `inputty-0.0.4/setup.py`

 * *Files identical despite different names*

