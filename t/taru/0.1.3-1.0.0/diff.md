# Comparing `tmp/taru-0.1.3.tar.gz` & `tmp/taru-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/taru-0.1.3.tar", last modified: Sun Jul 25 21:31:44 2021, max compression
+gzip compressed data, was "taru-1.0.0.tar", last modified: Tue May  9 07:41:29 2023, max compression
```

## Comparing `taru-0.1.3.tar` & `taru-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 dds      (197609) None     (197121)        0 2021-07-25 21:31:44.166774 taru-0.1.3/
--rw-r--r--   0 dds      (197609) None     (197121)     1058 2021-07-25 21:31:44.166774 taru-0.1.3/PKG-INFO
--rw-r--r--   0 dds      (197609) None     (197121)     1159 2021-07-25 21:26:10.000000 taru-0.1.3/README.md
--rw-r--r--   0 dds      (197609) None     (197121)       61 2021-07-25 21:31:44.167772 taru-0.1.3/setup.cfg
--rw-r--r--   0 dds      (197609) None     (197121)     1810 2021-07-25 21:30:00.000000 taru-0.1.3/setup.py
-drwxr-xr-x   0 dds      (197609) None     (197121)        0 2021-07-25 21:31:44.154806 taru-0.1.3/taru/
--rw-r--r--   0 dds      (197609) None     (197121)        0 2021-07-25 10:53:05.000000 taru-0.1.3/taru/__init__.py
--rwxr-xr-x   0 dds      (197609) None     (197121)     5092 2021-07-25 21:22:50.000000 taru-0.1.3/taru/cli.py
-drwxr-xr-x   0 dds      (197609) None     (197121)        0 2021-07-25 21:31:44.165777 taru-0.1.3/taru.egg-info/
--rw-r--r--   0 dds      (197609) None     (197121)     1058 2021-07-25 21:31:43.000000 taru-0.1.3/taru.egg-info/PKG-INFO
--rw-r--r--   0 dds      (197609) None     (197121)      227 2021-07-25 21:31:43.000000 taru-0.1.3/taru.egg-info/SOURCES.txt
--rw-r--r--   0 dds      (197609) None     (197121)        1 2021-07-25 21:31:43.000000 taru-0.1.3/taru.egg-info/dependency_links.txt
--rw-r--r--   0 dds      (197609) None     (197121)       40 2021-07-25 21:31:43.000000 taru-0.1.3/taru.egg-info/entry_points.txt
--rw-r--r--   0 dds      (197609) None     (197121)        1 2021-07-25 11:11:54.000000 taru-0.1.3/taru.egg-info/not-zip-safe
--rw-r--r--   0 dds      (197609) None     (197121)        5 2021-07-25 21:31:43.000000 taru-0.1.3/taru.egg-info/top_level.txt
+drwxr-xr-x   0 dds      (197609) None     (197121)        0 2023-05-09 07:41:29.291928 taru-1.0.0/
+-rw-r--r--   0 dds      (197609) None     (197121)     1069 2023-05-09 07:41:29.291928 taru-1.0.0/PKG-INFO
+-rw-r--r--   0 dds      (197609) None     (197121)     1159 2021-07-25 21:26:10.000000 taru-1.0.0/README.md
+-rw-r--r--   0 dds      (197609) None     (197121)       61 2023-05-09 07:41:29.292899 taru-1.0.0/setup.cfg
+-rw-r--r--   0 dds      (197609) None     (197121)     1810 2023-05-09 07:35:13.000000 taru-1.0.0/setup.py
+drwxr-xr-x   0 dds      (197609) None     (197121)        0 2023-05-09 07:41:29.274988 taru-1.0.0/taru/
+-rw-r--r--   0 dds      (197609) None     (197121)        0 2021-07-25 10:53:05.000000 taru-1.0.0/taru/__init__.py
+-rwxr-xr-x   0 dds      (197609) None     (197121)     5108 2023-05-09 07:40:14.000000 taru-1.0.0/taru/cli.py
+drwxr-xr-x   0 dds      (197609) None     (197121)        0 2023-05-09 07:41:29.287912 taru-1.0.0/taru.egg-info/
+-rw-r--r--   0 dds      (197609) None     (197121)     1069 2023-05-09 07:41:29.000000 taru-1.0.0/taru.egg-info/PKG-INFO
+-rw-r--r--   0 dds      (197609) None     (197121)      245 2023-05-09 07:41:29.000000 taru-1.0.0/taru.egg-info/SOURCES.txt
+-rw-r--r--   0 dds      (197609) None     (197121)        1 2023-05-09 07:41:29.000000 taru-1.0.0/taru.egg-info/dependency_links.txt
+-rw-r--r--   0 dds      (197609) None     (197121)       39 2023-05-09 07:41:29.000000 taru-1.0.0/taru.egg-info/entry_points.txt
+-rw-r--r--   0 dds      (197609) None     (197121)        1 2021-07-25 11:11:54.000000 taru-1.0.0/taru.egg-info/not-zip-safe
+-rw-r--r--   0 dds      (197609) None     (197121)        5 2023-05-09 07:41:29.000000 taru-1.0.0/taru.egg-info/top_level.txt
+drwxr-xr-x   0 dds      (197609) None     (197121)        0 2023-05-09 07:41:29.289907 taru-1.0.0/tests/
+-rw-r--r--   0 dds      (197609) None     (197121)     3197 2021-07-25 17:14:15.000000 taru-1.0.0/tests/test_cli.py
```

### Comparing `taru-0.1.3/PKG-INFO` & `taru-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: taru
-Version: 0.1.3
+Version: 1.0.0
 Summary: Taru processes a tar listing to display the cumulative size of files stored in individual directories.
 Home-page: https://github.com/dspinellis/taru
 Author: Diomidis Spinellis
 Author-email: dds@aueb.gr
 License: Apache Software License
 Keywords: tar,du,size
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
@@ -21,9 +21,7 @@
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: Utilities
 
 
 Taru is a Unix command-line tool that processes a tar(1) listing to display
 the cumulative size of files stored in individual directories.
 Its output and options are similar to the Unix disk usage command du(1).
-
-
```

### Comparing `taru-0.1.3/README.md` & `taru-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `taru-0.1.3/setup.py` & `taru-1.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 from setuptools import find_packages, setup
 
 dependencies = []
 
 setup(
     name='taru',
-    version='0.1.3',
+    version='1.0.0',
     url='https://github.com/dspinellis/taru',
     license='Apache Software License',
     author='Diomidis Spinellis',
     author_email='dds@aueb.gr',
     keywords='tar, du, size',
     description='Taru processes a tar listing to display the cumulative size of files stored in individual directories.',
     long_description=__doc__,
@@ -28,16 +28,16 @@
         ],
     },
     classifiers=[
         # As from http://pypi.python.org/pypi?%3Aaction=list_classifiers
         # 'Development Status :: 1 - Planning',
         # 'Development Status :: 2 - Pre-Alpha',
         # 'Development Status :: 3 - Alpha',
-        'Development Status :: 4 - Beta',
-        # 'Development Status :: 5 - Production/Stable',
+        # 'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         # 'Development Status :: 6 - Mature',
         # 'Development Status :: 7 - Inactive',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: POSIX',
         'Operating System :: MacOS',
```

### Comparing `taru-0.1.3/taru/cli.py` & `taru-1.0.0/taru/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 #
-# Copyright 2021 Diomidis Spinellis
+# Copyright 2021-2023 Diomidis Spinellis
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -19,15 +19,17 @@
 List the size of directories in a tar file
 """
 
 import argparse
 import re
 import sys
 
-TAR_LINE = re.compile(r'.{10}\s+\w+/\w+\s+(\d+) \d{4}-\d\d-\d\d \d\d:\d\d (.*)')
+TAR_LINE = re.compile(
+    r'.{10}\s+[^/]+/[^\s]+\s+(\d+) \d{4}-\d\d-\d\d \d\d:\d\d (.*)'
+)
 
 
 def humanize(num, power):
     """Return the number in units of power with the corresponding suffix"""
     num = int(num)
     if num < power:
         return f'{num}B'
```

### Comparing `taru-0.1.3/taru.egg-info/PKG-INFO` & `taru-1.0.0/taru.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: taru
-Version: 0.1.3
+Version: 1.0.0
 Summary: Taru processes a tar listing to display the cumulative size of files stored in individual directories.
 Home-page: https://github.com/dspinellis/taru
 Author: Diomidis Spinellis
 Author-email: dds@aueb.gr
 License: Apache Software License
 Keywords: tar,du,size
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
@@ -21,9 +21,7 @@
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: Utilities
 
 
 Taru is a Unix command-line tool that processes a tar(1) listing to display
 the cumulative size of files stored in individual directories.
 Its output and options are similar to the Unix disk usage command du(1).
-
-
```

