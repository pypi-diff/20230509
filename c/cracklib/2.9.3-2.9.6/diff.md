# Comparing `tmp/cracklib-2.9.3.tar.gz` & `tmp/cracklib-2.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cracklib-2.9.3.tar", last modified: Sun Apr 12 20:32:32 2015, max compression
+gzip compressed data, was "cracklib-2.9.6.tar", last modified: Tue May  9 15:50:23 2023, max compression
```

## Comparing `cracklib-2.9.3.tar` & `cracklib-2.9.6.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2015-04-12 20:32:32.000000 cracklib-2.9.3/
--rw-r--r--   0 jan       (1000) jan       (1000)     4782 2015-04-12 20:15:24.000000 cracklib-2.9.3/test_cracklib.py
--rw-r--r--   0 jan       (1000) jan       (1000)     2104 2015-04-12 20:15:24.000000 cracklib-2.9.3/setup.py.in
--rw-r--r--   0 jan       (1000) jan       (1000)     2064 2015-04-12 20:16:07.000000 cracklib-2.9.3/setup.py
--rw-r--r--   0 jan       (1000) jan       (1000)       97 2015-04-12 20:32:32.000000 cracklib-2.9.3/setup.cfg
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2015-04-12 20:32:32.000000 cracklib-2.9.3/cracklib.egg-info/
--rw-r--r--   0 jan       (1000) jan       (1000)        1 2015-04-12 20:32:32.000000 cracklib-2.9.3/cracklib.egg-info/dependency_links.txt
--rw-r--r--   0 jan       (1000) jan       (1000)       33 2015-04-12 20:32:32.000000 cracklib-2.9.3/cracklib.egg-info/top_level.txt
--rw-r--r--   0 jan       (1000) jan       (1000)      289 2015-04-12 20:32:32.000000 cracklib-2.9.3/cracklib.egg-info/SOURCES.txt
--rw-r--r--   0 jan       (1000) jan       (1000)      874 2015-04-12 20:32:32.000000 cracklib-2.9.3/cracklib.egg-info/PKG-INFO
--rw-r--r--   0 jan       (1000) jan       (1000)        1 2015-04-12 20:17:07.000000 cracklib-2.9.3/cracklib.egg-info/not-zip-safe
--rw-r--r--   0 jan       (1000) jan       (1000)     5496 2015-04-12 20:15:24.000000 cracklib-2.9.3/_cracklib.c
--rw-r--r--   0 jan       (1000) jan       (1000)      874 2015-04-12 20:32:32.000000 cracklib-2.9.3/PKG-INFO
--rw-r--r--   0 jan       (1000) jan       (1000)      334 2015-04-12 20:15:24.000000 cracklib-2.9.3/Makefile.am
--rw-r--r--   0 jan       (1000) jan       (1000)     5922 2015-04-12 20:15:24.000000 cracklib-2.9.3/cracklib.py
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2023-05-09 15:50:23.711738 cracklib-2.9.6/
+-rw-r--r--   0 jan       (1000) jan       (1000)      819 2023-05-09 15:50:23.711738 cracklib-2.9.6/PKG-INFO
+-rw-r--r--   0 jan       (1000) jan       (1000)     5496 2016-06-18 16:56:26.000000 cracklib-2.9.6/_cracklib.c
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2023-05-09 15:50:23.711738 cracklib-2.9.6/cracklib.egg-info/
+-rw-r--r--   0 jan       (1000) jan       (1000)      819 2023-05-09 15:50:23.000000 cracklib-2.9.6/cracklib.egg-info/PKG-INFO
+-rw-r--r--   0 jan       (1000) jan       (1000)      224 2023-05-09 15:50:23.000000 cracklib-2.9.6/cracklib.egg-info/SOURCES.txt
+-rw-r--r--   0 jan       (1000) jan       (1000)        1 2023-05-09 15:50:23.000000 cracklib-2.9.6/cracklib.egg-info/dependency_links.txt
+-rw-r--r--   0 jan       (1000) jan       (1000)        1 2023-05-09 15:46:44.000000 cracklib-2.9.6/cracklib.egg-info/not-zip-safe
+-rw-r--r--   0 jan       (1000) jan       (1000)       33 2023-05-09 15:50:23.000000 cracklib-2.9.6/cracklib.egg-info/top_level.txt
+-rw-r--r--   0 jan       (1000) jan       (1000)     5922 2023-05-09 15:43:09.000000 cracklib-2.9.6/cracklib.py
+-rw-r--r--   0 jan       (1000) jan       (1000)      102 2023-05-09 15:50:23.715738 cracklib-2.9.6/setup.cfg
+-rw-r--r--   0 jan       (1000) jan       (1000)     2064 2023-05-09 15:46:01.000000 cracklib-2.9.6/setup.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     4782 2016-06-18 16:56:26.000000 cracklib-2.9.6/test_cracklib.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cracklib-2.9.3/test_cracklib.py` & `cracklib-2.9.6/test_cracklib.py`

 * *Files identical despite different names*

### Comparing `cracklib-2.9.3/setup.py.in` & `cracklib-2.9.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,35 +19,35 @@
 
 import os, sys
 
 from setuptools import setup, Extension, find_packages
 
 extensions = [
     Extension("_cracklib",
-        ["@srcdir@/_cracklib.c"],
-        include_dirs = ["@top_srcdir@/lib"],
+        ["./_cracklib.c"],
+        include_dirs = ["../lib"],
         libraries = ["crack"],
-        library_dirs = ["@top_builddir@/lib/.libs"]),
+        library_dirs = ["../lib/.libs"]),
 ]
 
 setup(
     name="cracklib",
-    version="@VERSION@",
+    version="2.9.6",
     description="A CPython extension module wrapping the libcrack library",
     long_description="""\
 This CPython extension provides Python bindings for cracklib. It
 contains a pythonic interface to cracklib's functions and some Python
 convenience functions.
 """,
     author="Jan Dittberner",
     author_email="jan@dittberner.info",
     url="http://cracklib.sourceforge.net/",
     license="GPLv2+",
     py_modules=['cracklib', 'test_cracklib'],
-    package_dir={'': '@srcdir@'},
+    package_dir={'': '.'},
     ext_modules=extensions,
     zip_safe=False,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)",
         "Operating System :: OS Independent",
```

### Comparing `cracklib-2.9.3/cracklib.egg-info/PKG-INFO` & `cracklib-2.9.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cracklib
-Version: 2.9.3
+Version: 2.9.6
 Summary: A CPython extension module wrapping the libcrack library
 Home-page: http://cracklib.sourceforge.net/
 Author: Jan Dittberner
 Author-email: jan@dittberner.info
 License: GPLv2+
-Description: This CPython extension provides Python bindings for cracklib. It
-        contains a pythonic interface to cracklib's functions and some Python
-        convenience functions.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Systems Administration
+
+This CPython extension provides Python bindings for cracklib. It
+contains a pythonic interface to cracklib's functions and some Python
+convenience functions.
```

### Comparing `cracklib-2.9.3/_cracklib.c` & `cracklib-2.9.6/_cracklib.c`

 * *Files identical despite different names*

### Comparing `cracklib-2.9.3/PKG-INFO` & `cracklib-2.9.6/cracklib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cracklib
-Version: 2.9.3
+Version: 2.9.6
 Summary: A CPython extension module wrapping the libcrack library
 Home-page: http://cracklib.sourceforge.net/
 Author: Jan Dittberner
 Author-email: jan@dittberner.info
 License: GPLv2+
-Description: This CPython extension provides Python bindings for cracklib. It
-        contains a pythonic interface to cracklib's functions and some Python
-        convenience functions.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Systems Administration
+
+This CPython extension provides Python bindings for cracklib. It
+contains a pythonic interface to cracklib's functions and some Python
+convenience functions.
```

### Comparing `cracklib-2.9.3/cracklib.py` & `cracklib-2.9.6/cracklib.py`

 * *Files identical despite different names*

